# Comparing `tmp/vonage_jwt-0.0.1.tar.gz` & `tmp/vonage_jwt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage_jwt-0.0.1.tar", last modified: Fri Jun  2 15:13:28 2023, max compression
+gzip compressed data, was "vonage_jwt-1.0.0.tar", last modified: Fri Jun  2 19:18:42 2023, max compression
```

## Comparing `vonage_jwt-0.0.1.tar` & `vonage_jwt-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-02 15:13:28.828937 vonage_jwt-0.0.1/
--rw-r--r--   0 mkahan     (503) staff       (20)    11357 2023-06-02 02:36:35.000000 vonage_jwt-0.0.1/LICENSE
--rw-r--r--   0 mkahan     (503) staff       (20)     1864 2023-06-02 15:13:28.828643 vonage_jwt-0.0.1/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     1033 2023-06-02 11:52:51.000000 vonage_jwt-0.0.1/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      927 2023-06-02 15:13:18.000000 vonage_jwt-0.0.1/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2023-06-02 15:13:28.829061 vonage_jwt-0.0.1/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-02 15:13:28.822824 vonage_jwt-0.0.1/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-02 15:13:28.825019 vonage_jwt-0.0.1/src/vonage_jwt/
--rw-r--r--   0 mkahan     (503) staff       (20)        0 2023-06-02 11:52:51.000000 vonage_jwt-0.0.1/src/vonage_jwt/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1971 2023-06-02 11:52:51.000000 vonage_jwt-0.0.1/src/vonage_jwt/jwt.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-02 15:13:28.827678 vonage_jwt-0.0.1/src/vonage_jwt.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     1864 2023-06-02 15:13:28.000000 vonage_jwt-0.0.1/src/vonage_jwt.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      298 2023-06-02 15:13:28.000000 vonage_jwt-0.0.1/src/vonage_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2023-06-02 15:13:28.000000 vonage_jwt-0.0.1/src/vonage_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       21 2023-06-02 15:13:28.000000 vonage_jwt-0.0.1/src/vonage_jwt.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       11 2023-06-02 15:13:28.000000 vonage_jwt-0.0.1/src/vonage_jwt.egg-info/top_level.txt
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-02 15:13:28.828136 vonage_jwt-0.0.1/tests/
--rw-r--r--   0 mkahan     (503) staff       (20)     2334 2023-06-02 11:52:51.000000 vonage_jwt-0.0.1/tests/test_jwt_generator.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-02 19:18:42.550007 vonage_jwt-1.0.0/
+-rw-r--r--   0 mkahan     (503) staff       (20)    11357 2023-06-02 02:36:35.000000 vonage_jwt-1.0.0/LICENSE
+-rw-r--r--   0 mkahan     (503) staff       (20)     2340 2023-06-02 19:18:42.549664 vonage_jwt-1.0.0/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     1509 2023-06-02 15:20:28.000000 vonage_jwt-1.0.0/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      927 2023-06-02 15:20:34.000000 vonage_jwt-1.0.0/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2023-06-02 19:18:42.550061 vonage_jwt-1.0.0/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-02 19:18:42.542647 vonage_jwt-1.0.0/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-02 19:18:42.545426 vonage_jwt-1.0.0/src/vonage_jwt/
+-rw-r--r--   0 mkahan     (503) staff       (20)        0 2023-06-02 11:52:51.000000 vonage_jwt-1.0.0/src/vonage_jwt/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1971 2023-06-02 11:52:51.000000 vonage_jwt-1.0.0/src/vonage_jwt/jwt.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-02 19:18:42.548075 vonage_jwt-1.0.0/src/vonage_jwt.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2340 2023-06-02 19:18:42.000000 vonage_jwt-1.0.0/src/vonage_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      298 2023-06-02 19:18:42.000000 vonage_jwt-1.0.0/src/vonage_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2023-06-02 19:18:42.000000 vonage_jwt-1.0.0/src/vonage_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       21 2023-06-02 19:18:42.000000 vonage_jwt-1.0.0/src/vonage_jwt.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       11 2023-06-02 19:18:42.000000 vonage_jwt-1.0.0/src/vonage_jwt.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-02 19:18:42.549075 vonage_jwt-1.0.0/tests/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2334 2023-06-02 18:43:29.000000 vonage_jwt-1.0.0/tests/test_jwt_generator.py
```

### Comparing `vonage_jwt-0.0.1/LICENSE` & `vonage_jwt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vonage_jwt-0.0.1/PKG-INFO` & `vonage_jwt-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vonage_jwt
-Version: 0.0.1
+Version: 1.0.0
 Summary: A JWT Generator for Python. Creates JWTs for use with Vonage APIs.
 Author-email: Vonage Developer Relations <devrel@vonage.com>
 Project-URL: Homepage, https://github.com/Vonage/vonage-python-jwt
 Project-URL: Bug Tracker, https://github.com/Vonage/vonage-python-jwt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,14 +15,19 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vonage JWT Generator for Python
 
