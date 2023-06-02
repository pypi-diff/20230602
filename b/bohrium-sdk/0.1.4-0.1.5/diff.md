# Comparing `tmp/bohrium-sdk-0.1.4.tar.gz` & `tmp/bohrium-sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.1.4.tar", last modified: Tue May 30 07:26:08 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.1.5.tar", last modified: Fri Jun  2 07:32:26 2023, max compression
```

## Comparing `bohrium-sdk-0.1.4.tar` & `bohrium-sdk-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:26:08.436625 bohrium-sdk-0.1.4/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-30 07:26:08.436307 bohrium-sdk-0.1.4/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.1.4/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:26:08.429417 bohrium-sdk-0.1.4/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-30 07:26:08.000000 bohrium-sdk-0.1.4/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      493 2023-05-30 07:26:08.000000 bohrium-sdk-0.1.4/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-30 07:26:08.000000 bohrium-sdk-0.1.4/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-05-30 07:26:08.000000 bohrium-sdk-0.1.4/bohrium_sdk.egg-info/entry_points.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       13 2023-05-30 07:26:08.000000 bohrium-sdk-0.1.4/bohrium_sdk.egg-info/requires.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-05-30 07:26:08.000000 bohrium-sdk-0.1.4/bohrium_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:26:08.433804 bohrium-sdk-0.1.4/bohriumsdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.1.4/bohriumsdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.1.4/bohriumsdk/__main__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     6220 2023-05-30 07:14:12.000000 bohrium-sdk-0.1.4/bohriumsdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1970 2023-05-30 07:06:19.000000 bohrium-sdk-0.1.4/bohriumsdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     3766 2023-05-30 07:06:03.000000 bohrium-sdk-0.1.4/bohriumsdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.1.4/bohriumsdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2223 2023-05-30 07:25:30.000000 bohrium-sdk-0.1.4/bohriumsdk/project.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2835 2023-05-30 07:06:55.000000 bohrium-sdk-0.1.4/bohriumsdk/storage.py
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:26:08.435659 bohrium-sdk-0.1.4/bohriumsdk/test/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.1.4/bohriumsdk/test/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.1.4/bohriumsdk/test/test_node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2369 2023-05-30 01:45:00.000000 bohrium-sdk-0.1.4/bohriumsdk/test.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     3427 2023-05-30 07:24:18.000000 bohrium-sdk-0.1.4/bohriumsdk/util.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-30 07:26:08.436692 bohrium-sdk-0.1.4/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      515 2023-05-30 07:25:38.000000 bohrium-sdk-0.1.4/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 07:32:26.381287 bohrium-sdk-0.1.5/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-02 07:32:26.381085 bohrium-sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.1.5/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 07:32:26.374900 bohrium-sdk-0.1.5/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-02 07:32:26.000000 bohrium-sdk-0.1.5/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      493 2023-06-02 07:32:26.000000 bohrium-sdk-0.1.5/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-06-02 07:32:26.000000 bohrium-sdk-0.1.5/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-06-02 07:32:26.000000 bohrium-sdk-0.1.5/bohrium_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       13 2023-06-02 07:32:26.000000 bohrium-sdk-0.1.5/bohrium_sdk.egg-info/requires.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-06-02 07:32:26.000000 bohrium-sdk-0.1.5/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 07:32:26.379742 bohrium-sdk-0.1.5/bohriumsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.1.5/bohriumsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.1.5/bohriumsdk/__main__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     6220 2023-05-30 07:14:12.000000 bohrium-sdk-0.1.5/bohriumsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1970 2023-05-30 07:06:19.000000 bohrium-sdk-0.1.5/bohriumsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     3766 2023-05-30 07:06:03.000000 bohrium-sdk-0.1.5/bohriumsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.1.5/bohriumsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2223 2023-05-30 07:25:30.000000 bohrium-sdk-0.1.5/bohriumsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2835 2023-05-30 07:06:55.000000 bohrium-sdk-0.1.5/bohriumsdk/storage.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 07:32:26.380666 bohrium-sdk-0.1.5/bohriumsdk/test/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.1.5/bohriumsdk/test/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.1.5/bohriumsdk/test/test_node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2369 2023-05-30 01:45:00.000000 bohrium-sdk-0.1.5/bohriumsdk/test.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4730 2023-06-02 07:31:47.000000 bohrium-sdk-0.1.5/bohriumsdk/util.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-06-02 07:32:26.381353 bohrium-sdk-0.1.5/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      515 2023-06-02 07:32:20.000000 bohrium-sdk-0.1.5/setup.py
```

### Comparing `bohrium-sdk-0.1.4/bohriumsdk/client.py` & `bohrium-sdk-0.1.5/bohriumsdk/client.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.4/bohriumsdk/image.py` & `bohrium-sdk-0.1.5/bohriumsdk/image.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.4/bohriumsdk/job.py` & `bohrium-sdk-0.1.5/bohriumsdk/job.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.4/bohriumsdk/node.py` & `bohrium-sdk-0.1.5/bohriumsdk/node.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.4/bohriumsdk/project.py` & `bohrium-sdk-0.1.5/bohriumsdk/project.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.4/bohriumsdk/storage.py` & `bohrium-sdk-0.1.5/bohriumsdk/storage.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.4/bohriumsdk/test.py` & `bohrium-sdk-0.1.5/bohriumsdk/test.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.4/setup.py` & `bohrium-sdk-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 import setuptools
 setup(
     name="bohrium-sdk",
-    version="0.1.4",
+    version="0.1.5",
     author="dingzhaohan",
     author_email="dingzh@dp.tech",
     url="https://github.com/dingzhoahan",
     description="bohrium openapi python sdk",
     packages=setuptools.find_packages(),
     install_requires=['jupyter-rich'],
     python_requires='>=3.7',
```

