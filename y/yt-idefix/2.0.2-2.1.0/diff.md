# Comparing `tmp/yt_idefix-2.0.2.tar.gz` & `tmp/yt_idefix-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_idefix-2.0.2.tar", last modified: Fri May 26 16:31:28 2023, max compression
+gzip compressed data, was "yt_idefix-2.1.0.tar", last modified: Fri Jun  2 09:37:00 2023, max compression
```

## Comparing `yt_idefix-2.0.2.tar` & `yt_idefix-2.1.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:28.329536 yt_idefix-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 16:31:18.000000 yt_idefix-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-26 16:31:28.329536 yt_idefix-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-05-26 16:31:18.000000 yt_idefix-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-26 16:31:18.000000 yt_idefix-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:31:28.329536 yt_idefix-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:28.329536 yt_idefix-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/tests/test_C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/tests/test_dmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/tests/test_vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/tests/test_xdmf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:28.329536 yt_idefix-2.0.2/yt_idefix/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:28.329536 yt_idefix-2.0.2/yt_idefix/_io/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/_io/C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/_io/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/_io/dmp_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/_io/h5_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/_io/vtk_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34970 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:28.329536 yt_idefix-2.0.2/yt_idefix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-26 16:31:28.000000 yt_idefix-2.0.2/yt_idefix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-26 16:31:28.000000 yt_idefix-2.0.2/yt_idefix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:31:28.000000 yt_idefix-2.0.2/yt_idefix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-26 16:31:28.000000 yt_idefix-2.0.2/yt_idefix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 16:31:28.000000 yt_idefix-2.0.2/yt_idefix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 16:31:28.000000 yt_idefix-2.0.2/yt_idefix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:37:00.050260 yt_idefix-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-02 09:37:00.050260 yt_idefix-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:37:00.050260 yt_idefix-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:37:00.038260 yt_idefix-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:37:00.042260 yt_idefix-2.1.0/src/yt_idefix/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:37:00.046259 yt_idefix-2.1.0/src/yt_idefix/_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/_io/C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/_io/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/_io/dmp_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/_io/h5_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/_io/vtk_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34740 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:37:00.046259 yt_idefix-2.1.0/src/yt_idefix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-02 09:37:00.000000 yt_idefix-2.1.0/src/yt_idefix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-02 09:37:00.000000 yt_idefix-2.1.0/src/yt_idefix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:37:00.000000 yt_idefix-2.1.0/src/yt_idefix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-02 09:37:00.000000 yt_idefix-2.1.0/src/yt_idefix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-02 09:37:00.000000 yt_idefix-2.1.0/src/yt_idefix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:37:00.000000 yt_idefix-2.1.0/src/yt_idefix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:37:00.050260 yt_idefix-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-02 09:36:51.000000 yt_idefix-2.1.0/tests/test_C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-02 09:36:51.000000 yt_idefix-2.1.0/tests/test_dmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-02 09:36:51.000000 yt_idefix-2.1.0/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-06-02 09:36:51.000000 yt_idefix-2.1.0/tests/test_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-02 09:36:51.000000 yt_idefix-2.1.0/tests/test_xdmf.py
```

### Comparing `yt_idefix-2.0.2/LICENSE` & `yt_idefix-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.2/PKG-INFO` & `yt_idefix-2.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: yt_idefix
-Version: 2.0.2
-Summary: An extension module for yt, adding a frontend for Idefix
+Version: 2.1.0
+Summary: An extension module for yt, adding a frontend for Idefix and Pluto
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
 Keywords: astronomy astrophysics visualization amr adaptivemeshrefinement
@@ -55,21 +55,16 @@
 | Idefix | `.dmp` | v0.1.0          |                         |
 | Idefix | `.vtk` | v0.3.0          |                         |
 | Pluto  | `.vtk` | v0.9.0          |                         |
 | Pluto  |  XDMF  | v1.1.0          | `h5py`                  |
 
 ## Usage
 
