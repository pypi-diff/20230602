# Comparing `tmp/playmolecule-1.8.8.tar.gz` & `tmp/playmolecule-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.8.8.tar", last modified: Wed May 31 09:35:51 2023, max compression
+gzip compressed data, was "playmolecule-1.8.9.tar", last modified: Fri Jun  2 06:57:33 2023, max compression
```

## Comparing `playmolecule-1.8.8.tar` & `playmolecule-1.8.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:35:51.417353 playmolecule-1.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-31 09:35:26.000000 playmolecule-1.8.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-31 09:35:26.000000 playmolecule-1.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-31 09:35:51.417353 playmolecule-1.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-31 09:35:26.000000 playmolecule-1.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:35:51.417353 playmolecule-1.8.8/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-31 09:35:26.000000 playmolecule-1.8.8/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-31 09:35:26.000000 playmolecule-1.8.8/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-31 09:35:51.417353 playmolecule-1.8.8/playmolecule/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-31 09:35:26.000000 playmolecule-1.8.8/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-31 09:35:26.000000 playmolecule-1.8.8/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-05-31 09:35:26.000000 playmolecule-1.8.8/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    33527 2023-05-31 09:35:26.000000 playmolecule-1.8.8/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-05-31 09:35:26.000000 playmolecule-1.8.8/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-31 09:35:26.000000 playmolecule-1.8.8/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-31 09:35:26.000000 playmolecule-1.8.8/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-31 09:35:26.000000 playmolecule-1.8.8/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-31 09:35:26.000000 playmolecule-1.8.8/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-05-31 09:35:26.000000 playmolecule-1.8.8/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-31 09:35:26.000000 playmolecule-1.8.8/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:35:51.417353 playmolecule-1.8.8/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-31 09:35:51.000000 playmolecule-1.8.8/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-31 09:35:51.000000 playmolecule-1.8.8/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:35:51.000000 playmolecule-1.8.8/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:35:51.000000 playmolecule-1.8.8/playmolecule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-31 09:35:51.000000 playmolecule-1.8.8/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 09:35:51.000000 playmolecule-1.8.8/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-31 09:35:26.000000 playmolecule-1.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:35:51.417353 playmolecule-1.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-31 09:35:26.000000 playmolecule-1.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:35:51.417353 playmolecule-1.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-31 09:35:26.000000 playmolecule-1.8.8/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-31 09:35:26.000000 playmolecule-1.8.8/tests/test_app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-31 09:35:26.000000 playmolecule-1.8.8/tests/test_datacenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:57:33.420462 playmolecule-1.8.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-02 06:57:11.000000 playmolecule-1.8.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-02 06:57:11.000000 playmolecule-1.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-02 06:57:33.420462 playmolecule-1.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-02 06:57:11.000000 playmolecule-1.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:57:33.420462 playmolecule-1.8.9/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 06:57:33.420462 playmolecule-1.8.9/playmolecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33605 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-02 06:57:11.000000 playmolecule-1.8.9/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:57:33.420462 playmolecule-1.8.9/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-02 06:57:33.000000 playmolecule-1.8.9/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-02 06:57:33.000000 playmolecule-1.8.9/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 06:57:33.000000 playmolecule-1.8.9/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 06:57:33.000000 playmolecule-1.8.9/playmolecule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 06:57:33.000000 playmolecule-1.8.9/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 06:57:33.000000 playmolecule-1.8.9/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-02 06:57:11.000000 playmolecule-1.8.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 06:57:33.420462 playmolecule-1.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-02 06:57:11.000000 playmolecule-1.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:57:33.420462 playmolecule-1.8.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-02 06:57:11.000000 playmolecule-1.8.9/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-02 06:57:11.000000 playmolecule-1.8.9/tests/test_app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-02 06:57:11.000000 playmolecule-1.8.9/tests/test_datacenter.py
```

### Comparing `playmolecule-1.8.8/LICENSE.md` & `playmolecule-1.8.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/PKG-INFO` & `playmolecule-1.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.8.8
+Version: 1.8.9
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.8.8/playmolecule/__init__.py` & `playmolecule-1.8.9/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/playmolecule/_test_funcs.py` & `playmolecule-1.8.9/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/playmolecule/config.py` & `playmolecule-1.8.9/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/playmolecule/datacenter.py` & `playmolecule-1.8.9/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/playmolecule/devutils.py` & `playmolecule-1.8.9/playmolecule/devutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -639,25 +639,27 @@
             params = config["params"]
             if "pm_options" in config:
                 pm_options = config["pm_options"]
 
         # Override folders if running inside container and PM mode
         params = _fix_args(params, indir, SESSION)
         params["outdir"] = "/data/out"
-        params["scratchdir"] = "/data/scratch"
+        if "scratchdir" in params:
+            params["scratchdir"] = "/data/scratch"
         outdir = params["outdir"]
 
         # Prepare app folders
         errorfile = os.path.join(outdir, "pmwsjob.err")
         logfile = os.path.join(outdir, "log.txt")
         # TODO: Deprecate completedfile and sleepfile
         completedfile = os.path.join(outdir, "pmwsjob.done")
         sleepfile = os.path.join("/data", "pmwsjob.sleep")
         os.makedirs(params["outdir"], exist_ok=True)
-        os.makedirs(params["scratchdir"], exist_ok=True)
+        if "scratchdir" in params:
+            os.makedirs(params["scratchdir"], exist_ok=True)
     except Exception:
         _handle_error(
             f"Failed at initializing wrapper with error:\n{traceback.format_exc()}",
             JOB,
             None,
         )
         return
```

### Comparing `playmolecule-1.8.8/playmolecule/job.py` & `playmolecule-1.8.9/playmolecule/job.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/playmolecule/jsonlogger.py` & `playmolecule-1.8.9/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/playmolecule/local.py` & `playmolecule-1.8.9/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/playmolecule/playqueue.py` & `playmolecule-1.8.9/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/playmolecule/session.py` & `playmolecule-1.8.9/playmolecule/session.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/playmolecule/utils.py` & `playmolecule-1.8.9/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.8.9/playmolecule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.8.8
+Version: 1.8.9
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.8.8/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.8.9/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/pyproject.toml` & `playmolecule-1.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/tests/test.py` & `playmolecule-1.8.9/tests/test.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/tests/test_app_wrapper.py` & `playmolecule-1.8.9/tests/test_app_wrapper.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.8/tests/test_datacenter.py` & `playmolecule-1.8.9/tests/test_datacenter.py`

 * *Files identical despite different names*

