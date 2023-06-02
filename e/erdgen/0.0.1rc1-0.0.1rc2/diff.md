# Comparing `tmp/erdgen-0.0.1rc1.tar.gz` & `tmp/erdgen-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdgen-0.0.1rc1.tar", last modified: Fri Jun  2 00:57:38 2023, max compression
+gzip compressed data, was "erdgen-0.0.1rc2.tar", last modified: Fri Jun  2 18:45:25 2023, max compression
```

## Comparing `erdgen-0.0.1rc1.tar` & `erdgen-0.0.1rc2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:57:38.190090 erdgen-0.0.1rc1/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1068 2023-06-02 00:24:03.000000 erdgen-0.0.1rc1/LICENSE
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      169 2023-06-02 00:46:12.000000 erdgen-0.0.1rc1/MANIFEST.in
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     4336 2023-06-02 00:57:38.190090 erdgen-0.0.1rc1/PKG-INFO
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     3984 2023-06-02 00:24:03.000000 erdgen-0.0.1rc1/README.md
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:57:38.190090 erdgen-0.0.1rc1/erdgen/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:24:03.000000 erdgen-0.0.1rc1/erdgen/__init__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       87 2023-06-02 00:24:03.000000 erdgen-0.0.1rc1/erdgen/__main__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      419 2023-06-02 00:24:03.000000 erdgen-0.0.1rc1/erdgen/erdgen.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:57:38.190090 erdgen-0.0.1rc1/erdgen/src/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2977 2023-06-02 00:24:03.000000 erdgen-0.0.1rc1/erdgen/src/_.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:24:03.000000 erdgen-0.0.1rc1/erdgen/src/__init__.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:57:38.190090 erdgen-0.0.1rc1/erdgen.egg-info/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     4336 2023-06-02 00:57:38.000000 erdgen-0.0.1rc1/erdgen.egg-info/PKG-INFO
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      281 2023-06-02 00:57:38.000000 erdgen-0.0.1rc1/erdgen.egg-info/SOURCES.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        1 2023-06-02 00:57:38.000000 erdgen-0.0.1rc1/erdgen.egg-info/dependency_links.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      311 2023-06-02 00:57:38.000000 erdgen-0.0.1rc1/erdgen.egg-info/requires.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        7 2023-06-02 00:57:38.000000 erdgen-0.0.1rc1/erdgen.egg-info/top_level.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       38 2023-06-02 00:57:38.190090 erdgen-0.0.1rc1/setup.cfg
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      749 2023-06-02 00:57:04.000000 erdgen-0.0.1rc1/setup.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 18:45:25.511196 erdgen-0.0.1rc2/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1068 2023-06-02 00:24:03.000000 erdgen-0.0.1rc2/LICENSE
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      169 2023-06-02 18:44:51.000000 erdgen-0.0.1rc2/MANIFEST.in
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     4495 2023-06-02 18:45:25.507196 erdgen-0.0.1rc2/PKG-INFO
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     3912 2023-06-02 00:58:39.000000 erdgen-0.0.1rc2/README.md
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 18:45:25.507196 erdgen-0.0.1rc2/erdgen/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:24:03.000000 erdgen-0.0.1rc2/erdgen/__init__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       87 2023-06-02 00:24:03.000000 erdgen-0.0.1rc2/erdgen/__main__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      419 2023-06-02 00:24:03.000000 erdgen-0.0.1rc2/erdgen/erdgen.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 18:45:25.507196 erdgen-0.0.1rc2/erdgen/src/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     3004 2023-06-02 18:44:51.000000 erdgen-0.0.1rc2/erdgen/src/_.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:24:03.000000 erdgen-0.0.1rc2/erdgen/src/__init__.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 18:45:25.507196 erdgen-0.0.1rc2/erdgen.egg-info/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     4495 2023-06-02 18:45:25.000000 erdgen-0.0.1rc2/erdgen.egg-info/PKG-INFO
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      281 2023-06-02 18:45:25.000000 erdgen-0.0.1rc2/erdgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        1 2023-06-02 18:45:25.000000 erdgen-0.0.1rc2/erdgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       38 2023-06-02 18:45:25.000000 erdgen-0.0.1rc2/erdgen.egg-info/requires.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        7 2023-06-02 18:45:25.000000 erdgen-0.0.1rc2/erdgen.egg-info/top_level.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       38 2023-06-02 18:45:25.511196 erdgen-0.0.1rc2/setup.cfg
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      962 2023-06-02 18:44:51.000000 erdgen-0.0.1rc2/setup.py
```

### Comparing `erdgen-0.0.1rc1/LICENSE` & `erdgen-0.0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `erdgen-0.0.1rc1/PKG-INFO` & `erdgen-0.0.1rc2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: erdgen
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Generate a DBML ERD from DBT YML relationships
 Home-page: https://github.com/neo-andrew-moss/erdgen
 Author: Andrew Moss
 Author-email: andrew.moss@neofinancial.com
 License: MIT license
 Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `erdgen`
 
 > DBT YML ERD Generator
@@ -125,16 +130,13 @@
 
 ```bash
 make lint
 ```
 
 ## TODO
 
-- Package this on pypi
 - Add better error handling and reporting
 - Perhaps add a debug/verbose mode
 - Add tests lol
-- make pylint happy
-- better tooling and configs
 - make it less jank
```

