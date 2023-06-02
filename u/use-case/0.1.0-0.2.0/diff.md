# Comparing `tmp/use_case-0.1.0.tar.gz` & `tmp/use_case-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "use_case-0.1.0.tar", max compression
+gzip compressed data, was "use_case-0.2.0.tar", max compression
```

## Comparing `use_case-0.1.0.tar` & `use_case-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      312 2023-06-02 07:25:22.912670 use_case-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      803 2023-06-02 10:59:11.659345 use_case-0.1.0/README.md
--rw-r--r--   0        0        0     1387 2023-06-02 10:56:50.488811 use_case-0.1.0/use_case/.ipynb_checkpoints/Visualization-checkpoint.ipynb
--rw-r--r--   0        0        0        0 2023-06-02 11:00:22.931748 use_case-0.1.0/use_case/__init__.py
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 use_case-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      312 2023-06-02 11:23:01.743162 use_case-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1130 2023-06-02 11:15:16.078469 use_case-0.2.0/README.md
+-rw-r--r--   0        0        0     1387 2023-06-02 10:56:50.488811 use_case-0.2.0/use_case/.ipynb_checkpoints/Visualization-checkpoint.ipynb
+-rw-r--r--   0        0        0        0 2023-06-02 11:00:22.931748 use_case-0.2.0/use_case/__init__.py
+-rw-r--r--   0        0        0     1381 2023-06-02 11:07:44.039041 use_case-0.2.0/use_case/Visualization.ipynb
+-rw-r--r--   0        0        0     1410 1970-01-01 00:00:00.000000 use_case-0.2.0/PKG-INFO
```

### Comparing `use_case-0.1.0/use_case/.ipynb_checkpoints/Visualization-checkpoint.ipynb` & `use_case-0.2.0/use_case/.ipynb_checkpoints/Visualization-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `use_case-0.1.0/PKG-INFO` & `use_case-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: use-case
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -17,16 +17,28 @@
 1. Anaconda environment
 2. Install poetry
    1. $conda install -c conda-forge poetry
 3. Create project using poetry
    1. $poetry new use_case
 4. Add the required libraries
    1. $poetry add LIBRARY
-5. Publish the project
-6. Install the created libraries
+5. Test the library
+   1. Install Pytest
+      1. pip install pytest
+   2. Run the tests: 
+      1. $pytest -v .\tests\tests.py
+
+### Publish library 
+1. Build the project
+   1. poetry build
+2. Publish the project
+   1. poetry publish
+3. Install the created libraries (public access by default)
+   1. $pip install use-case
+   2. It will make only accessible the libraries
 
 
 # Main features: 
 
 * PEP 8 --> Style Guide
   * PyCharm native 
   * VSCode using Pylint (lastest python version supported 3.7)
```

