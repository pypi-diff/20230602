# Comparing `tmp/sutools-0.1.2.tar.gz` & `tmp/sutools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sutools-0.1.2.tar", last modified: Sat Apr 29 02:35:02 2023, max compression
+gzip compressed data, was "sutools-0.2.2.tar", last modified: Fri Jun  2 01:58:42 2023, max compression
```

## Comparing `sutools-0.1.2.tar` & `sutools-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:35:02.207953 sutools-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-29 02:34:38.000000 sutools-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-29 02:35:02.207953 sutools-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-29 02:34:38.000000 sutools-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-29 02:34:38.000000 sutools-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 02:35:02.207953 sutools-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-29 02:34:38.000000 sutools-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:35:02.199952 sutools-0.1.2/sutools/
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-29 02:34:38.000000 sutools-0.1.2/sutools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-04-29 02:34:38.000000 sutools-0.1.2/sutools/cli_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-29 02:34:38.000000 sutools-0.1.2/sutools/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-29 02:34:38.000000 sutools-0.1.2/sutools/meta_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:35:02.203953 sutools-0.1.2/sutools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-29 02:35:02.000000 sutools-0.1.2/sutools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-29 02:35:02.000000 sutools-0.1.2/sutools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 02:35:02.000000 sutools-0.1.2/sutools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 02:35:02.000000 sutools-0.1.2/sutools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:35:02.207953 sutools-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-04-29 02:34:38.000000 sutools-0.1.2/tests/test_cli_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18499 2023-04-29 02:34:38.000000 sutools-0.1.2/tests/test_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-29 02:34:38.000000 sutools-0.1.2/tests/test_meta_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-04-29 02:34:38.000000 sutools-0.1.2/tests/test_sutools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:58:42.039376 sutools-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-02 01:58:20.000000 sutools-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-06-02 01:58:42.035376 sutools-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-06-02 01:58:20.000000 sutools-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-02 01:58:20.000000 sutools-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 01:58:42.039376 sutools-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-02 01:58:20.000000 sutools-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:58:42.035376 sutools-0.2.2/sutools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-02 01:58:20.000000 sutools-0.2.2/sutools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-02 01:58:20.000000 sutools-0.2.2/sutools/bench_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-02 01:58:20.000000 sutools-0.2.2/sutools/cli_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-02 01:58:20.000000 sutools-0.2.2/sutools/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-02 01:58:20.000000 sutools-0.2.2/sutools/meta_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:58:42.035376 sutools-0.2.2/sutools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-06-02 01:58:42.000000 sutools-0.2.2/sutools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-02 01:58:42.000000 sutools-0.2.2/sutools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:58:42.000000 sutools-0.2.2/sutools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 01:58:42.000000 sutools-0.2.2/sutools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:58:42.035376 sutools-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-02 01:58:20.000000 sutools-0.2.2/tests/test_bench_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-06-02 01:58:20.000000 sutools-0.2.2/tests/test_cli_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18499 2023-06-02 01:58:20.000000 sutools-0.2.2/tests/test_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-02 01:58:20.000000 sutools-0.2.2/tests/test_meta_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-02 01:58:20.000000 sutools-0.2.2/tests/test_sutools.py
```

### Comparing `sutools-0.1.2/LICENSE` & `sutools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sutools-0.1.2/PKG-INFO` & `sutools-0.2.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sutools
-Version: 0.1.2
+Version: 0.2.2
 Summary: su (Super User) tools; per module utilities, designed to be lightweight, easy to configure, and reduce boilerplate code.
 Home-page: https://github.com/aastopher/sutools
 Author: Aaron Stopher
 Project-URL: Documentation, https://sutools.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/aastopher/sutools/issues
-Keywords: logs,logger,logging,cli,utils
+Keywords: logs,logger,logging,cli,utils,performance counter,benchmark
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -227,7 +227,85 @@
 **log output**
 ```
 16:16:34, 961 logger1 INFO 1 + 2 = 3
 16:16:34, 961 logger2 INFO 1 - 2 = -1
 ```
 
 ***
