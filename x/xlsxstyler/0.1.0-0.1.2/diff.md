# Comparing `tmp/xlsxstyler-0.1.0.tar.gz` & `tmp/xlsxstyler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlsxstyler-0.1.0.tar", max compression
+gzip compressed data, was "xlsxstyler-0.1.2.tar", max compression
```

## Comparing `xlsxstyler-0.1.0.tar` & `xlsxstyler-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      442 2023-06-02 08:44:50.915079 xlsxstyler-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       64 2023-06-02 08:31:04.542335 xlsxstyler-0.1.0/xlsxstyler/__init__.py
--rw-r--r--   0        0        0     9023 2023-06-02 08:29:20.799842 xlsxstyler-0.1.0/xlsxstyler/main.py
--rw-r--r--   0        0        0      700 2023-06-02 08:49:47.987306 xlsxstyler-0.1.0/setup.py
--rw-r--r--   0        0        0      511 2023-06-02 08:49:47.988304 xlsxstyler-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      459 2023-06-02 09:09:19.152044 xlsxstyler-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-06-02 09:02:54.470173 xlsxstyler-0.1.2/xlsxstyler/__init__.py
+-rw-r--r--   0        0        0     9023 2023-06-02 08:29:20.799842 xlsxstyler-0.1.2/xlsxstyler/main.py
+-rw-r--r--   0        0        0      700 2023-06-02 09:09:52.880127 xlsxstyler-0.1.2/setup.py
+-rw-r--r--   0        0        0      575 2023-06-02 09:09:52.880494 xlsxstyler-0.1.2/PKG-INFO
```

### Comparing `xlsxstyler-0.1.0/xlsxstyler/main.py` & `xlsxstyler-0.1.2/xlsxstyler/main.py`

 * *Files identical despite different names*

### Comparing `xlsxstyler-0.1.0/setup.py` & `xlsxstyler-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['openpyxl>=3.1.2,<4.0.0', 'pandas>=2.0.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'xlsxstyler',
-    'version': '0.1.0',
+    'version': '0.1.2',
     'description': 'Some rudimentary styling of excel tables and placing pictures using openpyxl',
     'long_description': None,
     'author': 'Gwang-Jin Kim',
     'author_email': 'gwang.jin.kim.phd@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