-After importing `yt` itself, make sure to activate the extension
-```python
-import yt
-import yt_idefix
-```
-
-Now `yt.load` will be able to read Pluto/Idefix output files.
+Integration with yt is seamless. *Installing* this plugin is all that's required to make yt
+compatible with data formats supported by `yt_idefix` !
 
 ### Additional arguments to `yt.load`
 The metadata are parsed from data file, definitions header file and inifile when loading dataset.
 
 Definitions header file (`definitions.h` for Pluto, or `definitions.hpp` for Idefix) and inifile (`pluto.ini` and `idefix.ini` respectively) are discovered automatically if they match default names, are located along with data files, and unique. Otherwise, they can be specified explicitly as paths (either relative to data files or absolute paths) with parameters `definitions_header` and `inifile` respectively.
 
 Geometry is parsed automatically whenever possible, but as a last resort, it can also be specified as a keyword argument (possible values are "cartesian", "spherical", "cylindrical" and "polar").
@@ -120,29 +115,7 @@
 # [('pluto-vtk', 'PRS'),   # standard output
 #  ('pluto-vtk', 'RHO'),   # standard output
 #  ('pluto-vtk', 'VX1'),   # standard output
 #  ('pluto-vtk', 'VX2'),   # standard output
 #  ('pluto-vtk', 'VX3'),   # standard output
 #  ('pluto-vtk', 'temp')]  # This is a user-defined output
 ```
-
-## Experimental features
-
-### Seamless plugin support
-*new in yt 4.2 (unreleased) + yt_idefix 0.16*
-
-`yt>=4.2` supports automatic
-loading for external frontends, i.e., the extra import line (`import yt_idefix`)
-will not be needed with this version.
-
-This feature is marked as experimental until yt 4.2.0 is released.
-In the mean time, this feature can be enabled by installing yt from source as, i.e.,
-```shell
-python -m pip install git+https://github.com/yt-project/yt.git
-```
-
-### Strecthed grids support
-*new in yt 4.1 + yt_idefix 0.12*
-- `yt_idefix>=0.12.0` natively supports `yt.SlicePlot` for streched grids
-- `yt>=4.1.0` is required from `yt.ProjectionPlot`
-
-Streched grids support is considered experimental as of yt 4.1
```

### Comparing `yt_idefix-2.0.2/README.md` & `yt_idefix-2.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -25,21 +25,16 @@
 | Idefix | `.dmp` | v0.1.0          |                         |
 | Idefix | `.vtk` | v0.3.0          |                         |
 | Pluto  | `.vtk` | v0.9.0          |                         |
 | Pluto  |  XDMF  | v1.1.0          | `h5py`                  |
 
 ## Usage
 
-After importing `yt` itself, make sure to activate the extension
-```python
-import yt
-import yt_idefix
-```
-
-Now `yt.load` will be able to read Pluto/Idefix output files.
+Integration with yt is seamless. *Installing* this plugin is all that's required to make yt
+compatible with data formats supported by `yt_idefix` !
 
 ### Additional arguments to `yt.load`
 The metadata are parsed from data file, definitions header file and inifile when loading dataset.
 
 Definitions header file (`definitions.h` for Pluto, or `definitions.hpp` for Idefix) and inifile (`pluto.ini` and `idefix.ini` respectively) are discovered automatically if they match default names, are located along with data files, and unique. Otherwise, they can be specified explicitly as paths (either relative to data files or absolute paths) with parameters `definitions_header` and `inifile` respectively.
 
 Geometry is parsed automatically whenever possible, but as a last resort, it can also be specified as a keyword argument (possible values are "cartesian", "spherical", "cylindrical" and "polar").
@@ -90,29 +85,7 @@
 # [('pluto-vtk', 'PRS'),   # standard output
 #  ('pluto-vtk', 'RHO'),   # standard output
 #  ('pluto-vtk', 'VX1'),   # standard output
 #  ('pluto-vtk', 'VX2'),   # standard output
 #  ('pluto-vtk', 'VX3'),   # standard output
 #  ('pluto-vtk', 'temp')]  # This is a user-defined output
 ```
-
-## Experimental features
-
-### Seamless plugin support
-*new in yt 4.2 (unreleased) + yt_idefix 0.16*
-
-`yt>=4.2` supports automatic
-loading for external frontends, i.e., the extra import line (`import yt_idefix`)
-will not be needed with this version.
-
-This feature is marked as experimental until yt 4.2.0 is released.
-In the mean time, this feature can be enabled by installing yt from source as, i.e.,
-```shell
-python -m pip install git+https://github.com/yt-project/yt.git
-```
-
-### Strecthed grids support
-*new in yt 4.1 + yt_idefix 0.12*
-- `yt_idefix>=0.12.0` natively supports `yt.SlicePlot` for streched grids
-- `yt>=4.1.0` is required from `yt.ProjectionPlot`
-
-Streched grids support is considered experimental as of yt 4.1
```

