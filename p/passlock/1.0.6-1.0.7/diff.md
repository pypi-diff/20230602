# Comparing `tmp/passlock-1.0.6.tar.gz` & `tmp/passlock-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passlock-1.0.6.tar", last modified: Fri Jun  2 17:07:23 2023, max compression
+gzip compressed data, was "passlock-1.0.7.tar", last modified: Fri Jun  2 17:13:26 2023, max compression
```

## Comparing `passlock-1.0.6.tar` & `passlock-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:07:23.401800 passlock-1.0.6/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     7591 2023-06-02 17:07:23.401800 passlock-1.0.6/PKG-INFO
--rwxrwxr-x   0 praveen   (1000) praveen   (1000)     7277 2023-06-01 15:11:43.000000 passlock-1.0.6/README.md
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:07:23.401800 passlock-1.0.6/passlock/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:51:00.000000 passlock-1.0.6/passlock/__init__.py
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:07:23.401800 passlock-1.0.6/passlock.egg-info/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     7591 2023-06-02 17:07:23.000000 passlock-1.0.6/passlock.egg-info/PKG-INFO
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      233 2023-06-02 17:07:23.000000 passlock-1.0.6/passlock.egg-info/SOURCES.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 17:07:23.000000 passlock-1.0.6/passlock.egg-info/dependency_links.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       53 2023-06-02 17:07:23.000000 passlock-1.0.6/passlock.egg-info/entry_points.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-02 17:07:23.000000 passlock-1.0.6/passlock.egg-info/requires.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        9 2023-06-02 17:07:23.000000 passlock-1.0.6/passlock.egg-info/top_level.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-02 17:07:23.401800 passlock-1.0.6/setup.cfg
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      751 2023-06-02 17:07:15.000000 passlock-1.0.6/setup.py
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:13:26.037962 passlock-1.0.7/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     7591 2023-06-02 17:13:26.037962 passlock-1.0.7/PKG-INFO
+-rwxrwxr-x   0 praveen   (1000) praveen   (1000)     7277 2023-06-01 15:11:43.000000 passlock-1.0.7/README.md
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:13:26.037962 passlock-1.0.7/passlock/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:51:00.000000 passlock-1.0.7/passlock/__init__.py
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:13:26.037962 passlock-1.0.7/passlock.egg-info/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     7591 2023-06-02 17:13:25.000000 passlock-1.0.7/passlock.egg-info/PKG-INFO
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      233 2023-06-02 17:13:25.000000 passlock-1.0.7/passlock.egg-info/SOURCES.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 17:13:25.000000 passlock-1.0.7/passlock.egg-info/dependency_links.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       53 2023-06-02 17:13:25.000000 passlock-1.0.7/passlock.egg-info/entry_points.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-02 17:13:25.000000 passlock-1.0.7/passlock.egg-info/requires.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        9 2023-06-02 17:13:25.000000 passlock-1.0.7/passlock.egg-info/top_level.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-02 17:13:26.037962 passlock-1.0.7/setup.cfg
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      754 2023-06-02 17:13:24.000000 passlock-1.0.7/setup.py
```

### Comparing `passlock-1.0.6/PKG-INFO` & `passlock-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passlock
-Version: 1.0.6
+Version: 1.0.7
 Summary: A simple password manager
 Home-page: https://github.com/Praveenms13/PyMongo-PasswordManager-CommandLineTool
 Author: M S Praveen Kumar
 Author-email: mspraveenkumar77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `passlock-1.0.6/README.md` & `passlock-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `passlock-1.0.6/passlock.egg-info/PKG-INFO` & `passlock-1.0.7/passlock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passlock
-Version: 1.0.6
+Version: 1.0.7
 Summary: A simple password manager
 Home-page: https://github.com/Praveenms13/PyMongo-PasswordManager-CommandLineTool
 Author: M S Praveen Kumar
 Author-email: mspraveenkumar77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `passlock-1.0.6/setup.py` & `passlock-1.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,22 @@
     required = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="passlock",
-    version="1.0.6",
+    version="1.0.7",
     author="M S Praveen Kumar",
     author_email="mspraveenkumar77@gmail.com",
     description="A simple password manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=required,
     url="https://github.com/Praveenms13/PyMongo-PasswordManager-CommandLineTool",
     entry_points={
         'console_scripts': [
-            'passlock=passlock.passlock:main'
+            'passlock = passlock.passlock:main',
         ]
     },
 )
```

