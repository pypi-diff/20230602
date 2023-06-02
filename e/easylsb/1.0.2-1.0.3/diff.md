# Comparing `tmp/easylsb-1.0.2.tar.gz` & `tmp/easylsb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\easylsb-1.0.2.tar", last modified: Fri Jun  2 09:35:27 2023, max compression
+gzip compressed data, was "dist\easylsb-1.0.3.tar", last modified: Fri Jun  2 09:44:15 2023, max compression
```

## Comparing `easylsb-1.0.2.tar` & `easylsb-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 09:35:27.000000 easylsb-1.0.2/
--rw-rw-rw-   0        0        0     1156 2023-06-02 09:35:27.000000 easylsb-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2023-06-02 09:35:07.000000 easylsb-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 09:35:27.000000 easylsb-1.0.2/easylsb.egg-info/
--rw-rw-rw-   0        0        0     1156 2023-06-02 09:35:26.000000 easylsb-1.0.2/easylsb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-06-02 09:35:27.000000 easylsb-1.0.2/easylsb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 09:35:26.000000 easylsb-1.0.2/easylsb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-06-02 09:35:26.000000 easylsb-1.0.2/easylsb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-06-02 09:35:26.000000 easylsb-1.0.2/easylsb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-02 09:35:26.000000 easylsb-1.0.2/easylsb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12813 2023-06-02 09:28:46.000000 easylsb-1.0.2/lsb.py
--rw-rw-rw-   0        0        0       42 2023-06-02 09:35:27.000000 easylsb-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-06-02 09:35:19.000000 easylsb-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:44:15.000000 easylsb-1.0.3/
+-rw-rw-rw-   0        0        0     1156 2023-06-02 09:44:15.000000 easylsb-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-06-02 09:35:07.000000 easylsb-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 09:44:15.000000 easylsb-1.0.3/easylsb.egg-info/
+-rw-rw-rw-   0        0        0     1156 2023-06-02 09:44:15.000000 easylsb-1.0.3/easylsb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-06-02 09:44:15.000000 easylsb-1.0.3/easylsb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 09:44:15.000000 easylsb-1.0.3/easylsb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-06-02 09:44:15.000000 easylsb-1.0.3/easylsb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2023-06-02 09:44:15.000000 easylsb-1.0.3/easylsb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-02 09:44:15.000000 easylsb-1.0.3/easylsb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12813 2023-06-02 09:28:46.000000 easylsb-1.0.3/lsb.py
+-rw-rw-rw-   0        0        0       42 2023-06-02 09:44:15.000000 easylsb-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      711 2023-06-02 09:44:06.000000 easylsb-1.0.3/setup.py
```

### Comparing `easylsb-1.0.2/PKG-INFO` & `easylsb-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easylsb
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple Python package for steganography
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
 Code to hide information in the given image:
```

### Comparing `easylsb-1.0.2/README.md` & `easylsb-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `easylsb-1.0.2/easylsb.egg-info/PKG-INFO` & `easylsb-1.0.3/easylsb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easylsb
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple Python package for steganography
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
 Code to hide information in the given image:
```

### Comparing `easylsb-1.0.2/lsb.py` & `easylsb-1.0.3/lsb.py`

 * *Files identical despite different names*

### Comparing `easylsb-1.0.2/setup.py` & `easylsb-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 import sys
 import os
 req=["wave", "des", "numpy"]
-if sys.version_info.major=='3':
+if sys.version_info.major==3:
     req.append('pillow')
 def readme():
     with open('README.md','r') as file:
         return file.read()
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 setup(
     name="easylsb",
-    version="1.0.2",
+    version="1.0.3",
     description="Simple Python package for steganography",
     long_description=readme(),
     long_description_content_type='text/markdown',
     py_modules=["lsb"],
     install_requires=req,
     entry_points={
         "console_scripts": [
```