+</br>
+
+## Benchy Usage Example
+
+</br>
+
+The `benchy` decorator is designed to collect performance timing and call info for selected functions. This can be used in combination with `@su.register`, the decorators are order independent.
+
+```python
+import sutools as su
+
+@su.benchy
+@su.register
+def add(x : int, y : int):
+    '''add two integers'''
+    return x + y
+
+@su.register
+@su.benchy
+def subtract(x : int, y : int):
+    '''subtract two integers'''
+    return x - y
+
+@su.benchy
+@su.register
+def calc(x : int, y : int, atype : str = '+') -> int:
+    '''calculates a thing'''
+    if atype == '+':
+        res = x + y
+    elif atype == '-':
+        res = x - y
+    return res
+
+add(1,2)
+add(2,2)
+subtract(1,2)
+calc(2,3, atype='-')
+
+```
+
+After the functions have been executed, the benchmark report can be accessed with `su.benchy.report`.
+
+```python
+# print the benchmark report
+print(su.benchy.report)
+```
+
+**Example output**
+
+```
+{'add': [{'args': [{'type': 'int', 'value': 1}, {'type': 'int', 'value': 2}],
+        'benchmark': 0.00015466799959540367,
+        'kwargs': None,
+        'result': {'type': 'int', 'value': 3}},
+        {'args': [{'type': 'int', 'value': 2}, {'type': 'int', 'value': 2}],
+        'benchmark': 6.068096263334155e-05,
+        'kwargs': None,
+        'result': {'type': 'int', 'value': 4}}],
+'calc': [{'args': [{'type': 'int', 'value': 2}, {'type': 'int', 'value': 3}],
+        'benchmark': 4.855601582676172e-05,
+        'kwargs': {'atype': {'length': 1, 'type': 'str'}},
+        'result': {'type': 'int', 'value': 5}}],
+'subtract': [{'args': [{'type': 'int', 'value': 1}, {'type': 'int', 'value': 2}],
+        'benchmark': 5.205394700169563e-05,
+        'kwargs': None,
+        'result': {'type': 'int', 'value': -1}}]}
+```
+
+The output of the benchmark report will adhere to the following format: `function > call records`. Call records consist of `{args, kwargs, result, benchmark}` there will be a record for each call of a given function.
+
+**NOTE:** given an iterable for `arg`, `kwarg`, or `result` the object will be summarized in terms of vector length.
+
+```
+{'function_name': [{'args': [{'type': 'arg_type', 'value': int}]
+                    'benchmark': float,
+                    'kwargs': {'kwarg_name': {'type': 'arg_type', 'length': int, }}
+                    'result': {'type': 'arg_type', 'value': float}}]}
+```
```

### Comparing `sutools-0.1.2/setup.py` & `sutools-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sutools",
-    version="0.1.2",
+    version="0.2.2",
     author="Aaron Stopher",
     packages=setuptools.find_packages(include=["sutools"]),
     description="su (Super User) tools; per module utilities, designed to be lightweight, easy to configure, and reduce boilerplate code.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aastopher/sutools",
     project_urls={
         "Documentation": "https://sutools.readthedocs.io",
         "Bug Tracker": "https://github.com/aastopher/sutools/issues",
     },
-    keywords=['logs', 'logger', 'logging', 'cli', 'utils'],
+    keywords=['logs', 'logger', 'logging', 'cli', 'utils','performance counter', 'benchmark'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8",
 )
```

### Comparing `sutools-0.1.2/sutools/__init__.py` & `sutools-0.2.2/sutools/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from sutools import cli_handler, log_handler, meta_handler
+from sutools import cli_handler, log_handler, meta_handler, bench_handler
 import inspect, os, logging, datetime
 
 # init store
-store = meta_handler.Bucket()
+store = meta_handler.Store()
+benchy = bench_handler.Benchy()
+
 
 def register(func):
     '''register a function to the store
     
     :param func: the function to register
     '''
-    store.add_func(func)
+    original_func = getattr(func, "__wrapped__", func)
+    store.add_func(original_func)
     return func
 
+
 def cli(desc = None, logs = False):
     '''init cli and register to store
     
     :param desc: description of the CLI
     :param logs: enable logging in CLI
     '''
 
@@ -82,8 +86,8 @@
     else:
         log_obj = log_handler.Logger(name, loggers, loglvl, filename, filepath, filefmt, fhandler, filecap, filetimeout, file, streamfmt, shandler, stream)
     store.add_log(log_obj)
     return log_obj
 
 def log():
     '''retrieve loggers namespace from store'''
-    return store.log.loggers
+    return store.log.loggers
```

### Comparing `sutools-0.1.2/sutools/cli_handler.py` & `sutools-0.2.2/sutools/cli_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.1.2/sutools/log_handler.py` & `sutools-0.2.2/sutools/log_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.1.2/sutools/meta_handler.py` & `sutools-0.2.2/sutools/meta_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 
 
-class Bucket:
+class Store:
     """internal object for storing function dictionary"""
 
     def __init__(self):
         self.funcs = {}  # init function registration dictionary
         self.cli = None  # init cli object store
         self.log = None  # init logger object store
