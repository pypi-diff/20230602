# Comparing `tmp/dq_module-1.1.1.tar.gz` & `tmp/dq_module-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dq_module-1.1.1.tar", last modified: Wed Mar 15 08:15:42 2023, max compression
+gzip compressed data, was "dist/dq_module-1.1.2.tar", last modified: Fri Jun  2 06:29:47 2023, max compression
```

## Comparing `dq_module-1.1.1.tar` & `dq_module-1.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:15:42.000000 dq_module-1.1.1/
--rw-r--r--   0 root         (0) root         (0)    13216 2023-03-15 08:15:42.000000 dq_module-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11346 2023-03-15 08:15:31.000000 dq_module-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:15:42.000000 dq_module-1.1.1/dataqualitycheck/
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-03-15 08:15:31.000000 dq_module-1.1.1/dataqualitycheck/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11938 2023-03-15 08:15:31.000000 dq_module-1.1.1/dataqualitycheck/commonutilities.py
--rw-rw-rw-   0 root         (0) root         (0)    10482 2023-03-15 08:15:31.000000 dq_module-1.1.1/dataqualitycheck/consistencycheck.py
--rw-rw-rw-   0 root         (0) root         (0)    37756 2023-03-15 08:15:31.000000 dq_module-1.1.1/dataqualitycheck/dataprofile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:15:42.000000 dq_module-1.1.1/dataqualitycheck/datasources/
--rw-rw-rw-   0 root         (0) root         (0)     7917 2023-03-15 08:15:31.000000 dq_module-1.1.1/dataqualitycheck/datasources/azureblobdf.py
--rw-rw-rw-   0 root         (0) root         (0)     2836 2023-03-15 08:15:31.000000 dq_module-1.1.1/dataqualitycheck/datasources/commonutilities.py
--rw-rw-rw-   0 root         (0) root         (0)     5534 2023-03-15 08:15:31.000000 dq_module-1.1.1/dataqualitycheck/datasources/databricksfilesystemdf.py
--rw-rw-rw-   0 root         (0) root         (0)     3539 2023-03-15 08:15:31.000000 dq_module-1.1.1/dataqualitycheck/datasources/databrickssqldf.py
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-03-15 08:15:31.000000 dq_module-1.1.1/dataqualitycheck/datasources/localfilesystemdf.py
--rw-rw-rw-   0 root         (0) root         (0)     5366 2023-03-15 08:15:31.000000 dq_module-1.1.1/dataqualitycheck/enumfile.py
--rw-rw-rw-   0 root         (0) root         (0)     1166 2023-03-15 08:15:31.000000 dq_module-1.1.1/dataqualitycheck/singledatasetqualitycheck.py
--rw-rw-rw-   0 root         (0) root         (0)    40659 2023-03-15 08:15:31.000000 dq_module-1.1.1/dataqualitycheck/singledatasetqualitycheckpolars.py
--rw-rw-rw-   0 root         (0) root         (0)    37038 2023-03-15 08:15:31.000000 dq_module-1.1.1/dataqualitycheck/singledatasetqualitycheckspark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 08:15:42.000000 dq_module-1.1.1/dq_module.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13216 2023-03-15 08:15:42.000000 dq_module-1.1.1/dq_module.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      739 2023-03-15 08:15:42.000000 dq_module-1.1.1/dq_module.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 08:15:42.000000 dq_module-1.1.1/dq_module.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-15 08:15:42.000000 dq_module-1.1.1/dq_module.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-03-15 08:15:42.000000 dq_module-1.1.1/dq_module.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-15 08:15:42.000000 dq_module-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-03-15 08:15:31.000000 dq_module-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:29:47.000000 dq_module-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)    13216 2023-06-02 06:29:47.000000 dq_module-1.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11346 2023-06-02 06:29:32.000000 dq_module-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:29:47.000000 dq_module-1.1.2/dataqualitycheck/
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11938 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/commonutilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    10482 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/consistencycheck.py
+-rw-rw-rw-   0 root         (0) root         (0)    37781 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/dataprofile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:29:47.000000 dq_module-1.1.2/dataqualitycheck/datasources/
+-rw-rw-rw-   0 root         (0) root         (0)     7917 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/datasources/azureblobdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/datasources/commonutilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     5534 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/datasources/databricksfilesystemdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3539 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/datasources/databrickssqldf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/datasources/localfilesystemdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5366 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/enumfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/singledatasetqualitycheck.py
+-rw-rw-rw-   0 root         (0) root         (0)    40659 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/singledatasetqualitycheckpolars.py
+-rw-rw-rw-   0 root         (0) root         (0)    37038 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/singledatasetqualitycheckspark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:29:47.000000 dq_module-1.1.2/dq_module.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13216 2023-06-02 06:29:47.000000 dq_module-1.1.2/dq_module.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      739 2023-06-02 06:29:47.000000 dq_module-1.1.2/dq_module.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 06:29:47.000000 dq_module-1.1.2/dq_module.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-02 06:29:47.000000 dq_module-1.1.2/dq_module.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-02 06:29:47.000000 dq_module-1.1.2/dq_module.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 06:29:47.000000 dq_module-1.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-06-02 06:29:32.000000 dq_module-1.1.2/setup.py
```

### Comparing `dq_module-1.1.1/PKG-INFO` & `dq_module-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_module
-Version: 1.1.1
+Version: 1.1.2
 Summary: data profiling and basic data quality rules check
 Home-page: UNKNOWN
 Author: Sweta
 Author-email: sweta.swami@decisionpoint.in
 License: UNKNOWN
 Description: ### dq-module
         dq-module is a tool which can be used to perform validations and profiling on the datasets.This tool is compatible with two run_engines `pyspark` and `polars`.
