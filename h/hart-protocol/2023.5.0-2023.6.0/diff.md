# Comparing `tmp/hart_protocol-2023.5.0.tar.gz` & `tmp/hart_protocol-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hart_protocol-2023.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hart_protocol-2023.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hart_protocol-2023.5.0.tar` & `hart_protocol-2023.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      429 2023-05-18 21:03:57.831139 hart_protocol-2023.5.0/.github/workflows/python-mypy.yml
--rw-r--r--   0        0        0      793 2023-05-18 21:03:57.831139 hart_protocol-2023.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      447 2023-05-18 21:03:57.831139 hart_protocol-2023.5.0/.gitignore
--rw-r--r--   0        0        0      649 2023-05-18 21:03:57.831139 hart_protocol-2023.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1305 2023-05-18 21:03:57.831139 hart_protocol-2023.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1100 2023-05-18 21:03:57.831139 hart_protocol-2023.5.0/LICENSE
--rw-r--r--   0        0        0     8501 2023-05-18 21:03:57.831139 hart_protocol-2023.5.0/README.md
--rw-r--r--   0        0        0        9 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/VERSION
--rw-r--r--   0        0        0      212 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/__init__.py
--rw-r--r--   0        0        0      493 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/__version__.py
--rw-r--r--   0        0        0     7840 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/_parsing.py
--rw-r--r--   0        0        0     4087 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/_unpacker.py
--rw-r--r--   0        0        0     1348 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/common.py
--rw-r--r--   0        0        0        0 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/py.typed
--rw-r--r--   0        0        0     1576 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/tools.py
--rw-r--r--   0        0        0     2205 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/universal.py
--rw-r--r--   0        0        0     1220 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/pyproject.toml
--rw-r--r--   0        0        0     9558 1970-01-01 00:00:00.000000 hart_protocol-2023.5.0/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/.github/workflows/python-mypy.yml
+-rw-r--r--   0        0        0      793 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      447 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/.gitignore
+-rw-r--r--   0        0        0      649 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1405 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1100 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/LICENSE
+-rw-r--r--   0        0        0     8501 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/README.md
+-rw-r--r--   0        0        0       25 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/hart_protocol/VERSION.py
+-rw-r--r--   0        0        0      212 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/hart_protocol/__init__.py
+-rw-r--r--   0        0        0      425 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/hart_protocol/__version__.py
+-rw-r--r--   0        0        0     7840 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/hart_protocol/_parsing.py
+-rw-r--r--   0        0        0     4087 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/hart_protocol/_unpacker.py
+-rw-r--r--   0        0        0     1348 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/hart_protocol/common.py
+-rw-r--r--   0        0        0        0 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/hart_protocol/py.typed
+-rw-r--r--   0        0        0     1576 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/hart_protocol/tools.py
+-rw-r--r--   0        0        0     2205 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/hart_protocol/universal.py
+-rw-r--r--   0        0        0     1274 2023-06-02 20:02:46.391642 hart_protocol-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0     9617 1970-01-01 00:00:00.000000 hart_protocol-2023.6.0/PKG-INFO
```

### Comparing `hart_protocol-2023.5.0/.github/workflows/python-publish.yml` & `hart_protocol-2023.6.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hart_protocol-2023.5.0/.pre-commit-config.yaml` & `hart_protocol-2023.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hart_protocol-2023.5.0/CHANGELOG.md` & `hart_protocol-2023.6.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/).
 
 ## [Unreleased]
 
+## [2023.6.0
+
+### Fixed
+- VERSION is now a python file so that it can be recognized by pyinstaller
+
 ## [2023.5.0]
 
 ### Fixed
 - missing final byte from message 16
 
 ## [2023.4.0]
```

### Comparing `hart_protocol-2023.5.0/LICENSE` & `hart_protocol-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hart_protocol-2023.5.0/README.md` & `hart_protocol-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `hart_protocol-2023.5.0/hart_protocol/_parsing.py` & `hart_protocol-2023.6.0/hart_protocol/_parsing.py`

 * *Files identical despite different names*

### Comparing `hart_protocol-2023.5.0/hart_protocol/_unpacker.py` & `hart_protocol-2023.6.0/hart_protocol/_unpacker.py`

 * *Files identical despite different names*

### Comparing `hart_protocol-2023.5.0/hart_protocol/common.py` & `hart_protocol-2023.6.0/hart_protocol/common.py`

 * *Files identical despite different names*

### Comparing `hart_protocol-2023.5.0/hart_protocol/tools.py` & `hart_protocol-2023.6.0/hart_protocol/tools.py`

 * *Files identical despite different names*

### Comparing `hart_protocol-2023.5.0/hart_protocol/universal.py` & `hart_protocol-2023.6.0/hart_protocol/universal.py`

 * *Files identical despite different names*

### Comparing `hart_protocol-2023.5.0/pyproject.toml` & `hart_protocol-2023.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 dist-name = "hart-protocol"
 author = "Blaise Thompson"
 home-page = "https://github.com/yaq-project/hart-protocol"
 description-file = "README.md"
 requires-python = ">=3.7"
 requires = []
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 
 [tool.flit.metadata.urls]
 Source = "https://github.com/yaq-project/hart-protocol"
 Issues = "https://github.com/yaq-project/hart-protocol/issues"
```

### Comparing `hart_protocol-2023.5.0/PKG-INFO` & `hart_protocol-2023.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: hart-protocol
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: A sans-io python implementation of the Highway Addressable Remote Transducer Protocol.
 Home-page: https://github.com/yaq-project/hart-protocol
 Author: Blaise Thompson
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Project-URL: Issues, https://github.com/yaq-project/hart-protocol/issues
 Project-URL: Source, https://github.com/yaq-project/hart-protocol
 Provides-Extra: dev
```

