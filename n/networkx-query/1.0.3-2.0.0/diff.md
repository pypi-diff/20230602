# Comparing `tmp/networkx_query-1.0.3.tar.gz` & `tmp/networkx_query-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networkx_query-1.0.3.tar", max compression
+gzip compressed data, was "networkx_query-2.0.0.tar", max compression
```

## Comparing `networkx_query-1.0.3.tar` & `networkx_query-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1100 2023-05-30 22:11:56.195003 networkx_query-1.0.3/LICENSE.md
--rw-r--r--   0        0        0     8908 2023-05-30 22:11:56.195003 networkx_query-1.0.3/README.md
--rw-r--r--   0        0        0      652 2023-05-30 22:11:56.195003 networkx_query-1.0.3/networkx_query/__init__.py
--rw-r--r--   0        0        0     4722 2023-05-30 22:11:56.195003 networkx_query-1.0.3/networkx_query/definition.py
--rw-r--r--   0        0        0     5851 2023-05-30 22:11:56.195003 networkx_query-1.0.3/networkx_query/operator.py
--rw-r--r--   0        0        0     2700 2023-05-30 22:11:56.195003 networkx_query-1.0.3/networkx_query/parser.py
--rw-r--r--   0        0        0     1310 2023-05-30 22:11:56.195003 networkx_query-1.0.3/networkx_query/query.py
--rw-r--r--   0        0        0     4463 2023-05-30 22:11:56.195003 networkx_query-1.0.3/networkx_query/relationship.py
--rw-r--r--   0        0        0     2136 2023-05-30 22:11:56.195003 networkx_query-1.0.3/networkx_query/utils.py
--rw-r--r--   0        0        0     3134 2023-05-30 22:11:56.195003 networkx_query-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    10036 1970-01-01 00:00:00.000000 networkx_query-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-06-02 14:22:12.667551 networkx_query-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0     8900 2023-06-02 14:22:12.667551 networkx_query-2.0.0/README.md
+-rw-r--r--   0        0        0      652 2023-06-02 14:22:12.667551 networkx_query-2.0.0/networkx_query/__init__.py
+-rw-r--r--   0        0        0     4722 2023-06-02 14:22:12.667551 networkx_query-2.0.0/networkx_query/definition.py
+-rw-r--r--   0        0        0     5851 2023-06-02 14:22:12.667551 networkx_query-2.0.0/networkx_query/operator.py
+-rw-r--r--   0        0        0     2700 2023-06-02 14:22:12.667551 networkx_query-2.0.0/networkx_query/parser.py
+-rw-r--r--   0        0        0     1310 2023-06-02 14:22:12.667551 networkx_query-2.0.0/networkx_query/query.py
+-rw-r--r--   0        0        0     4463 2023-06-02 14:22:12.667551 networkx_query-2.0.0/networkx_query/relationship.py
+-rw-r--r--   0        0        0     2136 2023-06-02 14:22:12.667551 networkx_query-2.0.0/networkx_query/utils.py
+-rw-r--r--   0        0        0     3131 2023-06-02 14:22:12.671551 networkx_query-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10015 1970-01-01 00:00:00.000000 networkx_query-2.0.0/PKG-INFO
```

### Comparing `networkx_query-1.0.3/LICENSE.md` & `networkx_query-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.3/README.md` & `networkx_query-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # networkx-query
 
