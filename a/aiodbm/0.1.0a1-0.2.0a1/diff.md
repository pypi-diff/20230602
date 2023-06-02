# Comparing `tmp/aiodbm-0.1.0a1.tar.gz` & `tmp/aiodbm-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodbm-0.1.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodbm-0.2.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodbm-0.1.0a1.tar` & `aiodbm-0.2.0a1.tar`

### file list

```diff
@@ -1,17 +1,24 @@
--rw-r--r--   0        0        0      221 2023-05-31 12:59:34.028365 aiodbm-0.1.0a1/.coveragerc
--rw-r--r--   0        0        0      964 2023-06-01 00:00:49.918153 aiodbm-0.1.0a1/.github/workflows/main.yml
--rw-r--r--   0        0        0      798 2023-06-01 00:00:49.918153 aiodbm-0.1.0a1/.github/workflows/release.yml
--rw-r--r--   0        0        0      110 2023-05-31 01:31:26.803876 aiodbm-0.1.0a1/.gitignore
--rw-r--r--   0        0        0      477 2023-05-31 13:13:07.581265 aiodbm-0.1.0a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1080 2023-05-31 00:53:23.248884 aiodbm-0.1.0a1/LICENSE
--rw-r--r--   0        0        0      121 2023-05-31 13:00:10.815989 aiodbm-0.1.0a1/Makefile
--rw-r--r--   0        0        0     2152 2023-06-01 00:52:05.226071 aiodbm-0.1.0a1/README.rst
--rw-r--r--   0        0        0      524 2023-05-31 01:02:36.048582 aiodbm-0.1.0a1/dbm_viewer.py
--rw-r--r--   0        0        0      378 2023-06-01 00:51:11.106230 aiodbm-0.1.0a1/examples/basic_usage.py
--rw-r--r--   0        0        0      736 2023-06-01 00:58:32.392882 aiodbm-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      200 2023-06-01 00:14:30.296139 aiodbm-0.1.0a1/src/aiodbm/__init__.py
--rw-r--r--   0        0        0     4630 2023-06-01 00:26:22.324764 aiodbm-0.1.0a1/src/aiodbm/core.py
--rw-r--r--   0        0        0        0 2023-05-31 00:55:46.532853 aiodbm-0.1.0a1/tests/__init__.py
--rw-r--r--   0        0        0     6320 2023-06-01 00:41:05.139768 aiodbm-0.1.0a1/tests/test_core.py
--rw-r--r--   0        0        0      397 2023-05-31 12:58:42.736904 aiodbm-0.1.0a1/tox.ini
--rw-r--r--   0        0        0     2777 1970-01-01 00:00:00.000000 aiodbm-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      221 2023-05-31 12:59:34.028365 aiodbm-0.2.0a1/.coveragerc
+-rw-r--r--   0        0        0      964 2023-06-01 00:00:49.918153 aiodbm-0.2.0a1/.github/workflows/main.yml
+-rw-r--r--   0        0        0      798 2023-06-01 00:00:49.918153 aiodbm-0.2.0a1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      110 2023-05-31 01:31:26.803876 aiodbm-0.2.0a1/.gitignore
+-rw-r--r--   0        0        0      477 2023-05-31 13:13:07.581265 aiodbm-0.2.0a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      142 2023-06-02 17:34:44.178645 aiodbm-0.2.0a1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1080 2023-05-31 00:53:23.248884 aiodbm-0.2.0a1/LICENSE
+-rw-r--r--   0        0        0      121 2023-05-31 13:00:10.815989 aiodbm-0.2.0a1/Makefile
+-rw-r--r--   0        0        0     2287 2023-06-02 17:30:00.580465 aiodbm-0.2.0a1/README.rst
+-rw-r--r--   0        0        0      634 2023-06-02 17:04:23.375256 aiodbm-0.2.0a1/docs/Makefile
+-rw-r--r--   0        0        0       37 2023-06-02 17:04:23.375256 aiodbm-0.2.0a1/docs/_static/custom.css
+-rw-r--r--   0        0        0       97 2023-06-02 17:31:54.543635 aiodbm-0.2.0a1/docs/api.rst
+-rw-r--r--   0        0        0     1856 2023-06-02 17:19:55.420980 aiodbm-0.2.0a1/docs/conf.py
+-rw-r--r--   0        0        0      347 2023-06-02 17:04:23.375256 aiodbm-0.2.0a1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-06-02 17:04:23.375256 aiodbm-0.2.0a1/docs/make.bat
+-rw-r--r--   0        0        0      378 2023-06-01 00:51:11.106230 aiodbm-0.2.0a1/examples/basic_usage.py
+-rw-r--r--   0        0        0      736 2023-06-01 00:58:32.392882 aiodbm-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-06-02 17:19:55.424980 aiodbm-0.2.0a1/src/aiodbm/__init__.py
+-rw-r--r--   0        0        0     8076 2023-06-02 17:27:04.806092 aiodbm-0.2.0a1/src/aiodbm/core.py
+-rw-r--r--   0        0        0        0 2023-05-31 00:55:46.532853 aiodbm-0.2.0a1/tests/__init__.py
+-rw-r--r--   0        0        0     2044 2023-06-02 17:03:15.638929 aiodbm-0.2.0a1/tests/measurements.py
+-rw-r--r--   0        0        0     8303 2023-06-02 17:03:15.638929 aiodbm-0.2.0a1/tests/test_core.py
+-rw-r--r--   0        0        0      397 2023-05-31 12:58:42.736904 aiodbm-0.2.0a1/tox.ini
+-rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 aiodbm-0.2.0a1/PKG-INFO
```

