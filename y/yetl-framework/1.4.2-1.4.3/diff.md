# Comparing `tmp/yetl-framework-1.4.2.tar.gz` & `tmp/yetl-framework-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.4.2.tar", last modified: Thu Jun  1 23:39:55 2023, max compression
+gzip compressed data, was "yetl-framework-1.4.3.tar", last modified: Fri Jun  2 00:40:16 2023, max compression
```

## Comparing `yetl-framework-1.4.2.tar` & `yetl-framework-1.4.3.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 23:39:55.697751 yetl-framework-1.4.2/
--rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-01 23:39:55.697751 yetl-framework-1.4.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-01 23:39:55.697751 yetl-framework-1.4.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 23:39:55.693751 yetl-framework-1.4.2/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 23:39:55.693751 yetl-framework-1.4.2/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 23:39:55.697751 yetl-framework-1.4.2/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3023 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8764 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 23:39:55.697751 yetl-framework-1.4.2/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3790 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4049 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 23:39:55.697751 yetl-framework-1.4.2/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-01 23:39:02.000000 yetl-framework-1.4.2/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 23:39:55.697751 yetl-framework-1.4.2/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-01 23:39:55.000000 yetl-framework-1.4.2/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      902 2023-06-01 23:39:55.000000 yetl-framework-1.4.2/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-01 23:39:55.000000 yetl-framework-1.4.2/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-01 23:39:55.000000 yetl-framework-1.4.2/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       29 2023-06-01 23:39:55.000000 yetl-framework-1.4.2/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-06-01 23:39:55.000000 yetl-framework-1.4.2/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.474318 yetl-framework-1.4.3/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-02 00:40:16.474318 yetl-framework-1.4.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-02 00:40:16.474318 yetl-framework-1.4.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1150 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.470318 yetl-framework-1.4.3/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.470318 yetl-framework-1.4.3/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.470318 yetl-framework-1.4.3/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15345 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.474318 yetl-framework-1.4.3/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3023 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8764 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.474318 yetl-framework-1.4.3/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3790 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4049 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.474318 yetl-framework-1.4.3/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.474318 yetl-framework-1.4.3/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-02 00:40:16.000000 yetl-framework-1.4.3/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      977 2023-06-02 00:40:16.000000 yetl-framework-1.4.3/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-02 00:40:16.000000 yetl-framework-1.4.3/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-02 00:40:16.000000 yetl-framework-1.4.3/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       29 2023-06-02 00:40:16.000000 yetl-framework-1.4.3/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-06-02 00:40:16.000000 yetl-framework-1.4.3/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.4.2/PKG-INFO` & `yetl-framework-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.4.2
+Version: 1.4.3
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.4.2/README.md` & `yetl-framework-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/setup.py` & `yetl-framework-1.4.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.4.2",
+    version="1.4.3",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
@@ -26,14 +26,15 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
     ],
     packages=[
         "yetl",
         "yetl.cli",
+        "yetl.cli.metadata_provider",
         "yetl.config",
         "yetl.config.table",
         "yetl.workflow",
 
     ],
     install_requires=[
           'PyYAML',
```

### Comparing `yetl-framework-1.4.2/yetl/__main__.py` & `yetl-framework-1.4.3/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/cli/_init.py` & `yetl-framework-1.4.3/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/config/__init__.py` & `yetl-framework-1.4.3/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/config/_config.py` & `yetl-framework-1.4.3/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/config/_decorators.py` & `yetl-framework-1.4.3/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/config/_logging_config.py` & `yetl-framework-1.4.3/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/config/_project.py` & `yetl-framework-1.4.3/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/config/_spark_context.py` & `yetl-framework-1.4.3/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/config/_tables.py` & `yetl-framework-1.4.3/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/config/_timeslice.py` & `yetl-framework-1.4.3/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/config/_utils.py` & `yetl-framework-1.4.3/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/config/deltalake.py` & `yetl-framework-1.4.3/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/config/table/_deltalake.py` & `yetl-framework-1.4.3/yetl/config/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/config/table/_factory.py` & `yetl-framework-1.4.3/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/config/table/_read.py` & `yetl-framework-1.4.3/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/config/table/_table.py` & `yetl-framework-1.4.3/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.4.3/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.2/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.4.3/yetl_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.4.2
+Version: 1.4.3
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.4.2/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.4.3/yetl_framework.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 README.md
 setup.py
 yetl/__init__.py
 yetl/__main__.py
 yetl/cli/_init.py
+yetl/cli/metadata_provider/__init__.py
+yetl/cli/metadata_provider/_xlsx.py
 yetl/config/__init__.py
 yetl/config/_config.py
 yetl/config/_decorators.py
 yetl/config/_logging_config.py
 yetl/config/_project.py
 yetl/config/_spark_context.py
 yetl/config/_stage_type.py
```

