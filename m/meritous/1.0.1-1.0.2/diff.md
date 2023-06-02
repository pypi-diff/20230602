# Comparing `tmp/meritous-1.0.1.tar.gz` & `tmp/meritous-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meritous-1.0.1.tar", last modified: Wed May 31 18:44:52 2023, max compression
+gzip compressed data, was "meritous-1.0.2.tar", last modified: Fri Jun  2 07:11:29 2023, max compression
```

## Comparing `meritous-1.0.1.tar` & `meritous-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,23 @@
--rw-r--r--   0        0        0      104 2023-05-31 06:55:37.038633 meritous-1.0.1/.codeclimate.yml
--rw-r--r--   0        0        0     3078 2023-03-04 08:09:15.684878 meritous-1.0.1/.gitignore
--rw-r--r--   0        0        0       13 2023-02-23 13:38:24.154245 meritous-1.0.1/.python-version
--rw-r--r--   0        0        0     1077 2023-03-04 08:01:19.863201 meritous-1.0.1/LICENSE
--rw-r--r--   0        0        0     1436 2023-05-31 18:40:49.536304 meritous-1.0.1/README.md
--rw-r--r--   0        0        0      173 2023-05-20 06:32:12.910513 meritous-1.0.1/noxfile.py
--rw-r--r--   0        0        0      716 2023-05-31 18:43:40.116557 meritous-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      525 2023-05-31 12:52:46.246777 meritous-1.0.1/samples/event.py
--rw-r--r--   0        0        0       92 2023-05-31 18:44:49.544654 meritous-1.0.1/src/meritous/__init__.py
--rw-r--r--   0        0        0     2705 2023-05-31 12:57:42.703498 meritous-1.0.1/src/meritous/core.py
--rw-r--r--   0        0        0      136 2023-05-31 07:11:11.756535 meritous-1.0.1/src/meritous/exceptions.py
--rw-r--r--   0        0        0      730 2023-05-31 12:52:30.814741 meritous-1.0.1/src/meritous/properties.py
--rw-r--r--   0        0        0       77 2023-05-21 08:42:46.724083 meritous-1.0.1/tests/meritous/test_data.py
--rw-r--r--   0        0        0      951 2023-05-31 14:00:10.046757 meritous-1.0.1/tests/meritous/test_model.py
--rw-r--r--   0        0        0      937 2023-05-31 12:55:36.751189 meritous-1.0.1/tests/meritous/test_property.py
--rw-r--r--   0        0        0      414 2023-05-31 13:58:51.550756 meritous-1.0.1/tests/meritous/test_schema.py
--rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 meritous-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      104 2023-05-31 06:55:37.038633 meritous-1.0.2/.codeclimate.yml
+-rw-r--r--   0        0        0     3078 2023-03-04 08:09:15.684878 meritous-1.0.2/.gitignore
+-rw-r--r--   0        0        0       13 2023-02-23 13:38:24.154245 meritous-1.0.2/.python-version
+-rw-r--r--   0        0        0     1077 2023-03-04 08:01:19.863201 meritous-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1703 2023-05-31 18:51:16.493149 meritous-1.0.2/README.md
+-rw-r--r--   0        0        0      634 2023-06-02 05:33:09.164663 meritous-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0     1033 2023-06-02 07:09:12.763159 meritous-1.0.2/docs/concepts.rst
+-rw-r--r--   0        0        0     1225 2023-06-02 05:49:41.373722 meritous-1.0.2/docs/conf.py
+-rw-r--r--   0        0        0      796 2023-06-02 06:50:30.751928 meritous-1.0.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-06-02 05:33:09.164663 meritous-1.0.2/docs/make.bat
+-rw-r--r--   0        0        0     1414 2023-06-02 06:53:50.484079 meritous-1.0.2/docs/start.rst
+-rw-r--r--   0        0        0      173 2023-05-20 06:32:12.910513 meritous-1.0.2/noxfile.py
+-rw-r--r--   0        0        0     1036 2023-06-02 07:06:55.169932 meritous-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      525 2023-05-31 12:52:46.246777 meritous-1.0.2/samples/event.py
+-rw-r--r--   0        0        0       92 2023-06-02 07:10:21.579689 meritous-1.0.2/src/meritous/__init__.py
+-rw-r--r--   0        0        0     5125 2023-06-02 07:03:52.144530 meritous-1.0.2/src/meritous/core.py
+-rw-r--r--   0        0        0      136 2023-05-31 07:11:11.756535 meritous-1.0.2/src/meritous/exceptions.py
+-rw-r--r--   0        0        0      836 2023-05-31 21:14:32.137146 meritous-1.0.2/src/meritous/properties.py
+-rw-r--r--   0        0        0       77 2023-05-21 08:42:46.724083 meritous-1.0.2/tests/meritous/test_data.py
+-rw-r--r--   0        0        0      951 2023-05-31 14:00:10.046757 meritous-1.0.2/tests/meritous/test_model.py
+-rw-r--r--   0        0        0      937 2023-05-31 12:55:36.751189 meritous-1.0.2/tests/meritous/test_property.py
+-rw-r--r--   0        0        0      414 2023-05-31 13:58:51.550756 meritous-1.0.2/tests/meritous/test_schema.py
+-rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 meritous-1.0.2/PKG-INFO
```

### Comparing `meritous-1.0.1/.gitignore` & `meritous-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `meritous-1.0.1/LICENSE` & `meritous-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meritous-1.0.1/README.md` & `meritous-1.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,32 @@
-![PyPI](https://img.shields.io/pypi/v/meritous?style=for-the-badge)
+[![PyPI](https://img.shields.io/pypi/v/meritous?style=for-the-badge)](https://pypi.org/project/meritous/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/meritous?style=for-the-badge)
 ![PyPI - License](https://img.shields.io/pypi/l/meritous?style=for-the-badge)
-![Codecov](https://img.shields.io/codecov/c/github/errant/meritous?style=for-the-badge)
-![Code Climate maintainability](https://img.shields.io/codeclimate/maintainability/errant/meritous?style=for-the-badge)
+[![Codecov](https://img.shields.io/codecov/c/github/errant/meritous?style=for-the-badge)](https://app.codecov.io/github/errant/meritous)
+[![Code Climate maintainability](https://img.shields.io/codeclimate/maintainability/errant/meritous?style=for-the-badge)](https://codeclimate.com/github/errant/meritous)
 
 # Meritous
 
 
 Meritous is an absurdly simply approach to "Models" in Python.
 
 It came about because there is no modern, framework agnostic approach to modelling data.
 
 On the face of it the usage is very trivial; but the intent is that Meritous is a building block for more complex data models. Essentially, it provides a simple Model class which can contain data to be used in Python applications. It then sets out a standard practice for transforming that data for storage or transport.
 
+- [Documentation](https://meritous.readthedocs.io/en/latest/)
+
+## Installation
+
+```bash
+pip install meritous
+```
+
+## Basic Usage
+
 ```python
 from meritous import Model
 from meritous.properties import UUIDProperty, StrProperty, DateProperty
 
 from datetime import date
 
 class EventModel(Model):
```

### Comparing `meritous-1.0.1/samples/event.py` & `meritous-1.0.2/samples/event.py`

 * *Files identical despite different names*

### Comparing `meritous-1.0.1/src/meritous/properties.py` & `meritous-1.0.2/src/meritous/properties.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,7 +27,13 @@
         return True
 
 
 class DateProperty(Property):
 
     def __init__(self, **kwargs):
         super().__init__(datetime.date, **kwargs)
+
+
+class IntProperty(Property):
+
+    def __init__(self, **kwargs):
+        super().__init__(int, **kwargs)
```

### Comparing `meritous-1.0.1/tests/meritous/test_model.py` & `meritous-1.0.2/tests/meritous/test_model.py`

 * *Files identical despite different names*

### Comparing `meritous-1.0.1/tests/meritous/test_property.py` & `meritous-1.0.2/tests/meritous/test_property.py`

 * *Files identical despite different names*

