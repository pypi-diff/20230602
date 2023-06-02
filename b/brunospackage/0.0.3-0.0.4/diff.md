# Comparing `tmp/brunospackage-0.0.3.tar.gz` & `tmp/brunospackage-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brunospackage-0.0.3.tar", last modified: Fri Jun  2 04:33:21 2023, max compression
+gzip compressed data, was "brunospackage-0.0.4.tar", last modified: Fri Jun  2 04:36:54 2023, max compression
```

## Comparing `brunospackage-0.0.3.tar` & `brunospackage-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:33:21.534015 brunospackage-0.0.3/
--rw-r--r--   0 bdtacchi   (501) staff       (20)      526 2023-06-02 04:33:21.533884 brunospackage-0.0.3/PKG-INFO
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:33:21.532557 brunospackage-0.0.3/brunospackage/
--rw-r--r--   0 bdtacchi   (501) staff       (20)       38 2023-06-02 04:15:24.000000 brunospackage-0.0.3/brunospackage/__init__.py
--rw-r--r--   0 bdtacchi   (501) staff       (20)     2023 2023-06-02 03:54:10.000000 brunospackage-0.0.3/brunospackage/functions.py
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:33:21.533625 brunospackage-0.0.3/brunospackage.egg-info/
--rw-r--r--   0 bdtacchi   (501) staff       (20)      526 2023-06-02 04:33:21.000000 brunospackage-0.0.3/brunospackage.egg-info/PKG-INFO
--rw-r--r--   0 bdtacchi   (501) staff       (20)      245 2023-06-02 04:33:21.000000 brunospackage-0.0.3/brunospackage.egg-info/SOURCES.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)        1 2023-06-02 04:33:21.000000 brunospackage-0.0.3/brunospackage.egg-info/dependency_links.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       18 2023-06-02 04:33:21.000000 brunospackage-0.0.3/brunospackage.egg-info/requires.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       14 2023-06-02 04:33:21.000000 brunospackage-0.0.3/brunospackage.egg-info/top_level.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       38 2023-06-02 04:33:21.534076 brunospackage-0.0.3/setup.cfg
--rw-r--r--   0 bdtacchi   (501) staff       (20)     1306 2023-06-02 04:33:15.000000 brunospackage-0.0.3/setup.py
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:36:54.462170 brunospackage-0.0.4/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      526 2023-06-02 04:36:54.462040 brunospackage-0.0.4/PKG-INFO
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:36:54.460856 brunospackage-0.0.4/brunospackage/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       52 2023-06-02 04:36:45.000000 brunospackage-0.0.4/brunospackage/__init__.py
+-rw-r--r--   0 bdtacchi   (501) staff       (20)     2023 2023-06-02 03:54:10.000000 brunospackage-0.0.4/brunospackage/functions.py
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:36:54.461841 brunospackage-0.0.4/brunospackage.egg-info/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      526 2023-06-02 04:36:54.000000 brunospackage-0.0.4/brunospackage.egg-info/PKG-INFO
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      245 2023-06-02 04:36:54.000000 brunospackage-0.0.4/brunospackage.egg-info/SOURCES.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)        1 2023-06-02 04:36:54.000000 brunospackage-0.0.4/brunospackage.egg-info/dependency_links.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       18 2023-06-02 04:36:54.000000 brunospackage-0.0.4/brunospackage.egg-info/requires.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       14 2023-06-02 04:36:54.000000 brunospackage-0.0.4/brunospackage.egg-info/top_level.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       38 2023-06-02 04:36:54.462221 brunospackage-0.0.4/setup.cfg
+-rw-r--r--   0 bdtacchi   (501) staff       (20)     1306 2023-06-02 04:36:50.000000 brunospackage-0.0.4/setup.py
```

### Comparing `brunospackage-0.0.3/PKG-INFO` & `brunospackage-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brunospackage
-Version: 0.0.3
+Version: 0.0.4
 Summary: My first Python package
 Author: Bruno Tacchi
 Author-email: bruno_tacchi@hotmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `brunospackage-0.0.3/brunospackage/functions.py` & `brunospackage-0.0.4/brunospackage/functions.py`

 * *Files identical despite different names*

### Comparing `brunospackage-0.0.3/brunospackage.egg-info/PKG-INFO` & `brunospackage-0.0.4/brunospackage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brunospackage
-Version: 0.0.3
+Version: 0.0.4
 Summary: My first Python package
 Author: Bruno Tacchi
 Author-email: bruno_tacchi@hotmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `brunospackage-0.0.3/setup.py` & `brunospackage-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="brunospackage",
```

