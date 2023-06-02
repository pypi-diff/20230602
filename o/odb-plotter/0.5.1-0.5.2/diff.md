# Comparing `tmp/odb-plotter-0.5.1.tar.gz` & `tmp/odb-plotter-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odb-plotter-0.5.1.tar", last modified: Thu Jun  1 01:15:51 2023, max compression
+gzip compressed data, was "odb-plotter-0.5.2.tar", last modified: Fri Jun  2 02:04:47 2023, max compression
```

## Comparing `odb-plotter-0.5.1.tar` & `odb-plotter-0.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-01 01:15:51.616334 odb-plotter-0.5.1/
--rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-05-25 14:12:43.000000 odb-plotter-0.5.1/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)     3435 2023-06-01 01:15:51.616334 odb-plotter-0.5.1/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)     1510 2023-06-01 01:13:26.000000 odb-plotter-0.5.1/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)     1339 2023-06-01 01:13:26.000000 odb-plotter-0.5.1/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-01 01:15:51.616334 odb-plotter-0.5.1/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-01 01:15:51.616334 odb-plotter-0.5.1/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-01 01:15:51.616334 odb-plotter-0.5.1/src/odb_plotter.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)     3435 2023-06-01 01:15:51.000000 odb-plotter-0.5.1/src/odb_plotter.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      525 2023-06-01 01:15:51.000000 odb-plotter-0.5.1/src/odb_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-01 01:15:51.000000 odb-plotter-0.5.1/src/odb_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)      195 2023-06-01 01:15:51.000000 odb-plotter-0.5.1/src/odb_plotter.egg-info/requires.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-01 01:15:51.000000 odb-plotter-0.5.1/src/odb_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-01 01:15:51.616334 odb-plotter-0.5.1/src/odbp/
--rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-01 01:15:43.000000 odb-plotter-0.5.1/src/odbp/__init__.py
--rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.5.1/src/odbp/__main__.py
--rw-r--r--   0 clark     (1000) clark     (1000)    24734 2023-06-01 00:43:21.000000 odb-plotter-0.5.1/src/odbp/cli.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-01 01:15:51.616334 odb-plotter-0.5.1/src/odbp/data/
--rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.5.1/src/odbp/data/config.toml
--rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.5.1/src/odbp/data/views.toml
--rw-r--r--   0 clark     (1000) clark     (1000)     3883 2023-06-01 00:43:21.000000 odb-plotter-0.5.1/src/odbp/npz_to_hdf.py
--rw-r--r--   0 clark     (1000) clark     (1000)    17191 2023-06-01 00:43:21.000000 odb-plotter-0.5.1/src/odbp/odb.py
--rw-r--r--   0 clark     (1000) clark     (1000)     4778 2023-06-01 00:43:21.000000 odb-plotter-0.5.1/src/odbp/odb_visualizer.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-01 01:15:51.616334 odb-plotter-0.5.1/src/odbp/py2_scripts/
--rw-r--r--   0 clark     (1000) clark     (1000)     6349 2023-05-25 14:12:43.000000 odb-plotter-0.5.1/src/odbp/py2_scripts/extract.py
--rw-r--r--   0 clark     (1000) clark     (1000)     7194 2023-06-01 00:43:21.000000 odb-plotter-0.5.1/src/odbp/py2_scripts/odb_to_npz.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2325 2023-06-01 00:43:21.000000 odb-plotter-0.5.1/src/odbp/read_hdf5.py
--rw-r--r--   0 clark     (1000) clark     (1000)    28772 2023-06-01 00:43:21.000000 odb-plotter-0.5.1/src/odbp/state.py
--rw-r--r--   0 clark     (1000) clark     (1000)     1576 2023-06-01 00:43:21.000000 odb-plotter-0.5.1/src/odbp/util.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 02:04:47.306397 odb-plotter-0.5.2/
+-rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-05-25 14:12:43.000000 odb-plotter-0.5.2/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)     3495 2023-06-02 02:04:47.306397 odb-plotter-0.5.2/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)     1570 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)     1194 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-02 02:04:47.306397 odb-plotter-0.5.2/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 02:04:47.303064 odb-plotter-0.5.2/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 02:04:47.303064 odb-plotter-0.5.2/src/odb_plotter.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)     3495 2023-06-02 02:04:47.000000 odb-plotter-0.5.2/src/odb_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      525 2023-06-02 02:04:47.000000 odb-plotter-0.5.2/src/odb_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-02 02:04:47.000000 odb-plotter-0.5.2/src/odb_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)      144 2023-06-02 02:04:47.000000 odb-plotter-0.5.2/src/odb_plotter.egg-info/requires.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-02 02:04:47.000000 odb-plotter-0.5.2/src/odb_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 02:04:47.306397 odb-plotter-0.5.2/src/odbp/
+-rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/__init__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.5.2/src/odbp/__main__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    24794 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/cli.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 02:04:47.306397 odb-plotter-0.5.2/src/odbp/data/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.5.2/src/odbp/data/config.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.5.2/src/odbp/data/views.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)     3964 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/npz_to_hdf.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    17381 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/odb.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     4832 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/odb_visualizer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-02 02:04:47.306397 odb-plotter-0.5.2/src/odbp/py2_scripts/
+-rw-r--r--   0 clark     (1000) clark     (1000)     6349 2023-05-25 14:12:43.000000 odb-plotter-0.5.2/src/odbp/py2_scripts/extract.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     7194 2023-06-01 00:43:21.000000 odb-plotter-0.5.2/src/odbp/py2_scripts/odb_to_npz.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2354 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/read_hdf5.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    28791 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/state.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     1925 2023-06-02 02:04:31.000000 odb-plotter-0.5.2/src/odbp/util.py
```

### Comparing `odb-plotter-0.5.1/LICENSE` & `odb-plotter-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.1/PKG-INFO` & `odb-plotter-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -60,14 +60,15 @@
 - First, implement an extensible, flexible api for accessing data within .odb files or .hdf5 files with odb data
 - Second, implement a user-friendly, sane-defaults cli to allow for quick data extraction, manipulation, and visualization with no hassle
 
 ## Changelog
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1 Implement new system information (pypi tags, this changelog)
+    * 0.5.2 Returning support to Python 3.8+ (type hinting)
 * Upcoming:
     * 0.6.0: Improved extractor across all file types. Improved Odb object iteration.
     * 0.7.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline
     * 0.8.0: Parametrize input values such as nodes, nodesets, frames, steps, parts, and colors (both in the API and CLI).
     * 0.9.0: Create two-dimensional plotting capabilities and sane defaults.
     * 0.10.0: Improve PyVista: views, gifs, non-interactive image saving, leaving viewer, etc. Ensure functionality of Abaqus 2019
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding (or following) a publication.
```

### Comparing `odb-plotter-0.5.1/README.md` & `odb-plotter-0.5.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 - First, implement an extensible, flexible api for accessing data within .odb files or .hdf5 files with odb data
 - Second, implement a user-friendly, sane-defaults cli to allow for quick data extraction, manipulation, and visualization with no hassle
 
 ## Changelog
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1 Implement new system information (pypi tags, this changelog)
+    * 0.5.2 Returning support to Python 3.8+ (type hinting)
 * Upcoming:
     * 0.6.0: Improved extractor across all file types. Improved Odb object iteration.
     * 0.7.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline
     * 0.8.0: Parametrize input values such as nodes, nodesets, frames, steps, parts, and colors (both in the API and CLI).
     * 0.9.0: Create two-dimensional plotting capabilities and sane defaults.
     * 0.10.0: Improve PyVista: views, gifs, non-interactive image saving, leaving viewer, etc. Ensure functionality of Abaqus 2019
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding (or following) a publication.
```

### Comparing `odb-plotter-0.5.1/pyproject.toml` & `odb-plotter-0.5.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 "platformdirs",
 "h5py",
 "numpy",
 "tomli>=1.1.0; python_version < '3.11'",
 "tomli_w",
 "pandas",
 "matplotlib",
