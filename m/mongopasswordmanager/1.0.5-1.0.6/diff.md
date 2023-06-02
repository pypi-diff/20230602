# Comparing `tmp/mongopasswordmanager-1.0.5.tar.gz` & `tmp/mongopasswordmanager-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongopasswordmanager-1.0.5.tar", last modified: Fri Jun  2 16:21:15 2023, max compression
+gzip compressed data, was "mongopasswordmanager-1.0.6.tar", last modified: Fri Jun  2 16:22:28 2023, max compression
```

## Comparing `mongopasswordmanager-1.0.5.tar` & `mongopasswordmanager-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:21:15.237801 mongopasswordmanager-1.0.5/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     7603 2023-06-02 16:21:15.237801 mongopasswordmanager-1.0.5/PKG-INFO
--rwxrwxr-x   0 praveen   (1000) praveen   (1000)     7277 2023-06-01 15:11:43.000000 mongopasswordmanager-1.0.5/README.md
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:21:15.237801 mongopasswordmanager-1.0.5/mongopasswordmanager.egg-info/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     7603 2023-06-02 16:21:15.000000 mongopasswordmanager-1.0.5/mongopasswordmanager.egg-info/PKG-INFO
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      284 2023-06-02 16:21:15.000000 mongopasswordmanager-1.0.5/mongopasswordmanager.egg-info/SOURCES.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 16:21:15.000000 mongopasswordmanager-1.0.5/mongopasswordmanager.egg-info/dependency_links.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       55 2023-06-02 16:21:15.000000 mongopasswordmanager-1.0.5/mongopasswordmanager.egg-info/entry_points.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-02 16:21:15.000000 mongopasswordmanager-1.0.5/mongopasswordmanager.egg-info/requires.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       12 2023-06-02 16:21:15.000000 mongopasswordmanager-1.0.5/mongopasswordmanager.egg-info/top_level.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-02 16:21:15.237801 mongopasswordmanager-1.0.5/setup.cfg
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      746 2023-06-02 16:21:11.000000 mongopasswordmanager-1.0.5/setup.py
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:22:28.090512 mongopasswordmanager-1.0.6/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     7603 2023-06-02 16:22:28.090512 mongopasswordmanager-1.0.6/PKG-INFO
+-rwxrwxr-x   0 praveen   (1000) praveen   (1000)     7277 2023-06-01 15:11:43.000000 mongopasswordmanager-1.0.6/README.md
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:22:28.090512 mongopasswordmanager-1.0.6/mongopasswordmanager.egg-info/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     7603 2023-06-02 16:22:28.000000 mongopasswordmanager-1.0.6/mongopasswordmanager.egg-info/PKG-INFO
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      304 2023-06-02 16:22:28.000000 mongopasswordmanager-1.0.6/mongopasswordmanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 16:22:28.000000 mongopasswordmanager-1.0.6/mongopasswordmanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       55 2023-06-02 16:22:28.000000 mongopasswordmanager-1.0.6/mongopasswordmanager.egg-info/entry_points.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-02 16:22:28.000000 mongopasswordmanager-1.0.6/mongopasswordmanager.egg-info/requires.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       12 2023-06-02 16:22:28.000000 mongopasswordmanager-1.0.6/mongopasswordmanager.egg-info/top_level.txt
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:22:28.090512 mongopasswordmanager-1.0.6/passmanager/
+-rwxrwxr-x   0 praveen   (1000) praveen   (1000)    25550 2023-06-02 15:35:43.000000 mongopasswordmanager-1.0.6/passmanager/pass.py
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-02 16:22:28.090512 mongopasswordmanager-1.0.6/setup.cfg
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      746 2023-06-02 16:22:26.000000 mongopasswordmanager-1.0.6/setup.py
```

### Comparing `mongopasswordmanager-1.0.5/PKG-INFO` & `mongopasswordmanager-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongopasswordmanager
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple password manager
 Home-page: https://github.com/Praveenms13/PyMongo-PasswordManager-CommandLineTool
 Author: M S Praveen Kumar
 Author-email: mspraveenkumar77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mongopasswordmanager-1.0.5/README.md` & `mongopasswordmanager-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mongopasswordmanager-1.0.5/mongopasswordmanager.egg-info/PKG-INFO` & `mongopasswordmanager-1.0.6/mongopasswordmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongopasswordmanager
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple password manager
 Home-page: https://github.com/Praveenms13/PyMongo-PasswordManager-CommandLineTool
 Author: M S Praveen Kumar
 Author-email: mspraveenkumar77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mongopasswordmanager-1.0.5/setup.py` & `mongopasswordmanager-1.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     required = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mongopasswordmanager",
-    version="1.0.5",
+    version="1.0.6",
     author="M S Praveen Kumar",
     author_email="mspraveenkumar77@gmail.com",
     description="A simple password manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=required,
     url="https://github.com/Praveenms13/PyMongo-PasswordManager-CommandLineTool",
```

