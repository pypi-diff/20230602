# Comparing `tmp/protloc_mex_x-0.0.3.tar.gz` & `tmp/protloc_mex_x-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protloc_mex_x-0.0.3.tar", max compression
+gzip compressed data, was "protloc_mex_x-0.0.4.tar", max compression
```

## Comparing `protloc_mex_x-0.0.3.tar` & `protloc_mex_x-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1091 2023-04-25 08:38:35.586641 protloc_mex_x-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0        2 2023-05-09 03:41:02.000000 protloc_mex_x-0.0.3/protloc_mex_X/__init__.py
--rw-r--r--   0        0        0    36861 2023-05-31 10:09:36.000000 protloc_mex_x-0.0.3/protloc_mex_X/ESM2_fr.py
--rw-r--r--   0        0        0     2999 2023-05-08 12:33:04.000000 protloc_mex_x-0.0.3/protloc_mex_X/examples/test1.txt
--rw-r--r--   0        0        0     2749 2023-05-09 03:13:02.000000 protloc_mex_x-0.0.3/protloc_mex_X/feature_corrlation.py
--rw-r--r--   0        0        0      863 2023-05-31 13:10:53.302882 protloc_mex_x-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-10 08:06:08.458858 protloc_mex_x-0.0.3/README.md
--rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 protloc_mex_x-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-25 08:38:35.586641 protloc_mex_x-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0        2 2023-05-09 03:41:02.000000 protloc_mex_x-0.0.4/protloc_mex_X/__init__.py
+-rw-r--r--   0        0        0    39068 2023-06-01 11:45:18.000000 protloc_mex_x-0.0.4/protloc_mex_X/ESM2_fr.py
+-rw-r--r--   0        0        0     2999 2023-05-08 12:33:04.000000 protloc_mex_x-0.0.4/protloc_mex_X/examples/test1.txt
+-rw-r--r--   0        0        0     2749 2023-05-09 03:13:02.000000 protloc_mex_x-0.0.4/protloc_mex_X/feature_corrlation.py
+-rw-r--r--   0        0        0      863 2023-06-02 07:08:20.652284 protloc_mex_x-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-10 08:06:08.458858 protloc_mex_x-0.0.4/README.md
+-rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 protloc_mex_x-0.0.4/PKG-INFO
```

### Comparing `protloc_mex_x-0.0.3/LICENSE.txt` & `protloc_mex_x-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.3/protloc_mex_X/ESM2_fr.py` & `protloc_mex_x-0.0.4/protloc_mex_X/ESM2_fr.py`

 * *Files 4% similar despite different names*

```diff
@@ -425,14 +425,66 @@
     # for i in range(dim):
     #     df_cls[f'average{i}'] = df_cls[f'average{i}'].fillna(0)
     if df_cls.isnull().any().any():
         df_cls = df_cls.fillna(0)
         
     return df_cls
 
+
+def phospho_feature_sim_cosine_weighted_average_test(dim, df_cls, df_phospho):
+    """
+    This function computes the overall phospho-representation for a single amino acid sequence 
+    using a cosine similarity-based weighting scheme. It merges the given dataframes on their 
+    index (protein_id), calculates the cosine similarity for each row, and then calculates the 
+    total weights for each protein. It then computes the sum of weighted features for each protein 
+    and returns this sum.
+    
+    Note: This function is designed to work with one amino acid sequence at a time.
+    
+    Parameters:
+    dim (int): The dimensionality of the feature vectors.
+    df_cls (DataFrame): The cls feature DataFrame.
+    df_phospho (DataFrame): The phospho feature DataFrame.
+    
+    Returns:
+    Series: The sum of the weighted features.
+    """
+    # Merge df_cls and df_phospho on index (protein_id)
+    df = pd.merge(df_cls, df_phospho, how='inner', left_index=True, right_index=True)
+    
+    # Calculate cosine similarity for each row in the merged dataframe
+    similarity = np.sum(df_cls.to_numpy() * df_phospho.to_numpy(), axis=1) / (np.linalg.norm(df_cls.to_numpy(), axis=1) * np.linalg.norm(df_phospho.to_numpy(), axis=1))
+    
+    # Add the similarity to the DataFrame
+    df['similarity'] = similarity
+    
+    # Calculate total weights (sum of abs similarities) for each protein
+    total_weights = df['similarity'].abs().groupby(df.index).sum()
+    
+    # Calculate sum of weighted features for each protein
+    weighted_features = df_phospho.copy()
+    weighted_features.columns = [f'weighted{i}' for i in range(dim)]
+    
+    # Calculate the weight for each row
+    df['weight'] = df['similarity'] / total_weights
+    
+    # Repeat the weights to the same dimension as the features
+    weights_matrix = np.repeat(df['weight'].values[:, np.newaxis], dim, axis=1)
+    
+    # Multiply each row of features by its weight
+    average_total = weighted_features.multiply(weights_matrix, axis=0)
+    
+    # Calculate the sum of the weighted features
+    average_total_final = average_total.sum(axis=0)
+    
+    return average_total_final
+
+
+
+
 ###后面都是legacy，可用于检验模型是否正确或无用的代码即不在完整工作流中运行，但不允许删除。
 
 class Esm2LastHiddenFeatureExtractor_legacy:
     def __init__(self, tokenizer, model, compute_cls=True, compute_eos=True, compute_mean=True, compute_segments=False):
         self.tokenizer = tokenizer
         self.model = model
         self.compute_cls = compute_cls
```

### Comparing `protloc_mex_x-0.0.3/protloc_mex_X/examples/test1.txt` & `protloc_mex_x-0.0.4/protloc_mex_X/examples/test1.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.3/protloc_mex_X/feature_corrlation.py` & `protloc_mex_x-0.0.4/protloc_mex_X/feature_corrlation.py`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.3/pyproject.toml` & `protloc_mex_x-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "protloc_mex_X"
-version = "0.0.3"
+version = "0.0.4"
 description = "Internal use kit"
 authors = ["Ze Yu Luo <1024226968@qq.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/yujuan-zhang/ProtLoc-mexl"
 repository = "https://github.com/yujuan-zhang/ProtLoc-mexl"
 documentation = "https://github.com/yujuan-zhang/ProtLoc-mexl/issues"
```

### Comparing `protloc_mex_x-0.0.3/PKG-INFO` & `protloc_mex_x-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protloc-mex-x
-Version: 0.0.3
+Version: 0.0.4
 Summary: Internal use kit
 Home-page: https://github.com/yujuan-zhang/ProtLoc-mexl
 License: MIT
 Author: Ze Yu Luo
 Author-email: 1024226968@qq.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
```

