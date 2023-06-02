# Comparing `tmp/vcclick-1.0.8.tar.gz` & `tmp/vcclick-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vcclick-1.0.8.tar", last modified: Sun Apr 25 15:46:36 2021, max compression
+gzip compressed data, was "dist\vcclick-1.0.9.tar", last modified: Fri Jun  2 07:46:18 2023, max compression
```

## Comparing `vcclick-1.0.8.tar` & `vcclick-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2021-04-25 15:46:36.000000 vcclick-1.0.8/
--rw-rw-rw-   0        0        0      791 2021-04-25 15:46:36.000000 vcclick-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2021-04-25 15:46:36.000000 vcclick-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      990 2021-04-25 15:46:17.000000 vcclick-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-04-25 15:46:36.000000 vcclick-1.0.8/vcclick/
--rw-rw-rw-   0        0        0    14508 2021-04-25 15:46:05.000000 vcclick-1.0.8/vcclick/main.py
--rw-rw-rw-   0        0        0       50 2021-02-19 18:36:26.000000 vcclick-1.0.8/vcclick/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 15:46:36.000000 vcclick-1.0.8/vcclick.egg-info/
--rw-rw-rw-   0        0        0        1 2021-04-25 15:46:36.000000 vcclick-1.0.8/vcclick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      791 2021-04-25 15:46:36.000000 vcclick-1.0.8/vcclick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2021-04-25 15:46:36.000000 vcclick-1.0.8/vcclick.egg-info/requires.txt
--rw-rw-rw-   0        0        0      198 2021-04-25 15:46:36.000000 vcclick-1.0.8/vcclick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2021-04-25 15:46:36.000000 vcclick-1.0.8/vcclick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 07:46:18.000000 vcclick-1.0.9/
+-rw-rw-rw-   0        0        0      782 2023-06-02 07:46:18.000000 vcclick-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-02 07:46:18.000000 vcclick-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      990 2023-06-02 07:45:52.000000 vcclick-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:46:18.000000 vcclick-1.0.9/vcclick/
+-rw-rw-rw-   0        0        0    15370 2023-06-02 07:45:03.000000 vcclick-1.0.9/vcclick/main.py
+-rw-rw-rw-   0        0        0       50 2021-02-19 18:36:26.000000 vcclick-1.0.9/vcclick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:46:18.000000 vcclick-1.0.9/vcclick.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-02 07:46:18.000000 vcclick-1.0.9/vcclick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      782 2023-06-02 07:46:18.000000 vcclick-1.0.9/vcclick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-06-02 07:46:18.000000 vcclick-1.0.9/vcclick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      198 2023-06-02 07:46:18.000000 vcclick-1.0.9/vcclick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 07:46:18.000000 vcclick-1.0.9/vcclick.egg-info/top_level.txt
```

### Comparing `vcclick-1.0.8/PKG-INFO` & `vcclick-1.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: vcclick
-Version: 1.0.8
+Version: 1.0.9
 Summary: vcclick by Viniette & Clarity.
 Home-page: UNKNOWN
 Author: Shoya Yasuda @ Viniette & Clarity, Inc.
 Author-email: selamatpagi1124@gmail.com
 License: Required: Copyright notice in any social outputs.     Permitted: Private Use, Commercial Use.     Forbidden: Sublicense, Modifications, Distribution, Patent Grant, Use Trademark, Hold Liable.
-Description: Private Use, Commercial Use are permitted.     Dont forget Copyright notice (e.g. https://vigne-cla.com/vcopt-tutorial/) in any social outputs. Thank you.     Required: Copyright notice in any social outputs.     Permitted: Private Use, Commercial Use.     Forbidden: Sublicense, Modifications, Distribution, Patent Grant, Use Trademark, Hold Liable.
 Platform: UNKNOWN
+
+Private Use, Commercial Use are permitted.     Dont forget Copyright notice (e.g. https://vigne-cla.com/vcopt-tutorial/) in any social outputs. Thank you.     Required: Copyright notice in any social outputs.     Permitted: Private Use, Commercial Use.     Forbidden: Sublicense, Modifications, Distribution, Patent Grant, Use Trademark, Hold Liable.
+
```

### Comparing `vcclick-1.0.8/setup.py` & `vcclick-1.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
  
 
 setup(
     name='vcclick',
-    version='1.0.8',
+    version='1.0.9',
     description='vcclick by Viniette & Clarity.',
     long_description='Private Use, Commercial Use are permitted. \
     Dont forget Copyright notice (e.g. https://vigne-cla.com/vcopt-tutorial/) in any social outputs. Thank you. \
     Required: Copyright notice in any social outputs. \
     Permitted: Private Use, Commercial Use. \
     Forbidden: Sublicense, Modifications, Distribution, Patent Grant, Use Trademark, Hold Liable.',
     author='Shoya Yasuda @ Viniette & Clarity, Inc.',
```

### Comparing `vcclick-1.0.8/vcclick.egg-info/PKG-INFO` & `vcclick-1.0.9/vcclick.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: vcclick
-Version: 1.0.8
+Version: 1.0.9
 Summary: vcclick by Viniette & Clarity.
 Home-page: UNKNOWN
 Author: Shoya Yasuda @ Viniette & Clarity, Inc.
 Author-email: selamatpagi1124@gmail.com
 License: Required: Copyright notice in any social outputs.     Permitted: Private Use, Commercial Use.     Forbidden: Sublicense, Modifications, Distribution, Patent Grant, Use Trademark, Hold Liable.
-Description: Private Use, Commercial Use are permitted.     Dont forget Copyright notice (e.g. https://vigne-cla.com/vcopt-tutorial/) in any social outputs. Thank you.     Required: Copyright notice in any social outputs.     Permitted: Private Use, Commercial Use.     Forbidden: Sublicense, Modifications, Distribution, Patent Grant, Use Trademark, Hold Liable.
 Platform: UNKNOWN
+
+Private Use, Commercial Use are permitted.     Dont forget Copyright notice (e.g. https://vigne-cla.com/vcopt-tutorial/) in any social outputs. Thank you.     Required: Copyright notice in any social outputs.     Permitted: Private Use, Commercial Use.     Forbidden: Sublicense, Modifications, Distribution, Patent Grant, Use Trademark, Hold Liable.
+
```

