# Comparing `tmp/energyplus_launch-3.6.8.tar.gz` & `tmp/energyplus_launch-3.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_launch-3.6.8.tar", last modified: Fri May 19 19:08:18 2023, max compression
+gzip compressed data, was "energyplus_launch-3.6.9.tar", last modified: Fri Jun  2 21:22:00 2023, max compression
```

## Comparing `energyplus_launch-3.6.8.tar` & `energyplus_launch-3.6.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:18.500853 energyplus_launch-3.6.8/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-05-19 19:08:18.500853 energyplus_launch-3.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:18.496853 energyplus_launch-3.6.8/energyplus_launch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-05-19 19:08:18.000000 energyplus_launch-3.6.8/energyplus_launch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-05-19 19:08:18.000000 energyplus_launch-3.6.8/energyplus_launch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-19 19:08:18.000000 energyplus_launch-3.6.8/energyplus_launch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-19 19:08:18.000000 energyplus_launch-3.6.8/energyplus_launch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-19 19:08:18.000000 energyplus_launch-3.6.8/energyplus_launch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-19 19:08:18.000000 energyplus_launch-3.6.8/energyplus_launch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:18.496853 energyplus_launch-3.6.8/eplaunch/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:18.496853 energyplus_launch-3.6.8/eplaunch/interface/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6214 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/dialog_external_viewers.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/dialog_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/dialog_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     5139 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/dialog_weather.py
--rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/dialog_workflow_dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    73621 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/frame_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/widget_dir_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/widget_file_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/widget_group_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/tk_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:18.500853 energyplus_launch-3.6.8/eplaunch/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/utilities/crossplatform.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/utilities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:18.500853 energyplus_launch-3.6.8/eplaunch/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:18.500853 energyplus_launch-3.6.8/eplaunch/workflows/default/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/default/file_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/default/idf_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/default/site_location.py
--rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/workflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/workflow_tester.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/workflow_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-05-19 19:08:18.500853 energyplus_launch-3.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:22:00.714933 energyplus_launch-3.6.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-06-02 21:22:00.714933 energyplus_launch-3.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:22:00.710933 energyplus_launch-3.6.9/energyplus_launch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-06-02 21:22:00.000000 energyplus_launch-3.6.9/energyplus_launch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-06-02 21:22:00.000000 energyplus_launch-3.6.9/energyplus_launch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 21:22:00.000000 energyplus_launch-3.6.9/energyplus_launch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-02 21:22:00.000000 energyplus_launch-3.6.9/energyplus_launch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-02 21:22:00.000000 energyplus_launch-3.6.9/energyplus_launch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-02 21:22:00.000000 energyplus_launch-3.6.9/energyplus_launch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:22:00.710933 energyplus_launch-3.6.9/eplaunch/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:22:00.710933 energyplus_launch-3.6.9/eplaunch/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6090 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/dialog_external_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/dialog_generic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/dialog_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5198 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/dialog_weather.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4689 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/dialog_workflow_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    73823 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/frame_main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/widget_dir_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/widget_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/interface/widget_group_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/tk_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:22:00.714933 energyplus_launch-3.6.9/eplaunch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/utilities/crossplatform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/utilities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:22:00.714933 energyplus_launch-3.6.9/eplaunch/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:22:00.714933 energyplus_launch-3.6.9/eplaunch/workflows/default/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/default/file_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/default/idf_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/default/site_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/workflow_tester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/eplaunch/workflows/workflow_thread.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-02 21:22:00.714933 energyplus_launch-3.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-06-02 21:21:52.000000 energyplus_launch-3.6.9/setup.py
```

### Comparing `energyplus_launch-3.6.8/LICENSE` & `energyplus_launch-3.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/PKG-INFO` & `energyplus_launch-3.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus_launch
-Version: 3.6.8
+Version: 3.6.9
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.6.8/README.md` & `energyplus_launch-3.6.9/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/energyplus_launch.egg-info/PKG-INFO` & `energyplus_launch-3.6.9/energyplus_launch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus-launch
-Version: 3.6.8
+Version: 3.6.9
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.6.8/energyplus_launch.egg-info/SOURCES.txt` & `energyplus_launch-3.6.9/energyplus_launch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/interface/config.py` & `energyplus_launch-3.6.9/eplaunch/interface/config.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/interface/dialog_external_viewers.py` & `energyplus_launch-3.6.9/eplaunch/interface/dialog_external_viewers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from platform import system
 from tkinter import Tk, Toplevel, Label, Listbox, SINGLE, Variable, Entry, DISABLED, StringVar, Button, Frame, \
     filedialog, E, EW, W, LEFT, messagebox
 from typing import Dict, List, Optional
 from pathlib import Path
 
