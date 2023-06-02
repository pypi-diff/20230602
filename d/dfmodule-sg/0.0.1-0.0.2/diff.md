# Comparing `tmp/dfmodule_sg-0.0.1.tar.gz` & `tmp/dfmodule_sg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfmodule_sg-0.0.1.tar", last modified: Fri Jun  2 05:50:10 2023, max compression
+gzip compressed data, was "dfmodule_sg-0.0.2.tar", last modified: Fri Jun  2 06:22:18 2023, max compression
```

## Comparing `dfmodule_sg-0.0.1.tar` & `dfmodule_sg-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 05:50:10.525856 dfmodule_sg-0.0.1/
--rw-rw-rw-   0        0        0      527 2023-06-02 05:50:10.525856 dfmodule_sg-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 05:50:10.523856 dfmodule_sg-0.0.1/dfmodule_sg.egg-info/
--rw-rw-rw-   0        0        0      527 2023-06-02 05:50:10.000000 dfmodule_sg-0.0.1/dfmodule_sg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-02 05:50:10.000000 dfmodule_sg-0.0.1/dfmodule_sg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 05:50:10.000000 dfmodule_sg-0.0.1/dfmodule_sg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-02 05:50:10.000000 dfmodule_sg-0.0.1/dfmodule_sg.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-02 05:50:10.000000 dfmodule_sg-0.0.1/dfmodule_sg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 05:50:10.000000 dfmodule_sg-0.0.1/dfmodule_sg.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 05:50:10.524855 dfmodule_sg-0.0.1/sample/
--rw-rw-rw-   0        0        0       40 2023-06-02 05:47:26.000000 dfmodule_sg-0.0.1/sample/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-02 05:50:10.525856 dfmodule_sg-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      785 2023-06-02 05:45:41.000000 dfmodule_sg-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 06:22:18.060375 dfmodule_sg-0.0.2/
+-rw-rw-rw-   0        0        0      527 2023-06-02 06:22:18.060375 dfmodule_sg-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 06:22:18.058375 dfmodule_sg-0.0.2/dfmodule_sg.egg-info/
+-rw-rw-rw-   0        0        0      527 2023-06-02 06:22:17.000000 dfmodule_sg-0.0.2/dfmodule_sg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-02 06:22:17.000000 dfmodule_sg-0.0.2/dfmodule_sg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 06:22:17.000000 dfmodule_sg-0.0.2/dfmodule_sg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 05:50:10.000000 dfmodule_sg-0.0.2/dfmodule_sg.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-02 06:22:17.000000 dfmodule_sg-0.0.2/dfmodule_sg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 06:22:17.000000 dfmodule_sg-0.0.2/dfmodule_sg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 06:22:18.059375 dfmodule_sg-0.0.2/sample/
+-rw-rw-rw-   0        0        0       86 2023-06-02 06:14:45.000000 dfmodule_sg-0.0.2/sample/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-02 06:22:18.061375 dfmodule_sg-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-06-02 06:21:48.000000 dfmodule_sg-0.0.2/setup.py
```

### Comparing `dfmodule_sg-0.0.1/PKG-INFO` & `dfmodule_sg-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfmodule_sg
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple dfmodule_sg example package
 Home-page: http://github.com/yourusername/sample_package
 Author: ente
 Author-email: your.email@example.com
 Keywords: dfmodule_sg,dfmodule
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dfmodule_sg-0.0.1/dfmodule_sg.egg-info/PKG-INFO` & `dfmodule_sg-0.0.2/dfmodule_sg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfmodule-sg
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple dfmodule_sg example package
 Home-page: http://github.com/yourusername/sample_package
 Author: ente
 Author-email: your.email@example.com
 Keywords: dfmodule_sg,dfmodule
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dfmodule_sg-0.0.1/setup.py` & `dfmodule_sg-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dfmodule_sg",
-    version="0.0.1",
+    version="0.0.2",
     description="A simple dfmodule_sg example package",
     author="ente",
     author_email="your.email@example.com",
     url="http://github.com/yourusername/sample_package",
     install_requires=['pandas', 'numpy'],
     packages=find_packages(exclude=['tests*']),
     keywords=['dfmodule_sg', 'dfmodule'],
```

