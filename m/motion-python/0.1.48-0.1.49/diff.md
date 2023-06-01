# Comparing `tmp/motion_python-0.1.48.tar.gz` & `tmp/motion_python-0.1.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.48.tar", max compression
+gzip compressed data, was "motion_python-0.1.49.tar", max compression
```

## Comparing `motion_python-0.1.48.tar` & `motion_python-0.1.49.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-01 19:39:38.490110 motion_python-0.1.48/README.md
--rw-r--r--   0        0        0      202 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/__init__.py
--rw-r--r--   0        0        0     1817 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/cli.py
--rw-r--r--   0        0        0    23617 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/component.py
--rw-r--r--   0        0        0    13729 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/execute.py
--rw-r--r--   0        0        0     4961 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/fit_task.py
--rw-r--r--   0        0        0     9364 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      595 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/route.py
--rw-r--r--   0        0        0     6283 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/utils.py
--rw-r--r--   0        0        0     1517 2023-06-01 19:40:01.520150 motion_python-0.1.48/pyproject.toml
--rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 motion_python-0.1.48/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-01 22:07:06.923974 motion_python-0.1.49/README.md
+-rw-r--r--   0        0        0      202 2023-06-01 22:07:06.923974 motion_python-0.1.49/motion/__init__.py
+-rw-r--r--   0        0        0     1817 2023-06-01 22:07:06.923974 motion_python-0.1.49/motion/cli.py
+-rw-r--r--   0        0        0    23617 2023-06-01 22:07:06.927974 motion_python-0.1.49/motion/component.py
+-rw-r--r--   0        0        0    13729 2023-06-01 22:07:06.927974 motion_python-0.1.49/motion/execute.py
+-rw-r--r--   0        0        0     5182 2023-06-01 22:07:06.927974 motion_python-0.1.49/motion/fit_task.py
+-rw-r--r--   0        0        0     9364 2023-06-01 22:07:06.927974 motion_python-0.1.49/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-01 22:07:06.927974 motion_python-0.1.49/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      595 2023-06-01 22:07:06.927974 motion_python-0.1.49/motion/route.py
+-rw-r--r--   0        0        0     6283 2023-06-01 22:07:06.927974 motion_python-0.1.49/motion/utils.py
+-rw-r--r--   0        0        0     1517 2023-06-01 22:07:32.552110 motion_python-0.1.49/pyproject.toml
+-rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 motion_python-0.1.49/PKG-INFO
```

### Comparing `motion_python-0.1.48/README.md` & `motion_python-0.1.49/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.48/motion/cli.py` & `motion_python-0.1.49/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.48/motion/component.py` & `motion_python-0.1.49/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.48/motion/execute.py` & `motion_python-0.1.49/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.48/motion/fit_task.py` & `motion_python-0.1.49/motion/fit_task.py`

 * *Files 14% similar despite different names*

```diff
@@ -144,9 +144,18 @@
             port=self.redis_port,
             password=self.redis_password,
             db=self.redis_db,
         )
 
         # Add outstanding batch back to queue
         for item in self.batch:
-            redis_con.lpush(self.queue_identifier, item)
+            # Pickle item object
+            pickled_item = cloudpickle.dumps(
+                (
+                    item,
+                    False,  # flush_fit should be False
+                )
+            )
+
+            redis_con.lpush(self.queue_identifier, pickled_item)
+
         self.batch = []
```

### Comparing `motion_python-0.1.48/motion/instance.py` & `motion_python-0.1.49/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.48/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.49/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.48/motion/route.py` & `motion_python-0.1.49/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.48/motion/utils.py` & `motion_python-0.1.49/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.48/pyproject.toml` & `motion_python-0.1.49/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.48"
+version = "0.1.49"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.48/PKG-INFO` & `motion_python-0.1.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.48
+Version: 0.1.49
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

