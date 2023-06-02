# Comparing `tmp/mongopasswordmanager-1.0.1.tar.gz` & `tmp/mongopasswordmanager-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongopasswordmanager-1.0.1.tar", last modified: Fri Jun  2 16:00:27 2023, max compression
+gzip compressed data, was "mongopasswordmanager-1.0.2.tar", last modified: Fri Jun  2 16:07:44 2023, max compression
```

## Comparing `mongopasswordmanager-1.0.1.tar` & `mongopasswordmanager-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:00:27.234400 mongopasswordmanager-1.0.1/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      230 2023-06-02 16:00:27.234400 mongopasswordmanager-1.0.1/PKG-INFO
--rwxrwxr-x   0 praveen   (1000) praveen   (1000)     7277 2023-06-01 15:11:43.000000 mongopasswordmanager-1.0.1/README.md
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:00:27.234400 mongopasswordmanager-1.0.1/mongopasswordmanager.egg-info/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      230 2023-06-02 16:00:27.000000 mongopasswordmanager-1.0.1/mongopasswordmanager.egg-info/PKG-INFO
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      237 2023-06-02 16:00:27.000000 mongopasswordmanager-1.0.1/mongopasswordmanager.egg-info/SOURCES.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 16:00:27.000000 mongopasswordmanager-1.0.1/mongopasswordmanager.egg-info/dependency_links.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       46 2023-06-02 16:00:27.000000 mongopasswordmanager-1.0.1/mongopasswordmanager.egg-info/requires.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 16:00:27.000000 mongopasswordmanager-1.0.1/mongopasswordmanager.egg-info/top_level.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-02 16:00:27.234400 mongopasswordmanager-1.0.1/setup.cfg
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      533 2023-06-02 16:00:20.000000 mongopasswordmanager-1.0.1/setup.py
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:07:44.532462 mongopasswordmanager-1.0.2/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     7603 2023-06-02 16:07:44.532462 mongopasswordmanager-1.0.2/PKG-INFO
+-rwxrwxr-x   0 praveen   (1000) praveen   (1000)     7277 2023-06-01 15:11:43.000000 mongopasswordmanager-1.0.2/README.md
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:07:44.532462 mongopasswordmanager-1.0.2/mongopasswordmanager.egg-info/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     7603 2023-06-02 16:07:44.000000 mongopasswordmanager-1.0.2/mongopasswordmanager.egg-info/PKG-INFO
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      284 2023-06-02 16:07:44.000000 mongopasswordmanager-1.0.2/mongopasswordmanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 16:07:44.000000 mongopasswordmanager-1.0.2/mongopasswordmanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       59 2023-06-02 16:07:44.000000 mongopasswordmanager-1.0.2/mongopasswordmanager.egg-info/entry_points.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       46 2023-06-02 16:07:44.000000 mongopasswordmanager-1.0.2/mongopasswordmanager.egg-info/requires.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       12 2023-06-02 16:07:44.000000 mongopasswordmanager-1.0.2/mongopasswordmanager.egg-info/top_level.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-02 16:07:44.532462 mongopasswordmanager-1.0.2/setup.cfg
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      770 2023-06-02 16:07:42.000000 mongopasswordmanager-1.0.2/setup.py
```

### Comparing `mongopasswordmanager-1.0.1/README.md` & `mongopasswordmanager-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mongopasswordmanager-1.0.1/setup.py` & `mongopasswordmanager-1.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from setuptools import setup, find_packages
 
 # Read the requirements from requirements.sh
 with open("requirements.sh") as f:
-    requirements = f.read().splitlines()
+    required = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mongopasswordmanager",
-    version="1.0.1",
+    version="1.0.2",
     author="M S Praveen Kumar",
     author_email="mspraveenkumar77@gmail.com",
     description="A simple password manager",
-    packages=find_packages(),
-    install_requires=requirements,  # Use the requirements from requirements.sh
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    install_requires=required,
+    url="https://github.com/Praveenms13/PyMongo-PasswordManager-CommandLineTool",
+    packages=["passmanager"],
+    entry_points={
+        'console_scripts': [
+            'passmanager = passmanager.pass:__main__'
+        ]
+    }
 )
```

