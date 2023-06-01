# Comparing `tmp/cc.xboxcontroller-0.1.0.tar.gz` & `tmp/cc.xboxcontroller-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc.xboxcontroller-0.1.0.tar", last modified: Thu Jun  1 22:27:53 2023, max compression
+gzip compressed data, was "cc.xboxcontroller-0.1.1.tar", last modified: Thu Jun  1 22:41:02 2023, max compression
```

## Comparing `cc.xboxcontroller-0.1.0.tar` & `cc.xboxcontroller-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 22:27:53.881653 cc.xboxcontroller-0.1.0/
--rw-rw-rw-   0        0        0     1090 2023-06-01 22:14:43.000000 cc.xboxcontroller-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1271 2023-06-01 22:27:53.880647 cc.xboxcontroller-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      746 2023-06-01 22:14:43.000000 cc.xboxcontroller-0.1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-06-01 22:14:43.000000 cc.xboxcontroller-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 22:27:53.881653 cc.xboxcontroller-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-06-01 22:26:59.000000 cc.xboxcontroller-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:27:53.839931 cc.xboxcontroller-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 22:27:53.859651 cc.xboxcontroller-0.1.0/src/cc/
--rw-rw-rw-   0        0        0       48 2023-06-01 22:14:43.000000 cc.xboxcontroller-0.1.0/src/cc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:27:53.879647 cc.xboxcontroller-0.1.0/src/cc/xboxcontroller/
--rw-rw-rw-   0        0        0       50 2023-06-01 22:14:43.000000 cc.xboxcontroller-0.1.0/src/cc/xboxcontroller/__init__.py
--rw-rw-rw-   0        0        0    14000 2023-06-01 22:26:21.000000 cc.xboxcontroller-0.1.0/src/cc/xboxcontroller/xboxcontroller.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:27:53.877648 cc.xboxcontroller-0.1.0/src/cc.xboxcontroller.egg-info/
--rw-rw-rw-   0        0        0     1271 2023-06-01 22:27:53.000000 cc.xboxcontroller-0.1.0/src/cc.xboxcontroller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-06-01 22:27:53.000000 cc.xboxcontroller-0.1.0/src/cc.xboxcontroller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 22:27:53.000000 cc.xboxcontroller-0.1.0/src/cc.xboxcontroller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-01 22:27:53.000000 cc.xboxcontroller-0.1.0/src/cc.xboxcontroller.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2023-06-01 22:27:53.000000 cc.xboxcontroller-0.1.0/src/cc.xboxcontroller.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 22:41:02.077659 cc.xboxcontroller-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-06-01 22:38:24.000000 cc.xboxcontroller-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1271 2023-06-01 22:41:02.041140 cc.xboxcontroller-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      746 2023-06-01 22:38:24.000000 cc.xboxcontroller-0.1.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-01 22:38:24.000000 cc.xboxcontroller-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 22:41:02.077659 cc.xboxcontroller-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-01 22:40:47.000000 cc.xboxcontroller-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:41:02.013167 cc.xboxcontroller-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-01 22:41:02.022156 cc.xboxcontroller-0.1.1/src/cc/
+-rw-rw-rw-   0        0        0       56 2023-06-01 22:38:42.000000 cc.xboxcontroller-0.1.1/src/cc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:41:02.040138 cc.xboxcontroller-0.1.1/src/cc/xboxcontroller/
+-rw-rw-rw-   0        0        0       58 2023-06-01 22:38:40.000000 cc.xboxcontroller-0.1.1/src/cc/xboxcontroller/__init__.py
+-rw-rw-rw-   0        0        0    14000 2023-06-01 22:38:24.000000 cc.xboxcontroller-0.1.1/src/cc/xboxcontroller/xboxcontroller.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:41:02.037140 cc.xboxcontroller-0.1.1/src/cc.xboxcontroller.egg-info/
+-rw-rw-rw-   0        0        0     1271 2023-06-01 22:41:01.000000 cc.xboxcontroller-0.1.1/src/cc.xboxcontroller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-06-01 22:41:02.000000 cc.xboxcontroller-0.1.1/src/cc.xboxcontroller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 22:41:01.000000 cc.xboxcontroller-0.1.1/src/cc.xboxcontroller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-01 22:41:01.000000 cc.xboxcontroller-0.1.1/src/cc.xboxcontroller.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2023-06-01 22:41:01.000000 cc.xboxcontroller-0.1.1/src/cc.xboxcontroller.egg-info/top_level.txt
```

### Comparing `cc.xboxcontroller-0.1.0/LICENSE` & `cc.xboxcontroller-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cc.xboxcontroller-0.1.0/PKG-INFO` & `cc.xboxcontroller-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc.xboxcontroller
-Version: 0.1.0
+Version: 0.1.1
 Summary: Getting input from Microsoft XBox 360 controllers via the XInput library on Windows.
 Home-page: https://github.com/uncertainty-cc/XboxController-Python
 Author: Uncertainty.
 Author-email: t_k_233@outlook.email
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cc.xboxcontroller-0.1.0/README.md` & `cc.xboxcontroller-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cc.xboxcontroller-0.1.0/setup.py` & `cc.xboxcontroller-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cc.xboxcontroller",
-    version="0.1.0",
+    version="0.1.1",
     author="Uncertainty.",
     author_email="t_k_233@outlook.email",
     description="Getting input from Microsoft XBox 360 controllers via the XInput library on Windows.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uncertainty-cc/XboxController-Python",
     project_urls={
```

### Comparing `cc.xboxcontroller-0.1.0/src/cc/xboxcontroller/xboxcontroller.py` & `cc.xboxcontroller-0.1.1/src/cc/xboxcontroller/xboxcontroller.py`

 * *Files identical despite different names*

### Comparing `cc.xboxcontroller-0.1.0/src/cc.xboxcontroller.egg-info/PKG-INFO` & `cc.xboxcontroller-0.1.1/src/cc.xboxcontroller.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc.xboxcontroller
-Version: 0.1.0
+Version: 0.1.1
 Summary: Getting input from Microsoft XBox 360 controllers via the XInput library on Windows.
 Home-page: https://github.com/uncertainty-cc/XboxController-Python
 Author: Uncertainty.
 Author-email: t_k_233@outlook.email
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

