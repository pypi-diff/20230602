# Comparing `tmp/pyRealEstate-0.0.1.tar.gz` & `tmp/pyRealEstate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRealEstate-0.0.1.tar", last modified: Fri Jun  2 21:43:14 2023, max compression
+gzip compressed data, was "pyRealEstate-0.0.2.tar", last modified: Fri Jun  2 21:53:20 2023, max compression
```

## Comparing `pyRealEstate-0.0.1.tar` & `pyRealEstate-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:43:14.555574 pyRealEstate-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-02 21:43:04.000000 pyRealEstate-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-02 21:43:14.555574 pyRealEstate-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:43:14.555574 pyRealEstate-0.0.1/pyRealEstate/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-02 21:43:04.000000 pyRealEstate-0.0.1/pyRealEstate/RealEstateMetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:43:04.000000 pyRealEstate-0.0.1/pyRealEstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:43:14.555574 pyRealEstate-0.0.1/pyRealEstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-02 21:43:14.000000 pyRealEstate-0.0.1/pyRealEstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-02 21:43:14.000000 pyRealEstate-0.0.1/pyRealEstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:43:14.000000 pyRealEstate-0.0.1/pyRealEstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 21:43:14.000000 pyRealEstate-0.0.1/pyRealEstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 21:43:14.000000 pyRealEstate-0.0.1/pyRealEstate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-02 21:43:04.000000 pyRealEstate-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-02 21:43:14.555574 pyRealEstate-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:20.865359 pyRealEstate-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-02 21:53:11.000000 pyRealEstate-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-02 21:53:20.865359 pyRealEstate-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-02 21:53:11.000000 pyRealEstate-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:20.865359 pyRealEstate-0.0.2/pyRealEstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-02 21:53:11.000000 pyRealEstate-0.0.2/pyRealEstate/RealEstateMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:53:11.000000 pyRealEstate-0.0.2/pyRealEstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:20.865359 pyRealEstate-0.0.2/pyRealEstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-02 21:53:20.000000 pyRealEstate-0.0.2/pyRealEstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-02 21:53:20.000000 pyRealEstate-0.0.2/pyRealEstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:53:20.000000 pyRealEstate-0.0.2/pyRealEstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 21:53:20.000000 pyRealEstate-0.0.2/pyRealEstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 21:53:20.000000 pyRealEstate-0.0.2/pyRealEstate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-02 21:53:11.000000 pyRealEstate-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-02 21:53:20.865359 pyRealEstate-0.0.2/setup.cfg
```

### Comparing `pyRealEstate-0.0.1/LICENSE` & `pyRealEstate-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.1/setup.cfg` & `pyRealEstate-0.0.2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = pyRealEstate
-version = 0.0.1
+version = 0.0.2
 author = Joshua Jorgensen
 author_email = joshua.j.jorgensen@gmail.com
 description = package to assist with data analytics in real estate
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/Joshua-Data-Wizard
+url = https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 install_requires = scikit-learn
```

