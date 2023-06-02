# Comparing `tmp/xlsxstyler-0.1.3.tar.gz` & `tmp/xlsxstyler-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlsxstyler-0.1.3.tar", max compression
+gzip compressed data, was "xlsxstyler-0.1.4.tar", max compression
```

## Comparing `xlsxstyler-0.1.3.tar` & `xlsxstyler-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      464 2023-06-02 09:31:32.294381 xlsxstyler-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       65 2023-06-02 09:02:54.470173 xlsxstyler-0.1.3/xlsxstyler/__init__.py
--rw-r--r--   0        0        0     9087 2023-06-02 09:53:49.677729 xlsxstyler-0.1.3/xlsxstyler/main.py
--rw-r--r--   0        0        0      706 2023-06-02 09:55:01.258704 xlsxstyler-0.1.3/setup.py
--rw-r--r--   0        0        0      581 2023-06-02 09:55:01.260260 xlsxstyler-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      464 2023-06-02 09:57:07.089653 xlsxstyler-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-06-02 09:02:54.470173 xlsxstyler-0.1.4/xlsxstyler/__init__.py
+-rw-r--r--   0        0        0     9097 2023-06-02 09:56:47.435376 xlsxstyler-0.1.4/xlsxstyler/main.py
+-rw-r--r--   0        0        0      706 2023-06-02 09:57:36.318240 xlsxstyler-0.1.4/setup.py
+-rw-r--r--   0        0        0      581 2023-06-02 09:57:36.319242 xlsxstyler-0.1.4/PKG-INFO
```

### Comparing `xlsxstyler-0.1.3/xlsxstyler/main.py` & `xlsxstyler-0.1.4/xlsxstyler/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 # these classes can be re-used to place data frames or images into excel sheets
 
 import openpyxl
 import re
 import os
 import validators
-import urllib3
+import urllib
+import io
 
 
 """
 # https://www.blog.pythonlibrary.org/2021/08/11/styling-excel-cells-with-openpyxl-and-python/
 """
 
 # This class was written 90% by ChatGPT
```

### Comparing `xlsxstyler-0.1.3/setup.py` & `xlsxstyler-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['openpyxl>=3.1.2,<4.0.0', 'validators>=0.20.0,<0.21.0']
 
 setup_kwargs = {
     'name': 'xlsxstyler',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Some rudimentary styling of excel tables and placing pictures using openpyxl',
     'long_description': None,
     'author': 'Gwang-Jin Kim',
     'author_email': 'gwang.jin.kim.phd@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `xlsxstyler-0.1.3/PKG-INFO` & `xlsxstyler-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlsxstyler
-Version: 0.1.3
+Version: 0.1.4
 Summary: Some rudimentary styling of excel tables and placing pictures using openpyxl
 License: MIT
 Author: Gwang-Jin Kim
 Author-email: gwang.jin.kim.phd@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

