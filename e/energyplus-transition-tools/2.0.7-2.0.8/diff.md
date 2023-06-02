# Comparing `tmp/energyplus_transition_tools-2.0.7.tar.gz` & `tmp/energyplus_transition_tools-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_transition_tools-2.0.7.tar", last modified: Fri Apr 14 16:21:38 2023, max compression
+gzip compressed data, was "energyplus_transition_tools-2.0.8.tar", last modified: Fri Jun  2 21:10:58 2023, max compression
```

## Comparing `energyplus_transition_tools-2.0.7.tar` & `energyplus_transition_tools-2.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:21:38.865039 energyplus_transition_tools-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-04-14 16:21:38.865039 energyplus_transition_tools-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:21:38.865039 energyplus_transition_tools-2.0.7/energyplus_transition/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      357 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/configure.py
--rw-r--r--   0 runner    (1001) docker     (122)     3769 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/energyplus_path.py
--rw-r--r--   0 runner    (1001) docker     (122)    20887 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/gui.py
--rw-r--r--   0 runner    (1001) docker     (122)     9640 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/international.py
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1517 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/transition_binary.py
--rw-r--r--   0 runner    (1001) docker     (122)     5286 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/transition_run_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:21:38.865039 energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-04-14 16:21:38.000000 energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-14 16:21:38.000000 energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 16:21:38.000000 energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-04-14 16:21:38.000000 energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-14 16:21:38.000000 energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-14 16:21:38.000000 energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-04-14 16:21:38.865039 energyplus_transition_tools-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:10:58.149353 energyplus_transition_tools-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-06-02 21:10:45.000000 energyplus_transition_tools-2.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-06-02 21:10:58.149353 energyplus_transition_tools-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-06-02 21:10:45.000000 energyplus_transition_tools-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:10:58.145353 energyplus_transition_tools-2.0.8/energyplus_transition/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-02 21:10:45.000000 energyplus_transition_tools-2.0.8/energyplus_transition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-02 21:10:45.000000 energyplus_transition_tools-2.0.8/energyplus_transition/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      357 2023-06-02 21:10:45.000000 energyplus_transition_tools-2.0.8/energyplus_transition/configure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3769 2023-06-02 21:10:45.000000 energyplus_transition_tools-2.0.8/energyplus_transition/energyplus_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20887 2023-06-02 21:10:45.000000 energyplus_transition_tools-2.0.8/energyplus_transition/gui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9640 2023-06-02 21:10:45.000000 energyplus_transition_tools-2.0.8/energyplus_transition/international.py
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-06-02 21:10:45.000000 energyplus_transition_tools-2.0.8/energyplus_transition/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1517 2023-06-02 21:10:45.000000 energyplus_transition_tools-2.0.8/energyplus_transition/transition_binary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5286 2023-06-02 21:10:45.000000 energyplus_transition_tools-2.0.8/energyplus_transition/transition_run_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 21:10:58.149353 energyplus_transition_tools-2.0.8/energyplus_transition_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-06-02 21:10:57.000000 energyplus_transition_tools-2.0.8/energyplus_transition_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-02 21:10:57.000000 energyplus_transition_tools-2.0.8/energyplus_transition_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 21:10:57.000000 energyplus_transition_tools-2.0.8/energyplus_transition_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-06-02 21:10:57.000000 energyplus_transition_tools-2.0.8/energyplus_transition_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-02 21:10:57.000000 energyplus_transition_tools-2.0.8/energyplus_transition_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-06-02 21:10:57.000000 energyplus_transition_tools-2.0.8/energyplus_transition_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-06-02 21:10:58.149353 energyplus_transition_tools-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-06-02 21:10:45.000000 energyplus_transition_tools-2.0.8/setup.py
```

### Comparing `energyplus_transition_tools-2.0.7/LICENSE.txt` & `energyplus_transition_tools-2.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `energyplus_transition_tools-2.0.7/PKG-INFO` & `energyplus_transition_tools-2.0.8/energyplus_transition_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: energyplus_transition_tools
-Version: 2.0.7
+Name: energyplus-transition-tools
+Version: 2.0.8
 Summary: A library and tkinter-based tool for transitioning EnergyPlus input files
 Home-page: https://github.com/myoldmopar/EnergyPlusTransitionTools
 Author: Edwin Lee, for NREL, for the United States Department of Energy
 License: ModifiedBSD
 Description: # EnergyPlusTransitionTools
         
         A library of transition functionality.
```

### Comparing `energyplus_transition_tools-2.0.7/README.md` & `energyplus_transition_tools-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_transition_tools-2.0.7/energyplus_transition/energyplus_path.py` & `energyplus_transition_tools-2.0.8/energyplus_transition/energyplus_path.py`

 * *Files identical despite different names*

### Comparing `energyplus_transition_tools-2.0.7/energyplus_transition/gui.py` & `energyplus_transition_tools-2.0.8/energyplus_transition/gui.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 class VersionUpdaterWindow(Tk):
     """ The main window, or Tk(), for the IDFVersionUpdater program.
     This initializer function creates instance variables, sets up threading, and builds the GUI"""
 
     # region class construction and basic event/closing functions
 
     def __init__(self):
+        fixup_taskbar_icon_on_windows(NAME)
         super().__init__(className=NAME)
 
         if system() == 'Darwin':
             self.icon_path = Path(__file__).resolve().parent / 'icons' / 'icon.icns'
             if self.icon_path.exists():
                 self.iconbitmap(str(self.icon_path))
             else:
@@ -98,15 +99,14 @@
         else:  # Linux
             self.icon_path = Path(__file__).resolve().parent / 'icons' / 'icon.png'
             img = PhotoImage(file=str(self.icon_path))
             if self.icon_path.exists():
                 self.iconphoto(False, img)
             else:
                 print(f"Could not set icon for Windows, expecting to find it at {self.icon_path}")
-        fixup_taskbar_icon_on_windows(NAME)
 
         self._gui_queue = Queue()
         self._check_queue()
 
         # load the settings here very early
         self.conf = Configuration()
```

### Comparing `energyplus_transition_tools-2.0.7/energyplus_transition/international.py` & `energyplus_transition_tools-2.0.8/energyplus_transition/international.py`

 * *Files identical despite different names*

### Comparing `energyplus_transition_tools-2.0.7/energyplus_transition/transition_binary.py` & `energyplus_transition_tools-2.0.8/energyplus_transition/transition_binary.py`

 * *Files identical despite different names*

### Comparing `energyplus_transition_tools-2.0.7/energyplus_transition/transition_run_thread.py` & `energyplus_transition_tools-2.0.8/energyplus_transition/transition_run_thread.py`

 * *Files identical despite different names*

### Comparing `energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/PKG-INFO` & `energyplus_transition_tools-2.0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: energyplus-transition-tools
-Version: 2.0.7
+Name: energyplus_transition_tools
+Version: 2.0.8
 Summary: A library and tkinter-based tool for transitioning EnergyPlus input files
 Home-page: https://github.com/myoldmopar/EnergyPlusTransitionTools
 Author: Edwin Lee, for NREL, for the United States Department of Energy
 License: ModifiedBSD
 Description: # EnergyPlusTransitionTools
         
         A library of transition functionality.
```

### Comparing `energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/SOURCES.txt` & `energyplus_transition_tools-2.0.8/energyplus_transition_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_transition_tools-2.0.7/setup.py` & `energyplus_transition_tools-2.0.8/setup.py`

 * *Files identical despite different names*

