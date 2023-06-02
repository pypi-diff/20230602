# Comparing `tmp/civilpy-0.0.44.tar.gz` & `tmp/civilpy-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civilpy-0.0.44.tar", last modified: Thu May 11 11:24:08 2023, max compression
+gzip compressed data, was "civilpy-0.0.45.tar", last modified: Fri Jun  2 14:28:51 2023, max compression
```

## Comparing `civilpy-0.0.44.tar` & `civilpy-0.0.45.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-05-11 11:24:08.676026 civilpy-0.0.44/
--rw-rw-r--   0 dane      (1000) dane      (1000)     1688 2023-05-11 11:08:17.000000 civilpy-0.0.44/.gitlab-ci.yml
--rw-rw-r--   0 dane      (1000) dane      (1000)     1088 2023-05-11 11:08:17.000000 civilpy-0.0.44/LICENSE
--rw-rw-r--   0 dane      (1000) dane      (1000)      112 2023-05-11 11:08:17.000000 civilpy-0.0.44/MANIFEST.in
--rw-rw-r--   0 dane      (1000) dane      (1000)     4750 2023-05-11 11:24:08.676026 civilpy-0.0.44/PKG-INFO
--rw-rw-r--   0 dane      (1000) dane      (1000)     4148 2023-05-11 11:08:17.000000 civilpy-0.0.44/README.md
--rw-rw-r--   0 dane      (1000) dane      (1000)       24 2023-05-11 11:08:17.000000 civilpy-0.0.44/pytest.ini
--rw-rw-r--   0 dane      (1000) dane      (1000)      236 2023-05-11 11:08:17.000000 civilpy-0.0.44/requirements.txt
--rw-rw-r--   0 dane      (1000) dane      (1000)       38 2023-05-11 11:24:08.676026 civilpy-0.0.44/setup.cfg
--rw-rw-r--   0 dane      (1000) dane      (1000)     2530 2023-05-11 11:23:48.000000 civilpy-0.0.44/setup.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-05-11 11:24:08.668026 civilpy-0.0.44/src/
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-05-11 11:24:08.672026 civilpy-0.0.44/src/civilpy/
--rw-rw-r--   0 dane      (1000) dane      (1000)      118 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/CLI.py
--rw-rw-r--   0 dane      (1000) dane      (1000)      111 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/__init__.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-05-11 11:24:08.672026 civilpy-0.0.44/src/civilpy/construction/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/construction/__init__.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-05-11 11:24:08.672026 civilpy-0.0.44/src/civilpy/environmental/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/environmental/__init__.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-05-11 11:24:08.672026 civilpy-0.0.44/src/civilpy/general/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/general/__init__.py
--rw-rw-r--   0 dane      (1000) dane      (1000)     1027 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/general/database_tools.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/general/gis.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/general/kml_tools.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/general/math.py
--rw-rw-r--   0 dane      (1000) dane      (1000)     5919 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/general/microstation.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/general/pdf.py
--rw-rw-r--   0 dane      (1000) dane      (1000)     2519 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/general/photos.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/general/physics.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/general/plan_development.py
--rw-rw-r--   0 dane      (1000) dane      (1000)       78 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/general/pointclouds.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-05-11 11:24:08.672026 civilpy-0.0.44/src/civilpy/geotechnical/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/geotechnical/__init__.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-05-11 11:24:08.672026 civilpy-0.0.44/src/civilpy/state/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/state/__init__.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-05-11 11:24:08.676026 civilpy-0.0.44/src/civilpy/state/ohio/
--rw-rw-r--   0 dane      (1000) dane      (1000)     2589 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/state/ohio/D6_file_explorer.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/state/ohio/__init__.py
--rw-rw-r--   0 dane      (1000) dane      (1000)    42198 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/state/ohio/dot.py
--rw-rw-r--   0 dane      (1000) dane      (1000)    16507 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/state/ohio/search_tools.py
--rw-rw-r--   0 dane      (1000) dane      (1000)    91957 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/state/ohio/snbi.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-05-11 11:24:08.676026 civilpy-0.0.44/src/civilpy/structural/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/structural/__init__.py
--rw-rw-r--   0 dane      (1000) dane      (1000)    20861 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/structural/beam_bending.py
--rw-rw-r--   0 dane      (1000) dane      (1000)     6027 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/structural/steel.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-05-11 11:24:08.676026 civilpy-0.0.44/src/civilpy/transportation/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/transportation/__init__.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-05-11 11:24:08.676026 civilpy-0.0.44/src/civilpy/water_resources/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/water_resources/__init__.py
--rw-rw-r--   0 dane      (1000) dane      (1000)    18085 2023-05-11 11:08:17.000000 civilpy-0.0.44/src/civilpy/water_resources/hydraulics.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-05-11 11:24:08.672026 civilpy-0.0.44/src/civilpy.egg-info/
--rw-rw-r--   0 dane      (1000) dane      (1000)     4750 2023-05-11 11:24:08.000000 civilpy-0.0.44/src/civilpy.egg-info/PKG-INFO
--rw-rw-r--   0 dane      (1000) dane      (1000)     1353 2023-05-11 11:24:08.000000 civilpy-0.0.44/src/civilpy.egg-info/SOURCES.txt
--rw-rw-r--   0 dane      (1000) dane      (1000)        1 2023-05-11 11:24:08.000000 civilpy-0.0.44/src/civilpy.egg-info/dependency_links.txt
--rw-rw-r--   0 dane      (1000) dane      (1000)      513 2023-05-11 11:24:08.000000 civilpy-0.0.44/src/civilpy.egg-info/requires.txt
--rw-rw-r--   0 dane      (1000) dane      (1000)        8 2023-05-11 11:24:08.000000 civilpy-0.0.44/src/civilpy.egg-info/top_level.txt
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-05-11 11:24:08.676026 civilpy-0.0.44/tests/
--rw-rw-r--   0 dane      (1000) dane      (1000)    13769 2023-05-11 11:08:17.000000 civilpy-0.0.44/tests/test_ohio_dot_bridge.py
--rw-rw-r--   0 dane      (1000) dane      (1000)     2181 2023-05-11 11:08:17.000000 civilpy-0.0.44/tests/test_ohio_dot_functions.py
--rw-rw-r--   0 dane      (1000) dane      (1000)     5519 2023-05-11 11:08:17.000000 civilpy-0.0.44/tests/test_ohio_dot_project.py
--rw-rw-r--   0 dane      (1000) dane      (1000)    13098 2023-05-11 11:08:17.000000 civilpy-0.0.44/tests/test_ohio_dot_snbi_transfer.py
--rw-rw-r--   0 dane      (1000) dane      (1000)     2900 2023-05-11 11:08:17.000000 civilpy-0.0.44/tests/test_steel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.677655 civilpy-0.0.45/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2023-06-02 13:37:25.000000 civilpy-0.0.45/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-02 13:37:25.000000 civilpy-0.0.45/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-02 13:37:25.000000 civilpy-0.0.45/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4750 2023-06-02 14:28:51.673655 civilpy-0.0.45/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4148 2023-06-02 13:37:25.000000 civilpy-0.0.45/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 13:37:25.000000 civilpy-0.0.45/pytest.ini
+-rw-rw-rw-   0 root         (0) root         (0)      972 2023-06-02 13:59:42.000000 civilpy-0.0.45/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 14:28:51.677655 civilpy-0.0.45/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2642 2023-06-02 13:59:42.000000 civilpy-0.0.45/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.669655 civilpy-0.0.45/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/CLI.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/construction/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/construction/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/environmental/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/environmental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/general/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/general/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/general/database_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/general/gis.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/general/kml_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/general/math.py
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/general/microstation.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/general/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/general/photos.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/general/physics.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/general/plan_development.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/general/pointclouds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/geotechnical/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/geotechnical/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/state/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/state/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/state/ohio/
+-rw-rw-rw-   0 root         (0) root         (0)     2589 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/state/ohio/D6_file_explorer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/state/ohio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42197 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/state/ohio/dot.py
+-rw-rw-rw-   0 root         (0) root         (0)    16514 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/state/ohio/search_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    91957 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/state/ohio/snbi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/structural/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/structural/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20861 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/structural/beam_bending.py
+-rw-rw-rw-   0 root         (0) root         (0)     5946 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/structural/steel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/transportation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/transportation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/water_resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/water_resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18085 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/water_resources/hydraulics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4750 2023-06-02 14:28:51.000000 civilpy-0.0.45/src/civilpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-06-02 14:28:51.000000 civilpy-0.0.45/src/civilpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 14:28:51.000000 civilpy-0.0.45/src/civilpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      577 2023-06-02 14:28:51.000000 civilpy-0.0.45/src/civilpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-02 14:28:51.000000 civilpy-0.0.45/src/civilpy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13769 2023-06-02 13:37:25.000000 civilpy-0.0.45/tests/test_ohio_dot_bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)     2181 2023-06-02 13:37:25.000000 civilpy-0.0.45/tests/test_ohio_dot_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5324 2023-06-02 13:37:25.000000 civilpy-0.0.45/tests/test_ohio_dot_project.py
+-rw-rw-rw-   0 root         (0) root         (0)    13098 2023-06-02 13:37:25.000000 civilpy-0.0.45/tests/test_ohio_dot_snbi_transfer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2900 2023-06-02 13:37:25.000000 civilpy-0.0.45/tests/test_steel.py
```

### Comparing `civilpy-0.0.44/LICENSE` & `civilpy-0.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.44/PKG-INFO` & `civilpy-0.0.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.44
+Version: 0.0.45
 Summary: Civil Engineering Tools in Python
 Home-page: https://daneparks.com/Dane/civilpy
 Author: Dane Parks
 Author-email: Dane@daneparks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.44 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.45 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
 Parks Author-email: Dane@daneparks.com Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Environment :: Console ::
 Curses Description-Content-Type: text/markdown License-File: LICENSE # CivilPy
