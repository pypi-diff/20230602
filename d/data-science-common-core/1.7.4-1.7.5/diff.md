# Comparing `tmp/data_science_common_core-1.7.4.tar.gz` & `tmp/data-science-common-core-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_science_common_core-1.7.4.tar", max compression
+gzip compressed data, was "data-science-common-core-1.7.5.tar", max compression
```

## Comparing `data_science_common_core-1.7.4.tar` & `data-science-common-core-1.7.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       31 2022-11-28 14:04:39.888572 data_science_common_core-1.7.4/common/__init__.py
--rw-r--r--   0        0        0     1772 2023-01-17 16:07:12.581941 data_science_common_core-1.7.4/common/catrf.py
--rw-r--r--   0        0        0     2239 2023-02-28 09:59:05.828156 data_science_common_core-1.7.4/common/constants.py
--rw-r--r--   0        0        0    28618 2022-11-28 14:04:39.888964 data_science_common_core-1.7.4/common/custom_hgb.py
--rw-r--r--   0        0        0    14915 2022-11-28 14:04:39.889163 data_science_common_core-1.7.4/common/custom_multi.py
--rw-r--r--   0        0        0    17580 2022-11-28 14:04:39.889365 data_science_common_core-1.7.4/common/ft.py
--rw-r--r--   0        0        0    12414 2023-02-24 16:00:22.756007 data_science_common_core-1.7.4/common/io.py
--rw-r--r--   0        0        0    23926 2022-11-28 14:04:39.889798 data_science_common_core-1.7.4/common/logic.py
--rw-r--r--   0        0        0    15836 2023-01-17 16:07:12.582499 data_science_common_core-1.7.4/common/model.py
--rw-r--r--   0        0        0     1013 2023-01-17 16:07:12.582596 data_science_common_core-1.7.4/common/pipeline.py
--rw-r--r--   0        0        0    11465 2023-02-24 16:00:22.756911 data_science_common_core-1.7.4/common/plot.py
--rw-r--r--   0        0        0     2100 2022-11-28 14:04:39.890367 data_science_common_core-1.7.4/common/query.py
--rw-r--r--   0        0        0     6947 2023-01-17 16:07:12.582751 data_science_common_core-1.7.4/common/setup.py
--rw-r--r--   0        0        0     2639 2023-01-17 16:07:12.582836 data_science_common_core-1.7.4/common/transformer.py
--rw-r--r--   0        0        0     8736 2022-11-28 14:04:39.890677 data_science_common_core-1.7.4/common/utils.py
--rw-r--r--   0        0        0     1089 2023-02-28 10:22:38.907231 data_science_common_core-1.7.4/pyproject.toml
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 data_science_common_core-1.7.4/setup.py
--rw-r--r--   0        0        0     1479 1970-01-01 00:00:00.000000 data_science_common_core-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0       31 2022-08-16 12:51:34.846327 data-science-common-core-1.7.5/common/__init__.py
+-rw-r--r--   0        0        0     1772 2023-01-04 09:26:13.978265 data-science-common-core-1.7.5/common/catrf.py
+-rw-r--r--   0        0        0     2239 2023-06-02 13:30:43.079798 data-science-common-core-1.7.5/common/constants.py
+-rw-r--r--   0        0        0    28618 2022-09-16 13:05:55.366098 data-science-common-core-1.7.5/common/custom_hgb.py
+-rw-r--r--   0        0        0    14915 2022-10-06 09:48:34.061975 data-science-common-core-1.7.5/common/custom_multi.py
+-rw-r--r--   0        0        0    17492 2023-06-02 13:33:52.153362 data-science-common-core-1.7.5/common/ft.py
+-rw-r--r--   0        0        0    12414 2023-06-02 13:30:43.079972 data-science-common-core-1.7.5/common/io.py
+-rw-r--r--   0        0        0    23926 2022-11-18 13:02:14.591758 data-science-common-core-1.7.5/common/logic.py
+-rw-r--r--   0        0        0    15836 2023-01-04 09:26:13.980885 data-science-common-core-1.7.5/common/model.py
+-rw-r--r--   0        0        0     1013 2023-06-02 13:30:43.080198 data-science-common-core-1.7.5/common/pipeline.py
+-rw-r--r--   0        0        0    11465 2023-06-02 13:30:43.082632 data-science-common-core-1.7.5/common/plot.py
+-rw-r--r--   0        0        0     2100 2022-09-08 15:24:02.191811 data-science-common-core-1.7.5/common/query.py
+-rw-r--r--   0        0        0     6947 2023-01-04 09:26:13.981645 data-science-common-core-1.7.5/common/setup.py
+-rw-r--r--   0        0        0     2639 2023-06-02 13:30:43.082938 data-science-common-core-1.7.5/common/transformer.py
+-rw-r--r--   0        0        0     8736 2022-11-25 15:53:01.257516 data-science-common-core-1.7.5/common/utils.py
+-rw-r--r--   0        0        0     1089 2023-06-02 13:53:26.121282 data-science-common-core-1.7.5/pyproject.toml
+-rw-r--r--   0        0        0     1343 2023-06-02 14:00:02.818002 data-science-common-core-1.7.5/setup.py
+-rw-r--r--   0        0        0     1479 2023-06-02 14:00:02.818182 data-science-common-core-1.7.5/PKG-INFO
```

### Comparing `data_science_common_core-1.7.4/common/catrf.py` & `data-science-common-core-1.7.5/common/catrf.py`

 * *Files identical despite different names*

### Comparing `data_science_common_core-1.7.4/common/constants.py` & `data-science-common-core-1.7.5/common/constants.py`

 * *Files identical despite different names*

### Comparing `data_science_common_core-1.7.4/common/custom_hgb.py` & `data-science-common-core-1.7.5/common/custom_hgb.py`

 * *Files identical despite different names*

### Comparing `data_science_common_core-1.7.4/common/custom_multi.py` & `data-science-common-core-1.7.5/common/custom_multi.py`

 * *Files identical despite different names*

### Comparing `data_science_common_core-1.7.4/common/ft.py` & `data-science-common-core-1.7.5/common/ft.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,16 +217,15 @@
 
         # Label Encoding for LDA
         if params["prediction_type"] == "classification":
             oe = OrdinalEncoder()
             label_enc = label.astype(int).astype(str).values.sum(axis=1)
             label_enc = oe.fit_transform(label_enc.reshape(-1, 1)).flatten()
         else:
