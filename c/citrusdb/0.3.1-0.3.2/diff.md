# Comparing `tmp/citrusdb-0.3.1.tar.gz` & `tmp/citrusdb-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citrusdb-0.3.1.tar", last modified: Fri Jun  2 08:17:54 2023, max compression
+gzip compressed data, was "citrusdb-0.3.2.tar", last modified: Fri Jun  2 09:58:57 2023, max compression
```

## Comparing `citrusdb-0.3.1.tar` & `citrusdb-0.3.2.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.407555 citrusdb-0.3.1/
--rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.3.1/LICENSE
--rw-r--r--   0 debabrata   (501) staff       (20)     2249 2023-06-02 08:17:54.407377 citrusdb-0.3.1/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)     1666 2023-06-01 13:10:08.000000 citrusdb-0.3.1/README.md
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.403327 citrusdb-0.3.1/citrusdb/
--rw-r--r--   0 debabrata   (501) staff       (20)      166 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.404803 citrusdb-0.3.1/citrusdb/api/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.1/citrusdb/api/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     3969 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/api/index.py
--rw-r--r--   0 debabrata   (501) staff       (20)     5708 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/api/local.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.402253 citrusdb-0.3.1/citrusdb/db/
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.405351 citrusdb-0.3.1/citrusdb/db/index/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.1/citrusdb/db/index/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/db/index/hnswlib.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.406148 citrusdb-0.3.1/citrusdb/db/sqlite/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/db/sqlite/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     2712 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/db/sqlite/db.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1322 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/db/sqlite/queries.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1369 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/db/sqlite/query_builder.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.406604 citrusdb-0.3.1/citrusdb/embedding/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.1/citrusdb/embedding/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.3.1/citrusdb/embedding/openai.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.407146 citrusdb-0.3.1/citrusdb/utils/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/utils/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      205 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/utils/types.py
--rw-r--r--   0 debabrata   (501) staff       (20)      663 2023-06-01 13:09:38.000000 citrusdb-0.3.1/citrusdb/utils/utils.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 08:17:54.404270 citrusdb-0.3.1/citrusdb.egg-info/
--rw-r--r--   0 debabrata   (501) staff       (20)     2249 2023-06-02 08:17:54.000000 citrusdb-0.3.1/citrusdb.egg-info/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)      606 2023-06-02 08:17:54.000000 citrusdb-0.3.1/citrusdb.egg-info/SOURCES.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-06-02 08:17:54.000000 citrusdb-0.3.1/citrusdb.egg-info/dependency_links.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       40 2023-06-02 08:17:54.000000 citrusdb-0.3.1/citrusdb.egg-info/requires.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        9 2023-06-02 08:17:54.000000 citrusdb-0.3.1/citrusdb.egg-info/top_level.txt
--rw-r--r--   0 debabrata   (501) staff       (20)      672 2023-06-02 08:17:44.000000 citrusdb-0.3.1/pyproject.toml
--rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-06-02 08:17:54.407603 citrusdb-0.3.1/setup.cfg
--rw-r--r--   0 debabrata   (501) staff       (20)      894 2023-06-02 08:17:37.000000 citrusdb-0.3.1/setup.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.052688 citrusdb-0.3.2/
+-rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.3.2/LICENSE
+-rw-r--r--   0 debabrata   (501) staff       (20)     2249 2023-06-02 09:58:57.052513 citrusdb-0.3.2/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)     1666 2023-06-01 13:10:08.000000 citrusdb-0.3.2/README.md
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.048411 citrusdb-0.3.2/citrusdb/
+-rw-r--r--   0 debabrata   (501) staff       (20)      166 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.049900 citrusdb-0.3.2/citrusdb/api/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.2/citrusdb/api/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     3969 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/api/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     5708 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/api/local.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.047210 citrusdb-0.3.2/citrusdb/db/
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.050244 citrusdb-0.3.2/citrusdb/db/index/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.2/citrusdb/db/index/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/db/index/hnswlib.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.051076 citrusdb-0.3.2/citrusdb/db/sqlite/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/db/sqlite/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     2749 2023-06-02 09:56:23.000000 citrusdb-0.3.2/citrusdb/db/sqlite/db.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1322 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/db/sqlite/queries.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1369 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/db/sqlite/query_builder.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.051428 citrusdb-0.3.2/citrusdb/embedding/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.2/citrusdb/embedding/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.3.2/citrusdb/embedding/openai.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.051933 citrusdb-0.3.2/citrusdb/utils/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/utils/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      205 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/utils/types.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      663 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/utils/utils.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.049349 citrusdb-0.3.2/citrusdb.egg-info/
+-rw-r--r--   0 debabrata   (501) staff       (20)     2249 2023-06-02 09:58:57.000000 citrusdb-0.3.2/citrusdb.egg-info/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)      649 2023-06-02 09:58:57.000000 citrusdb-0.3.2/citrusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-06-02 09:58:57.000000 citrusdb-0.3.2/citrusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       40 2023-06-02 09:58:57.000000 citrusdb-0.3.2/citrusdb.egg-info/requires.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       20 2023-06-02 09:58:57.000000 citrusdb-0.3.2/citrusdb.egg-info/top_level.txt
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.052295 citrusdb-0.3.2/cloud-temp/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 10:48:15.000000 citrusdb-0.3.2/cloud-temp/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     2065 2023-06-02 09:23:04.000000 citrusdb-0.3.2/cloud-temp/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      672 2023-06-02 09:58:22.000000 citrusdb-0.3.2/pyproject.toml
+-rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-06-02 09:58:57.052738 citrusdb-0.3.2/setup.cfg
+-rw-r--r--   0 debabrata   (501) staff       (20)      894 2023-06-02 09:58:15.000000 citrusdb-0.3.2/setup.py
```

### Comparing `citrusdb-0.3.1/LICENSE` & `citrusdb-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.1/PKG-INFO` & `citrusdb-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.3.1
+Version: 0.3.2
 Summary: open-source vector database. store and retrieve embeddings for your next project!
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: citrusdb Version: 0.3.1 Summary: open-source vector
+Metadata-Version: 2.1 Name: citrusdb Version: 0.3.2 Summary: open-source vector
 database. store and retrieve embeddings for your next project! Home-page:
 https://github.com/0xDebabrata/citrus Author: Debabrata Mondal Author-email:
 Debabrata Mondal
 js@protonmail.com> Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `citrusdb-0.3.1/README.md` & `citrusdb-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.1/citrusdb/api/index.py` & `citrusdb-0.3.2/citrusdb/api/index.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.1/citrusdb/api/local.py` & `citrusdb-0.3.2/citrusdb/api/local.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.1/citrusdb/db/index/hnswlib.py` & `citrusdb-0.3.2/citrusdb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.1/citrusdb/db/sqlite/db.py` & `citrusdb-0.3.2/citrusdb/db/sqlite/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,16 @@
         persist_directory: str,
     ):
         ensure_valid_path(persist_directory)
 
         self._con = sqlite3.connect(
             os.path.join(
                 persist_directory, "citrus.db"
-            )
+            ),
+            check_same_thread=False
         )
 
         cur = self._con.cursor()
         cur.execute("PRAGMA foreign_keys = ON")    # Enable foreign keys
         cur.executescript(f'''
         BEGIN;
         {queries.CREATE_INDEX_MANAGER_TABLE}
```

