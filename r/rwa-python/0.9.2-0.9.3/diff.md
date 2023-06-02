# Comparing `tmp/rwa-python-0.9.2.tar.gz` & `tmp/rwa-python-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwa-python-0.9.2.tar", last modified: Wed May 31 20:27:06 2023, max compression
+gzip compressed data, was "rwa-python-0.9.3.tar", last modified: Fri Jun  2 19:01:29 2023, max compression
```

## Comparing `rwa-python-0.9.2.tar` & `rwa-python-0.9.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 flaurent  (1000) flaurent  (1000)        0 2023-05-31 20:27:06.070110 rwa-python-0.9.2/
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)    11369 2023-05-31 09:33:20.000000 rwa-python-0.9.2/LICENSE
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)     3406 2023-05-31 20:27:06.070110 rwa-python-0.9.2/PKG-INFO
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)     2663 2023-05-31 09:33:20.000000 rwa-python-0.9.2/README.rst
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)      500 2023-05-31 10:36:26.000000 rwa-python-0.9.2/pyproject.toml
-drwxr-xr-x   0 flaurent  (1000) flaurent  (1000)        0 2023-05-31 20:27:06.066110 rwa-python-0.9.2/rwa/
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)      425 2023-05-31 09:33:20.000000 rwa-python-0.9.2/rwa/__init__.py
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)    35975 2023-05-31 19:38:43.000000 rwa-python-0.9.2/rwa/generic.py
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)    15106 2023-05-31 09:33:20.000000 rwa-python-0.9.2/rwa/hdf5.py
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)    10160 2023-05-31 09:33:20.000000 rwa-python-0.9.2/rwa/lazy.py
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)    14199 2023-05-31 11:15:17.000000 rwa-python-0.9.2/rwa/pandas.py
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)     7715 2023-05-31 19:38:43.000000 rwa-python-0.9.2/rwa/scipy.py
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)     9967 2023-05-31 09:33:20.000000 rwa-python-0.9.2/rwa/sequence.py
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)    18539 2023-05-31 09:33:20.000000 rwa-python-0.9.2/rwa/storable.py
-drwxr-xr-x   0 flaurent  (1000) flaurent  (1000)        0 2023-05-31 20:27:06.066110 rwa-python-0.9.2/rwa_python.egg-info/
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)     3406 2023-05-31 20:27:06.000000 rwa-python-0.9.2/rwa_python.egg-info/PKG-INFO
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)      422 2023-05-31 20:27:06.000000 rwa-python-0.9.2/rwa_python.egg-info/SOURCES.txt
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)        1 2023-05-31 20:27:06.000000 rwa-python-0.9.2/rwa_python.egg-info/dependency_links.txt
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)       28 2023-05-31 20:27:06.000000 rwa-python-0.9.2/rwa_python.egg-info/requires.txt
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)        4 2023-05-31 20:27:06.000000 rwa-python-0.9.2/rwa_python.egg-info/top_level.txt
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)       38 2023-05-31 20:27:06.070110 rwa-python-0.9.2/setup.cfg
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)     1521 2023-05-31 19:39:28.000000 rwa-python-0.9.2/setup.py
-drwxr-xr-x   0 flaurent  (1000) flaurent  (1000)        0 2023-05-31 20:27:06.070110 rwa-python-0.9.2/tests/
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)     2729 2023-05-31 09:33:20.000000 rwa-python-0.9.2/tests/test_autoserial_hdf5.py
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)     4288 2023-05-31 09:33:20.000000 rwa-python-0.9.2/tests/test_native_hdf5.py
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)     9146 2023-05-31 19:59:27.000000 rwa-python-0.9.2/tests/test_pandas.py
--rw-r--r--   0 flaurent  (1000) flaurent  (1000)     3904 2023-05-31 11:43:58.000000 rwa-python-0.9.2/tests/test_scipy.py
+drwxr-xr-x   0 flaurent  (1000) flaurent  (1000)        0 2023-06-02 19:01:29.661096 rwa-python-0.9.3/
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)    11369 2023-05-31 09:33:20.000000 rwa-python-0.9.3/LICENSE
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     3406 2023-06-02 19:01:29.661096 rwa-python-0.9.3/PKG-INFO
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     2663 2023-05-31 09:33:20.000000 rwa-python-0.9.3/README.rst
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)      485 2023-06-02 18:41:48.000000 rwa-python-0.9.3/pyproject.toml
+drwxr-xr-x   0 flaurent  (1000) flaurent  (1000)        0 2023-06-02 19:01:29.661096 rwa-python-0.9.3/rwa/
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)      425 2023-05-31 09:33:20.000000 rwa-python-0.9.3/rwa/__init__.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)    35975 2023-05-31 19:38:43.000000 rwa-python-0.9.3/rwa/generic.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)    15106 2023-05-31 09:33:20.000000 rwa-python-0.9.3/rwa/hdf5.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)    10160 2023-05-31 09:33:20.000000 rwa-python-0.9.3/rwa/lazy.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)    14237 2023-06-02 18:36:44.000000 rwa-python-0.9.3/rwa/pandas.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     7715 2023-05-31 19:38:43.000000 rwa-python-0.9.3/rwa/scipy.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     9967 2023-05-31 09:33:20.000000 rwa-python-0.9.3/rwa/sequence.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)    18539 2023-05-31 09:33:20.000000 rwa-python-0.9.3/rwa/storable.py
+drwxr-xr-x   0 flaurent  (1000) flaurent  (1000)        0 2023-06-02 19:01:29.661096 rwa-python-0.9.3/rwa_python.egg-info/
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     3406 2023-06-02 19:01:29.000000 rwa-python-0.9.3/rwa_python.egg-info/PKG-INFO
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)      422 2023-06-02 19:01:29.000000 rwa-python-0.9.3/rwa_python.egg-info/SOURCES.txt
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)        1 2023-06-02 19:01:29.000000 rwa-python-0.9.3/rwa_python.egg-info/dependency_links.txt
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)       28 2023-06-02 19:01:29.000000 rwa-python-0.9.3/rwa_python.egg-info/requires.txt
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)        4 2023-06-02 19:01:29.000000 rwa-python-0.9.3/rwa_python.egg-info/top_level.txt
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)       38 2023-06-02 19:01:29.661096 rwa-python-0.9.3/setup.cfg
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     1521 2023-06-02 18:42:02.000000 rwa-python-0.9.3/setup.py
+drwxr-xr-x   0 flaurent  (1000) flaurent  (1000)        0 2023-06-02 19:01:29.661096 rwa-python-0.9.3/tests/
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     2729 2023-05-31 09:33:20.000000 rwa-python-0.9.3/tests/test_autoserial_hdf5.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     4288 2023-05-31 09:33:20.000000 rwa-python-0.9.3/tests/test_native_hdf5.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     9146 2023-05-31 19:59:27.000000 rwa-python-0.9.3/tests/test_pandas.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     3904 2023-05-31 11:43:58.000000 rwa-python-0.9.3/tests/test_scipy.py
```

### Comparing `rwa-python-0.9.2/LICENSE` & `rwa-python-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.2/PKG-INFO` & `rwa-python-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwa-python
-Version: 0.9.2
+Version: 0.9.3
 Summary: HDF5-based serialization library for Python datatypes
 Home-page: https://github.com/DecBayComp/RWA-python
 Author: François Laurent
 Author-email: francois.laurent@pasteur.fr
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rwa-python-0.9.2/README.rst` & `rwa-python-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.2/rwa/generic.py` & `rwa-python-0.9.3/rwa/generic.py`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.2/rwa/hdf5.py` & `rwa-python-0.9.3/rwa/hdf5.py`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.2/rwa/lazy.py` & `rwa-python-0.9.3/rwa/lazy.py`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.2/rwa/pandas.py` & `rwa-python-0.9.3/rwa/pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 from __future__ import absolute_import
 
 from .generic import *
 import warnings
 import sys
+import numpy as np
 
 class Python35Warning(DeprecationWarning):
     pass
 
 warnings.filterwarnings("ignore", category=FutureWarning, module="rwa.pandas")
 
 
@@ -159,15 +160,15 @@
         # convert Int64Index into Index
         class pandas_Int64Index(object):
             """
             Placeholder type.
             """
             __slot__ = ()
             pass
-        peek_int64index = peek_numerical_index(pandas.Index, lambda a: a.astype(np.int64))
+        peek_int64index = peek_numerical_index(pandas.Index, lambda a: np.asarray(a).astype(np.int64))
 
     try:
         # UInt64Index is missing in 0.17.1
         pandas_UInt64Index = pandas.UInt64Index
         peek_uint64index = peek_numerical_index(pandas.UInt64Index)
     except AttributeError:
         # convert UInt64 into Int64
@@ -187,15 +188,15 @@
         # convert Float64Index into Index
         class pandas_Float64Index(object):
             """
             Placeholder type.
             """
             __slot__ = ()
             pass
-        peek_float64index = peek_numerical_index(pandas.Index, lambda a: a.astype(np.float64))
+        peek_float64index = peek_numerical_index(pandas.Index, lambda a: np.asarray(a).astype(np.float64))
 
     if True:
         poke_rangeindex = poke([('start','_start'), ('stop','_stop'), ('step','_step'), 'name'])
     else:
         poke_rangeindex = poke(['_start', '_stop', '_step', 'name'])
     try:
         # RangeIndex is missing in 0.17.1
@@ -220,15 +221,15 @@
             """
             Placeholder type.
             """
             __slot__ = ()
             pass
         def peek_rangeindex(*args, **kwargs):
             attrs = peek_as_dict(*args, **kwargs)
-            return pandas.Int64Index( \
+            return pandas.Index( \
                 range( \
                     attrs.pop('_start', None), \
                     attrs.pop('_stop', None), \
                     attrs.pop('_step', None)), \
                 **attrs)
 
     # some Pandas types have moved several times; force the key
```