-            bins = np.histogram(label, params["regression_bins"])[1]
-            label_enc = np.digitize(label, bins)
+            label_enc = label
 
         df_wanted = df.loc[:, self.col_names]
         res = apply_function(self._fit_one_column, params, df_wanted, label_enc, axis=1)
         self.enc = [i[0] for i in res]
         self.dim_red = [i[1] for i in res]
 
         return self
```

### Comparing `data_science_common_core-1.7.4/common/io.py` & `data-science-common-core-1.7.5/common/io.py`

 * *Files identical despite different names*

### Comparing `data_science_common_core-1.7.4/common/logic.py` & `data-science-common-core-1.7.5/common/logic.py`

 * *Files identical despite different names*

### Comparing `data_science_common_core-1.7.4/common/model.py` & `data-science-common-core-1.7.5/common/model.py`

 * *Files identical despite different names*

### Comparing `data_science_common_core-1.7.4/common/pipeline.py` & `data-science-common-core-1.7.5/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `data_science_common_core-1.7.4/common/plot.py` & `data-science-common-core-1.7.5/common/plot.py`

 * *Files identical despite different names*

### Comparing `data_science_common_core-1.7.4/common/query.py` & `data-science-common-core-1.7.5/common/query.py`

 * *Files identical despite different names*

### Comparing `data_science_common_core-1.7.4/common/setup.py` & `data-science-common-core-1.7.5/common/setup.py`

 * *Files identical despite different names*

### Comparing `data_science_common_core-1.7.4/common/transformer.py` & `data-science-common-core-1.7.5/common/transformer.py`

 * *Files identical despite different names*

### Comparing `data_science_common_core-1.7.4/common/utils.py` & `data-science-common-core-1.7.5/common/utils.py`

 * *Files identical despite different names*

### Comparing `data_science_common_core-1.7.4/pyproject.toml` & `data-science-common-core-1.7.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-science-common-core"
-version = "1.7.4"
+version = "1.7.5"
 description = "Data Science Common Core"
 authors = ["Unsal Gokdag <unsal.gokdag@forto.com>", "PietroAnsidei <pietro.ansidei@forto.com>", "Naomi Nguyen <naomi.nguyen@forto.com>", "Kumar Rajendrababu <kumar.rajendrababu@forto.com>"]
 packages = [
     { include = "common/*.py"},
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `data_science_common_core-1.7.4/PKG-INFO` & `data-science-common-core-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: data-science-common-core
-Version: 1.7.4
+Version: 1.7.5
 Summary: Data Science Common Core
 Author: Unsal Gokdag
 Author-email: unsal.gokdag@forto.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: catboost (>=1.0.6,<2.0.0)
 Requires-Dist: db-dtypes (>=1.0.2,<2.0.0)
 Requires-Dist: google-cloud-bigquery (>=3.2.0,<4.0.0)
 Requires-Dist: google-cloud-bigquery-storage (>=2.14.1,<3.0.0)
 Requires-Dist: google-cloud-storage (>=2.4.0,<3.0.0)
 Requires-Dist: grpcio (==1.51.1)
 Requires-Dist: gspread (>=5.4.0,<6.0.0)
```

