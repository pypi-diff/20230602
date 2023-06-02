# Comparing `tmp/hybrid_index-0.0.11.tar.gz` & `tmp/hybrid_index-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hybrid_index-0.0.11.tar", last modified: Fri Jun  2 10:11:54 2023, max compression
+gzip compressed data, was "hybrid_index-0.1.0.tar", last modified: Fri Jun  2 09:44:51 2023, max compression
```

## Comparing `hybrid_index-0.0.11.tar` & `hybrid_index-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 10:11:54.316802 hybrid_index-0.0.11/
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      481 2023-06-02 10:11:54.316802 hybrid_index-0.0.11/PKG-INFO
-drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 10:11:54.312801 hybrid_index-0.0.11/hybrid/
-drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 10:11:54.312801 hybrid_index-0.0.11/hybrid/hybrid_index/
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)       83 2023-06-02 09:42:53.000000 hybrid_index-0.0.11/hybrid/hybrid_index/__init__.py
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)     7078 2023-06-02 08:36:03.000000 hybrid_index-0.0.11/hybrid/hybrid_index/index.py
-drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 10:11:54.312801 hybrid_index-0.0.11/hybrid/hybrid_index.egg-info/
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      481 2023-06-02 10:11:54.000000 hybrid_index-0.0.11/hybrid/hybrid_index.egg-info/PKG-INFO
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      283 2023-06-02 10:11:54.000000 hybrid_index-0.0.11/hybrid/hybrid_index.egg-info/SOURCES.txt
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)        1 2023-06-02 10:11:54.000000 hybrid_index-0.0.11/hybrid/hybrid_index.egg-info/dependency_links.txt
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      359 2023-06-02 10:11:54.000000 hybrid_index-0.0.11/hybrid/hybrid_index.egg-info/requires.txt
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)       13 2023-06-02 10:11:54.000000 hybrid_index-0.0.11/hybrid/hybrid_index.egg-info/top_level.txt
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)       38 2023-06-02 10:11:54.316802 hybrid_index-0.0.11/setup.cfg
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)     1410 2023-06-02 10:09:08.000000 hybrid_index-0.0.11/setup.py
+drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 09:44:51.848622 hybrid_index-0.1.0/
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      549 2023-06-02 09:44:51.848622 hybrid_index-0.1.0/PKG-INFO
+drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 09:44:51.844622 hybrid_index-0.1.0/hybrid/
+drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 09:44:51.848622 hybrid_index-0.1.0/hybrid/hybrid_index/
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)       83 2023-06-02 09:42:53.000000 hybrid_index-0.1.0/hybrid/hybrid_index/__init__.py
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)     7078 2023-06-02 08:36:03.000000 hybrid_index-0.1.0/hybrid/hybrid_index/index.py
+drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 09:44:51.848622 hybrid_index-0.1.0/hybrid/hybrid_index.egg-info/
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      549 2023-06-02 09:44:51.000000 hybrid_index-0.1.0/hybrid/hybrid_index.egg-info/PKG-INFO
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      308 2023-06-02 09:44:51.000000 hybrid_index-0.1.0/hybrid/hybrid_index.egg-info/SOURCES.txt
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)        1 2023-06-02 09:44:51.000000 hybrid_index-0.1.0/hybrid/hybrid_index.egg-info/dependency_links.txt
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      393 2023-06-02 09:44:51.000000 hybrid_index-0.1.0/hybrid/hybrid_index.egg-info/requires.txt
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)       13 2023-06-02 09:44:51.000000 hybrid_index-0.1.0/hybrid/hybrid_index.egg-info/top_level.txt
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      968 2023-06-02 09:14:47.000000 hybrid_index-0.1.0/pyproject.toml
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      555 2023-06-02 09:44:51.848622 hybrid_index-0.1.0/setup.cfg
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)     1464 2023-06-02 09:43:20.000000 hybrid_index-0.1.0/setup.py
```

### Comparing `hybrid_index-0.0.11/hybrid/hybrid_index/index.py` & `hybrid_index-0.1.0/hybrid/hybrid_index/index.py`

 * *Files identical despite different names*

### Comparing `hybrid_index-0.0.11/setup.py` & `hybrid_index-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("hybrid/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="hybrid_index",
-    version="0.0.11",
+    version="0.0.10",
     description="Easy to use hybrid index for semantic + keyword search",
     package_dir={"": "hybrid"},
     packages=find_packages(where="hybrid"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gigagiova/hybrid-index",
     author="Giovanni del Gallo",
@@ -29,14 +29,16 @@
       "charset-normalizer >=3.1.0",
       "click",
       "distlib >=0.3.6",
       "faiss-gpu >=1.7.2",
       "filelock >=3.10.7",
       "frozenlist >=1.3.3",
       "idna >=3.4",
+      "mkl-fft >=1.3.6",
+      "mkl-service >=2.4.0",
       "multidict >=6.0.4",
       "nltk",
       "numpy",
       "openai >=0.27.7",
       "platformdirs >=3.2.0",
       "regex",
       "requests >=2.31.0",
```

