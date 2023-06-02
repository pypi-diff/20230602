# Comparing `tmp/cuefig-0.0.8.tar.gz` & `tmp/cuefig-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuefig-0.0.8.tar", last modified: Sun Apr 24 09:27:26 2022, max compression
+gzip compressed data, was "cuefig-0.0.9.tar", last modified: Wed May 11 15:18:40 2022, max compression
```

## Comparing `cuefig-0.0.8.tar` & `cuefig-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-04-24 09:27:26.523723 cuefig-0.0.8/
--rw-rw-rw-   0        0        0     1086 2022-03-25 05:00:09.000000 cuefig-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       38 2022-04-24 08:10:45.000000 cuefig-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1676 2022-04-24 09:27:26.522723 cuefig-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      919 2022-04-24 09:26:00.000000 cuefig-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-04-24 09:27:26.515723 cuefig-0.0.8/cuefig/
--rw-rw-rw-   0        0        0      383 2022-04-24 08:32:15.000000 cuefig-0.0.8/cuefig/__init__.py
--rw-rw-rw-   0        0        0      803 2022-04-24 09:05:35.000000 cuefig-0.0.8/cuefig/cli.py
-drwxrwxrwx   0        0        0        0 2022-04-24 09:27:26.520724 cuefig-0.0.8/cuefig/logger/
--rw-rw-rw-   0        0        0     1203 2022-03-25 05:18:10.000000 cuefig-0.0.8/cuefig/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-24 09:27:26.521723 cuefig-0.0.8/cuefig/utils/
--rw-rw-rw-   0        0        0       91 2022-03-25 04:36:36.000000 cuefig-0.0.8/cuefig/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-24 09:27:26.520724 cuefig-0.0.8/cuefig.egg-info/
--rw-rw-rw-   0        0        0     1676 2022-04-24 09:27:26.000000 cuefig-0.0.8/cuefig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2022-04-24 09:27:26.000000 cuefig-0.0.8/cuefig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-24 09:27:26.000000 cuefig-0.0.8/cuefig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2022-04-24 09:27:26.000000 cuefig-0.0.8/cuefig.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2022-04-24 09:27:26.000000 cuefig-0.0.8/cuefig.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-04-24 09:27:26.000000 cuefig-0.0.8/cuefig.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-04-24 09:27:26.521723 cuefig-0.0.8/img/
--rw-rw-rw-   0        0        0    63341 2022-03-25 04:40:00.000000 cuefig-0.0.8/img/img.png
--rw-rw-rw-   0        0        0       42 2022-04-24 09:27:26.523723 cuefig-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2703 2022-04-24 09:27:09.000000 cuefig-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-11 15:18:40.597531 cuefig-0.0.9/
+-rw-rw-rw-   0        0        0     1086 2022-03-25 05:00:09.000000 cuefig-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       74 2022-05-11 15:16:37.000000 cuefig-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1676 2022-05-11 15:18:40.597531 cuefig-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      919 2022-04-24 09:26:00.000000 cuefig-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-05-11 15:18:40.590575 cuefig-0.0.9/cuefig/
+-rw-rw-rw-   0        0        0      383 2022-04-24 08:32:15.000000 cuefig-0.0.9/cuefig/__init__.py
+-rw-rw-rw-   0        0        0      803 2022-04-24 09:05:35.000000 cuefig-0.0.9/cuefig/cli.py
+drwxrwxrwx   0        0        0        0 2022-05-11 15:18:40.595560 cuefig-0.0.9/cuefig/logger/
+-rw-rw-rw-   0        0        0     1203 2022-03-25 05:18:10.000000 cuefig-0.0.9/cuefig/logger/__init__.py
+-rw-rw-rw-   0        0        0     1098 2022-03-24 12:06:52.000000 cuefig-0.0.9/cuefig/logger/logging.yaml
+drwxrwxrwx   0        0        0        0 2022-05-11 15:18:40.596531 cuefig-0.0.9/cuefig/utils/
+-rw-rw-rw-   0        0        0       91 2022-03-25 04:36:36.000000 cuefig-0.0.9/cuefig/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-11 15:18:40.594561 cuefig-0.0.9/cuefig.egg-info/
+-rw-rw-rw-   0        0        0     1676 2022-05-11 15:18:40.000000 cuefig-0.0.9/cuefig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2022-05-11 15:18:40.000000 cuefig-0.0.9/cuefig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-11 15:18:40.000000 cuefig-0.0.9/cuefig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2022-05-11 15:18:40.000000 cuefig-0.0.9/cuefig.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2022-05-11 15:18:40.000000 cuefig-0.0.9/cuefig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2022-05-11 15:18:40.000000 cuefig-0.0.9/cuefig.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-05-11 15:18:40.596531 cuefig-0.0.9/img/
+-rw-rw-rw-   0        0        0    63341 2022-03-25 04:40:00.000000 cuefig-0.0.9/img/img.png
+-rw-rw-rw-   0        0        0       42 2022-05-11 15:18:40.598531 cuefig-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2703 2022-05-11 15:17:48.000000 cuefig-0.0.9/setup.py
```

### Comparing `cuefig-0.0.8/LICENSE` & `cuefig-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cuefig-0.0.8/PKG-INFO` & `cuefig-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuefig
-Version: 0.0.8
+Version: 0.0.9
 Summary: A config framework that you can cue and hint quickly.
 Home-page: https://github.com/FavorMylikes/cuefig
 Author: 麦丽素
 Author-email: l786112323@gmail.com
 License: MIT License
 Description: # How to use
```

### Comparing `cuefig-0.0.8/README.md` & `cuefig-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cuefig-0.0.8/cuefig/cli.py` & `cuefig-0.0.9/cuefig/cli.py`

 * *Files identical despite different names*

### Comparing `cuefig-0.0.8/cuefig/logger/__init__.py` & `cuefig-0.0.9/cuefig/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `cuefig-0.0.8/cuefig.egg-info/PKG-INFO` & `cuefig-0.0.9/cuefig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuefig
-Version: 0.0.8
+Version: 0.0.9
 Summary: A config framework that you can cue and hint quickly.
 Home-page: https://github.com/FavorMylikes/cuefig
 Author: 麦丽素
 Author-email: l786112323@gmail.com
 License: MIT License
 Description: # How to use
```

### Comparing `cuefig-0.0.8/img/img.png` & `cuefig-0.0.9/img/img.png`

 * *Files identical despite different names*

### Comparing `cuefig-0.0.8/setup.py` & `cuefig-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages, Command
 import os
 import re
 import sys
 
 __PATH__ = os.path.abspath(os.path.dirname(__file__))
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 
 def read_readme():
     with open('README.md', mode="r", encoding="utf8") as f:
         return f.read()
```

