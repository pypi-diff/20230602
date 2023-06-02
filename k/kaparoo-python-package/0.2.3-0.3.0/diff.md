# Comparing `tmp/kaparoo_python_package-0.2.3.tar.gz` & `tmp/kaparoo_python_package-0.3.0.tar.gz`

## Comparing `kaparoo_python_package-0.2.3.tar` & `kaparoo_python_package-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/py.typed
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/filesystem/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/filesystem/exceptions.py
--rw-r--r--   0        0        0    23306 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/filesystem/path.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/filesystem/types.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/utils/__init__.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/utils/optional.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/utils/singleton.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/kaparoo/utils/types.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/LICENSE
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/README.md
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/kaparoo/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/kaparoo/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/kaparoo/py.typed
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/kaparoo/beartype/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/kaparoo/beartype/numerics.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/kaparoo/filesystem/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/kaparoo/filesystem/exceptions.py
+-rw-r--r--   0        0        0    23306 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/kaparoo/filesystem/path.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/kaparoo/filesystem/types.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/kaparoo/utils/__init__.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/kaparoo/utils/optional.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/kaparoo/utils/singleton.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/kaparoo/utils/types.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/README.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 kaparoo_python_package-0.3.0/PKG-INFO
```

### Comparing `kaparoo_python_package-0.2.3/kaparoo/filesystem/__init__.py` & `kaparoo_python_package-0.3.0/kaparoo/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.3/kaparoo/filesystem/path.py` & `kaparoo_python_package-0.3.0/kaparoo/filesystem/path.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.3/kaparoo/utils/optional.py` & `kaparoo_python_package-0.3.0/kaparoo/utils/optional.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.3/kaparoo/utils/singleton.py` & `kaparoo_python_package-0.3.0/kaparoo/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.3/.gitignore` & `kaparoo_python_package-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.3/LICENSE` & `kaparoo_python_package-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.3/README.md` & `kaparoo_python_package-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.3/pyproject.toml` & `kaparoo_python_package-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: CPython",
     "Typing :: Typed",
 ]
+dependencies = [
+    "beartype>=0.14.0",
+]
 
 [project.optional-dependencies]
 dev = [
     "hatch>=1.7.0",
     "ruff>=0.0.263",
     "mypy>=1.2.0",
     "black>=23.3.0",
```

### Comparing `kaparoo_python_package-0.2.3/PKG-INFO` & `kaparoo_python_package-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaparoo-python-package
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Python package for (personally) common and useful features.
 Project-URL: GitHub, https://www.github.com/kaparoo/python-package
 Author-email: Jaewoo Park <kaparoo2001@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jaewoo Park
         
@@ -33,14 +33,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
+Requires-Dist: beartype>=0.14.0
 Provides-Extra: dev
 Requires-Dist: black>=23.3.0; extra == 'dev'
 Requires-Dist: hatch>=1.7.0; extra == 'dev'
 Requires-Dist: mypy>=1.2.0; extra == 'dev'
 Requires-Dist: pytest>=7.3.1; extra == 'dev'
 Requires-Dist: ruff>=0.0.263; extra == 'dev'
 Description-Content-Type: text/markdown
```