### Comparing `erdgen-0.0.1rc1/README.md` & `erdgen-0.0.1rc2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -112,14 +112,11 @@
 
 ```bash
 make lint
 ```
 
 ## TODO
 
-- Package this on pypi
 - Add better error handling and reporting
 - Perhaps add a debug/verbose mode
 - Add tests lol
-- make pylint happy
-- better tooling and configs
 - make it less jank
```

### Comparing `erdgen-0.0.1rc1/erdgen/src/_.py` & `erdgen-0.0.1rc2/erdgen/src/_.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """src"""
 import os
 from functools import reduce
 from typing import List, Tuple, Dict, Union
 import yaml
 from jinja2 import Template
 
+
 def load_yml(file: str) -> Dict:
     """load_yml"""
     with open(file, "r") as stream:
         try:
             return yaml.safe_load(stream)
         except yaml.YAMLError as err:
             print(err)
@@ -23,17 +24,19 @@
     relationships = data["models"][0].get("relationships", [])
     join_cols = [rel["join"][0]["local"] for rel in relationships]
 
     if include_non_join_keys or not relationships:
         return [(col["name"], "int") for col in columns]
     else:
         return [
-            (col["name"], "int") # Always int
+            (col["name"], "int")  # Always int
             for col in columns
-            if col["name"] in join_cols or "Id" in col["name"] or "id" in col["name"] # Include `id` & `ID` columns always
+            if col["name"] in join_cols
+            or "Id" in col["name"]
+            or "id" in col["name"]  # Include `id` & `ID` columns always
         ]
 
 
 def extract_relationships(file: str) -> List[Tuple[str, str, str, str, str]]:
     """extract_relationships"""
     data = load_yml(file)
     relationships = data["models"][0].get("relationships", [])
```

### Comparing `erdgen-0.0.1rc1/erdgen.egg-info/PKG-INFO` & `erdgen-0.0.1rc2/erdgen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: erdgen
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Generate a DBML ERD from DBT YML relationships
 Home-page: https://github.com/neo-andrew-moss/erdgen
 Author: Andrew Moss
 Author-email: andrew.moss@neofinancial.com
 License: MIT license
 Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `erdgen`
 
 > DBT YML ERD Generator
@@ -125,16 +130,13 @@
 
 ```bash
 make lint
 ```
 
 ## TODO
 
-- Package this on pypi
 - Add better error handling and reporting
 - Perhaps add a debug/verbose mode
 - Add tests lol
-- make pylint happy
-- better tooling and configs
 - make it less jank
```