-"vtk==9.2.2; python_version < '3.11'", # pyvista is unstable on some platforms with vtk 9.2.5 or greater
-"vtk==9.2.4; python_version >= '3.11'",
 "pyreadline3; platform_system == 'Windows'",
 "pyvista",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://www.cmml.me.msstate.edu"
```

### Comparing `odb-plotter-0.5.1/src/odb_plotter.egg-info/PKG-INFO` & `odb-plotter-0.5.2/src/odb_plotter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -60,14 +60,15 @@
 - First, implement an extensible, flexible api for accessing data within .odb files or .hdf5 files with odb data
 - Second, implement a user-friendly, sane-defaults cli to allow for quick data extraction, manipulation, and visualization with no hassle
 
 ## Changelog
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1 Implement new system information (pypi tags, this changelog)
+    * 0.5.2 Returning support to Python 3.8+ (type hinting)
 * Upcoming:
     * 0.6.0: Improved extractor across all file types. Improved Odb object iteration.
     * 0.7.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline
     * 0.8.0: Parametrize input values such as nodes, nodesets, frames, steps, parts, and colors (both in the API and CLI).
     * 0.9.0: Create two-dimensional plotting capabilities and sane defaults.
     * 0.10.0: Improve PyVista: views, gifs, non-interactive image saving, leaving viewer, etc. Ensure functionality of Abaqus 2019
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding (or following) a publication.
```

### Comparing `odb-plotter-0.5.1/src/odb_plotter.egg-info/SOURCES.txt` & `odb-plotter-0.5.2/src/odb_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.1/src/odbp/cli.py` & `odb-plotter-0.5.2/src/odbp/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 import sys
 try:
     import tomllib
 except ModuleNotFoundError:
     import tomli as tomllib
 import numpy as np
 import pandas as pd
-from typing import Any, Union, TextIO
+from typing import Any, Union, TextIO, List, Tuple, Dict
 from .odb_visualizer import OdbVisualizer
 from .util import confirm
 from .state import CLIOptions, UserOptions, process_input, print_state, load_views_dict
 from odbp import __version__
 
 
 def cli() -> None:
 
     main_loop: bool = True
 
     # TODO Process input toml file and/or cli switches here
     state: OdbVisualizer
     user_options: UserOptions
-    result: Union[tuple[OdbVisualizer, UserOptions], pd.DataFrame]
+    result: Union[Tuple[OdbVisualizer, UserOptions], pd.DataFrame]
     result = process_input()
     print(f"ODBPlotter {__version__}")
     if isinstance(result, pd.DataFrame):
         sys.exit(print(result))
 
     else:
         state, user_options = result
@@ -111,16 +111,16 @@
 
         except EOFError:
             print("\nExiting")
             main_loop = False
 
 
 def select_files(state: OdbVisualizer, user_options: UserOptions) -> None:
-    odb_options: tuple[str, str] = ("odb", ".odb")
-    hdf_options: tuple[str, str, str, str, str ,str] = (".hdf", "hdf", ".hdf5", "hdf5", "hdfs", ".hdfs")
+    odb_options: Tuple[str, str] = ("odb", ".odb")
+    hdf_options: Tuple[str, str, str, str, str ,str] = (".hdf", "hdf", ".hdf5", "hdf5", "hdfs", ".hdfs")
     user_input: str
 
     # select odb
     while True:
         user_input = input('Please enter either "hdf" if you plan to open .hdf5 file or "odb" if you plan to open a .odb file: ').strip().lower()
 
         if user_input in odb_options or user_input in hdf_options:
@@ -186,15 +186,15 @@
     meltpoint: Union[float, None] = None
     low_temp: Union[float, None] = None
     time_sample: Union[int, None] = None
 
     if user_options.config_file_path is not None:
         config_file: TextIO
         with open(user_options.config_file_path, "rb") as config_file:
-            config: dict[str, Any] = tomllib.load(config_file)
+            config: Dict[str, Any] = tomllib.load(config_file)
 
         if "hdf_file_path" in config:
             if config["hdf_file_path"] != state.hdf_file_path:
                 print("INFO: File name provided and File Name in the config do not match. This could be an issue, or it might be fine")
 
         if "meltpoint" in config:
             meltpoint = config["meltpoint"]
@@ -254,15 +254,15 @@
 
         if isinstance(user_options.config_file_path, str):
             state.dump_config_to_toml(user_options.config_file_path)
 
     state.select_colormap()
 
 
-def set_title_and_label(state: OdbVisualizer, user_options: UserOptions):
+def set_title_and_label(state: OdbVisualizer, user_options: UserOptions) -> None:
     default_title: str = ""
 
     if hasattr(state, "hdf_file_path"):
         default_title = state.hdf_file_path.split(os.sep)[-1].split(".")[0]
     elif hasattr(state, "odb_file_path"):
         default_title = state.odb_file_path.split(os.sep)[-1].split(".")[0]
 
@@ -294,15 +294,15 @@
             user_input = default_label
 
         if confirm(f"You entered {user_input}", "Is this correct", "yes"):
             user_options.image_label = user_input
             break
 
 
