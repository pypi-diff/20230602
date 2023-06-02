# Comparing `tmp/tldraw-0.0.3.tar.gz` & `tmp/tldraw-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldraw-0.0.3.tar", max compression
+gzip compressed data, was "tldraw-0.1.0.tar", max compression
```

## Comparing `tldraw-0.0.3.tar` & `tldraw-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-04-24 08:16:11.663668 tldraw-0.0.3/LICENSE
--rw-r--r--   0        0        0      843 2023-05-21 17:45:54.523183 tldraw-0.0.3/README.md
--rw-r--r--   0        0        0      571 2023-05-21 17:45:42.579934 tldraw-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      165 2023-05-15 18:16:19.953893 tldraw-0.0.3/tldraw/__init__.py
--rw-r--r--   0        0        0      320 2023-05-15 18:18:52.187379 tldraw-0.0.3/tldraw/comp.tsx
--rw-r--r--   0        0        0      245 2023-05-20 16:51:27.378161 tldraw-0.0.3/tldraw/tldraw.py
--rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 tldraw-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-24 08:16:11.663668 tldraw-0.1.0/LICENSE
+-rw-r--r--   0        0        0      879 2023-06-02 20:48:23.730846 tldraw-0.1.0/README.md
+-rw-r--r--   0        0        0      571 2023-06-02 20:43:23.128962 tldraw-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      212 2023-06-02 20:40:28.237924 tldraw-0.1.0/tldraw/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-15 18:18:52.187379 tldraw-0.1.0/tldraw/comp.tsx
+-rw-r--r--   0        0        0      245 2023-05-20 16:51:27.378161 tldraw-0.1.0/tldraw/tldraw.py
+-rw-r--r--   0        0        0     2006 2023-06-02 20:48:24.934888 tldraw-0.1.0/tldraw/tldraw_matplotlib.py
+-rw-r--r--   0        0        0     1183 2023-06-02 14:17:44.885169 tldraw-0.1.0/tldraw/tldraw_matplotlib_component.tsx
+-rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 tldraw-0.1.0/PKG-INFO
```

### Comparing `tldraw-0.0.3/LICENSE` & `tldraw-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tldraw-0.0.3/README.md` & `tldraw-0.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 jupyterlab   (or alternative VS Code Jupyter Lab)
 ```
 
 
 
 # Changelog
 
+## 0.1.0
+
+* Added TldrawMatplotlib
+
 ## 0.0.3
 
 * refactor readme
 * add jupyterlite demo
 ## 0.0.2
 
 * refactor code
```

### Comparing `tldraw-0.0.3/pyproject.toml` & `tldraw-0.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tldraw"
-version = "0.0.3"
+version = "0.1.0"
 description = "Tldraw fo Jupyter"
 authors = ["kolibril13 <44469195+kolibril13@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.14"
```

### Comparing `tldraw-0.0.3/PKG-INFO` & `tldraw-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldraw
-Version: 0.0.3
+Version: 0.1.0
 Summary: Tldraw fo Jupyter
 License: MIT
 Author: kolibril13
 Author-email: 44469195+kolibril13@users.noreply.github.com
 Requires-Python: >=3.8,<3.14
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -40,14 +40,18 @@
 jupyterlab   (or alternative VS Code Jupyter Lab)
 ```
 
 
 
 # Changelog
 
+## 0.1.0
+
+* Added TldrawMatplotlib
+
 ## 0.0.3
 
 * refactor readme
 * add jupyterlite demo
 ## 0.0.2
 
 * refactor code
```

