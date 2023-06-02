# Comparing `tmp/citrusdb-0.3.0.tar.gz` & `tmp/citrusdb-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citrusdb-0.3.0.tar", last modified: Thu Jun  1 13:26:10 2023, max compression
+gzip compressed data, was "citrusdb-0.3.1.tar", last modified: Fri Jun  2 08:17:54 2023, max compression
```

## Comparing `citrusdb-0.3.0.tar` & `citrusdb-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.128952 citrusdb-0.3.0/
--rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.3.0/LICENSE
--rw-r--r--   0 debabrata   (501) staff       (20)     2175 2023-06-01 13:26:10.128769 citrusdb-0.3.0/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)     1666 2023-06-01 13:10:08.000000 citrusdb-0.3.0/README.md
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.125799 citrusdb-0.3.0/citrusdb/
--rw-r--r--   0 debabrata   (501) staff       (20)      166 2023-06-01 13:09:38.000000 citrusdb-0.3.0/citrusdb/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.127263 citrusdb-0.3.0/citrusdb/api/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.0/citrusdb/api/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     3969 2023-06-01 13:09:38.000000 citrusdb-0.3.0/citrusdb/api/index.py
--rw-r--r--   0 debabrata   (501) staff       (20)     5708 2023-06-01 13:09:38.000000 citrusdb-0.3.0/citrusdb/api/local.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.124397 citrusdb-0.3.0/citrusdb/db/
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.127632 citrusdb-0.3.0/citrusdb/db/index/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.0/citrusdb/db/index/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-01 13:09:38.000000 citrusdb-0.3.0/citrusdb/db/index/hnswlib.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.127985 citrusdb-0.3.0/citrusdb/embedding/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.0/citrusdb/embedding/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.3.0/citrusdb/embedding/openai.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.128544 citrusdb-0.3.0/citrusdb/utils/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 13:09:38.000000 citrusdb-0.3.0/citrusdb/utils/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      205 2023-06-01 13:09:38.000000 citrusdb-0.3.0/citrusdb/utils/types.py
--rw-r--r--   0 debabrata   (501) staff       (20)      663 2023-06-01 13:09:38.000000 citrusdb-0.3.0/citrusdb/utils/utils.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.126756 citrusdb-0.3.0/citrusdb.egg-info/
--rw-r--r--   0 debabrata   (501) staff       (20)     2175 2023-06-01 13:26:10.000000 citrusdb-0.3.0/citrusdb.egg-info/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)      484 2023-06-01 13:26:10.000000 citrusdb-0.3.0/citrusdb.egg-info/SOURCES.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-06-01 13:26:10.000000 citrusdb-0.3.0/citrusdb.egg-info/dependency_links.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       40 2023-06-01 13:26:10.000000 citrusdb-0.3.0/citrusdb.egg-info/requires.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        9 2023-06-01 13:26:10.000000 citrusdb-0.3.0/citrusdb.egg-info/top_level.txt
--rw-r--r--   0 debabrata   (501) staff       (20)      598 2023-06-01 13:22:53.000000 citrusdb-0.3.0/pyproject.toml
--rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-06-01 13:26:10.129004 citrusdb-0.3.0/setup.cfg
--rw-r--r--   0 debabrata   (501) staff       (20)      771 2023-06-01 13:23:08.000000 citrusdb-0.3.0/setup.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.407555 citrusdb-0.3.1/
+-rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.3.1/LICENSE
+-rw-r--r--   0 debabrata   (501) staff       (20)     2249 2023-06-02 08:17:54.407377 citrusdb-0.3.1/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)     1666 2023-06-01 13:10:08.000000 citrusdb-0.3.1/README.md
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.403327 citrusdb-0.3.1/citrusdb/
+-rw-r--r--   0 debabrata   (501) staff       (20)      166 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.404803 citrusdb-0.3.1/citrusdb/api/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.1/citrusdb/api/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     3969 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/api/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     5708 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/api/local.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.402253 citrusdb-0.3.1/citrusdb/db/
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.405351 citrusdb-0.3.1/citrusdb/db/index/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.1/citrusdb/db/index/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/db/index/hnswlib.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.406148 citrusdb-0.3.1/citrusdb/db/sqlite/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/db/sqlite/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     2712 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/db/sqlite/db.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1322 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/db/sqlite/queries.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1369 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/db/sqlite/query_builder.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.406604 citrusdb-0.3.1/citrusdb/embedding/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.1/citrusdb/embedding/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.3.1/citrusdb/embedding/openai.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.407146 citrusdb-0.3.1/citrusdb/utils/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/utils/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      205 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/utils/types.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      663 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/utils/utils.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.404270 citrusdb-0.3.1/citrusdb.egg-info/
+-rw-r--r--   0 debabrata   (501) staff       (20)     2249 2023-06-02 08:17:54.000000 citrusdb-0.3.1/citrusdb.egg-info/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)      606 2023-06-02 08:17:54.000000 citrusdb-0.3.1/citrusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-06-02 08:17:54.000000 citrusdb-0.3.1/citrusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       40 2023-06-02 08:17:54.000000 citrusdb-0.3.1/citrusdb.egg-info/requires.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        9 2023-06-02 08:17:54.000000 citrusdb-0.3.1/citrusdb.egg-info/top_level.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)      672 2023-06-02 08:17:44.000000 citrusdb-0.3.1/pyproject.toml
+-rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-06-02 08:17:54.407603 citrusdb-0.3.1/setup.cfg
+-rw-r--r--   0 debabrata   (501) staff       (20)      894 2023-06-02 08:17:37.000000 citrusdb-0.3.1/setup.py
```

### Comparing `citrusdb-0.3.0/LICENSE` & `citrusdb-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.0/PKG-INFO` & `citrusdb-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.3.0
-Summary: citrus.
+Version: 0.3.1
+Summary: open-source vector database. store and retrieve embeddings for your next project!
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
-Metadata-Version: 2.1 Name: citrusdb Version: 0.3.0 Summary: citrus. Home-page:
+Metadata-Version: 2.1 Name: citrusdb Version: 0.3.1 Summary: open-source vector
+database. store and retrieve embeddings for your next project! Home-page:
 https://github.com/0xDebabrata/citrus Author: Debabrata Mondal Author-email:
 Debabrata Mondal
 js@protonmail.com> Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE # ð citrus. ### open-source (distributed) vector
