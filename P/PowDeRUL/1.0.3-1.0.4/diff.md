# Comparing `tmp/PowDeRUL-1.0.3.tar.gz` & `tmp/PowDeRUL-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PowDeRUL-1.0.3.tar", last modified: Fri Jun  2 09:22:21 2023, max compression
+gzip compressed data, was "PowDeRUL-1.0.4.tar", last modified: Fri Jun  2 09:28:46 2023, max compression
```

## Comparing `PowDeRUL-1.0.3.tar` & `PowDeRUL-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 09:22:21.504227 PowDeRUL-1.0.3/
--rw-------   0 runner    (1000) runner    (1000)     1060 2023-06-02 07:54:31.000000 PowDeRUL-1.0.3/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 09:22:21.504227 PowDeRUL-1.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 09:22:21.504227 PowDeRUL-1.0.3/PowDeRUL.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 09:22:21.000000 PowDeRUL-1.0.3/PowDeRUL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      210 2023-06-02 09:22:21.000000 PowDeRUL-1.0.3/PowDeRUL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 09:22:21.000000 PowDeRUL-1.0.3/PowDeRUL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      120 2023-06-02 09:22:21.000000 PowDeRUL-1.0.3/PowDeRUL.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 09:22:21.000000 PowDeRUL-1.0.3/PowDeRUL.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)     3909 2023-06-02 07:54:31.000000 PowDeRUL-1.0.3/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      429 2023-06-02 09:22:14.000000 PowDeRUL-1.0.3/pyproject.toml
--rw-------   0 runner    (1000) runner    (1000)      519 2023-06-02 09:22:21.504227 PowDeRUL-1.0.3/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      833 2023-06-02 09:22:02.000000 PowDeRUL-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 09:28:46.380127 PowDeRUL-1.0.4/
+-rw-------   0 runner    (1000) runner    (1000)     1060 2023-06-02 07:54:31.000000 PowDeRUL-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 09:28:46.380127 PowDeRUL-1.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 09:28:46.380127 PowDeRUL-1.0.4/PowDeRUL.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 09:28:46.000000 PowDeRUL-1.0.4/PowDeRUL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      200 2023-06-02 09:28:46.000000 PowDeRUL-1.0.4/PowDeRUL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 09:28:46.000000 PowDeRUL-1.0.4/PowDeRUL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      120 2023-06-02 09:28:46.000000 PowDeRUL-1.0.4/PowDeRUL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 09:28:46.000000 PowDeRUL-1.0.4/PowDeRUL.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)     3909 2023-06-02 07:54:31.000000 PowDeRUL-1.0.4/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      429 2023-06-02 09:28:31.000000 PowDeRUL-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-02 09:28:46.380127 PowDeRUL-1.0.4/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      833 2023-06-02 09:28:18.000000 PowDeRUL-1.0.4/setup.py
```

### Comparing `PowDeRUL-1.0.3/LICENSE` & `PowDeRUL-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PowDeRUL-1.0.3/README.md` & `PowDeRUL-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `PowDeRUL-1.0.3/setup.py` & `PowDeRUL-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PowDeRUL',
-    version='1.0.3',
+    version='1.0.4',
     description='Python package for calculating lifetime of components',
     author='PGarn',
     author_email='paul.garnier@ens-rennes.fr',
     url='https://github.com/PGarn/LifeTime',
     packages=find_packages(),
     package_data={
         'PowDeRUL': ['function/*','example/*'],
```