+from eplaunch.interface import set_dialog_geometry
+
 
 class TkViewerDialog(Toplevel):
     CLOSE_SIGNAL_OK = 0
     CLOSE_SIGNAL_CANCEL = 1
 
     def __init__(self, parent_window, list_of_suffixes: List[str], dict_of_viewer_overrides: Dict[str, Optional[Path]]):
         super().__init__()
         self.title("Viewers")
         self.exit_code = self.CLOSE_SIGNAL_CANCEL
         self.suffixes = ['txt'] + list_of_suffixes
         self.extension_to_viewer = dict_of_viewer_overrides
         self._define_tk_variables()
         self._build_gui()
-        self.update_idletasks()
-        self.geometry(
-            "%dx%d+%d+%d" % (
-                self.winfo_width(), self.winfo_height(), parent_window.winfo_x() + 25, parent_window.winfo_y() + 25
-            )
-        )
+        set_dialog_geometry(self, parent_window)
         self.grab_set()
         self.transient(parent_window)
 
     def _define_tk_variables(self):
         self._tk_var_extension_list = Variable()
         self._tk_var_application_path = StringVar()
```

### Comparing `energyplus_launch-3.6.8/eplaunch/interface/dialog_generic.py` & `energyplus_launch-3.6.9/eplaunch/interface/dialog_generic.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/interface/dialog_output.py` & `energyplus_launch-3.6.9/eplaunch/interface/dialog_output.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/interface/dialog_weather.py` & `energyplus_launch-3.6.9/eplaunch/interface/dialog_weather.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from pathlib import Path
-from tkinter import Tk, Toplevel, StringVar, Button, EW, Entry, ALL, DISABLED, filedialog, Label, OptionMenu, E, \
-    HORIZONTAL
+from platform import system
+from tkinter import Tk, Toplevel, StringVar, EW, Entry, ALL, DISABLED, filedialog, Label, OptionMenu, E, HORIZONTAL
+if system() == 'Darwin':
+    from tkmacosx import Button
+else:
+    from tkinter.ttk import Button
 from tkinter.ttk import Separator
 from typing import List, Optional
 
+from eplaunch.interface import set_dialog_geometry
+
 
 class TkWeatherDialog(Toplevel):
     CLOSE_SIGNAL_OK = 0
     CLOSE_SIGNAL_CANCEL = 1
     WEATHER_TYPE_DD = "DD"
     WEATHER_TYPE_EPW = "EPW"
 
@@ -18,49 +24,45 @@
         # assume cancel to allow for closing the dialog with the X
         self.exit_code = self.CLOSE_SIGNAL_CANCEL
         self.selected_weather_file: Optional[Path] = None
         self._epw_from_select = None
         # build the gui and call required modal methods
         self._define_tk_variables()
         self._build_gui(recent_files)
-        self.update_idletasks()
-        self.geometry(
-            "%dx%d+%d+%d" % (
-                self.winfo_width(), self.winfo_height(), parent_window.winfo_x() + 25, parent_window.winfo_y() + 25
-            )
-        )
+        set_dialog_geometry(self, parent_window)
         self.grab_set()
         self.transient(parent_window)
 
     def _define_tk_variables(self):
         self._tk_var_recent = StringVar(value="")
         self._tk_var_recent.trace('w', self._recent_changed)
         self._tk_var_select_epw_name = StringVar(value="<select_an_epw>")
 
     def _build_gui(self, recent_files: List[Path]):
         pad = {'padx': 3, 'pady': 3}
