# Comparing `tmp/rapidwright-2022.2.3.tar.gz` & `tmp/rapidwright-2023.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/proj/xsjhdstaff2/clavin/workspace3/RapidWright/python/dist/.tmp-w8wxc724/rapidwright-2022.2.3.tar", last modified: Wed May  3 23:18:31 2023, max compression
+gzip compressed data, was "/proj/xsjhdstaff2/clavin/workspace2/RapidWright/python/dist/.tmp-_qzzu3q4/rapidwright-2023.1.0.tar", last modified: Thu Jun  1 23:32:32 2023, max compression
```

## Comparing `rapidwright-2022.2.3.tar` & `rapidwright-2023.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 clavin   (25463) users      (100)        0 2023-05-03 23:18:31.000000 rapidwright-2022.2.3/
--rwxr-xr-x   0 clavin   (25463) users      (100)   526323 2023-05-03 23:18:24.000000 rapidwright-2022.2.3/LICENSE.TXT
--rw-r--r--   0 clavin   (25463) users      (100)     1076 2023-05-03 23:18:31.000000 rapidwright-2022.2.3/PKG-INFO
--rw-r--r--   0 clavin   (25463) users      (100)     2860 2022-08-02 03:11:34.000000 rapidwright-2022.2.3/README.md
--rw-r--r--   0 clavin   (25463) users      (100)       77 2023-05-03 23:18:31.000000 rapidwright-2022.2.3/setup.cfg
--rw-r--r--   0 clavin   (25463) users      (100)     2587 2023-05-03 23:17:07.000000 rapidwright-2022.2.3/setup.py
-drwxr-xr-x   0 clavin   (25463) users      (100)        0 2023-05-03 23:18:31.000000 rapidwright-2022.2.3/src/
-drwxr-xr-x   0 clavin   (25463) users      (100)        0 2023-05-03 23:18:31.000000 rapidwright-2022.2.3/src/rapidwright/
--rw-r--r--   0 clavin   (25463) users      (100)      883 2022-08-02 03:11:34.000000 rapidwright-2022.2.3/src/rapidwright/__init__.py
--rw-r--r--   0 clavin   (25463) users      (100)     1839 2023-05-03 23:17:07.000000 rapidwright-2022.2.3/src/rapidwright/rapidwright.py
-drwxr-xr-x   0 clavin   (25463) users      (100)        0 2023-05-03 23:18:31.000000 rapidwright-2022.2.3/src/rapidwright.egg-info/
--rw-r--r--   0 clavin   (25463) users      (100)     1076 2023-05-03 23:18:31.000000 rapidwright-2022.2.3/src/rapidwright.egg-info/PKG-INFO
--rw-r--r--   0 clavin   (25463) users      (100)      373 2023-05-03 23:18:31.000000 rapidwright-2022.2.3/src/rapidwright.egg-info/SOURCES.txt
--rw-r--r--   0 clavin   (25463) users      (100)        1 2023-05-03 23:18:31.000000 rapidwright-2022.2.3/src/rapidwright.egg-info/dependency_links.txt
--rw-r--r--   0 clavin   (25463) users      (100)       53 2023-05-03 23:18:31.000000 rapidwright-2022.2.3/src/rapidwright.egg-info/entry_points.txt
--rw-r--r--   0 clavin   (25463) users      (100)        1 2023-05-03 23:18:31.000000 rapidwright-2022.2.3/src/rapidwright.egg-info/not-zip-safe
--rw-r--r--   0 clavin   (25463) users      (100)        7 2023-05-03 23:18:31.000000 rapidwright-2022.2.3/src/rapidwright.egg-info/requires.txt
--rw-r--r--   0 clavin   (25463) users      (100)       12 2023-05-03 23:18:31.000000 rapidwright-2022.2.3/src/rapidwright.egg-info/top_level.txt
+drwxr-xr-x   0 clavin   (25463) users      (100)        0 2023-06-01 23:32:32.000000 rapidwright-2023.1.0/
+-rwxr-xr-x   0 clavin   (25463) users      (100)   526323 2023-06-01 23:32:26.000000 rapidwright-2023.1.0/LICENSE.TXT
+-rw-r--r--   0 clavin   (25463) users      (100)     1076 2023-06-01 23:32:32.000000 rapidwright-2023.1.0/PKG-INFO
+-rw-r--r--   0 clavin   (25463) users      (100)     2860 2022-06-08 19:33:55.000000 rapidwright-2023.1.0/README.md
+-rw-r--r--   0 clavin   (25463) users      (100)       78 2023-06-01 23:32:32.000000 rapidwright-2023.1.0/setup.cfg
+-rw-r--r--   0 clavin   (25463) users      (100)     2587 2023-06-01 23:31:18.000000 rapidwright-2023.1.0/setup.py
+drwxr-xr-x   0 clavin   (25463) users      (100)        0 2023-06-01 23:32:32.000000 rapidwright-2023.1.0/src/
+drwxr-xr-x   0 clavin   (25463) users      (100)        0 2023-06-01 23:32:32.000000 rapidwright-2023.1.0/src/rapidwright/
+-rw-r--r--   0 clavin   (25463) users      (100)      883 2022-06-08 19:33:55.000000 rapidwright-2023.1.0/src/rapidwright/__init__.py
+-rw-r--r--   0 clavin   (25463) users      (100)     1839 2023-06-01 21:09:19.000000 rapidwright-2023.1.0/src/rapidwright/rapidwright.py
+drwxr-xr-x   0 clavin   (25463) users      (100)        0 2023-06-01 23:32:32.000000 rapidwright-2023.1.0/src/rapidwright.egg-info/
+-rw-r--r--   0 clavin   (25463) users      (100)     1076 2023-06-01 23:32:32.000000 rapidwright-2023.1.0/src/rapidwright.egg-info/PKG-INFO
+-rw-r--r--   0 clavin   (25463) users      (100)      373 2023-06-01 23:32:32.000000 rapidwright-2023.1.0/src/rapidwright.egg-info/SOURCES.txt
+-rw-r--r--   0 clavin   (25463) users      (100)        1 2023-06-01 23:32:32.000000 rapidwright-2023.1.0/src/rapidwright.egg-info/dependency_links.txt
+-rw-r--r--   0 clavin   (25463) users      (100)       53 2023-06-01 23:32:32.000000 rapidwright-2023.1.0/src/rapidwright.egg-info/entry_points.txt
+-rw-r--r--   0 clavin   (25463) users      (100)        1 2023-06-01 23:32:32.000000 rapidwright-2023.1.0/src/rapidwright.egg-info/not-zip-safe
+-rw-r--r--   0 clavin   (25463) users      (100)        7 2023-06-01 23:32:32.000000 rapidwright-2023.1.0/src/rapidwright.egg-info/requires.txt
+-rw-r--r--   0 clavin   (25463) users      (100)       12 2023-06-01 23:32:32.000000 rapidwright-2023.1.0/src/rapidwright.egg-info/top_level.txt
```

### Comparing `rapidwright-2022.2.3/LICENSE.TXT` & `rapidwright-2023.1.0/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `rapidwright-2022.2.3/PKG-INFO` & `rapidwright-2023.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidwright
-Version: 2022.2.3
+Version: 2023.1.0
 Summary: Xilinx RapidWright Framework Wrapped for Python.
 Home-page: https://github.com/Xilinx/RapidWright
 Author: Chris Lavin
 Author-email: chris.lavin@amd.com
 License: Apache 2.0 and Others
 Project-URL: Changelog, https://github.com/Xilinx/RapidWright/blob/master/RELEASE_NOTES.TXT
 Project-URL: Issue Tracker, https://github.com/Xilinx/RapidWright/issues
```

