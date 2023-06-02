# Comparing `tmp/passlock-1.0.8.tar.gz` & `tmp/passlock-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passlock-1.0.8.tar", last modified: Fri Jun  2 17:26:53 2023, max compression
+gzip compressed data, was "passlock-1.0.9.tar", last modified: Fri Jun  2 17:31:53 2023, max compression
```

## Comparing `passlock-1.0.8.tar` & `passlock-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:26:53.659196 passlock-1.0.8/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     6083 2023-06-02 17:26:53.659196 passlock-1.0.8/PKG-INFO
--rwxrwxr-x   0 praveen   (1000) praveen   (1000)     5769 2023-06-02 17:26:36.000000 passlock-1.0.8/README.md
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:26:53.659196 passlock-1.0.8/passlock/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:51:00.000000 passlock-1.0.8/passlock/__init__.py
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:26:53.659196 passlock-1.0.8/passlock.egg-info/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     6083 2023-06-02 17:26:53.000000 passlock-1.0.8/passlock.egg-info/PKG-INFO
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      233 2023-06-02 17:26:53.000000 passlock-1.0.8/passlock.egg-info/SOURCES.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 17:26:53.000000 passlock-1.0.8/passlock.egg-info/dependency_links.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       53 2023-06-02 17:26:53.000000 passlock-1.0.8/passlock.egg-info/entry_points.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-02 17:26:53.000000 passlock-1.0.8/passlock.egg-info/requires.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        9 2023-06-02 17:26:53.000000 passlock-1.0.8/passlock.egg-info/top_level.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-02 17:26:53.659196 passlock-1.0.8/setup.cfg
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      754 2023-06-02 17:26:51.000000 passlock-1.0.8/setup.py
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:31:53.737393 passlock-1.0.9/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     6027 2023-06-02 17:31:53.737393 passlock-1.0.9/PKG-INFO
+-rwxrwxr-x   0 praveen   (1000) praveen   (1000)     5713 2023-06-02 17:31:44.000000 passlock-1.0.9/README.md
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:31:53.733393 passlock-1.0.9/passlock/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:51:00.000000 passlock-1.0.9/passlock/__init__.py
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:31:53.737393 passlock-1.0.9/passlock.egg-info/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     6027 2023-06-02 17:31:53.000000 passlock-1.0.9/passlock.egg-info/PKG-INFO
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      233 2023-06-02 17:31:53.000000 passlock-1.0.9/passlock.egg-info/SOURCES.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 17:31:53.000000 passlock-1.0.9/passlock.egg-info/dependency_links.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       53 2023-06-02 17:31:53.000000 passlock-1.0.9/passlock.egg-info/entry_points.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-02 17:31:53.000000 passlock-1.0.9/passlock.egg-info/requires.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        9 2023-06-02 17:31:53.000000 passlock-1.0.9/passlock.egg-info/top_level.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-02 17:31:53.737393 passlock-1.0.9/setup.cfg
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      754 2023-06-02 17:31:51.000000 passlock-1.0.9/setup.py
```

### Comparing `passlock-1.0.8/PKG-INFO` & `passlock-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passlock
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple password manager
 Home-page: https://github.com/Praveenms13/PyMongo-PasswordManager-CommandLineTool
 Author: M S Praveen Kumar
 Author-email: mspraveenkumar77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -30,25 +30,20 @@
 Before running this password manager, please ensure that the following requirements are met:
 
 - Python 3.x is installed on your system.
 - MongoDB is installed and running.
 
 ## Installation
 
-To Install this tool run :
+To Install this tool via pip :
 
 ```bash
-  git clone git@github.com:Praveenms13/PyMongo-PasswordManager.git
-```
-
-Navigate to the project directory:
-
-```
-cd Password_Manager/
+pip install passlock
 ```
+pip package url: https://pypi.org/project/passlock/
 
 install the required packages
 
 ```
 pip install pymongo
 pip install json
 pip install sys
```

### Comparing `passlock-1.0.8/README.md` & `passlock-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,20 @@
 Before running this password manager, please ensure that the following requirements are met:
 
 - Python 3.x is installed on your system.
 - MongoDB is installed and running.
 
 ## Installation
 
-To Install this tool run :
+To Install this tool via pip :
 
 ```bash
-  git clone git@github.com:Praveenms13/PyMongo-PasswordManager.git
-```
-
-Navigate to the project directory:
-
-```
-cd Password_Manager/
+pip install passlock
 ```
+pip package url: https://pypi.org/project/passlock/
 
 install the required packages
 
 ```
 pip install pymongo
 pip install json
 pip install sys
```

### Comparing `passlock-1.0.8/passlock.egg-info/PKG-INFO` & `passlock-1.0.9/passlock.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passlock
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple password manager
 Home-page: https://github.com/Praveenms13/PyMongo-PasswordManager-CommandLineTool
 Author: M S Praveen Kumar
 Author-email: mspraveenkumar77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -30,25 +30,20 @@
 Before running this password manager, please ensure that the following requirements are met:
 
 - Python 3.x is installed on your system.
 - MongoDB is installed and running.
 
 ## Installation
 
-To Install this tool run :
+To Install this tool via pip :
 
 ```bash
-  git clone git@github.com:Praveenms13/PyMongo-PasswordManager.git
-```
-
-Navigate to the project directory:
-
-```
-cd Password_Manager/
+pip install passlock
 ```
+pip package url: https://pypi.org/project/passlock/
 
 install the required packages
 
 ```
 pip install pymongo
 pip install json
 pip install sys
```

### Comparing `passlock-1.0.8/setup.py` & `passlock-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     required = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="passlock",
-    version="1.0.8",
+    version="1.0.9",
     author="M S Praveen Kumar",
     author_email="mspraveenkumar77@gmail.com",
     description="A simple password manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=required,
```

