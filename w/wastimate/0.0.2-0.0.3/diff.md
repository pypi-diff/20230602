# Comparing `tmp/wastimate-0.0.2.tar.gz` & `tmp/wastimate-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wastimate-0.0.2.tar", last modified: Thu Jun  1 18:58:09 2023, max compression
+gzip compressed data, was "wastimate-0.0.3.tar", last modified: Fri Jun  2 20:17:23 2023, max compression
```

## Comparing `wastimate-0.0.2.tar` & `wastimate-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 18:58:09.360717 wastimate-0.0.2/
--rw-rw-rw-   0        0        0      710 2023-06-01 18:58:09.360717 wastimate-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-01 18:58:09.360717 wastimate-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1184 2023-06-01 18:57:29.000000 wastimate-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:58:09.356716 wastimate-0.0.2/wastimate/
--rw-rw-rw-   0        0        0       24 2023-06-01 18:54:29.000000 wastimate-0.0.2/wastimate/__init__.py
--rw-rw-rw-   0        0        0     8730 2023-06-01 18:25:14.000000 wastimate-0.0.2/wastimate/framework.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:58:09.359717 wastimate-0.0.2/wastimate.egg-info/
--rw-rw-rw-   0        0        0      710 2023-06-01 18:58:09.000000 wastimate-0.0.2/wastimate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-06-01 18:58:09.000000 wastimate-0.0.2/wastimate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 18:58:09.000000 wastimate-0.0.2/wastimate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-01 18:58:09.000000 wastimate-0.0.2/wastimate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-01 18:58:09.000000 wastimate-0.0.2/wastimate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 20:17:23.620276 wastimate-0.0.3/
+-rw-rw-rw-   0        0        0      710 2023-06-02 20:17:23.619277 wastimate-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-02 20:17:23.620276 wastimate-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1184 2023-06-02 20:16:52.000000 wastimate-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:17:23.616286 wastimate-0.0.3/wastimate/
+-rw-rw-rw-   0        0        0       24 2023-06-01 18:54:29.000000 wastimate-0.0.3/wastimate/__init__.py
+-rw-rw-rw-   0        0        0    10504 2023-06-02 20:14:44.000000 wastimate-0.0.3/wastimate/framework.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:17:23.619277 wastimate-0.0.3/wastimate.egg-info/
+-rw-rw-rw-   0        0        0      710 2023-06-02 20:17:23.000000 wastimate-0.0.3/wastimate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-06-02 20:17:23.000000 wastimate-0.0.3/wastimate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 20:17:23.000000 wastimate-0.0.3/wastimate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-02 20:17:23.000000 wastimate-0.0.3/wastimate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-02 20:17:23.000000 wastimate-0.0.3/wastimate.egg-info/top_level.txt
```

### Comparing `wastimate-0.0.2/PKG-INFO` & `wastimate-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wastimate
-Version: 0.0.2
+Version: 0.0.3
 Summary: General framework for estimating waste quantities in time.
 Home-page: UNKNOWN
 Author: Hando Tohver
 Author-email: <handotohver@gmail.com>
 License: UNKNOWN
 Description: Package that offers a general framework for estimating radioactive waste quantities in time and enables the modeling of various waste management strategies.
 Keywords: python,radioactive waste,Modeling
```

### Comparing `wastimate-0.0.2/setup.py` & `wastimate-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'General framework for estimating waste quantities in time.'
 LONG_DESCRIPTION = 'Package that offers a general framework for estimating radioactive waste quantities in time and enables the modeling of various waste management strategies.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="wastimate",
```

### Comparing `wastimate-0.0.2/wastimate.egg-info/PKG-INFO` & `wastimate-0.0.3/wastimate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wastimate
-Version: 0.0.2
+Version: 0.0.3
 Summary: General framework for estimating waste quantities in time.
 Home-page: UNKNOWN
 Author: Hando Tohver
 Author-email: <handotohver@gmail.com>
 License: UNKNOWN
 Description: Package that offers a general framework for estimating radioactive waste quantities in time and enables the modeling of various waste management strategies.
 Keywords: python,radioactive waste,Modeling
```

