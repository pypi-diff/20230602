# Comparing `tmp/brunospackage-0.0.7.tar.gz` & `tmp/brunospackage-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brunospackage-0.0.7.tar", last modified: Fri Jun  2 05:10:29 2023, max compression
+gzip compressed data, was "brunospackage-0.0.8.tar", last modified: Fri Jun  2 08:19:43 2023, max compression
```

## Comparing `brunospackage-0.0.7.tar` & `brunospackage-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 05:10:29.575219 brunospackage-0.0.7/
--rw-r--r--   0 bdtacchi   (501) staff       (20)      540 2023-06-02 05:10:29.575096 brunospackage-0.0.7/PKG-INFO
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 05:10:29.574167 brunospackage-0.0.7/brunospackage/
--rw-r--r--   0 bdtacchi   (501) staff       (20)       52 2023-06-02 04:36:45.000000 brunospackage-0.0.7/brunospackage/__init__.py
--rw-r--r--   0 bdtacchi   (501) staff       (20)     4685 2023-06-02 05:10:07.000000 brunospackage-0.0.7/brunospackage/functions.py
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 05:10:29.574895 brunospackage-0.0.7/brunospackage.egg-info/
--rw-r--r--   0 bdtacchi   (501) staff       (20)      540 2023-06-02 05:10:29.000000 brunospackage-0.0.7/brunospackage.egg-info/PKG-INFO
--rw-r--r--   0 bdtacchi   (501) staff       (20)      245 2023-06-02 05:10:29.000000 brunospackage-0.0.7/brunospackage.egg-info/SOURCES.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)        1 2023-06-02 05:10:29.000000 brunospackage-0.0.7/brunospackage.egg-info/dependency_links.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       18 2023-06-02 05:10:29.000000 brunospackage-0.0.7/brunospackage.egg-info/requires.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       14 2023-06-02 05:10:29.000000 brunospackage-0.0.7/brunospackage.egg-info/top_level.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       38 2023-06-02 05:10:29.575271 brunospackage-0.0.7/setup.cfg
--rw-r--r--   0 bdtacchi   (501) staff       (20)     1630 2023-06-02 05:10:18.000000 brunospackage-0.0.7/setup.py
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 08:19:43.443461 brunospackage-0.0.8/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      540 2023-06-02 08:19:43.443338 brunospackage-0.0.8/PKG-INFO
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 08:19:43.442274 brunospackage-0.0.8/brunospackage/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       52 2023-06-02 04:36:45.000000 brunospackage-0.0.8/brunospackage/__init__.py
+-rw-r--r--   0 bdtacchi   (501) staff       (20)    16297 2023-06-02 08:18:13.000000 brunospackage-0.0.8/brunospackage/functions.py
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 08:19:43.443144 brunospackage-0.0.8/brunospackage.egg-info/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      540 2023-06-02 08:19:43.000000 brunospackage-0.0.8/brunospackage.egg-info/PKG-INFO
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      245 2023-06-02 08:19:43.000000 brunospackage-0.0.8/brunospackage.egg-info/SOURCES.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)        1 2023-06-02 08:19:43.000000 brunospackage-0.0.8/brunospackage.egg-info/dependency_links.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       18 2023-06-02 08:19:43.000000 brunospackage-0.0.8/brunospackage.egg-info/requires.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       14 2023-06-02 08:19:43.000000 brunospackage-0.0.8/brunospackage.egg-info/top_level.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       38 2023-06-02 08:19:43.443511 brunospackage-0.0.8/setup.cfg
+-rw-r--r--   0 bdtacchi   (501) staff       (20)     1630 2023-06-02 08:19:34.000000 brunospackage-0.0.8/setup.py
```

### Comparing `brunospackage-0.0.7/PKG-INFO` & `brunospackage-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brunospackage
-Version: 0.0.7
+Version: 0.0.8
 Summary: Helper functions that I use often
 Author: Bruno Tacchi
 Author-email: bruno_tacchi@hotmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `brunospackage-0.0.7/brunospackage.egg-info/PKG-INFO` & `brunospackage-0.0.8/brunospackage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brunospackage
-Version: 0.0.7
+Version: 0.0.8
 Summary: Helper functions that I use often
 Author: Bruno Tacchi
 Author-email: bruno_tacchi@hotmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `brunospackage-0.0.7/setup.py` & `brunospackage-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7' 
+VERSION = '0.0.8' 
 DESCRIPTION = 'Helper functions that I use often'
 LONG_DESCRIPTION = '''A package that allows me to import functions that I use often.'''
 # DataFramePlotter - given a dataframe with multiple variables, plots each variable against time in a tkinter window. Requires pandas, matplotlib, tkinter, and re. The usage is: 
 #     import brunospackage as bp
 #     plotter = bp.DataFramePlotter(df, nameOfTimeColumn, unit_format)
 #     plotter.run()'''
```

