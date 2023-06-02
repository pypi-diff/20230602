# Comparing `tmp/ndtiff-2.0.0.tar.gz` & `tmp/ndtiff-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndtiff-2.0.0.tar", last modified: Fri May  5 18:40:50 2023, max compression
+gzip compressed data, was "ndtiff-2.0.1.tar", last modified: Fri Jun  2 21:18:31 2023, max compression
```

## Comparing `ndtiff-2.0.0.tar` & `ndtiff-2.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:40:50.313797 ndtiff-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-05 18:40:50.313797 ndtiff-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-05 18:40:39.000000 ndtiff-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:40:50.313797 ndtiff-2.0.0/ndtiff/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/_superclass.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/nd_tiff_current.py
--rw-r--r--   0 runner    (1001) docker     (123)    28211 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/nd_tiff_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    44915 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/ndtiff_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:40:50.313797 ndtiff-2.0.0/ndtiff/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/test/data_loading_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/test/test_custom_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:40:50.313797 ndtiff-2.0.0/ndtiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-05 18:40:50.000000 ndtiff-2.0.0/ndtiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-05 18:40:50.000000 ndtiff-2.0.0/ndtiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:40:50.000000 ndtiff-2.0.0/ndtiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 18:40:50.000000 ndtiff-2.0.0/ndtiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 18:40:50.000000 ndtiff-2.0.0/ndtiff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-05 18:40:39.000000 ndtiff-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 18:40:50.313797 ndtiff-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-05 18:40:39.000000 ndtiff-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:18:31.840706 ndtiff-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-02 21:18:31.840706 ndtiff-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 21:18:15.000000 ndtiff-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:18:31.836706 ndtiff-2.0.1/ndtiff/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/_superclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42655 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/nd_tiff_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28211 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/nd_tiff_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44915 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/ndtiff_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:18:31.840706 ndtiff-2.0.1/ndtiff/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/test/data_loading_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-02 21:18:15.000000 ndtiff-2.0.1/ndtiff/test/test_custom_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:18:31.840706 ndtiff-2.0.1/ndtiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-02 21:18:31.000000 ndtiff-2.0.1/ndtiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-02 21:18:31.000000 ndtiff-2.0.1/ndtiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:18:31.000000 ndtiff-2.0.1/ndtiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 21:18:31.000000 ndtiff-2.0.1/ndtiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 21:18:31.000000 ndtiff-2.0.1/ndtiff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-02 21:18:15.000000 ndtiff-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 21:18:31.840706 ndtiff-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-02 21:18:15.000000 ndtiff-2.0.1/setup.py
```

### Comparing `ndtiff-2.0.0/PKG-INFO` & `ndtiff-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndtiff
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python libraries for NDTiff datasets
 Home-page: https://github.com/micro-manager/NDTiffStorage
 Author: Henry Pinkard
 Author-email: henry.pinkard@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ndtiff-2.0.0/ndtiff/_superclass.py` & `ndtiff-2.0.1/ndtiff/_superclass.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.0.0/ndtiff/file_io.py` & `ndtiff-2.0.1/ndtiff/file_io.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.0.0/ndtiff/nd_tiff_current.py` & `ndtiff-2.0.1/ndtiff/nd_tiff_current.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import json
 import dask.array as da
 import warnings
 import struct
 import threading
 from functools import partial
 from ndtiff.file_io import NDTiffFileIO, BUILTIN_FILE_IO
+import time
 
 _POSITION_AXIS = "position"
 _ROW_AXIS = "row"
 _COLUMN_AXIS = "column"
 _Z_AXIS = "z"
 _TIME_AXIS = "time"
 _CHANNEL_AXIS = "channel"
@@ -424,15 +425,15 @@
                 if axis_name not in self.axes.keys():
                     self.axes[axis_name] = []
                     self.axes_types[axis_name] = type(axes[axis_name])
                 self.axes[axis_name].append(axes[axis_name])
                 self.axes[axis_name] = sorted(list(set(self.axes[axis_name])))
 
             # update the map of channel names to channel indices
-            self._parse_string_axes()
+            self._parse_string_axes(axes)
 
         if not hasattr(self, 'image_width'):
             self._parse_first_index(index_entry)
 
         return axes
 
     def _consolidate_axes(self, channel: int or str, z: int, position: int,
@@ -452,29 +453,32 @@
         for axis_name in axis_positions.keys():
             # convert any string-valued axes passed as ints into strings
             if self.axes_types[axis_name] == str and type(axis_positions[axis_name]) == int:
                 axis_positions[axis_name] = self._string_axes_values[axis_name][axis_positions[axis_name]]
 
         return axis_positions
 
-    def _parse_string_axes(self):
+    def _parse_string_axes(self, axes=None):
         """
         As of NDTiff 3.2, axes are allowed to take string values: e.g. {'channel': 'DAPI'}
         This is allowed on any axis. This function returns a tuple of possible values along
         the string axis in order to be able to interconvert integer values and string values.
+
+        param axes: if not None, only parse the string axis values for the given axes
         """
         # iterate through the key_combos for each image
         if self.major_version >= 3 and self.minor_version >= 2:
             self._string_axes_values = {axis_name: [] for axis_name in self.axes_types.keys()
                                         if self.axes_types[axis_name] is str}
-            for key in self.index.keys():
+            for key in self.index.keys() if axes is None else [[(key, axes[key]) for key in axes.keys()]]:
                 for axis_name, position in key:
                     if axis_name in self._string_axes_values.keys() and \
                             position not in self._string_axes_values[axis_name]:
                         self._string_axes_values[axis_name].append(position)
+
             if _CHANNEL_AXIS in self._string_axes_values:
                 self._channels = {name: self._string_axes_values[_CHANNEL_AXIS].index(name)
                                   for name in self._string_axes_values[_CHANNEL_AXIS]}
         else:
             # before string-valued axes were allowed in NDTiff 3.1
             if 'ChNames' in self.summary_metadata:
                 # It was created by a MM MDA/Clojure acquistiion engine
```

### Comparing `ndtiff-2.0.0/ndtiff/nd_tiff_v2.py` & `ndtiff-2.0.1/ndtiff/nd_tiff_v2.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.0.0/ndtiff/ndtiff_v1.py` & `ndtiff-2.0.1/ndtiff/ndtiff_v1.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.0.0/ndtiff/test/data_loading_test.py` & `ndtiff-2.0.1/ndtiff/test/data_loading_test.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.0.0/ndtiff/test/test_custom_io.py` & `ndtiff-2.0.1/ndtiff/test/test_custom_io.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.0.0/ndtiff.egg-info/PKG-INFO` & `ndtiff-2.0.1/ndtiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndtiff
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python libraries for NDTiff datasets
 Home-page: https://github.com/micro-manager/NDTiffStorage
 Author: Henry Pinkard
 Author-email: henry.pinkard@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ndtiff-2.0.0/setup.py` & `ndtiff-2.0.1/setup.py`

 * *Files identical despite different names*

