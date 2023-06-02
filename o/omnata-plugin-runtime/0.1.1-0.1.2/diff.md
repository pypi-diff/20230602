# Comparing `tmp/omnata_plugin_runtime-0.1.1.tar.gz` & `tmp/omnata_plugin_runtime-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_plugin_runtime-0.1.1.tar", max compression
+gzip compressed data, was "omnata_plugin_runtime-0.1.2.tar", max compression
```

## Comparing `omnata_plugin_runtime-0.1.1.tar` & `omnata_plugin_runtime-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    26526 2023-06-01 22:20:56.690904 omnata_plugin_runtime-0.1.1/LICENSE
--rw-r--r--   0        0        0      296 2023-06-01 22:20:56.690904 omnata_plugin_runtime-0.1.1/README.md
--rw-r--r--   0        0        0      939 2023-06-01 22:20:56.690904 omnata_plugin_runtime-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1213 2023-06-01 22:20:56.694903 omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/__init__.py
--rw-r--r--   0        0        0     3277 2023-06-01 22:20:56.694903 omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/api.py
--rw-r--r--   0        0        0    29524 2023-06-01 22:20:56.694903 omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/configuration.py
--rw-r--r--   0        0        0    12646 2023-06-01 22:20:56.694903 omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/forms.py
--rw-r--r--   0        0        0     3547 2023-06-01 22:20:56.694903 omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/logging.py
--rw-r--r--   0        0        0    64614 2023-06-01 22:20:56.694903 omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/omnata_plugin.py
--rw-r--r--   0        0        0    18222 2023-06-01 22:20:56.694903 omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/plugin_entrypoints.py
--rw-r--r--   0        0        0    10078 2023-06-01 22:20:56.694903 omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/rate_limiting.py
--rw-r--r--   0        0        0     2611 2023-06-01 22:20:56.694903 omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/record_transformer.py
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 omnata_plugin_runtime-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-02 01:57:09.992673 omnata_plugin_runtime-0.1.2/LICENSE
+-rw-r--r--   0        0        0      296 2023-06-02 01:57:09.992673 omnata_plugin_runtime-0.1.2/README.md
+-rw-r--r--   0        0        0      840 2023-06-02 01:57:09.992673 omnata_plugin_runtime-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1213 2023-06-02 01:57:09.996673 omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/__init__.py
+-rw-r--r--   0        0        0     3277 2023-06-02 01:57:09.996673 omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/api.py
+-rw-r--r--   0        0        0    29524 2023-06-02 01:57:09.996673 omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/configuration.py
+-rw-r--r--   0        0        0    12646 2023-06-02 01:57:09.996673 omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/forms.py
+-rw-r--r--   0        0        0     3547 2023-06-02 01:57:09.996673 omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/logging.py
+-rw-r--r--   0        0        0    64614 2023-06-02 01:57:09.996673 omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/omnata_plugin.py
+-rw-r--r--   0        0        0    18222 2023-06-02 01:57:09.996673 omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/plugin_entrypoints.py
+-rw-r--r--   0        0        0    10078 2023-06-02 01:57:09.996673 omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/rate_limiting.py
+-rw-r--r--   0        0        0     2611 2023-06-02 01:57:09.996673 omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/record_transformer.py
+-rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 omnata_plugin_runtime-0.1.2/PKG-INFO
```

### Comparing `omnata_plugin_runtime-0.1.1/LICENSE` & `omnata_plugin_runtime-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/__init__.py` & `omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/api.py` & `omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/api.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/configuration.py` & `omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/configuration.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/forms.py` & `omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/forms.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/logging.py` & `omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/logging.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/omnata_plugin.py` & `omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/omnata_plugin.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/plugin_entrypoints.py` & `omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/plugin_entrypoints.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/rate_limiting.py` & `omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.1/src/omnata_plugin_runtime/record_transformer.py` & `omnata_plugin_runtime-0.1.2/src/omnata_plugin_runtime/record_transformer.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.1/PKG-INFO` & `omnata_plugin_runtime-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 Metadata-Version: 2.1
 Name: omnata-plugin-runtime
-Version: 0.1.1
+Version: 0.1.2
 Summary: A development kit to assist with building, testing and publishing Omnata Plugins
 Author: James Weakley
 Author-email: james.weakley@omnata.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: markdown (>=3,<4)
+Requires-Dist: jinja2 (>=3,<4)
 Requires-Dist: pandas
-Requires-Dist: progress (>=1,<2)
 Requires-Dist: pydantic (>=1,<2)
-Requires-Dist: python-slugify (>=8,<9)
-Requires-Dist: questionary (>=1,<2)
 Requires-Dist: snowflake-cli-labs (>=0.2.9,<0.3.0)
-Requires-Dist: tabulate
-Requires-Dist: typer
-Requires-Dist: vcrpy (>=4,<5)
 Description-Content-Type: text/markdown
 
 # omnata-plugin-runtime
 Data classes, interfaces and application logic specifically used to interface with plugins.
 
 This repo is published on PyPi as omnata-plugin-runtime.
```

