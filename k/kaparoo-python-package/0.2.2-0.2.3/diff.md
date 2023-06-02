# Comparing `tmp/kaparoo_python_package-0.2.2.tar.gz` & `tmp/kaparoo_python_package-0.2.3.tar.gz`

## Comparing `kaparoo_python_package-0.2.2.tar` & `kaparoo_python_package-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/py.typed
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/filesystem/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/filesystem/exceptions.py
--rw-r--r--   0        0        0    23306 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/filesystem/path.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/filesystem/types.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/utils/__init__.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/utils/optional.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/kaparoo/utils/singleton.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/LICENSE
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/README.md
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/py.typed
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/filesystem/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/filesystem/exceptions.py
+-rw-r--r--   0        0        0    23306 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/filesystem/path.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/filesystem/types.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/utils/__init__.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/utils/optional.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/utils/singleton.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/utils/types.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/README.md
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/PKG-INFO
```

### Comparing `kaparoo_python_package-0.2.2/kaparoo/filesystem/__init__.py` & `kaparoo_python_package-0.2.3/kaparoo/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.2/kaparoo/filesystem/path.py` & `kaparoo_python_package-0.2.3/kaparoo/filesystem/path.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.2/kaparoo/utils/optional.py` & `kaparoo_python_package-0.2.3/kaparoo/utils/optional.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.2/kaparoo/utils/singleton.py` & `kaparoo_python_package-0.2.3/kaparoo/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.2/.gitignore` & `kaparoo_python_package-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.2/LICENSE` & `kaparoo_python_package-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.2/README.md` & `kaparoo_python_package-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.2/pyproject.toml` & `kaparoo_python_package-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.2/PKG-INFO` & `kaparoo_python_package-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaparoo-python-package
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for (personally) common and useful features.
 Project-URL: GitHub, https://www.github.com/kaparoo/python-package
 Author-email: Jaewoo Park <kaparoo2001@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jaewoo Park
```

