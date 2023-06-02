# Comparing `tmp/sunwoolabs-0.0.1.tar.gz` & `tmp/sunwoolabs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunwoolabs-0.0.1.tar", last modified: Fri Jun  2 05:48:47 2023, max compression
+gzip compressed data, was "sunwoolabs-0.0.2.tar", last modified: Fri Jun  2 06:15:32 2023, max compression
```

## Comparing `sunwoolabs-0.0.1.tar` & `sunwoolabs-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 05:48:47.208102 sunwoolabs-0.0.1/
--rw-rw-rw-   0        0        0      443 2023-06-02 05:48:47.207103 sunwoolabs-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 05:48:47.179104 sunwoolabs-0.0.1/sample/
--rw-rw-rw-   0        0        0        0 2023-06-02 05:47:06.000000 sunwoolabs-0.0.1/sample/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-02 05:48:47.209013 sunwoolabs-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      711 2023-06-02 05:46:44.000000 sunwoolabs-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:48:47.205101 sunwoolabs-0.0.1/sunwoolabs.egg-info/
--rw-rw-rw-   0        0        0      443 2023-06-02 05:48:47.000000 sunwoolabs-0.0.1/sunwoolabs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-06-02 05:48:47.000000 sunwoolabs-0.0.1/sunwoolabs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 05:48:47.000000 sunwoolabs-0.0.1/sunwoolabs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-02 05:48:47.000000 sunwoolabs-0.0.1/sunwoolabs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-02 05:48:47.000000 sunwoolabs-0.0.1/sunwoolabs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 05:48:47.000000 sunwoolabs-0.0.1/sunwoolabs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 06:15:32.274919 sunwoolabs-0.0.2/
+-rw-rw-rw-   0        0        0      443 2023-06-02 06:15:32.272919 sunwoolabs-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 06:15:32.257918 sunwoolabs-0.0.2/sample/
+-rw-rw-rw-   0        0        0       72 2023-06-02 06:14:13.000000 sunwoolabs-0.0.2/sample/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-02 06:15:32.274919 sunwoolabs-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      711 2023-06-02 06:13:02.000000 sunwoolabs-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 06:15:32.271919 sunwoolabs-0.0.2/sunwoolabs.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-06-02 06:15:32.000000 sunwoolabs-0.0.2/sunwoolabs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-06-02 06:15:32.000000 sunwoolabs-0.0.2/sunwoolabs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 06:15:32.000000 sunwoolabs-0.0.2/sunwoolabs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 05:48:47.000000 sunwoolabs-0.0.2/sunwoolabs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-02 06:15:32.000000 sunwoolabs-0.0.2/sunwoolabs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 06:15:32.000000 sunwoolabs-0.0.2/sunwoolabs.egg-info/top_level.txt
```

### Comparing `sunwoolabs-0.0.1/setup.py` & `sunwoolabs-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sunwoolabs",
-    version="0.0.1",
+    version="0.0.2",
     description="preprocessing module for time series",
     author="Heo, Sun-Woo",
     author_email="tjsdn447@hanyang.ac.kr",
     url="http://github.com/Ssunder4s/",
     install_requires=['pandas', 'numpy'], # 수정 필요
     packages=find_packages(exclude=['tests*']),
     keywords=['dfmodule_sw', 'time series', 'sequentila'],
```

