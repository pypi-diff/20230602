# Comparing `tmp/phase_dev-0.0.3.tar.gz` & `tmp/phase_dev-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phase_dev-0.0.3.tar", last modified: Thu Jun  1 07:30:02 2023, max compression
+gzip compressed data, was "phase_dev-1.0.0.tar", last modified: Fri Jun  2 10:03:31 2023, max compression
```

## Comparing `phase_dev-0.0.3.tar` & `phase_dev-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-01 07:30:02.903530 phase_dev-0.0.3/
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1062 2023-06-01 07:28:57.000000 phase_dev-0.0.3/LICENSE
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)      913 2023-06-01 07:30:02.903530 phase_dev-0.0.3/PKG-INFO
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)      447 2023-04-28 13:48:35.000000 phase_dev-0.0.3/README.md
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)      659 2023-06-01 07:29:42.000000 phase_dev-0.0.3/pyproject.toml
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)       38 2023-06-01 07:30:02.903530 phase_dev-0.0.3/setup.cfg
-drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-01 07:30:02.900530 phase_dev-0.0.3/src/
-drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-01 07:30:02.901530 phase_dev-0.0.3/src/phase/
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)       46 2023-06-01 07:28:57.000000 phase_dev-0.0.3/src/phase/__init__.py
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)     3510 2023-06-01 07:28:57.000000 phase_dev-0.0.3/src/phase/phase.py
-drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-01 07:30:02.901530 phase_dev-0.0.3/src/phase/utils/
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)        0 2023-06-01 07:28:57.000000 phase_dev-0.0.3/src/phase/utils/__init__.py
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)     4728 2023-06-01 07:28:57.000000 phase_dev-0.0.3/src/phase/utils/crypto.py
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)       44 2023-06-01 07:28:57.000000 phase_dev-0.0.3/src/phase/version.py
-drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-01 07:30:02.902530 phase_dev-0.0.3/src/phase_dev.egg-info/
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)      913 2023-06-01 07:30:02.000000 phase_dev-0.0.3/src/phase_dev.egg-info/PKG-INFO
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)      395 2023-06-01 07:30:02.000000 phase_dev-0.0.3/src/phase_dev.egg-info/SOURCES.txt
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)        1 2023-06-01 07:30:02.000000 phase_dev-0.0.3/src/phase_dev.egg-info/dependency_links.txt
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)       55 2023-06-01 07:30:02.000000 phase_dev-0.0.3/src/phase_dev.egg-info/requires.txt
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)        6 2023-06-01 07:30:02.000000 phase_dev-0.0.3/src/phase_dev.egg-info/top_level.txt
-drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-01 07:30:02.903530 phase_dev-0.0.3/tests/
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1504 2023-06-01 07:28:57.000000 phase_dev-0.0.3/tests/test_decrypt.py
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1378 2023-05-28 08:54:34.000000 phase_dev-0.0.3/tests/test_encrypt.py
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1103 2023-06-01 07:28:57.000000 phase_dev-0.0.3/tests/test_init.py
+drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-02 10:03:31.985133 phase_dev-1.0.0/
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1062 2023-06-01 07:28:57.000000 phase_dev-1.0.0/LICENSE
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)      913 2023-06-02 10:03:31.984133 phase_dev-1.0.0/PKG-INFO
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)      447 2023-06-02 09:41:28.000000 phase_dev-1.0.0/README.md
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)      659 2023-06-02 09:41:35.000000 phase_dev-1.0.0/pyproject.toml
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)       38 2023-06-02 10:03:31.985133 phase_dev-1.0.0/setup.cfg
+drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-02 10:03:31.981133 phase_dev-1.0.0/src/
+drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-02 10:03:31.982133 phase_dev-1.0.0/src/phase/
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)       46 2023-06-01 07:28:57.000000 phase_dev-1.0.0/src/phase/__init__.py
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)     3510 2023-06-01 07:28:57.000000 phase_dev-1.0.0/src/phase/phase.py
+drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-02 10:03:31.983133 phase_dev-1.0.0/src/phase/utils/
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)        0 2023-06-01 07:28:57.000000 phase_dev-1.0.0/src/phase/utils/__init__.py
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)     4728 2023-06-01 07:28:57.000000 phase_dev-1.0.0/src/phase/utils/crypto.py
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)       44 2023-06-02 09:41:46.000000 phase_dev-1.0.0/src/phase/version.py
+drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-02 10:03:31.983133 phase_dev-1.0.0/src/phase_dev.egg-info/
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)      913 2023-06-02 10:03:31.000000 phase_dev-1.0.0/src/phase_dev.egg-info/PKG-INFO
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)      395 2023-06-02 10:03:31.000000 phase_dev-1.0.0/src/phase_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)        1 2023-06-02 10:03:31.000000 phase_dev-1.0.0/src/phase_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)       55 2023-06-02 10:03:31.000000 phase_dev-1.0.0/src/phase_dev.egg-info/requires.txt
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)        6 2023-06-02 10:03:31.000000 phase_dev-1.0.0/src/phase_dev.egg-info/top_level.txt
+drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-02 10:03:31.984133 phase_dev-1.0.0/tests/
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1504 2023-06-01 07:28:57.000000 phase_dev-1.0.0/tests/test_decrypt.py
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1378 2023-05-28 08:54:34.000000 phase_dev-1.0.0/tests/test_encrypt.py
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1103 2023-06-01 07:28:57.000000 phase_dev-1.0.0/tests/test_init.py
```

### Comparing `phase_dev-0.0.3/LICENSE` & `phase_dev-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phase_dev-0.0.3/PKG-INFO` & `phase_dev-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phase_dev
-Version: 0.0.3
+Version: 1.0.0
 Summary: Python SDK for Phase
 Author-email: Phase <rohan@phase.dev>
 Project-URL: Homepage, https://phase.dev
 Project-URL: Documentation, https://docs.phase.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 
 # Python SDK for Phase
 
 SDK to integrate Phase in server-side applications running Python
 
 ## Install
 
