# Comparing `tmp/pyGATs-0.0.5.tar.gz` & `tmp/pyGATs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGATs-0.0.5.tar", last modified: Fri Mar 10 10:10:16 2023, max compression
+gzip compressed data, was "pyGATs-0.0.6.tar", last modified: Fri Jun  2 11:50:58 2023, max compression
```

## Comparing `pyGATs-0.0.5.tar` & `pyGATs-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:10:16.952694 pyGATs-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-10 10:10:06.000000 pyGATs-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-10 10:10:16.952694 pyGATs-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-10 10:10:06.000000 pyGATs-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-10 10:10:06.000000 pyGATs-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 10:10:16.952694 pyGATs-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:10:16.952694 pyGATs-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:10:16.952694 pyGATs-0.0.5/src/pyGATs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-10 10:10:16.000000 pyGATs-0.0.5/src/pyGATs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-10 10:10:16.000000 pyGATs-0.0.5/src/pyGATs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 10:10:16.000000 pyGATs-0.0.5/src/pyGATs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-10 10:10:16.000000 pyGATs-0.0.5/src/pyGATs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-10 10:10:16.000000 pyGATs-0.0.5/src/pyGATs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:10:16.952694 pyGATs-0.0.5/src/pygats/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-10 10:10:06.000000 pyGATs-0.0.5/src/pygats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-03-10 10:10:06.000000 pyGATs-0.0.5/src/pygats/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-03-10 10:10:06.000000 pyGATs-0.0.5/src/pygats/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31664 2023-03-10 10:10:06.000000 pyGATs-0.0.5/src/pygats/pygats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:10:16.952694 pyGATs-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-10 10:10:06.000000 pyGATs-0.0.5/tests/test_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-10 10:10:06.000000 pyGATs-0.0.5/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-10 10:10:06.000000 pyGATs-0.0.5/tests/test_pygats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:50:58.540125 pyGATs-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-02 11:50:46.000000 pyGATs-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-02 11:50:58.540125 pyGATs-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-02 11:50:46.000000 pyGATs-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-02 11:50:46.000000 pyGATs-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:50:58.540125 pyGATs-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:50:58.536125 pyGATs-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:50:58.540125 pyGATs-0.0.6/src/pyGATs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-02 11:50:58.000000 pyGATs-0.0.6/src/pyGATs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-02 11:50:58.000000 pyGATs-0.0.6/src/pyGATs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:50:58.000000 pyGATs-0.0.6/src/pyGATs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-02 11:50:58.000000 pyGATs-0.0.6/src/pyGATs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 11:50:58.000000 pyGATs-0.0.6/src/pyGATs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:50:58.540125 pyGATs-0.0.6/src/pygats/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-02 11:50:46.000000 pyGATs-0.0.6/src/pygats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-02 11:50:46.000000 pyGATs-0.0.6/src/pygats/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-02 11:50:46.000000 pyGATs-0.0.6/src/pygats/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19722 2023-06-02 11:50:46.000000 pyGATs-0.0.6/src/pygats/pygats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-06-02 11:50:46.000000 pyGATs-0.0.6/src/pygats/recog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:50:58.540125 pyGATs-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-02 11:50:46.000000 pyGATs-0.0.6/tests/test_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-02 11:50:46.000000 pyGATs-0.0.6/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-02 11:50:46.000000 pyGATs-0.0.6/tests/test_pygats.py
```

### Comparing `pyGATs-0.0.5/LICENSE` & `pyGATs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.5/PKG-INFO` & `pyGATs-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGATs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automate end-to-end and exploratory testing
 Author: vsysoev
 License: MIT License
         
         Copyright (c) 2022 IntegraSDL
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyGATs-0.0.5/README.md` & `pyGATs-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.5/pyproject.toml` & `pyGATs-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyGATs"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="vsysoev" },
 ]
 description = "Automate end-to-end and exploratory testing"
 keywords = ["gui", "testing", "automatic"]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pyGATs-0.0.5/src/pyGATs.egg-info/PKG-INFO` & `pyGATs-0.0.6/src/pyGATs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGATs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automate end-to-end and exploratory testing
 Author: vsysoev
 License: MIT License
         
         Copyright (c) 2022 IntegraSDL
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyGATs-0.0.5/src/pygats/formatters.py` & `pyGATs-0.0.6/src/pygats/formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         Print Markdown header with spaces lines
 
         Args:
             level (int): Level of header. Count of # in markdown header.
             text (string): Header text
         """
         print()
-        header_level = '#'*level
+        header_level = '#' * level
         print(f'{header_level} {text}')
         print()
 
     @staticmethod
     def print_para(text):
         """
         Print Markdown paragraph
```

### Comparing `pyGATs-0.0.5/src/pygats/misc.py` & `pyGATs-0.0.6/src/pygats/misc.py`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.5/tests/test_formatters.py` & `pyGATs-0.0.6/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.5/tests/test_misc.py` & `pyGATs-0.0.6/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.5/tests/test_pygats.py` & `pyGATs-0.0.6/tests/test_pygats.py`

 * *Files identical despite different names*

