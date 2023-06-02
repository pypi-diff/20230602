# Comparing `tmp/mongopasswordmanager-1.0.3.tar.gz` & `tmp/mongopasswordmanager-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongopasswordmanager-1.0.3.tar", last modified: Fri Jun  2 16:11:55 2023, max compression
+gzip compressed data, was "mongopasswordmanager-1.0.4.tar", last modified: Fri Jun  2 16:17:06 2023, max compression
```

## Comparing `mongopasswordmanager-1.0.3.tar` & `mongopasswordmanager-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:11:55.901377 mongopasswordmanager-1.0.3/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     7603 2023-06-02 16:11:55.901377 mongopasswordmanager-1.0.3/PKG-INFO
--rwxrwxr-x   0 praveen   (1000) praveen   (1000)     7277 2023-06-01 15:11:43.000000 mongopasswordmanager-1.0.3/README.md
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:11:55.901377 mongopasswordmanager-1.0.3/mongopasswordmanager.egg-info/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     7603 2023-06-02 16:11:55.000000 mongopasswordmanager-1.0.3/mongopasswordmanager.egg-info/PKG-INFO
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      284 2023-06-02 16:11:55.000000 mongopasswordmanager-1.0.3/mongopasswordmanager.egg-info/SOURCES.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 16:11:55.000000 mongopasswordmanager-1.0.3/mongopasswordmanager.egg-info/dependency_links.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       59 2023-06-02 16:11:55.000000 mongopasswordmanager-1.0.3/mongopasswordmanager.egg-info/entry_points.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-02 16:11:55.000000 mongopasswordmanager-1.0.3/mongopasswordmanager.egg-info/requires.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       12 2023-06-02 16:11:55.000000 mongopasswordmanager-1.0.3/mongopasswordmanager.egg-info/top_level.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-02 16:11:55.901377 mongopasswordmanager-1.0.3/setup.cfg
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      770 2023-06-02 16:11:54.000000 mongopasswordmanager-1.0.3/setup.py
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:17:06.515559 mongopasswordmanager-1.0.4/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     7603 2023-06-02 16:17:06.515559 mongopasswordmanager-1.0.4/PKG-INFO
+-rwxrwxr-x   0 praveen   (1000) praveen   (1000)     7277 2023-06-01 15:11:43.000000 mongopasswordmanager-1.0.4/README.md
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:17:06.515559 mongopasswordmanager-1.0.4/mongopasswordmanager.egg-info/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     7603 2023-06-02 16:17:06.000000 mongopasswordmanager-1.0.4/mongopasswordmanager.egg-info/PKG-INFO
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      284 2023-06-02 16:17:06.000000 mongopasswordmanager-1.0.4/mongopasswordmanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 16:17:06.000000 mongopasswordmanager-1.0.4/mongopasswordmanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       55 2023-06-02 16:17:06.000000 mongopasswordmanager-1.0.4/mongopasswordmanager.egg-info/entry_points.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-02 16:17:06.000000 mongopasswordmanager-1.0.4/mongopasswordmanager.egg-info/requires.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       12 2023-06-02 16:17:06.000000 mongopasswordmanager-1.0.4/mongopasswordmanager.egg-info/top_level.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-02 16:17:06.515559 mongopasswordmanager-1.0.4/setup.cfg
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      766 2023-06-02 16:17:02.000000 mongopasswordmanager-1.0.4/setup.py
```

### Comparing `mongopasswordmanager-1.0.3/PKG-INFO` & `mongopasswordmanager-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongopasswordmanager
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple password manager
 Home-page: https://github.com/Praveenms13/PyMongo-PasswordManager-CommandLineTool
 Author: M S Praveen Kumar
 Author-email: mspraveenkumar77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mongopasswordmanager-1.0.3/README.md` & `mongopasswordmanager-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mongopasswordmanager-1.0.3/mongopasswordmanager.egg-info/PKG-INFO` & `mongopasswordmanager-1.0.4/mongopasswordmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongopasswordmanager
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple password manager
 Home-page: https://github.com/Praveenms13/PyMongo-PasswordManager-CommandLineTool
 Author: M S Praveen Kumar
 Author-email: mspraveenkumar77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mongopasswordmanager-1.0.3/setup.py` & `mongopasswordmanager-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,22 @@
     required = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mongopasswordmanager",
-    version="1.0.3",
+    version="1.0.4",
     author="M S Praveen Kumar",
     author_email="mspraveenkumar77@gmail.com",
     description="A simple password manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=required,
     url="https://github.com/Praveenms13/PyMongo-PasswordManager-CommandLineTool",
     packages=["passmanager"],
     entry_points={
         'console_scripts': [
-            'passmanager = passmanager.pass:__main__'
+            'passmanager = passmanager.pass:main'
         ]
     }
 )
```

