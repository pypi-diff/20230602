# Comparing `tmp/odb-plotter-0.5.2.tar.gz` & `tmp/odb-plotter-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odb-plotter-0.5.2.tar", last modified: Fri Jun  2 02:04:47 2023, max compression
+gzip compressed data, was "odb-plotter-0.5.3.tar", last modified: Fri Jun  2 17:24:04 2023, max compression
```

## Comparing `odb-plotter-0.5.2.tar` & `odb-plotter-0.5.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 02:04:47.306397 odb-plotter-0.5.2/
--rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-05-25 14:12:43.000000 odb-plotter-0.5.2/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)     3495 2023-06-02 02:04:47.306397 odb-plotter-0.5.2/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)     1570 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)     1194 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-02 02:04:47.306397 odb-plotter-0.5.2/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 02:04:47.303064 odb-plotter-0.5.2/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 02:04:47.303064 odb-plotter-0.5.2/src/odb_plotter.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)     3495 2023-06-02 02:04:47.000000 odb-plotter-0.5.2/src/odb_plotter.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      525 2023-06-02 02:04:47.000000 odb-plotter-0.5.2/src/odb_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-02 02:04:47.000000 odb-plotter-0.5.2/src/odb_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)      144 2023-06-02 02:04:47.000000 odb-plotter-0.5.2/src/odb_plotter.egg-info/requires.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-02 02:04:47.000000 odb-plotter-0.5.2/src/odb_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 02:04:47.306397 odb-plotter-0.5.2/src/odbp/
--rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/__init__.py
--rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.5.2/src/odbp/__main__.py
--rw-r--r--   0 clark     (1000) clark     (1000)    24794 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/cli.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 02:04:47.306397 odb-plotter-0.5.2/src/odbp/data/
--rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.5.2/src/odbp/data/config.toml
--rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.5.2/src/odbp/data/views.toml
--rw-r--r--   0 clark     (1000) clark     (1000)     3964 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/npz_to_hdf.py
--rw-r--r--   0 clark     (1000) clark     (1000)    17381 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/odb.py
--rw-r--r--   0 clark     (1000) clark     (1000)     4832 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/odb_visualizer.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 02:04:47.306397 odb-plotter-0.5.2/src/odbp/py2_scripts/
--rw-r--r--   0 clark     (1000) clark     (1000)     6349 2023-05-25 14:12:43.000000 odb-plotter-0.5.2/src/odbp/py2_scripts/extract.py
--rw-r--r--   0 clark     (1000) clark     (1000)     7194 2023-06-01 00:43:21.000000 odb-plotter-0.5.2/src/odbp/py2_scripts/odb_to_npz.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2354 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/read_hdf5.py
--rw-r--r--   0 clark     (1000) clark     (1000)    28791 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/state.py
--rw-r--r--   0 clark     (1000) clark     (1000)     1925 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/util.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 17:24:04.418469 odb-plotter-0.5.3/
+-rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.5.3/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)     3535 2023-06-02 17:24:04.418469 odb-plotter-0.5.3/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)     1610 2023-06-02 17:23:51.000000 odb-plotter-0.5.3/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)     1194 2023-06-02 17:21:42.000000 odb-plotter-0.5.3/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-02 17:24:04.418469 odb-plotter-0.5.3/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 17:24:04.415136 odb-plotter-0.5.3/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 17:24:04.418469 odb-plotter-0.5.3/src/odb_plotter.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)     3535 2023-06-02 17:24:04.000000 odb-plotter-0.5.3/src/odb_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      525 2023-06-02 17:24:04.000000 odb-plotter-0.5.3/src/odb_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-02 17:24:04.000000 odb-plotter-0.5.3/src/odb_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)      144 2023-06-02 17:24:04.000000 odb-plotter-0.5.3/src/odb_plotter.egg-info/requires.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-02 17:24:04.000000 odb-plotter-0.5.3/src/odb_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 17:24:04.418469 odb-plotter-0.5.3/src/odbp/
+-rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-02 17:23:51.000000 odb-plotter-0.5.3/src/odbp/__init__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.5.3/src/odbp/__main__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    24794 2023-06-02 17:21:42.000000 odb-plotter-0.5.3/src/odbp/cli.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 17:24:04.418469 odb-plotter-0.5.3/src/odbp/data/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.5.3/src/odbp/data/config.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.5.3/src/odbp/data/views.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)     3964 2023-06-02 17:21:42.000000 odb-plotter-0.5.3/src/odbp/npz_to_hdf.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    17386 2023-06-02 17:23:51.000000 odb-plotter-0.5.3/src/odbp/odb.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     4832 2023-06-02 17:21:42.000000 odb-plotter-0.5.3/src/odbp/odb_visualizer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 17:24:04.418469 odb-plotter-0.5.3/src/odbp/py2_scripts/
+-rw-r--r--   0 clark     (1000) clark     (1000)     6349 2023-05-25 14:12:43.000000 odb-plotter-0.5.3/src/odbp/py2_scripts/extract.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     7194 2023-06-01 00:43:21.000000 odb-plotter-0.5.3/src/odbp/py2_scripts/odb_to_npz.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2354 2023-06-02 17:21:42.000000 odb-plotter-0.5.3/src/odbp/read_hdf5.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    28791 2023-06-02 17:21:42.000000 odb-plotter-0.5.3/src/odbp/state.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     1925 2023-06-02 17:21:42.000000 odb-plotter-0.5.3/src/odbp/util.py
```

### Comparing `odb-plotter-0.5.2/LICENSE` & `odb-plotter-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.2/PKG-INFO` & `odb-plotter-0.5.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -59,16 +59,17 @@
 ### I intend for this project to serve two purposes:
 - First, implement an extensible, flexible api for accessing data within .odb files or .hdf5 files with odb data
 - Second, implement a user-friendly, sane-defaults cli to allow for quick data extraction, manipulation, and visualization with no hassle
 
 ## Changelog
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
-    * 0.5.1 Implement new system information (pypi tags, this changelog)
-    * 0.5.2 Returning support to Python 3.8+ (type hinting)
+    * 0.5.1: Implement new system information (pypi tags, this changelog)
+    * 0.5.2: Returning support to Python 3.8+ (type hinting)
+    * 0.5.3: Patching conversion bugs
 * Upcoming:
     * 0.6.0: Improved extractor across all file types. Improved Odb object iteration.
     * 0.7.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline
     * 0.8.0: Parametrize input values such as nodes, nodesets, frames, steps, parts, and colors (both in the API and CLI).
     * 0.9.0: Create two-dimensional plotting capabilities and sane defaults.
     * 0.10.0: Improve PyVista: views, gifs, non-interactive image saving, leaving viewer, etc. Ensure functionality of Abaqus 2019
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding (or following) a publication.
```

### Comparing `odb-plotter-0.5.2/README.md` & `odb-plotter-0.5.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 ### I intend for this project to serve two purposes:
 - First, implement an extensible, flexible api for accessing data within .odb files or .hdf5 files with odb data
 - Second, implement a user-friendly, sane-defaults cli to allow for quick data extraction, manipulation, and visualization with no hassle
 
 ## Changelog
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
-    * 0.5.1 Implement new system information (pypi tags, this changelog)
-    * 0.5.2 Returning support to Python 3.8+ (type hinting)
+    * 0.5.1: Implement new system information (pypi tags, this changelog)
+    * 0.5.2: Returning support to Python 3.8+ (type hinting)
+    * 0.5.3: Patching conversion bugs
 * Upcoming:
     * 0.6.0: Improved extractor across all file types. Improved Odb object iteration.
     * 0.7.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline
     * 0.8.0: Parametrize input values such as nodes, nodesets, frames, steps, parts, and colors (both in the API and CLI).
     * 0.9.0: Create two-dimensional plotting capabilities and sane defaults.
     * 0.10.0: Improve PyVista: views, gifs, non-interactive image saving, leaving viewer, etc. Ensure functionality of Abaqus 2019
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding (or following) a publication.
```

### Comparing `odb-plotter-0.5.2/pyproject.toml` & `odb-plotter-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.2/src/odb_plotter.egg-info/PKG-INFO` & `odb-plotter-0.5.3/src/odb_plotter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -59,16 +59,17 @@
 ### I intend for this project to serve two purposes:
 - First, implement an extensible, flexible api for accessing data within .odb files or .hdf5 files with odb data
 - Second, implement a user-friendly, sane-defaults cli to allow for quick data extraction, manipulation, and visualization with no hassle
 
 ## Changelog
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
-    * 0.5.1 Implement new system information (pypi tags, this changelog)
-    * 0.5.2 Returning support to Python 3.8+ (type hinting)
+    * 0.5.1: Implement new system information (pypi tags, this changelog)
+    * 0.5.2: Returning support to Python 3.8+ (type hinting)
+    * 0.5.3: Patching conversion bugs
 * Upcoming:
     * 0.6.0: Improved extractor across all file types. Improved Odb object iteration.
     * 0.7.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline
     * 0.8.0: Parametrize input values such as nodes, nodesets, frames, steps, parts, and colors (both in the API and CLI).
     * 0.9.0: Create two-dimensional plotting capabilities and sane defaults.
     * 0.10.0: Improve PyVista: views, gifs, non-interactive image saving, leaving viewer, etc. Ensure functionality of Abaqus 2019
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding (or following) a publication.
```

### Comparing `odb-plotter-0.5.2/src/odb_plotter.egg-info/SOURCES.txt` & `odb-plotter-0.5.3/src/odb_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.2/src/odbp/cli.py` & `odb-plotter-0.5.3/src/odbp/cli.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.2/src/odbp/data/config.toml` & `odb-plotter-0.5.3/src/odbp/data/config.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.2/src/odbp/npz_to_hdf.py` & `odb-plotter-0.5.3/src/odbp/npz_to_hdf.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.2/src/odbp/odb.py` & `odb-plotter-0.5.3/src/odbp/odb.py`

 * *Files 0% similar despite different names*

```diff
@@ -561,15 +561,15 @@
             }
         pickle_file: TextIO
         with open(
             self._odb_to_npz_conversion_pickle_path, "wb") as pickle_file:
             pickle.dump(odb_to_npz_pickle_input_dict, pickle_file, protocol=2)
 
         odb_convert_args: List[Union[pathlib.Path, str]]  = [
-            abaqus_executable,
+            self.abaqus_executable,
             "python",
             self._odb_to_npz_script_path,
             odb_path,
             self._odb_to_npz_conversion_pickle_path,
             self._npz_result_path
         ]
```

### Comparing `odb-plotter-0.5.2/src/odbp/odb_visualizer.py` & `odb-plotter-0.5.3/src/odbp/odb_visualizer.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.2/src/odbp/py2_scripts/extract.py` & `odb-plotter-0.5.3/src/odbp/py2_scripts/extract.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.2/src/odbp/py2_scripts/odb_to_npz.py` & `odb-plotter-0.5.3/src/odbp/py2_scripts/odb_to_npz.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.2/src/odbp/read_hdf5.py` & `odb-plotter-0.5.3/src/odbp/read_hdf5.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.2/src/odbp/state.py` & `odb-plotter-0.5.3/src/odbp/state.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.2/src/odbp/util.py` & `odb-plotter-0.5.3/src/odbp/util.py`

 * *Files identical despite different names*

