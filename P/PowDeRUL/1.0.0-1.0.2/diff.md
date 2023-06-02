# Comparing `tmp/PowDeRUL-1.0.0.tar.gz` & `tmp/PowDeRUL-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PowDeRUL-1.0.0.tar", last modified: Fri Jun  2 08:03:53 2023, max compression
+gzip compressed data, was "PowDeRUL-1.0.2.tar", last modified: Fri Jun  2 08:22:34 2023, max compression
```

## Comparing `PowDeRUL-1.0.0.tar` & `PowDeRUL-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 08:03:53.484689 PowDeRUL-1.0.0/
--rw-------   0 runner    (1000) runner    (1000)     1060 2023-06-02 07:54:31.000000 PowDeRUL-1.0.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 08:03:53.484689 PowDeRUL-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 08:03:53.484689 PowDeRUL-1.0.0/PowDeRUL.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 08:03:53.000000 PowDeRUL-1.0.0/PowDeRUL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      210 2023-06-02 08:03:53.000000 PowDeRUL-1.0.0/PowDeRUL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 08:03:53.000000 PowDeRUL-1.0.0/PowDeRUL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      120 2023-06-02 08:03:53.000000 PowDeRUL-1.0.0/PowDeRUL.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 08:03:53.000000 PowDeRUL-1.0.0/PowDeRUL.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)     3909 2023-06-02 07:54:31.000000 PowDeRUL-1.0.0/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 PowDeRUL-1.0.0/pyproject.toml
--rw-------   0 runner    (1000) runner    (1000)      519 2023-06-02 08:03:53.488689 PowDeRUL-1.0.0/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      759 2023-06-02 08:03:22.000000 PowDeRUL-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 08:22:34.282646 PowDeRUL-1.0.2/
+-rw-------   0 runner    (1000) runner    (1000)     1060 2023-06-02 07:54:31.000000 PowDeRUL-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 08:22:34.282646 PowDeRUL-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 08:22:34.282646 PowDeRUL-1.0.2/PowDeRUL.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 08:22:33.000000 PowDeRUL-1.0.2/PowDeRUL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      210 2023-06-02 08:22:33.000000 PowDeRUL-1.0.2/PowDeRUL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 08:22:33.000000 PowDeRUL-1.0.2/PowDeRUL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      120 2023-06-02 08:22:33.000000 PowDeRUL-1.0.2/PowDeRUL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 08:22:33.000000 PowDeRUL-1.0.2/PowDeRUL.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)     3909 2023-06-02 07:54:31.000000 PowDeRUL-1.0.2/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      429 2023-06-02 08:21:26.000000 PowDeRUL-1.0.2/pyproject.toml
+-rw-------   0 runner    (1000) runner    (1000)      519 2023-06-02 08:22:34.286646 PowDeRUL-1.0.2/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      759 2023-06-02 08:21:23.000000 PowDeRUL-1.0.2/setup.py
```

### Comparing `PowDeRUL-1.0.0/LICENSE` & `PowDeRUL-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PowDeRUL-1.0.0/README.md` & `PowDeRUL-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PowDeRUL-1.0.0/setup.cfg` & `PowDeRUL-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PowDeRUL
-version = 0.0.1
+version = 1.0.2
 author = PGarn
 author_email = paul.garnier@ens-rennes.fr
 description = Python package for calculating lifetime of components
 url = https://github.com/PGarn/LifeTime
 
 [options]
 packages = find:
```

### Comparing `PowDeRUL-1.0.0/setup.py` & `PowDeRUL-1.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PowDeRUL',
-    version='1.0.0',
+    version='1.0.2',
     description='Python package for calculating lifetime of components',
     author='PGarn',
     author_email='paul.garnier@ens-rennes.fr',
     url='https://github.com/PGarn/LifeTime',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