```

### Comparing `sutools-0.1.2/sutools.egg-info/PKG-INFO` & `sutools-0.2.2/sutools.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sutools
-Version: 0.1.2
+Version: 0.2.2
 Summary: su (Super User) tools; per module utilities, designed to be lightweight, easy to configure, and reduce boilerplate code.
 Home-page: https://github.com/aastopher/sutools
 Author: Aaron Stopher
 Project-URL: Documentation, https://sutools.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/aastopher/sutools/issues
-Keywords: logs,logger,logging,cli,utils
+Keywords: logs,logger,logging,cli,utils,performance counter,benchmark
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -227,7 +227,85 @@
 **log output**
 ```
 16:16:34, 961 logger1 INFO 1 + 2 = 3
 16:16:34, 961 logger2 INFO 1 - 2 = -1
 ```
 
 ***
+</br>
+
+## Benchy Usage Example
+
+</br>
+
+The `benchy` decorator is designed to collect performance timing and call info for selected functions. This can be used in combination with `@su.register`, the decorators are order independent.
+
+```python
+import sutools as su
+
+@su.benchy
+@su.register
+def add(x : int, y : int):
+    '''add two integers'''
+    return x + y
+
+@su.register
+@su.benchy
+def subtract(x : int, y : int):
+    '''subtract two integers'''
+    return x - y
+
+@su.benchy
+@su.register
+def calc(x : int, y : int, atype : str = '+') -> int:
+    '''calculates a thing'''
+    if atype == '+':
+        res = x + y
+    elif atype == '-':
+        res = x - y
+    return res
+
+add(1,2)
+add(2,2)
+subtract(1,2)
+calc(2,3, atype='-')
+
+```
+
+After the functions have been executed, the benchmark report can be accessed with `su.benchy.report`.
+
+```python
+# print the benchmark report
+print(su.benchy.report)
+```
+
+**Example output**
+
+```
+{'add': [{'args': [{'type': 'int', 'value': 1}, {'type': 'int', 'value': 2}],
+        'benchmark': 0.00015466799959540367,
+        'kwargs': None,
+        'result': {'type': 'int', 'value': 3}},
+        {'args': [{'type': 'int', 'value': 2}, {'type': 'int', 'value': 2}],
+        'benchmark': 6.068096263334155e-05,
+        'kwargs': None,
+        'result': {'type': 'int', 'value': 4}}],
+'calc': [{'args': [{'type': 'int', 'value': 2}, {'type': 'int', 'value': 3}],
+        'benchmark': 4.855601582676172e-05,
+        'kwargs': {'atype': {'length': 1, 'type': 'str'}},
+        'result': {'type': 'int', 'value': 5}}],
+'subtract': [{'args': [{'type': 'int', 'value': 1}, {'type': 'int', 'value': 2}],
+        'benchmark': 5.205394700169563e-05,
+        'kwargs': None,
+        'result': {'type': 'int', 'value': -1}}]}
+```
+
+The output of the benchmark report will adhere to the following format: `function > call records`. Call records consist of `{args, kwargs, result, benchmark}` there will be a record for each call of a given function.
+
+**NOTE:** given an iterable for `arg`, `kwarg`, or `result` the object will be summarized in terms of vector length.
+
+```
+{'function_name': [{'args': [{'type': 'arg_type', 'value': int}]
+                    'benchmark': float,
+                    'kwargs': {'kwarg_name': {'type': 'arg_type', 'length': int, }}
+                    'result': {'type': 'arg_type', 'value': float}}]}
+```
```

### Comparing `sutools-0.1.2/tests/test_cli_handler.py` & `sutools-0.2.2/tests/test_cli_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 def test_cli_desc(capsys, monkeypatch):
     def func_test(
         test, test2: str, test3: str = "test", test4="test2", teest4: str = "test"
     ) -> str:
         pass # pass since we are only testing the function description
     
-    store = meta_handler.Bucket()
+    store = meta_handler.Store()
     store.add_func(func_test)
 
     expected = "Test CLI"
     cli_obj = cli_handler.CLI(expected, False)
     cli_obj.add_funcs(store.funcs)
 
     monkeypatch.setattr(sys, "exit", lambda x: None)
@@ -41,15 +41,15 @@
 def test_cli_logs_on(capsys, monkeypatch, mock_atexit_register):
     expected = "test log"
 
     def func_test():
         log_obj.loggers.func_test.info(expected)
         return expected
 