-`pip install phase-sdk`
+`pip install phase-dev`
 
 ## Import
 
 ```python
 from phase import Phase;
 ```
```

### Comparing `phase_dev-0.0.3/pyproject.toml` & `phase_dev-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phase_dev"
-version = "0.0.3"
+version = "1.0.0"
 description = "Python SDK for Phase"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `phase_dev-0.0.3/src/phase/phase.py` & `phase_dev-1.0.0/src/phase/phase.py`

 * *Files identical despite different names*

### Comparing `phase_dev-0.0.3/src/phase/utils/crypto.py` & `phase_dev-1.0.0/src/phase/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `phase_dev-0.0.3/src/phase_dev.egg-info/PKG-INFO` & `phase_dev-1.0.0/src/phase_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phase-dev
-Version: 0.0.3
+Version: 1.0.0
 Summary: Python SDK for Phase
 Author-email: Phase <rohan@phase.dev>
 Project-URL: Homepage, https://phase.dev
 Project-URL: Documentation, https://docs.phase.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 
 # Python SDK for Phase
 
 SDK to integrate Phase in server-side applications running Python
 
 ## Install
 
-`pip install phase-sdk`
+`pip install phase-dev`
 
 ## Import
 
 ```python
 from phase import Phase;
 ```
```

### Comparing `phase_dev-0.0.3/tests/test_decrypt.py` & `phase_dev-1.0.0/tests/test_decrypt.py`

 * *Files identical despite different names*

### Comparing `phase_dev-0.0.3/tests/test_encrypt.py` & `phase_dev-1.0.0/tests/test_encrypt.py`

 * *Files identical despite different names*

### Comparing `phase_dev-0.0.3/tests/test_init.py` & `phase_dev-1.0.0/tests/test_init.py`

 * *Files identical despite different names*