### Comparing `yt_idefix-2.0.2/pyproject.toml` & `yt_idefix-2.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 requires = [
     "setuptools>=61.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yt_idefix"
-version = "2.0.2"
-description = "An extension module for yt, adding a frontend for Idefix"
+description = "An extension module for yt, adding a frontend for Idefix and Pluto"
 authors = [
     { name = "C.M.T. Robert" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Framework :: Matplotlib",
@@ -30,23 +29,25 @@
 keywords = [
     "astronomy astrophysics visualization amr adaptivemeshrefinement",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "inifix>=4.1.0",
     "numpy>=1.17.3",
-    "yt>=4.1.0",
+    "yt>=4.2.0",
 ]
+dynamic = ["version"]
+
+[tool.setuptools.dynamic]
+version = {attr = "yt_idefix.__version__"}
 
 [project.optional-dependencies]
 HDF5 = ["h5py>=3.1.0"]
 
 [project.entry-points."yt.frontends"]
-# these entry points require yt 4.2 (unreleased at the time of writing)
-# they are included early for testing purposes
 IdefixDmpkDataset = "yt_idefix.api:IdefixDmpDataset"
 IdefixVtkDataset = "yt_idefix.api:IdefixVtkDataset"
 PlutoVtkDataset = "yt_idefix.api:PlutoVtkDataset"
 PlutoXdmfDataset = "yt_idefix.api:PlutoXdmfDataset"
 
 [project.license]
 text = "GPL-3.0"
@@ -69,14 +70,15 @@
 
 [tool.setuptools.package-data]
 yt_idefix = [
     "py.typed",
 ]
 
 [tool.setuptools.packages.find]
+where = ["src"]
 namespaces = false
 
 [tool.ruff]
 exclude = [
     "*/api.py",
     "*/__init__.py",
 ]
@@ -100,15 +102,15 @@
 known-third-party = [
   "numpy",
   "matplotlib",
   "unyt",
   "yaml",
   "pytest",
 ]
-known-first-party = ["yt"]
+known-first-party = ["yt", "yt_idefix"]
 
 [tool.mypy]
 python_version = 3.8
 show_error_codes = true
 warn_unused_configs = true
 warn_unreachable = true
 show_error_context = true
```

### Comparing `yt_idefix-2.0.2/tests/test_C_io.py` & `yt_idefix-2.1.0/tests/test_C_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.2/tests/test_dmp.py` & `yt_idefix-2.1.0/tests/test_dmp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 
 import numpy as np
 from numpy.testing import assert_equal
 
 import yt
-import yt_idefix  # noqa: F401
 from yt_idefix._io.dmp_io import read_idefix_dmpfile
 from yt_idefix.api import IdefixDmpDataset
 
 DATA_DIR = Path(__file__).parent / "data"
 idefix_khi = DATA_DIR.joinpath("khi", "dump.0100.dmp")
```

### Comparing `yt_idefix-2.0.2/tests/test_loading.py` & `yt_idefix-2.1.0/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.2/tests/test_vtk.py` & `yt_idefix-2.1.0/tests/test_vtk.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.2/tests/test_xdmf.py` & `yt_idefix-2.1.0/tests/test_xdmf.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.2/yt_idefix/_backports.py` & `yt_idefix-2.1.0/src/yt_idefix/_backports.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.2/yt_idefix/_io/commons.py` & `yt_idefix-2.1.0/src/yt_idefix/_io/commons.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.2/yt_idefix/_io/dmp_io.py` & `yt_idefix-2.1.0/src/yt_idefix/_io/dmp_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.2/yt_idefix/_io/h5_io.py` & `yt_idefix-2.1.0/src/yt_idefix/_io/h5_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.2/yt_idefix/_io/vtk_io.py` & `yt_idefix-2.1.0/src/yt_idefix/_io/vtk_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.2/yt_idefix/data_structures.py` & `yt_idefix-2.1.0/src/yt_idefix/data_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Final, Literal
 
 import inifix
 import numpy as np
 import numpy.testing as npt
 
-import yt
 from yt.data_objects.index_subobjects.stretched_grid import StretchedGrid
 from yt.data_objects.static_output import Dataset
 from yt.funcs import setdefaultattr
+from yt.geometry.api import Geometry
 from yt.geometry.grid_geometry_handler import GridIndex
 from yt.utilities.lib.misc_utilities import (  # type: ignore [import]
     _obtain_coords_and_widths,
 )
 from yt.utilities.on_demand_imports import _h5py as h5py
 from yt_idefix._backports import removesuffix
 
@@ -419,23 +419,15 @@
                     stacklevel=2,
                 )
             geom_str = from_input
         else:
             assert from_disk
             geom_str = from_disk
 
-        def parse_geometry(geom: str):
-            if yt.version_info >= (4, 2):
-                from yt.geometry.api import Geometry  # type: ignore [attr-defined]
-
-                return Geometry(geom)
-            else:
-                return geom
-
-        self.geometry = parse_geometry(geom_str)
+        self.geometry = Geometry(geom_str)
 
     def _parse_inifile(self) -> None:
         if not self._inifile:
             return
 
         with open(self._inifile, "rb") as fh:
             self.parameters.update(inifix.load(fh))
```

### Comparing `yt_idefix-2.0.2/yt_idefix/definitions.py` & `yt_idefix-2.1.0/src/yt_idefix/definitions.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.2/yt_idefix/fields.py` & `yt_idefix-2.1.0/src/yt_idefix/fields.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.2/yt_idefix/io.py` & `yt_idefix-2.1.0/src/yt_idefix/io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.2/yt_idefix.egg-info/PKG-INFO` & `yt_idefix-2.1.0/src/yt_idefix.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: yt-idefix
-Version: 2.0.2
-Summary: An extension module for yt, adding a frontend for Idefix
+Version: 2.1.0
+Summary: An extension module for yt, adding a frontend for Idefix and Pluto
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
 Keywords: astronomy astrophysics visualization amr adaptivemeshrefinement
@@ -55,21 +55,16 @@
 | Idefix | `.dmp` | v0.1.0          |                         |
 | Idefix | `.vtk` | v0.3.0          |                         |
 | Pluto  | `.vtk` | v0.9.0          |                         |
 | Pluto  |  XDMF  | v1.1.0          | `h5py`                  |
 
 ## Usage
 
-After importing `yt` itself, make sure to activate the extension
-```python
-import yt
-import yt_idefix
-```
-
-Now `yt.load` will be able to read Pluto/Idefix output files.
+Integration with yt is seamless. *Installing* this plugin is all that's required to make yt
+compatible with data formats supported by `yt_idefix` !
 
 ### Additional arguments to `yt.load`
 The metadata are parsed from data file, definitions header file and inifile when loading dataset.
 
 Definitions header file (`definitions.h` for Pluto, or `definitions.hpp` for Idefix) and inifile (`pluto.ini` and `idefix.ini` respectively) are discovered automatically if they match default names, are located along with data files, and unique. Otherwise, they can be specified explicitly as paths (either relative to data files or absolute paths) with parameters `definitions_header` and `inifile` respectively.
 
 Geometry is parsed automatically whenever possible, but as a last resort, it can also be specified as a keyword argument (possible values are "cartesian", "spherical", "cylindrical" and "polar").
@@ -120,29 +115,7 @@
 # [('pluto-vtk', 'PRS'),   # standard output
 #  ('pluto-vtk', 'RHO'),   # standard output
 #  ('pluto-vtk', 'VX1'),   # standard output
 #  ('pluto-vtk', 'VX2'),   # standard output
 #  ('pluto-vtk', 'VX3'),   # standard output
 #  ('pluto-vtk', 'temp')]  # This is a user-defined output
 ```
-
-## Experimental features
-
-### Seamless plugin support
-*new in yt 4.2 (unreleased) + yt_idefix 0.16*
-
-`yt>=4.2` supports automatic
-loading for external frontends, i.e., the extra import line (`import yt_idefix`)
-will not be needed with this version.
-
-This feature is marked as experimental until yt 4.2.0 is released.
-In the mean time, this feature can be enabled by installing yt from source as, i.e.,
-```shell
-python -m pip install git+https://github.com/yt-project/yt.git
-```
-
-### Strecthed grids support
-*new in yt 4.1 + yt_idefix 0.12*
-- `yt_idefix>=0.12.0` natively supports `yt.SlicePlot` for streched grids
-- `yt>=4.1.0` is required from `yt.ProjectionPlot`
-
-Streched grids support is considered experimental as of yt 4.1
```

