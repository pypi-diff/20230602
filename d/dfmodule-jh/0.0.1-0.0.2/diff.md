# Comparing `tmp/dfmodule_jh-0.0.1.tar.gz` & `tmp/dfmodule_jh-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfmodule_jh-0.0.1.tar", last modified: Fri Jun  2 05:50:09 2023, max compression
+gzip compressed data, was "dfmodule_jh-0.0.2.tar", last modified: Fri Jun  2 06:22:26 2023, max compression
```

## Comparing `dfmodule_jh-0.0.1.tar` & `dfmodule_jh-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 05:50:09.868208 dfmodule_jh-0.0.1/
--rw-rw-rw-   0        0        0      538 2023-06-02 05:50:09.868208 dfmodule_jh-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 05:50:09.867221 dfmodule_jh-0.0.1/dfmodule_jh.egg-info/
--rw-rw-rw-   0        0        0      538 2023-06-02 05:50:09.000000 dfmodule_jh-0.0.1/dfmodule_jh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-02 05:50:09.000000 dfmodule_jh-0.0.1/dfmodule_jh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 05:50:09.000000 dfmodule_jh-0.0.1/dfmodule_jh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-02 05:50:09.000000 dfmodule_jh-0.0.1/dfmodule_jh.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-02 05:50:09.000000 dfmodule_jh-0.0.1/dfmodule_jh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 05:50:09.000000 dfmodule_jh-0.0.1/dfmodule_jh.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 05:50:09.867221 dfmodule_jh-0.0.1/sample/
--rw-rw-rw-   0        0        0       51 2023-06-02 05:47:16.000000 dfmodule_jh-0.0.1/sample/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-02 05:50:09.869208 dfmodule_jh-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      796 2023-06-02 05:45:35.000000 dfmodule_jh-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 06:22:26.738747 dfmodule_jh-0.0.2/
+-rw-rw-rw-   0        0        0      538 2023-06-02 06:22:26.738747 dfmodule_jh-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 06:22:26.737747 dfmodule_jh-0.0.2/dfmodule_jh.egg-info/
+-rw-rw-rw-   0        0        0      538 2023-06-02 06:22:26.000000 dfmodule_jh-0.0.2/dfmodule_jh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-02 06:22:26.000000 dfmodule_jh-0.0.2/dfmodule_jh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 06:22:26.000000 dfmodule_jh-0.0.2/dfmodule_jh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 05:50:09.000000 dfmodule_jh-0.0.2/dfmodule_jh.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-02 06:22:26.000000 dfmodule_jh-0.0.2/dfmodule_jh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 06:22:26.000000 dfmodule_jh-0.0.2/dfmodule_jh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 06:22:26.737747 dfmodule_jh-0.0.2/sample/
+-rw-rw-rw-   0        0        0      112 2023-06-02 06:14:26.000000 dfmodule_jh-0.0.2/sample/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-02 06:22:26.739746 dfmodule_jh-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      796 2023-06-02 06:21:58.000000 dfmodule_jh-0.0.2/setup.py
```

### Comparing `dfmodule_jh-0.0.1/PKG-INFO` & `dfmodule_jh-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfmodule_jh
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple dfmodule example package 11111
 Home-page: http://github.com/yourusername/sample_package
 Author: Your Name123
 Author-email: your.email@example.com
 Keywords: dfmodule_jh,dfmodule
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dfmodule_jh-0.0.1/dfmodule_jh.egg-info/PKG-INFO` & `dfmodule_jh-0.0.2/dfmodule_jh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfmodule-jh
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple dfmodule example package 11111
 Home-page: http://github.com/yourusername/sample_package
 Author: Your Name123
 Author-email: your.email@example.com
 Keywords: dfmodule_jh,dfmodule
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dfmodule_jh-0.0.1/setup.py` & `dfmodule_jh-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dfmodule_jh",
-    version="0.0.1",
+    version="0.0.2",
     description="A simple dfmodule example package 11111",
     author="Your Name123",
     author_email="your.email@example.com",
     url="http://github.com/yourusername/sample_package",
     install_requires=['pandas', 'numpy'],
     packages=find_packages(exclude=['tests*']),
     keywords=['dfmodule_jh', 'dfmodule'],
```