+        button_text = "Choose This Configuration"
         if self.alt_text:
             Label(self, text=self.alt_text).grid(row=0, column=0, columnspan=3, sticky=EW, **pad)
             Separator(self, orient=HORIZONTAL).grid(row=1, column=0, columnspan=3, sticky=EW, **pad)
         Label(self, text="No Weather File (Design Run)").grid(row=2, column=0, columnspan=2, sticky=E, **pad)
-        Button(self, text="Go", command=self._go_dd).grid(row=2, column=2, sticky=EW, **pad)
+        Button(self, text=button_text, command=self._go_dd).grid(row=2, column=2, sticky=EW, **pad)
         Separator(self, orient=HORIZONTAL).grid(row=3, column=0, columnspan=3, sticky=EW, **pad)
         if recent_files:
             self._epw_from_recent = None
             self._recent_file_paths = recent_files
             self._recent_file_names = [x.name for x in recent_files]
             Label(self, text="Use Recent").grid(row=4, column=0, sticky=E, **pad)
             self.recent_options = OptionMenu(self, self._tk_var_recent, *self._recent_file_names)
             self.recent_options.grid(row=4, column=1, sticky=EW, **pad)
-            Button(self, text="Go", command=self._go_recent).grid(row=4, column=2, sticky=EW, **pad)
+            Button(self, text=button_text, command=self._go_recent).grid(row=4, column=2, sticky=EW, **pad)
             Separator(self, orient=HORIZONTAL).grid(row=5, column=0, columnspan=3, sticky=EW, **pad)
             self._tk_var_recent.set(str(self._recent_file_names[0]))
         Button(self, text="Select EPW", command=self._select_epw).grid(row=6, column=0, sticky=EW, **pad)
         Entry(self, textvariable=self._tk_var_select_epw_name, state=DISABLED).grid(row=6, column=1, sticky=EW, **pad)
-        Button(self, text="Go", command=self._go_select).grid(row=6, column=2, sticky=EW, **pad)
+        Button(self, text=button_text, command=self._go_select).grid(row=6, column=2, sticky=EW, **pad)
         Separator(self, orient=HORIZONTAL).grid(row=7, column=0, columnspan=3, sticky=EW, **pad)
         Button(self, text="Cancel", command=self._cancel).grid(row=8, column=0, columnspan=3, **pad)
         self.grid_rowconfigure(ALL, weight=1)
         self.grid_columnconfigure(ALL, weight=1)
 
     def _recent_changed(self, *_):
         selected_name = self._tk_var_recent.get()
```

### Comparing `energyplus_launch-3.6.8/eplaunch/interface/dialog_workflow_dirs.py` & `energyplus_launch-3.6.9/eplaunch/interface/dialog_workflow_dirs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from pathlib import Path
 from tkinter import Tk, Toplevel, Frame, Button, EW, NSEW, Listbox, Variable, SINGLE, Scrollbar, LEFT, BOTH, RIGHT, ALL
 from tkinter.filedialog import askdirectory
 from tkinter.messagebox import showerror
 from typing import List
 
+from eplaunch.interface import set_dialog_geometry
+
 
 class TkWorkflowsDialog(Toplevel):
     CLOSE_SIGNAL_OK = 0
     CLOSE_SIGNAL_CANCEL = 1
 
     def __init__(self, parent_window, current_workflow_dirs: List[Path], auto_found_workflow_dirs: List[Path]):
         super().__init__()
@@ -16,20 +18,15 @@
         self.exit_code = self.CLOSE_SIGNAL_CANCEL
         self.list_of_directories: List[Path] = []
         self._auto_find_dirs = auto_found_workflow_dirs
         self._tk_var_all_directories = Variable(value=current_workflow_dirs)
         self.selected_index = -1
         # build the gui and call required modal methods
         self._build_gui()
-        self.update_idletasks()
-        self.geometry(
-            "%dx%d+%d+%d" % (
-                self.winfo_width(), self.winfo_height(), parent_window.winfo_x() + 25, parent_window.winfo_y() + 25
-            )
-        )
+        set_dialog_geometry(self, parent_window)
         self.grab_set()
         self.transient(parent_window)
 
     def _update_from_traces(self, _=None):
         selected_indices = self.listbox.curselection()
         if len(selected_indices) != 1:
             self.selected_index = -1