-    store = meta_handler.Bucket()
+    store = meta_handler.Store()
     store.add_func(func_test)
 
     log_obj = log_handler.Logger(
         "test_logger",
         list(store.funcs.keys()),
         logging.INFO,
         None,
@@ -85,15 +85,15 @@
 
 
 def test_cli_logs_off(capsys, monkeypatch, mock_atexit_register):
     def func_test():
         log_obj.loggers.func_test.info("fail")
         print("pass")
 
-    store = meta_handler.Bucket()
+    store = meta_handler.Store()
     store.add_func(func_test)
 
     log_obj = log_handler.Logger(
         "test_logger",
         list(store.funcs.keys()),
         logging.INFO,
         None,
@@ -163,30 +163,30 @@
 
     namespace = argparse.Namespace(command="func_test", help=True, x=1, y=2, c="+")
 
     with patch(
         "sutools.cli_handler.argparse.ArgumentParser.parse_args", return_value=namespace
     ):
         cli_obj = cli_handler.CLI("description", False)
-        store = meta_handler.Bucket()
+        store = meta_handler.Store()
         store.add_func(func_test)
         cli_obj.add_funcs(store.funcs)
 
         monkeypatch.setattr(sys, "exit", lambda *args: None)
 
         cli_obj.parse()
 
     assert expected in cli_obj.parser.format_help()
 
 def test_async_func(capsys, monkeypatch, mock_atexit_register):
     async def func_test():
         await asyncio.sleep(0.1)
         print('pass')
 
-    store = meta_handler.Bucket()
+    store = meta_handler.Store()
     store.add_func(func_test)
 
     log_obj = log_handler.Logger(
         "test_logger",
         list(store.funcs.keys()),
         logging.INFO,
         None,
```

### Comparing `sutools-0.1.2/tests/test_log_handler.py` & `sutools-0.2.2/tests/test_log_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.1.2/tests/test_meta_handler.py` & `sutools-0.2.2/tests/test_meta_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,53 +13,57 @@
     monkeypatch.setattr(log_handler.atexit, "register", mock_atexit_register)
     return mock_atexit_register
 
 
 ### Tests
 
 
-# Define a test function for the add_func method of the meta_handler.Bucket class
+# Define a test function for the add_func method of the meta_handler.Store class
 def test_add_func():
     def func_test1():
-        pass
+        '''
+        null function, testing function storage
+        '''
 
     def func_test2():
-        pass
+        '''
+        null function, testing function storage
+        '''
 
     expected = ["func_test1", "func_test2"]
-    # Create a new meta_handler.Bucket object
-    store = meta_handler.Bucket()
+    # Create a new meta_handler.Store object
+    store = meta_handler.Store()
 
     # Add test functions to the store
     store.add_func(func_test1)
     store.add_func(func_test2)
 
     # Assert that the function was added correctly
     assert all(item in store.funcs for item in expected)
 
 
-# Define a test function for the add_cli method of the meta_handler.Bucket class
+# Define a test function for the add_cli method of the meta_handler.Store class
 def test_add_cli():
-    # Create a new meta_handler.Bucket object
-    store = meta_handler.Bucket()
+    # Create a new meta_handler.Store object
+    store = meta_handler.Store()
 
     # Create a new cli_handler.CLI object
     cli_obj = cli_handler.CLI("desc", False)
 
     # Add the cli_handler.CLI object to the store
     store.add_cli(cli_obj)
 
     # Assert that the CLI object was added correctly
     assert isinstance(store.cli, cli_handler.CLI)
 
 
-# Define a test function for the add_log method of the meta_handler.Bucket class
+# Define a test function for the add_log method of the meta_handler.Store class
 def test_add_log(mock_atexit_register):
-    # Create a new meta_handler.Bucket object
-    store = meta_handler.Bucket()
+    # Create a new meta_handler.Store object
+    store = meta_handler.Store()
 
     # Create a new log_handler.Logger object
     log_obj = log_handler.Logger(
         "test_logger",
         ["logger1", "logger2", "logger3"],
         logging.INFO,
         None,
```

### Comparing `sutools-0.1.2/tests/test_sutools.py` & `sutools-0.2.2/tests/test_sutools.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 @pytest.fixture
 def mock_atexit_register(monkeypatch):
     mock_atexit_register = Mock()
     monkeypatch.setattr(su.log_handler.atexit, "register", mock_atexit_register)
     return mock_atexit_register
 
 
-# #### Methods
-
+##### Methods
 
 # Test 1: this should test the register decorator from sutools
 # the result should be that the su.store contains a
 # none empty dictionary for the func property
 def test_register():
     def _get_defaults(func):
         """helper function to collect default func args"""
@@ -175,8 +174,8 @@
         monkeypatch.setattr(sys, "exit", lambda *args: None)
 
         # call the cli() function to execute the desired command and capture the log output
         su.cli(desc=expected_cli, logs=True)
 
     captured = capsys.readouterr()
 
-    assert expected_log in captured.out
+    assert expected_log in captured.out
```

