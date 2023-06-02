# Comparing `tmp/yo-1.0.2.tar.gz` & `tmp/yo-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yo-1.0.2.tar", last modified: Fri Jun  2 18:55:31 2023, max compression
+gzip compressed data, was "yo-1.0.3.tar", last modified: Fri Jun  2 21:52:33 2023, max compression
```

## Comparing `yo-1.0.2.tar` & `yo-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 18:55:31.402872 yo-1.0.2/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1848 2023-04-17 22:02:18.000000 yo-1.0.2/LICENSE.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3099 2023-06-02 18:55:31.402872 yo-1.0.2/PKG-INFO
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2532 2023-05-09 18:31:11.000000 yo-1.0.2/README.md
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   156525 2023-03-01 19:22:05.000000 yo-1.0.2/THIRD_PARTY_LICENSES.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      307 2023-06-02 18:55:31.402872 yo-1.0.2/setup.cfg
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3427 2023-06-02 18:54:59.000000 yo-1.0.2/setup.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 18:55:31.402872 yo-1.0.2/tests/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7971 2023-03-01 19:22:05.000000 yo-1.0.2/tests/test_api.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7350 2023-03-21 16:43:28.000000 yo-1.0.2/tests/test_cmds.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 18:55:31.402872 yo-1.0.2/yo/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        0 2023-01-25 21:25:24.000000 yo-1.0.2/yo/__init__.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1998 2023-03-01 19:22:05.000000 yo-1.0.2/yo/__main__.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)    67881 2023-06-02 18:54:59.000000 yo-1.0.2/yo/api.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 18:55:31.402872 yo-1.0.2/yo/data/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8092 2023-03-21 20:11:11.000000 yo-1.0.2/yo/data/sample.yo.ini
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 18:55:31.402872 yo-1.0.2/yo/data/yo-tasks/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2396 2023-03-01 19:22:05.000000 yo-1.0.2/yo/data/yo-tasks/drgn
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1956 2023-03-01 19:22:05.000000 yo-1.0.2/yo/data/yo-tasks/ocid
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2032 2023-03-01 19:22:05.000000 yo-1.0.2/yo/data/yo-tasks/test-deps
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       23 2023-01-25 21:25:24.000000 yo-1.0.2/yo/data/yo-tasks/test-existing-task
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1957 2023-03-01 19:22:05.000000 yo-1.0.2/yo/data/yo-tasks/test-run-many
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2008 2023-03-01 19:22:05.000000 yo-1.0.2/yo/data/yo-tasks/test-task
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1277 2023-03-23 17:58:33.000000 yo-1.0.2/yo/data/yo_tasklib.sh
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   108412 2023-06-02 18:54:59.000000 yo-1.0.2/yo/main.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     5886 2023-03-02 23:11:21.000000 yo-1.0.2/yo/oci.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8366 2023-03-23 18:16:50.000000 yo-1.0.2/yo/util.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 18:55:31.402872 yo-1.0.2/yo.egg-info/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3099 2023-06-02 18:55:31.000000 yo-1.0.2/yo.egg-info/PKG-INFO
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      541 2023-06-02 18:55:31.000000 yo-1.0.2/yo.egg-info/SOURCES.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        1 2023-06-02 18:55:31.000000 yo-1.0.2/yo.egg-info/dependency_links.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       36 2023-06-02 18:55:31.000000 yo-1.0.2/yo.egg-info/entry_points.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       64 2023-06-02 18:55:31.000000 yo-1.0.2/yo.egg-info/requires.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        3 2023-06-02 18:55:31.000000 yo-1.0.2/yo.egg-info/top_level.txt
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 21:52:33.761397 yo-1.0.3/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1848 2023-04-17 22:02:18.000000 yo-1.0.3/LICENSE.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3099 2023-06-02 21:52:33.761397 yo-1.0.3/PKG-INFO
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2532 2023-05-09 18:31:11.000000 yo-1.0.3/README.md
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   156525 2023-03-01 19:22:05.000000 yo-1.0.3/THIRD_PARTY_LICENSES.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      307 2023-06-02 21:52:33.761397 yo-1.0.3/setup.cfg
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3427 2023-06-02 21:52:19.000000 yo-1.0.3/setup.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 21:52:33.757397 yo-1.0.3/tests/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7971 2023-03-01 19:22:05.000000 yo-1.0.3/tests/test_api.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7350 2023-03-21 16:43:28.000000 yo-1.0.3/tests/test_cmds.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 21:52:33.757397 yo-1.0.3/yo/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        0 2023-01-25 21:25:24.000000 yo-1.0.3/yo/__init__.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1998 2023-03-01 19:22:05.000000 yo-1.0.3/yo/__main__.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)    67881 2023-06-02 18:54:59.000000 yo-1.0.3/yo/api.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 21:52:33.757397 yo-1.0.3/yo/data/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8092 2023-03-21 20:11:11.000000 yo-1.0.3/yo/data/sample.yo.ini
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 21:52:33.761397 yo-1.0.3/yo/data/yo-tasks/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2396 2023-03-01 19:22:05.000000 yo-1.0.3/yo/data/yo-tasks/drgn
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1956 2023-03-01 19:22:05.000000 yo-1.0.3/yo/data/yo-tasks/ocid
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2032 2023-03-01 19:22:05.000000 yo-1.0.3/yo/data/yo-tasks/test-deps
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       23 2023-01-25 21:25:24.000000 yo-1.0.3/yo/data/yo-tasks/test-existing-task
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1957 2023-03-01 19:22:05.000000 yo-1.0.3/yo/data/yo-tasks/test-run-many
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2008 2023-03-01 19:22:05.000000 yo-1.0.3/yo/data/yo-tasks/test-task
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1277 2023-03-23 17:58:33.000000 yo-1.0.3/yo/data/yo_tasklib.sh
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   109190 2023-06-02 21:52:19.000000 yo-1.0.3/yo/main.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     5886 2023-03-02 23:11:21.000000 yo-1.0.3/yo/oci.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8366 2023-03-23 18:16:50.000000 yo-1.0.3/yo/util.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 21:52:33.757397 yo-1.0.3/yo.egg-info/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3099 2023-06-02 21:52:33.000000 yo-1.0.3/yo.egg-info/PKG-INFO
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      541 2023-06-02 21:52:33.000000 yo-1.0.3/yo.egg-info/SOURCES.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        1 2023-06-02 21:52:33.000000 yo-1.0.3/yo.egg-info/dependency_links.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       36 2023-06-02 21:52:33.000000 yo-1.0.3/yo.egg-info/entry_points.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       64 2023-06-02 21:52:33.000000 yo-1.0.3/yo.egg-info/requires.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        3 2023-06-02 21:52:33.000000 yo-1.0.3/yo.egg-info/top_level.txt
```

### Comparing `yo-1.0.2/LICENSE.txt` & `yo-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/PKG-INFO` & `yo-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yo
-Version: 1.0.2
+Version: 1.0.3
 Summary: A fast and simple CLI client for managing OCI instances
 Home-page: https://github.com/oracle/yo
 Author: Oracle
 Author-email: stephen.s.brennan@oracle.com
 License: UPL
 Keywords: oci client
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yo-1.0.2/README.md` & `yo-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/THIRD_PARTY_LICENSES.txt` & `yo-1.0.3/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/setup.py` & `yo-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from setuptools import find_packages
 from setuptools import setup
 
 long_description = open("README.md").read()
 
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 
 setup(
     name="yo",
     version=VERSION,
     description="A fast and simple CLI client for managing OCI instances",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `yo-1.0.2/tests/test_api.py` & `yo-1.0.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/tests/test_cmds.py` & `yo-1.0.3/tests/test_cmds.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/yo/__main__.py` & `yo-1.0.3/yo/__main__.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/yo/api.py` & `yo-1.0.3/yo/api.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/yo/data/sample.yo.ini` & `yo-1.0.3/yo/data/sample.yo.ini`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/yo/data/yo-tasks/drgn` & `yo-1.0.3/yo/data/yo-tasks/drgn`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/yo/data/yo-tasks/ocid` & `yo-1.0.3/yo/data/yo-tasks/ocid`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/yo/data/yo-tasks/test-deps` & `yo-1.0.3/yo/data/yo-tasks/test-deps`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/yo/data/yo-tasks/test-run-many` & `yo-1.0.3/yo/data/yo-tasks/test-run-many`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/yo/data/yo-tasks/test-task` & `yo-1.0.3/yo/data/yo-tasks/test-task`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/yo/data/yo_tasklib.sh` & `yo-1.0.3/yo/data/yo_tasklib.sh`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/yo/main.py` & `yo-1.0.3/yo/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3118,29 +3118,52 @@
     name = "help"
     description = "show help for yo"
 
     def run(self) -> None:
         print(__doc__.strip())
 
 
+def _extend(ctx: YoCtx) -> None:
+    """
+    This is for advanced users to add custom extension scripts.  It is not
+    mentioned in the documentation, and for good reason: there is no stable API
+    defined (yet). However, it can still be useful to stick a stub in here for
+    something.
+    """
+    # The configuration "extension_modules" is still supported, but no longer
+    # recommended. Entry points (below) are a better way that don't require the
+    # user to manually configure things.
+    for module in ctx.config.extension_modules:
+        importlib.import_module(module)
+
+    # The importlib.metadata API is from Python 3.8+. So we can support the
+    # prior versions by falling back to pkg_resources.
+    try:
+        from importlib.metadata import entry_points  # novermin
+    except ImportError:
+        import pkg_resources
+
+        def entry_points(group):  # type: ignore
+            return pkg_resources.iter_entry_points(group)
+
+    for entry_point in entry_points(group="yo.extensions.v1"):
+        entry_point.load()
+
+
 def main() -> None:
     os.environ["OCI_PYTHON_SDK_NO_SERVICE_IMPORTS"] = "True"
     try:
         desc = (
             "A simple OCI client. Use 'yo help' for an overview, or yo -h "
             "for a listing of each command. For a help on a particular "
             "command, use 'yo COMMAND -h'."
         )
         parser = argparse.ArgumentParser(description=desc)
         ctx, aliases = YoCmd.setup_config()
-        # This is for advanced users to add custom extension scripts.
-        # It is not mentioned in the documentation, and for good reason:
-        # there is no stable API defined (yet).
-        for module in ctx.config.extension_modules:
-            importlib.import_module(module)
+        _extend(ctx)
         YoCmd.add_commands(
             parser,
             default="help",
             shortest_prefix=(not aliases),
             cmd_aliases=aliases,
         )
         argcomplete.autocomplete(parser)
```

### Comparing `yo-1.0.2/yo/oci.py` & `yo-1.0.3/yo/oci.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/yo/util.py` & `yo-1.0.3/yo/util.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.2/yo.egg-info/PKG-INFO` & `yo-1.0.3/yo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yo
-Version: 1.0.2
+Version: 1.0.3
 Summary: A fast and simple CLI client for managing OCI instances
 Home-page: https://github.com/oracle/yo
 Author: Oracle
 Author-email: stephen.s.brennan@oracle.com
 License: UPL
 Keywords: oci client
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yo-1.0.2/yo.egg-info/SOURCES.txt` & `yo-1.0.3/yo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

