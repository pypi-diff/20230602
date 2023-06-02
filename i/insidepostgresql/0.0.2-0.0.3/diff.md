# Comparing `tmp/insidepostgresql-0.0.2.tar.gz` & `tmp/insidepostgresql-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insidepostgresql-0.0.2.tar", last modified: Sat May 27 21:57:16 2023, max compression
+gzip compressed data, was "insidepostgresql-0.0.3.tar", last modified: Fri Jun  2 05:09:16 2023, max compression
```

## Comparing `insidepostgresql-0.0.2.tar` & `insidepostgresql-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-27 21:57:16.017189 insidepostgresql-0.0.2/
--rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-05-27 20:03:17.000000 insidepostgresql-0.0.2/LICENSE
--rw-rw-r--   0 demir     (1000) demir     (1000)     2183 2023-05-27 21:57:16.017189 insidepostgresql-0.0.2/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)     1661 2023-05-27 21:51:18.000000 insidepostgresql-0.0.2/README.md
--rw-rw-r--   0 demir     (1000) demir     (1000)      695 2023-05-27 21:57:16.017189 insidepostgresql-0.0.2/setup.cfg
--rw-rw-r--   0 demir     (1000) demir     (1000)      943 2023-05-27 21:57:07.000000 insidepostgresql-0.0.2/setup.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-27 21:57:16.013189 insidepostgresql-0.0.2/src/
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-27 21:57:16.017189 insidepostgresql-0.0.2/src/insidepostgresql.egg-info/
--rw-rw-r--   0 demir     (1000) demir     (1000)     2183 2023-05-27 21:57:16.000000 insidepostgresql-0.0.2/src/insidepostgresql.egg-info/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)      311 2023-05-27 21:57:16.000000 insidepostgresql-0.0.2/src/insidepostgresql.egg-info/SOURCES.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-05-27 21:57:16.000000 insidepostgresql-0.0.2/src/insidepostgresql.egg-info/dependency_links.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       34 2023-05-27 21:57:16.000000 insidepostgresql-0.0.2/src/insidepostgresql.egg-info/requires.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       11 2023-05-27 21:57:16.000000 insidepostgresql-0.0.2/src/insidepostgresql.egg-info/top_level.txt
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-27 21:57:16.017189 insidepostgresql-0.0.2/src/postgresql/
--rw-rw-r--   0 demir     (1000) demir     (1000)       25 2023-05-27 20:03:59.000000 insidepostgresql-0.0.2/src/postgresql/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     5363 2023-05-27 21:47:24.000000 insidepostgresql-0.0.2/src/postgresql/postgresql.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-06-02 05:09:16.006121 insidepostgresql-0.0.3/
+-rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-05-27 20:03:17.000000 insidepostgresql-0.0.3/LICENSE
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4856 2023-06-02 05:09:16.006121 insidepostgresql-0.0.3/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4334 2023-06-02 05:08:27.000000 insidepostgresql-0.0.3/README.md
+-rw-rw-r--   0 demir     (1000) demir     (1000)      695 2023-06-02 05:09:16.006121 insidepostgresql-0.0.3/setup.cfg
+-rw-rw-r--   0 demir     (1000) demir     (1000)      943 2023-06-02 05:06:37.000000 insidepostgresql-0.0.3/setup.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-06-02 05:09:16.006121 insidepostgresql-0.0.3/src/
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-06-02 05:09:16.006121 insidepostgresql-0.0.3/src/insidepostgresql.egg-info/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4856 2023-06-02 05:09:16.000000 insidepostgresql-0.0.3/src/insidepostgresql.egg-info/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)      311 2023-06-02 05:09:16.000000 insidepostgresql-0.0.3/src/insidepostgresql.egg-info/SOURCES.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-06-02 05:09:16.000000 insidepostgresql-0.0.3/src/insidepostgresql.egg-info/dependency_links.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       34 2023-06-02 05:09:16.000000 insidepostgresql-0.0.3/src/insidepostgresql.egg-info/requires.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       11 2023-06-02 05:09:16.000000 insidepostgresql-0.0.3/src/insidepostgresql.egg-info/top_level.txt
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-06-02 05:09:16.006121 insidepostgresql-0.0.3/src/postgresql/
+-rw-rw-r--   0 demir     (1000) demir     (1000)       25 2023-05-27 20:03:59.000000 insidepostgresql-0.0.3/src/postgresql/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     9089 2023-06-01 09:41:17.000000 insidepostgresql-0.0.3/src/postgresql/postgresql.py
```

### Comparing `insidepostgresql-0.0.2/LICENSE` & `insidepostgresql-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `insidepostgresql-0.0.2/setup.cfg` & `insidepostgresql-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = insidecocuhbase
-version = 0.0.2
+version = 0.0.3
 author = Huseyin Demir
 author_email = huseyin.d3r@gmail.com
 description = A simple Python package
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/adiosamig/insidepgs
 project_urls =
```

### Comparing `insidepostgresql-0.0.2/setup.py` & `insidepostgresql-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "insidepostgresql",
-    version = "0.0.2",
+    version = "0.0.3",
     author = "Huseyin Demir",
     author_email = "huseyin.d3r@gmail.com",
     description = "Check and analyze a PostgreSQL cluster.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adiosamig/insidepgs",
     install_requires=[
```

