# Comparing `tmp/edgaro-1.0.1.1.tar.gz` & `tmp/edgaro-1.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgaro-1.0.1.1.tar", last modified: Thu Mar 23 14:50:03 2023, max compression
+gzip compressed data, was "edgaro-1.0.1.2.tar", last modified: Fri Jun  2 11:07:35 2023, max compression
```

## Comparing `edgaro-1.0.1.1.tar` & `edgaro-1.0.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:50:03.599177 edgaro-1.0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-03-23 14:50:03.595177 edgaro-1.0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:50:03.591177 edgaro-1.0.1.1/edgaro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:50:03.595177 edgaro-1.0.1.1/edgaro/balancing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/balancing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/balancing/nested_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/balancing/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/balancing/transformer_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:50:03.595177 edgaro-1.0.1.1/edgaro/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/base/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/base/base_transformer_array.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:50:03.595177 edgaro-1.0.1.1/edgaro/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16032 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21672 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/data/dataset_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:50:03.595177 edgaro-1.0.1.1/edgaro/explain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/explain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/explain/explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/explain/explainer_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    23271 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/explain/explainer_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    27137 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/explain/explainer_result_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:50:03.595177 edgaro-1.0.1.1/edgaro/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25616 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/edgaro/model/model_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:50:03.595177 edgaro-1.0.1.1/edgaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-03-23 14:50:03.000000 edgaro-1.0.1.1/edgaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-23 14:50:03.000000 edgaro-1.0.1.1/edgaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:50:03.000000 edgaro-1.0.1.1/edgaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-23 14:50:03.000000 edgaro-1.0.1.1/edgaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-23 14:50:03.000000 edgaro-1.0.1.1/edgaro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 14:50:03.599177 edgaro-1.0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:50:03.595177 edgaro-1.0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/test/test_balancing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/test/test_balancing_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/test/test_balancing_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/test/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/test/test_dataset_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/test/test_explain.py
--rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-03-23 14:49:55.000000 edgaro-1.0.1.1/test/test_model_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.747987 edgaro-1.0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-02 11:07:35.747987 edgaro-1.0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.739987 edgaro-1.0.1.2/edgaro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.739987 edgaro-1.0.1.2/edgaro/balancing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/balancing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/balancing/nested_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/balancing/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/balancing/transformer_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.739987 edgaro-1.0.1.2/edgaro/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/base/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/base/base_transformer_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.743987 edgaro-1.0.1.2/edgaro/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21672 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/data/dataset_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.743987 edgaro-1.0.1.2/edgaro/explain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/explain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/explain/explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/explain/explainer_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23271 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/explain/explainer_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27137 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/explain/explainer_result_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.743987 edgaro-1.0.1.2/edgaro/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25616 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/edgaro/model/model_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.739987 edgaro-1.0.1.2/edgaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-02 11:07:35.000000 edgaro-1.0.1.2/edgaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-02 11:07:35.000000 edgaro-1.0.1.2/edgaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:07:35.000000 edgaro-1.0.1.2/edgaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 11:07:35.000000 edgaro-1.0.1.2/edgaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 11:07:35.000000 edgaro-1.0.1.2/edgaro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:07:35.747987 edgaro-1.0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:35.747987 edgaro-1.0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_balancing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_balancing_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_balancing_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_dataset_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-02 11:07:22.000000 edgaro-1.0.1.2/test/test_model_array.py
```

### Comparing `edgaro-1.0.1.1/LICENSE` & `edgaro-1.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/PKG-INFO` & `edgaro-1.0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgaro
-Version: 1.0.1.1
+Version: 1.0.1.2
 Summary: Explainable imbalanceD learninG compARatOr
 Home-page: https://github.com/adrianstando/edgaro
 Author: Adrian Stańdo
 Author-email: adrian.j.stando@gmail.com
 Project-URL: Documentation, https://adrianstando.github.io/edgaro
 Project-URL: Code repository, https://github.com/adrianstando/edgaro
 Keywords: XAI,imbalance,machine learning,AI
