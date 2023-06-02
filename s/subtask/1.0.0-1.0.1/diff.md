# Comparing `tmp/subtask-1.0.0.tar.gz` & `tmp/subtask-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subtask-1.0.0.tar", max compression
+gzip compressed data, was "subtask-1.0.1.tar", max compression
```

## Comparing `subtask-1.0.0.tar` & `subtask-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-27 11:47:52.018372 subtask-1.0.0/LICENSE
--rw-r--r--   0        0        0      576 2023-05-27 11:47:52.018372 subtask-1.0.0/README.md
--rw-r--r--   0        0        0     1302 2023-05-27 11:47:52.018372 subtask-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      200 2023-05-27 11:47:52.018372 subtask-1.0.0/subtask/__init__.py
--rw-r--r--   0        0        0     4842 2023-05-27 11:47:52.018372 subtask-1.0.0/subtask/__subtask.py
--rw-r--r--   0        0        0        0 2023-05-27 11:47:52.018372 subtask-1.0.0/subtask/py.typed
--rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 subtask-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-02 09:11:31.959627 subtask-1.0.1/LICENSE
+-rw-r--r--   0        0        0      576 2023-06-02 09:11:31.959627 subtask-1.0.1/README.md
+-rw-r--r--   0        0        0     1302 2023-06-02 09:11:31.959627 subtask-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      200 2023-06-02 09:11:31.959627 subtask-1.0.1/subtask/__init__.py
+-rw-r--r--   0        0        0     4900 2023-06-02 09:11:31.959627 subtask-1.0.1/subtask/__subtask.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:11:31.959627 subtask-1.0.1/subtask/py.typed
+-rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 subtask-1.0.1/PKG-INFO
```

### Comparing `subtask-1.0.0/LICENSE` & `subtask-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `subtask-1.0.0/README.md` & `subtask-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `subtask-1.0.0/pyproject.toml` & `subtask-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "subtask"
-version = "1.0.0"
+version = "1.0.1"
 description = "A simple wrapper around `subprocess.Popen` to reduce the painfulness of running multiple processes concurrently."
 authors = ["Miguel Guthridge <hdsq@outlook.com.au>"]
 license = "MIT"
 readme = "README.md"
 
 repository = "https://github.com/MiguelGuthridge/subtask"
 documentation = "https://github.com/MiguelGuthridge/subtask"
```

### Comparing `subtask-1.0.0/subtask/__subtask.py` & `subtask-1.0.1/subtask/__subtask.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,22 +121,26 @@
         self.process.send_signal(signal.SIGINT)
 
     def kill(self) -> None:
         """Kill the process forcefully (useful if it's not responding)"""
         self.process.kill()
 
     @overload
-    def wait(self, timeout: int) -> Optional[int]:
+    def wait(self, timeout: float) -> Optional[int]:
+        ...
+
+    @overload
+    def wait(self) -> int:
         ...
 
     @overload
     def wait(self, timeout: None = None) -> int:
         ...
 
-    def wait(self, timeout: Optional[int] = None) -> Optional[int]:
+    def wait(self, timeout: Optional[float] = None) -> Optional[int]:
         """Wait for the process to finish executing and return its exit code"""
         try:
             ret = self.process.wait(timeout)
         except subprocess.TimeoutExpired:
             return None
         return ret
```

### Comparing `subtask-1.0.0/PKG-INFO` & `subtask-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subtask
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple wrapper around `subprocess.Popen` to reduce the painfulness of running multiple processes concurrently.
 Home-page: https://github.com/MiguelGuthridge/subtask
 License: MIT
 Keywords: popen,task,process,subprocess,subtask
 Author: Miguel Guthridge
 Author-email: hdsq@outlook.com.au
 Requires-Python: >=3.9,<4.0
```