### Comparing `rapidwright-2022.2.3/README.md` & `rapidwright-2023.1.0/README.md`

 * *Files identical despite different names*

### Comparing `rapidwright-2022.2.3/setup.py` & `rapidwright-2023.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # limitations under the License.
 ################################################################################
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='rapidwright',
-    version='2022.2.3',
+    version='2023.1.0',
     license='Apache 2.0 and Others',
     description='Xilinx RapidWright Framework Wrapped for Python.',
     long_description='',
     author='Chris Lavin',
     author_email='chris.lavin@amd.com',
     url='https://github.com/Xilinx/RapidWright',
     packages=find_packages(where='src'),
```

### Comparing `rapidwright-2022.2.3/src/rapidwright/__init__.py` & `rapidwright-2023.1.0/src/rapidwright/__init__.py`

 * *Files identical despite different names*

### Comparing `rapidwright-2022.2.3/src/rapidwright/rapidwright.py` & `rapidwright-2023.1.0/src/rapidwright/rapidwright.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ################################################################################
 import jpype
 import jpype.imports
 from jpype.types import *
 from typing import List, Optional
 import os, urllib.request, platform
 
-version='2022.2.3'
+version='2023.1.0'
 
 def start_jvm():
     os_str = 'lin64'
     if platform.system() == 'Windows':
         os_str = 'win64'
     kwargs = {}
     if not os.environ.get('RAPIDWRIGHT_PATH'):
```

### Comparing `rapidwright-2022.2.3/src/rapidwright.egg-info/PKG-INFO` & `rapidwright-2023.1.0/src/rapidwright.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidwright
-Version: 2022.2.3
+Version: 2023.1.0
 Summary: Xilinx RapidWright Framework Wrapped for Python.
 Home-page: https://github.com/Xilinx/RapidWright
 Author: Chris Lavin
 Author-email: chris.lavin@amd.com
 License: Apache 2.0 and Others
 Project-URL: Changelog, https://github.com/Xilinx/RapidWright/blob/master/RELEASE_NOTES.TXT
 Project-URL: Issue Tracker, https://github.com/Xilinx/RapidWright/issues
```