```

### Comparing `energyplus_launch-3.6.8/eplaunch/interface/frame_main.py` & `energyplus_launch-3.6.9/eplaunch/interface/frame_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
 
 class EPLaunchWindow(Tk):
 
     # region Construction and GUI building functions
 
     def __init__(self):
+        fixup_taskbar_icon_on_windows(NAME)
         super().__init__(className=NAME)
         # set the form title and icon, basic stuff
         self.title("EnergyPlus Launch")
         self.option_add('*Dialog.msg.font', 'Helvetica 12')
         if system() == 'Darwin':
             self.icon_path = Path(__file__).resolve().parent.parent / 'icons' / 'icon.icns'
             if self.icon_path.exists():
@@ -66,15 +67,14 @@
         else:  # Linux
             self.icon_path = Path(__file__).resolve().parent.parent / 'icons' / 'icon.png'
             img = PhotoImage(file=str(self.icon_path))
             if self.icon_path.exists():
                 self.iconphoto(False, img)
             else:
                 print(f"Could not set icon for Windows, expecting to find it at {self.icon_path}")
-        fixup_taskbar_icon_on_windows(NAME)
         self.pad = {'padx': 3, 'pady': 3}
         self.dd_only_string = '<No_Weather_File>'  # Can we change to just using blank?  It's fine for now.
         self.generic_dialogs = TkGenericDialog(self.pad)
 
         # check the version of python for whether we can show extended UTF characters
         self.extended_utf8 = version_info >= (3, 7, 6)
 
@@ -812,55 +812,41 @@
             cache.add_config(
                 self.workflow_manager.current_workflow.name,
                 selected_file_name,
                 {'weather': str(new_weather_path)}
             )
         self._update_file_list()
 
-    def _set_weather_for_current_group(self):
+    def _apply_weather_to_a_file_list(self, list_of_file_paths: List[Path]):
         dialog_weather = TkWeatherDialog(self, list(self.conf.weathers_recent))
         self.wait_window(dialog_weather)
         if dialog_weather.exit_code == TkWeatherDialog.CLOSE_SIGNAL_CANCEL:
             return
         if not dialog_weather.selected_weather_file:
             weather_file_to_use = self.dd_only_string
         else:
             weather_file_to_use = dialog_weather.selected_weather_file
             if weather_file_to_use not in self.conf.weathers_recent:
                 self.conf.weathers_recent.appendleft(weather_file_to_use)
                 self._repopulate_recent_weather_list(weather_file_to_use)
-        for selected_path in self.conf.group_locations:
+        for selected_path in list_of_file_paths:
             workflow_directory_cache = CacheFile(selected_path.parent)
             workflow_directory_cache.add_config(
                 self.workflow_manager.current_workflow.name,
                 selected_path.name,
                 {'weather': str(weather_file_to_use)}
             )
         self._update_file_list()
 
+    def _set_weather_for_current_group(self):
+        self._apply_weather_to_a_file_list(self.conf.group_locations)
+
     def _open_weather_dialog(self) -> None:
-        dialog_weather = TkWeatherDialog(self, list(self.conf.weathers_recent))
-        self.wait_window(dialog_weather)
-        if dialog_weather.exit_code == TkWeatherDialog.CLOSE_SIGNAL_CANCEL:
-            return
-        if not dialog_weather.selected_weather_file:
-            weather_file_to_use = self.dd_only_string
-        else:
-            weather_file_to_use = dialog_weather.selected_weather_file
-            if weather_file_to_use not in self.conf.weathers_recent:
-                self.conf.weathers_recent.appendleft(weather_file_to_use)
-                self._repopulate_recent_weather_list(weather_file_to_use)
-        for selected_file_name in self.conf.file_selection:
-            workflow_directory_cache = CacheFile(self.conf.directory)
-            workflow_directory_cache.add_config(
-                self.workflow_manager.current_workflow.name,
-                selected_file_name,
-                {'weather': str(weather_file_to_use)}
-            )
-        self._update_file_list()
+        current_paths = [self.conf.directory / x for x in self.conf.file_selection]
+        self._apply_weather_to_a_file_list(current_paths)
 
     # endregion
 
     # region workflow running, tracking, callbacks and handlers
 
     def _repopulate_workflow_context_menu(self):
         """Clears and repopulates the workflow context menu; tries to reselect the last context saved in config"""
