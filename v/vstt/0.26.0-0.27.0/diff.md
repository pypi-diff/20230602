# Comparing `tmp/vstt-0.26.0.tar.gz` & `tmp/vstt-0.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstt-0.26.0.tar", last modified: Thu Jun  1 13:11:05 2023, max compression
+gzip compressed data, was "vstt-0.27.0.tar", last modified: Fri Jun  2 12:47:36 2023, max compression
```

## Comparing `vstt-0.26.0.tar` & `vstt-0.27.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:05.591822 vstt-0.26.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-01 13:10:53.000000 vstt-0.26.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 13:11:05.591822 vstt-0.26.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-01 13:10:53.000000 vstt-0.26.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-01 13:10:53.000000 vstt-0.26.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:11:05.591822 vstt-0.26.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:05.587822 vstt-0.26.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:05.587822 vstt-0.26.0/src/vstt/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-06-01 13:10:53.000000 vstt-0.26.0/src/vstt/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:05.587822 vstt-0.26.0/src/vstt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 13:11:05.000000 vstt-0.26.0/src/vstt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-01 13:11:05.000000 vstt-0.26.0/src/vstt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:11:05.000000 vstt-0.26.0/src/vstt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-01 13:11:05.000000 vstt-0.26.0/src/vstt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-01 13:11:05.000000 vstt-0.26.0/src/vstt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 13:11:05.000000 vstt-0.26.0/src/vstt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:11:05.591822 vstt-0.26.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_vis.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-01 13:10:53.000000 vstt-0.26.0/tests/test_vstt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:47:36.739976 vstt-0.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-02 12:47:25.000000 vstt-0.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-02 12:47:36.739976 vstt-0.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-02 12:47:25.000000 vstt-0.27.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-02 12:47:25.000000 vstt-0.27.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 12:47:36.739976 vstt-0.27.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:47:36.735976 vstt-0.27.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:47:36.735976 vstt-0.27.0/src/vstt/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11314 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-06-02 12:47:25.000000 vstt-0.27.0/src/vstt/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:47:36.739976 vstt-0.27.0/src/vstt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-02 12:47:36.000000 vstt-0.27.0/src/vstt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-02 12:47:36.000000 vstt-0.27.0/src/vstt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 12:47:36.000000 vstt-0.27.0/src/vstt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-02 12:47:36.000000 vstt-0.27.0/src/vstt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-02 12:47:36.000000 vstt-0.27.0/src/vstt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-02 12:47:36.000000 vstt-0.27.0/src/vstt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:47:36.739976 vstt-0.27.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-02 12:47:25.000000 vstt-0.27.0/tests/test_vstt.py
```

### Comparing `vstt-0.26.0/LICENSE` & `vstt-0.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/PKG-INFO` & `vstt-0.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 0.26.0
+Version: 0.27.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
 Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `vstt-0.26.0/README.md` & `vstt-0.27.0/README.md`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/pyproject.toml` & `vstt-0.27.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,23 @@
   "Operating System :: POSIX :: Linux",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
-dependencies = ["psychopy", "psychopy-sounddevice", "numpy", "click", "PyQt5"]
+dependencies = [
+  "psychopy",
+  "psychopy-sounddevice",
+  "numpy",
+  "click",
+  "PyQt5",
+  "requests",
+  "packaging"
+]
 dynamic = ["version"]
 
 [project.scripts]
 vstt = "vstt.__main__:main"
 
 [project.urls]
 Github = "https://github.com/ssciwr/vstt"
```

### Comparing `vstt-0.26.0/src/vstt/__main__.py` & `vstt-0.27.0/src/vstt/__main__.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/common.py` & `vstt-0.27.0/src/vstt/common.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/display.py` & `vstt-0.27.0/src/vstt/display.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/display_widget.py` & `vstt-0.27.0/src/vstt/display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/experiment.py` & `vstt-0.27.0/src/vstt/experiment.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/geom.py` & `vstt-0.27.0/src/vstt/geom.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/gui.py` & `vstt-0.27.0/src/vstt/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from PyQt5.QtCore import Qt
 from vstt.display_widget import DisplayOptionsWidget
 from vstt.experiment import Experiment
 from vstt.meta_widget import MetadataWidget
 from vstt.results_widget import ResultsWidget
 from vstt.task import MotorTask
 from vstt.trials_widget import TrialsWidget
+from vstt.update import check_for_new_version
+from vstt.update import do_pip_upgrade
 
 
 class Gui(QtWidgets.QMainWindow):
     def __init__(self, filename: Optional[str] = None, win: Optional[Window] = None):
         super().__init__()
         self.experiment = Experiment()
         self._win = win