### Comparing `rwa-python-0.9.2/rwa/scipy.py` & `rwa-python-0.9.3/rwa/scipy.py`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.2/rwa/sequence.py` & `rwa-python-0.9.3/rwa/sequence.py`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.2/rwa/storable.py` & `rwa-python-0.9.3/rwa/storable.py`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.2/rwa_python.egg-info/PKG-INFO` & `rwa-python-0.9.3/rwa_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwa-python
-Version: 0.9.2
+Version: 0.9.3
 Summary: HDF5-based serialization library for Python datatypes
 Home-page: https://github.com/DecBayComp/RWA-python
 Author: François Laurent
 Author-email: francois.laurent@pasteur.fr
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rwa-python-0.9.2/setup.py` & `rwa-python-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     with open(os.path.join(pwd, 'README.rst'), encoding='utf-8') as f:
         long_description = f.read()
 except OSError:
     long_description = ''
 
 setup(
     name = 'rwa-python',
-    version = '0.9.2',
+    version = '0.9.3',
     description = 'HDF5-based serialization library for Python datatypes',
     long_description = long_description,
     url = 'https://github.com/DecBayComp/RWA-python',
     author = 'François Laurent',
     author_email = 'francois.laurent@pasteur.fr',
     license = 'Apache 2.0',
     classifiers = [
```

### Comparing `rwa-python-0.9.2/tests/test_autoserial_hdf5.py` & `rwa-python-0.9.3/tests/test_autoserial_hdf5.py`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.2/tests/test_native_hdf5.py` & `rwa-python-0.9.3/tests/test_native_hdf5.py`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.2/tests/test_pandas.py` & `rwa-python-0.9.3/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.2/tests/test_scipy.py` & `rwa-python-0.9.3/tests/test_scipy.py`

 * *Files identical despite different names*

