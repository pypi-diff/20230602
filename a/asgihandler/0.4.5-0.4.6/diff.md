# Comparing `tmp/asgihandler-0.4.5.tar.gz` & `tmp/asgihandler-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgihandler-0.4.5.tar", last modified: Sat May 27 01:36:05 2023, max compression
+gzip compressed data, was "asgihandler-0.4.6.tar", last modified: Fri Jun  2 01:47:06 2023, max compression
```

## Comparing `asgihandler-0.4.5.tar` & `asgihandler-0.4.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 01:36:05.470078 asgihandler-0.4.5/
--rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.4.5/LICENSE
--rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3117 2023-05-27 01:36:05.470078 asgihandler-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     2483 2023-05-02 06:18:39.000000 asgihandler-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 01:36:05.451107 asgihandler-0.4.5/asgihandler/
--rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.4.5/asgihandler/__init__.py
--rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.4.5/asgihandler/__version__.py
--rw-rw-rw-   0        0        0     1260 2023-05-27 01:35:04.000000 asgihandler-0.4.5/asgihandler/core.py
--rw-rw-rw-   0        0        0      460 2023-05-26 18:39:50.000000 asgihandler-0.4.5/asgihandler/userCheck.py
-drwxrwxrwx   0        0        0        0 2023-05-27 01:36:05.468077 asgihandler-0.4.5/asgihandler.egg-info/
--rw-rw-rw-   0        0        0     3117 2023-05-27 01:36:05.000000 asgihandler-0.4.5/asgihandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-05-27 01:36:05.000000 asgihandler-0.4.5/asgihandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 01:36:05.000000 asgihandler-0.4.5/asgihandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 01:36:05.000000 asgihandler-0.4.5/asgihandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-27 01:36:05.000000 asgihandler-0.4.5/asgihandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 01:36:05.470078 asgihandler-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0     3878 2023-05-27 01:36:03.000000 asgihandler-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:47:06.276867 asgihandler-0.4.6/
+-rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3117 2023-06-02 01:47:06.276867 asgihandler-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2483 2023-05-02 06:18:39.000000 asgihandler-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 01:47:06.258868 asgihandler-0.4.6/asgihandler/
+-rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.4.6/asgihandler/__init__.py
+-rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.4.6/asgihandler/__version__.py
+-rw-rw-rw-   0        0        0     1260 2023-05-27 01:35:04.000000 asgihandler-0.4.6/asgihandler/core.py
+-rw-rw-rw-   0        0        0      460 2023-06-02 01:45:31.000000 asgihandler-0.4.6/asgihandler/userCheck.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:47:06.275867 asgihandler-0.4.6/asgihandler.egg-info/
+-rw-rw-rw-   0        0        0     3117 2023-06-02 01:47:06.000000 asgihandler-0.4.6/asgihandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-06-02 01:47:06.000000 asgihandler-0.4.6/asgihandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 01:47:06.000000 asgihandler-0.4.6/asgihandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-02 01:47:06.000000 asgihandler-0.4.6/asgihandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-02 01:47:06.000000 asgihandler-0.4.6/asgihandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 01:47:06.276867 asgihandler-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     3878 2023-06-02 01:47:03.000000 asgihandler-0.4.6/setup.py
```

### Comparing `asgihandler-0.4.5/LICENSE` & `asgihandler-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `asgihandler-0.4.5/PKG-INFO` & `asgihandler-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.4.5
+Version: 0.4.6
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `asgihandler-0.4.5/README.md` & `asgihandler-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `asgihandler-0.4.5/asgihandler/core.py` & `asgihandler-0.4.6/asgihandler/core.py`

 * *Files identical despite different names*

### Comparing `asgihandler-0.4.5/asgihandler.egg-info/PKG-INFO` & `asgihandler-0.4.6/asgihandler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.4.5
+Version: 0.4.6
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `asgihandler-0.4.5/setup.py` & `asgihandler-0.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'asgihandler'
 DESCRIPTION = 'ASGIHandler'
 URL = 'https://github.com/GreaterWMS/GreaterWMS'
 EMAIL = 'singosgu@gmail.com'
 AUTHOR = 'Singosgu'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.4.5'
+VERSION = '0.4.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
 ]
 
 # What packages are optional?
```

