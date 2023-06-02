# Comparing `tmp/playmolecule-1.8.9.tar.gz` & `tmp/playmolecule-1.8.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.8.9.tar", last modified: Fri Jun  2 06:57:33 2023, max compression
+gzip compressed data, was "playmolecule-1.8.9.1.tar", last modified: Fri Jun  2 08:42:21 2023, max compression
```

## Comparing `playmolecule-1.8.9.tar` & `playmolecule-1.8.9.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:57:33.420462 playmolecule-1.8.9/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-02 06:57:11.000000 playmolecule-1.8.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-02 06:57:11.000000 playmolecule-1.8.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-02 06:57:33.420462 playmolecule-1.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-02 06:57:11.000000 playmolecule-1.8.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:57:33.420462 playmolecule-1.8.9/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 06:57:33.420462 playmolecule-1.8.9/playmolecule/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    33605 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:57:33.420462 playmolecule-1.8.9/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-02 06:57:33.000000 playmolecule-1.8.9/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-02 06:57:33.000000 playmolecule-1.8.9/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 06:57:33.000000 playmolecule-1.8.9/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 06:57:33.000000 playmolecule-1.8.9/playmolecule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 06:57:33.000000 playmolecule-1.8.9/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 06:57:33.000000 playmolecule-1.8.9/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-02 06:57:11.000000 playmolecule-1.8.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 06:57:33.420462 playmolecule-1.8.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-02 06:57:11.000000 playmolecule-1.8.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:57:33.420462 playmolecule-1.8.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-02 06:57:11.000000 playmolecule-1.8.9/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-02 06:57:11.000000 playmolecule-1.8.9/tests/test_app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-02 06:57:11.000000 playmolecule-1.8.9/tests/test_datacenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:21.489279 playmolecule-1.8.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-02 08:42:21.489279 playmolecule-1.8.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:21.489279 playmolecule-1.8.9.1/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-02 08:42:21.489279 playmolecule-1.8.9.1/playmolecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33556 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:21.489279 playmolecule-1.8.9.1/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-02 08:42:21.000000 playmolecule-1.8.9.1/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-02 08:42:21.000000 playmolecule-1.8.9.1/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:42:21.000000 playmolecule-1.8.9.1/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:42:21.000000 playmolecule-1.8.9.1/playmolecule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 08:42:21.000000 playmolecule-1.8.9.1/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 08:42:21.000000 playmolecule-1.8.9.1/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:42:21.489279 playmolecule-1.8.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:21.489279 playmolecule-1.8.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/tests/test_app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-02 08:41:44.000000 playmolecule-1.8.9.1/tests/test_datacenter.py
```

### Comparing `playmolecule-1.8.9/LICENSE.md` & `playmolecule-1.8.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/PKG-INFO` & `playmolecule-1.8.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.8.9
+Version: 1.8.9.1
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.8.9/playmolecule/__init__.py` & `playmolecule-1.8.9.1/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/playmolecule/_test_funcs.py` & `playmolecule-1.8.9.1/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/playmolecule/config.py` & `playmolecule-1.8.9.1/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/playmolecule/datacenter.py` & `playmolecule-1.8.9.1/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/playmolecule/devutils.py` & `playmolecule-1.8.9.1/playmolecule/devutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,18 +525,17 @@
 def report_alive(outdir):
     from datetime import datetime
     import time
 
     os.makedirs(outdir, exist_ok=True)
 
     while True:
-        current_date = datetime.now()
         try:
-            with open(os.path.join(outdir, ".pm.alive"), "w", buffering=0) as f:
-                f.write(current_date.isoformat())
+            with open(os.path.join(outdir, ".pm.alive"), "w") as f:
+                f.write(datetime.now().isoformat())
         except Exception:
             pass
         time.sleep(5)
 
 
 def app_wrapper2(
     func,
```

### Comparing `playmolecule-1.8.9/playmolecule/job.py` & `playmolecule-1.8.9.1/playmolecule/job.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/playmolecule/jsonlogger.py` & `playmolecule-1.8.9.1/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/playmolecule/local.py` & `playmolecule-1.8.9.1/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/playmolecule/playqueue.py` & `playmolecule-1.8.9.1/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/playmolecule/session.py` & `playmolecule-1.8.9.1/playmolecule/session.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/playmolecule/utils.py` & `playmolecule-1.8.9.1/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.8.9.1/playmolecule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.8.9
+Version: 1.8.9.1
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.8.9/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.8.9.1/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/pyproject.toml` & `playmolecule-1.8.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/tests/test.py` & `playmolecule-1.8.9.1/tests/test.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/tests/test_app_wrapper.py` & `playmolecule-1.8.9.1/tests/test_app_wrapper.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.9/tests/test_datacenter.py` & `playmolecule-1.8.9.1/tests/test_datacenter.py`

 * *Files identical despite different names*

