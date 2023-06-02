# Comparing `tmp/reflect-client-1.0.0.tar.gz` & `tmp/reflect-client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflect-client-1.0.0.tar", last modified: Mon May  1 16:03:57 2023, max compression
+gzip compressed data, was "reflect-client-1.0.1.tar", last modified: Fri Jun  2 10:44:21 2023, max compression
```

## Comparing `reflect-client-1.0.0.tar` & `reflect-client-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-05-01 16:03:57.392304 reflect-client-1.0.0/
--rw-r--r--   0 victor    (1000) victor    (1000)      350 2023-05-01 16:03:57.391304 reflect-client-1.0.0/PKG-INFO
--rw-r--r--   0 victor    (1000) victor    (1000)     2027 2023-05-01 16:03:33.000000 reflect-client-1.0.0/README.md
-drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-05-01 16:03:57.390304 reflect-client-1.0.0/reflect_client.egg-info/
--rw-r--r--   0 victor    (1000) victor    (1000)      350 2023-05-01 16:03:57.000000 reflect-client-1.0.0/reflect_client.egg-info/PKG-INFO
--rw-r--r--   0 victor    (1000) victor    (1000)      237 2023-05-01 16:03:57.000000 reflect-client-1.0.0/reflect_client.egg-info/SOURCES.txt
--rw-r--r--   0 victor    (1000) victor    (1000)        1 2023-05-01 16:03:57.000000 reflect-client-1.0.0/reflect_client.egg-info/dependency_links.txt
--rw-r--r--   0 victor    (1000) victor    (1000)       11 2023-05-01 16:03:57.000000 reflect-client-1.0.0/reflect_client.egg-info/requires.txt
--rw-r--r--   0 victor    (1000) victor    (1000)        4 2023-05-01 16:03:57.000000 reflect-client-1.0.0/reflect_client.egg-info/top_level.txt
--rw-r--r--   0 victor    (1000) victor    (1000)       38 2023-05-01 16:03:57.392304 reflect-client-1.0.0/setup.cfg
--rw-r--r--   0 victor    (1000) victor    (1000)      514 2023-05-01 15:17:35.000000 reflect-client-1.0.0/setup.py
-drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-05-01 16:03:57.390304 reflect-client-1.0.0/src/
--rw-r--r--   0 victor    (1000) victor    (1000)     3944 2023-05-01 13:15:11.000000 reflect-client-1.0.0/src/Client.py
--rw-r--r--   0 victor    (1000) victor    (1000)        0 2023-05-01 15:17:35.000000 reflect-client-1.0.0/src/__init__.py
+drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-02 10:44:21.520117 reflect-client-1.0.1/
+-rw-r--r--   0 victor    (1000) victor    (1000)      350 2023-06-02 10:44:21.519117 reflect-client-1.0.1/PKG-INFO
+-rw-r--r--   0 victor    (1000) victor    (1000)     2027 2023-05-01 16:03:33.000000 reflect-client-1.0.1/README.md
+drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-02 10:44:21.517118 reflect-client-1.0.1/reflect_client/
+-rw-r--r--   0 victor    (1000) victor    (1000)     3944 2023-05-01 13:15:11.000000 reflect-client-1.0.1/reflect_client/Client.py
+-rw-r--r--   0 victor    (1000) victor    (1000)        0 2023-05-01 15:17:35.000000 reflect-client-1.0.1/reflect_client/__init__.py
+drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-02 10:44:21.519117 reflect-client-1.0.1/reflect_client.egg-info/
+-rw-r--r--   0 victor    (1000) victor    (1000)      350 2023-06-02 10:44:21.000000 reflect-client-1.0.1/reflect_client.egg-info/PKG-INFO
+-rw-r--r--   0 victor    (1000) victor    (1000)      259 2023-06-02 10:44:21.000000 reflect-client-1.0.1/reflect_client.egg-info/SOURCES.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)        1 2023-06-02 10:44:21.000000 reflect-client-1.0.1/reflect_client.egg-info/dependency_links.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)       11 2023-06-02 10:44:21.000000 reflect-client-1.0.1/reflect_client.egg-info/requires.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)       15 2023-06-02 10:44:21.000000 reflect-client-1.0.1/reflect_client.egg-info/top_level.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)       38 2023-06-02 10:44:21.520117 reflect-client-1.0.1/setup.cfg
+-rw-r--r--   0 victor    (1000) victor    (1000)      517 2023-06-02 10:43:50.000000 reflect-client-1.0.1/setup.py
```

### Comparing `reflect-client-1.0.0/README.md` & `reflect-client-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `reflect-client-1.0.0/setup.py` & `reflect-client-1.0.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "reflect-client",
-    version = "1.0.0",
+    version = "1.0.1",
     description = "Python library for communicating with an API built with Reflect over HTTP or UNIX sockets",
     author = "Victor Westerlund",
     author_email = "victor.vesterlund@gmail.com",
     url = "https://github.com/victorwesterlund/reflect-client-python",
-    packages = find_packages(),
+    packages = ["reflect_client"],
     # The requirement.txt file should also be updated when changing this
     install_requires = ["validators"]
 )
```

### Comparing `reflect-client-1.0.0/src/Client.py` & `reflect-client-1.0.1/reflect_client/Client.py`

 * *Files identical despite different names*