```

### Comparing `civilpy-0.0.44/README.md` & `civilpy-0.0.45/README.md`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.44/setup.py` & `civilpy-0.0.45/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='civilpy',
-    version='0.0.44',
+    version='0.0.45',
     packages=find_packages('src', exclude=['test', 'secrets', 'docs', 'res']),
     description='Civil Engineering Tools in Python',
     url="https://daneparks.com/Dane/civilpy",
     author_email="Dane@daneparks.com",
     author="Dane Parks",
     py_modules=[
         "civilpy.state.ohio.dot",
@@ -41,15 +41,15 @@
         "Environment :: Console :: Curses",
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "numpy>=1.14.5",
         "folium>=0.12.1",
-        "pandas>=1.5.3",
+        "pandas>=1.1.5",
         "Pillow>=9.4.0",
         "Pint>=0.18.2",
         "coverage>=7.1.0",
         "matplotlib>=3.6.3",
         "webdriver-manager>=3.8.5",
         "selenium>=3.141.0",
         "msedge-selenium-tools>=3.141.4",
@@ -69,13 +69,17 @@
         "tifftools>=1.3.7",
         "natsort>=8.2.0",
         "html5lib>=1.1",
         "requests>=2.28.2",
         "pyntcloud>=0.3.1",
         "laspy>=2.4.1",
         "openpyxl>=3.1.2",
-        "earthpy>=0.9.4"
+        "earthpy>=0.9.4",
+        "pymupdf>=1.22.3",
+        "tqdm>=4.65.0",
+        "pyodbc>=4.0.39",
+        "pytesseract>=0.3.10"
     ],
 
     extras_require={
     }
 )
```