```

### Comparing `dq_module-1.1.1/README.md` & `dq_module-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.1/dataqualitycheck/commonutilities.py` & `dq_module-1.1.2/dataqualitycheck/commonutilities.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.1/dataqualitycheck/consistencycheck.py` & `dq_module-1.1.2/dataqualitycheck/consistencycheck.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.1/dataqualitycheck/dataprofile.py` & `dq_module-1.1.2/dataqualitycheck/dataprofile.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,16 +243,16 @@
             )
         return result_data
 
     def find_mode_spark(self, df, column_to_be_checked):
         df = df.filter(col(column_to_be_checked).isNotNull()
                        ).groupBy(column_to_be_checked).count()
         mode_val_count = df.agg(max("count")).take(1)[0][0]
-        result = df.filter(col("count") == mode_val_count).select(
-            column_to_be_checked).rdd.flatMap(lambda x: x).collect()
+        result = df.filter(col("count") == mode_val_count).select(column_to_be_checked).collect()
+        result = [row[column_to_be_checked] for row in result]
         return str(result)
 
     def find_mode_polars(self, df, column_to_be_checked):
         df = df.filter(pl.col(column_to_be_checked).is_not_null()).groupby(
             column_to_be_checked, maintain_order=True).count()
         mode_val_count = df.select(pl.col("count").max()).item()
         result = df.filter(pl.col("count") == mode_val_count).select(
```

### Comparing `dq_module-1.1.1/dataqualitycheck/datasources/azureblobdf.py` & `dq_module-1.1.2/dataqualitycheck/datasources/azureblobdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.1/dataqualitycheck/datasources/commonutilities.py` & `dq_module-1.1.2/dataqualitycheck/datasources/commonutilities.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.1/dataqualitycheck/datasources/databricksfilesystemdf.py` & `dq_module-1.1.2/dataqualitycheck/datasources/databricksfilesystemdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.1/dataqualitycheck/datasources/databrickssqldf.py` & `dq_module-1.1.2/dataqualitycheck/datasources/databrickssqldf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.1/dataqualitycheck/datasources/localfilesystemdf.py` & `dq_module-1.1.2/dataqualitycheck/datasources/localfilesystemdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.1/dataqualitycheck/enumfile.py` & `dq_module-1.1.2/dataqualitycheck/enumfile.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.1/dataqualitycheck/singledatasetqualitycheck.py` & `dq_module-1.1.2/dataqualitycheck/singledatasetqualitycheck.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.1/dataqualitycheck/singledatasetqualitycheckpolars.py` & `dq_module-1.1.2/dataqualitycheck/singledatasetqualitycheckpolars.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.1/dataqualitycheck/singledatasetqualitycheckspark.py` & `dq_module-1.1.2/dataqualitycheck/singledatasetqualitycheckspark.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.1/dq_module.egg-info/PKG-INFO` & `dq_module-1.1.2/dq_module.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq-module
-Version: 1.1.1
+Version: 1.1.2
 Summary: data profiling and basic data quality rules check
 Home-page: UNKNOWN
 Author: Sweta
 Author-email: sweta.swami@decisionpoint.in
 License: UNKNOWN
 Description: ### dq-module
         dq-module is a tool which can be used to perform validations and profiling on the datasets.This tool is compatible with two run_engines `pyspark` and `polars`.
```

### Comparing `dq_module-1.1.1/dq_module.egg-info/SOURCES.txt` & `dq_module-1.1.2/dq_module.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.1/setup.py` & `dq_module-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # COMMAND ----------
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read() 
     
 setuptools.setup(
     name="dq_module",
-    version="1.1.1",
+    version="1.1.2",
     author="Sweta",
     author_email="sweta.swami@decisionpoint.in",
     description="data profiling and basic data quality rules check",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # packages=setuptools.find_packages(include=['*']),
     packages=['dataqualitycheck', 'dataqualitycheck.datasources'],
```