### Comparing `aiodbm-0.1.0a1/.github/workflows/main.yml` & `aiodbm-0.2.0a1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aiodbm-0.1.0a1/.github/workflows/release.yml` & `aiodbm-0.2.0a1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aiodbm-0.1.0a1/LICENSE` & `aiodbm-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodbm-0.1.0a1/README.rst` & `aiodbm-0.2.0a1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-======
-aiodbm
-======
+=======================
+aiodbm: DBM for AsyncIO
+=======================
 
-A AsyncIO wrapper for Python's `DBM library <https://docs.python.org/3/library/dbm.html>`_.
+An AsyncIO bridge for Python's DBM library.
 
 |release| |python| |tests| |codecov| |docs| |pre-commit| |Code style: black|
 
 Description
 -----------
 
-* Supports 100% of GDBM API
+* Supports 100% of DBM and GDBM API
 * Typing support
 * Docstrings for all methods
+* Good test coverage
 
-To ensure DBM can be used safely with AsyncIO, all DB operations are serialized,
-i.e. only one DB operation occurs at any given time.
+To ensure DBM can be used safely with AsyncIO, all DB operations are serialized and run in a separate thread.
 
-This library is primarily made for GDBM, but should work with other implementations too.
+This library is developed and tested primarily with GDBM, but should work with other implementations too.
 
 Usage
 -----
 
 Here is a basic example on how to use the queue:
 
 .. code:: python
 
     import asyncio
 
     import aiodbm
 
 
     async def main():
-        async with aiodbm.open("data.dbm", "c") as db:  # opening/creating database
+        async with aiodbm.open("example.dbm", "c") as db:  # opening/creating database
             await db.set("alpha", "green")  # creating new key alpha with value green
             value = await db.get("alpha")  # fetching value for key alpha
             print(value)
             await db.delete("alpha")  # delete key alpha
 
 
     asyncio.run(main())
@@ -47,14 +47,20 @@
 You can install this library directly from PyPI with the following command:
 
 .. code:: shell
 
     pip install aiodbm
 
 
+Reference
+---------
+
+See also Python's `DBM documentation <https://docs.python.org/3/library/dbm.html>`_
+
+
 .. |release| image:: https://img.shields.io/pypi/v/aiodbm?label=release
    :target: https://pypi.org/project/aiodbm/
 .. |python| image:: https://img.shields.io/pypi/pyversions/aiodbm
    :target: https://pypi.org/project/aiodbm/
 .. |tests| image:: https://github.com/ErikKalkoken/aiodbm/actions/workflows/main.yml/badge.svg
    :target: https://github.com/ErikKalkoken/aiodbm/actions
 .. |codecov| image:: https://codecov.io/gh/ErikKalkoken/aiodbm/branch/main/graph/badge.svg?token=V43h7hl1Te
```

### Comparing `aiodbm-0.1.0a1/pyproject.toml` & `aiodbm-0.2.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiodbm-0.1.0a1/tests/test_core.py` & `aiodbm-0.2.0a1/tests/test_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,54 @@
+import asyncio
+import dbm
 import shutil
 import sys
 import tempfile
+import time
 import unittest
 from pathlib import Path
 
 import aiodbm
+from aiodbm.core import Message
 
 python_version = f"{sys.version_info.major}{sys.version_info.minor}"
 
 
+class TestMessage(unittest.IsolatedAsyncioTestCase):
+    async def test_str(self):
+        def alpha():
+            pass
+
+        # given
+        future = asyncio.get_running_loop().create_future()
+        message = Message(future, alpha)
+        # then
+        self.assertIn("alpha", str(message))
+
+    def test_can_create_stop_signal(self):
+        # when
+        message = Message.create_stop_signal()
+        # then
+        self.assertTrue(message.is_stop_signal)
+
+    def test_future_strict_raises_error_when_no_future(self):
+        # given
+        message = Message.create_stop_signal()
+        # when/then
+        with self.assertRaises(ValueError):
+            message.future_strict
+
+    def test_func_strict_raises_error_when_no_func(self):
+        # given
+        message = Message.create_stop_signal()
+        # when/then
+        with self.assertRaises(ValueError):
+            message.func_strict
+
+
 class DbmAsyncioTestCase(unittest.IsolatedAsyncioTestCase):
     def setUp(self) -> None:
         self.temp_dir = Path(tempfile.mkdtemp())
         self.data_path = str(self.temp_dir / "data.dbm")
 
     def tearDown(self) -> None:
         shutil.rmtree(self.temp_dir, ignore_errors=True)