### Comparing `civilpy-0.0.44/src/civilpy/general/database_tools.py` & `civilpy-0.0.45/src/civilpy/general/database_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.44/src/civilpy/general/microstation.py` & `civilpy-0.0.45/src/civilpy/general/microstation.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.44/src/civilpy/general/photos.py` & `civilpy-0.0.45/src/civilpy/general/photos.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.44/src/civilpy/state/ohio/D6_file_explorer.py` & `civilpy-0.0.45/src/civilpy/state/ohio/D6_file_explorer.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.44/src/civilpy/state/ohio/dot.py` & `civilpy-0.0.45/src/civilpy/state/ohio/dot.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
             yyy     - Three digit wall number
             aa      - Two digit wall plan sheet type
             ###     - Three digit number identifying the number of drawings of the same type
     """
     print(help(help_function))
 
 
-
 basemap_labels = {
     'KB': '3D Model KB',
     'KM': '3D Modeling KM',
     'BC': 'Aerial and Ground Combined',
     'BA': 'Aerial Mapping',
     'BS': 'Bridge',
     'KD': 'Digital Terrain Model',
```

### Comparing `civilpy-0.0.44/src/civilpy/state/ohio/search_tools.py` & `civilpy-0.0.45/src/civilpy/state/ohio/search_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,14 @@
         route_num = re.sub('\D', '', route_num).lstrip('0')
         # Inserts a decimal to convert text based milepost to usable value
         section_num = self.raw_data['Straight Line Mileage'][:-3] + '.' + self.raw_data['Straight Line Mileage'][2:]
         section_num = re.sub('/[^0-9.]/g', '', section_num).lstrip('0')
 
         return f"{county_code}-{route_num}-{section_num}"
 
-
     def get_d6_plan_sets(self, district_df_path="G:\\ref\\New folder\\PLANINDX.TXT"):
         """
         Using the "CTY-RT-SEC" from a SFN, this function finds the various
         plan sets potentially associated with that structure, it rounds the 'section'
         value up and down to be inclusive, effectively giving every plan segment
         for that 1 mile segment.
 