```

### Comparing `edgaro-1.0.1.1/README.md` & `edgaro-1.0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/edgaro/balancing/nested_transformer.py` & `edgaro-1.0.1.2/edgaro/balancing/nested_transformer.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/edgaro/balancing/transformer.py` & `edgaro-1.0.1.2/edgaro/balancing/transformer.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/edgaro/balancing/transformer_array.py` & `edgaro-1.0.1.2/edgaro/balancing/transformer_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/edgaro/base/base_transformer.py` & `edgaro-1.0.1.2/edgaro/base/base_transformer.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/edgaro/base/base_transformer_array.py` & `edgaro-1.0.1.2/edgaro/base/base_transformer_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/edgaro/data/dataset.py` & `edgaro-1.0.1.2/edgaro/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,17 +221,23 @@
             profile.to_notebook_iframe()
 
     @property
     def imbalance_ratio(self) -> float:
         """
         float : Imbalance Ratio of the Dataset; is the ratio of the majority class to the minority class
         """
-        if self.target is None:
+        if self.was_split:
+            y = self.train.target
+        else:
+            y = self.target
+
+        if y is None:
             return float(0)
-        names, counts = np.unique(self.target, return_counts=True)
+
+        names, counts = np.unique(y, return_counts=True)
         if len(names) == 1:
             return float(0)
         elif len(names) > 2:
             raise Exception('Target has too many classes for binary classification!')
         else:
             return float(max(counts) / min(counts))
```

### Comparing `edgaro-1.0.1.1/edgaro/data/dataset_array.py` & `edgaro-1.0.1.2/edgaro/data/dataset_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/edgaro/explain/explainer.py` & `edgaro-1.0.1.2/edgaro/explain/explainer.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/edgaro/explain/explainer_array.py` & `edgaro-1.0.1.2/edgaro/explain/explainer_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/edgaro/explain/explainer_result.py` & `edgaro-1.0.1.2/edgaro/explain/explainer_result.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/edgaro/explain/explainer_result_array.py` & `edgaro-1.0.1.2/edgaro/explain/explainer_result_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/edgaro/model/model.py` & `edgaro-1.0.1.2/edgaro/model/model.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/edgaro/model/model_array.py` & `edgaro-1.0.1.2/edgaro/model/model_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/edgaro.egg-info/PKG-INFO` & `edgaro-1.0.1.2/edgaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgaro
-Version: 1.0.1.1
+Version: 1.0.1.2
 Summary: Explainable imbalanceD learninG compARatOr
 Home-page: https://github.com/adrianstando/edgaro
 Author: Adrian Stańdo
 Author-email: adrian.j.stando@gmail.com
 Project-URL: Documentation, https://adrianstando.github.io/edgaro
 Project-URL: Code repository, https://github.com/adrianstando/edgaro
 Keywords: XAI,imbalance,machine learning,AI
```

### Comparing `edgaro-1.0.1.1/edgaro.egg-info/SOURCES.txt` & `edgaro-1.0.1.2/edgaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/setup.py` & `edgaro-1.0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="edgaro",
-    version="1.0.1.1",
+    version="1.0.1.2",
     description="Explainable imbalanceD learninG compARatOr",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/adrianstando/edgaro",
     author="Adrian Stańdo",
     author_email="adrian.j.stando@gmail.com",
     classifiers=[
```

### Comparing `edgaro-1.0.1.1/test/test_balancing.py` & `edgaro-1.0.1.2/test/test_balancing.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/test/test_balancing_array.py` & `edgaro-1.0.1.2/test/test_balancing_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/test/test_balancing_nested.py` & `edgaro-1.0.1.2/test/test_balancing_nested.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/test/test_dataset.py` & `edgaro-1.0.1.2/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/test/test_dataset_array.py` & `edgaro-1.0.1.2/test/test_dataset_array.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/test/test_explain.py` & `edgaro-1.0.1.2/test/test_explain.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/test/test_model.py` & `edgaro-1.0.1.2/test/test_model.py`

 * *Files identical despite different names*

### Comparing `edgaro-1.0.1.1/test/test_model_array.py` & `edgaro-1.0.1.2/test/test_model_array.py`

 * *Files identical despite different names*