@@ -138,14 +174,45 @@
             # given
             await db.set("alpha", "green")
             # when
             result = await db.setdefault("alpha", b"blue")
             # then
             self.assertEqual(result, b"green")
 
+    async def test_should_stop_thread_after_leaving_context(self):
+        async with aiodbm.open(self.data_path, "c") as db:
+            pass
+        # then
+        time.sleep(1)
+        self.assertFalse(db.is_alive())
+
+    async def test_should_stop_thread_when_closing(self):
+        async with aiodbm.open(self.data_path, "c") as db:
+            # when
+            await db.close()
+            # then
+            time.sleep(1)
+            self.assertFalse(db.is_alive())
+
+    async def test_can_open_without_context_manager(self):
+        db = await aiodbm.open(self.data_path, "c")
+        await db.get("dummy")
+        await db.close()
+
+    async def test_open_raises_exception_when_opening_fails(self):
+        with self.assertRaises(dbm.error):
+            await aiodbm.open(self.data_path, "r")
+
+    async def test_can_call_close_multiple_timers(self):
+        # given
+        db = await aiodbm.open(self.data_path, "c")
+        await db.close()
+        # when/then
+        await db.close()
+
 
 @unittest.skipIf(python_version in ["38", "39"], reason="Unsupported Python")
 class TestGdbmFunctions(DbmAsyncioTestCase):
     async def test_firstkey_should_return_first_key(self):
         async with aiodbm.open(self.data_path, "c") as db:
             # given
             await db.set("alpha", "green")
```

### Comparing `aiodbm-0.1.0a1/PKG-INFO` & `aiodbm-0.2.0a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 Metadata-Version: 2.1
 Name: aiodbm
-Version: 0.1.0a1
-Summary: A AsyncIO wrapper for DBM.
+Version: 0.2.0a1
+Summary: An AsyncIO bridge for DBM.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Source, https://github.com/ErikKalkoken/aiodbm
 Project-URL: Tracker, https://github.com/ErikKalkoken/aiodbm/issues
 
-======
-aiodbm
-======
+=======================
+aiodbm: DBM for AsyncIO
+=======================
 
-A AsyncIO wrapper for Python's `DBM library <https://docs.python.org/3/library/dbm.html>`_.
+An AsyncIO bridge for Python's DBM library.
 
 |release| |python| |tests| |codecov| |docs| |pre-commit| |Code style: black|
 
 Description
 -----------
 
-* Supports 100% of GDBM API
+* Supports 100% of DBM and GDBM API
 * Typing support
 * Docstrings for all methods
+* Good test coverage
 
-To ensure DBM can be used safely with AsyncIO, all DB operations are serialized,
-i.e. only one DB operation occurs at any given time.
+To ensure DBM can be used safely with AsyncIO, all DB operations are serialized and run in a separate thread.
 
-This library is primarily made for GDBM, but should work with other implementations too.
+This library is developed and tested primarily with GDBM, but should work with other implementations too.
 
 Usage
 -----
 
 Here is a basic example on how to use the queue:
 
 .. code:: python
 
     import asyncio
 
     import aiodbm
 
 
     async def main():
-        async with aiodbm.open("data.dbm", "c") as db:  # opening/creating database
+        async with aiodbm.open("example.dbm", "c") as db:  # opening/creating database
             await db.set("alpha", "green")  # creating new key alpha with value green
             value = await db.get("alpha")  # fetching value for key alpha
             print(value)
             await db.delete("alpha")  # delete key alpha
 
 
     asyncio.run(main())
@@ -63,14 +63,20 @@
 You can install this library directly from PyPI with the following command:
 
 .. code:: shell
 
     pip install aiodbm
 
 
+Reference
+---------
+
+See also Python's `DBM documentation <https://docs.python.org/3/library/dbm.html>`_
+
+
 .. |release| image:: https://img.shields.io/pypi/v/aiodbm?label=release
    :target: https://pypi.org/project/aiodbm/
 .. |python| image:: https://img.shields.io/pypi/pyversions/aiodbm
    :target: https://pypi.org/project/aiodbm/
 .. |tests| image:: https://github.com/ErikKalkoken/aiodbm/actions/workflows/main.yml/badge.svg
    :target: https://github.com/ErikKalkoken/aiodbm/actions
 .. |codecov| image:: https://codecov.io/gh/ErikKalkoken/aiodbm/branch/main/graph/badge.svg?token=V43h7hl1Te
```