@@ -300,15 +299,16 @@
     def tiff_to_pdf(self, tiff_path: str) -> str:
         """
         Helper function to be used by the bridge object to convert tiff files to pdf
         :param tiff_path:
         :return:
         """
         pdf_path = tiff_path.replace('.tiff', '.pdf')
-        if not os.path.exists(tiff_path): raise Exception(f'{tiff_path} does not find.')
+        if not os.path.exists(tiff_path):
+            raise Exception(f'{tiff_path} Not found.')
         image = Image.open(tiff_path)
 
         images = []
         for i, page in enumerate(ImageSequence.Iterator(image)):
             page = page.convert("RGB")
             images.append(page)
         if len(images) == 1:
```

### Comparing `civilpy-0.0.44/src/civilpy/state/ohio/snbi.py` & `civilpy-0.0.45/src/civilpy/state/ohio/snbi.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.44/src/civilpy/structural/beam_bending.py` & `civilpy-0.0.45/src/civilpy/structural/beam_bending.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.44/src/civilpy/structural/steel.py` & `civilpy-0.0.45/src/civilpy/structural/steel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import pandas as pd
-import requests
-import io
 import pint
 
 units = pint.UnitRegistry()
 
-url = 'https://daneparks.com/Dane/civilpy/-/raw/master/src/civilpy/structural/res/steel_shapes.csv'
-s = requests.get(url).content
-steel_tables = pd.read_csv(io.StringIO(s.decode('utf-8')))
+steel_tables = pd.read_csv('https://raw.githubusercontent.com/drparks71w/CivilPy/master/src/civilpy/structural/res/steel_shapes.csv')
 
 
 def hello_world(user_input="World"):
     return f"Hello {user_input}!"
 
 
 class SteelSection:
```

### Comparing `civilpy-0.0.44/src/civilpy/water_resources/hydraulics.py` & `civilpy-0.0.45/src/civilpy/water_resources/hydraulics.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.44/src/civilpy.egg-info/PKG-INFO` & `civilpy-0.0.45/src/civilpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.44
+Version: 0.0.45
 Summary: Civil Engineering Tools in Python
 Home-page: https://daneparks.com/Dane/civilpy
 Author: Dane Parks
 Author-email: Dane@daneparks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.44 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.45 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
 Parks Author-email: Dane@daneparks.com Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Environment :: Console ::
 Curses Description-Content-Type: text/markdown License-File: LICENSE # CivilPy
```

### Comparing `civilpy-0.0.44/src/civilpy.egg-info/SOURCES.txt` & `civilpy-0.0.45/src/civilpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.44/tests/test_ohio_dot_bridge.py` & `civilpy-0.0.45/tests/test_ohio_dot_bridge.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.44/tests/test_ohio_dot_functions.py` & `civilpy-0.0.45/tests/test_ohio_dot_functions.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.44/tests/test_ohio_dot_project.py` & `civilpy-0.0.45/tests/test_ohio_dot_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,93 +1,95 @@
 import unittest
 from civilpy.state.ohio.dot import Project
 
 # //TODO - Fix this test, unstable API