-[Coverage Status](https://img.shields.io/coveralls/geronimo-iia/networkx-query/master.svg)](https://coveralls.io/r/geronimo-iia/networkx-query)
+[![Coverage Status](https://img.shields.io/coveralls/geronimo-iia/networkx-query/master.svg)](https://coveralls.io/r/geronimo-iia/networkx-query)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/fe669a02b4aa46b5b1faf619ba2bf382)](https://www.codacy.com/app/geronimo-iia/networkx-query?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=geronimo-iia/networkx-query&amp;utm_campaign=Badge_Grade)[![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/geronimo-iia/networkx-query.svg)](https://scrutinizer-ci.com/g/geronimo-iia/networkx-query/?branch=master)
 [![PyPI Version](https://img.shields.io/pypi/v/networkx-query.svg)](https://pypi.org/project/networkx-query)
 [![PyPI License](https://img.shields.io/pypi/l/networkx-query.svg)](https://pypi.org/project/networkx-query)
 
 Versions following [Semantic Versioning](https://semver.org/)
 
 ## Overview
 
-NetworkX Query Tool (preview)
+NetworkX Query Tool
 
 See [documentation](https://geronimo-iia.github.io/networkx-query).
 
 
 ## Installation
 
 Install this library directly into an activated virtual environment:
```

### Comparing `networkx_query-1.0.3/networkx_query/__init__.py` & `networkx_query-2.0.0/networkx_query/__init__.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.3/networkx_query/definition.py` & `networkx_query-2.0.0/networkx_query/definition.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.3/networkx_query/operator.py` & `networkx_query-2.0.0/networkx_query/operator.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.3/networkx_query/parser.py` & `networkx_query-2.0.0/networkx_query/parser.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.3/networkx_query/query.py` & `networkx_query-2.0.0/networkx_query/query.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.3/networkx_query/relationship.py` & `networkx_query-2.0.0/networkx_query/relationship.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.3/networkx_query/utils.py` & `networkx_query-2.0.0/networkx_query/utils.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.3/pyproject.toml` & `networkx_query-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "networkx_query"
-version = "1.0.3"
+version = "2.0.0"
 description = "NetworkX Query Tool"
 license = "MIT"
 authors = ["Jerome Guibert <jguibert@gmail.com>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/networkx_query"
 documentation = "https://geronimo-iia.github.io/networkx-query/"
 repository = "https://github.com/geronimo-iia/networkx-query"
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.7",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
-networkx = "^2.4"
+networkx = "*"
 
 [tool.poetry.dev-dependencies]
 black = "22.3.0"             # The uncompromising code formatter.
 isort = "5.9.3"              #A Python utility / library to sort Python imports.
 ruff = "^0.0.264"
 mypy = "*"
 types-setuptools = "^67.7.0"
```

### Comparing `networkx_query-1.0.3/PKG-INFO` & `networkx_query-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networkx-query
-Version: 1.0.3
+Version: 2.0.0
 Summary: NetworkX Query Tool
 Home-page: https://pypi.org/project/networkx_query
 License: MIT
 Keywords: networkx,graph,query
 Author: Jerome Guibert
 Author-email: jguibert@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -17,31 +17,31 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: networkx (>=2.4,<3.0)
+Requires-Dist: networkx
 Project-URL: Documentation, https://geronimo-iia.github.io/networkx-query/
 Project-URL: Repository, https://github.com/geronimo-iia/networkx-query
 Description-Content-Type: text/markdown
 
 # networkx-query
 
-[Coverage Status](https://img.shields.io/coveralls/geronimo-iia/networkx-query/master.svg)](https://coveralls.io/r/geronimo-iia/networkx-query)
+[![Coverage Status](https://img.shields.io/coveralls/geronimo-iia/networkx-query/master.svg)](https://coveralls.io/r/geronimo-iia/networkx-query)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/fe669a02b4aa46b5b1faf619ba2bf382)](https://www.codacy.com/app/geronimo-iia/networkx-query?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=geronimo-iia/networkx-query&amp;utm_campaign=Badge_Grade)[![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/geronimo-iia/networkx-query.svg)](https://scrutinizer-ci.com/g/geronimo-iia/networkx-query/?branch=master)
 [![PyPI Version](https://img.shields.io/pypi/v/networkx-query.svg)](https://pypi.org/project/networkx-query)
 [![PyPI License](https://img.shields.io/pypi/l/networkx-query.svg)](https://pypi.org/project/networkx-query)
 
 Versions following [Semantic Versioning](https://semver.org/)
 
 ## Overview
 
-NetworkX Query Tool (preview)
+NetworkX Query Tool
 
 See [documentation](https://geronimo-iia.github.io/networkx-query).
 
 
 ## Installation
 
 Install this library directly into an activated virtual environment:
```