+[![PyPI version](https://badge.fury.io/py/vonage-jwt.svg)](https://badge.fury.io/py/vonage-jwt)
+[![Build Status](https://github.com/Vonage/vonage-python-jwt/workflows/Build/badge.svg)](https://github.com/Vonage/vonage-python-jwt/actions)
+[![Python versions supported](https://img.shields.io/pypi/pyversions/vonage-jwt)](https://pypi.python.org/pypi/vonage-jwt)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+
 This package provides functionality to generate a JWT in Python code.
 
 It is used by the [Vonage Python SDK](https://github.com/Vonage/vonage-python-sdk).
 
 ## Installation
 
 Install from the Python Package Index with pip:
```

### Comparing `vonage_jwt-0.0.1/README.md` & `vonage_jwt-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Vonage JWT Generator for Python
 
+[![PyPI version](https://badge.fury.io/py/vonage-jwt.svg)](https://badge.fury.io/py/vonage-jwt)
+[![Build Status](https://github.com/Vonage/vonage-python-jwt/workflows/Build/badge.svg)](https://github.com/Vonage/vonage-python-jwt/actions)
+[![Python versions supported](https://img.shields.io/pypi/pyversions/vonage-jwt)](https://pypi.python.org/pypi/vonage-jwt)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+
 This package provides functionality to generate a JWT in Python code.
 
 It is used by the [Vonage Python SDK](https://github.com/Vonage/vonage-python-sdk).
 
 ## Installation
 
 Install from the Python Package Index with pip:
```

### Comparing `vonage_jwt-0.0.1/pyproject.toml` & `vonage_jwt-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vonage_jwt"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
   { name="Vonage Developer Relations", email="devrel@vonage.com" },
 ]
 description = "A JWT Generator for Python. Creates JWTs for use with Vonage APIs."
 readme = "README.md"
 dependencies = [
     "pyjwt[crypto] >=1.6.4"
```

### Comparing `vonage_jwt-0.0.1/src/vonage_jwt/jwt.py` & `vonage_jwt-1.0.0/src/vonage_jwt/jwt.py`

 * *Files identical despite different names*

### Comparing `vonage_jwt-0.0.1/src/vonage_jwt.egg-info/PKG-INFO` & `vonage_jwt-1.0.0/src/vonage_jwt.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vonage-jwt
-Version: 0.0.1
+Version: 1.0.0
 Summary: A JWT Generator for Python. Creates JWTs for use with Vonage APIs.
 Author-email: Vonage Developer Relations <devrel@vonage.com>
 Project-URL: Homepage, https://github.com/Vonage/vonage-python-jwt
 Project-URL: Bug Tracker, https://github.com/Vonage/vonage-python-jwt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,14 +15,19 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vonage JWT Generator for Python
 
+[![PyPI version](https://badge.fury.io/py/vonage-jwt.svg)](https://badge.fury.io/py/vonage-jwt)
+[![Build Status](https://github.com/Vonage/vonage-python-jwt/workflows/Build/badge.svg)](https://github.com/Vonage/vonage-python-jwt/actions)
+[![Python versions supported](https://img.shields.io/pypi/pyversions/vonage-jwt)](https://pypi.python.org/pypi/vonage-jwt)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+
 This package provides functionality to generate a JWT in Python code.
 
 It is used by the [Vonage Python SDK](https://github.com/Vonage/vonage-python-sdk).
 
 ## Installation
 
 Install from the Python Package Index with pip:
```

### Comparing `vonage_jwt-0.0.1/tests/test_jwt_generator.py` & `vonage_jwt-1.0.0/tests/test_jwt_generator.py`

 * *Files identical despite different names*

