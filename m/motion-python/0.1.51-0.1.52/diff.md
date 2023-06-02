# Comparing `tmp/motion_python-0.1.51.tar.gz` & `tmp/motion_python-0.1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.51.tar", max compression
+gzip compressed data, was "motion_python-0.1.52.tar", max compression
```

## Comparing `motion_python-0.1.51.tar` & `motion_python-0.1.52.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-02 00:11:05.158117 motion_python-0.1.51/README.md
--rw-r--r--   0        0        0      202 2023-06-02 00:11:05.158117 motion_python-0.1.51/motion/__init__.py
--rw-r--r--   0        0        0     1817 2023-06-02 00:11:05.158117 motion_python-0.1.51/motion/cli.py
--rw-r--r--   0        0        0    23617 2023-06-02 00:11:05.158117 motion_python-0.1.51/motion/component.py
--rw-r--r--   0        0        0    14089 2023-06-02 00:11:05.158117 motion_python-0.1.51/motion/execute.py
--rw-r--r--   0        0        0     5182 2023-06-02 00:11:05.158117 motion_python-0.1.51/motion/fit_task.py
--rw-r--r--   0        0        0     9364 2023-06-02 00:11:05.162117 motion_python-0.1.51/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-02 00:11:05.162117 motion_python-0.1.51/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      595 2023-06-02 00:11:05.162117 motion_python-0.1.51/motion/route.py
--rw-r--r--   0        0        0     6283 2023-06-02 00:11:05.162117 motion_python-0.1.51/motion/utils.py
--rw-r--r--   0        0        0     1555 2023-06-02 00:11:26.690306 motion_python-0.1.51/pyproject.toml
--rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 motion_python-0.1.51/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-02 16:01:25.780389 motion_python-0.1.52/README.md
+-rw-r--r--   0        0        0      202 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/__init__.py
+-rw-r--r--   0        0        0     1817 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/cli.py
+-rw-r--r--   0        0        0    23617 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/component.py
+-rw-r--r--   0        0        0    14131 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/execute.py
+-rw-r--r--   0        0        0     5182 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/fit_task.py
+-rw-r--r--   0        0        0     9364 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      595 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/route.py
+-rw-r--r--   0        0        0     6283 2023-06-02 16:01:25.784389 motion_python-0.1.52/motion/utils.py
+-rw-r--r--   0        0        0     1555 2023-06-02 16:01:43.648863 motion_python-0.1.52/pyproject.toml
+-rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 motion_python-0.1.52/PKG-INFO
```

### Comparing `motion_python-0.1.51/README.md` & `motion_python-0.1.52/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.51/motion/cli.py` & `motion_python-0.1.52/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.51/motion/component.py` & `motion_python-0.1.52/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.51/motion/execute.py` & `motion_python-0.1.52/motion/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
                 self._save_state_func,
             )
         else:
             # Load state
             self._state = self._loadState()
             self.version = self._redis_con.get(f"MOTION_VERSION:{self._instance_name}")
 
+        self.version = int(self.version)
+
         # Set up routes
         self._infer_routes: Dict[str, Route] = infer_routes
         self._fit_routes: Dict[str, Dict[str, Route]] = {
             rkey: {route.udf.__name__: route for route in routes}
             for rkey, routes in fit_routes.items()
         }
```

### Comparing `motion_python-0.1.51/motion/fit_task.py` & `motion_python-0.1.52/motion/fit_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.51/motion/instance.py` & `motion_python-0.1.52/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.51/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.52/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.51/motion/route.py` & `motion_python-0.1.52/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.51/motion/utils.py` & `motion_python-0.1.52/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.51/pyproject.toml` & `motion_python-0.1.52/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.51"
+version = "0.1.52"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.51/PKG-INFO` & `motion_python-0.1.52/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.51
+Version: 0.1.52
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

