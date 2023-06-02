# Comparing `tmp/sallron-0.2.8.tar.gz` & `tmp/sallron-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sallron-0.2.8.tar", last modified: Thu Jan 14 17:25:56 2021, max compression
+gzip compressed data, was "sallron-0.2.9.tar", last modified: Mon Feb  8 20:31:46 2021, max compression
```

## Comparing `sallron-0.2.8.tar` & `sallron-0.2.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 17:25:56.487033 sallron-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (116)     4119 2021-01-14 17:25:56.487033 sallron-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2190 2021-01-14 17:25:39.000000 sallron-0.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 17:25:56.479032 sallron-0.2.8/sallron/
--rw-r--r--   0 runner    (1001) docker     (116)      200 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 17:25:56.479032 sallron-0.2.8/sallron/db/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5153 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/db/caching.py
--rw-r--r--   0 runner    (1001) docker     (116)    11534 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/db/mongo.py
--rw-r--r--   0 runner    (1001) docker     (116)     2892 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/enforcer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 17:25:56.483032 sallron-0.2.8/sallron/extensions/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3859 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/extensions/e_raptor.py
--rw-r--r--   0 runner    (1001) docker     (116)     3840 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/eye.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 17:25:56.483032 sallron-0.2.8/sallron/util/
--rw-r--r--   0 runner    (1001) docker     (116)       21 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1351 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/util/discord.py
--rw-r--r--   0 runner    (1001) docker     (116)     1218 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/util/executor.py
--rw-r--r--   0 runner    (1001) docker     (116)     4077 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/util/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 17:25:56.487033 sallron-0.2.8/sallron/util/modifiers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/util/modifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1238 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/util/modifiers/get_vtex_categories_mod.py
--rw-r--r--   0 runner    (1001) docker     (116)     2443 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/util/parser.py
--rw-r--r--   0 runner    (1001) docker     (116)     1793 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/util/s3.py
--rw-r--r--   0 runner    (1001) docker     (116)      842 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/util/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     1136 2021-01-14 17:25:39.000000 sallron-0.2.8/sallron/util/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 17:25:56.479032 sallron-0.2.8/sallron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4119 2021-01-14 17:25:56.000000 sallron-0.2.8/sallron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      626 2021-01-14 17:25:56.000000 sallron-0.2.8/sallron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-14 17:25:56.000000 sallron-0.2.8/sallron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      143 2021-01-14 17:25:56.000000 sallron-0.2.8/sallron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2021-01-14 17:25:56.000000 sallron-0.2.8/sallron.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-14 17:25:56.487033 sallron-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1696 2021-01-14 17:25:39.000000 sallron-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-08 20:31:46.623359 sallron-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     4119 2021-02-08 20:31:46.623359 sallron-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2190 2021-02-08 20:31:26.000000 sallron-0.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-08 20:31:46.619359 sallron-0.2.9/sallron/
+-rw-r--r--   0 runner    (1001) docker     (116)      200 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-08 20:31:46.623359 sallron-0.2.9/sallron/db/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5153 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/db/caching.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11534 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/db/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2892 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/enforcer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-08 20:31:46.623359 sallron-0.2.9/sallron/extensions/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3859 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/extensions/e_raptor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3840 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/eye.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-08 20:31:46.623359 sallron-0.2.9/sallron/util/
+-rw-r--r--   0 runner    (1001) docker     (116)       21 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1351 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/util/discord.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1218 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/util/executor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4077 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/util/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-08 20:31:46.623359 sallron-0.2.9/sallron/util/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/util/modifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1238 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/util/modifiers/get_vtex_categories_mod.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2443 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/util/parser.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1793 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/util/s3.py
+-rw-r--r--   0 runner    (1001) docker     (116)      842 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/util/settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1136 2021-02-08 20:31:26.000000 sallron-0.2.9/sallron/util/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-08 20:31:46.619359 sallron-0.2.9/sallron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     4119 2021-02-08 20:31:46.000000 sallron-0.2.9/sallron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      626 2021-02-08 20:31:46.000000 sallron-0.2.9/sallron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-08 20:31:46.000000 sallron-0.2.9/sallron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      135 2021-02-08 20:31:46.000000 sallron-0.2.9/sallron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        8 2021-02-08 20:31:46.000000 sallron-0.2.9/sallron.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-02-08 20:31:46.623359 sallron-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1696 2021-02-08 20:31:26.000000 sallron-0.2.9/setup.py
```

### Comparing `sallron-0.2.8/PKG-INFO` & `sallron-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: sallron
-Version: 0.2.8
+Version: 0.2.9
 Summary: Collected data middleware for DB.
 Home-page: https://github.com/elint-tech/sallron/
 Author: elint-tech
 Author-email: contato@elint.com.br
 License: proprietary