@@ -1050,15 +1036,14 @@
             # since we could be asking for many files, we don't want to ask for each
             # get a backup file to use only once, and apply that to any missing ones as needed
             if backup_weather_file_to_use:
                 weather_file_to_use = backup_weather_file_to_use
             else:
                 # if we need weather, didn't find one in the cache, and didn't have a backup, ask for one now
                 recent_files = list(self.conf.weathers_recent)
-                # favorite_files = self.conf.weathers_favorite
                 w = TkWeatherDialog(self, recent_files, "*At least one file is missing a weather configuration*")
                 self.wait_window(w)
                 if w.exit_code == TkWeatherDialog.CLOSE_SIGNAL_CANCEL:
                     return False, '', ''
                 else:  # a valid response was encountered
                     if not w.selected_weather_file:
                         weather_file_to_use = self.dd_only_string
@@ -1361,17 +1346,28 @@
             #         Popen(['gtk-launch', desktop_file, full_path])
             #     else:  # try falling back to the default application
             #         Popen(['xdg-open', full_path])
             # else:
             #     Popen(['xdg-open', full_path])
         else:  # assuming Mac
             if text_file_override:  # will open in the default text editor specifically
-                Popen(['open', '-t', full_path])
+                Popen(['open', '-e', full_path])
             else:
-                Popen(['open', full_path])
+                # alright, because we are trying to launch using `open`, we are severely limited
+                # in how much information we can get out of the running child process
+                # we can get info about the actual `open` process, but not the process that `open` spawns
+                # it is launched as a new process whose parent is simply launchd (root)
+                # I tried checking the running status of the open process, child subprocesses, and even
+                # some hacky tricks to check the incremental PID after the open call, and nothing worked
+                # reliably.  So I'm just going to pick a few known file extensions that I feel comfortable
+                # dispatching to a default program (htm, html, csv), and then send everything else to text
+                if full_path.endswith('htm') or full_path.endswith('html') or full_path.endswith('csv'):
+                    Popen(['open', full_path])
+                else:
+                    Popen(['open', '-e', full_path])
 
     def _open_text_editor(self) -> None:
         for file_name in self.conf.file_selection:
             full_path_str = self.conf.directory / file_name
             if 'txt' in self.conf.viewer_overrides and self.conf.viewer_overrides['txt']:
                 text_editor_binary = str(self.conf.viewer_overrides['txt'])
                 Popen([text_editor_binary, full_path_str])
```

### Comparing `energyplus_launch-3.6.8/eplaunch/interface/widget_dir_list.py` & `energyplus_launch-3.6.9/eplaunch/interface/widget_dir_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/interface/widget_file_list.py` & `energyplus_launch-3.6.9/eplaunch/interface/widget_file_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/interface/widget_group_list.py` & `energyplus_launch-3.6.9/eplaunch/interface/widget_group_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/utilities/cache.py` & `energyplus_launch-3.6.9/eplaunch/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/utilities/crossplatform.py` & `energyplus_launch-3.6.9/eplaunch/utilities/crossplatform.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/utilities/version.py` & `energyplus_launch-3.6.9/eplaunch/utilities/version.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/workflows/base.py` & `energyplus_launch-3.6.9/eplaunch/workflows/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/workflows/default/file_details.py` & `energyplus_launch-3.6.9/eplaunch/workflows/default/file_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/workflows/default/idf_details.py` & `energyplus_launch-3.6.9/eplaunch/workflows/default/idf_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/workflows/default/site_location.py` & `energyplus_launch-3.6.9/eplaunch/workflows/default/site_location.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/workflows/manager.py` & `energyplus_launch-3.6.9/eplaunch/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/workflows/workflow.py` & `energyplus_launch-3.6.9/eplaunch/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/workflows/workflow_tester.py` & `energyplus_launch-3.6.9/eplaunch/workflows/workflow_tester.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/eplaunch/workflows/workflow_thread.py` & `energyplus_launch-3.6.9/eplaunch/workflows/workflow_thread.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.8/setup.py` & `energyplus_launch-3.6.9/setup.py`

 * *Files identical despite different names*