@@ -221,14 +223,34 @@
         QtWidgets.QMessageBox.about(
             self,
             "About VSTT",
             f"Visuomotor Serial Targeting Task (VSTT)\n\nVersion {vstt.__version__}\n\n"
             + "https://ssciwr.github.io/vstt",
         )
 
+    def check_for_updates(self) -> None:
+        title = "Update VSTT"
+        QtWidgets.QApplication.setOverrideCursor(Qt.WaitCursor)
+        new_version_available, new_version_message = check_for_new_version()
+        QtWidgets.QApplication.restoreOverrideCursor()
+        if not new_version_available:
+            QtWidgets.QMessageBox.information(
+                self,
+                title,
+                new_version_message,
+            )
+            return
+        yes_no = QtWidgets.QMessageBox.question(self, title, new_version_message)
+        if yes_no != QtWidgets.QMessageBox.Yes:
+            return
+        QtWidgets.QApplication.setOverrideCursor(Qt.WaitCursor)
+        upgrade_success, upgrade_message = do_pip_upgrade()
+        QtWidgets.QApplication.restoreOverrideCursor()
+        QtWidgets.QMessageBox.information(self, title, upgrade_message)
+
 
 def _add_action(
     name: str,
     callback: Callable,
     menu: QtWidgets.QMenu,
     toolbar: Optional[QtWidgets.QToolBar] = None,
     shortcut: Optional[str] = None,
@@ -296,9 +318,10 @@
         experiment_menu,
         toolbar,
         "Ctrl+R",
         QtWidgets.QStyle.SP_DialogYesButton,
     )
     help_menu = menu.addMenu("&Help")
     _add_action("&About", gui.about, help_menu)
+    _add_action("&Check for updates", gui.check_for_updates, help_menu)
     toolbar.setContextMenuPolicy(Qt.PreventContextMenu)
     return toolbar
```

### Comparing `vstt-0.26.0/src/vstt/joystick_wrapper.py` & `vstt-0.27.0/src/vstt/joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/meta.py` & `vstt-0.27.0/src/vstt/meta.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/meta_widget.py` & `vstt-0.27.0/src/vstt/meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/results_widget.py` & `vstt-0.27.0/src/vstt/results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/stat.py` & `vstt-0.27.0/src/vstt/stat.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/task.py` & `vstt-0.27.0/src/vstt/task.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/trial.py` & `vstt-0.27.0/src/vstt/trial.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/trials_widget.py` & `vstt-0.27.0/src/vstt/trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/types.py` & `vstt-0.27.0/src/vstt/types.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt/vis.py` & `vstt-0.27.0/src/vstt/vis.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/src/vstt.egg-info/PKG-INFO` & `vstt-0.27.0/src/vstt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 0.26.0
+Version: 0.27.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
 Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `vstt-0.26.0/src/vstt.egg-info/SOURCES.txt` & `vstt-0.27.0/src/vstt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/vstt/meta_widget.py
 src/vstt/results_widget.py
 src/vstt/stat.py
 src/vstt/task.py
 src/vstt/trial.py
 src/vstt/trials_widget.py
 src/vstt/types.py
+src/vstt/update.py
 src/vstt/vis.py
 src/vstt.egg-info/PKG-INFO
 src/vstt.egg-info/SOURCES.txt
 src/vstt.egg-info/dependency_links.txt
 src/vstt.egg-info/entry_points.txt
 src/vstt.egg-info/requires.txt
 src/vstt.egg-info/top_level.txt
@@ -36,9 +37,10 @@
 tests/test_meta.py
 tests/test_meta_widget.py
 tests/test_results_widget.py
 tests/test_stat.py
 tests/test_task.py
 tests/test_trial.py
 tests/test_trials_widget.py
+tests/test_update.py
 tests/test_vis.py
 tests/test_vstt.py
```

### Comparing `vstt-0.26.0/tests/test_display.py` & `vstt-0.27.0/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/tests/test_display_widget.py` & `vstt-0.27.0/tests/test_display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/tests/test_experiment.py` & `vstt-0.27.0/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/tests/test_geom.py` & `vstt-0.27.0/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/tests/test_gui.py` & `vstt-0.27.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/tests/test_joystick_wrapper.py` & `vstt-0.27.0/tests/test_joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/tests/test_meta.py` & `vstt-0.27.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/tests/test_meta_widget.py` & `vstt-0.27.0/tests/test_meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/tests/test_results_widget.py` & `vstt-0.27.0/tests/test_results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/tests/test_stat.py` & `vstt-0.27.0/tests/test_stat.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/tests/test_task.py` & `vstt-0.27.0/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/tests/test_trial.py` & `vstt-0.27.0/tests/test_trial.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/tests/test_trials_widget.py` & `vstt-0.27.0/tests/test_trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.26.0/tests/test_vis.py` & `vstt-0.27.0/tests/test_vis.py`

 * *Files identical despite different names*