-def set_directories(user_options: UserOptions):
+def set_directories(user_options: UserOptions) -> None:
     print(f"For setting all of these data directories, Please enter either absolute paths, or paths relative to your present working directory: {os.getcwd()}")
     user_input: str
 
     gen_hdf_dir: bool = False
     if hasattr(user_options, "hdf_source_directory"):
         gen_hdf_dir = confirm(f".hdf5 source directory is currently set to {user_options.hdf_source_directory}.", "Would you like to overwrite it?")
     else:
@@ -359,29 +359,29 @@
                     else:
                         user_options.results_directory = os.path.join(os.getcwd(), user_input)
                     break
             else:
                 print(f"Error: That directory does not exist. Please enter the absolute path to a directory or the path relative to your present working directory: {os.getcwd()}")
 
 
-def set_extrema(state: OdbVisualizer):
+def set_extrema(state: OdbVisualizer) -> None:
     x_low: float
     x_high: float
     y_low: float
     y_high: float
     z_low: float
     z_high: float
     while True:
         # Get the desired coordinates and time steps to plot
-        extrema: dict[tuple[str, str], tuple[float, float]] = {
+        extrema: Dict[Tuple[str, str], Tuple[float, float]] = {
                 ("lower X", "upper X"): tuple(),
                 ("lower Y", "upper Y"): tuple(),
                 ("lower Z", "upper Z"): tuple(),
                 }
-        extremum: tuple[str, str]
+        extremum: Tuple[str, str]
         for extremum in extrema.keys():
             extrema[extremum] = process_extrema(extremum)
 
         x_low, x_high = extrema[("lower X", "upper X")]
         y_low, y_high = extrema[("lower Y", "upper Y")]
         z_low, z_high = extrema[("lower Z", "upper Z")]
         print()
@@ -437,17 +437,17 @@
             print("Error, Time Sample must be an integer greater than or equal than 1")
 
 
 def set_time(state: OdbVisualizer) -> None:
     lower_time: Union[int, float] = 0
     upper_time: Union[int, float] = float("inf")
     while True:
-        values: list[tuple[str, Union[int, float], str]] = [("lower time", 0, "0"), ("upper time", float("inf"), "infinity")]
+        values: List[Tuple[str, Union[int, float], str]] = [("lower time", 0, "0"), ("upper time", float("inf"), "infinity")]
         i: int
-        v: tuple[str, Union[int, float], str]
+        v: Tuple[str, Union[int, float], str]
         for i, v in enumerate(values): 
             key: str
             default: Union[int, float]
             default_text: str
             key, default, default_text = v
             while True:
                 try:
@@ -470,16 +470,16 @@
         if confirm(f"You entered {lower_time} as the starting time and {upper_time} as the ending time.", "Is this correct", "yes"):
             state.set_time_low(lower_time)
             state.set_time_high(upper_time)
             print(f"Time Range: from {state.time_low} to {state.time_high if state.time_high != float('inf') else 'infinity'}")
             break
 
 
-def process_extrema(keys: "tuple[str, str]") -> "tuple[float, float]":
-    results: list[float] = list()
+def process_extrema(keys: "Tuple[str, str]") -> "Tuple[float, float]":
+    results: List[float] = list()
     i: int
     key: str
     inf_addon: str
     inf_val: float
     for i, key in enumerate(keys):
         if i % 2 == 1:
             inf_addon = ""
@@ -498,21 +498,21 @@
 
             except ValueError:
                 print("Error, all selected coordinates and time steps must be numbers")
 
     return tuple(results)
 
 
-def load_hdf(state: OdbVisualizer):
+def load_hdf(state: OdbVisualizer) -> None:
     state.process_hdf()
 
 
 # TODO Fix
-def set_views(state: OdbVisualizer):
-    views_dict: dict[str, dict[str, int]] = load_views_dict()
+def set_views(state: OdbVisualizer) -> None:
+    views_dict: Dict[str, Dict[str, int]] = load_views_dict()
     while True:
         print("Please Select a Preset View for your plots")
         print('To view all default presets, please enter "list"')
         print('Or, to specify your own view angle, please enter "custom"')
         user_input: str = input("> ").strip().lower()
         if user_input == "list":
             print_views(views_dict)
@@ -542,15 +542,15 @@
                     state.roll = views_dict[user_input]["roll"]
                     return
 
             except:
                 print('Error: input must be "list," "custom," or the index or name of a named view as seen from the "list" command.')
 
 
-def get_custom_view() -> "tuple[int, int, int]":
+def get_custom_view() -> "Tuple[int, int, int]":
     elev: int
     azim: int
     roll: int
     while True:
         while True:
             try:
                 elev = int(input("Elevation Angle in Degrees: "))
@@ -572,19 +572,19 @@
 
         if confirm(f"X Rotation: {elev}\nY Rotation: {azim}\nZ Rotation: {roll}", "Is this correct?", "yes"):
             break
 
     return (elev, azim, roll)
 
 
-def print_views(views: "dict[str, dict[str, int]]") -> None:
+def print_views(views: "Dict[str, Dict[str, int]]") -> None:
     print("Index | Name | Rotation Values")
-    v: tuple[str, dict[str, int]]
+    v: Tuple[str, Dict[str, int]]
     view: str
-    vals: dict[str, int]
+    vals: Dict[str, int]
     key: str
     val: int
     for i, v in enumerate(views.items()):
         view, vals = v
         print(f"{i + 1}: `{view}")
         for key, val in vals.items():
             print(f"\t{key}: {val}")
@@ -646,8 +646,8 @@
             print('Error: The plotter could not save a screenshot. Please close the viewing window by hitting the "q" key instead.')
 
     else:
         plot.screenshot(save_str)
         # with plot.window_size_context((1920, 1080)):
         #     plot.screenshot(save_str)
 
-    del plot
+    del plot
```

### Comparing `odb-plotter-0.5.1/src/odbp/data/config.toml` & `odb-plotter-0.5.2/src/odbp/data/config.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.1/src/odbp/npz_to_hdf.py` & `odb-plotter-0.5.2/src/odbp/npz_to_hdf.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,67 +17,68 @@
 """
 
 
 import h5py
 import pathlib
 import os
 import numpy as np
-from .util import NDArrayType, NPZFileType, H5PYFileType, PathType
+from typing import Dict, List, Tuple
+from .util import NDArrayType, NPZFileType, H5PYFileType
 
 
 def convert_npz_to_hdf(
-    hdf_path: PathType,
-    npz_dir: PathType = pathlib.Path("tmp_npz")
+    hdf_path: pathlib.Path,
+    npz_dir: pathlib.Path = pathlib.Path("tmp_npz")
     ) -> None:
 
     # Format of the npz_dir:
     # node_coords.npz (locations per node)
     # step_frame_times/<step>.npz (times per step)
     # temps/<step>/<frame>.npz (temperatures per node per frame)
     # All of these must exist (error if they do not)
     # They're the only things we care about
 
     hdf_path = pathlib.Path(hdf_path)
     npz_dir = pathlib.Path(npz_dir)
 
-    step_frame_times_dir = npz_dir / pathlib.Path("step_frame_times")
-    step_frame_times: dict[str, NDArrayType] = dict()
-    root: PathType
-    files: list[PathType]
+    step_frame_times_dir: pathlib.Path = npz_dir / pathlib.Path("step_frame_times")
+    step_frame_times: Dict[str, NDArrayType] = dict()
+    root: pathlib.Path
+    files: List[pathlib.Path]
     for root, _, files in os.walk(step_frame_times_dir):
         root = pathlib.Path(root)
-        file: PathType
+        file: pathlib.Path
         for file in files:
             file = pathlib.Path(file)
             key: str = str(file.stem)
             step_frame_times_file: NPZFileType
             with np.load(root / file) as step_frame_times_file:
                 time_data: NDArrayType = step_frame_times_file[
                         step_frame_times_file.files[0]
                         ]
 
             step_frame_times[key] = time_data
 
-    node_coords_path: PathType = npz_dir / pathlib.Path("node_coords.npz")
+    node_coords_path: pathlib.Path = npz_dir / pathlib.Path("node_coords.npz")
     node_coords_file: NPZFileType
     with np.load(node_coords_path) as node_coords_file:
         coordinate_data: NDArrayType = node_coords_file[
                 node_coords_file.files[0]
                 ]
 
-    temps_dir: PathType = npz_dir / pathlib.Path("temps")
-    temp_dict: dict[str, dict[str, NDArrayType]] = dict()
-    root: PathType
-    files: list[PathType]
+    temps_dir: pathlib.Path = npz_dir / pathlib.Path("temps")
+    temp_dict: Dict[str, Dict[str, NDArrayType]] = dict()
+    root: pathlib.Path
+    files: List[pathlib.Path]
     for root, _, files in os.walk(temps_dir):
         root = pathlib.Path(root)
         step_name: str = root.stem
         temp_dict[step_name] = dict()
         files.sort()
-        file: PathType
+        file: pathlib.Path
         for file in files:
             file = pathlib.Path(file)
             temps_file: NPZFileType
             with np.load(root / file) as temps_file:
                 temps_data: NDArrayType = temps_file[
                         temps_file.files[0]
                         ]
@@ -89,15 +90,15 @@
     hdf5_file: H5PYFileType
     with h5py.File(hdf_path, "w") as hdf5_file:
         # Temps/Coords
         step: str
         node_data: NDArrayType
         for step in temp_dict:
             i: int
-            items: tuple[str, dict[str, NDArrayType]]
+            items: Tuple[str, Dict[str, NDArrayType]]
             for i, items in enumerate(temp_dict[step].items()):
                 file: str
                 node_data: NDArrayType
                 file, node_data = items
                 frame: str = pathlib.Path(file).stem
                 target_len: int = len(node_data)
                 hdf5_file.create_dataset(
```

### Comparing `odb-plotter-0.5.1/src/odbp/odb.py` & `odb-plotter-0.5.2/src/odbp/odb.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 import shutil
 import pathlib
 import pickle
 import multiprocessing
 
 import pandas as pd
 
-from typing import TextIO, Callable, Any
+from typing import TextIO, Callable, Union, Any, List, Dict
 from abc import abstractmethod
 
 from .npz_to_hdf import convert_npz_to_hdf
 from .read_hdf5 import get_odb_data
-from .util import NullableIntList, NullableStrList, DataFrameType, MultiprocessingPoolType, PathType
+from .util import NullableIntList, NullableStrList, DataFrameType, MultiprocessingPoolType
 
 
 class Odb():
     """
     Stores Data from a .hdf5, implements extractor methods to transfer from .odb to .hdf5
     Implements abilities to resize the dimenisons or timeframe of the data
     """
@@ -59,22 +59,22 @@
 
     def __init__(self) -> None:
         """
         Type Hints and hard-coded parameters. See the @staticmethod
         "constructors" of this class in order to learn about initialization
         """
 
-        self._odb_handler: OdbLoader | OdbUnloader = OdbLoader()
+        self._odb_handler: Union[OdbLoader, OdbUnloader] = OdbLoader()
         self._odb: DataFrameType 
 
-        self._odb_path: PathType
-        self._odb_source_dir: PathType | None
+        self._odb_path: pathlib.Path
+        self._odb_source_dir: Union[pathlib.Path, None]
 
-        self._hdf_path: PathType
-        self._hdf_source_dir: PathType | None
+        self._hdf_path: pathlib.Path
+        self._hdf_source_dir: Union[pathlib.Path, None]
 
         self._abaqus_executable: str = "abaqus"
 
         self._nodesets: NullableStrList = None
         self._frames: NullableIntList = None
 
         self._x_low: float
@@ -87,26 +87,26 @@
         self._temp_low: float
         self._temp_high: float
 
         self._time_low: float
         self._time_high: float
 
         # Hardcoded paths for Python 3 - 2 communication
-        self._odb_to_npz_script_path: PathType = pathlib.Path(
+        self._odb_to_npz_script_path: pathlib.Path = pathlib.Path(
             pathlib.Path(__file__).parent,
             "py2_scripts",
             "odb_to_npz.py"
         )
 
-        self._odb_to_npz_conversion_pickle_path: PathType = pathlib.Path(
+        self._odb_to_npz_conversion_pickle_path: pathlib.Path = pathlib.Path(
             pathlib.Path.cwd(),
             "odb_to_npz_conversion.pickle"
         )
 
-        self._npz_result_path: PathType = pathlib.Path(
+        self._npz_result_path: pathlib.Path = pathlib.Path(
             pathlib.Path.cwd(),
             "npz_path.pickle"
         )
 
         # TODO
         """self._parts: NullableStrList
         self._nodes: dict[str, list[int]]"""
@@ -363,77 +363,77 @@
             if value < self.time_low:
                 raise ValueError(f"The value for time_high ({value}) must not be less than the value for time_low ({self.time_low})")
 
         self._time_high = value
 
 
     @property
-    def odb_source_dir(self) -> PathType | None:
+    def odb_source_dir(self) -> "Union[pathlib.Path, None]":
         return self._odb_source_dir
 
 
     @odb_source_dir.setter
-    def odb_source_dir(self, value: PathType) -> None:
+    def odb_source_dir(self, value: pathlib.Path) -> None:
         value = pathlib.Path(value)
 
         if not value.exists():
             raise FileNotFoundError(f"Directory {value} does not exist")
 
         self._odb_source_dir = value
 
 
     @property
-    def odb_path(self) -> PathType | None:
+    def odb_path(self) -> "Union[pathlib.Path, None]":
         return self._odb_path
 
 
     @odb_path.setter
-    def odb_path(self, value: PathType) -> None:
+    def odb_path(self, value: pathlib.Path) -> None:
         value = pathlib.Path(value)
 
         if value.exists():
             self._odb_path = value
             return
 
         if self.odb_source_dir is not None:
-            source_dir_path: PathType = self.odb_source_dir / value
+            source_dir_path: pathlib.Path = self.odb_source_dir / value
             if source_dir_path.exists():
                 self._odb_path = source_dir_path
                 return
 
-        cwd_path: PathType = pathlib.Path.cwd() / value
+        cwd_path: pathlib.Path = pathlib.Path.cwd() / value
         if cwd_path.exists():
             self._odb_path = cwd_path
             return
 
         raise FileNotFoundError(f"File {value} could not be found")
 
 
     @property
-    def hdf_source_dir(self) -> PathType | None:
+    def hdf_source_dir(self) -> "Union[pathlib.Path, None]":
         return self._hdf_source_dir
 
 
     @hdf_source_dir.setter
-    def hdf_source_dir(self, value: PathType) -> None:
+    def hdf_source_dir(self, value: pathlib.Path) -> None:
         value = pathlib.Path(value)
 
         if not value.exists():
             raise FileNotFoundError(f"Directory {value} does not exist")
 
         self._hdf_source_dir = value
 
 
     @property
-    def hdf_path(self) -> PathType:
+    def hdf_path(self) -> pathlib.Path:
         return self._hdf_path
 
 
     @hdf_path.setter
-    def hdf_path(self, value: PathType) -> None:
+    def hdf_path(self, value: pathlib.Path) -> None:
         value = pathlib.Path(value)
 
         if value.is_absolute():
             self._hdf_path = value
             return
 
         if hasattr(self, "_hdf_source_dir"):
@@ -450,30 +450,30 @@
 
     @abaqus_executable.setter
     def abaqus_executable(self, value: str) -> None:
         self._abaqus_executable = value
 
 
     @property
-    def frames(self) -> list[int]:
+    def frames(self) -> "List[int]":
         return self._frames
 
 
     @frames.setter
-    def frames(self, value: list[int]) -> None:
+    def frames(self, value: "List[int]") -> None:
         self._frames = value
 
 
     @property
-    def nodesets(self) -> list[int]:
+    def nodesets(self) -> "List[int]":
         return self._nodesets
 
 
     @nodesets.setter
-    def nodesets(self, value: list[int]) -> None:
+    def nodesets(self, value: "List[int]") -> None:
         self._nodesets = value
 
 
     """def set_parts(self, parts: "list[str]") -> None:
         if not isinstance(parts, list):
             new_list: list[str] = [parts]
             self.parts = new_list
@@ -496,17 +496,17 @@
 
         else:
             self.nodesets = nodesets"""
 
 
     def convert_odb_to_hdf(
             self,
-            hdf_path: PathType | None = None,
+            hdf_path: "Union[pathlib.Path, None]" = None,
             *,
-            odb_path: PathType | None = None,
+            odb_path: "Union[pathlib.Path, None]" = None,
             set_odb: bool = False,
             set_hdf: bool = False
             ) -> None:
 
         if odb_path is not None:
             odb_path = pathlib.Path(odb_path)
             if set_odb:
@@ -535,52 +535,52 @@
 
         self._convert_odb_to_hdf(hdf_path, odb_path)
 
 
     @classmethod
     def convert(
             cls,
-            hdf_path: PathType,
-            odb_path: PathType
+            hdf_path: pathlib.Path,
+            odb_path: pathlib.Path
             ) -> None:
         hdf_path = pathlib.Path(hdf_path)
         odb_path = pathlib.Path(odb_path)
         cls()._convert_odb_to_hdf(hdf_path, odb_path)
 
 
     def _convert_odb_to_hdf(
             self,
-            hdf_path: PathType,
-            odb_path: PathType
+            hdf_path: pathlib.Path,
+            odb_path: pathlib.Path
             ) -> None:
 
-        odb_to_npz_pickle_input_dict: dict[
-            str, list[str] | list[int] | None
+        odb_to_npz_pickle_input_dict: Dict[
+            str, Union[List[str], List[int], None]
             ] = {
                 "nodesets": self._nodesets,
                 "frames": self._frames
             }
         pickle_file: TextIO
         with open(
             self._odb_to_npz_conversion_pickle_path, "wb") as pickle_file:
             pickle.dump(odb_to_npz_pickle_input_dict, pickle_file, protocol=2)
 
-        odb_convert_args: list[PathType | str]  = [
+        odb_convert_args: List[Union[pathlib.Path, str]]  = [
             abaqus_executable,
             "python",
             self._odb_to_npz_script_path,
             odb_path,
             self._odb_to_npz_conversion_pickle_path,
             self._npz_result_path
         ]
 
         subprocess.run(odb_convert_args, shell=True)
 
         result_file: TextIO
-        result_dir: PathType
+        result_dir: pathlib.Path
         with open(self._npz_result_path, "rb") as result_file:
             result_dir = pathlib.Path(pickle.load(result_file))
 
         pathlib.Path.unlink(self._npz_result_path)
 
         convert_npz_to_hdf(hdf_path, result_dir)
 
@@ -619,15 +619,15 @@
 
 
     # TODO generator method for time steps. Overload __iter__?
 
 
 class OdbLoader:
 
-    def load_hdf(self, hdf_path: PathType) -> DataFrameType:
+    def load_hdf(self, hdf_path: pathlib.Path) -> DataFrameType:
         return get_odb_data(hdf_path)
 
 
 class OdbUnloader:
 
     @abstractmethod
     def unload_hdf(self) -> None:
```

### Comparing `odb-plotter-0.5.1/src/odbp/odb_visualizer.py` & `odb-plotter-0.5.2/src/odbp/odb_visualizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 plotting capabilities.
 """
 
 import operator
 import multiprocessing
 import numpy as np
 import pyvista as pv
+from typing import Union, Tuple, List
 from .odb import Odb
 from .util import DataFrameType, MultiprocessingPoolType
 
 
 class OdbVisualizer(Odb):
     """
     Serves exactly as a normal Odb instance, but includes
@@ -35,15 +36,15 @@
         
         super().__init__()
 
         self._interactive: bool = False
         self._colormap: str = "turbo"
 
         # TODO ???
-        self._angle: str | tuple[float, float, float]
+        self._angle: Union[str, Tuple[float, float, float]]
 
 
     @property
     def colormap(self) -> str:
         return self._colormap
     
 
@@ -58,55 +59,55 @@
 
 
     @interactive.setter
     def interactive(self, value: bool) -> None:
         self._interactive = value
 
 
-    def plot_3d_all_times(self, label: str = "") -> list[pv.Plotter]:
+    def plot_3d_all_times(self, label: str = "") -> "List[pv.Plotter]":
         """
         """
 
         times: DataFrameType = np.sort(self._filtered_nodes["Time"].unique())
         
-        plotting_args: list[
-            tuple[
+        plotting_args: List[
+            Tuple[
                 float,
                 str
                 ]
             ] = [(time, label) for time in times]
-        results: list[pv.Plotter] = list()
+        results: List[pv.Plotter] = list()
         time: float
         for time in times:
             results.append(self.plot_3d_single(time, label))
         # TODO Any way to make this work?
         """
         # TODO dataclass
-        plotting_args: list[
-            tuple[
+        plotting_args: List[
+            Tuple[
                 float,
                 str
                 ]
             ] = [(time, label) for time in times]
-        results: list[pv.Plotter] = list()
+        results: List[pv.Plotter] = list()
         pool: MultiprocessingPoolType
         with multiprocessing.Pool() as pool:
             results: list[pv.Plotter] = pool.starmap(
                 self.plot_3d_single,
                 plotting_args
                 )"""
 
         return results 
 
 
     def plot_3d_single(
         self,
         time: float,
         label: str
-        )-> pv.Plotter | None:
+        )-> "Union[pv.Plotter, None]":
         """
         """
 
         dims_columns: set[str] = {"X", "Y", "Z"}
         combined_label: str = f"{label}-{round(time, 2):.2f}"
 
         plotter: pv.Plotter = pv.Plotter(
```

### Comparing `odb-plotter-0.5.1/src/odbp/py2_scripts/extract.py` & `odb-plotter-0.5.2/src/odbp/py2_scripts/extract.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.1/src/odbp/py2_scripts/odb_to_npz.py` & `odb-plotter-0.5.2/src/odbp/py2_scripts/odb_to_npz.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.1/src/odbp/read_hdf5.py` & `odb-plotter-0.5.2/src/odbp/read_hdf5.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,40 +11,41 @@
 """
 
 import h5py
 import multiprocessing
 import pathlib
 import numpy as np
 import pandas as pd
-from .util import NDArrayType, DataFrameType, H5PYGroupType, H5PYFileType, MultiprocessingPoolType, PathType
+from typing import Tuple, List
+from .util import NDArrayType, DataFrameType, H5PYGroupType, H5PYFileType, MultiprocessingPoolType
 
 
 def get_odb_data(
-    hdf_path: PathType
+    hdf_path: pathlib.Path
     ) -> DataFrameType:
     """
-    get_node_coords(hdf_path: PathType) -> DataFrameType
+    get_node_coords(hdf_path: pathlib.Path) -> DataFrameType
     return a data frame with nodes by integer index and floating point
     3-dimensional coordinates.
     """
 
     try:
         hdf_file: H5PYFileType
         with h5py.File(hdf_path) as hdf_file:
             step: str
             for step in hdf_file["nodes"].keys():
                 frame_name: str
                 # TODO dataclass
-                args_list: list[tuple(H5PYFileType, str, str)] = [
+                args_list: List[Tuple(H5PYFileType, str, str)] = [
                         (hdf_path, step, frame_name)
                         for frame_name
                         in hdf_file["nodes"][step].keys() 
                         ]
 
-                results: list[DataFrameType]
+                results: List[DataFrameType]
                 pool: MultiprocessingPoolType
                 with multiprocessing.Pool() as pool:
                     results = pool.starmap(get_frame_data, args_list)
 
                 return pd.concat(results)
 
     except (FileNotFoundError, OSError):
```

### Comparing `odb-plotter-0.5.1/src/odbp/state.py` & `odb-plotter-0.5.2/src/odbp/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     import tomli as tomllib
 import sys
 import os
 import platformdirs
 import subprocess
 import pickle
 import pandas as pd
-from typing import Union, Any, TextIO
+from typing import Union, Any, TextIO, Tuple, List, Dict
 from .odb_visualizer import OdbVisualizer
 from .util import confirm
 from odbp import __version__
 
 
 class UserOptions():
     """
@@ -40,83 +40,83 @@
 
 
 class CLIOptions():
     """
     Struct to store cli options without repeating
     """
     def __init__(self) -> None:
-        self.quit_options: list[str] = ["exit", "quit", "q"]
+        self.quit_options: List[str] = ["exit", "quit", "q"]
         self.quit_help: str = "Exit ODBPlotter"
         self.quit_options_formatted: str = ", ".join(self.quit_options)
 
-        self.select_options: list[str] = ["select"]
+        self.select_options: List[str] = ["select"]
         self.select_help: str = "Select a .hdf5 file or a .odb file"
         self.select_options_formatted: str = ", ".join(self.select_options)
 
-        self.convert_options: list[str] = ["convert"]
+        self.convert_options: List[str] = ["convert"]
         self.convert_help: str = "Convert a selected .odb file to a .hdf5 file"
         self.convert_options_formatted: str = ", ".join(self.convert_options)
 
-        self.extrema_options: list[str] = ["extrema", "range"]
+        self.extrema_options: List[str] = ["extrema", "range"]
         self.extrema_help: str = "Set the upper and lower x, y, and z bounds for plotting"
         self.extrema_options_formatted: str = ", ".join(self.extrema_options)
 
-        self.time_options: list[str] = ["time"]
+        self.time_options: List[str] = ["time"]
         self.time_help: str = "Set the upper and lower time bounds"
         self.time_options_formatted: str = ", ".join(self.time_options)
 
-        self.time_sample_options: list[str] = ["sample"]
+        self.time_sample_options: List[str] = ["sample"]
         self.time_sample_help: str = "Set the Time Sample for the hdf5 file"
         self.time_sample_options_formatted: str = ", ".join(self.time_sample_options)
 
-        self.meltpoint_options: list[str] = ["meltpoint", "melt", "point"]
+        self.meltpoint_options: List[str] = ["meltpoint", "melt", "point"]
         self.meltpoint_help: str = "Set the Melting Point for the hdf5 file"
         self.meltpoint_options_formatted: str = ", ".join(self.meltpoint_options)
 
-        self.low_temp_options: list[str] = ["low", "low-temp"]
+        self.low_temp_options: List[str] = ["low", "low-temp"]
         self.low_temp_help: str = "Set the Lower Temperate Bound for the hdf5 file"
         self.low_temp_options_formatted: str = ", ".join(self.low_temp_options)
 
-        self.title_label_options: list[str] = ["title", "label"]
+        self.title_label_options: List[str] = ["title", "label"]
         self.title_label_help: str = "Set the title and label of the output plots"
         self.title_label_options_formatted: str = ", ".join(self.title_label_options)
 
-        self.directory_options: list[str] = ["dir", "dirs", "directory", "directories"]
+        self.directory_options: List[str] = ["dir", "dirs", "directory", "directories"]
         self.directory_help: str = "Set the source and output directories"
         self.directory_options_formatted: str = ", ".join(self.directory_options)
 
-        self.process_options: list[str] = ["process", "run", "load"]
+        self.process_options: List[str] = ["process", "run", "load"]
         self.process_help: str = "Actually load the selected data from the file set in select"
         self.process_options_formatted: str = ", ".join(self.process_options)
 
-        self.angle_options: list[str] = ["angle",]
+        self.angle_options: List[str] = ["angle",]
         self.angle_help: str = "Update the viewing angle"
         self.angle_options_formatted: str = ", ".join(self.angle_options)
 
-        self.show_all_options: list[str] = ["show-all", "plot-all"]
+        self.show_all_options: List[str] = ["show-all", "plot-all"]
         self.show_all_help: str = "Toggle if each time step will be shown in the PyVista interactive viewer"
         self.show_all_options_formatted: str = ", ".join(self.show_all_options)
 
-        self.plot_options: list[str] = ["plot", "show"]
+        self.plot_options: List[str] = ["plot", "show"]
         self.plot_help: str = "Plot each selected timestep"
         self.plot_options_formatted: str = ", ".join(self.plot_options)
         
-        self.state_options: list[str] = ["state", "status", "settings"]
+        self.state_options: List[str] = ["state", "status", "settings"]
         self.state_help: str = "Show the current state of the settings of the plotter"
         self.state_options_formatted: str = ", ".join(self.state_options)
 
-        self.abaqus_options: list[str] = ["abaqus", "abq", "abqpy"]
+        self.abaqus_options: List[str] = ["abaqus", "abq", "abqpy"]
         self.abaqus_help: str = "Select the Abaqus executable program to use to process .odb file"
         self.abaqus_options_formatted: str = ", ".join(self.abaqus_options)
 
-        self.nodeset_options: list[str] = ["node", "nodes", "nodeset", "nodesets"]
+        self.nodeset_options: List[str] = ["node", "nodes", "nodeset", "nodesets"]
         self.nodeset_help: str = "Select the target nodeset (i.e., the named nodeset that contains all the data)"
         self.nodeset_options_formatted: str = ", ".join(self.nodeset_options)
 
-        self.help_options: list[str] = ["help", "use", "usage"]
+        self.help_options: List[str] = ["help", "use", "usage"]
         self.help_help: str = "Show this menu"
         self.help_options_formatted: str = ", ".join(self.help_options)
 
         self.longest_len: int = max(
                 len(self.quit_options_formatted),
                 len(self.select_options_formatted),
                 len(self.convert_options_formatted),
@@ -155,15 +155,15 @@
 {self.abaqus_options_formatted.ljust(self.longest_len)} -- {self.abaqus_help}
 {self.nodeset_options_formatted.ljust(self.longest_len)} -- {self.nodeset_help}
 {self.state_options_formatted.ljust(self.longest_len)} -- {self.state_help}"""
     )
 
 
 def print_state(state: OdbVisualizer, user_options: UserOptions) -> None:
-    lines: list[dict[str, str]] = [
+    lines: List[Dict[str, str]] = [
         {
             ".hdf5 file": f"{state.hdf_file_path if hasattr(state, 'hdf_file_path') else 'not set'}",
             ".odb file": f"{state.odb_file_path if hasattr(state, 'odb_file_path') else 'not set'}",
         },
         {
             "Source directory of .hdf5 files": f"{user_options.hdf_source_directory}",
             "Source directory of .odb files": f"{user_options.odb_source_directory}",
@@ -198,30 +198,30 @@
             "Data loaded into memory": f"{'Yes' if state.loaded else 'No'}",
             "Abaqus Program": f"{state.abaqus_program if hasattr(state, 'abaqus_program') else 'not set'}",
         },
     ]
 
     key: str
     val: str
-    sub_dict: dict[str, str]
+    sub_dict: Dict[str, str]
     max_len = 0
     for sub_dict in lines:
         for key in sub_dict.keys():
             max_len = max(max_len, len(key))
 
     final_state_output: str = ""
     for sub_dict in lines:
         for key, val in sub_dict.items():
             final_state_output += key.ljust(max_len) + ": " + val + "\n"
         final_state_output += "\n" 
 
     print(final_state_output, end="") # No ending newline because we added it above
 
 
-def process_input() -> "Union[tuple[OdbVisualizer, UserOptions], pd.DataFrame]": # Returns UserOptions or Pandas Dataframe
+def process_input() -> "Union[Tuple[OdbVisualizer, UserOptions], pd.DataFrame]": # Returns UserOptions or Pandas Dataframe
     """
     The goal is to have a hierarchy of options. If a user passes in an option via a command-line switch, that option is set.
     If an option is not set by a switch, then the toml input file is used.
     If an option is not set by the input file (if any), then prompt for it
     Possibly also include a default config file, like in $HOME/.config? Not sure
     """
 
@@ -277,15 +277,15 @@
         #return extract_from_file(args)
         return extract_from_file(args)
 
     else:
         return generate_cli_settings(args)
 
 
-def generate_cli_settings(args: argparse.Namespace) -> "tuple[OdbVisualizer, UserOptions]":
+def generate_cli_settings(args: argparse.Namespace) -> "Tuple[OdbVisualizer, UserOptions]":
 
     state: OdbVisualizer = OdbVisualizer()
     user_options: UserOptions = UserOptions()
 
     # Stage 1: User platformdirs to read base-line settings
     odbp_config_dir: str = platformdirs.user_config_dir("odbp")
     if not os.path.exists(odbp_config_dir):
@@ -299,15 +299,15 @@
         with open(os.path.join(os.path.dirname(os.path.realpath(__file__)), "data", "config.toml"), "r") as base_config_file:
             config_data = base_config_file.read()
 
         with open(config_file_path, "w") as new_config_file:
             new_config_file.write(config_data)
 
     config_file: TextIO
-    config_settings: dict[str, Any]
+    config_settings: Dict[str, Any]
     with open(config_file_path, "rb") as config_file:
         config_settings = tomllib.load(config_file)
     state, user_options = read_setting_dict(state, user_options, config_settings)
 
     # Stage 2: Use the input_file if it exists
     if args.input_file:
         input_file_path: str = args.input_file
@@ -315,22 +315,22 @@
             if not os.path.exists(os.path.join(os.getcwd(), input_file_path)):
                 print(F"Error: Input File {input_file_path} could not be found")
                 sys.exit(1)
             else:
                 input_file_path = os.path.join(os.getcwd(), input_file_path)
 
         input_file: TextIO
-        input_settings: dict[str, Any]
+        input_settings: Dict[str, Any]
         with open(input_file_path, "rb") as input_file:
             input_settings = tomllib.load(input_file)
 
         state, user_options = read_setting_dict(state, user_options, input_settings)
 
     # Stage 3: pass in the (other) dict values from args
-    cli_flags: dict[str, any] = vars(args)
+    cli_flags: Dict[str, any] = vars(args)
     cli_flags = {k: v for k, v in cli_flags.items() if v is not None}
     state, user_options = read_setting_dict(state, user_options, cli_flags)
 
     if not os.path.exists(user_options.results_directory):
         print(f"Directory {user_options.results_directory} does not exist. Creating it now.")
         os.makedirs(user_options.results_directory)
 
@@ -353,55 +353,55 @@
     state: OdbVisualizer
     state, _ = generate_cli_settings(args)
 
     odb_extract_script_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "py2_scripts", "extract.py")
     temp_save_path = os.path.join(os.getcwd(), "temp.pickle")
 
     # Because of the python3-2 cross-talk, we use strings of "None", unfortunately
-    parts: Union[list[str], None] = None
-    nodesets: Union[list[str], None] = None
-    nodes: Union[dict[str, list[int]], None] = None
+    parts: Union[List[str], None] = None
+    nodesets: Union[List[str], None] = None
+    nodes: Union[Dict[str, List[int]], None] = None
     if hasattr(state, "parts"):
         parts = state.parts
 
     if hasattr(state, "nodesets"):
         nodesets = state.nodesets
 
     if hasattr(state, "nodes"):
         nodes = state.nodes
 
     # subprocess won't handle the Nones or dicts or lists well, so instead we pickle in the output path, and read in the python2 version
     # They're all built-ins, so pickle should work
     temp_file: TextIO
-    input_dict: dict[str, Any] = {
+    input_dict: Dict[str, Any] = {
         "parts": parts,
         "nodesets": nodesets,
         "nodes": nodes,
     }
     # TODO Time Sample
     with open(temp_save_path, "wb") as temp_file:
         pickle.dump(input_dict, temp_file, protocol=2)
-    odb_extract_args: list[str] = [state.abaqus_program, "python", odb_extract_script_path, state.odb_file_path, temp_save_path]
+    odb_extract_args: List[str] = [state.abaqus_program, "python", odb_extract_script_path, state.odb_file_path, temp_save_path]
     subprocess.run(odb_extract_args, shell=True)
 
-    #odb_to_npz_args: list[str] = [self.abaqus_program, "python", odb_to_npz_script_path, os.path.join(os.getcwd(), self.odb_file_path), str(self.time_sample)]
+    #odb_to_npz_args: List[str] = [self.abaqus_program, "python", odb_to_npz_script_path, os.path.join(os.getcwd(), self.odb_file_path), str(self.time_sample)]
     #subprocess.run(odb_to_npz_args, shell=True)
 
     return_data: pd.DataFrame
     with open(temp_save_path, "rb") as temp_file:
         # From the Pickle Spec, decoding numpy arrays from python 2 must use encoding="latin-1"
         return_data = pd.DataFrame(pickle.load(temp_file, encoding="latin-1"))
 
     if os.path.exists(temp_save_path):
         os.remove(temp_save_path)
 
     return return_data
 
 
-def read_setting_dict(state: OdbVisualizer, user_options: UserOptions, settings_dict: "dict[str, Any]") -> "tuple[OdbVisualizer, UserOptions]":
+def read_setting_dict(state: OdbVisualizer, user_options: UserOptions, settings_dict: "Dict[str, Any]") -> "Tuple[OdbVisualizer, UserOptions]":
     hdf_source_dir: str
     if "hdf_source_directory" in settings_dict:
         hdf_source_dir = os.path.abspath(settings_dict["hdf_source_directory"])
 
         if not os.path.exists(hdf_source_dir):
             print(f"Error: The directory {hdf_source_dir} does not exist")
             sys.exit(1)
@@ -473,15 +473,15 @@
         else:
             user_options = output
 
         # If none of these values are set, read as many as are available out of the .toml config file
         # Otherwise, the file must have already been read
 
         # Search for the stored toml values for this hdf
-        config: Union[dict[str, Any], None] = None
+        config: Union[Dict[str, Any], None] = None
         if user_options.config_file_path is None:
             print(f".toml config file for {state.hdf_file_path} could not be found")
         else:
             config_file: TextIO
             with open(user_options.config_file_path, "rb") as config_file:
                 config = tomllib.load(config_file)
 
@@ -584,15 +584,15 @@
         if isinstance(settings_dict["view"], dict):
             state.angle = "custom"
             state.elev = settings_dict["view"]["elev"]
             state.azim = settings_dict["view"]["azim"]
             state.roll = settings_dict["view"]["roll"]
         
         else:
-            given_view: dict[str, int] = view(settings_dict["view"])
+            given_view: Dict[str, int] = view(settings_dict["view"])
             elev: int = given_view["elev"]
             azim: int = given_view["azim"]
             roll: int = given_view["roll"]
             state.angle=settings_dict["view"]
             state.elev = elev
             state.azim = azim
             state.roll = roll
@@ -622,23 +622,23 @@
             state.set_abaqus(settings_dict["abaqus"])
     else:
         state.set_abaqus(settings_dict.get("abaqus", "abaqus"))
 
     return (state, user_options)
 
 
-def load_views_dict() -> "dict[str, dict[str, int]]":
+def load_views_dict() -> "Dict[str, Dict[str, int]]":
     views_file: TextIO
     with open(os.path.join(os.path.dirname(os.path.realpath(__file__)), "data", "views.toml"), "rb") as views_file:
         return tomllib.load(views_file)
 
 
 # Used to define the "view" type for argparse
-def view(string: str) -> "dict[str, int]":
-    views_dict: dict[str, dict[str, int]] = load_views_dict()
+def view(string: str) -> "Dict[str, int]":
+    views_dict: Dict[str, Dict[str, int]] = load_views_dict()
     if string in views_dict:
         return views_dict[string]
 
     # Otherwise, try to parse the user's input as a 3-tuple
     formatted_string: str = string.replace("(", "")
     formatted_string = formatted_string.replace(")", "")
     formatted_string = formatted_string.replace("[", "")
```