-# class TestProject(unittest.TestCase):
-#     def setUp(self):
-#         # Creates a 'test project' and makes sure none of the attributes have changed
-#         self.tp = Project(pid='96213')
-#
-#     def tearDown(self):
-#         pass
-#
-#     def test_init(self):
-#         # //TODO - make tests less dependent on getting specific values from project points arrays
-#         self.assertIsInstance(self.tp.objectid, int)
-#         self.assertIsInstance(self.tp.gis_id, int)
-#         self.assertEqual(self.tp.pid_nbr, 96213)
-#         self.assertEqual(self.tp.district_nbr, 6)
-#         self.assertEqual(self.tp.locale_short_nme, 'MRW')
-#         self.assertEqual(self.tp.county_nme, 'Morrow')
-#         self.assertEqual(self.tp.project_nme, 'MRW SR 314 (8.080) (20.57)')
-#         self.assertEqual(self.tp.contract_type, 'Standard Build')
-#         self.assertEqual(self.tp.primary_fund_category_txt, 'District Preservation (Pv & Br)')
-#         self.assertEqual(self.tp.project_manager_nme, 'HIPP, JEFFREY P')
-#         self.assertEqual(self.tp.reservoir_year, None)
-#         self.assertEqual(self.tp.tier, None)
-#         self.assertEqual(self.tp.odot_letting, 'ODOT Let')
-#         self.assertEqual(self.tp.schedule_type_short_nme, 'Standard')
-#         self.assertEqual(self.tp.env_project_manager_nme, 'TURNER, AMY S')
-#         self.assertEqual(self.tp.area_engineer_nme, 'DENNIS, WADE R')
-#         self.assertEqual(self.tp.project_engineer_nme, 'STOVER, DONALD L')
-#         self.assertEqual(self.tp.design_agency, 'DISTRICT 6-ENGINEERING')
-#         self.assertEqual(self.tp.sponsoring_agency, 'DISTRICT 6-PLANNING')
-#         self.assertEqual(self.tp.pdp_short_name, 'Path 2')
-#         self.assertEqual(self.tp.primary_work_category, 'Bridge Preservation')
-#         self.assertEqual(self.tp.project_status, 'Not Filed')
-#         self.assertEqual(self.tp.fiscal_year, '2024')
-#         self.assertEqual(self.tp.inhouse_design_full_nme, 'HIPP, JEFFREY P')
-#         self.assertEqual(self.tp.est_total_constr_cost, 650000)
-#         self.assertEqual(self.tp.state_project_nbr, None)
-#         self.assertEqual(self.tp.constr_vendor_nme, None)
-#         self.assertEqual(self.tp.stip_flag, None)
-#         self.assertEqual(self.tp.current_stip_co_amt, None)
-#         self.assertEqual(self.tp.project_plans_url, 'http://contracts.dot.state.oh.us/search.jsp?cabinetId=1002&PID_NUM=96213')
-#         self.assertEqual(self.tp.project_addenda_url, 'http://contracts.dot.state.oh.us/search.jsp?cabinetId=1000&PID_NUM=96213')
-#         self.assertEqual(self.tp.project_proposal_url, 'http://contracts.dot.state.oh.us/search.jsp?cabinetId=1003&PID_NUM=96213')
-#         self.assertEqual(self.tp.fmis_proj_desc, None)
-#         self.assertEqual(self.tp.award_milestone_dt, 1699228800000)
-#         self.assertEqual(self.tp.begin_constr_milestone_dt, 1713139200000)
-#         self.assertEqual(self.tp.end_constr_milestone_dt, 1722470400000)
-#         self.assertEqual(self.tp.open_traffic_dt, None)
-#         self.assertEqual(self.tp.central_office_close_dt, None)
-#         self.assertIsInstance(self.tp.source_last_updated, int)
-#         self.assertIsInstance(self.tp.cod_last_updated, int)
-#         self.assertEqual(self.tp.preserv_funds_ind, 'Y')
-#         self.assertEqual(self.tp.major_brg_funds_ind, 'N')
-#         self.assertEqual(self.tp.major_new_funds_ind, 'N')
-#         self.assertEqual(self.tp.major_rehab_funds_ind, 'N')
-#         self.assertEqual(self.tp.mpo_funds_ind, 'N')
-#         self.assertEqual(self.tp.safety_funds_ind, 'N')
-#         self.assertEqual(self.tp.local_funds_ind, 'N')
-#         self.assertEqual(self.tp.other_funds_ind, 'N')
-#         self.assertEqual(self.tp.nlf_id, 'SMRWSR00314**C')
-#         self.assertIsInstance(self.tp.ctl_begin, float)
-#         self.assertEqual(self.tp.ctl_end, None)
-#         self.assertEqual(self.tp.gis_feature_type, 'POINT')
-#         self.assertEqual(self.tp.route_type, 'SR')
-#         self.assertEqual(self.tp.route_id, '00314')
-#         self.assertIsInstance(self.tp.structure_file_nbr, str)
-#         self.assertIsInstance(self.tp.main_structure_type, str)
-#         self.assertIsInstance(self.tp.sufficiency_rating, str)
-#         self.assertIsInstance(self.tp.ovrl_structure_length, float)
-#         self.assertIsInstance(self.tp.deck_area, int)
-#         self.assertIsInstance(self.tp.deck_width, int)
-#         self.assertEqual(self.tp.feature_intersect, '                         ')
-#         self.assertIsInstance(self.tp.year_built, str)
-#         self.assertIsInstance(self.tp.longitude_begin_nbr, float)
-#         self.assertIsInstance(self.tp.latitude_begin_nbr, float)
-#         self.assertEqual(self.tp.longitude_end_nbr, None)
-#         self.assertEqual(self.tp.latitude_end_nbr, None)
-#         self.assertEqual(self.tp.county_cd_work_location, 'MRW')
-#         self.assertEqual(self.tp.county_nme_work_location, 'MORROW')
-#         self.assertEqual(self.tp.district_work_location, '06')
-#         self.assertEqual(self.tp.pavement_treatment_type, None)
-#         self.assertEqual(self.tp.pavement_treatment_category, None)
-#         self.assertEqual(self.tp.created_user, 'TIMS@P31_AG')
-#         self.assertIsInstance(self.tp.created_date, int)
-#         self.assertEqual(self.tp.last_edited_user, 'TIMS@P31_AG')
-#         self.assertIsInstance(self.tp.last_edited_date, int)
-#
+
+
+class TestProject(unittest.TestCase):
+    def setUp(self):
+        # Creates a 'test project' and makes sure none of the attributes have changed
+        self.tp = Project(pid='96213')
+
+    def tearDown(self):
+        pass
+
+    def test_init(self):
+        # //TODO - make tests less dependent on getting specific values from project points arrays
+        self.assertIsInstance(self.tp.objectid, int)
+        self.assertIsInstance(self.tp.gis_id, int)
+        self.assertEqual(self.tp.pid_nbr, 96213)
+        self.assertEqual(self.tp.district_nbr, 6)
+        self.assertEqual(self.tp.locale_short_nme, 'MRW')
+        self.assertEqual(self.tp.county_nme, 'Morrow')
+        self.assertEqual(self.tp.project_nme, 'MRW SR 314 (8.080) (20.57)')
+        self.assertEqual(self.tp.contract_type, 'Standard Build')
+        self.assertEqual(self.tp.primary_fund_category_txt, 'District Preservation (Pv & Br)')
+        self.assertEqual(self.tp.project_manager_nme, 'HIPP, JEFFREY P')
+        self.assertEqual(self.tp.reservoir_year, None)
+        self.assertEqual(self.tp.tier, None)
+        self.assertEqual(self.tp.odot_letting, 'ODOT Let')
+        self.assertEqual(self.tp.schedule_type_short_nme, 'Standard')
+        self.assertEqual(self.tp.env_project_manager_nme, 'TURNER, AMY S')
+        self.assertEqual(self.tp.area_engineer_nme, 'DENNIS, WADE R')
+        self.assertEqual(self.tp.project_engineer_nme, 'STOVER, DONALD L')
+        self.assertEqual(self.tp.design_agency, 'DISTRICT 6-ENGINEERING')
+        self.assertEqual(self.tp.sponsoring_agency, 'DISTRICT 6-PLANNING')
+        self.assertEqual(self.tp.pdp_short_name, 'Path 2')
+        self.assertEqual(self.tp.primary_work_category, 'Bridge Preservation')
+        self.assertEqual(self.tp.project_status, 'Not Filed')
+        self.assertEqual(self.tp.fiscal_year, '2024')
+        self.assertEqual(self.tp.inhouse_design_full_nme, 'HIPP, JEFFREY P')
+        self.assertEqual(self.tp.est_total_constr_cost, 650000)
+        self.assertEqual(self.tp.state_project_nbr, None)
+        self.assertEqual(self.tp.constr_vendor_nme, None)
+        self.assertEqual(self.tp.stip_flag, 'N')
+        self.assertEqual(self.tp.current_stip_co_amt, None)
+        self.assertEqual(self.tp.project_plans_url, 'http://contracts.dot.state.oh.us/search.jsp?cabinetId=1002&PID_NUM=96213')
+        self.assertEqual(self.tp.project_addenda_url, 'http://contracts.dot.state.oh.us/search.jsp?cabinetId=1000&PID_NUM=96213')
+        self.assertEqual(self.tp.project_proposal_url, 'http://contracts.dot.state.oh.us/search.jsp?cabinetId=1003&PID_NUM=96213')
+        self.assertEqual(self.tp.fmis_proj_desc, None)
+        self.assertEqual(self.tp.award_milestone_dt, 1699228800000)
+        self.assertEqual(self.tp.begin_constr_milestone_dt, 1713139200000)
+        self.assertEqual(self.tp.end_constr_milestone_dt, 1722470400000)
+        self.assertEqual(self.tp.open_traffic_dt, None)
+        self.assertEqual(self.tp.central_office_close_dt, None)
+        self.assertIsInstance(self.tp.source_last_updated, int)
+        self.assertIsInstance(self.tp.cod_last_updated, int)
+        self.assertEqual(self.tp.preserv_funds_ind, 'Y')
+        self.assertEqual(self.tp.major_brg_funds_ind, 'N')
+        self.assertEqual(self.tp.major_new_funds_ind, 'N')
+        self.assertEqual(self.tp.major_rehab_funds_ind, 'N')
+        self.assertEqual(self.tp.mpo_funds_ind, 'N')
+        self.assertEqual(self.tp.safety_funds_ind, 'N')
+        self.assertEqual(self.tp.local_funds_ind, 'N')
+        self.assertEqual(self.tp.other_funds_ind, 'N')
+        self.assertEqual(self.tp.nlf_id, 'SMRWSR00314**C')
+        self.assertIsInstance(self.tp.ctl_begin, float)
+        self.assertEqual(self.tp.ctl_end, None)
+        self.assertEqual(self.tp.gis_feature_type, 'POINT')
+        self.assertEqual(self.tp.route_type, 'SR')
+        self.assertEqual(self.tp.route_id, '00314')
+        self.assertIsInstance(self.tp.structure_file_nbr, str)
+        self.assertIsInstance(self.tp.main_structure_type, str)
+        self.assertIsInstance(self.tp.sufficiency_rating, str)
+        self.assertIsInstance(self.tp.ovrl_structure_length, int)
+        self.assertIsInstance(self.tp.deck_area, int)
+        self.assertIsInstance(self.tp.deck_width, int)
+        self.assertEqual(self.tp.feature_intersect, '')
+        self.assertIsInstance(self.tp.year_built, str)
+        self.assertIsInstance(self.tp.longitude_begin_nbr, float)
+        self.assertIsInstance(self.tp.latitude_begin_nbr, float)
+        self.assertEqual(self.tp.longitude_end_nbr, None)
+        self.assertEqual(self.tp.latitude_end_nbr, None)
+        self.assertEqual(self.tp.county_cd_work_location, 'MRW')
+        self.assertEqual(self.tp.county_nme_work_location, 'MORROW')
+        self.assertEqual(self.tp.district_work_location, '06')
+        self.assertEqual(self.tp.pavement_treatment_type, None)
+        self.assertEqual(self.tp.pavement_treatment_category, None)
+        self.assertEqual(self.tp.created_user, 'TIMS@P31_AG')
+        self.assertIsInstance(self.tp.created_date, int)
+        self.assertEqual(self.tp.last_edited_user, 'TIMS@P31_AG')
+        self.assertIsInstance(self.tp.last_edited_date, int)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `civilpy-0.0.44/tests/test_ohio_dot_snbi_transfer.py` & `civilpy-0.0.45/tests/test_ohio_dot_snbi_transfer.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.44/tests/test_steel.py` & `civilpy-0.0.45/tests/test_steel.py`

 * *Files identical despite different names*

