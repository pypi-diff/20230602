# Comparing `tmp/easyglobals-0.0.4.tar.gz` & `tmp/easyglobals-0.0.5.tar.gz`

## Comparing `easyglobals-0.0.4.tar` & `easyglobals-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/.gitignore
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/Easy_Globals.iml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/vcs.xml
--rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/workspace.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 easyglobals-0.0.4/src/EasyGlobals/EasyGlobals.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 easyglobals-0.0.4/src/EasyGlobals/__init__.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 easyglobals-0.0.4/tests/example_complex.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 easyglobals-0.0.4/tests/example_minimal.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 easyglobals-0.0.4/tests/example_multiprocess_easyglobals.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 easyglobals-0.0.4/LICENSE
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 easyglobals-0.0.4/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 easyglobals-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 easyglobals-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/.gitignore
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/Easy_Globals.iml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/vcs.xml
+-rw-r--r--   0        0        0    13306 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 easyglobals-0.0.5/src/EasyGlobals/EasyGlobals.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 easyglobals-0.0.5/src/EasyGlobals/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 easyglobals-0.0.5/tests/attribute_test.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 easyglobals-0.0.5/tests/example_complex.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 easyglobals-0.0.5/tests/example_minimal.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 easyglobals-0.0.5/tests/example_multiprocess_easyglobals.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 easyglobals-0.0.5/tests/example_multiprocess_easyglobals2.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 easyglobals-0.0.5/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 easyglobals-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 easyglobals-0.0.5/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 easyglobals-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 easyglobals-0.0.5/PKG-INFO
```

### Comparing `easyglobals-0.0.4/.idea/inspectionProfiles/Project_Default.xml` & `easyglobals-0.0.5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.4/src/EasyGlobals/EasyGlobals.py` & `easyglobals-0.0.5/tests/attribute_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,36 @@
+import time
+
 from pymemcache.client import base
 from pymemcache import serde
 class Globals:
 
     # Don t put this in init, that will break with setattr
     client = base.Client(('localhost', 11211), serde=serde.pickle_serde)
 
     def __setattr__(self, key, value):
         self.client.set(key, value)
-            # Note the variable down locally
-        object.__setattr__(self, key, 'in_db')
+    def __getattr__(self, key):
+        return self.client.get(key)
+
+
+    # def __getattribute__(self, key):
+    #     # print(f'Key: {key}')
+
+        # except AttributeError:
+        #     # If a variable doesn't exist in the class yet, check if it is in DB first.
+        #     # If so create it as  local variable too.
+        #     object.__setattr__(self, 'RetrievalValueTest', self.client.get(key))
+        #     if   self.RetrievalValueTest is not None:
+        #         # print('added key')
+        #         object.__setattr__(self, key, 'in_db')
+        #         return  self.RetrievalValueTest
+        #     else:
+        #         print(f'ERROR: Key --> {key} <-- not found in Memcahced Globals!')
+        #         raise AttributeError
+
+g = Globals()
+g.a = 5
 
-    def __getattribute__(self, key):
-        # print(f'Key: {key}')
-        try:
-            # To make class itself callable
-            if object.__getattribute__(self, key) == 'in_db':
-                return self.client.get(key)
-            else:
-                return  object.__getattribute__(self, key)
-
-
-        except AttributeError:
-            # If a variable doesn't exist in the class yet, check if it is in DB first.
-            # If so create it as  local variable too.
-            object.__setattr__(self, 'RetrievalValueTest', self.client.get(key))
-            if   self.RetrievalValueTest is not None:
-                # print('added key')
-                object.__setattr__(self, key, 'in_db')
-                return  self.RetrievalValueTest
-            else:
-                print(f'ERROR: Key --> {key} <-- not found in Memcahced Globals!')
-                raise AttributeError
+print(g.a)
+time.sleep(0.5)
+print(g.b)
```

### Comparing `easyglobals-0.0.4/tests/example_complex.py` & `easyglobals-0.0.5/tests/example_complex.py`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.4/tests/example_multiprocess_easyglobals.py` & `easyglobals-0.0.5/tests/example_multiprocess_easyglobals.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from EasyGlobals import EasyGlobals
+# from EasyGlobals import EasyGlobals
+import attribute_test as EasyGlobals
+
 import multiprocessing
 
 def write_to_globals():
     g = EasyGlobals.Globals()
     for i in range(1_000):
         g.testvar = i
 
@@ -24,7 +26,27 @@
     processlist[i].start()
 
 for process in processlist:
     process.join()
 print('Done reading')
 write_process.join()
 print('Done writing')
+
+
+
+class myclass:
+    def __init__(self):
+        self.x = 'tset'
+
+
+class myclass2:
+    def __init__(self):
+        self.x = 2
+        self.y = myclass()
+
+tst = myclass2()
+print(tst.__dict__)
+print(tst.x)
+print(tst.y.x)
+globals.test4 = tst
+
+print(globals.test4)
```