```

### Comparing `citrusdb-0.3.0/README.md` & `citrusdb-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.0/citrusdb/api/index.py` & `citrusdb-0.3.1/citrusdb/api/index.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.0/citrusdb/api/local.py` & `citrusdb-0.3.1/citrusdb/api/local.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.0/citrusdb/db/index/hnswlib.py` & `citrusdb-0.3.1/citrusdb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.0/citrusdb/utils/utils.py` & `citrusdb-0.3.1/citrusdb/utils/utils.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.0/citrusdb.egg-info/PKG-INFO` & `citrusdb-0.3.1/citrusdb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.3.0
-Summary: citrus.
+Version: 0.3.1
+Summary: open-source vector database. store and retrieve embeddings for your next project!
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
-Metadata-Version: 2.1 Name: citrusdb Version: 0.3.0 Summary: citrus. Home-page:
+Metadata-Version: 2.1 Name: citrusdb Version: 0.3.1 Summary: open-source vector
+database. store and retrieve embeddings for your next project! Home-page:
 https://github.com/0xDebabrata/citrus Author: Debabrata Mondal Author-email:
 Debabrata Mondal
 js@protonmail.com> Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE # ð citrus. ### open-source (distributed) vector
```

### Comparing `citrusdb-0.3.0/setup.py` & `citrusdb-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="citrusdb",
-    version="0.3.0",
+    version="0.3.1",
     author="Debabrata Mondal",
     author_email="debabrata.js@protonmail.com",
     description="(distributed) vector database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/0xDebabrata/citrus",
-    packages=find_packages(exclude=["demo"]),
+    packages=(
+        find_packages(
+            exclude=["demo"]
+        ) +
+        ["citrusdb.db.index", "citrusdb.db.sqlite"]
+    ),
+    include_package_data=True,
     install_requires=[
         "numpy",
         "hnswlib",
         "openai",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
```

