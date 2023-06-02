# Comparing `tmp/brunospackage-0.0.2.tar.gz` & `tmp/brunospackage-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brunospackage-0.0.2.tar", last modified: Fri Jun  2 04:24:47 2023, max compression
+gzip compressed data, was "brunospackage-0.0.3.tar", last modified: Fri Jun  2 04:33:21 2023, max compression
```

## Comparing `brunospackage-0.0.2.tar` & `brunospackage-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:24:47.568368 brunospackage-0.0.2/
--rw-r--r--   0 bdtacchi   (501) staff       (20)      526 2023-06-02 04:24:47.568244 brunospackage-0.0.2/PKG-INFO
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:24:47.567038 brunospackage-0.0.2/brunospackage/
--rw-r--r--   0 bdtacchi   (501) staff       (20)       38 2023-06-02 04:15:24.000000 brunospackage-0.0.2/brunospackage/__init__.py
--rw-r--r--   0 bdtacchi   (501) staff       (20)     2023 2023-06-02 03:54:10.000000 brunospackage-0.0.2/brunospackage/functions.py
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:24:47.568032 brunospackage-0.0.2/brunospackage.egg-info/
--rw-r--r--   0 bdtacchi   (501) staff       (20)      526 2023-06-02 04:24:47.000000 brunospackage-0.0.2/brunospackage.egg-info/PKG-INFO
--rw-r--r--   0 bdtacchi   (501) staff       (20)      245 2023-06-02 04:24:47.000000 brunospackage-0.0.2/brunospackage.egg-info/SOURCES.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)        1 2023-06-02 04:24:47.000000 brunospackage-0.0.2/brunospackage.egg-info/dependency_links.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       21 2023-06-02 04:24:47.000000 brunospackage-0.0.2/brunospackage.egg-info/requires.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       14 2023-06-02 04:24:47.000000 brunospackage-0.0.2/brunospackage.egg-info/top_level.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       38 2023-06-02 04:24:47.568418 brunospackage-0.0.2/setup.cfg
--rw-r--r--   0 bdtacchi   (501) staff       (20)     1312 2023-06-02 04:24:43.000000 brunospackage-0.0.2/setup.py
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:33:21.534015 brunospackage-0.0.3/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      526 2023-06-02 04:33:21.533884 brunospackage-0.0.3/PKG-INFO
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:33:21.532557 brunospackage-0.0.3/brunospackage/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       38 2023-06-02 04:15:24.000000 brunospackage-0.0.3/brunospackage/__init__.py
+-rw-r--r--   0 bdtacchi   (501) staff       (20)     2023 2023-06-02 03:54:10.000000 brunospackage-0.0.3/brunospackage/functions.py
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:33:21.533625 brunospackage-0.0.3/brunospackage.egg-info/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      526 2023-06-02 04:33:21.000000 brunospackage-0.0.3/brunospackage.egg-info/PKG-INFO
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      245 2023-06-02 04:33:21.000000 brunospackage-0.0.3/brunospackage.egg-info/SOURCES.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)        1 2023-06-02 04:33:21.000000 brunospackage-0.0.3/brunospackage.egg-info/dependency_links.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       18 2023-06-02 04:33:21.000000 brunospackage-0.0.3/brunospackage.egg-info/requires.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       14 2023-06-02 04:33:21.000000 brunospackage-0.0.3/brunospackage.egg-info/top_level.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       38 2023-06-02 04:33:21.534076 brunospackage-0.0.3/setup.cfg
+-rw-r--r--   0 bdtacchi   (501) staff       (20)     1306 2023-06-02 04:33:15.000000 brunospackage-0.0.3/setup.py
```

### Comparing `brunospackage-0.0.2/PKG-INFO` & `brunospackage-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brunospackage
-Version: 0.0.2
+Version: 0.0.3
 Summary: My first Python package
 Author: Bruno Tacchi
 Author-email: bruno_tacchi@hotmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `brunospackage-0.0.2/brunospackage/functions.py` & `brunospackage-0.0.3/brunospackage/functions.py`

 * *Files identical despite different names*

### Comparing `brunospackage-0.0.2/brunospackage.egg-info/PKG-INFO` & `brunospackage-0.0.3/brunospackage.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brunospackage
-Version: 0.0.2
+Version: 0.0.3
 Summary: My first Python package
 Author: Bruno Tacchi
 Author-email: bruno_tacchi@hotmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `brunospackage-0.0.2/setup.py` & `brunospackage-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="brunospackage", 
         version=VERSION,
         author="Bruno Tacchi",
         author_email="bruno_tacchi@hotmail.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['matplotlib', 'pandas', 're'], # add any additional packages that 
+        install_requires=['matplotlib', 'pandas'], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         # import pandas as pd
         # import matplotlib.pyplot as plt
         # from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
         # from matplotlib.figure import Figure
         # import tkinter as tk
         # import re
```

