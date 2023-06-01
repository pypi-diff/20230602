# Comparing `tmp/pyotb-2.0.0.dev1.tar.gz` & `tmp/pyotb-2.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyotb-2.0.0.dev1.tar", last modified: Thu Jun  1 19:22:00 2023, max compression
+gzip compressed data, was "pyotb-2.0.0.dev2.tar", last modified: Thu Jun  1 22:03:40 2023, max compression
```

## Comparing `pyotb-2.0.0.dev1.tar` & `pyotb-2.0.0.dev2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:22:00.039908 pyotb-2.0.0.dev1/
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-31 10:05:27.000000 pyotb-2.0.0.dev1/AUTHORS.md
--rw-rw-rw-   0 root         (0) root         (0)    11354 2023-05-24 08:56:49.000000 pyotb-2.0.0.dev1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    16453 2023-06-01 19:22:00.039908 pyotb-2.0.0.dev1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2346 2023-05-31 10:05:27.000000 pyotb-2.0.0.dev1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:22:00.035908 pyotb-2.0.0.dev1/pyotb/
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-06-01 18:37:23.000000 pyotb-2.0.0.dev1/pyotb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5556 2023-06-01 18:37:23.000000 pyotb-2.0.0.dev1/pyotb/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    66822 2023-06-01 18:37:23.000000 pyotb-2.0.0.dev1/pyotb/core.py
--rw-rw-rw-   0 root         (0) root         (0)    22175 2023-06-01 18:37:23.000000 pyotb-2.0.0.dev1/pyotb/functions.py
--rw-rw-rw-   0 root         (0) root         (0)    13150 2023-06-01 18:37:23.000000 pyotb-2.0.0.dev1/pyotb/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:22:00.035908 pyotb-2.0.0.dev1/pyotb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16453 2023-06-01 19:22:00.000000 pyotb-2.0.0.dev1/pyotb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2023-06-01 19:22:00.000000 pyotb-2.0.0.dev1/pyotb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 19:22:00.000000 pyotb-2.0.0.dev1/pyotb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-01 19:22:00.000000 pyotb-2.0.0.dev1/pyotb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-01 19:22:00.000000 pyotb-2.0.0.dev1/pyotb.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1780 2023-06-01 18:37:23.000000 pyotb-2.0.0.dev1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 19:22:00.039908 pyotb-2.0.0.dev1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:22:00.039908 pyotb-2.0.0.dev1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     9942 2023-05-24 08:56:50.000000 pyotb-2.0.0.dev1/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)     1769 2023-05-24 08:56:50.000000 pyotb-2.0.0.dev1/tests/test_numpy.py
--rw-rw-rw-   0 root         (0) root         (0)     3813 2023-05-24 08:56:50.000000 pyotb-2.0.0.dev1/tests/test_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-05-24 08:56:50.000000 pyotb-2.0.0.dev1/tests/tests_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 22:03:40.875204 pyotb-2.0.0.dev2/
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-30 15:37:02.000000 pyotb-2.0.0.dev2/AUTHORS.md
+-rw-rw-rw-   0 root         (0) root         (0)    11354 2023-05-24 08:56:53.000000 pyotb-2.0.0.dev2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    16453 2023-06-01 22:03:40.875204 pyotb-2.0.0.dev2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2346 2023-05-31 07:58:34.000000 pyotb-2.0.0.dev2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 22:03:40.871204 pyotb-2.0.0.dev2/pyotb/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-06-01 21:35:33.000000 pyotb-2.0.0.dev2/pyotb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5556 2023-06-01 18:37:22.000000 pyotb-2.0.0.dev2/pyotb/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    66822 2023-06-01 18:37:22.000000 pyotb-2.0.0.dev2/pyotb/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    22175 2023-06-01 18:37:22.000000 pyotb-2.0.0.dev2/pyotb/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13150 2023-06-01 18:37:22.000000 pyotb-2.0.0.dev2/pyotb/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 22:03:40.875204 pyotb-2.0.0.dev2/pyotb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16453 2023-06-01 22:03:40.000000 pyotb-2.0.0.dev2/pyotb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-01 22:03:40.000000 pyotb-2.0.0.dev2/pyotb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 22:03:40.000000 pyotb-2.0.0.dev2/pyotb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-01 22:03:40.000000 pyotb-2.0.0.dev2/pyotb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-01 22:03:40.000000 pyotb-2.0.0.dev2/pyotb.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2023-06-01 18:37:22.000000 pyotb-2.0.0.dev2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 22:03:40.875204 pyotb-2.0.0.dev2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 22:03:40.875204 pyotb-2.0.0.dev2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     9942 2023-05-31 10:05:29.000000 pyotb-2.0.0.dev2/tests/test_core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1769 2023-05-24 08:56:53.000000 pyotb-2.0.0.dev2/tests/test_numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2023-05-24 08:56:53.000000 pyotb-2.0.0.dev2/tests/test_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-05-24 08:56:53.000000 pyotb-2.0.0.dev2/tests/tests_data.py
```

### Comparing `pyotb-2.0.0.dev1/LICENSE` & `pyotb-2.0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.0.dev1/PKG-INFO` & `pyotb-2.0.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyotb
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: Library to enable easy use of the Orfeo ToolBox (OTB) in Python
 Author: Nicolas Narçon, Vincent Delbar
 Author-email: Rémi Cresson <remi.cresson@inrae.fr>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pyotb-2.0.0.dev1/README.md` & `pyotb-2.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.0.dev1/pyotb/apps.py` & `pyotb-2.0.0.dev2/pyotb/apps.py`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.0.dev1/pyotb/core.py` & `pyotb-2.0.0.dev2/pyotb/core.py`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.0.dev1/pyotb/functions.py` & `pyotb-2.0.0.dev2/pyotb/functions.py`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.0.dev1/pyotb/helpers.py` & `pyotb-2.0.0.dev2/pyotb/helpers.py`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.0.dev1/pyotb.egg-info/PKG-INFO` & `pyotb-2.0.0.dev2/pyotb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyotb
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: Library to enable easy use of the Orfeo ToolBox (OTB) in Python
 Author: Nicolas Narçon, Vincent Delbar
 Author-email: Rémi Cresson <remi.cresson@inrae.fr>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pyotb-2.0.0.dev1/pyproject.toml` & `pyotb-2.0.0.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.0.dev1/tests/test_core.py` & `pyotb-2.0.0.dev2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.0.dev1/tests/test_numpy.py` & `pyotb-2.0.0.dev2/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.0.dev1/tests/test_pipeline.py` & `pyotb-2.0.0.dev2/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.0.dev1/tests/tests_data.py` & `pyotb-2.0.0.dev2/tests/tests_data.py`

 * *Files identical despite different names*

