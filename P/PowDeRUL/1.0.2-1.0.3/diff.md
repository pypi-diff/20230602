# Comparing `tmp/PowDeRUL-1.0.2.tar.gz` & `tmp/PowDeRUL-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PowDeRUL-1.0.2.tar", last modified: Fri Jun  2 08:22:34 2023, max compression
+gzip compressed data, was "PowDeRUL-1.0.3.tar", last modified: Fri Jun  2 09:22:21 2023, max compression
```

## Comparing `PowDeRUL-1.0.2.tar` & `PowDeRUL-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 08:22:34.282646 PowDeRUL-1.0.2/
--rw-------   0 runner    (1000) runner    (1000)     1060 2023-06-02 07:54:31.000000 PowDeRUL-1.0.2/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 08:22:34.282646 PowDeRUL-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 08:22:34.282646 PowDeRUL-1.0.2/PowDeRUL.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 08:22:33.000000 PowDeRUL-1.0.2/PowDeRUL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      210 2023-06-02 08:22:33.000000 PowDeRUL-1.0.2/PowDeRUL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 08:22:33.000000 PowDeRUL-1.0.2/PowDeRUL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      120 2023-06-02 08:22:33.000000 PowDeRUL-1.0.2/PowDeRUL.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 08:22:33.000000 PowDeRUL-1.0.2/PowDeRUL.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)     3909 2023-06-02 07:54:31.000000 PowDeRUL-1.0.2/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      429 2023-06-02 08:21:26.000000 PowDeRUL-1.0.2/pyproject.toml
--rw-------   0 runner    (1000) runner    (1000)      519 2023-06-02 08:22:34.286646 PowDeRUL-1.0.2/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      759 2023-06-02 08:21:23.000000 PowDeRUL-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 09:22:21.504227 PowDeRUL-1.0.3/
+-rw-------   0 runner    (1000) runner    (1000)     1060 2023-06-02 07:54:31.000000 PowDeRUL-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 09:22:21.504227 PowDeRUL-1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 09:22:21.504227 PowDeRUL-1.0.3/PowDeRUL.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 09:22:21.000000 PowDeRUL-1.0.3/PowDeRUL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      210 2023-06-02 09:22:21.000000 PowDeRUL-1.0.3/PowDeRUL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 09:22:21.000000 PowDeRUL-1.0.3/PowDeRUL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      120 2023-06-02 09:22:21.000000 PowDeRUL-1.0.3/PowDeRUL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 09:22:21.000000 PowDeRUL-1.0.3/PowDeRUL.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)     3909 2023-06-02 07:54:31.000000 PowDeRUL-1.0.3/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      429 2023-06-02 09:22:14.000000 PowDeRUL-1.0.3/pyproject.toml
+-rw-------   0 runner    (1000) runner    (1000)      519 2023-06-02 09:22:21.504227 PowDeRUL-1.0.3/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      833 2023-06-02 09:22:02.000000 PowDeRUL-1.0.3/setup.py
```

### Comparing `PowDeRUL-1.0.2/LICENSE` & `PowDeRUL-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PowDeRUL-1.0.2/README.md` & `PowDeRUL-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PowDeRUL-1.0.2/setup.cfg` & `PowDeRUL-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PowDeRUL
-version = 1.0.2
+version = 1.0.3
 author = PGarn
 author_email = paul.garnier@ens-rennes.fr
 description = Python package for calculating lifetime of components
 url = https://github.com/PGarn/LifeTime
 
 [options]
 packages = find:
```

### Comparing `PowDeRUL-1.0.2/setup.py` & `PowDeRUL-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PowDeRUL',
-    version='1.0.2',
+    version='1.0.3',
     description='Python package for calculating lifetime of components',
     author='PGarn',
     author_email='paul.garnier@ens-rennes.fr',
     url='https://github.com/PGarn/LifeTime',
     packages=find_packages(),
+    package_data={
+        'PowDeRUL': ['function/*','example/*'],
+    },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
     ],
     install_requires=[
```