### Comparing `easyglobals-0.0.4/.gitignore` & `easyglobals-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.4/LICENSE` & `easyglobals-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.4/README.md` & `easyglobals-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Introduction
  EasyGlobals is an easy to use variable sharing library for Python that can quickly share complex objects between processes as if they had shared memory.
 
-It uses Memcached in the background to share full objects and other complex variables between Python processes. Inspired by many closed source languages which have an easy way to share "global" variables between processes while retaining pythonic syntax.
+It uses Memcached in the background to share full objects and other complex variables between Python processes. Inspired by many closed source languages which have an easy way to share "global" variables between processes while retaining pythonic syntax. No need for Multiprocessing Manager dicts, queues and other complex data pipelines in your program anymore.
 
 # Usage
+After installation following the instructions down below, try running the following example
 ```
 import EasyGlobals
 globals = EasyGlobals.Globals()
 
 globals.test1 = 4
 globals.test2 = 'hello world'
 globals.test3 = {'dictkey1': globals.test1, 'dictkey2': globals.test2} #  Dict
```

### Comparing `easyglobals-0.0.4/pyproject.toml` & `easyglobals-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "EasyGlobals"
-version = "0.0.4"
+version = "0.0.5"
 dependencies = [
     "pymemcache"
 ]
 authors = [
   { name="Yacob", email="asnaeb2@gmail.com" },
 ]
-description = "An easy to use variable sharing library for Python that can quickly share complex objects between processes as if they had shared memory."
+description = "An easy to use variable sharing library for Python using Memcached to can quickly share complex objects between processes as if they had shared memory."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `easyglobals-0.0.4/PKG-INFO` & `easyglobals-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: EasyGlobals
-Version: 0.0.4
-Summary: An easy to use variable sharing library for Python that can quickly share complex objects between processes as if they had shared memory.
+Version: 0.0.5
+Summary: An easy to use variable sharing library for Python using Memcached to can quickly share complex objects between processes as if they had shared memory.
 Project-URL: Homepage, https://github.com/YacobBY/Easy_Globals
 Project-URL: Bug Tracker, https://github.com/YacobBY/Easy_Globals/issues
 Author-email: Yacob <asnaeb2@gmail.com>
 License-File: LICENSE
 Keywords: Globals,Python,Shared memory
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,17 +13,18 @@
 Requires-Python: >=3.7
 Requires-Dist: pymemcache
 Description-Content-Type: text/markdown
 
 # Introduction
  EasyGlobals is an easy to use variable sharing library for Python that can quickly share complex objects between processes as if they had shared memory.
 
-It uses Memcached in the background to share full objects and other complex variables between Python processes. Inspired by many closed source languages which have an easy way to share "global" variables between processes while retaining pythonic syntax.
+It uses Memcached in the background to share full objects and other complex variables between Python processes. Inspired by many closed source languages which have an easy way to share "global" variables between processes while retaining pythonic syntax. No need for Multiprocessing Manager dicts, queues and other complex data pipelines in your program anymore.
 
 # Usage
+After installation following the instructions down below, try running the following example
 ```
 import EasyGlobals
 globals = EasyGlobals.Globals()
 
 globals.test1 = 4
 globals.test2 = 'hello world'
 globals.test3 = {'dictkey1': globals.test1, 'dictkey2': globals.test2} #  Dict
```