### Comparing `citrusdb-0.3.1/citrusdb/db/sqlite/queries.py` & `citrusdb-0.3.2/citrusdb/db/sqlite/queries.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.1/citrusdb/db/sqlite/query_builder.py` & `citrusdb-0.3.2/citrusdb/db/sqlite/query_builder.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.1/citrusdb/utils/utils.py` & `citrusdb-0.3.2/citrusdb/utils/utils.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.1/citrusdb.egg-info/PKG-INFO` & `citrusdb-0.3.2/citrusdb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.3.1
+Version: 0.3.2
 Summary: open-source vector database. store and retrieve embeddings for your next project!
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: citrusdb Version: 0.3.1 Summary: open-source vector
+Metadata-Version: 2.1 Name: citrusdb Version: 0.3.2 Summary: open-source vector
 database. store and retrieve embeddings for your next project! Home-page:
 https://github.com/0xDebabrata/citrus Author: Debabrata Mondal Author-email:
 Debabrata Mondal
 js@protonmail.com> Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `citrusdb-0.3.1/citrusdb.egg-info/SOURCES.txt` & `citrusdb-0.3.2/citrusdb.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -17,8 +17,10 @@
 citrusdb/db/sqlite/db.py
 citrusdb/db/sqlite/queries.py
 citrusdb/db/sqlite/query_builder.py
 citrusdb/embedding/__init__.py
 citrusdb/embedding/openai.py
 citrusdb/utils/__init__.py
 citrusdb/utils/types.py
-citrusdb/utils/utils.py
+citrusdb/utils/utils.py
+cloud-temp/__init__.py
+cloud-temp/index.py
```

### Comparing `citrusdb-0.3.1/pyproject.toml` & `citrusdb-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "citrusdb"
-version = "0.3.1"
+version = "0.3.2"
 
 authors = [
   { name="Debabrata Mondal", email="debabrata.js@protonmail.com" },
 ]
 description = "open-source vector database. store and retrieve embeddings for your next project!"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `citrusdb-0.3.1/setup.py` & `citrusdb-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="citrusdb",
-    version="0.3.1",
+    version="0.3.2",
     author="Debabrata Mondal",
     author_email="debabrata.js@protonmail.com",
     description="(distributed) vector database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/0xDebabrata/citrus",
     packages=(
```