-Download-URL: https://github.com/elint-tech/e-raptor/dist/sallron-0.2.8tar.gz
+Download-URL: https://github.com/elint-tech/e-raptor/dist/sallron-0.2.9tar.gz
 Description: sallron |PyPI version fury.io| |PyPI pyversions|
         ================================================
         
             Dynamically schedule data aggregation ⚔️ 👁️ 🗄️
         
         API agnostic data aggregation scheduler that automatically interacts
         with your interface class and sends responses to DB.
```

### Comparing `sallron-0.2.8/README.rst` & `sallron-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/sallron/db/caching.py` & `sallron-0.2.9/sallron/db/caching.py`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/sallron/db/mongo.py` & `sallron-0.2.9/sallron/db/mongo.py`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/sallron/enforcer.py` & `sallron-0.2.9/sallron/enforcer.py`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/sallron/extensions/e_raptor.py` & `sallron-0.2.9/sallron/extensions/e_raptor.py`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/sallron/eye.py` & `sallron-0.2.9/sallron/eye.py`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/sallron/util/discord.py` & `sallron-0.2.9/sallron/util/discord.py`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/sallron/util/executor.py` & `sallron-0.2.9/sallron/util/executor.py`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/sallron/util/logger.py` & `sallron-0.2.9/sallron/util/logger.py`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/sallron/util/modifiers/get_vtex_categories_mod.py` & `sallron-0.2.9/sallron/util/modifiers/get_vtex_categories_mod.py`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/sallron/util/parser.py` & `sallron-0.2.9/sallron/util/parser.py`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/sallron/util/s3.py` & `sallron-0.2.9/sallron/util/s3.py`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/sallron/util/settings.py` & `sallron-0.2.9/sallron/util/settings.py`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/sallron/util/stats.py` & `sallron-0.2.9/sallron/util/stats.py`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/sallron.egg-info/PKG-INFO` & `sallron-0.2.9/sallron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: sallron
-Version: 0.2.8
+Version: 0.2.9
 Summary: Collected data middleware for DB.
 Home-page: https://github.com/elint-tech/sallron/
 Author: elint-tech
 Author-email: contato@elint.com.br
 License: proprietary
-Download-URL: https://github.com/elint-tech/e-raptor/dist/sallron-0.2.8tar.gz
+Download-URL: https://github.com/elint-tech/e-raptor/dist/sallron-0.2.9tar.gz
 Description: sallron |PyPI version fury.io| |PyPI pyversions|
         ================================================
         
             Dynamically schedule data aggregation ⚔️ 👁️ 🗄️
         
         API agnostic data aggregation scheduler that automatically interacts
         with your interface class and sends responses to DB.
```

### Comparing `sallron-0.2.8/sallron.egg-info/SOURCES.txt` & `sallron-0.2.9/sallron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sallron-0.2.8/setup.py` & `sallron-0.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # python3 -m twine upload dist/*
 
 from setuptools import setup, find_packages
 from os.path import join, dirname
 
 here = dirname(__file__)
 
-_VERSION = '0.2.8'
+_VERSION = '0.2.9'
 
 setup(name='sallron',
       version=_VERSION,
       description="Collected data middleware for DB.",
       long_description=open(join(here, 'README.rst')).read(),
       license='proprietary',
       author='elint-tech',
```

