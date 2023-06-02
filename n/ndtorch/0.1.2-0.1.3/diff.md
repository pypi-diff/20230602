# Comparing `tmp/ndtorch-0.1.2.tar.gz` & `tmp/ndtorch-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndtorch-0.1.2.tar", last modified: Fri May 26 04:30:25 2023, max compression
+gzip compressed data, was "ndtorch-0.1.3.tar", last modified: Fri Jun  2 15:38:43 2023, max compression
```

## Comparing `ndtorch-0.1.2.tar` & `ndtorch-0.1.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.257227 ndtorch-0.1.2/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1816 2023-05-23 16:05:19.000000 ndtorch-0.1.2/.gitignore
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      152 2023-05-23 16:04:29.000000 ndtorch-0.1.2/.readthedocs.yml
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1069 2023-05-23 16:04:29.000000 ndtorch-0.1.2/LICENSE
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2627 2023-05-26 04:30:25.257227 ndtorch-0.1.2/PKG-INFO
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2142 2023-05-25 17:05:08.000000 ndtorch-0.1.2/README.MD
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.245227 ndtorch-0.1.2/docs/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      638 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/Makefile
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      804 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/make.bat
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.249227 ndtorch-0.1.2/docs/pics/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1376301 2023-05-25 16:59:32.000000 ndtorch-0.1.2/docs/pics/change.gif
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1239706 2023-05-24 09:08:54.000000 ndtorch-0.1.2/docs/pics/collision.gif
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    92012 2023-05-25 15:47:52.000000 ndtorch-0.1.2/docs/pics/logo.svg
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  2852797 2023-05-25 15:55:45.000000 ndtorch-0.1.2/docs/pics/manifold.gif
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       37 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/requirements.txt
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.253227 ndtorch-0.1.2/docs/source/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2195 2023-05-25 16:17:36.000000 ndtorch-0.1.2/docs/source/conf.py
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.253227 ndtorch-0.1.2/docs/source/examples/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1140881 2023-05-26 04:18:09.000000 ndtorch-0.1.2/docs/source/examples/ndtorch.ipynb
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      940 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/index.rst
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.253227 ndtorch-0.1.2/docs/source/modules/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       48 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/derivative.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       46 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/evaluate.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       43 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/index.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/jet.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/pfp.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/propagate.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       44 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/series.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/signature.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       42 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/util.rst
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.257227 ndtorch-0.1.2/ndtorch/
--rwxrwxr-x   0 imorozov  (1000) imorozov  (1000)     8286 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/__init__.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     6769 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/derivative.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7451 2023-05-25 16:03:14.000000 ndtorch-0.1.2/ndtorch/evaluate.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     3475 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/index.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    22741 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/jet.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    16434 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/pfp.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7699 2023-05-25 16:03:21.000000 ndtorch-0.1.2/ndtorch/propagate.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    11429 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/series.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     5563 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/signature.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2976 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/util.py
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.257227 ndtorch-0.1.2/ndtorch.egg-info/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2627 2023-05-26 04:30:25.000000 ndtorch-0.1.2/ndtorch.egg-info/PKG-INFO
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      909 2023-05-26 04:30:25.000000 ndtorch-0.1.2/ndtorch.egg-info/SOURCES.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        1 2023-05-26 04:30:25.000000 ndtorch-0.1.2/ndtorch.egg-info/dependency_links.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      135 2023-05-26 04:30:25.000000 ndtorch-0.1.2/ndtorch.egg-info/requires.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        8 2023-05-26 04:30:25.000000 ndtorch-0.1.2/ndtorch.egg-info/top_level.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1140881 2023-05-26 04:18:09.000000 ndtorch-0.1.2/ndtorch.ipynb
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      736 2023-05-26 04:27:32.000000 ndtorch-0.1.2/pyproject.toml
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       38 2023-05-26 04:30:25.257227 ndtorch-0.1.2/setup.cfg
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-02 15:38:43.036982 ndtorch-0.1.3/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1822 2023-06-01 15:51:48.000000 ndtorch-0.1.3/.gitignore
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      152 2023-05-23 16:04:29.000000 ndtorch-0.1.3/.readthedocs.yml
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1069 2023-05-23 16:04:29.000000 ndtorch-0.1.3/LICENSE
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2601 2023-06-02 15:38:43.036982 ndtorch-0.1.3/PKG-INFO
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2115 2023-06-02 07:44:11.000000 ndtorch-0.1.3/README.MD
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-02 15:38:42.984983 ndtorch-0.1.3/docs/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      638 2023-05-23 16:04:29.000000 ndtorch-0.1.3/docs/Makefile
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      804 2023-05-23 16:04:29.000000 ndtorch-0.1.3/docs/make.bat
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-02 15:38:43.008983 ndtorch-0.1.3/docs/pics/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1376301 2023-05-25 16:59:32.000000 ndtorch-0.1.3/docs/pics/change.gif
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1239706 2023-05-24 09:08:54.000000 ndtorch-0.1.3/docs/pics/collision.gif
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    92012 2023-05-25 15:47:52.000000 ndtorch-0.1.3/docs/pics/logo.svg
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  2852797 2023-05-25 15:55:45.000000 ndtorch-0.1.3/docs/pics/manifold.gif
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       37 2023-05-23 16:04:29.000000 ndtorch-0.1.3/docs/requirements.txt
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-02 15:38:43.024983 ndtorch-0.1.3/docs/source/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2195 2023-05-25 16:17:36.000000 ndtorch-0.1.3/docs/source/conf.py
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-02 15:38:43.024983 ndtorch-0.1.3/docs/source/examples/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1440373 2023-06-02 15:35:58.000000 ndtorch-0.1.3/docs/source/examples/ndtorch.ipynb
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      940 2023-05-23 16:04:29.000000 ndtorch-0.1.3/docs/source/index.rst
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-02 15:38:43.028982 ndtorch-0.1.3/docs/source/modules/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       48 2023-05-23 16:04:29.000000 ndtorch-0.1.3/docs/source/modules/derivative.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       46 2023-05-23 16:04:29.000000 ndtorch-0.1.3/docs/source/modules/evaluate.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       43 2023-05-23 16:04:29.000000 ndtorch-0.1.3/docs/source/modules/index.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2023-05-23 16:04:29.000000 ndtorch-0.1.3/docs/source/modules/jet.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2023-05-23 16:04:29.000000 ndtorch-0.1.3/docs/source/modules/pfp.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-05-23 16:04:29.000000 ndtorch-0.1.3/docs/source/modules/propagate.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       44 2023-05-23 16:04:29.000000 ndtorch-0.1.3/docs/source/modules/series.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-05-23 16:04:29.000000 ndtorch-0.1.3/docs/source/modules/signature.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       42 2023-05-23 16:04:29.000000 ndtorch-0.1.3/docs/source/modules/util.rst
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-02 15:38:43.036982 ndtorch-0.1.3/ndtorch/
+-rwxrwxr-x   0 imorozov  (1000) imorozov  (1000)     8286 2023-05-23 16:04:29.000000 ndtorch-0.1.3/ndtorch/__init__.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     6769 2023-05-23 16:04:29.000000 ndtorch-0.1.3/ndtorch/derivative.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7452 2023-05-26 16:55:36.000000 ndtorch-0.1.3/ndtorch/evaluate.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     3475 2023-05-23 16:04:29.000000 ndtorch-0.1.3/ndtorch/index.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    22741 2023-05-23 16:04:29.000000 ndtorch-0.1.3/ndtorch/jet.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    16434 2023-05-23 16:04:29.000000 ndtorch-0.1.3/ndtorch/pfp.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7699 2023-05-25 16:03:21.000000 ndtorch-0.1.3/ndtorch/propagate.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    11435 2023-05-29 12:23:39.000000 ndtorch-0.1.3/ndtorch/series.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     8352 2023-05-28 05:42:56.000000 ndtorch-0.1.3/ndtorch/signature.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2976 2023-05-23 16:04:29.000000 ndtorch-0.1.3/ndtorch/util.py
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-02 15:38:43.036982 ndtorch-0.1.3/ndtorch.egg-info/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2601 2023-06-02 15:38:42.000000 ndtorch-0.1.3/ndtorch.egg-info/PKG-INFO
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      909 2023-06-02 15:38:42.000000 ndtorch-0.1.3/ndtorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        1 2023-06-02 15:38:42.000000 ndtorch-0.1.3/ndtorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      135 2023-06-02 15:38:42.000000 ndtorch-0.1.3/ndtorch.egg-info/requires.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        8 2023-06-02 15:38:42.000000 ndtorch-0.1.3/ndtorch.egg-info/top_level.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1440373 2023-06-02 15:35:58.000000 ndtorch-0.1.3/ndtorch.ipynb
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      737 2023-06-02 15:37:37.000000 ndtorch-0.1.3/pyproject.toml
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       38 2023-06-02 15:38:43.036982 ndtorch-0.1.3/setup.cfg
```

### Comparing `ndtorch-0.1.2/.gitignore` & `ndtorch-0.1.3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Dev
+notes
 dev.ipynb
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `ndtorch-0.1.2/LICENSE` & `ndtorch-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/PKG-INFO` & `ndtorch-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ndtorch
-Version: 0.1.2
+Version: 0.1.3
 Summary: Higher order partial derivatives computation with respect to one or several tensor-like variables, application to nonlinear dynamics
 Author-email: Ivan Morozov <i.a.morozov@inp.nsk.su>
 License: MIT
 Keywords: torch,derivative
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: examples
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/ndtorch/badge/?version=latest)](https://ndtorch.readthedocs.io/en/latest/?badge=latest)
@@ -97,12 +97,10 @@
 
 <p align="center">
   <img width="576" height="576" src="docs/pics/collision.gif">
 </p>
 
 Reduce real part of a hyperbolic fixed point
 
-Collision of fixed points
-
 <p align="center">
   <img width="576" height="576" src="docs/pics/change.gif">
 </p>
```

### Comparing `ndtorch-0.1.2/README.MD` & `ndtorch-0.1.3/README.MD`

 * *Files 5% similar despite different names*

```diff
@@ -82,12 +82,10 @@
 
 <p align="center">
   <img width="576" height="576" src="docs/pics/collision.gif">
 </p>
 
 Reduce real part of a hyperbolic fixed point
 
-Collision of fixed points
-
 <p align="center">
   <img width="576" height="576" src="docs/pics/change.gif">
 </p>
```

### Comparing `ndtorch-0.1.2/docs/Makefile` & `ndtorch-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/docs/make.bat` & `ndtorch-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/docs/pics/change.gif` & `ndtorch-0.1.3/docs/pics/change.gif`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/docs/pics/collision.gif` & `ndtorch-0.1.3/docs/pics/collision.gif`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/docs/pics/logo.svg` & `ndtorch-0.1.3/docs/pics/logo.svg`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/docs/pics/manifold.gif` & `ndtorch-0.1.3/docs/pics/manifold.gif`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/docs/source/conf.py` & `ndtorch-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/docs/source/examples/ndtorch.ipynb` & `ndtorch-0.1.3/docs/source/examples/ndtorch.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9274945175438596%*

 * *Differences: {"'cells'": "{227: {'execution_count': 15, 'id': '8c172e35-8002-43ab-9d28-4c6b9610c820', 'source': "*

 * *            "['# Note, similar to tune spread example, it is possible to compute advance "*

 * *            "spread\\n', '# First order computation can be performed using error propagation\\n', "*

 * *            "'# Or higher order jets can be sampled']}, insert: [(95, OrderedDict([('cell_type', "*

 * *            "'markdown'), ('id', '7056772b-ad88-465f-ab99-5de6f5e9a464'), ('metadata', "*

 * *            "OrderedDict()), ('s […]*

```diff
@@ -3264,20 +3264,4068 @@
                 "\n",
                 "    lr += 0.005\n",
                 "    gradient = derivative(1, objective, knobs, intermediate=False)\n",
                 "    knobs = knobs - lr*gradient"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "7056772b-ad88-465f-ab99-5de6f5e9a464",
+            "metadata": {},
+            "source": [
+                "# Example-10: Alignment indices chaos indicators"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "b5b8e139-1eb3-497e-909f-c6351dd3c8c3",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "\n",
+                "torch.set_printoptions(precision=8, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "4ac5ba1c-91af-46bd-bdfb-05e0a896f110",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "a883b669-2946-4b45-8101-a2c32ab2c92d",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set fixed parameters\n",
+                "\n",
+                "a1, b1 = 0, 1\n",
+                "a2, b2 = 0, 1\n",
+                "\n",
+                "f1 = torch.tensor(2.0*numpy.pi*0.38, dtype=dtype, device=device)\n",
+                "f2 = torch.tensor(2.0*numpy.pi*0.41, dtype=dtype, device=device)\n",
+                "\n",
+                "cf1, sf1 = f1.cos(), f1.sin()\n",
+                "cf2, sf2 = f2.cos(), f2.sin()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "7e2e4e7d-76d1-4f16-9c39-640fbcb0919a",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set 4D symplectic mapping\n",
+                "\n",
+                "def mapping(x):\n",
+                "    q1, p1, q2, p2 = x\n",
+                "    return torch.stack([\n",
+                "        b1*(p1 + (q1**2 - q2**2))*sf1 + q1*(cf1 + a1*sf1),\n",
+                "        -((q1*(1 + a1**2)*sf1)/b1) + (p1 + (q1**2 - q2**2))*(cf1 - a1*sf1),\n",
+                "        q2*cf2 + (p2*b2 + q2*(a2 - 2*q1*b2))*sf2,\n",
+                "        -((q2*(1 + a2**2)*sf2)/b2) + (p2 - 2*q1*q2)*(cf2 - a2*sf2)\n",
+                "    ])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "c52b6cdc-defc-4401-9438-3ef068ddb250",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set 4D symplectic mapping with tangent dynamics\n",
+                "\n",
+                "def tangent(x, vs):\n",
+                "    x, m = derivative(1, mapping, x)\n",
+                "    vs = torch.func.vmap(lambda v: m @ v)(vs)\n",
+                "    return x, vs/vs.norm(dim=-1, keepdim=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "041045e3-e9e6-4975-a9a7-74e82bd54c43",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set generalized alignment indices computation\n",
+                "\n",
+                "# Note, if number if vectors is equal to two, the index tends towards zero for regular orbits\n",
+                "# And tends towards a constant value for chaotic motion\n",
+                "# If the number of vectors is greater than two, index tends towards zero for all cases\n",
+                "# But for chaotic orbits, zero is reached (exponentialy) faster\n",
+                "\n",
+                "def gali(vs, threshold=1.0E-12):\n",
+                "    return (threshold + torch.linalg.svdvals(vs).prod()).log10()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "f9a0791b-873c-4915-bf36-4f15096d063a",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "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\n",
+                        "text/plain": [
+                            "<Figure size 576x576 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "# First, consider two initial conditions (regular and chaotic)\n",
+                "\n",
+                "count = 1024\n",
+                "\n",
+                "plt.figure(figsize=(8, 8))\n",
+                "\n",
+                "x = torch.tensor([0.50000, 0.0, 0.05, 0.0], dtype=dtype)\n",
+                "orbit = []\n",
+                "for _ in range(count):\n",
+                "    x = mapping(x)\n",
+                "    orbit.append(x)\n",
+                "q, p, *_ = torch.stack(orbit).T\n",
+                "plt.scatter(q, p, s =1, color='blue')\n",
+                "\n",
+                "x = torch.tensor([0.68925, 0.0, 0.10, 0.0], dtype=dtype)\n",
+                "orbit = []\n",
+                "for _ in range(count):\n",
+                "    x = mapping(x)\n",
+                "    orbit.append(x)\n",
+                "q, p, *_ = torch.stack(orbit).T\n",
+                "plt.scatter(q, p, s =1, color='red')\n",
+                "\n",
+                "plt.show()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "3abcd814-9305-4e11-82a8-449c2ffae2db",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAABIYAAAEvCAYAAAAwxMqBAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8qNh9FAAAACXBIWXMAAAsTAAALEwEAmpwYAAAjoklEQVR4nO3dfZBl6V0f9u9vNNOgUSTk7V47saSexoWcRDhlIB1FFE5iA8Gy7PLa8Uug7paVbSfNSnYydtkhQFfhcspdFWzKZFL2KpkyM0HMNZjClk0FBQVhKk5SBXGvIWaFUCFj9egF0GwvKFqaqFfWkz9uj3Zmp9/vPff186k6dfuce+85T2/N3dP97d/ze6q1FgAAAAAWz6VJDwAAAACAyRAMAQAAACwowRAAAADAghIMAQAAACwowRAAAADAghIMAQAAACyoy5MewINWVlba2trapIcBAAAAMDeeffbZ51trjx/13FQFQ2tra9nZ2Zn0MAAAAADmRlXtHvdc51PJqurtVfWRqvpoVX1719cDAAAA4Gw6DYaq6lVJ/naSP5TkLUm+pare0uU1AQAAADibriuG3prko621X26tHST5oSRPdHxNAAAAAM6g62DoDUk+/sD+Jw6PAQAAADBhE1+uvqo2q2qnqnbu3bs36eEAAAAALIyug6FPJnnTA/tvPDz2Ra21m6219dba+uOPH7lyGgAAAAAd6DoY+qdJ3lxVX15VS0m+OcmPdnxNAAAAAM6g02Cotfb5JH8+yQeSfDjJD7fWPtTlNSet309WVpKqwbayMjgGAAAAMG0ud32B1tr7k7y/6+tMg34/eeqp5KWXXj62t5dsbAy+7vUmMy4AAACAo0y8+fQ82dp6OBS67+Bg8BwAAADANBEMjdDduxd7DgAAAGASBEMjtLqafEv6+XRW8oVUvpDKp7OSb0k/jz026dEBAAAAPEwwNEJ33tHPrTyVx7OXSlJJHs9ebmcj7/iNvibUAAAAwFQRDI3Q73v/Vr40jzYZ+pIc5L/9V1v6DAEAAABTRTA0Sic0ElrNXX2GAAAAgKkiGBql1dVjn7qb1bSWVD26razENDMAAABg7ARDo7S9nVy58sjhz2Up35ntY9+2t5dsbAiHAAAAgPESDI1Sr5fcvp0sL6claUnuZTlP5VZ+ML0T33pwED2IAAAAgLG6POkBzJ1eL+n18qpLSWvne6seRAAAAMA4qRjqyAnthkb6HgAAAICLEgx15Jh2Q8daWhq8BwAAAGBcBEMdeaDd0KmWl5NbtwbvAQAAABgXwVBX+v30ttby/AuX0q6tpd3pp7U8tN25MwiF9vaSJ588eil7S9oDAAAAXREMdaHfTzY3k93dQQK0uzvYfyDZ6feTp54ahEJncT88eu1rBUQAAADAaAiGurC1lezvP3xsf/+h9ei3tpKXXjr/qV98MdnYEA4BAAAAwxMMdeG4decfOD7M0vQHBw9lTAAAAAAXIhjqwnHrzj9wfNil6YcJlgAAAAASwVA3treTq1cfPnb16kPr0Z93OftXGjZYAgAAABAMdaHXS27efHit+le/+pGXnHU5+1daWnooYwIAAAC4EMFQl37rt17+em/vkZXJer3k+efzyDL2Ry1pf9/ycnLr1uC9AAAAAMMQDHXluJXJrl8/12nuh0f3A6L7y9ZXHb2trFixDAAAADgbwVBXjusOvbd37uSm30+eemrw1tMIjgAAAICzEgx15aTu0Odca35rK3nppSHHc2hvL9nYEA4BAAAAgqHunNQd+pxrzY96afqDg3NnUwAAAMAcEgx1pdc7fsmxc64138XS9KMOmwAAAIDZIxjq0o0bydWrDx+7evXca81vbydXroxwXEkee2y05wMAAABmj2CoS71ecvNmcu3aoPPztWuD/XOuNd/rJbdvH1+AdBF7expUAwAAwKITDHWt1xuU/KyuDuZvbW1dKHW5v2x9a0dv95ezH4X7K5u99rUCIgAAAJhngqGu9fvJ5mayuztIcHZ3B/sjTlxOCo6qLnbOF18cBEQqigAAAGA+CYa6trWV7O8/fGx/f6zLgo26ebWKIgAAAJgPgqGuHbf81xiXBdvevnjV0ElefDHZ2BAOAQAAwKwSDHXtuHKdLtagP0avlzz9dDfnPjg4erqZKWcAAAAw/QRDXdveHsmS9cN65pnRNqg+i709FUUAAAAwzToLhqrqb1TVL1bVP6+q91XV67u61lQb0ZL1oxrKaSubveY1o73mwcFY2ykBAAAA51CttW5OXPVNSf5xa+3zVfXdSdJa+29Oes/6+nrb2dnpZDycXb+fXL8+qPgZharkC18YzbkAAACA86mqZ1tr60c911nFUGvtf2utff5w96eTvLGrazFax1UW3bmTXLrAv5jW9CACAACAaTSuHkMb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\n",
+                        "text/plain": [
+                            "<Figure size 1440x360 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "# Compute and plot the last gali index at each iteration\n",
+                "# Note, running minimum is appended at each iteration\n",
+                "\n",
+                "plt.figure(figsize=(20, 5))\n",
+                "\n",
+                "x = torch.tensor([0.50000, 0.0, 0.05, 0.0], dtype=dtype, device=device)\n",
+                "vs = torch.eye(4, dtype=dtype, device=device)\n",
+                "out = []\n",
+                "for _ in range(count):\n",
+                "    x, vs = tangent(x, vs)\n",
+                "    res = gali(vs)\n",
+                "    out.append(res if not out else min(res, out[-1]))\n",
+                "out = torch.stack(out)\n",
+                "plt.scatter(range(count), out, color='blue', marker='o')\n",
+                "    \n",
+                "x = torch.tensor([0.68925, 0.0, 0.10, 0.0], dtype=dtype, device=device)\n",
+                "vs = torch.eye(4, dtype=dtype, device=device)\n",
+                "out = []\n",
+                "for _ in range(count):\n",
+                "    x, vs = tangent(x, vs)\n",
+                "    res = gali(vs)\n",
+                "    out.append(res if not out else min(res, out[-1]))\n",
+                "out = torch.stack(out)\n",
+                "plt.scatter(range(count), out, color='red', marker='o')\n",
+                "               \n",
+                "plt.show()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "ce599a3d-c656-408d-8d7d-37f02241decf",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAbsAAAHLCAYAAABRSzbfAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8qNh9FAAAACXBIWXMAAAsTAAALEwEAmpwYAAEAAElEQVR4nOydeXhdVb3+PzuHpGlOk54mTRs70FJaCqW1gGGUqYggsyDiRRQUBBy4gAKKFn7CBRRBFBBEUUGQ4QoIMggyXArIKAHpbSkUSmkp7e0Y0qQnpAnJ/v3xrm/WOqcpKk1LWtb7POc5J3tYe+19Tta73u+0kjRNiYiIiIiI2JRR8mF3ICIiIiIiYn0jkl1ERERExCaPSHYREREREZs8ItlFRERERGzyiGQXEREREbHJI5JdRERERMQmj0h2ERERERF9DkmSXJokyatJkvxvkiR3JUmSW5f2ItlFRERERPRFPAxMTNP048BrwPfXpbFIdhERERERfQ5pmj6Upul77s9ngRHr0l4ku4iIiIiIvo7jgQfWpYHNeqkjEREREREbMT7zmc+ky5cv79U2X3jhhZeBtmDTtWmaXmt/JEnyCFDXw6lT0zS92x0zFXgPuHld+hLJLiIiIiKC5cuX09DQ0KttJknSlqZp/dr2p2m67z85/yvAwcCn0nUs5BzJLiIiIiICSJGA6htIkuQzwHeBvdI0bV3X9iLZRUREREQ49B2yA64C+gEPJ0kC8Gyapl//oI1FsouIiIiI6HNI03Rsb7YXyS4iIiIigr5mxuxtxNSDiIiIiIhNHlHZRURERESwqSu7SHYREREREWzqZBfNmBERERERmzyisouIiIiIICq7iIiIiIiIjRxR2UVEREREEJVdRERERETERo6o7CIiIiIiHDZdZRfJLiIiIiICmTE7P+xOrDdEM2ZERERExCaPqOwiIiIiIogBKhERERERERs5orKLiIiIiGBTV3aR7CIiIiIiHDZdsotmzIiIiIiITR5R2UVEREREsKmbMaOyi4iIiIjY5BGVXUREREQEm7qyi2QXEREREcGmTnbRjBkRERERsckjKruIiIiICKKyi4iIiIiI2MgRlV1EREREhMOmq+wi2UVEREREEM2YERERERERGzmisouIiIiIICq7iIiIiIiIjRxR2UVEREREEJVdRERERETERo6o7CIiIiIi2NSVXSS7iIiIiAiHTZfsohkzIiIiImKTR1R2ERERERFs6mbMqOwiIiIiIjZ5RGUXEREREcGmruwi2UVEREREILLr/LA7sd4QzZgREREREZs8orKLiIiIiGBTN2NGZRcRERERsckjKruIiIiICIdNV9lFsouIiIiIIJoxIyIiIiIiNnJEZRcRERERQVR2ERERERERGzmisouIiIiIoK8puyRJLgAOA7qApcBX0jRd9EHbi8ouIiIiIqIv4tI0TT+epul2wH3A/1uXxqKyi4iIiIigrym7NE2bgz+zqIMfGJHsIiIiIiIcep3sBidJ0hD8fW2aptf+qycnSXIRcCywEpiyLh2JZBcRERERsb6wPE3T+rXtTJLkEaCuh11T0zS9O03TqcDUJEm+D5wC/PCDdiSSXUREREQEH4YZM03Tff/FQ28G7mcdyC4GqERERERE9DkkSTIu+PMw4NV1aS8qu4iIiIgI+lqACnBxkiTjUerBfODr69JYJLuIiIiICPoa2aVp+rnebC+aMSMiIiIiNnlEZRcRERERQV9Tdr2NqOwiIiIiIjZ5RGUXEREREeGw6Sq7SHYREREREUQzZkRERERExEaOqOwiIiIiIojKLiIiIiIiYiNHVHYREREREURlFxERERERsZEjKruIiIiICIfOD7sD6w2R7CIiIiIiiGbMiIiIiIiIjRxR2UVEREREEJVdRERERETERo6o7CIiIiIi2NSVXSS7iIiIiAg2dbKLZsyIiIiIiE0eUdlFRERERBCVXURERERExEaOqOw2ELJJkubTNPmw+xERERGxdmy6yi6S3QZCJLqIiIi+jWjGjNjIkE2S9MPuQ0RERERfQlR2myCiioyIiPj3EZVdRERERETERo2o7CIiIiIiiMouIiIiIiJiI0dUdhERERERbOrKLpJdRERERITDpkt20YwZEREREbHJIyq7iIiIiAg2dTNmVHYfUWSTJI3J5xERER8VRGX3EUVMPI+IiCjEpq3sItlFRERERLCpk100Y0ZEREREbPKIyi4iIiIigqjsIiIiIiIiNnJEZRcRERER4dD5YXdgvSGSXUREREQE0YwZ0Sfx7+bIvd/xtq/43T7HfLyIiIiNHVHZbaT4Z3ly2SRJw2PyaZrYtnBfSGS2rfi8sM3itnrvjiIiIj5cRGUXsRGimMyySZLmR6yp2orPC48PX9ZmPk2T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cSI/XsShjz09t5CcJiJEu52urwTLsogvXJYV9BLk+hUM2VlCS0Uk44lN/wdKSC6B7tOGj/bsRghuhzvdq926EeB02b5nC2AHl4l4VCOp1eLYhhERERGPdnQlSe3kFh/zarhloiF+JhOxix8RERERARzZASqxgkpERERExBGPqOwiIiIiImJtzIiIiIiIiMMdUdlFRERERABR2UVERERERBzWiMouIiIiIiKWC4uIiIiIeHQgmjEjIiIiIiIOY0RlFxERERFxxJsxo7KLiIiIiDjiEZVdRERERARwZPvsItlFRERERMQKKhEREREREYc7orKLiIiIiABigEpERERERMRhjajsIiIiIiKOeJ9dJLuIiIiIiCOe7KIZMyIiIiLiiEdUdhERERERQAxQiYiIiIiIOKwRlV1ERERERPTZRUREREREHO6Iyi4iIiIiAjiyfXaR7CIiIiIiohkzIiIiIiLicEdUdhERERERQFR2ERERERERhzWisouIiIiIoEYMUImIiIiIeBQgmjEjIiIiIiIOY0RlFxERERERUw8iIiIiIiIOd0RlFxEREREBHNkBKlHZRURERETUzZit/BwIkiR5UZIkdyVJMp4kyepg3duTJLk/SZJ7kiR5+t4cLyq7iIiIiIhDEXcCzwc+bxcmSbICeClwHDAHuDpJkmNrtdqE/BrJLiIiIiICOLTMmLVa7Q8ASZKEq84FvlGr1XYDDyZJcj9wEnD9RMeLZsyIiIiIiMMJc4EN5vtGt2xCRGUXEREREcE4XDkIM1p82FKSJDeb75fUarVL9EuSJFcDPRn7XVSr1X7YyguJZBcRERERQa1We8af4Zxn7cdum4D55vs8t2xCRDNmRERERMThhB8BL02SZEqSJI8BlgI37mmnSHYREREREYcckiR5XpIkG4FTgZ8kSXIlQK1Wuwv4FrAG+F/gDXuKxARIarXawbzeiIiIiIiIPzuisouIiIiIOOIRyS4iIiIi4ohHJLuIiIiIiCMekewiIiIiIo54RLKLiIiIiDjiEckuIiIiIuKIRyS7iIiIiIgjHpHsIiIiIiKOePz/1fweHee7lD4AAAAASUVORK5CYII=\n",
+                        "text/plain": [
+                            "<Figure size 576x576 with 2 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "# Compute indicator using all avaliable vectors for a grid of initial conditions\n",
+                "\n",
+                "def gali(vs):\n",
+                "    return torch.linalg.svdvals(vs.nan_to_num()).prod()\n",
+                "\n",
+                "# Set grid\n",
+                "\n",
+                "n1 = 501\n",
+                "n2 = 501\n",
+                "\n",
+                "q1 = torch.linspace(-1.0, +1.0, n1, dtype=dtype, device=device)\n",
+                "q2 = torch.linspace(+0.0, +1.0, n2, dtype=dtype, device=device)\n",
+                "\n",
+                "qs = torch.stack(torch.meshgrid(q1, q2, indexing='ij')).swapaxes(-1, 0).reshape(n1*n2, -1)\n",
+                "ps = torch.full_like(qs, 1.0E-10)\n",
+                "\n",
+                "q1, q2, p1, p2 = torch.hstack([qs, ps]).T\n",
+                "\n",
+                "vs = torch.tensor(n1*n2*[torch.eye(4).tolist()], dtype=dtype, device=device)\n",
+                "qs = torch.stack([q1, p1, q2, p2]).T\n",
+                "\n",
+                "# Set tast\n",
+                "# Perform 512 iterations, compute min of indicator value over the next 64 iterations\n",
+                "\n",
+                "def task(qs, vs, count=512, total=64, level=1.0E-10):\n",
+                "    for _ in range(count):\n",
+                "        qs, vs = tangent(qs, vs)\n",
+                "    out = []\n",
+                "    for _ in range(total):\n",
+                "        qs, vs = tangent(qs, vs)\n",
+                "        out.append(gali(vs))\n",
+                "    return (torch.stack(out).min() + level*torch.sign(qs.norm())).log10()\n",
+                "\n",
+                "# Compute and clean data\n",
+                "\n",
+                "out = torch.vmap(task)(qs, vs)\n",
+                "out = out.nan_to_num(neginf=0.0)\n",
+                "out[(out >= -2.0)*(out != 0.0)] = -2.0\n",
+                "out[out == 0.0] = torch.nan\n",
+                "out = out.reshape(n1, n2)\n",
+                "\n",
+                "# Plot\n",
+                "\n",
+                "plt.figure(figsize=(8, 8))\n",
+                "plt.imshow(\n",
+                "    out.cpu().numpy(),\n",
+                "    vmin=-10.0,\n",
+                "    vmax=-2.0,\n",
+                "    aspect='equal',\n",
+                "    origin='lower',\n",
+                "    cmap='hot', \n",
+                "    interpolation='nearest')\n",
+                "plt.colorbar()\n",
+                "plt.axis('off')\n",
+                "plt.show()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "b1b42a98-fe47-4ae7-9613-114ed5b49e66",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
+                "# Example-11: Closed orbit (dispersion)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "70f1f56c-1877-4291-8a2f-9d75c8d5d249",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# In this example derivatives of closed orbit with respect to momentum deviation are computed"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "43e44d11-1a03-4f8c-a3a7-82df2e4bb4a1",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.evaluate import compare\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "torch.set_printoptions(precision=8, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "0d70fa1d-1104-4f6c-85e1-a623639ce449",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "be0696f0-5b8b-4028-9f3e-4d473175c1b3",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "eb26687c-9b4f-436b-ba87-b2848af36127",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "# Note, here observation poins are locations between elements, lattice start and lattice end\n",
+                "# An observable (closed orbit) is computed at observation points\n",
+                "\n",
+                "# All maps are expected to have identical signature of differentible parameters\n",
+                "# State and momentum deviation in this example\n",
+                "# But each map can have any number of additional args and kwargs after required parameters\n",
+                "\n",
+                "def map_01_02(x, w): return quad(x, w, 0.19, 0.50)\n",
+                "def map_02_03(x, w): return drif(x, w, 0.45)\n",
+                "def map_03_04(x, w): return sext(x, w, 0.00, 0.10)\n",
+                "def map_04_05(x, w): return drif(x, w, 0.45)\n",
+                "def map_05_06(x, w): return bend(x, w, 22.92, 0.015, 0.00, 3.0)\n",
+                "def map_06_07(x, w): return drif(x, w, 0.45)\n",
+                "def map_07_08(x, w): return sext(x, w, 0.00, 0.10)\n",
+                "def map_08_09(x, w): return drif(x, w, 0.45)\n",
+                "def map_09_10(x, w): return quad(x, w, -0.21, 0.50)\n",
+                "def map_10_11(x, w): return quad(x, w, -0.21, 0.50)\n",
+                "def map_11_12(x, w): return drif(x, w, 0.45)\n",
+                "def map_12_13(x, w): return sext(x, w, 0.00, 0.10)\n",
+                "def map_13_14(x, w): return drif(x, w, 0.45)\n",
+                "def map_14_15(x, w): return bend(x, w, 22.92, 0.015, 0.00, 3.0)\n",
+                "def map_15_16(x, w): return drif(x, w, 0.45)\n",
+                "def map_16_17(x, w): return sext(x, w, 0.00, 0.10)\n",
+                "def map_17_18(x, w): return drif(x, w, 0.45)\n",
+                "def map_18_19(x, w): return quad(x, w, 0.19, 0.50)\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02,\n",
+                "    map_02_03,\n",
+                "    map_03_04,\n",
+                "    map_04_05,\n",
+                "    map_05_06,\n",
+                "    map_06_07,\n",
+                "    map_07_08,\n",
+                "    map_08_09,\n",
+                "    map_09_10,\n",
+                "    map_10_11,\n",
+                "    map_11_12,\n",
+                "    map_12_13,\n",
+                "    map_13_14,\n",
+                "    map_14_15,\n",
+                "    map_15_16,\n",
+                "    map_16_17,\n",
+                "    map_17_18,\n",
+                "    map_18_19    \n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, w):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, w)\n",
+                "    return x"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "e4bda838-f9e7-40aa-8cbf-568852ae112b",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# The first step is to compute dynamical fixed point\n",
+                "\n",
+                "# Set initial guess\n",
+                "# Note, in this example zero is a fixed point\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "# Set knobs\n",
+                "\n",
+                "w = torch.tensor([0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "# Find fixed point\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, w, power=1)\n",
+                "\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "c95878f6-0ab7-45ea-b7f2-971c6f682986",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "(0, 0, 0, 0, 0): [0. 0. 0. 0.]\n",
+                        "(0, 0, 0, 0, 1): [1.81613351 0.         0.         0.        ]\n",
+                        "(0, 0, 0, 0, 2): [0.56855511 0.         0.         0.        ]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute parametric closed orbit\n",
+                "\n",
+                "pfp = parametric_fixed_point((2, ), fp, [w], fodo)\n",
+                "chop(pfp)\n",
+                "\n",
+                "# Print series representation\n",
+                "\n",
+                "for key, value in series((4, 1), (0, 2), pfp).items():\n",
+                "    print(f'{key}: {value.cpu().numpy()}')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "81c0b250-6e0c-455f-8884-6686a06ba96e",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n",
+                        "tensor([1.81613351e-03, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00], dtype=torch.float64)\n",
+                        "tensor([1.81670206e-03, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00], dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([1.81670185e-03, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00], dtype=torch.float64)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Check convergence\n",
+                "\n",
+                "print(evaluate(series((4, 1), (0, 0), pfp), [x, w + 1.0E-3]))\n",
+                "print(evaluate(series((4, 1), (0, 1), pfp), [x, w + 1.0E-3]))\n",
+                "print(evaluate(series((4, 1), (0, 2), pfp), [x, w + 1.0E-3]))\n",
+                "print()\n",
+                "\n",
+                "out = fixed_point(16, fodo, x, w + 1.0E-3, power=1)\n",
+                "chop([out])\n",
+                "\n",
+                "print(out)\n",
+                "print()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "022f1ef1-96de-4139-bf64-b6517788184b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Propagate closed orbit\n",
+                "\n",
+                "out = []\n",
+                "\n",
+                "jet = identity((0, 1), fp, parametric=pfp)\n",
+                "out.append(jet)\n",
+                "\n",
+                "for mapping in transport:\n",
+                "    jet = propagate((4, 1), (0, 2), jet, [w], mapping)\n",
+                "    out.append(jet)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "cff7e5c8-d2d5-4903-901a-40811262f87e",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Check periodicity\n",
+                "\n",
+                "print(compare(pfp, jet))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "cae68275-4659-450a-bc95-c309fda3cfad",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "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\n",
+                        "text/plain": [
+                            "<Figure size 1440x360 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "# Plot 1st order dispersion\n",
+                "\n",
+                "pos = [0.00, 0.50, 0.95, 1.05, 1.50, 4.50, 4.95, 5.05, 5.50, 6.00, 6.50, 6.95, 7.05, 7.50, 10.50, 10.95, 11.05, 11.50, 12.00]\n",
+                "res = torch.stack([series((4, 1), (0, 2), jet)[(0, 0, 0, 0, 1)][0] for jet in out])\n",
+                "\n",
+                "plt.figure(figsize=(20, 5))\n",
+                "plt.plot(pos, res.cpu().numpy(), marker='x', color='blue')\n",
+                "plt.show()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "4ebb02ef-1954-4d15-98d5-9a409ad718d6",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "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axQ2om5TeEySpFL3559pdVCDBnDTTWnrxvjx6diaa2adTpKS9deH++6DUaNgzz3hsstg003h3nvTJEVJkkrbEotDMcbZwGmkos5YoG+McXQIoXsIoX3h3fYAxoUQxgPrAFcXPvYH4EpSgWkY0L3wmCRJpWbOHHjwQWjYEC68EHbZJfUUeugh2GijrNNJ0qI1bgz9+8M776Ti0CmnwJZbwtNPp8mKkiSVlhBz7JUmLy8vFhQUZB1DklQGxQgvvAAXXQSjR8P226dVQrvvnnUySVo6836fde0KY8bADjuk32e77ZZ1MklSWRVCGB5jzFvUbSXVkFqSpEy9914qArVvDzNnwlNPzT8mSWVNCLDffmnV4wMPwNSp6ffZfvul7WeSJJUki0OSpDJt3Dg46CDYaafUT+juu9OqoYMPdiy9pLKvShU49tj0++266+DNN2GbbdKxL77IOp0kqbywOCRJKpO++gpOPhm22AJeeQW6d08Tf045BapWzTqdJJWslVZKPdQmTYKzz4bevVNftQsugB9/zDqdJKmsszgkSSpTfvkFunVLzVofeAD+/e90stStG6yyStbpJKl0rbUW3HhjWkl06KHp8iabwA03wF9/ZZ1OklRWWRySJJUJM2fC7bensfRXXZX6bnzySTq29tpZp5OkFatePejVC0aMSNtqL7gANtssHZszJ+t0kqSyxuKQJCmnzZ0LTzyRRjyfeSZsvTUMGwZ9+qRCkSRVZNtsAwMHwpAhsM460KULNG0KL76YJp5JklQcFockSTnr1VeheXM4/HBYbTUYNCgdy1vkAE5JqrhatoT334cnn4Q//4R9903H/ve/rJNJksoCi0OSpJwzYgS0aQOtW8P338Ojj8IHH8BeezmBTJIWJwTo2BHGjoW77krfd9wRDjkk9SiSJGlxLA5JknLGp5/CEUfAttvC8OFw881pVP2RR0IlX7EkqViqVk3N+idOhMsvh5degiZN0rGvv846nSQpF/lWW5KUue++g7POgkaN4Jln4KKLYPLkNK65evWs00lS2bTqqnDFFWmi48knw/33p0mPl18Ov/6adTpJUi6xOCRJyszvv8PVV6cxzHfcAZ07w4QJcM01UKtW1ukkqXxYZx24804YMwb22Qe6d08N/e+8M02ClCTJ4pAkaYWbPRt69oSGDeHSS+Ff/4JRo9Kn2htskHU6SSqfGjZMDavffx+22AJOPz1tN3vyyTQZUpJUcVkckiStMDGmbWNbbgknnQT168Nbb8GAAbD55lmnk6SKoXlzGDIEBg6ElVaCTp1g++3htdeyTiZJyorFIUnSCvHWW7DLLnDggWmizoAB849JklasEGDvvdN0yF69YPp02HNPaNsWPvww63SSpBXN4pAkqVSNGQPt20OLFvD552nr2McfQ4cOjqWXpKxVrgxHH50mQ954Y9pytu22cNRR8NlnWaeTJK0oFockSaVi6lQ47jjYait4443UZHrCBDj+eKhSJet0kqSiatSAc89NkyIvuAD69UsTJM85B77/Put0kqTSZnFIklSifvoJunZNjU8fewzOPDONUb7ootTbQpKUu1ZfHa67LhXzjzwSbrstTZS89lr444+s00mSSovFIUlSifjrL7jppnQS0aMHHHxw2qZw881Qu3bW6SRJS6NuXXjgARg5EvbYAy6+OBX9//vfNHFSklS+WBySJC2XOXPgkUfS9oPzzksTbz74AB59FDbeOOt0kqTlscUW8OyzMHQo1KsHJ5wAW2+djsWYdTpJUkmxOCRJWiYxwksvpcalnTtDnTrw6qswaBA0bZp1OklSSWrRAt5+G/r3h7lzYf/95x+TJJV9FockSUtt2DBo1QratYPffoM+fdKEm1atsk4mSSotIcABB8CoUXDffamf3K67pkLR2LFZp5MkLQ+LQ5KkYps4ETp2TFvHRo2CO+5IJwSHHgqVfEWRpAqhShU48cT0mnDVVTBkCGy5ZdpyNm1a1ukkScvCt/KSpCX65hs49VTYfHMYOBAuuyydFJx2GlSrlnU6SVIWVl4ZLrkEJk+G00+HXr1S0+qLL4aff846nSRpaVgckiQt1q+/wn/+A5tumrYQnHBCKgr95z+w2mpZp5Mk5YLateHWW9OEygMOSGPvN9kEbrkFZszIOp0kqTgsDkmS/mbWLLj77lQUuuIKaNsWxoxJx9ZdN+t0kqRcVL8+9O6dJlZutx2cc06aZPnYY6mJtSQpdxWrOBRCaBtCGBdCmBhC6LqI2zcKIeSHEEaEEEaGENoVHt84hPBnCOHDwq97S/oHkCSVnBihb19o0iRtI2vcGN57D556CjbbLOt0kqSyoFkzeOWV9LXmmnDUUWmy5csvp9cZSVLuWWJxKIRQGbgL2BtoAhwWQmiy0N0uBfrGGJsBnYC7i9w2KcbYtPDr5BLKLUkqYfn5sMMOqbl0jRrw4ovw+uvpmCRJS6t1aygogMcfh19+SatQ99wThg/POpkkaWHFWTm0PTAxxjg5xjgT6AN0WOg+EZjXfaIW8GXJRZQklaaRI9NI+n/9C776Ch56CD78MB0LIet0kqSyrFIlOOywNNnyttvSa05eXjo2aVLW6SRJ8xSnOLQB8EWR61MLjxV1BXBkCGEqMBA4vcht9Qu3m70RQmixPGElSSXn88+hc2do2hTefRd69IDx46FLF6hcOet0kqTypHp1OOOMVBC69FJ47rk0AfOMM+Dbb7NOJ0kqqYbUhwEPxxjrAu2AR0MIlYCvgI0Kt5udAzweQvjbfJsQwokhhIIQQsH06dNLKJIkaVG+/x7OOy/1EHrySTj//DSG+PzzoWbNrNNJksqz1VaDK69Mky+PPTYNOmjQALp3h99+yzqdJFVcxSkOTQM2LHK9buGxoo4D+gLEGN8FagC1Y4wzYozfFx4fDkwC/tbSNMbYM8aYF2PMq1OnztL/FJKkJfrzT7j++vQm/Oab4YgjYMKEdGyNNbJOJ0mqSNZbD+69F0aPhjZt4PLL04TMe+5JEzMlSStWcYpDw4CGIYT6IYRqpIbTzy10nylAK4AQwuak4tD0EEKdwobWhBA2ARoCk0sqvCRpyebMgQcfhIYNoWtXaNEi9Xx48EHYcMMlP16SpNLSqBE8/TS88056nfr3v2GLLaBfPyebSdKKtMTiUIxxNnAa8DIwljSVbHQIoXsIoX3h3c4FTgghfAQ8AXSJMUZgN2BkCOFDoB9wcozxh1L4OSRJC4kRnn8ett4ajjsO6tZN08eefx623DLrdJIkzbfTTjB0aOpFVLUqHHII7LgjvPFG1skkqWIIMcdK8nl5ebGgoCDrGJJUpr37LlxwAbz1VuotdM01cOCBTh+TJOW+OXPgkUfgsstg6lTYZx+49lrYaqusk0lS2RZCGB5jzFvUbSXVkFqSlAPGjUtFoJ13Tv2E7rkHRo2Cgw6yMCRJKhsqV4ZjjkkTNK+/Pn3Qsc026diUKVmnk6TyyeKQJJUDX34JJ52U+jQMHpymvkycCCefnJbnS5JU1tSsmVbBTp4M554LTzyRVsNecAH8YKMKSSpRFockqQz7+We49NI04eWhh1Ijz0mToFs3WGWVrNNJkrT81lwTbrghrY499FC48cY0ebNHjzSJU5K0/CwOSVIZNGMG3HZbenN89dXQoQOMHQu33w5rr511OkmSSl69etCrF3z4Ydo+feGFaSXRQw+lPkWSpGVncUiSypC5c+Hxx2HzzeGss6BpUygoSEvtGzTIOp0kSaVv663hxRchPx/WWw+OPTa9Hr74YprUKUlaehaHJKmMGDwY8vLgiCOgVi14+eV0bLvtsk4mSdKKt8ce8L//Qd++8NdfsO++6dh772WdTJLKHotDkpTjPvgAWreGNm3gxx/hscdg+PB03QlkkqSKLAQ45BAYMwbuugs++QR22gkOPjj1KJIkFY/FIUnKUZMnw+GHp5VBI0bALbekN71HHAGV/O0tSdL/q1p1/lCGK65Iq2u32AJOOQW++irrdJKU+zy9kKQcM306nHkmNG4MAwbAxRenN7tnnQXVq2edTpKk3LXKKnD55TBxIpx8Mvz3v2mi52WXwS+/ZJ1OknKXxSFJyhG//w5XXZUaS995J3Tpkt7cXn116jEkSZKKZ5110mvp2LGpF9GVV6Yi0R13wMyZWaeTpNxjcUiSMjZrFtx3X3rT2q0btGoFo0ZBz56w/vpZp5MkqezadFN48kl4/33Ycks444w08bNPnzQBVJKUWBySpIzECP37pzerJ5+cVgy9/TY880x64ypJkkpG8+bw2mvw0ktp69lhh8H226djkiSLQ5KUiTffhJ13hoMOgsqV4dln5x+TJEklLwRo2zYNeXjkkdTjb889Ya+94MMPs04nSdmyOCRJK9Do0dC+Pey2G0yZkhpljhyZjjmWXpKk0lepEhx1VBp1f9NNUFAAzZrBkUfCZ59lnU6SsmFxSJJWgKlT4dhjYeutYehQuPZamDABjjsOqlTJOp0kSRVPjRpwzjlpImjXrvD009CoEZx9Nnz3XdbpJGnFsjgkSaXoxx/hwguhYUPo3TuNo5/3JnSllbJOJ0mSVl89fWgzcWJaUXT77akP4DXXwB9/ZJ1OklYMi0OSVAr++gtuvDG9ubzhBjjkkPnL19daK+t0kiRpYRtskLZ7f/wx7LEHXHJJmnZ2//0we3bW6SSpdFkckqQSNGcO9OoFm20G558PO+wwv/HlxhtnnU6SJC1JkybzB0VsvDGceCJstRUMGJAmjUpSeWRxSJJKQIwwcGBqaNmlC6y99vyRudtsk3U6SZK0tHbdFd5+G555Jl0/4ID5xySpvLE4JEnL6f334V//gn32Sb0Jnnxy/jFJklR2hQD775+2mvXsCZ9+mgpEHTrAmDFZp5OkkmNxSJKW0YQJ0LFj2jo2ejTceWd6o9ixYxqTK0mSyocqVeCEE9Jr/9VXw+uvp61mxx8P06ZlnU6Slp+nL5K0lL75Bk49NfUkGDgQLrssTSA79VSoVi3rdJIkqbSsvDJcfHF63T/jjNRTcNNN4aKL4Kefsk4nScvO4pAkFdOvv8Lll6cJZD17pgaVEyfCf/4Dq66adTpJkrSi1K4Nt9ySJpEedBBcd116f3DzzTBjRtbpJGnpWRySpCWYORPuuit9Mti9O7Rrl7aP3XUXrLtu1ukkSVJW6teHxx6DDz6AvDw491xo1AgefRTmzs06nSQVn8UhSVqMuXNTc+kmTeC002DzzeF//4O+faFhw6zTSZKkXNGsGbz8MgweDGutBUcfDdtuC4MGpYmmkpTrLA5J0iIMGZIaTXfqBDVrwosvQn4+bL991skkSVKu2nNPGDYMHn8cfvkF9t4bWrWCgoKsk0nSPytWcSiE0DaEMC6EMDGE0HURt28UQsgPIYwIIYwMIbQrcttFhY8bF0LYqyTDS1JJ++ij+W/kvvkGHn4YPvwwbSULIet0kiQp11WqBIcdBp98ArffDh9/DM2bw6GHpl6FkpSLllgcCiFUBu4C9gaaAIeFEJosdLdLgb4xxmZAJ+Duwsc2Kby+BdAWuLvwz5OknPL552kJeLNmaevYDTfA+PHQuTNU9reWJElaStWqwemnp8lm3brBCy+kLeqnnw7ffpt1OklaUHFWDm0PTIwxTo4xzgT6AB0Wuk8EViu8XAv4svByB6BPjHFGjPFTYGLhnydJOeH771PzyM02S72Ezj8/vYk77zyoUSPrdJIkqaxbbbU00GLiRDj+eLjnnjTZrHt3+O23rNNJUlKc4tAGwBdFrk8tPFbUFcCRIYSpwEDg9KV4LCGEE0MIBSGEgunTpxczuiQtuz/+mD929tZb4YgjYMIEuP56WGONrNNJkqTyZr31UmFo9GjYay+4/PL0PuTuu2HWrKzTSaroSqoh9WHAwzHGukA74NEQQrH/7BhjzxhjXowxr06dOiUUSZL+bvZseOCBtFLoootgt91Sn6EHH4QNN8w6nSRJKu8aNYJ+/eDdd9PlU09Nk1GfesrJZpKyU5wCzjSg6ClT3cJjRR0H9AWIMb4L1ABqF/OxklTqYoTnnoNttklLujfcEN54Ix3bcsus00mSpIpmxx3Te5Hnn4fq1aFjx3Ts9dezTiapIipOcWgY0DCEUD+EUI3UYPq5he4zBWgFEELYnFQcml54v04hhOohhPpAQ+D9kgovScXxzjtphVCHDmnl0NNPzz8mSZKUlRBg333nr2L+8kto2RL22QdGjsw6naSKZInFoRjjbOA04GVgLGkq2egQQvcQQvvCu50LnBBC+Ah4AugSk9GkFUVjgEHAqTHGOaXxg0jSwj75BA44AHbZJTWBvPdeGDUKDjzQsfSSJCl3VK4MxxyTJqVef336EKtpU+jSBaZMyTqdpIogxBzb2JqXlxcLCgqyjiGpDPvyS7jiitRbaOWV4YIL4Oyz02VJkqRc98MPaXDG7ben66efnnolrrlmtrkklW0hhOExxrxF3VZSDaklKXM//wyXXAKbbgoPPwynnZbG0l96qYUhSZJUdqy5JvTokVYSHXYY3HRTmmzWowf8+WfW6SSVRxaHJJV5M2akcfQNGsA118D++6ctZbfdBg5AlCRJZdVGG8FDD6WeRDvvDBdemCauPvQQzLFZh6QSZHFIUpk1dy707g2NG6dtY82awfDh8PjjsMkmWaeTJEkqGVttBS++CPn5sP76cOyxaQLr88+niayStLwsDkkqk155BbbbDo48EtZYI10fPBi23TbrZJIkSaVjjz3gvffgqadg5kxo3x523z0dk6TlYXFIUpkyfDi0bg177QU//ZRWDhUUpGOSJEnlXQhw8MEwejTcfXfqS7TTTnDQQTBuXNbpJJVVFocklQmTJ8Phh0NeHowYkXoMffJJOlbJ32SSJKmCqVoVTjkFJk6E//wnraLeYgs4+WT46qus00kqazylkpTTpk+HM85IfYUGDEjTyCZNgjPPhOrVs04nSZKUrVVWgcsuS++PTjkFHnggTW7t1g1++SXrdJLKCotDknLS77/DlVemCWR33w3HHJM+GbvqKqhVK+t0kiRJuWXtteGOO2DsWNhvv/SeqUEDuP321J9Ikv6JxSFJOWXWLLj33vSJ12WXwZ57wqhRcN99aTqHJEmSFm/TTaFPHxg2DLbeOq22btwYnngiTXqVpEWxOCQpJ8QITz8NW26ZlkQ3aABvvw39+6c3NJIkSSq+vDx49VUYNAhWWy31aWzePB2TpIVZHJKUuaFD05SNgw+GypXh2WfhzTdh552zTiZJklR2hZAmvH7wATz6KHz/fZrw2qZNGvAhSfNYHJKUmVGj0p743XeHqVNTA8WRI6F9+/RmRpIkScuvUiU48sg06fXmm2H4cNh2WzjiCPj006zTScoFFockrXBffAHHHgvbbJNWCF13HYwfn45VqZJ1OkmSpPKpRg04+2yYPBkuugieeQYaNYKzzoLvvss6naQsWRyStML8+CNceCFsthn07p3enEyalI6ttFLW6SRJkiqGWrXgmmtgwgTo3DlNOWvQAK6+Ok2MlVTxWBySVOr++gtuuAE22SR979gxrRS68UZYa62s00mSJFVMG2wA99+ftvq3bAmXXgoNG0LPnjB7dtbpJK1IFocklZo5c6BXr7RS6IILUtPpESPSsXr1sk4nSZIkgM03hwED4K23oH59OOmkNEH2mWfSRFlJ5Z/FIUklLkZ48UVo2hS6dIF11oEhQ2DgwNRnSJIkSblnl11SgWjAgDQc5MAD5x+TVL5ZHJJUov73v7Qsed994c8/4ckn4f330zFJkiTlthCgQwf4+OO05ezzz6FFizRNdsyYrNNJKi0WhySViPHj4ZBDYMcdYexYuPPO9AaiY0fH0kuSJJU1VarA8cenptXXXANvvAFbbQXHHQdTp2adTlJJszgkabl8/TX8+9/QpAm89BJcfjlMnAinngrVqmWdTpIkSctjpZXS2PtJk+DMM+Gxx1LT6q5d4aefsk4nqaRYHJK0TH79NRWCNt00LTk+6aT0puGKK2DVVbNOJ0mSpJJUuzbcfDOMGwcHHww9eqRJtDfdlCbTSirbLA5JWiozZ6YtYw0aQPfu0K5d2j52112p8bQkSZLKr403hkcfhQ8+gO23h/POg0aN4JFH0qRaSWWTxSFJxTJ3bmou3aQJnH46bLFFaj7dt29aWixJkqSKo2lTGDQIXn0V6tSBzp1h221Tm4EYs04naWlZHJK0REOGpE+GOnVK+84HDpx/TJIkSRVXq1ZpMm2fPvDbb2lVeatWMGxY1skkLQ2LQ5IW66OPoG3b9AI/fTr06gUjRsDeezuBTJIkSUmlSnDooWli7e23w8cfpw8RDz00DSqRlPuKVRwKIbQNIYwLIUwMIXRdxO23hBA+LPwaH0L4qchtc4rc9lwJZpdUSj77DI46Cpo1S58E3Xhjaj549NFQuXLW6SRJkpSLqlVL7QcmTYJu3eCFF2DzzdMU22++yTqdpH8S4hI2hIYQKgPjgdbAVGAYcFiMccxi7n860CzGeGzh9d9ijKsUN1BeXl4sKCgo7t0llaDvv4err07NpStVSuNKu3aF1VfPOpkkSZLKmq+/TgNMevaEmjVT8+pzznGyrZSVEMLwGGPeom4rzsqh7YGJMcbJMcaZQB+gwz/c/zDgiaWPKSkrf/wB116bxpHedhsceSRMmADXXWdhSJIkSctm3XXh7rvTZNu2beGKK2DTTdOxWbOyTiepqOIUhzYAvihyfWrhsb8JIdQD6gNDihyuEUIoCCG8F0LYfzGPO7HwPgXTp08vXnJJy232bPjvf9O0sYsvht13h5Ej4YEHoG7drNNJkiSpPNhsM3jqKXjvPWjcOG0za9IkHXOymZQbSrohdSegX4xxTpFj9QqXLR0O3BpCaLDwg2KMPWOMeTHGvDp16pRwJEkLixGefRa23hpOOAE22giGDoXnnksj6iVJkqSStsMO8PrrqRdRjRrQsWM6lp+fdTJJxSkOTQM2LHK9buGxRenEQlvKYozTCr9PBl4Hmi11Skkl5u23oUUL2H9/mDsX+veHd95JxyRJkqTSFALssw98+CE89BB89RX861/Qrl1awS4pG8UpDg0DGoYQ6ocQqpEKQH+bOhZCaAysAbxb5NgaIYTqhZdrA7sAi2xkLal0jR2bCkK77pomSNx3H4waBQcc4Fh6SZIkrViVK0OXLjB+PPToAe++C02bQufOMGVK1umkimeJxaEY42zgNOBlYCzQN8Y4OoTQPYTQvshdOwF94oLjzzYHCkIIHwH5wHWLm3ImqXRMm5a2jm25JQwZAlddBRMnwoknQpUqWaeTJElSRVazJpx/PkyenKaZPflk6lF03nlpkq6kFWOJo+xXNEfZSyXj55/h+uvh1ltT4+l//xsuuQRs6yVJkqRc9cUXcNll0KsXrLYaXHQRnHFGKiJJWj7LO8peUhkyYwbccksaS3/ttWnb2CefpCKRhSFJkiTlsg03TL2IPvoo9cTs2jVN1n3wQZgzZ8mPl7RsLA5J5cTcufDYY9CoEZxzDmy3HXzwAfTunQpFkiRJUlmx1Vbw/PNpulndunDccWnS7vPPp8m7kkqWxSGpjIsRXn4Ztt0WjjoK1lwTXnklfTVzNqAkSZLKsN13T82q+/WDWbOgffv5xySVHItDUhk2fDjsuSe0bZt6DPXuDQUF0Lp11skkSZKkkhECHHQQjB4N99yTJpztvDMceCCMG5d1Oql8sDgklUGTJsFhh0FeHowcCbfdlvoKHX44VPJftSRJksqhqlXh5JPT5N3u3WHwYNhiCzjpJPjqq6zTSWWbp5FSGfLtt2law+abw3PPwaWXpkLRGWdA9epZp5MkSZJK3yqrQLdu6X3wv/+dGlhvuml6b/zzz1mnk8omi0NSGfDbb+nTkQYN4O674dhj0ycmV16ZRnxKkiRJFc3aa8Ptt8PYsakX0dVXp/fLt92WJvhKKj6LQ1IOmzUr7avedFO4/PLUS2jUKLj3XlhvvazTSZIkSdlr0ACeeAKGDYNttoGzzkor7R9/PE30lbRkFoekHBRjmsiwxRZpqWzDhvDOO9C/PzRunHU6SZIkKffk5cGrr6ZJvrVqwRFHpGODB2edTMp9FoekHPPGG7DjjnDIIanp3nPPwdChsNNOWSeTJEmSclsI0KZNmur72GPw44/peps28MEHWaeTcpfFISlHfPwx7Lsv7LEHTJsGDzyQJpHtt196kZMkSZJUPJUqpZVDn3wCt9ySCkPbbZem+06enHU6KfdYHJIyNmUKHHNM2h/91ltw3XUwYUJqOl25ctbpJEmSpLKrevXUg2jSJLj4YhgwILVpOPNMmD4963RS7rA4JGXkxx/hggtgs81Ss7xzzkmfYlx4IdSsmXU6SZIkqfyoVStNM5swAbp0gTvvTI2sr7oKfv8963RS9iwOSSvYn3/CDTfAJpvAjTfCoYfC+PHp8pprZp1OkiRJKr822AB69kwTgFu1gm7d0mTg++6D2bOzTidlx+KQtILMmQMPPZRWCl1wQWow/eGH0KsX1KuXdTpJkiSp4th8c3jmmdTWYZNN4OST06Tg/v3T5GCporE4JJWyGOHFF6Fp09RHaL31YMgQGDgQtt4663SSJElSxbXLLqlANGBAamJ90EGw887w5ptZJ5NWLItDUgnp0QPy8xc8dvfdaS/zvvvCX39B377wv/9By5bZZJQkSZK0oBCgQ4c0Pfj++9PAmN12g/bt4dxz//4ePz8/vfeXyhOLQ1IJad4cOnZMLxbjxqUXlFNPTY2n77oLxoyBQw5xLL0kSZKUi6pUgeOPT02rr70W3ngDbrkF2rVLH/JCeq/fsWN67y+VJyHm2IbKvLy8WFBQkHUMaZm89hrst19aJRQjdO6cJiGsskrWySRJkiQtje+/TxPO7rgjNatu3RpGjEiFIncCqCwKIQyPMeYt6jZXDkklZPZsePTRNI0sRjj7bHj4YQtDkiRJUlm01lpw881pJdFmm8Hgwen7HntknUwqeRaHpBIwY0ZaXtqrF6y0Elx6aSoULbw/WZIkSVLZ8umn8MMPsN128M47qT/R3LlZp5JKlsUhaTn9/nvaSvbMM7DyyvDCC3DllWm56bweRJIkSZLKnnk9hvr2hWHDoFMneP55aNMGZs3KOp1UciwOScvhp5/SC8Nrr6Vm088/P3//ccuW819EJEmSJJU9w4bN7zEUAjzxRGpa/dpraez9X39lnVAqGTaklpbRt9+mwtCYMelF4qCDsk4kSZIkaUW45540mXiPPeDZZ2HVVbNOJC2ZDamlEjZlCrRoAePHp9VCFoYkSZKkiuOUU+CRR2DoUGjVKk02k8qyYhWHQghtQwjjQggTQwhdF3H7LSGEDwu/xocQfipyW+cQwoTCr84lmF3KxPjxsOuu8M03aWLBXntlnUiSJEnSinbkkdC/P4wcmVYQffVV1omkZbfE4lAIoTJwF7A30AQ4LITQpOh9YoxnxxibxhibAncA/QsfuyZwObADsD1weQhhjRL9CaQV6KOP0oqhv/5Kzel22SXrRJIkSZKy0r49DByYJprtumv6LpVFxVk5tD0wMcY4OcY4E+gDdPiH+x8GPFF4eS9gcIzxhxjjj8BgoO3yBJay8s476ROBatXgzTehWbOsE0mSJEnK2r/+lRpU//hj+iB57NisE0lLrzjFoQ2AL4pcn1p47G9CCPWA+sCQpX2slMtefRVat4bateGtt6BRo6wTSZIkScoVO+wAb7wBs2enAtHw4VknkpZOSTek7gT0izHOWZoHhRBODCEUhBAKpk+fXsKRpOXzzDOwzz6w6aZpxVC9elknkiRJkpRrttoqfZC8yirQsmVqVi2VFcUpDk0DNixyvW7hsUXpxPwtZcV+bIyxZ4wxL8aYV6dOnWJEklaMRx6BQw6BbbeF11+HddfNOpEkSZKkXLXppqlAtMEGaXDNSy9lnUgqnuIUh4YBDUMI9UMI1UgFoOcWvlMIoTGwBvBukcMvA21CCGsUNqJuU3hMynl33gmdO6c+Q4MHwxq2UpckSZK0BHXrplVDm2+eGlb37Zt1ImnJllgcijHOBk4jFXXGAn1jjKNDCN1DCO2L3LUT0CfGGIs89gfgSlKBaRjQvfCYlLNihKuvhtNPhw4d4IUX0tJQSZIkSSqOOnXSdOMdd4TDDoMHHsg6kfTPQpFaTk7Iy8uLBQUFWcdQBRUjXHgh3HADHHUUPPggVKmSdSpJkiRJZdEff8BBB8GgQXDTTXDOOVknUkUWQhgeY8xb1G0l3ZBaKrPmzIGTTkqFoVNPhYcftjAkSZIkadmttBI8+ywcfDCcey5cdln6QFrKNRaHJGDWLDjiCLj/frjkErjjDqjkvw5JkiRJy6laNejTB449Fq68Es46C+bOzTqVtCDXRajC+/PPNJHsxRehRw84//ysE0mSJEkqTypXhv/+F2rVgltugV9+SR9Mu1NBucKnoiq0X35JEwSGDoX77oMTT8w6kSRJkqTyKITUd2j11eHyy9O5yOOPQ/XqWSeTLA6pAvvuO9h7b/jwQ+jdO00RkCRJkqTSEkLqO1SrVtpett9+8MwzsPLKWSdTRWdXFVVIX34Ju+8Oo0alX8YWhiRJkiStKGeemSYjv/YatGkDP/2UdSJVdBaHVOFMngy77gpTpsBLL8G++2adSJIkSVJFc8wx0LcvDBsGLVvCt99mnUgVmcUhVSijR6fC0M8/w5AhsMceWSeSJEmSVFEddBA8/zyMGwctWsAXX2SdSBWVxSFVGMOGwW67pctDh0Lz5tnmkSRJkqS99oJXXoGvv04fZI8fn3UiVUQWh1QhvPEGtGqVGr+99RZssUXWiSRJkiQp2XVXeP11+OOPtIJo5MisE6misTikcu/FF6FtW9hwQ3jzTdhkk6wTSZIkSdKCmjVL5yvVqqXhOe++m3UiVSQWh1Su9ekD++8PW26ZVg9tsEHWiSRJkiRp0Ro3TjsdateGPfeEV1/NOpEqCotDKrd69oTDD4edd04jImvXzjqRJEmSJP2zevXSCqIGDWCffWDAgKwTqSKwOKRy6cYb4aSTYO+9YdAgWG21rBNJkiRJUvGsu27qQbTttnDwwfDoo1knUnlncUjlSoxw6aVw/vlw6KHwzDNQs2bWqSRJkiRp6ay5JgwenPoPHX003HVX1olUnlkcUrkxdy6ccQZcfTWccAL07p2auUmSJElSWbTKKmnATocOcNppcM016QNxqaRZHFK5MHs2dOkCd94J550H990HlStnnUqSJEmSlk+NGvDUU3DkkXDJJXDhhRaIVPKqZB1AWl4zZkCnTqlR21VXwcUXQwhZp5IkSZKkklG1KvTqlXqp3nAD/Pwz3H23H4ir5LhySGVOjx6Qn58u//Yb7LtvKgx16JAq6RaGJEmSJJU3lSqlnRIXX5wmM7duDbNmzb89Pz+dK0nLwuKQypzmzaFjR3juOWjTJo2pX3VVOPPMrJNJkiRJUukJIfVYPfHEVAxq0QL+/DNd7tgxnStJy8JtZSpzWraEe++FAw9Me21XXTWtHGrZMutkkiRJklT67rsPVl4ZbrkFGjeG339PfYk8J9KycuWQypzPP4eLLkpV87lz04ohfwlKkiRJqkhuvhkOOACmTElTmrfeOutEKsssDqlMGTcuLZ388ss01rFbN7jnnvk9iCRJkiSpIsjPhzffhEMPha++gu22S+dJ0rKwOKQy48MPU2Ho119TZbx/f+jeHfr2TftrLRBJkiRJqgjm9Rjq2xf69EmriD7/PBWIJk/OOp3KIotDKhPeeQf22ANq1IDjj4enn56/laxly/RLcdiwTCNKkiRJ0goxbFg6B5p3TnT22XDXXWnEfYsWMGZMtvlU9oQY45LvFEJb4DagMvDfGON1i7hPR+AKIAIfxRgPLzw+B/i48G5TYozt/+nvysvLiwUFBUvzM6icGzwY9t8f6tZNlzfaKOtEkiRJkpR7Ro1KE51nzoRBgyAvL+tEyiUhhOExxkU+K5a4ciiEUBm4C9gbaAIcFkJostB9GgIXAbvEGLcAzipy858xxqaFX/9YGJJ69Fhwe1j//tCuHdSqBUOHWhiSJEmSpMXZcsvUh2juXNhtN3jjjfm35een8y1pUYqzrWx7YGKMcXKMcSbQB+iw0H1OAO6KMf4IEGP8tmRjqqJo3nx+/6BeveDgg9Pxe++FddbJNpskSZIk5boGDdL508yZ0Lo1DBw4v0dR8+ZZp1OuqlKM+2wAfFHk+lRgh4XusxlACOFt0tazK2KMgwpvqxFCKABmA9fFGAcsV2KVa/P6B+23H/z+O1StCgMGpNVDkiRJkqQl69gxDfE55BDYd9806fnZZ+f3KJIWVlINqasADYE9gMOA+0MIqxfeVq9wT9vhwK0hhAYLPziEcGIIoSCEUDB9+vQSiqSyKEZ4661UGAI47zwLQ5IkSZK0tPbfH845J51j/forTJyYdSLlsuIUh6YBGxa5XrfwWFFTgedijLNijJ8C40nFImKM0wq/TwZeB5ot/BfEGHvGGPNijHl16tRZ6h9C5UOMcP75cNllUL06XHIJ3H+/I+olSZIkaWnl58ODD0LXrmkV0Yknwo03Zp1Kuao4xaFhQMMQQv0QQjWgE/DcQvcZQFo1RAihNmmb2eQQwhohhOpFju8COFRPfzNnDpxwAtx0UxpX/+KLcNVVaYvZvB5EkiRJkqQlm9djqG9fuPZaeP759AH8+edDt27pg3mpqCUWh2KMs4HTgJeBsUDfGOPoEEL3EMK86WMvA9+HEMYA+cD5Mcbvgc2BghDCR4XHr4sxWhzSAmbOhMMPhwcegFatUmGoVat027weRMOGZZtRkiRJksqKYcPSedS8HkNt2sALL6SG1FddBWeemSaaSfOEmGMlw7y8vFhQUJB1DK0gf/yRJpK99FJa4njuuVknkiRJkqTyaV4rj5tugqOPTh/QVynOmCqVCyGE4YU9of/Gp4Ey88svqXP+W29Bz55pW5kkSZIkqXSEADfcAGusAZdems7J+vRJW85UsVkcUia++w7atoWPPoInnoBDD806kSRJkiSVfyGk4T+rrQZnnJE+sB8wAFZeOetkylJJjbKXim3aNNhtNxg9Gp591sKQJEmSJK1op58OvXrBkCHQujX8+GPWiZQli0NaoSZNgl13halTYdAgaNcu60SSJEmSVDEdfTT06wfDh6fm1d98k3UiZcXikFaYUaNSYejXX1N1evfds04kSZIkSRXbAQekSWYTJkCLFjBlStaJlAWLQ1oh3n8/FYMqVYKhQyFvkf3RJUmSJEkrWuvWMHgwfPtt+kB/3LisE2lFszikUpefD61aweqrp8lkTZpknUiSJEmSVNTOO8Prr8OMGWkF0YcfZp1IK5LFIZWq55+HvfeGevXgzTehfv2sE0mSJEmSFqVp03TeVqMG7LEHvPNO1om0olgcUql54gk48EDYait44w1Yf/2sE0mSJEmS/slmm6UdH2uvPX+7mco/i0MqFffeC0ccAbvsAq+9BmutlXUiSZIkSVJxbLRRWkHUsCHsuy/07591IpU2i0MqcddfD6ecAvvsAy+9BKutlnUiSZIkSdLSWGed1D92u+3gkEOgV6+sE6k0WRxSiYkRLr4YunaFTp1SdblmzaxTSZIkSZKWxRprwCuvwL/+BV26wB13ZJ1IpcXikErE3Llw2mlw7bVw0knw2GNQtWrWqSRJkiRJy2OVVeCFF+CAA+CMM+Cqq9LCAJUvFoe03GbNgs6d4e674YIL4J57oHLlrFNJkiRJkkpC9erQty8cfTR06wbnn2+BqLypknUAlW1//ZW2kD37LFxzTdpSFkLWqSRJkiRJJalKFXjoIahVC266CX7+OQ0icmFA+WBxSMvst9+gQwcYMgTuugv+/e+sE0mSJEmSSkulSnDbbalAdNVV8Msv8OijUK1a1sm0vCwOaZn88AO0awcFBemXwZFHZp1IkiRJklTaQoArr0wFovPPh19/hX79YKWVsk6m5WHPIS21r7+GPfaAESPSLwELQ5IkSZJUsZx3HvTsCYMGwd57p1VEKrssDmmpfP45tGgBkyfDwIGw//5ZJ5IkSZIkZeGEE+CJJ+Cdd9K4++++yzqRlpXFIRXbJ5/Arrumf/CDB0OrVlknkiRJkiRl6dBD04Ci0aNht91g2rSsE2lZWBxSsYwYkf6hz5oFb7wBO+2UdSJJkiRJUi5o1y5tL5s6NS0omDQp60RaWhaHtERvvZV6DNWsCW++CVtvnXUiSZIkSVIu2X33NMn6119TK5JRo7JOpKVhcUj/6OWXoU0bWG+9VCRq2DDrRJIkSZKkXJSXB0OHpolmu+8O77+fdSIVl8UhLVa/frDfftCoUfoHvuGGWSeSJEmSJOWyJk3SwoLVV099avPzs06k4rA4pEV66KHUWGz77dM/5rXXzjqRJEmSJKksqF8/tSSpVy+NuX/++awTaUmKVRwKIbQNIYwLIUwMIXRdzH06hhDGhBBGhxAeL3K8cwhhQuFX55IKrtJz221w7LGw555pW9nqq2edSJIkSZJUlqy/fhpmtNVWcOCBaeS9cleVJd0hhFAZuAtoDUwFhoUQnosxjilyn4bARcAuMcYfQwhrFx5fE7gcyAMiMLzwsT+W/I+i5RUjdO8OV1wBBx0EvXtD9epZp5IkSZIklUVrrQWvvQbt28MRR8Avv8BJJ2WdSotSnJVD2wMTY4yTY4wzgT5Ah4XucwJw17yiT4zx28LjewGDY4w/FN42GGhbMtG1PHr0WHDvZ4xwyCGpMNSlC/TpY2FIkiRJkrR8VlsNXnoJ9tkHTj7578Wh/Px0fqpsFac4tAHwRZHrUwuPFbUZsFkI4e0QwnshhLZL8VhloHlz6Ngx/UOcMyf9Q3366bTc74EHoMoS15RJkiRJkrRkNWtC//7QsiX07JlWEcWYzkc7dkznp8pWSZUAqgANgT2AusDQEMJWxX1wCOFE4ESAjTbaqIQi6Z+0bAl9+6bVQmuvDWPHwtFHw8MPp7GDkiRJkiSVlKpVYfBg2H9/ePxxGDcOPv88nZe2bJl1OhVn5dA0oOgQ87qFx4qaCjwXY5wVY/wUGE8qFhXnscQYe8YY82KMeXXq1Fma/FpG332XqrS//ZYKQ61bQ69eFoYkSZIkSaWjcmV47jnYaScYPhz+/BOGDUu9iJSt4hSHhgENQwj1QwjVgE7AcwvdZwBp1RAhhNqkbWaTgZeBNiGENUIIawBtCo8pI198AWedlUYKXnllWsp33HEwYsSCPYgkSZIkSSppr78OEybAUUfBzJlw4YXp/LRbN5g+Pet0FdcSi0MxxtnAaaSizligb4xxdAihewihfeHdXga+DyGMAfKB82OM38cYfwCuJBWYhgHdC49pBRs/Ho4/Hho0gDvvhF13hTXWgEGD4L//TUv55vUgkiRJkiSppM3rMdS3LzzyCLz8Mqy+ehp3f9VVqUh01llpUYNWrBBjzDrDAvLy8mJBQUHWMcqNESPg2muhX780fez44+G88+DJJ1PTr6J7O/Pz05K+Cy7ILq8kSZIkqXzq0WPx56H77QfXXw+9e6d2J0cdlVYVbbZZdnnLmxDC8Bhj3iJvszhUPr35JlxzTVoZtNpqcOqpcOaZsM46WSeTJEmSJGnRPv8cbrwx7XCZMQMOOgguugi23TbrZGXfPxWHitNzSGVEjPDii2nL2G67pQZf11wDU6ak7xaGJEmSJEm5rF49uOOOVCTq2hVeeQW22w7atoWhQ9N5r0qexaFyYM4c6NMHmjWDffdN+zPvuAM++yxVWGvVyjqhJEmSJEnFt/ba8xc7XHstfPAB7L57WgzxwgsWiUqaxaEybMYMuP9+aNQIDjssXX/4YZg4EU47DVZaKeuEkiRJkiQtu1q10gqizz9Pw5WmTk39iZo2hSeegNmzs05YPlgcKoN++w1uugk22QROPDFNHevfH0aPhs6doWrVrBNKkiRJklRyatZMvXQnToRevWDWLDj88LRYomfPtFhCy87iUBny/fdwxRVpD+Z550HjxjB4MLz/PhxwAFTy/6YkSZIkqRyrWhWOPhpGjUqLJNZaC046CerXT4sofvst64Rlk+WEMmDaNDj33FQU+s9/oEULeO89eO012HPPNOZPkiRJkqSKolKltEjif/9LiyY23zwtothoo7So4vvvs05YtlgcymETJ6ZtY5tsArfdlp74H38MAwbADjtknU6SJEmSpGyFkBZNvPZaWkSx225pUUW9enDOOWmxhZbM4lAO+uij1GC6USN45BE47jiYMAEefRS23DLrdJIkSZIk5Z4ddkiLKUaNSosrbr89bTc74YR0Tq3FsziUQ95+O42ib9oUXnwxLYn77DO4++70hJYkSZIkSf9siy3S4ooJE+D449Plxo2hUyf48MOs0+Umi0MZixEGDUpL33bdNe2XvPLKNKbv+uth3XWzTihJkiRJUtlTv35abPHZZ3D++TBwIDRrBvvsA2+9lXW63GJxKCNz5kDfvrDddrD33vDpp6mv0GefwaWXpvH0kiRJkiRp+ay7Llx3HUyZAlddlSZ+t2iRvl56KS3aqOgsDq1gM2fCAw+kTuqHHgp//AEPPgiTJsEZZ8DKK2edUJIkSZKk8mf11eGSS9JOndtuS9/btYNtt02LN+bMyTphdiwOlbAePSA/f8Fj+fmpOnnrrdCgQdrzuOqq8NRTMHo0HHMMVKuWSVxJkiRJkiqUlVZKizMmTkyLNf78My3e2HzztJhj5szFn9v36JFN5tJmcaiENW8OHTvOfxI991xqMn3DDXD22ak49PLLUFAABx8MlStnm1eSJEmSpIqoWrW0WGP0aOjXLy3iOP542GST1PLlkEPmn9vn56dz/ebNM41cakLMsc11eXl5saCgIOsYyyU/PxV+GjWCd99Nx/bdFy66CHbeOdtskiRJkiTp72KEwYPhmmvgjTdgtdVg9mz497/h4YfT1rOWLbNOuexCCMNjjHmLus2VQ6WgZUvYcMNUGNpiC/joI3j+eQtDkiRJkiTlqhCgTRt4/XV4++00VfyPP+DGG+GUU8p2YWhJLA6Vgvx8+OILOO00+OYb+P77rBNJkiRJkqTi2nlnOOecNEn8nHPgnnv+3oOoPLE4VMLm7UPs1w/uuCMtOyvag0iSJEmSJOW2eef2Tz8NN91U/s/tLQ6VsGHDFtyH2LJluj5sWLa5JEmSJElS8VS0c3sbUkuSJEmSJJVzNqSWJEmSJEnSIlkckiRJkiRJqsAsDkmSJEmSJFVgFockSZIkSZIqMItDkiRJkiRJFZjFIUmSJEmSpArM4pAkSZIkSVIFZnFIkiRJkiSpAgsxxqwzLCCEMB34POscJaQ28F3WIaR/4HNUuc7nqHKdz1GVBT5Plet8jirXlZfnaL0YY51F3ZBzxaHyJIRQEGPMyzqHtDg+R5XrfI4q1/kcVVng81S5zueocl1FeI66rUySJEmSJKkCszgkSZIkSZJUgVkcKl09sw4gLYHPUeU6n6PKdT5HVRb4PFWu8zmqXFfun6P2HJIkSZIkSarAXDkkSZIkSZJUgVkcKiUhhLYhhHEhhIkhhK5Z55GKCiFsGELIDyGMCSGMDiGcmXUmaVFCCJVDCCNCCC9knUVaWAhh9RBCvxDCJyGEsSGEnbLOJBUVQji78HV+VAjhiRBCjawzqWILITwYQvg2hDCqyLE1QwiDQwgTCr+vkWVGVWyLeY7eUPhaPzKE8EwIYfUMI5Yai0OlIIRQGbgL2BtoAhwWQmiSbSppAbOBc2OMTYAdgVN9jipHnQmMzTqEtBi3AYNijI2BbfC5qhwSQtgAOAPIizFuCVQGOmWbSuJhoO1Cx7oCr8UYGwKvFV6XsvIwf3+ODga2jDFuDYwHLlrRoVYEi0OlY3tgYoxxcoxxJtAH6JBxJun/xRi/ijF+UHj5V9IJzQbZppIWFEKoC+wD/DfrLNLCQgi1gN2ABwBijDNjjD9lGkr6uypAzRBCFWAl4MuM86iCizEOBX5Y6HAHoFfh5V7A/isyk1TUop6jMcZXYoyzC6++B9Rd4cFWAItDpWMD4Isi16fiibdyVAhhY6AZ8L+Mo0gLuxW4AJibcQ5pUeoD04GHCrc+/jeEsHLWoaR5YozTgBuBKcBXwM8xxleyTSUt0joxxq8KL38NrJNlGGkJjgVeyjpEabA4JFVgIYRVgKeBs2KMv2SdR5onhLAv8G2McXjWWaTFqAJsC9wTY2wG/I5bIZRDCvu2dCAVMtcHVg4hHJltKumfxTRK23HaykkhhEtI7Tl6Z52lNFgcKh3TgA2LXK9beEzKGSGEqqTCUO8YY/+s80gL2QVoH0L4jLQ1918hhMeyjSQtYCowNcY4b9VlP1KxSMoVewKfxhinxxhnAf2BnTPOJC3KNyGE9QAKv3+bcR7pb0IIXYB9gSMKi5jljsWh0jEMaBhCqB9CqEZq/vdcxpmk/xdCCKQ+GWNjjDdnnUdaWIzxohhj3RjjxqTfoUNijH7irZwRY/wa+CKE0KjwUCtgTIaRpIVNAXYMIaxU+LrfCpumKzc9B3QuvNwZeDbDLNLfhBDaklodtI8x/pF1ntJicagUFDarOg14mfQi3DfGODrbVNICdgGOIq3G+LDwq13WoSSpjDkd6B1CGAk0Ba7JNo40X+Gqtn7AB8DHpPf9PTMNpQovhPAE8C7QKIQwNYRwHHAd0DqEMIG04u26LDOqYlvMc/ROYFVgcOF5072ZhiwloZyuiJIkSZIkSVIxuHJIkiRJkiSpArM4JEmSJEmSVIFZHJIkSZIkSarALA5JkiRJkiRVYBaHJEmSJEmSKjCLQ5IkSZIkSRWYxSFJkiRJkqQKzOKQJEmSJElSBfZ/qylDPLwQ/dsAAAAASUVORK5CYII=\n",
+                        "text/plain": [
+                            "<Figure size 1440x360 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "# Plot 2nd order dispersion\n",
+                "\n",
+                "pos = [0.00, 0.50, 0.95, 1.05, 1.50, 4.50, 4.95, 5.05, 5.50, 6.00, 6.50, 6.95, 7.05, 7.50, 10.50, 10.95, 11.05, 11.50, 12.00]\n",
+                "res = torch.stack([series((4, 1), (0, 2), jet)[(0, 0, 0, 0, 2)][0] for jet in out])\n",
+                "\n",
+                "plt.figure(figsize=(20, 5))\n",
+                "plt.plot(pos, res.cpu().numpy(), marker='x', color='blue')\n",
+                "plt.show()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "a85452e8-6cfb-47ef-a434-366de354b268",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
+                "# Example-12: Closed orbit (quadrupole shift)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "ad32fff3-f3da-4bd0-80e5-6ae33b617a50",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.evaluate import compare\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "torch.set_printoptions(precision=6, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "02473f42-5b53-48d1-a478-9e3e1e4d04e9",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "5af703e0-68ed-4dec-a1d4-496aaea2c8cb",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "1d3cb9e4-34ec-46f6-8215-e21743c55323",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, d): \n",
+                "    dxf, dyf, dxd, dyd = d\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    x = slip(x, -dxf, -dyf)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxd, +dyd)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = slip(x, -dxd, -dyd)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxf, +dyf)\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, d):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, d)\n",
+                "    return x"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "b421fbd5-6d20-4531-b0ed-54fa3270fb49",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "fp = fixed_point(16, fodo, x, d, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "bb5b15aa-cf71-4b90-aee5-41b63c29f504",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[-4.621551e-01, 0.000000e+00, 1.165780e+00, 0.000000e+00],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                            "          [0.000000e+00, 3.344042e+00, 0.000000e+00, -4.891066e+00],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute parametric fixed point\n",
+                "\n",
+                "pfp = parametric_fixed_point((1, ), fp, [d], fodo)\n",
+                "chop(pfp)\n",
+                "pfp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "4ec9581a-17f5-46eb-8d17-9d500befb801",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[-4.621551e-01, 0.000000e+00, 1.165780e+00, 0.000000e+00],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                            "          [0.000000e+00, 3.344042e+00, 0.000000e+00, -4.891066e+00],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Propagate parametric fixed point\n",
+                "\n",
+                "out = propagate((4, 4), (0, 1), pfp, [d], fodo)\n",
+                "chop(out)\n",
+                "out"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "5b83a5e1-dbcc-4468-a52b-94aa952c1ef2",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-8.428998e-04, 0.000000e+00, -7.200015e-03, 0.000000e+00], dtype=torch.float64)\n",
+                        "tensor([-8.428998e-04, 0.000000e+00, -7.200015e-03, 0.000000e+00], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Test single random shift\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = 1.0E-3*torch.randn_like(x)\n",
+                "\n",
+                "fp = fixed_point(64, fodo, x, d, power=1, epsilon=1.0E-9)\n",
+                "chop([fp])\n",
+                "\n",
+                "print(fp)\n",
+                "print(evaluate(pfp, [x, d]))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "2f0ebe1d-d86c-454f-ad59-86802a0f58d9",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-2.280223e-05,  0.000000e+00, -3.266640e-05,  0.000000e+00], dtype=torch.float64)\n",
+                        "tensor([1.267704e-03, 0.000000e+00, 5.887239e-03, 0.000000e+00], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Estimate center & spread (tracking)\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = 1.0E-3*torch.randn(8192, 4, dtype=dtype, device=device)\n",
+                "\n",
+                "fp = torch.func.vmap(lambda d: fixed_point(64, fodo, x, d, power=1))(d)\n",
+                "chop([fp])\n",
+                "\n",
+                "print(fp.T.mean(-1))\n",
+                "print(fp.T.std(-1))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "3838c50a-21c7-4a2c-8220-641697a0a905",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-2.510959e-05,  0.000000e+00, -1.240353e-05,  0.000000e+00], dtype=torch.float64)\n",
+                        "tensor([1.260521e-03, 0.000000e+00, 5.920052e-03, 0.000000e+00], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Estimate center & spread (surrogate)\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = 1.0E-3*torch.randn(8192, 4, dtype=dtype, device=device)\n",
+                "\n",
+                "fp = torch.func.vmap(lambda d: evaluate(pfp, [x, d]))(d)\n",
+                "chop([fp])\n",
+                "\n",
+                "print(fp.T.mean(-1))\n",
+                "print(fp.T.std(-1))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "7d4d5f58-b78d-4632-af6d-0955ec51b2c7",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([1.254045e-03, 0.000000e+00, 5.924960e-03, 0.000000e+00], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Estimate spread (error propagation)\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "s = derivative(1, lambda d: evaluate(pfp, [x, d]), d, intermediate=False)\n",
+                "\n",
+                "print((s @ (1.0E-3*torch.eye(4,  dtype=dtype, device=device))**2 @ s.T).diag().sqrt())"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "8eed591e-97f4-4c13-a53b-fc4fb0736995",
+            "metadata": {},
+            "source": [
+                "# Example-13: Closed orbit (sextupole shift)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "e8c85315-a67e-4f13-ad35-8e2136f6b6d1",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.evaluate import compare\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "torch.set_printoptions(precision=6, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "d6b913f4-e7ee-4410-8a97-cf1ac9f52a15",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "3ae4b140-8589-4973-b6f8-d588ecbc8316",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "f22acc90-000b-4e94-baca-a613df54181e",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, d):\n",
+                "    dxsf1, dysf1, dxsd1, dysd1, dxsf2, dysf2, dxsd2, dysd2 = d\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxsf1, +dysf1)\n",
+                "    x = sext(x, [0.0], 0.50, 0.10)\n",
+                "    x = slip(x, -dxsf1, -dysf1)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxsd1, +dysd1)\n",
+                "    x = sext(x, [0.0], -0.50, 0.10)\n",
+                "    x = slip(x, -dxsd1, -dysd1)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxsd2, +dysd2)\n",
+                "    x = sext(x, [0.0], -0.50, 0.10)\n",
+                "    x = slip(x, -dxsd2, -dysd2)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxsf2, +dysf2)\n",
+                "    x = sext(x, [0.0], 0.50, 0.10)\n",
+                "    x = slip(x, -dxsf2, -dysf2)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, d):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, d)\n",
+                "    return x"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "56b58c71-f4ae-44e4-b818-6ba412efb93a",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = torch.tensor([0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "fp = fixed_point(16, fodo, x, d, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "f6fb2e38-d269-4a4f-bf38-31c9de7a887e",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute & check parametric fixed point\n",
+                "# Note, there is no first order contribution from sextupole shifts\n",
+                "\n",
+                "pfp = parametric_fixed_point((2, ), fp, [d], fodo)\n",
+                "out = propagate((4, 8), (0, 2), pfp, [d], fodo)\n",
+                "print(compare(pfp, out))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "f4411bab-734c-45a2-8bbc-0dfaee9d8407",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-5.256659e-07, -4.918902e-08, -2.067269e-06, -5.124183e-08], dtype=torch.float64)\n",
+                        "tensor([-5.246926e-07, -4.909385e-08, -2.075087e-06, -5.138894e-08], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Test for a random shift\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = 1.0E-3*torch.randn(8, dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(64, fodo, x, d, power=1, epsilon=1.0E-9)\n",
+                "\n",
+                "print(fp)\n",
+                "print(evaluate(pfp, [x, d]))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "3cac879f-551a-4ec5-9bf5-d7922d316f06",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-8.407849e-09, -3.266832e-11,  3.976001e-08, -1.611143e-10], dtype=torch.float64)\n",
+                        "tensor([6.868134e-07, 3.121643e-08, 1.807462e-06, 2.967522e-08], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Estimate center & spread (tracking)\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = 1.0E-3*torch.randn(8192, 8, dtype=dtype, device=device)\n",
+                "\n",
+                "fp = torch.func.vmap(lambda d: fixed_point(64, fodo, x, d, power=1))(d)\n",
+                "chop([fp])\n",
+                "\n",
+                "print(fp.T.mean(-1))\n",
+                "print(fp.T.std(-1))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "757522a2-5e28-4141-9e33-29f34fa63c7d",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.156708e-09, 2.567181e-11, 3.218317e-09, 7.290918e-11], dtype=torch.float64)\n",
+                        "tensor([6.811972e-07, 3.105100e-08, 1.816353e-06, 2.926991e-08], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Estimate center & spread (surrogate)\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = 1.0E-3*torch.randn(8192, 8, dtype=dtype, device=device)\n",
+                "\n",
+                "fp = torch.func.vmap(lambda d: evaluate(pfp, [x, d]))(d)\n",
+                "chop([fp])\n",
+                "\n",
+                "print(fp.T.mean(-1))\n",
+                "print(fp.T.std(-1))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "81d75dce-4460-47cb-aa13-7f87d0fe0d05",
+            "metadata": {},
+            "source": [
+                "# Example-14: Closed orbit (responce matrix & correction)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "2583e9ab-5501-4f49-b395-f59e9f4c73e7",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# In this example orbit responce matrix is computed\n",
+                "# Quadrupole shifts are introduced and responce matrix is used to correct the orbit at observation locations\n",
+                "\n",
+                "# Correctors are at sextupole centers\n",
+                "# Observation points are at bend centers"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "b0a8970a-837c-4af3-8417-4615d2071ad6",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.evaluate import compare\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "torch.set_printoptions(precision=6, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "b6a506da-4f29-4794-ba37-0e5392536963",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "da6570f1-8968-455a-9938-b797b1821a3a",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=25):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "b17fe3a9-6c67-43f0-bf2b-42ac0a8eb7ee",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, c, d): \n",
+                "    cxsf1, cxsd1, cxsf2, cxsd2, cysf1, cysd1, cysf2, cysd2 = c\n",
+                "    dxf, dyf, dxd, dyd = d\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    x = slip(x, -dxf, -dyf)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = kick(x, cxsf1, cysf1)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 1.5)\n",
+                "    return x\n",
+                "\n",
+                "def map_02_03(x, c, d):\n",
+                "    cxsf1, cxsd1, cxsf2, cxsd2, cysf1, cysd1, cysf2, cysd2 = c\n",
+                "    dxf, dyf, dxd, dyd = d\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 1.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = kick(x, cxsd1, cysd1)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxd, +dyd)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = slip(x, -dxd, -dyd)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = kick(x, cxsd2, cysd2)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 1.5)\n",
+                "    return x\n",
+                "\n",
+                "def map_03_04(x, c, d):\n",
+                "    cxsf1, cxsd1, cxsf2, cxsd2, cysf1, cysd1, cysf2, cysd2 = c\n",
+                "    dxf, dyf, dxd, dyd = d\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 1.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = kick(x, cxsf2, cysf2)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxf, +dyf)\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02,\n",
+                "    map_02_03,\n",
+                "    map_03_04\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, c, d):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, c, d)\n",
+                "    return x\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "c = torch.tensor(8*[0.0], dtype=dtype, device=device)\n",
+                "d = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "print(fodo(x, c, d))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "0e69337a-c507-4471-962e-5f69dfb2b8c3",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "c = torch.tensor(8*[0.0], dtype=dtype, device=device)\n",
+                "d = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, c, d, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "02f19aad-3b9c-4497-a4d3-935bbb6b89da",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[7.583253e+00, 5.939607e+00, 7.583253e+00, 5.939607e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                            "          [-4.334732e-01, -9.086786e-02, 4.334732e-01, 9.086786e-02, 0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 1.349234e+01, 2.165892e+01, 1.349234e+01, 2.165892e+01],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, -4.019148e-01, -7.725758e-02, 4.019148e-01, 7.725758e-02]],\n",
+                            "         dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute parametric fixed point\n",
+                "\n",
+                "pfp = parametric_fixed_point((1, ), fp, [c], fodo, d)\n",
+                "chop(pfp)\n",
+                "pfp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "63760982-d712-4ce6-ad69-055c1ce8678b",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[7.583253e+00, 5.939607e+00, 7.583253e+00, 5.939607e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                            "          [-4.334732e-01, -9.086786e-02, 4.334732e-01, 9.086786e-02, 0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 1.349234e+01, 2.165892e+01, 1.349234e+01, 2.165892e+01],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, -4.019148e-01, -7.725758e-02, 4.019148e-01, 7.725758e-02]],\n",
+                            "         dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Propagate parametric fixed point\n",
+                "\n",
+                "out = propagate((4, 8), (0, 1), pfp, [c], fodo, d)\n",
+                "chop(out)\n",
+                "out"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "f4dd52aa-5eda-4910-962e-d84e18589062",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Orbit derivatives at observation locations\n",
+                "\n",
+                "bag = []\n",
+                "\n",
+                "pfp = propagate((4, 8), (0, 1), pfp, [c], map_01_02, d)\n",
+                "chop(pfp)\n",
+                "bag.append(pfp)\n",
+                "\n",
+                "pfp = propagate((4, 8), (0, 1), pfp, [c], map_02_03, d)\n",
+                "chop(pfp)\n",
+                "bag.append(pfp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "61afd3e6-b21c-4fcb-aceb-d5ea5552fe66",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([[6.221115e+00, 4.042085e+00, 6.753998e+00, 4.569069e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                        "        [6.753998e+00, 4.569069e+00, 6.221115e+00, 4.042085e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                        "        [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 1.808222e+01, 2.754871e+01, 1.855563e+01, 2.802741e+01],\n",
+                        "        [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 1.855563e+01, 2.802741e+01, 1.808222e+01, 2.754871e+01]],\n",
+                        "       dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute responce matrix\n",
+                "\n",
+                "def orbit(c, pfp):\n",
+                "    qx, _, qy, _ = evaluate(pfp, [x, c]) \n",
+                "    return torch.stack([qx, qy])\n",
+                "\n",
+                "pfp1, pfp2 = bag\n",
+                "\n",
+                "rx1, ry1 = derivative(1, orbit, c, pfp1, intermediate=False)\n",
+                "rx2, ry2 = derivative(1, orbit, c, pfp2, intermediate=False)\n",
+                "\n",
+                "rm = torch.stack([rx1, rx2, ry1, ry2])\n",
+                "print(rm)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "99e550ce-9345-4582-9ee2-f6d39bd4e237",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-2.161122e-03, -2.161122e-03, -3.001730e-03, -3.001730e-03], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Generate perturbed orbit\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "c = torch.tensor(8*[0.0], dtype=dtype, device=device)\n",
+                "d = torch.tensor([0.001, 0.001, -0.001, 0.001], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, c, d, power=1)\n",
+                "\n",
+                "qx1, _, qy1, _ = map_01_02(fp, c, d)\n",
+                "qx2, _, qy2, _ = map_02_03(map_01_02(fp, c, d), c, d)\n",
+                "\n",
+                "o = torch.stack([qx1, qx2, qy1, qy2])\n",
+                "chop([o])\n",
+                "print(o)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "1394e6ef-4c84-435a-bbce-82b035466e8c",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Correct orbit\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "c = - (torch.linalg.pinv(rm) @ o)\n",
+                "d = torch.tensor([0.001, 0.001, -0.001, 0.001], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, c, d, power=1)\n",
+                "\n",
+                "qx1, _, qy1, _ = map_01_02(fp, c, d)\n",
+                "qx2, _, qy2, _ = map_02_03(map_01_02(fp, c, d), c, d)\n",
+                "\n",
+                "o = torch.stack([qx1, qx2, qy1, qy2])\n",
+                "chop([o])\n",
+                "print(o)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "0e23c026-350b-4d62-82e1-5ddbb49f4573",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
+                "# Example-15: Tune (chromaticity)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "0d6f923d-601e-4736-b214-8e2df57d5918",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "False\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "from twiss.twiss import twiss\n",
+                "\n",
+                "torch.set_printoptions(precision=6, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "e8ef0143-3b64-4487-8a4d-73ef78b0c491",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "1942acce-37c9-4b5c-80e6-9fbd0573816e",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "a69d84a9-7376-4ed6-b669-cd34e56abe50",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, w, k):\n",
+                "    ksf, ksd, ksb = k\n",
+                "    x = quad(x, w, 0.19, 0.50)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = sext(x, w, ksf, 0.10)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = bend(x, w, 22.92, 0.015, ksb, 3.0)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = sext(x, w, ksd, 0.10)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = quad(x, w, -0.21, 0.50)\n",
+                "    x = quad(x, w, -0.21, 0.50)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = sext(x, w, ksd, 0.10)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = bend(x, w, 22.92, 0.015, ksb, 3.0)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = sext(x, w, ksf, 0.10)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = quad(x, w, 0.19, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, d, k):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, d, k)\n",
+                "    return x\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "w = torch.tensor(1*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "print(fodo(x, w, k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "1c148092-c7ba-41b3-b2de-4f0027d02a0e",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "w = torch.tensor(1*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, w, k, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "f5ac8f74-78ac-437d-b5d0-35f7ac1b16a9",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "   tensor([[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]], dtype=torch.float64)],\n",
+                            "  [tensor([[1.816134e+00],\n",
+                            "           [0.000000e+00],\n",
+                            "           [0.000000e+00],\n",
+                            "           [0.000000e+00]], dtype=torch.float64),\n",
+                            "   tensor([[[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]],\n",
+                            "   \n",
+                            "           [[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]],\n",
+                            "   \n",
+                            "           [[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]],\n",
+                            "   \n",
+                            "           [[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]]], dtype=torch.float64)]]]"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute parametric fixed point\n",
+                "\n",
+                "pfp = parametric_fixed_point((1, 1), fp, [w, k], fodo)\n",
+                "chop(pfp)\n",
+                "pfp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "e47fbd61-c250-4f37-8c2c-92d4fe55e6bd",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "   tensor([[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]], dtype=torch.float64)],\n",
+                            "  [tensor([[1.816134e+00],\n",
+                            "           [0.000000e+00],\n",
+                            "           [0.000000e+00],\n",
+                            "           [0.000000e+00]], dtype=torch.float64),\n",
+                            "   tensor([[[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]],\n",
+                            "   \n",
+                            "           [[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]],\n",
+                            "   \n",
+                            "           [[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]],\n",
+                            "   \n",
+                            "           [[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]]], dtype=torch.float64)]]]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Propagate parametric fixed point\n",
+                "\n",
+                "out = propagate((4, 1, 3), (0, 1, 1), pfp, [w, k], fodo)\n",
+                "chop(out)\n",
+                "out"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "d4d080e8-ec1e-41fa-ad29-6c8bddfba185",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Propagate parametric identity (surrogate model for linear dynamics)\n",
+                "\n",
+                "jet = identity((1, 1, 1), fp, parametric=pfp)\n",
+                "jet = propagate((4, 1, 3), (1, 1, 1), jet, [w, k], fodo)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "d64e48f0-a136-478f-99cb-2a0dc8face2c",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute tune\n",
+                "\n",
+                "def tune(w, k):\n",
+                "    m = derivative(1, lambda x: evaluate(jet, [x, w, k]), fp, intermediate=False)\n",
+                "    t, *_ = twiss(m)\n",
+                "    return t\n",
+                "\n",
+                "print(tune(w, k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "3cc1098c-ef11-4ecb-9f21-7f5f71634db2",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[[tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64), tensor([[0., 0., 0.],\n",
+                        "        [0., 0., 0.]], dtype=torch.float64)], [tensor([[-2.343079e-01],\n",
+                        "        [-2.416176e-01]], dtype=torch.float64), tensor([[[3.618782e-01],\n",
+                        "         [8.705079e-02],\n",
+                        "         [5.873074e+00]],\n",
+                        "\n",
+                        "        [[-2.986097e-01],\n",
+                        "         [-4.727344e-01],\n",
+                        "         [-1.106560e+01]]], dtype=torch.float64)]]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute parametric tune\n",
+                "\n",
+                "t = derivative((1, 1), tune, w, k)\n",
+                "\n",
+                "print(t)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "02dd6a3f-856e-44a1-a736-a51279aa6721",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n",
+                        "tensor([2.525452e-01, 1.196688e-01], dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([2.525452e-01, 1.196687e-01], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Check convergence\n",
+                "\n",
+                "print(evaluate(t, [w, k]))\n",
+                "print(evaluate(t, [w + 1.0E-3, k]))\n",
+                "print()\n",
+                "\n",
+                "print(tune(w + 1.0E-3, k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "44d0a4ad-d7d7-46fe-9d34-00343d8bcabf",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n",
+                        "tensor([2.525452e-01, 1.196688e-01], dtype=torch.float64)\n",
+                        "tensor([2.526084e-01, 1.195504e-01], dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([2.526084e-01, 1.195502e-01], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Check convergence\n",
+                "\n",
+                "print(evaluate(t, [w, k]))\n",
+                "print(evaluate(t, [w + 1.0E-3, k]))\n",
+                "print(evaluate(t, [w + 1.0E-3, k + 1.0E-2]))\n",
+                "print()\n",
+                "\n",
+                "print(tune(w + 1.0E-3, k + 1.0E-2))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 13,
+            "id": "b1075e4f-a003-4096-a0d8-5f0c8c39b374",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "(0, 0, 0, 0): tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n",
+                        "(1, 0, 0, 0): tensor([-2.343079e-01, -2.416176e-01], dtype=torch.float64)\n",
+                        "(1, 1, 0, 0): tensor([3.618782e-01, -2.986097e-01], dtype=torch.float64)\n",
+                        "(1, 0, 1, 0): tensor([8.705079e-02, -4.727344e-01], dtype=torch.float64)\n",
+                        "(1, 0, 0, 1): tensor([5.873074e+00, -1.106560e+01], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Series representation\n",
+                "\n",
+                "for key, value in clean(series((1, 3), (1, 1), t)).items():\n",
+                "    print(f'{key}: {value}')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 14,
+            "id": "b53e320f-97ec-4a6d-b224-a6a9d71c4516",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-2.343079e-01, -2.416176e-01], dtype=torch.float64)\n",
+                        "tensor([-2.498002e-16,  2.553513e-15], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set chromaticity to zero\n",
+                "\n",
+                "A = derivative((1, 1), lambda w, k: evaluate(t, [w, k]), w, k, intermediate=False)\n",
+                "b = derivative(1, lambda w, k: evaluate(t, [w, k]), w, k, intermediate=False).flatten()\n",
+                "\n",
+                "print(derivative(1, lambda w: evaluate(t, [w, k]), w, intermediate=False).flatten())\n",
+                "print(derivative(1, lambda w: evaluate(t, [w, - (torch.linalg.pinv(A.squeeze()) @ b)]), w, intermediate=False).flatten())"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 15,
+            "id": "9dd20a0e-5a86-4d33-bb2f-852583a72b9a",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-2.343079e-01, -2.416176e-01], dtype=torch.float64)\n",
+                        "tensor([1.000000e+00, 1.000000e+00], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set chromaticity to one\n",
+                "\n",
+                "A = derivative((1, 1), lambda w, k: evaluate(t, [w, k]), w, k, intermediate=False)\n",
+                "b = -1.0 + derivative(1, lambda w, k: evaluate(t, [w, k]), w, k, intermediate=False).flatten()\n",
+                "\n",
+                "print(derivative(1, lambda w: evaluate(t, [w, k]), w, intermediate=False).flatten())\n",
+                "print(derivative(1, lambda w: evaluate(t, [w, - (torch.linalg.pinv(A.squeeze()) @ b)]), w, intermediate=False).flatten())"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "4e5bec9a-8ca0-4ee4-8daf-3fc4ae4ced3e",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
+                "# Example-16: Tune (responce matrix & correction)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "34e2bb90-1151-46c8-af48-3547ce2e1ec8",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "from twiss.twiss import twiss\n",
+                "\n",
+                "torch.set_printoptions(precision=6, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "5fd86cee-b7a5-4313-ac9e-79fd196ca36e",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "65117f39-b23e-4d8f-ad71-b27367bfef3c",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "2f417785-0148-48e4-a207-9944d1018918",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, k):\n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.0, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.0, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, k):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, k)\n",
+                "    return x\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "print(fodo(x, k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "a2ec343b-0827-4df0-91bb-6dab993fadcf",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, k, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "835bfd5f-0466-422c-9632-0a53ecaba004",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute parametric fixed point\n",
+                "\n",
+                "pfp = parametric_fixed_point((1, ), fp, [k], fodo)\n",
+                "chop(pfp)\n",
+                "pfp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "fa3bf81b-3c99-41d7-9e72-656020d24e69",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Propagate parametric fixed point\n",
+                "\n",
+                "out = propagate((4, 3), (0, 1), pfp, [k], fodo)\n",
+                "chop(out)\n",
+                "out"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "12e6f7b1-98ea-46aa-af37-68d064b7706d",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Propagate parametric identity (surrogate model for linear dynamics)\n",
+                "\n",
+                "jet = identity((1, 1), fp, parametric=pfp)\n",
+                "jet = propagate((4, 3), (1, 1), jet, [k], fodo)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "6d1d9d72-ac01-4016-b716-3e877d58e4aa",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute tune\n",
+                "\n",
+                "def tune(k):\n",
+                "    m = derivative(1, lambda x: evaluate(jet, [x, k]), fp, intermediate=False)\n",
+                "    t, *_ = twiss(m)\n",
+                "    return t\n",
+                "\n",
+                "print(tune(k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "4929b534-0a35-4db5-a7fd-3241bbba02b8",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Compute parametric tune\n",
+                "\n",
+                "t = derivative((1, ), tune, k)"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": null,
-            "id": "68ada124-8f01-4432-b221-8a060ddc04b9",
+            "execution_count": 11,
+            "id": "7730bec7-4b61-4158-b54b-b19afdd38580",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n",
+                        "tensor([2.646746e-01, 9.564416e-02], dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([2.646564e-01, 9.339156e-02], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Check convergence\n",
+                "\n",
+                "print(evaluate(t, [k]))\n",
+                "print(evaluate(t, [k + torch.tensor([5.0E-3, 5.0E-3, 1.0E-3], dtype=dtype, device=device)]))\n",
+                "print()\n",
+                "\n",
+                "print(tune(k + torch.tensor([5.0E-3, 5.0E-3, 1.0E-3], dtype=dtype, device=device)))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "c14a8261-a260-46a7-99cd-781ff07d1f6e",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([[1.217003e+00, 3.230152e-01, 4.195000e+00],\n",
+                        "        [-7.757018e-01, -2.437956e+00, -8.197983e+00]], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Responce matrix\n",
+                "\n",
+                "print(derivative(1, lambda k: evaluate(t, [k]), k, intermediate=False))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 13,
+            "id": "ae0da0a6-9871-4d10-bde8-09710dc97160",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n",
+                        "tensor([2.627666e-01, 1.199040e-01], dtype=torch.float64)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Correct tunes (increase horizontal by 0.01)\n",
+                "\n",
+                "A = derivative(1, lambda k: evaluate(t, [k]), k, intermediate=False)\n",
+                "b = -torch.tensor([0.01, 0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "print(tune(k))\n",
+                "print(tune(-(torch.linalg.pinv(A) @ b)))\n",
+                "print()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "e45a0bb3-6dbc-4c4f-9aee-3e65e1e011a7",
             "metadata": {},
+            "source": [
+                "# Example-17: Tune (spread)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "64adfd8a-c67e-4096-b71c-432890488fa9",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "from twiss.twiss import twiss\n",
+                "\n",
+                "torch.set_printoptions(precision=6, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "f59699d6-947f-4fac-9327-f9a33c587476",
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
-            "source": []
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "043ba457-21bc-485c-ae26-398d51b84e88",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "efb457a6-9b0c-49e5-9c7f-23e7b71185d3",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, k):\n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.0, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.0, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, k):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, k)\n",
+                "    return x\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "print(fodo(x, k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "7a674c73-751e-431e-b177-a4ed852e815b",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, k, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "88be5819-14c8-44b5-a6eb-60f31490f5ef",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64),\n",
+                            "  tensor([[[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]],\n",
+                            "  \n",
+                            "          [[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]],\n",
+                            "  \n",
+                            "          [[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]],\n",
+                            "  \n",
+                            "          [[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute parametric fixed point\n",
+                "\n",
+                "pfp = parametric_fixed_point((2, ), fp, [k], fodo)\n",
+                "chop(pfp)\n",
+                "pfp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "21e78d86-e754-4a96-ab7e-ca82055202fd",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64),\n",
+                            "  tensor([[[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]],\n",
+                            "  \n",
+                            "          [[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]],\n",
+                            "  \n",
+                            "          [[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]],\n",
+                            "  \n",
+                            "          [[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Propagate parametric fixed point\n",
+                "\n",
+                "out = propagate((4, 3), (0, 2), pfp, [k], fodo)\n",
+                "chop(out)\n",
+                "out"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "f8ca945d-51a8-4a33-a353-957373ea9d45",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Propagate parametric identity (surrogate model for linear dynamics)\n",
+                "\n",
+                "jet = identity((1, 2), fp, parametric=pfp)\n",
+                "jet = propagate((4, 3), (1, 2), jet, [k], fodo)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "8c7a76f9-198e-444d-9cec-2772b562fcea",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute tune\n",
+                "\n",
+                "def tune(k):\n",
+                "    m = derivative(1, lambda x: evaluate(jet, [x, k]), fp, intermediate=False)\n",
+                "    t, *_ = twiss(m)\n",
+                "    return t\n",
+                "\n",
+                "print(tune(k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "75a24168-d78c-4344-8465-99db88121365",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.528008e-01, 1.197898e-01], dtype=torch.float64)\n",
+                        "tensor([1.984397e-03, 4.095296e-03], dtype=torch.float64)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute tune spread (direct)\n",
+                "\n",
+                "sf = 1.0E-3\n",
+                "sd = 1.0E-3\n",
+                "sb = 1.0E-4\n",
+                "\n",
+                "def wrapper(k):\n",
+                "    t, *_ = twiss(derivative(1, fodo, x, k, intermediate=False))\n",
+                "    return t\n",
+                "\n",
+                "err = torch.tensor([sf, sd, sb])*torch.randn(8192).unsqueeze(1).to(dtype).to(device)\n",
+                "out = torch.func.vmap(wrapper)(err).T\n",
+                "\n",
+                "print(out.mean(-1))\n",
+                "print(out.std(-1))\n",
+                "print()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "fd14777c-8b0c-4171-834f-4b6bcd3b1ad7",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Compute parametric tune\n",
+                "\n",
+                "t = derivative((1, ), tune, k)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "825b1694-45c2-4156-b403-f836e3d04b00",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527896e-01, 1.198895e-01], dtype=torch.float64)\n",
+                        "tensor([1.943349e-03, 4.000173e-03], dtype=torch.float64)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute tune spread (surrogate)\n",
+                "\n",
+                "sf = 1.0E-3\n",
+                "sd = 1.0E-3\n",
+                "sb = 1.0E-4\n",
+                "\n",
+                "err = torch.tensor([sf, sd, sb])*torch.randn(8192).unsqueeze(1).to(dtype).to(device)\n",
+                "out = torch.func.vmap(lambda k: evaluate(t, [k]))(err).T\n",
+                "\n",
+                "print(out.mean(-1))\n",
+                "print(out.std(-1))\n",
+                "print()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "29cd7b36-7df2-4145-b057-d1c708871dfc",
+            "metadata": {},
+            "source": [
+                "# Example-18: Parametric twiss"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "3e4c3903-481b-4de1-9f3b-54ade0534303",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "from twiss.twiss import twiss\n",
+                "from twiss.twiss import propagate as propagate_twiss\n",
+                "from twiss.convert import wolski_to_cs\n",
+                "\n",
+                "torch.set_printoptions(precision=3, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "d2fd7482-8a02-4433-9865-48e50fa167ec",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "d5a8c2a4-e707-48e6-b611-32283e6810b8",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "f0e309fd-0d4a-4a08-a2a3-8cf4ea352c03",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, k): \n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    return x\n",
+                "\n",
+                "def map_02_03(x, k):\n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.1)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    return x\n",
+                "\n",
+                "def map_03_04(x, k):\n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.1)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02,\n",
+                "    map_02_03,\n",
+                "    map_03_04\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, k):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, k)\n",
+                "    return x\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "print(fodo(x, k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "608c0359-293a-43b8-8d38-6f122c118f8c",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, k, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "566da1db-4fe5-48fd-bde2-c266e5082f7c",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute parametric fixed point\n",
+                "\n",
+                "pfp = parametric_fixed_point((1, ), fp, [k], fodo)\n",
+                "chop(pfp)\n",
+                "pfp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "648fb483-852d-405f-956f-347ab3240d55",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Propagate parametric fixed point\n",
+                "\n",
+                "out = propagate((4, 3), (0, 1), pfp, [k], fodo)\n",
+                "chop(out)\n",
+                "out"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "86ba29c9-e517-45d2-8b77-fd729789c1cd",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Propagate parametric identity (surrogate model for linear dynamics)\n",
+                "\n",
+                "jet = identity((1, 1), fp, parametric=pfp)\n",
+                "jet = propagate((4, 3), (1, 1), jet, [k], fodo)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "b7e8a435-158a-4f96-adff-cfcad2f44253",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.528e-01, 1.199e-01, 8.703e+00, 8.703e+00, 1.553e+01, 1.678e+01, 1.678e+01, 9.586e+00], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute twiss\n",
+                "\n",
+                "# Note, exact or jet one-turn transport can be used\n",
+                "# Other maps can be replaced with jets too\n",
+                "\n",
+                "def fn(k, fodo):\n",
+                "    \n",
+                "    bxs = []\n",
+                "    bys = []\n",
+                "    \n",
+                "    m = derivative(1, fodo, fp, intermediate=False)\n",
+                "    \n",
+                "    t, _, w = twiss(m)\n",
+                "    _, bx, _, by = wolski_to_cs(w)\n",
+                "    \n",
+                "    for mapping in transport:\n",
+                "        w = propagate_twiss(w, derivative(1, mapping, x, k, intermediate=False))\n",
+                "        _, bx, _, by = wolski_to_cs(w)\n",
+                "        bxs.append(bx)\n",
+                "        bys.append(by)\n",
+                "    \n",
+                "    return torch.stack([*t, *bxs, *bys])\n",
+                "\n",
+                "print(fn(k, fodo=lambda x: evaluate(jet, [x, k])))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "f9098db2-d0e7-459d-92ae-eda18d9f3b3d",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[tensor([2.528e-01, 1.199e-01, 8.703e+00, 8.703e+00, 1.553e+01, 1.678e+01, 1.678e+01, 9.586e+00], dtype=torch.float64), tensor([[ 1.217e+00,  3.230e-01,  4.195e+00],\n",
+                        "        [-7.757e-01, -2.438e+00, -8.198e+00],\n",
+                        "        [-3.111e+01, -1.531e+01, -1.101e+02],\n",
+                        "        [-3.111e+01, -1.531e+01, -1.101e+02],\n",
+                        "        [-1.749e+00, -3.120e+01, -1.799e+02],\n",
+                        "        [ 1.153e+02,  3.308e+02,  1.106e+03],\n",
+                        "        [ 1.153e+02,  3.308e+02,  1.106e+03],\n",
+                        "        [ 5.215e+01,  2.146e+02,  6.957e+02]], dtype=torch.float64)]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute parametric derivative using exact map (tune & beta)\n",
+                "\n",
+                "d = derivative((1, ), lambda k: fn(k, fodo=lambda x: fodo(x, k)), k)\n",
+                "\n",
+                "print(d)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "62ac9c73-5b26-4651-8e24-9eb3d676f577",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[tensor([2.528e-01, 1.199e-01, 8.703e+00, 8.703e+00, 1.553e+01, 1.678e+01, 1.678e+01, 9.586e+00], dtype=torch.float64), tensor([[ 1.217e+00,  3.230e-01,  4.195e+00],\n",
+                        "        [-7.757e-01, -2.438e+00, -8.198e+00],\n",
+                        "        [-3.111e+01, -1.531e+01, -1.101e+02],\n",
+                        "        [-3.111e+01, -1.531e+01, -1.101e+02],\n",
+                        "        [-1.749e+00, -3.120e+01, -1.799e+02],\n",
+                        "        [ 1.153e+02,  3.308e+02,  1.106e+03],\n",
+                        "        [ 1.153e+02,  3.308e+02,  1.106e+03],\n",
+                        "        [ 5.215e+01,  2.146e+02,  6.957e+02]], dtype=torch.float64)]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute parametric derivative using jet map (tune & beta)\n",
+                "\n",
+                "d = derivative((1, ), lambda k: fn(k, fodo=lambda x: evaluate(jet, [x, k])), k)\n",
+                "\n",
+                "print(d)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "2255334e-8ccf-49e8-8888-b2b685dd0fa1",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "0.253 0.120 8.703 8.703 15.532 16.780 16.780 9.586\n",
+                        "0.255 0.116 8.645 8.645 15.481 17.337 17.337 9.922\n",
+                        "0.255 0.116 8.646 8.646 15.482 17.366 17.366 9.940\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Check covergence\n",
+                "\n",
+                "dk = torch.tensor([1.0E-3, 1.0E-3, 1.0E-4], dtype=dtype, device=device)\n",
+                "\n",
+                "values = fn(k, fodo=lambda x: fodo(x, k))\n",
+                "print(' '.join([f'{value:.3f}' for value in values.cpu().tolist()]))\n",
+                "\n",
+                "values = evaluate(d, [dk])\n",
+                "print(' '.join([f'{value:.3f}' for value in values.cpu().tolist()]))\n",
+                "\n",
+                "values = fn(k + dk, fodo=lambda x: fodo(x, k + dk))\n",
+                "print(' '.join([f'{value:.3f}' for value in values.cpu().tolist()]))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 13,
+            "id": "654152a0-e66b-4ec1-8716-102b72a9aeac",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([[ 1.217e+00,  3.230e-01,  4.195e+00],\n",
+                        "        [-7.757e-01, -2.438e+00, -8.198e+00],\n",
+                        "        [-3.111e+01, -1.531e+01, -1.101e+02],\n",
+                        "        [-3.111e+01, -1.531e+01, -1.101e+02],\n",
+                        "        [-1.749e+00, -3.120e+01, -1.799e+02],\n",
+                        "        [ 1.153e+02,  3.308e+02,  1.106e+03],\n",
+                        "        [ 1.153e+02,  3.308e+02,  1.106e+03],\n",
+                        "        [ 5.215e+01,  2.146e+02,  6.957e+02]], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Responce matrix\n",
+                "\n",
+                "m = derivative((1, ), lambda k: fn(k, fodo=lambda x: evaluate(jet, [x, k])), k, intermediate=False)\n",
+                "\n",
+                "print(m)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 14,
+            "id": "4b423bb2-1173-42e9-a7ee-779e77d7761f",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.064e-03, -1.258e-03, -4.094e-05], dtype=torch.float64)\n",
+                        "tensor(9.036e-01, dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.000e-03, -1.000e-03, -9.990e-05], dtype=torch.float64)\n",
+                        "tensor(4.251e-02, dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor(8.589e-05, dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor(3.559e-10, dtype=torch.float64)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Correction\n",
+                "\n",
+                "# The target values (tunes and beta functions) are associated with model response matrix\n",
+                "# Given measured values, the goal is to alter knobs to get target values\n",
+                "\n",
+                "# Set target values\n",
+                "\n",
+                "vf = fn(k, fodo=lambda x: fodo(x, k))\n",
+                "\n",
+                "# Set initial solution\n",
+                "\n",
+                "sol = torch.zeros_like(dk)\n",
+                "\n",
+                "# Iterate\n",
+                "\n",
+                "for _ in range(4):\n",
+                "\n",
+                "    # Compute current values and set difference\n",
+                "\n",
+                "    vi = fn(k + dk + sol, fodo=lambda x: evaluate(jet, [x, k + dk + sol]))\n",
+                "\n",
+                "    # Set difference\n",
+                "\n",
+                "    dv = vf - vi\n",
+                "\n",
+                "    # Update solution\n",
+                "\n",
+                "    sol += torch.linalg.pinv(m) @ dv\n",
+                "\n",
+                "    # Verbose\n",
+                "\n",
+                "    print(-dk)\n",
+                "    print(sol)\n",
+                "    print(dv.norm())\n",
+                "    print()\n",
+                "    \n",
+                "    # Continue"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 15,
+            "id": "961c67f7-3585-49d5-b32b-3b8741235952",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Note, similar to tune spread example, it is possible to compute twiss spread\n",
+                "# First order computation can be performed using error propagation\n",
+                "# Or higher order jets can be sampled"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "28236397-30e5-434b-91c1-b7fdd80d0020",
+            "metadata": {},
+            "source": [
+                "# Example-19: Parametric phase advance"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "2383d32c-d2f3-4a53-86fd-f5cad0f49333",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "from twiss.twiss import twiss\n",
+                "from twiss.twiss import propagate as propagate_twiss\n",
+                "from twiss.twiss import advance\n",
+                "\n",
+                "torch.set_printoptions(precision=3, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "5eefd972-305b-4283-aa5f-26aec1b400f3",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "5b93d925-59de-4f3d-aa1b-39f123af6fc4",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "bb119a41-088f-4c08-8e3e-9f18bd4d3963",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, k): \n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    return x\n",
+                "\n",
+                "def map_02_03(x, k):\n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.1)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    return x\n",
+                "\n",
+                "def map_03_04(x, k):\n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.1)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02,\n",
+                "    map_02_03,\n",
+                "    map_03_04\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, k):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, k)\n",
+                "    return x\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "print(fodo(x, k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "4562e010-2f28-49ac-b3c2-f3276f64bab9",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, k, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "d08f85d3-8e4c-43c0-a101-ba77d2f89b5c",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute parametric fixed point\n",
+                "\n",
+                "pfp = parametric_fixed_point((1, ), fp, [k], fodo)\n",
+                "chop(pfp)\n",
+                "pfp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "91a8fa30-fbab-4869-ba91-6eeb563ae1a2",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Propagate parametric fixed point\n",
+                "\n",
+                "out = propagate((4, 3), (0, 1), pfp, [k], fodo)\n",
+                "chop(out)\n",
+                "out"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "6c1b99c3-e3b6-4f3c-a1ca-72e68d2fb9f2",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Propagate parametric identity (surrogate model for linear dynamics)\n",
+                "\n",
+                "jet = identity((1, 1), fp, parametric=pfp)\n",
+                "jet = propagate((4, 3), (1, 1), jet, [k], fodo)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "3c291b54-e05e-481d-b730-efb83291a148",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.528e-01, 1.199e-01, 2.521e-01, 1.084e+00, 2.521e-01, 2.468e-01, 2.599e-01, 2.468e-01], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute phase advance\n",
+                "\n",
+                "# Note, exact or jet one-turn transport can be used\n",
+                "# Other maps can be replaced with jets too\n",
+                "\n",
+                "def fn(k, fodo):\n",
+                "    \n",
+                "    mus = []\n",
+                "    \n",
+                "    m = derivative(1, fodo, fp, intermediate=False)\n",
+                "    \n",
+                "    t, n, _ = twiss(m)\n",
+                "    \n",
+                "    for mapping in transport:\n",
+                "        mu, n = advance(n, derivative(1, mapping, x, k, intermediate=False))\n",
+                "        mus.append(mu)\n",
+                "    \n",
+                "    mus = torch.stack(mus).T\n",
+                "\n",
+                "    return torch.stack([*t, *mus.flatten()])\n",
+                "\n",
+                "print(fn(k, fodo=lambda x: evaluate(jet, [x, k])))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "65210434-411d-464a-a126-50ea5dad6160",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[tensor([2.528e-01, 1.199e-01, 2.521e-01, 1.084e+00, 2.521e-01, 2.468e-01, 2.599e-01, 2.468e-01], dtype=torch.float64), tensor([[1.217e+00, 3.230e-01, 4.195e+00],\n",
+                        "        [-7.757e-01, -2.438e+00, -8.198e+00],\n",
+                        "        [4.458e-01, 4.852e-01, 2.926e+00],\n",
+                        "        [6.755e+00, 1.059e+00, 2.051e+01],\n",
+                        "        [4.458e-01, 4.852e-01, 2.926e+00],\n",
+                        "        [-1.523e+00, -5.303e+00, -1.726e+01],\n",
+                        "        [-1.827e+00, -4.712e+00, -1.699e+01],\n",
+                        "        [-1.523e+00, -5.303e+00, -1.726e+01]], dtype=torch.float64)]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute parametric derivative using exact map (tune & advance)\n",
+                "\n",
+                "d = derivative((1, ), lambda k: fn(k, fodo=lambda x: fodo(x, k)), k)\n",
+                "\n",
+                "print(d)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "b2a73415-1cb4-4f43-a6bc-d99693fcadab",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[tensor([2.528e-01, 1.199e-01, 2.521e-01, 1.084e+00, 2.521e-01, 2.468e-01, 2.599e-01, 2.468e-01], dtype=torch.float64), tensor([[1.217e+00, 3.230e-01, 4.195e+00],\n",
+                        "        [-7.757e-01, -2.438e+00, -8.198e+00],\n",
+                        "        [4.458e-01, 4.852e-01, 2.926e+00],\n",
+                        "        [6.755e+00, 1.059e+00, 2.051e+01],\n",
+                        "        [4.458e-01, 4.852e-01, 2.926e+00],\n",
+                        "        [-1.523e+00, -5.303e+00, -1.726e+01],\n",
+                        "        [-1.827e+00, -4.712e+00, -1.699e+01],\n",
+                        "        [-1.523e+00, -5.303e+00, -1.726e+01]], dtype=torch.float64)]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute parametric derivative using jet map (tune & advance)\n",
+                "\n",
+                "d = derivative((1, ), lambda k: fn(k, fodo=lambda x: evaluate(jet, [x, k])), k)\n",
+                "\n",
+                "print(d)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "38100b72-0f3c-4704-937a-58644a215e86",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "0.253 0.120 0.252 1.084 0.252 0.247 0.260 0.247\n",
+                        "0.255 0.116 0.253 1.094 0.253 0.238 0.252 0.238\n",
+                        "0.255 0.116 0.253 1.094 0.253 0.238 0.251 0.238\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Check covergence\n",
+                "\n",
+                "dk = torch.tensor([1.0E-3, 1.0E-3, 1.0E-4], dtype=dtype, device=device)\n",
+                "\n",
+                "values = fn(k, fodo=lambda x: fodo(x, k))\n",
+                "print(' '.join([f'{value:.3f}' for value in values.cpu().tolist()]))\n",
+                "\n",
+                "values = evaluate(d, [dk])\n",
+                "print(' '.join([f'{value:.3f}' for value in values.cpu().tolist()]))\n",
+                "\n",
+                "values = fn(k + dk, fodo=lambda x: fodo(x, k + dk))\n",
+                "print(' '.join([f'{value:.3f}' for value in values.cpu().tolist()]))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 13,
+            "id": "e36040dd-367b-47a9-884a-a0ccab42d509",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([[1.217e+00, 3.230e-01, 4.195e+00],\n",
+                        "        [-7.757e-01, -2.438e+00, -8.198e+00],\n",
+                        "        [4.458e-01, 4.852e-01, 2.926e+00],\n",
+                        "        [6.755e+00, 1.059e+00, 2.051e+01],\n",
+                        "        [4.458e-01, 4.852e-01, 2.926e+00],\n",
+                        "        [-1.523e+00, -5.303e+00, -1.726e+01],\n",
+                        "        [-1.827e+00, -4.712e+00, -1.699e+01],\n",
+                        "        [-1.523e+00, -5.303e+00, -1.726e+01]], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Responce matrix\n",
+                "\n",
+                "m = derivative((1, ), lambda k: fn(k, fodo=lambda x: evaluate(jet, [x, k])), k, intermediate=False)\n",
+                "\n",
+                "print(m)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 14,
+            "id": "9328e331-744a-4b7d-9e1c-0edb99240c7d",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.043e-03, -1.068e-03, -8.224e-05], dtype=torch.float64)\n",
+                        "tensor(1.846e-02, dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor(2.001e-04, dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor(2.786e-08, dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor(2.344e-15, dtype=torch.float64)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Correction\n",
+                "\n",
+                "# The target values (tunes and advance functions) are associated with model response matrix\n",
+                "# Given measured values, the goal is to alter knobs to get target values\n",
+                "\n",
+                "# Set target values\n",
+                "\n",
+                "vf = fn(k, fodo=lambda x: fodo(x, k))\n",
+                "\n",
+                "# Set initial solution\n",
+                "\n",
+                "sol = torch.zeros_like(dk)\n",
+                "\n",
+                "# Iterate\n",
+                "\n",
+                "for _ in range(4):\n",
+                "\n",
+                "    # Compute current values and set difference\n",
+                "\n",
+                "    vi = fn(k + dk + sol, fodo=lambda x: evaluate(jet, [x, k + dk + sol]))\n",
+                "\n",
+                "    # Set difference\n",
+                "\n",
+                "    dv = vf - vi\n",
+                "\n",
+                "    # Update solution\n",
+                "\n",
+                "    sol += torch.linalg.pinv(m) @ dv\n",
+                "\n",
+                "    # Verbose\n",
+                "\n",
+                "    print(-dk)\n",
+                "    print(sol)\n",
+                "    print(dv.norm())\n",
+                "    print()\n",
+                "    \n",
+                "    # Continue"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 15,
+            "id": "8c172e35-8002-43ab-9d28-4c6b9610c820",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Note, similar to tune spread example, it is possible to compute advance spread\n",
+                "# First order computation can be performed using error propagation\n",
+                "# Or higher order jets can be sampled"
+            ]
         }
     ],
     "metadata": {
         "colab": {
             "collapsed_sections": [
                 "myt0_gMIOq7b",
                 "5d97819c"
```

### Comparing `ndtorch-0.1.2/docs/source/index.rst` & `ndtorch-0.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/ndtorch/__init__.py` & `ndtorch-0.1.3/ndtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/ndtorch/derivative.py` & `ndtorch-0.1.3/ndtorch/derivative.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/ndtorch/evaluate.py` & `ndtorch-0.1.3/ndtorch/evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,15 @@
 @multimethod
 def compare(probe:Series, other:Series) -> bool:
     """
     Compare series
 
     Parameters
     ----------
-    probe, other: Table
+    probe, other: Series
         series to compare
 
     Returns
     -------
     bool
 
     Examples
```

### Comparing `ndtorch-0.1.2/ndtorch/index.py` & `ndtorch-0.1.3/ndtorch/index.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/ndtorch/jet.py` & `ndtorch-0.1.3/ndtorch/jet.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/ndtorch/pfp.py` & `ndtorch-0.1.3/ndtorch/pfp.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/ndtorch/propagate.py` & `ndtorch-0.1.3/ndtorch/propagate.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/ndtorch/series.py` & `ndtorch-0.1.3/ndtorch/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     series = {}
 
     for (count, factor), array in zip(signature(table, factor=True), flatten(table, target=list)):
         if not all(i <= j for i, j in zip(count, order)):
             continue
         count = index(dimension, count)
         array = factor*array.permute(*reversed(range(len(array.shape))))
-        array = array.flatten().reshape(-1, len(array))
+        array = array.flatten().reshape(len(count), -1)
         for key, value in zip(count, array):
             key = tuple(key.tolist())
             if key not in series:
                 series[key]  = value
             else:
                 series[key] += value
 
@@ -316,15 +316,15 @@
     >>> clean(s)
     {(1, 0, 0, 0): tensor([1., 0.]),
      (0, 1, 0, 0): tensor([0., 1.]),
      (1, 0, 1, 0): tensor([1., 0.]),
      (0, 1, 0, 1): tensor([0., 1.])}
 
     """
-    return {key: value for key, value in probe.items() if torch.any(value > epsilon)}
+    return {key: value for key, value in probe.items() if torch.any(value.abs() > epsilon)}
 
 
 def fetch(probe:Series,
           index:list[tuple[int, ...]]) -> Series:
     """
     Fetch series
```

### Comparing `ndtorch-0.1.2/ndtorch/signature.py` & `ndtorch-0.1.3/ndtorch/signature.py`

 * *Files 23% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     for i in ns:
         table = table[i]
     return table[n]
 
 
 def set(table:Table, index:tuple[int, ...], value:Union[Tensor, Table]) -> None:
     """
-    Set derivative table element at a given (bottom) element signature.
+    Set derivative table element at a given (bottom) element signature
 
     Note, index can correspond to a bottom element or a subtable
 
     Parameters
     ----------
     table: Table
         input derivative table representation
@@ -180,17 +180,18 @@
 
     *ns, n = index
     for i in ns:
         table = table[i]
     table[n] = value
 
 
+@multimethod
 def apply(table:Table, index:tuple[int, ...], function:Callable) -> None:
     """
-    Apply function (modifies element at index).
+    Apply function (modifies element at index)
 
     Note, index can correspond to a bottom element or a subtable
 
     Parameters
     ----------
     table: Table
         input derivative table representation
@@ -212,11 +213,129 @@
     ...    y1, y2 = y
     ...    return (x1 + x2 + x1**2 + x1*x2 + x2**2)*(1 + y1 + y2)
     >>> x = torch.tensor([0.0, 0.0])
     >>> y = torch.zeros_like(x)
     >>> t = derivative((2, 1), fn, x, y)
     >>> apply(t, (1, 1), torch.log)
     >>> get(t, (1, 1))
+    tensor([[0., 0.],
+            [0., 0.]])
 
     """
     value = get(table, index)
     set(table, index, function(value))
+
+
+@multimethod
+def apply(table:Table, index:list[tuple[int, ...]], function:Callable) -> None:
+    """
+    Apply function (modifies element at list of indices)
+
+    Parameters
+    ----------
+    table: Table
+        input derivative table representation
+    index: int[tuple[int, ...]]
+        list of element signatures
+    function: Callable
+        function to apply
+
+    Returns
+    -------
+    None
+
+    Examples
+    --------
+    >>> import torch
+    >>> from ndtorch.derivative import derivative
+    >>> def fn(x, y):
+    ...    x1, x2 = x
+    ...    y1, y2 = y
+    ...    return (x1 + x2 + x1**2 + x1*x2 + x2**2)*(1 + y1 + y2)
+    >>> x = torch.tensor([0.0, 0.0])
+    >>> y = torch.zeros_like(x)
+    >>> t = derivative((2, 1), fn, x, y)
+    >>> apply(t, [(1, 0), (1, 1)], torch.log)
+    >>> get(t, [(1)])
+    [tensor([0., 0.]),
+    tensor([[0., 0.],
+            [0., 0.]])]
+
+    """
+    [*map(lambda index: apply(table, index, function), index)]
+
+
+@multimethod
+def apply(table:Table, function:Callable) -> None:
+    """
+    Apply function to all bottom elements
+
+    Parameters
+    ----------
+    table: Table
+        input derivative table representation
+    function: Callable
+        function to apply
+
+    Returns
+    -------
+    None
+
+    Examples
+    --------
+    >>> import torch
+    >>> from ndtorch.derivative import derivative
+    >>> def fn(x, y):
+    ...    x1, x2 = x
+    ...    y1, y2 = y
+    ...    return (x1 + x2 + x1**2 + x1*x2 + x2**2)*(1 + y1 + y2)
+    >>> x = torch.tensor([0.0, 0.0])
+    >>> y = torch.zeros_like(x)
+    >>> t = derivative((2, 1), fn, x, y)
+    >>> apply(t, torch.norm)
+    >>> t
+    [[tensor(0.), tensor(0.)],
+     [tensor(1.4142), tensor(2.)],
+     [tensor(3.1623), tensor(4.4721)]]
+
+    """
+    apply(table, signature(table), function)
+
+
+def chop(table:Table, threshold:float=1.0E-9, value:float=0.0) -> None:
+    """
+    Chop tensor elements in a table below a given threshold
+
+    Parameters
+    ----------
+    table: Table
+        input derivative table representation
+    threshold: float, default=1.0E-9
+        threshold value
+    value: float, default=0.0
+        set value
+
+    Returns
+    -------
+    None
+
+    Examples
+    --------
+    >>> import torch
+    >>> from ndtorch.derivative import derivative
+    >>> def fn(x, y):
+    ...    x1, x2 = x
+    ...    y1, y2 = y
+    ...    return (x1 + x2 + x1**2 + x1*x2 + x2**2)*(1 + y1 + y2)
+    >>> x = torch.tensor([0.0, 0.0])
+    >>> y = torch.zeros_like(x)
+    >>> t = derivative((0, 1), fn, x, y)
+    >>> apply(t, lambda x: x + 1.0E-10)
+    >>> chop(t)
+    >>> t
+    [[tensor(0.), tensor([0., 0.])]]
+
+    """
+    def inner(tensor):
+        tensor[tensor.abs() < threshold] = value
+        return tensor
+    apply(table, inner)
```

### Comparing `ndtorch-0.1.2/ndtorch/util.py` & `ndtorch-0.1.3/ndtorch/util.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/ndtorch.egg-info/PKG-INFO` & `ndtorch-0.1.3/ndtorch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ndtorch
-Version: 0.1.2
+Version: 0.1.3
 Summary: Higher order partial derivatives computation with respect to one or several tensor-like variables, application to nonlinear dynamics
 Author-email: Ivan Morozov <i.a.morozov@inp.nsk.su>
 License: MIT
 Keywords: torch,derivative
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: examples
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/ndtorch/badge/?version=latest)](https://ndtorch.readthedocs.io/en/latest/?badge=latest)
@@ -97,12 +97,10 @@
 
 <p align="center">
   <img width="576" height="576" src="docs/pics/collision.gif">
 </p>
 
 Reduce real part of a hyperbolic fixed point
 
-Collision of fixed points
-
 <p align="center">
   <img width="576" height="576" src="docs/pics/change.gif">
 </p>
```

### Comparing `ndtorch-0.1.2/ndtorch.egg-info/SOURCES.txt` & `ndtorch-0.1.3/ndtorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.2/ndtorch.ipynb` & `ndtorch-0.1.3/ndtorch.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9274945175438596%*

 * *Differences: {"'cells'": "{227: {'execution_count': 15, 'id': '8c172e35-8002-43ab-9d28-4c6b9610c820', 'source': "*

 * *            "['# Note, similar to tune spread example, it is possible to compute advance "*

 * *            "spread\\n', '# First order computation can be performed using error propagation\\n', "*

 * *            "'# Or higher order jets can be sampled']}, insert: [(95, OrderedDict([('cell_type', "*

 * *            "'markdown'), ('id', '7056772b-ad88-465f-ab99-5de6f5e9a464'), ('metadata', "*

 * *            "OrderedDict()), ('s […]*

```diff
@@ -3264,20 +3264,4068 @@
                 "\n",
                 "    lr += 0.005\n",
                 "    gradient = derivative(1, objective, knobs, intermediate=False)\n",
                 "    knobs = knobs - lr*gradient"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "7056772b-ad88-465f-ab99-5de6f5e9a464",
+            "metadata": {},
+            "source": [
+                "# Example-10: Alignment indices chaos indicators"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "b5b8e139-1eb3-497e-909f-c6351dd3c8c3",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "\n",
+                "torch.set_printoptions(precision=8, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "4ac5ba1c-91af-46bd-bdfb-05e0a896f110",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "a883b669-2946-4b45-8101-a2c32ab2c92d",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set fixed parameters\n",
+                "\n",
+                "a1, b1 = 0, 1\n",
+                "a2, b2 = 0, 1\n",
+                "\n",
+                "f1 = torch.tensor(2.0*numpy.pi*0.38, dtype=dtype, device=device)\n",
+                "f2 = torch.tensor(2.0*numpy.pi*0.41, dtype=dtype, device=device)\n",
+                "\n",
+                "cf1, sf1 = f1.cos(), f1.sin()\n",
+                "cf2, sf2 = f2.cos(), f2.sin()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "7e2e4e7d-76d1-4f16-9c39-640fbcb0919a",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set 4D symplectic mapping\n",
+                "\n",
+                "def mapping(x):\n",
+                "    q1, p1, q2, p2 = x\n",
+                "    return torch.stack([\n",
+                "        b1*(p1 + (q1**2 - q2**2))*sf1 + q1*(cf1 + a1*sf1),\n",
+                "        -((q1*(1 + a1**2)*sf1)/b1) + (p1 + (q1**2 - q2**2))*(cf1 - a1*sf1),\n",
+                "        q2*cf2 + (p2*b2 + q2*(a2 - 2*q1*b2))*sf2,\n",
+                "        -((q2*(1 + a2**2)*sf2)/b2) + (p2 - 2*q1*q2)*(cf2 - a2*sf2)\n",
+                "    ])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "c52b6cdc-defc-4401-9438-3ef068ddb250",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set 4D symplectic mapping with tangent dynamics\n",
+                "\n",
+                "def tangent(x, vs):\n",
+                "    x, m = derivative(1, mapping, x)\n",
+                "    vs = torch.func.vmap(lambda v: m @ v)(vs)\n",
+                "    return x, vs/vs.norm(dim=-1, keepdim=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "041045e3-e9e6-4975-a9a7-74e82bd54c43",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set generalized alignment indices computation\n",
+                "\n",
+                "# Note, if number if vectors is equal to two, the index tends towards zero for regular orbits\n",
+                "# And tends towards a constant value for chaotic motion\n",
+                "# If the number of vectors is greater than two, index tends towards zero for all cases\n",
+                "# But for chaotic orbits, zero is reached (exponentialy) faster\n",
+                "\n",
+                "def gali(vs, threshold=1.0E-12):\n",
+                "    return (threshold + torch.linalg.svdvals(vs).prod()).log10()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "f9a0791b-873c-4915-bf36-4f15096d063a",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAfIAAAHSCAYAAAAXPUnmAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8qNh9FAAAACXBIWXMAAAsTAAALEwEAmpwYAABXa0lEQVR4nO3dfXBc1Zkn/u9JjAE5L9i+ChCIjYygBZgUnghj40i2kwaMzChmkp2gkIzTIWN+MzRbtcpYw1bWIznsVCVSISa1zdTgCvQ4rNc4Y9aMYjvY7sSyHcdvYkxiIGoQcmzMkKAWL5VIWQzJ+f3x9Mm93e7WW7/cl/5+qlS33ySdttX3ueec5zxHaa1BRERE/vQBtxtAREREU8dATkRE5GMM5ERERD7GQE5ERORjDOREREQ+xkBORETkY9PcbsBUWJalr7jiCrebQUREVBbPPvtsSmtdnes5XwbyK664An19fW43g4iIqCyUUqfyPcehdSIiIh9jICciIvIxBnIiIiIfYyAnIiLyMQZyIiIiH2MgJyIi8jEGciIiIh9jICciIvIxBnIiIiIfYyAnIiLyMQZyIiIiH2MgJyIi8jEGciIiIh9jICciIvIxBnIiIiIfYyAnIiLyMQZyIiIiH2MgrwSpFNDVBSSTQFsbcMstwOHD8tjhw8DKlfKceV0q5XaLiYhogqa53QAqoVQKiMWA3buBQ4fk9unT8tzx48DwMFBXB/T3A4ODwJ//uQTy3buBzZsBy3K3/URENC4G8qBJpYB4HGhuBqJRIJGwnzNBHJAgvnQp8N57wJw5EsxnzZLnEgn5GZGIBP/RUaCqSn4egzsRkacwkAdJMgmsWiVB+TvfkWBtfPzjwLRpEsxnzQLuuUd65fv2ATU18hqt5djYCIyMSBBfvz7zd3R02LfNRUMkwgBPROQSzpEHgZnbXrNGgnhVlR3Ezz9fjlVVMmReVwe8+SZQXS2BuqlJvgDg058G2tuB6dMlgI+OAuEwUF8vz4+OZs6jx2Iy5x6LcX6diMgl7JH7nbMXfvPN8tiKFcAzz0jg/eQngd/+VnrOoRBw4EBmL3rHDgm+c+fKY/G4DK03NUnwTyQkmBurVwM7d0qP/eBBecwcTe997Vr21omIyoSB3O9aWyWIV1cD11wD/Oxn0hsfHZXe9xNPSAA3LEsCrZPzsUgk8zhjhsy39/RI8N65U4L86KgE+ZoaOS5YAHR2yvelUnbA7+0FNm6Un8XATkRUdAzkfmV6vPffDxw7BgwNAS+/LM/Nny9LyqYSNLMDvbltetkzZthJcABwySXAyZOZr2lpkeBeWyvBPB6Xi4D16+XonGcnIqKCMJD7kbPHW1cnQTwcBs6eledz9bqLwflzo1EJ6kNDsrStqkoeN0PzAHDbbcDVV0uP/rHH5LHRUfs9mIsBZsMTEU0ZA7kfxeN2EO/vl+OCBZJs1tQkgbHUTFBPpWRY3zkkPzIit0dHpZ033mgHekDaaXrogFwQmAsEzq0TEU0KA7kfmaDZ0CC3+/uBL37RnqMuZwDM7v1blj107hxCNz34U6ck0/3mm4H77gNOnJDHOjrkNfG4PA+UZlSBiChgGMj9JJmUYLdggQS7eNzukbe0ZCa1eYEJ3ubiYu1aKQ8LSFLeRRcB+/fLFyBz/evWyTSBCfgsRENENCYGcj9pbZX550TCDnC9vTJ83dPjvR5srrn6WMy+GLnnHhl2Hx0Fjh6V93H2rP0enZwXBERE9CcM5H6RSgHXXQf88peSJX7woPTCb7xRvsxwu9eFQsCePfZ95zD8vn1SMnbtWgns+/bZa9g53E5ElBMDuV/E45Ik1t4uQ9A7d0oPfedOmRv3e081GrXf18qVwNatdtIbYPfIgXOnGPz+3omICsBA7hfObPDubmDZMlnWtWyZf3rjY7EsKRzjzFg3WfFmmdrwsNzetAkYGJDh9+pq9tKJqKIxkHudM5ABsmTr2DEJeqVaL+6WXO8nHreXqZkeOyDFZu68MxgXMUREBWAg9zpnIAuH5ctUSwtSEM/HORJhcgIAZrITEaUpbbau9JH6+nrd19fndjNKy7mv+GOPAdu2yXByezszuIHMf5+eHrtnzmpxRBRASqlntdb1uZ4rSo9cKbUCwHcBfBDA97TW3856/mEAy9N3qwB8TGt9Ufq5PwA4kX7utNa6uRht8j1nYZTqagni1dWys9miRe62zQvMv49ZftfbK7115zC8mX4gIgqwggO5UuqDAB4BcAuAMwCOKaV6tNYvmtdorf+b4/X3A1jg+BG/11rfUGg7Aid7F7LHH5fiLw8+KFuPVjrz79Kcvu4zpWDXrpWM95077TXrLPlKRAH2gSL8jIUABrTWg1rrswCeBPC5MV7fAmBzEX5vMKVSssxseNh+zLKAp5+WOurd3a41zVNMYlwoJD3vzk4J2lVV9m5sgN1zj8fdaysRUQkVY2j9MgCvOu6fAXBTrhcqpeYCqAHwE8fDFyil+gC8D+DbWuuni9Am/zKBx/TAd+8GliyRIMWeeG65st3D4czNY5jdTkQBVe6s9bsAbNVa/8Hx2Fyt9WtKqXkAfqKUOqG1fiX7G5VSawCsAYA5c+aUp7XllkpJhnY4LGuk6+rscqXOHcIov+z67sC5/27cYY2IAqQYQ+uvAfiE4/7l6cdyuQtZw+pa69fSx0EAvcicP3e+boPWul5rXV9dXV1om73JLDVbsECG0Ts6ZL30ffexRzlRpneeHaDNlIVZl9/WJkfn40REPlSMHvkxAFcppWogAfwuAF/KfpFSqg7ATACHHI/NBDCqtX5XKWUBWAKgswht8qfmZsm+BiRZa3BQstWvvpo9x0I5VwE4xWJy8TQykrntKhGRTxQcyLXW7yulogB2QZafPa61fkEp9S0AfVrrnvRL7wLwpM5cuH4NgEeVUn+EjA5825ntXnF6euzs685O2W/8wQeZ4FYM2asAANl17cgRd9pDRFQkLAjjBWbO1hm4vba3eNB0ddk99KYmrjknIk8reUEYKkAqBaxeLT3xpiY5vvSS1BHnzl6l4yz9yipwRORjxUh2o0LE4xK86+qAdevkODAgPUaufS4dy5I58Y6OsYN4MinbqiaT5WoZEdGksEfutkjELjP6zDPAn/85cPHFwMKFzFR3k5nu2L1blv8BXMdPRJ7EQO4mEyzWrZP7o6PSE+/s5Jpxt5ks97VrgenTmXBIRJ7FQO4mEyxMAZjrrpMgzp64+5xZ7pZlD7EzEZGIPIZz5G5qbpYgbpKujh9ntTGvyC4s09oq0x933CHz6iwgQ0QewUDuhlRKgsG990pP/NAhqeCWSNj7aZO3dHfbiYjr18toCqvCEZEHcGjdDaYUqxEOS1nWri732kRjC4WAAwfsC61IxJ4aGRk5t747EVGZMJC7oblZsqFDITnxm126qqs5P+5lZsmaYf6vRkbs4jJMUiSiMmMgd0NPjwyj33qrnPi5G5c/mXn0VMrukRMRlRkDuRvMCb+5WXp4Bw/aa5XZo/OfXPuhG7xII6ISY7KbG8yJv6dH5soTCSnPyh5d8JgtU1tamBRHRCXBHnk5mb2wUyng+eeB+fMloFdVsd53UI2OyjGRkJ45R1yIqMgYyMspO1t93z5WcasUixdLUlwqxQs2IioqBvJyMjtumR4566kHX1WVHGfMkIu4GTN44UZERcVAXm4zZnAYvZJEo/J/3twsORG5LtyYEEdEBWAgLydnARGDQT3YnBnt+XriLCxDRAVgIC8nZwERM1fOoVZiYRkiKgADeTk5C4gYnCMnFpYhogIwkJeLWXoGyHC6s9QnESAB3dRwN8Gcc+dENA4G8nKJxTicTuNzzpcfOyZbp/b2Ahs3MpgTUU6s7FZuNTXA0BCrfFFukYjUFgAkiNfWypHb2xJRHuyRl0s0avewurpkfTGH1ylb9nz50NC529tyuRoROTCQl4M58XZ3A2fP2hukEOXjDOjZ29ua4XeAUzRExEBeFs4T7+bNmclMRGPJtbOa+dvh3xARgYG8PJwn3rG2vCSaiOzsdg6vE1U0JruVgwnePOFSsZhRnng88/FUSubUmUxJVDHYIy8nJilRseQaXk+lgNWrJaES4MgPUYVgj7zUnD2kfL0oosnKNcoTj0sQD4cl272jgz1zogrAHnmpmeDd2ytZ6wCTlKg0ctXyB7jMkSjg2CMvpVRKTqrhsPSUeno4V06lY3rp0SjQ2CiPjY7KkXPnRIHFQF5K8bjdM1q7VoI6T6RUapYFLF8ut6uq5MhpHaLA4tB6KUUiMqS+cydw5gzQ388661Qe0WjmTmpce04UWOyRl9qNN8rQen8/0NTEEymVR3YyXK7kuFRKeum33AIkk+60k4gKxh55KZmh9fZ24NZbueyMvCN7qVprK7Bjh7ttIqIpYSAvpeyKbkReYZaqNTYC06fbKyqIyHcYyEuJ5VjJq3JdZLJgEZEvMZATVSLnRaYJ4Gb9eW8vsHEjgzmRTzDZrRSSSWDlSiYQkT84d+drapIhdy5TI/IN9shLobXVTiJiAhF5XfbSNOc2uxxuJ/I8BvJSMIlDTCAiP8jO5XDedvbWuXUqkScxkJdCKMSeOAWD6Zk3N9vL1UZG7GIzDOhEruMceamkUrJZBXegIj8zvfWeHgniTU3yOMu9EnkGe+SlEovZddZZlpX8LhKRnjgAtLRkln8lIlcxkJeK2XVq6VKe8Mj/LEuCd1tb5oUpk+GIXMdAXipm16lly3iCo2DItfGKMxmOo05ErijKHLlSaoVSKqmUGlBKPZDj+a8qpYaUUs+lv77ueG61Uurl9NfqYrTHE6JRoLNTjkRBkGvjleZmmTe//nrZfKWtjTkhRGVWcI9cKfVBAI8AuAXAGQDHlFI9WusXs166RWsdzfreWQDaAdQD0ACeTX/vW4W2yzXOoUb2UCjoTBLc4KDs8JdIANXV/NsnKqNiDK0vBDCgtR4EAKXUkwA+ByA7kOdyG4A9Wus309+7B8AKAJuL0K7yy95RiiezsjPXUc3NEmM4dVtiZpi9oQFYtw5YsIA5IURlVoxAfhmAVx33zwC4KcfrPq+UagTwEoD/prV+Nc/3XlaENrnD7CjFfceLLpmUWYpQyL7/9a8D/+N/ADfdJPeHhoCPfQw4dgz4zneA4WHg8ceBhx8GHnpIvtekLjhVVcnPZsCfAmcxmT177MeZBEdUNuVKdvshgM1a63eVUvcC2AjgM5P5AUqpNQDWAMCcOXOK38Ji4LalU5ZMAmvWAL//PaC1PKYUMG0a8Gd/BuzaBQwMyMitceiQrIgaGLAfO3VKjsPDklzd3w/81V9JkHd+b7ZNm2SBwYsvyq6ejz5qXzTQFGQnwTGwE5VMMQL5awA+4bh/efqxP9FaDzvufg9Ap+N7l2V9b2+uX6K13gBgAwDU19frQhpcMty2dFKcwXtgAHgrT2bEoUNyrK0FbrvN/t5cPfJwGLjgArn/jW8A/+t/Afffn7tHfvQosG8fMHu2/H7nBcHttwNz5gDz58t/K3vsk5Srfjuz24lKQmldWExUSk2DDJd/FhKYjwH4ktb6BcdrLtVav56+fSeAv9daL0onuz0L4M/SL/0PAJ8yc+b51NfX676+voLaTe5wDpGbXrYxc6YE61w98lIEU9NJNNO7c+dKj/w3v5HcLadwWKZ/AQ7FT1oqJSs4jh8HHnwQOHCAPXOiSVJKPau1rs/1XME9cq31+0qpKIBdAD4I4HGt9QtKqW8B6NNa9wD4r0qpZgDvA3gTwFfT3/umUupBSPAHgG+NF8TJf1IpKXQ3Ogps25Y5RF5TI+fzCy8ENmwo73D2WNO7nZ3SY58/Xy4+EonMofmDByWwM6hPQDwOdHXZ9xMJmRPp6HCtSURBUnCP3A2e65Fz/i+vZFKGqU+etB8zQ+R+GbJ2XogA0rF0BvWlS2UU4aqrZI4+FuP8egbzDwjIP2JXF9DezkBONAlj9cgZyIuho0PqqofDwObN3o9MZZBMAvfeCzz3HPDOO/LYvHnAV77ij+A9Fmdgzw7qgIwyXHKJ3P70p2Vq2M/vt6iyL3p5EUw0ISUdWieHREI2lFiyxP/RaorMsPTjj0vmuDFvnqzMC0JP1bLszqR5v0eOSI983z6ZOjAjEIcOyXTCnXcyoAM4NyGUSXBEBWMgLwZThnXvXnsytQJ3PMseRp85E6irC3av1LIkkBsmsP/0p3L/17+WwN7VJb13Jsxlyc5uZw+daNIYyIvB2UXbv1+G2CuoIIwZav7+9+0gPnu2JIQFoQc+GdmB3WTpnz17bsLc6CjwwgtAd3fl/Tv9ibOHzsqIRFPCQF5M0ai9T3OF9CZSKZlNcAaoIA2jFyoUkoz47IS5qiq50EkkJMgvWSKPV3QvPbsyInvnRBPCQF5MFVYQJpkEVq2S6mkA0NgILF9e4cEoD+egjZFMAq2twHXXSa4kIMG9YlMszChWc7Nc9ZgrHaCiPldEk8Ws9WKpoN5DdkJbbS1w990VGnyKwPTWnXGrtraCE+S6uuwEOK4EIQIwdtZ6UfYjJ9jZt/G42y0pqWQSWLxYzrXDw7Jj5fbt0tvkuXZqTG9982ZZXl1bayfILV5cgVt8RyISwAEZnjB/WKmU/KNU1D8G0fg4tF4s2dm3AZNKSbB5/HGpjQ5IwNm+nXPhxWICekuLjG688ood0I8ckc1cKqLYjGXJVY0Z4TK4VI0oJw6tF6JChtOTSeCOOzLrojc2Ak89Fei37Tpnxvv+/fKYGXKvyOVrFfJ5I8qFld1KxczldXYGtoeQTMqmIkNDcn/WLOkxcii9fExOgqlTbyxdCixbVoEB3WBgpwrCym6lUgHD6XfcIUF85kzZNrQik69cZtamt7XJ0Hpvr1SQM1+jo5KrUHHxzAy1j4xU3LJPIicG8kIEeLmZWR9ueoBf/3pmoRMqPzOHbrLcTUA39d53766wpWvmAnpoSNbvcUc1qlDMWp8qk0F7+DCwcqWMQQdEdpGXcNjOMSL3mYC+datcXMViUkMlkZB4tnp1hSR2Z19I791bIW+cKBN75FMVi8lZ06wVAoAdO9xtUxGYKpnOIM5lvN7kjGMbN9pr0XfurLC9e6qq5Lh/vwy3B3SUjCgfBvJC3XYbcPXVUjA7AGIxCQQVn0jlM85hd1OuPJGwt1pdsCDA+Q1m06LRURleT6UC+kaJcmMgnypTV725GejpkV1CfC6ZBDZtktvLlnG60Y8sy+6dA3a1uEQCOHoUOO+8AK5FN1cxZhWJc+dBZrZTBWAgnyozruksJ+njIT3nMrO6OruTQ/7jrOtu1qK/954kxgGy1eyVVwYwoOdaRcIiMlQBuI68UAG44k+lpBTowEDlbj8adLnWojc2Ah/6UMC3UQ3A55MIYK314nPWfDY9cx+fJDo77ZP7174W4JN6BTNr0Q8dkj/XcBhQSubS77jDnl8PHMuSIB6PB/QNEjGQT02ANkhJJqV+OiAJ+FxmFmwmoO/ZAzz6qEyjDAzIAoyWloDGugB9Xoly4Rz5VASootuaNbKL2cyZsgGKjwcWaJJCIeDAAbtmQCIhUyyB2z41QJ9XolzYI58K5wJeH2+rmEwCJ07I7U9+kkPqlchsNJa9fWpnZ4DqHI01/cWtUSkA2CMvhM8zYu+9F3jrLdkI5dFH3W4NuSV7+9QFC+yyr2fPArfeGuBcMZ9/hokABvLC+HjILpUCTp+W2/PnszdO8jewZ4/cTiaB1lbguuskzgW2jnskImsud++WmhD8IJAPcfnZZARkKYuzlnptrcyN8/xFuTgrxQFS033jRl//+Z9r5Up5g7W1wN13B/BqhYKA25gWixmG6+319dksFrNrqd99N4M45eesFGfquJuqcUBAYl53NzA4CPT3S/q+szIckQ8wkE9GczOwYYN9NvNhDdNUSk7IgKwlZgU3Go+zjns8LuXM16+X544d8/U1rTDp+7EY67WTLzGQT0ZPj105xYecQ+rc1YwmyyR/mwTvQO20Nla9diKPYyCfjEjEvlo/eFAygnw0Lu0cUl+yxMcnXXJVvp3WDh4MwMWhjxNYqXJxHflkmDPYyZNy5mptdbtFkzI6KsfGRg6pU+HM/Hk4LPcTCemd+7rca74151xvTh7GHvlUmL3HfbIHudkwY+tWub98uc97TeQZpqCMSYYzFeK2bAGeftpXA1Zj43pz8jAuP6sAzp1W6+okr4eBnIotlZKAvmmTpJIEajVXQJaekn9x97MKlkoBp04Bc+YAN98svSSeh6gUzMzT9u0B3IwlALscUnAxkE+GD+fJOjuBRx6RKm4XXRSgoU7yLLOaK1Bz50QexkA+USZF12fbIR45IseZM30zpU8B4NyMJRyWYL5+vXyEAhPMzYX94cMB2mGG/IjJbhPhXGcTDvumYEQyCbz6qtz++tfZG6fyci5Tc1aGW706AEVkADsBrq5OqsINDjIBhVzBHvlExGJ2EF+yRLoWHu+Vp1LAHXfISrnaWjvZjajcTEDfvFlqtZsiMr4fao9EZO7q4YeB6moJ5oEaciC/YI98Mkz5qhkzPF8worPTLkJ3553sJJD7zLpzZxEZwP44+e5v1CTAdXXJDmp1dfLG4nEuUaOyYiCfCGfwNh9ejzt+XI7sjZOXODdhAaRI0fr1Mlvlw60LhLmob26WMs4ev8in4OE68snwyVrSZBJYswZQCnj0Uc6Nk3d1dEggX7sWqKqSxwKx7pyoyLiNaaFybfvk0V55KgWsWiXTdU1NDOLkbWawK3A7qhGVEQP5RJjs1HBY1tN4eOgsFpMgXlvL5Wbkffl2VGtoCFiJV6ISYtb6REQi0r1NJKT74OGugtkY5c47eRIk/3BmtpvVXHfcEYDMdqIyYCCfCJOh09np6d54KmUnuZn5RiI/sSzpiTtLvJrEOF/zYVVI8g8G8vGYDyDg+VrLZr/xcJjblJJ/ZZd4TaWAW26R2S3fxkEzPcd15lQCRQnkSqkVSqmkUmpAKfVAjudblVIvKqV+oZT6sVJqruO5Pyilnkt/9RSjPUVlPoAeLwAD2MPqCxZ4+nqDaFymxGtnp6zCSCTkerqhwaeVUM30nFlnTlREBQdypdQHATwC4HYA1wJoUUpdm/Wy4wDqtdafBLAVQKfjud9rrW9IfzUX2p6iSqUkndbjCW4Ah9UpeEwiXCwmvfOaGpk7X7XKh51an0zPkT8Vo0e+EMCA1npQa30WwJMAPud8gdZ6r9Y63V/EYQCXF+H3ll48LpN0x4653ZJxcVidgioUAvbsAX70IzsRbvFiHw61cytUKpFiBPLLALzquH8m/Vg+9wD4keP+BUqpPqXUYaXUqiK0p3iam+2yix6f2zJNC4V4nqBgMnPnJhGuq8vzH8vJYUIcTVFZk92UUl8GUA+gy/Hw3HS1mi8B+Cel1JV5vndNOuD3DQ0NlaG1kHKL/f2ZNZQ9KJUCdu2S276cPySaIJPVHg4DjY2+uMaeGJ9uk0zeUIyCMK8B+ITj/uXpxzIopcIAvglgqdb6XfO41vq19HFQKdULYAGAV7K/X2u9AcAGQEq0FqHd4/NJDWWzQUpNTUCW6hCNwQy1O3cXbmmx9zTy5YhUPC5vpLER2L1bzjksBEETVIwe+TEAVymlapRS0wHcBSAj+1wptQDAowCatdZvOB6fqZQ6P33bArAEwItFaFNxmDmtUMjTc1tHj8pxzhx+9qlymPwxU6vJB7sL52e2RJ0+Xd5Ma6vbLSIfKTiQa63fBxAFsAvALwH8QGv9glLqW0opk4XeBeBDAP4ta5nZNQD6lFI/B7AXwLe11t4I5D6Zr0qlgLNn5fb8+e62hajcTDBvb5dr7aEhn1aDc6boNzWxvjJNSlFqrWutdwLYmfXYPzhuh/N8388AXF+MNhSdWT8OeHaDFEA+94cOyW2PDhgQlZQp79rVlbllry/3OQ+F5MrEB7sskndw05R8mptlrurUKTlLeHTyzfQ8Fi/msjOqbJGIlH0AfL7PuelEjIz49GqEyo2BPJ+eHpmrSiTk/owZnuyZP/+8HKdP52edKpvpmQP2cXRUeuq+ioUmqXZkxBejguQ+BvJ8zOX96KiUSvNoxvr8+cC+fZwfJ3Jy7nPe1gY8/riPtkV17u1qeuREY2Agz8d5ee9RqZS9btw3vQ2iMnDGwi1b7G1R777bs7Nk5zJvgmgc3P0sHx9krbMsK9HYcm2L2tLi6Y810aQxkOfj8W0HUyng4EG5vWSJT3oYRC7I3hY1kfDsx3pifNDJoPJiIM/H49sOsjdONHFmW9T2dmDpUrsanC9joY+2VqbyYCDPJZWSD0l3t2e3HeTe40STY9Jeli2T+4mET/c3N1XgzHmJPfSKx2S3XLLXcRJRYJgRrE2b7P3NDxzw0QVxdhKcT4pXUemwR56LueIdHZUPiMd2IkmlgOPH5XZVlbttIfIb0zPfvh2orZVg7tthdkCKV4XDdvEq374RmioG8lzMFa9HoyTnx4kKFwrJcjTA5wlwpnjVI49IWr7HOh5UehxazyWVkg/D6Khkx3gsWnJ+nKg4zEf74EF7b/ONG332uTLFq3bvlo0XzAmCKgZ75LnE43Jl29Ulc+Qe+lQnk8C2bXLbowMGRL5hhtk3b7YXqfiuZ27exK23yn2eGCoOe+S5OHdf8FjGejQqhS1qaz03UEDkW2Y71NWrfdwzN3VpPXbOotJjIM/Fw+VZ58yRY2Ojz04yRB6XHcwbGnxUnx1gSdcKxqH1XDy8LvOVVzKPRFQ8JpjX1Uk2e2ur2y0qEg+f06hwDOS5eLRyUjIJnD4ttxcudLctREFl6rM3NQH33w+sXOnDojHZPHpOo+Lg0HouZo7JY3NNra3AyZPSWzD1H4io+EIhYMcOCeI7dwKDgz4rGpPNo+c0Kg72yH3k/vuB6mrg4Yd9fEIh8pHubnuY3ZflXA3LkiAej3N4PYAYyJ3MPFIs5slhqIceAoaG5EhEpWd2TjPB/I47fFw8jcPrgcVA7uSsWeyxzVKSSTvBbcECd9tCVEly7Wnuy+Jp2ZutUGAwkDs1N0uGy6JFQG8vMDzsdov+JBqV+fHaWs6PE5Vb9p7mTzwhn0Nf9czN8jTnvFwyGZBsvsrGZDennh7JbHnpJbn0PnsW2LPH7VYBAObOlePSpZwfJ3KD2dO8oUGG2bu6pIiaR0tOTExrq5zzAMnuI19ij9zJDD3ddpvc99AY9ssvZx6JqPzMMHttrdzftMnnndl164B584A33vDhEAMZ7JE7maGnVEq6wB6aS7rpJmD/fjkSkXtCIdmbxPTMlywBvvY1iYO+Gy07cEDW1g0OAn19siyG1eF8R2mt3W7DpNXX1+u+vj63m1E2ZjM2QObKfXeyIAqgZFKC+dCQ3G9q8mF99lRKRiGPHJFegi+vRiqDUupZrXV9ruc4tO4DsZhkygL8jBF5hTMB7sYbZaq5s9PtVk2SZUmj9+2TI08wvsRAnovH6hKb7YW5zTCRt4RCkg/70Y/K/W3bPHPaoArCQJ4LCycQ0STEYvY6c9/tZ06+x0Cei4cKJ6RSwPHjcruqyt22EFFuZpi9qcnez9z3wdxjI5OUH7PWnVIp6YVHIp7J3IzFgERC5uGiUbdbQ0T5mC1QW1okmMdiPl9jbkYmR0bsx5ht60kM5E7OEq0eCeTGkiX8/BB5nWXJZzWRkOKQHR0+jn1mRHJkxM62nTHDc+dGYiC3pVLyB9ve7okhdWPFCmDLFjkSkfdFo8CxY9Ir37dPbvtuWRqQWVfD8NC5kWycIzficbnqPHbM7ZZkWLdOik6sW+d2S4hoIswQe3u7lFQ2w+y+ZVn2vF4sxjlzD2IgNyIR+1PnocWgoVDmkYi8z7JkWH3ZMrnv+1KupqOzfr0kATCYewoDuWFZwHnnyW2TJk5EVIBo1F6W1tDg42AeidhbvyUSXJrrMQzkTrGY/LEuWOCJK85UCti1S2779gRAVMHMJivV1VLKddUqT5xaJs9s/dbeLl/NzVya5iEM5E6hEHDrrfIH6oErzlhMruRra30+x0ZUwcwa89payXfx7ci0mS/o6JAtn1k0yzMYyLN5qBiMccUVwOzZbreCiKYqFALuvltuJxI+DuaGOU+yZ+4JDOTZzJILD6wVWbFChuQ4JUXkf9Fo5jSzh3JqJ8+cJ03PPBZjQHcRAzng2VKE69bJvFptracGCIhoCsw0c22t3H/88QDkvpie+eioHdCp7BjIAc9ukmKWnN12mycGCIioQJYFbN8uI23Dwz5OfjNMz5wbQbiKgRzw5Lw4EQWTSX6rqZHkN18PsRvRqLyRlhZPjm4GHQM5YF9VAp76I3z++cwjEQVDKARceaXcDsQe5uYc+thjMroZiKsT/2Agd/LYEPv8+ZlHIgqOWEzmywcGAjS1bIppHTniqU5R0DGQO3lsiN1MO3H6iSh4nEvSzE5pvo97sZhsyn7TTcxmL6Oi7H6mlFoB4LsAPgjge1rrb2c9fz6A7wP4FIBhAF/UWv8q/dx/B3APgD8A+K9a613FaNOUOIfYiYhKLHunNMDne5iHQsCOHRK4q6tlR8m2NrlS8eUWcP5QcI9cKfVBAI8AuB3AtQBalFLXZr3sHgBvaa1rATwM4Dvp770WwF0ArgOwAsA/p38eEVHgmZ3SzPrygwcD0nk1nSKzeN73W8B5WzGG1hcCGNBaD2qtzwJ4EsDnsl7zOQAb07e3AvisUkqlH39Sa/2u1vokgIH0zyNwaJ2oEpj15eFwQKq+OVkWsGSJ260IvGIE8ssAvOq4fyb9WM7XaK3fB/AOgNkT/N7S82BBmGRSrs7NRS0RBZcz3gWukmM0KhutjI4GJBHAe4oyR14OSqk1ANYAwJw5c4r7w022OuCZOfLWVvlAT5/OaSWiShCNSqz76U+laExzs10UytcsC5gxQ/YyB+S2R86zQVGMQP4agE847l+efizXa84opaYB+Cgk6W0i3wsA0FpvALABAOrr63UR2m2LRIBTp4ANG2TT4EWLivrjp2LdOmBwUI5EFHyWJflhhw7J/TvukNuBuJCPRCTxbXRU6k53dMiVSyDenPuKMbR+DMBVSqkapdR0SPJaT9ZregCsTt/+AoCfaK11+vG7lFLnK6VqAFwF4GgR2jR5P/iBLOj0yNKzZ56Rqk/PPON2S4ioXCIRYOlSuR2o9eVmC9TqapnGXL8+YPMH7io4kKfnvKMAdgH4JYAfaK1fUEp9SynVnH7ZYwBmK6UGALQCeCD9vS8A+AGAFwE8A+A+rfUfCm3TpMXjcpVYXe2ZP67R0cwjEQWfZQFbtwKNjXL/+98PwMYqTpGIDKuHwzJ3QEVRlDlyrfVOADuzHvsHx+3/B+C/5PnefwTwj8Vox5SZYR/A3pqIiMgFlgUsXw7s3w+cPAncfjtw9GhARqHN/EEiIan6M2bI+TcQb849rOwGZCZjeKRHzqVnRJUrGgXmzZPbJ08GaIgdsCtoAqz+ViS+yVovOTM37pE58kWL5MLVA3l3RFRmliU1VG69FTh9OmAxzhSLSaWkA2WqvwHMZp8iJTln/lJfX6/7+vrcbkZJXXONJLvV1QG//KXbrSEiN9xyi4xCz54tdSUCsRwtWyplDzkwkz0vpdSzWuv6XM9xaN2jOjrkYtXXdZeJqCCxmIzMDQ8Dq1YFrGduOKc2GxoClt1XHgzkhoequ6VSEsBHRiRrlYgqUygEHDggObj9/QGbK3eKRGT4sb8/wFcspcNAbnhoL/JYTP6eZ89mQRiiSufc7nTTpoB2WC1Lzr3V1XLy88B52E8YyA0P7UVu1o4PD8vVOBFVtmhUeuUDAwHee+HAAann0dTkifOwnzCQGyaT0kOJFkuX8u+ZiOS0dOedcvu99wI68mw6U93d0iMP5JssDQZyDzI98vnzPXVdQUQuamuTgmj79gV0rtx0pnp65M2uXs1gPkEM5B70/POZRyIiywIWLJDbTzwR0LlyQHrmTU2ykJ5z5RPCQO5B8+dnHomIALvS4+BggOfKLQvYuNHOWfLQiiKvYiD3IJZnJaJcolHghhvk9sc+5mpTSsuZsxSLyVB7SwuDeR4M5OZqL5nkVR8ReZplAb/7ndx++ukAD687maShRIJD7XkwkJurvWjUM+vIiYjyeeIJ4MILJb7de6/brSkDMzRZUyPL09jZOgcDubnaC4U8s46cQ+tElM+iRcB118lts/tyoEWjkvx28qSMmrKzdQ7ufmai5YkTnlnr1dICHDsmRyKibDNmyPHNN6WD6pFTV2mY5Dez5s4DnS2vYY/cXO3t3++Z/cg3b5aVF5s3u90SIvKiRx+VkebBQXtr70CzLNmAoqNDbjOTPQN75B682jOj/eZIROQUCgGXXiqjzQcPut0aF5i9MQDuYQ4GcmGu9oiIyPuam4HeXjkSh9aJiPxoyRI5nndeBY4w9/TI/GNPj9st8QQGcg8y+XfHj1fgB5SIJqStDWhslNrrFTFP7uTcrTKZBFaurJBF9bkxkHuQyb9j/QMiysey7DyavXvdbUvZOSu/tbZK77y11e1WuYZz5B5kWcC6dZKR2tDgdmuIyKteey3zWJHMyXLdOrdb4hr2yD1q3Tqgv7+i/zaJaBx//GPmsSIdOCAnywcfrNi5SAZyjwqFMo9ERNk+8IHMY0Vybnva0iIrkCosoFfyf7+NyRJE5EOzZ2ceK5KpBWISizxS2KucOEcO2MkSALBjh7ttSXv++cwjEVG23/4281ixPFjYq5wYyAGguzvz6AHz58uykvnz3W4JEXnVkiXAqVP2mvKKVsGFvRjIAZmI9khPnIhoon71q8wjVSbOkXsUh9aJaDxnz2YeyaGCNlZhIPeohQvlqHVF/B0SERWX2VilszPwycwM5B51zz1Aba3srmryN4iInKZPzzySgynjeuSIJDNHo263qGQYyFMpe59bD3V9e3qAgQG5ze1MiSiXmprMIzmYMq7XXy/3A1yUg8lusZisOwSAGTM8s7dtJCL5d/v2ud0SIvKiVMrO0T1wwN22eJplyTGZlH80cz9A2CM33d3GRk+tPbQse56ciChbRwfw9tty+/LL3WyJx0WjQDgsxWICOk/JQG72DF2+3HNXaqZp5khEZPzwh3K84ALg8cfdbYunWVbmQvsAZrNzaD0alSF1D/XGjRUrgC1b5EhE5PThD8vxyisDPf1bHM7zvMlmBzwzlVoo9shNQgTguau0Bx+0N/UhIjIOH7ZXU/3+9+62xRec+5ebbHYPdt6mioHcMFdpHiq2v26dLEGrqfHU9QURuexLXwLefx+YNg3YtMnt1viMCebxeGBOrBxaN5qbgd5eOXrEgQOyBG1gAJg7NzCjQERUgGQSePNNub1wIbBokbvt8aWADa8zkBs9PVI0YNkyz/zHRiKyIcKuXUBDg9utISK3pVLAHXcA77wjW5cyyW2KzLB6QIbXObQOyKdjZARob/fUf6xlASdPSo+c8+RElS2ZlB64KRT1ta8xyW3KnHPmAcBADsgwy/r1ktXosf/Y++8HqqvlSESVKZkEbrpJLuwByZ0xI8NUoGQSWLpURmN9Wo+dQ+uAp4dZHnoIGBqSI5ehEVWeVAq4/XYZTgeACy8Etm/3XJ/Dv6JR2dQCAFpbfbmlNXvkgKeHWebOzTwSUWXp6LB74hdeCPzkJxxSL6oFC+Q4c6YsFfIhBnKPe/nlzCMRVYZUSjqLjz4q96uqgOPHmaVedG1tQFMT8NZbvi1aX1AgV0rNUkrtUUq9nD7OzPGaG5RSh5RSLyilfqGU+qLjuX9VSp1USj2X/rqhkPYE0U03yfHVV307fUNEk5RKAS0twCOPyHrx884Dfvxj9sRLwrKAjRt9XSSm0B75AwB+rLW+CsCP0/ezjQL4K631dQBWAPgnpdRFjufXaq1vSH89V2B7AqetTRJbTp4M9Ha6RJSWTAKLF8seH4AsM9u/nz3xksqeXk0mgZUrfdN7KjSQfw7AxvTtjQBWZb9Aa/2S1vrl9O3/BPAGgOoCf2/FsCxJqAQ4T04UdMmk1IwwS8zCYSnTzCBeZtGo1BXxSe+p0EB+sdb69fTtXwO4eKwXK6UWApgO4BXHw/+YHnJ/WCl1foHtmRqP74bz4ouZRyIKnmRSNukaGgJmzZIO4ubNnszBDT6TAGeOHjfu8jOlVALAJTme+qbzjtZaK6X0GD/nUgBPAFittf5j+uH/DrkAmA5gA4C/B/CtPN+/BsAaAJgzZ854zZ4cU65vZMTeIYefHiIqg1RKMtMff9zeAOWee2TKllzS1iYFPHwyZz5uINdah/M9p5T6jVLqUq316+lA/Uae130EwA4A39RaH3b8bNObf1cpFQfwd2O0YwMk2KO+vj7vBcOUNDcDu3dLrfV9++Qxj5RpBYBPfxo4dEgSXlIpXmMQBUUqBXzhC/ZpBwAaG1nsxXWWJXGhpUV65W1tnj7xFjq03gNgdfr2agD/nv0CpdR0ANsAfF9rvTXruUvTRwWZX3++wPZMTU+PZJbs2yeTUh67Cmtrk2bt3w/EYm63hoiKwVRrM0H8wguB++4DnnrK0zGjcrS2Slzo6vL8ibfQQP5tALcopV4GEE7fh1KqXin1vfRr/hJAI4Cv5lhmtkkpdQLACQAWgP9ZYHumJhKRSOlRlmVP1YyOutsWIipMMgnccotUaxsclMdmz5Y14rEYg7hndHfLkiFATrwezqMqqESr1noYwGdzPN4H4Ovp2/8bwP/O8/2fKeT3F41lSVbJ6tWSqRiPe2ponYj8LZWSIJ1KAU8+CQwPy+Pz5gGXXw5s2MA14p4TCsmcZiwGHDxorwf0YGxgrXXDFAWIxz03tA5IVSdArto5T07kH8kksGqVLCMzZs+W3cs8PvVKliUJ0ImEVH9rbpaeuccSohnInUxRAA+KRu2LwlhMslyJyJsOHwbuvluWkb35pgyh19YCt90mgT0WYw/cN5ybapkVTr290vHzSDBnIPcJM0+eSHCenMiLkkng3nuBs2el9/3WW/YceF0d8PTTDN6+5OzgNTfLOkGPTcEykBMRFSCVkjXfjz0mvW9j1iyZA1++nEPogbF5s1yl1dRI5R6PzHMykBuplD0/7oH/mFw4T07kDeZ00dAgpwzn/PecOcAXv8jgHUhmOPTkSZkrr672RK+cgdwwcx+AJ/5jcuE8OZG7TPa5qR1VWyt10WtqJIAvXMgAHmimN3XzzXK7ocETyW8M5IYzocGjLEvm2BIJzy5nJAqcsXrft90GXH21LDnm/HcFiEYli31kBFi/Xh5LJOS+iz0rBnLDJDSYDVQ8OsRudtV78kng/vt58iAqFTP3/dRTdtb5wIAc77xTOmTRqCdPE1QqzjgxY4Z9Vedyz4qBPJvHh9hjMdkhaXhYTiJ79rjdIqLgMMH7yBHgvfekHojB3jf9iWVJZ2/xYrnv8r7lDOTZPD7EHgpJcYnHHuP+5ETFYIL30aMSvH/2s8zna2pkYxPOfVOGeFyGaKqrgW98w9WRXAbybB4uCmOcOiXHp5+WprJ3QDRxJmHNJCAfP25X3zRqaqSQl2Vx+JzyiEQk63HnTuChh1ydK2cg96FYTEZ0hoelAEVvr9stIvI2Z/DOFbgbGwGlgPnzGbxpgkxZ71gM2LtXHjt40JW1wQzkTsmkbF3n8UmwUAi45hoZAnzvPbdbQ+Q94/W6w2F7R0EmrdGUmT+a/ftlrjORkHmYrVvL+gfFQO7U2irDJIODwIEDnv5kL1kigfz11+X6w8PXHUQl59xd7PnnpUyqM1ENsIM3AzeVxDvvyHHfvrKXb1Va67L9smKpr6/XfX19xf/Bhw/LxNhbb8l/Qmdn8X9HkaRSwE03yTXH0qUcXqfK4kxQu/JK6RANDJz7uqVLpUgLgzeVTCplb4ENyB9dCXrkSqlntdb1uZ5jj9zpwAEJ4oCMxXmYZck+xoODwOnTLNlKwZdvnnvfPjma3cWef55z3VRGZq68owP44Q9lvnN4mEPrrolEpBD+8eNyxvC4DRuA22+Xsr+dnZ4eQCCakrGS1EyC2pVXysUstwYl11iWzHGePi1fd9whcztlCuYM5E6W5atoGArJSezkSc8PIBBNiLMc6oMPAtddJ8tzDc5zk2eZfaYBmecp4zw5A7mTD3ZAyxaL2XsgM+mN/MjZ6z5yROa7TTnUs2eB9nZ5jsGbPK2tzR42mj1brkbLhIHcyePlWXMJhYDzzpO/HZZsJb8YqxQqwHKo5EOWlVnk44EHypaFzEDu5PHyrPmYHdF4wiMvSyblYjMUktvZRVmYYU6+19NjJ0yPjJTt1zKQO/mgPGsu5oT35JPAl78MLFrkbnuIDGfw3rVLhstNAF+6FNAauP56ZphTQEQiwHe/C7z2Wll/LQN5Nh/Ok0ejwD//syTch8PAs8+yd07ll11NrapKKlYmEnbwNkvEGLgpkCwLmDNHAvl555Xt1zKQZ4vFZMN4lzeKnwzLkhGdz35Wms25cioHc83b3Axs3mwHbSczwBUKMXhThbj00sxjGTCQB8SiRcCddwKbNgEXX+x2ayiIssugai0Z5mYDKIA1zInwk59kHsuAgTxbNCpjgwcP+m4915Ejcty2zXdNJw9yDpWPjtpz3E5NTZJZfuONcp+Bmyre3LnA228DF1xQtpKbDOTZLAt44QUZI1y1yvObpzg98YQMr4+Olr2wEAWISVAbGTl3WZizDOrChbJa07J8MwtFVHqf/jTw858Dv/512YrCMJDnsm4dcOwY0N9f9l1sCrFoEXDffVIJa2CAZVtpYrKT1LZty+x5L10qtcuTSZZBJZqwiy4qW1EYBvJcDhyQFPCmJt+tKW9rA556SjZTeeopu8dElM0E8FxJaswuJ5qiEyfk+PbbUmd4x46S/0oG8lyamyWDp7vbd2cwywI+/3nplQ8OsldOmZJJoLVVBp0efJBJakRFV1srWaDnnw/cf39ZfiUDeS49PXKGW7bMN8PqTm1t9vDotm3slVc60/MG7N734KDMHIXDwJIlDNxERWPmpd59F3joIWDFipL/SgbyXHxaqtWwLGD7dkl4GxgAWlpknS9P1JUjXznUtWuB6dOlR37ggK/qHhH5w/XXS48csIe5SoyBPBfLkjOczyq8OYVCwN13S22bREJ6ZMwsDjZn0poZkTEBPFfPm6V8iUpozhzgnnvK8qsYyHNJpYDVq+0JRB8OrwNy0t67Vy4OTUYyBYuz533ihN0RAJiwRuSKgwflePq0TNNy+ZlL4nEJ4nV1kvjmU5YFLF8uJ/dt2+TikEuHgsEE8FdeAU6ezMw6b2yU/3cGbyIXvPKKHM8/v2zTswzkuUQidt3JMl1RlUo0CmzZIolNDQ0yL8pg7i9jbUYC2D3vqipmnBO5xmw+8KEPAb/9rXwIy/RBZCDPxbKAjRvl7DkyUrYye6VgWcDTT0sQHxpiMPeTsdZ5m2vLBQu4KoHIE8yGWzNmANOmAe3tZfvVDOT5WJb8h7S1ydHHvfJQSIL34sUSzG+/HTh6lCd/L8nV6wbkvABwnTeR5zi3/+vpkfuAdP4AqUPy139dlqYwkI/FFIbx8Ty5EQrZqyJOnpSiMU89xWDgtrHqmre32xf1DNxELjJB28x5x2ISG/btA3bvliGzmhp5bvp0mR9/+OGyNY+BfCymMAwgQ+0+P5Nu2CBLkIaHJaAzmJefcyvQEyeAV1+VCytj6VLZjIS9bqIicgbiXB8qU/KwuxuYPdvuaW/ebL/GDI+NjNi3AeklnTkjiUgAcPasfJ04UZZiMAADeX6plPyHhcMSzH20eUo+oZDMtzqDOUu4lsfhw3IOuflm4PHHM5/jMjGiCRgvGDtLGGZ/kOJxmSbdvVtOgC0t0lEzP6u1Vc7zg4PAF78ogdokPANy7u/slNebghw33ij7cYyOShD/6EeBd96R58Lh8hYU01r77utTn/qULrnOTq0Brdvb5fbQUOl/Z5n092s9e7a8vdmz5T6VRn+/1k1NWtfU2P/egNaLF2vd2Kj12rWB+tOiSjE0lHlezL4/3msm85zR3m6fk3P9DvN8rvP20JDW4bD9fFOTHDs75fn+fq3nzZPH7rtPHj90SOvaWnksHLZ/lvk5tbXyfYsX2z8XkA92CT7UAPp0npjIHnk+kYhkhh08KFd5AeommZ45M9mLz5m05lwmdvPN9rTZiRO+LRhIfuEcKp7IB/vwYeArX5GhoY4O+ePM1QPOtZRi7Vq7x2vuZxfVikQy7wPy+t5embZ0fr95bmREEo1Nz3bvXjk6q1s5v888vnjxue2zLMkWTSRk/qq7W/bSaG6WHaYiEWDePOmR79olCSvxuJRHrK2V7+vsBKqrgW98Q/YbHxiQf2OT3DJzJvDWW1LEodwf7nwR3stfZemRa21ftTU1lef3lVl/v9bV1XZPkb3DqTMdAudFPyD/pk1NHPWgLPl6nbmeG+u1+b536VK7JzmR319XZ//Rml6qGZU097WWP2hnrzZfj9p57jTPmV7s2rX2UJX5+eYDtHatfLW32z3szk77+509Ya3tn9Pfb7++sfHcXrSz7WvX2o8532N/v/3vYNrU2Wl/n/lwO99bf788Hw5LD76Eo7dgj3yKurslaeG663y9ljwfsyzN9My7umT+dvt21uGeCGfv+/jxzLrmCxYwYY3GkN2DzfWc6ZE6k6vGy9Mxa5kXL5b7uTbtyFWCOh6XHvlNN8k8cnNz5uZRpnd+5Ig8VlsrPWnA7tFGIpm99aYm+zVDQ/I9AwPy+qoqmWO+7jp7udaMGZnrLc1898iIzGmPjACbNtk94R07MneqjEblZwwNSQLQkiWZHz6zptMczXszR8uSE6JzFMKMLlRX28vMmpvl95nXOJOM3Dpx5ovwXv4qW48815VlAPX321NBgNbnnScXl3SuoSG5AG9sPHdqLByWTkFA/0xoPKYH198/fs9svB55e7vdq3b2UMeaQ9ba7pXed1/+oSDTC811Tss3Cmm+J3uIydmjdfaanT/b+bj5kJh2ZvfKnUNazp/pnMt2/v6JzM1P5N/cBzBGj7yggApgFoA9AF5OH2fmed0fADyX/upxPF4D4AiAAQBbAEyfyO8tWyA3f0TO4ZaAGhqSz/5558lbnTZNAhWHhO3gvXixnbTm/Fq6lAE8UCYTkJ3M+cIEo+yh3Xy/J9drnMHPJG7lC265fqZzWHoyvzc7UI73PdlD6s4LDudrsh/P92+c/VqfB99iKmUg7wTwQPr2AwC+k+d1v8vz+A8A3JW+/S8A/mYiv7dsgdz8UZd47sNLDh2yg3mlZrU7p+vuuy9ztAKQ5NbGRnmOATyAnD3WyVzAmz8cM0c73kjeeAE5X0CbSHBjAAycUgbyJIBL07cvBZDM87pzAjkABSAFYFr6/mIAuybye8veIw9wTzyXQ4e0njXLPhfV1AQ7YGXn2WQnrJl/A7NkrNIubAJlMkEwV498vO939srNH1K+8weDLU3CWIG80GS3i7XWr6dv/xrAxXled4FSqg/A+wC+rbV+GsBsAG9rrd9Pv+YMgMsKbE9xmUQI5xKFCshcWrRIVq984QtSgfDkSclB2bRJEuH8vkzNuYd3VVVmopphEtZGR+X1sZj/33dFGKtoSK4kr2zOP47Nm/MXFsn3/c7kKfP6fIVBTDIVUYHGDeRKqQSAS3I89U3nHa21VkrpPD9mrtb6NaXUPAA/UUqdAPDOZBqqlFoDYA0AzJkzZzLfOnWWlbn+0ax5rIBgblnA1q0SwPbulSTQgQFJRL38cklu9cOuW+a8fPHFwM9+Jsm8u3ZJZTtn8OamJD5nAvhYGd7xuHyOm5ryB9fWVvnDMH8c2RsmZQfqbNnBmYGaykBJj32K36xUEsAyrfXrSqlLAfRqrcfstyil/hXAdgBPARgCcInW+n2l1GIAHVrr28b7vfX19bqvr2/K7Z6Uri6JWHV1Uoavs7PiPpyplLztbdskmBtz5gBXXCE13L3QWzXn8uuvB+6/X2qWm6CdbfZs4K67uIe3L+XqdZvPaXu7BF+zVCi7mMlYJT6BzB45a+aShyilntVa1+d8rsBA3gVgWGv9baXUAwBmaa3bsl4zE8Co1vpdpZQF4BCAz2mtX1RK/RuAp7TWTyql/gXAL7TW/zze7y1rIM/eqq5ChtdzMQF969bMjT4++lHgwx8GLrlEihqVs6fuXMt99KhMBcyenRm8Z8+WvQtMj/yNNzhU7hu56meboO28qDaf04YGYN06qf9gNhOosAtvCqZSBvLZkMzzOQBOAfhLrfWbSql6AP+f1vrrSqmbATwK4I8APgDgn7TWj6W/fx6AJyHL2I4D+LLW+t3xfm9ZAzkwsSv5CmIC+pYtwOnT5z4/bx4wa5bs5rdgAfD730uNiT/8AbjsMhmWn2xnJ5kE7r1XRk7POw+49lrg5ZeB9947d/vPr31NzuELFzJo+0a+z1hHhz1UboLyWJ/HlSvtOXBTkISfWQqAkgVyt5Q9kOfqAdCfAnpvL/D669Ijf/NNKVc8EZddBnz84xKYzfz0iRMyNA4A//EfwPvvS974K69IGeN8GhvlAoHD5D6RHYzz9bJbWmS+urZ2YpmWZmh8wQJ/JHEQTdBYgZwlWiciEpGu4MhIIEu1TlV2dUIgs+ecr0f+xhvSk3/tNfkCZNjb2L8/9++bORO48srMHvn113Mq05eys7+zk8hMhnkiYeen9PSMfyEdCgF79pSu3UQexEA+EcPDMo7c339uFitlCIWkhz4WZ7BXamI98qoq7yTVUQHMrlzr1tn7OwPnZns7M8y7u+38FCI6BwP5RLS2ShA3hfOpIBMJ9uRTuZLTnM+tWiWfJcDevjLXXHf2Zha8eCbKi4F8Irq7ZeK3v1+KRJg9cjmWS2TLLrhiPicmWMfj8hmqq5PP1FjFVRi8iSaMgXwizH6fpuDEWJWdiCqVGQ4Ph2ULSbOt5fr18rmJRuV15iJ4vOIqRDQhDOQT5dyb1vQ0iCqFM8t8eNie5z5wwP4sjIxIQZZ8mYfZvWz2uomKgoF8Mpzzf0SVxDkM3tsrPW8z3WSsXy8JbM4gHo3ywpeoxBjIJyMet4tTMHudgix7nbdzGLyhQYL4ww/LMgNnkM4O2Ox1E5UcA/lkmPXk5jZRUGUnojkDsklaO3GCG4QQeQAD+WSYyiPxuNstISqeXEvGxkpEY5IakacwkE/WePsRE/lJ9pKx0dHx6yVwuJzIUz7gdgN8p7lZCnvv2CFVqoj8zCwZq62V+8ePy4Vqa6scOfpE5HnskU9WT49dDDwaZV1n8rbxdu4zw+Nmm17ncdkyDp8T+QB3P5usVEpOcocOAffdx+Vo5E0mgI+M2MvCnMPh3JqXyFfG2v2MQ+uTZVnArbfat4m8yJnL4dycJPt5Dp0T+R6H1qeCRS7I65qbpXDLihXAM8/IyJGz4hozz4kCg4F8Kpi1S16Rb4i8p0eS2M6elT29gcwiRvwbJgoMDq1PRSoFdHXJkchNZoh89erMv8dIRIbUzUbv4TB730QBxR75VJiT58gItzQld0Uidu3zePzcHncqJevC+TdKFFgM5FPh3O2JxWGolMbLLrcsYONG+zW5nuffJlGgMZBPBbc0pVJyBu+JVBJksCaqaAzkhRgelmHN5mYOW1LxOIO32ahnaEgeq6rKv983EVUkBvJCtLbaNap37HC3LRQczqVhJmB3ddnPcwtdInJgIC9Ed7cc162TEy0TiqgY8g2VNzYCy5dzKoeIMjCQFyIUkkQj5+5R7CnRZI2X0OYsQMQLRSLKwnXkhYrF7N2jxtr6kQjIXYNgvHKppofOIE5EOTCQF2p0VI4DA1JNi2gsuYK2Kd7CIXMimgIOrReqqkqOrJxF40mlJPs8HM4cveHyMSIqAAN5oTh/SRMVi9nZ562tkl/BvxkiKhCH1gvF+UuaKDMNM2+eXVKViKhA7JETFct42edmGubzn7frnxMRFYiBnKhYxiunymkYIioBBnKiYnFWZMuFSW1EVAKcIy+GVAro6JAv7lFeuSzL3uiEfwdEVCYM5MUQjwPr18tXQwOQTLrdIiqlXEVdjPGKuxARFRmH1ovB7FC1aRPQ3y9Li7iJSnCNNRc+3vA6EVGRKa21222YtPr6et3X1+d2M86VTAJr1gBKAY8+KrXYKThSKVkLbpaRcUtRIioTpdSzWuv6XM+xR15MoRDwoQ/JGmH2yoPHTKEAUp0tkZDbHR2uNYmIiIG82MzWpuZIwZBKyfTJ2rXSEx8dtQM5EZGLGMiLbfZsYNkyOZL/5CvqYnrjnZ0SzFMpFnUhIk9gIC+28YqCkLfl+//LTmLjmnAi8ggG8mIzGewjI9JrYyKUv+TLOmfgJiKP4jryYrMsKcO5fj3XEntdMgmsXAkcPmyvC+cmOETkM+yRlwLXEvtDa6usMHjpJWBgANi9G9i8mUGciHyFPfJSYK/OH7q7gaYm4Lbb5H4iIevEiYh8hIG8lMzQLUu2elMoJGv9OzpkXTgRkQ8VNLSulJoFYAuAKwD8CsBfaq3fynrNcgAPOx6qA3CX1vpppdS/AlgK4J30c1/VWj9XSJs8IZmUYdu33gIOHQLOngX27HG7VZSPZcmQull2RkTkI4X2yB8A8GOt9VUAfpy+n0FrvVdrfYPW+gYAnwEwCmC34yVrzfOBCOKAPff62mtyn6Va3Wc2Okkmc294wukQIvKpQpPdPgdgWfr2RgC9AP5+jNd/AcCPtNajBf5ebzNV3WpqgEceYXDwArM+vLdXLrIALicjokAoNJBfrLV+PX371wAuHuf1dwHIrl36j0qpf0C6R6+1fjfXNyql1gBYAwBz5syZeovLwcy9OteRc015+aRSUoHt+HFJXguF7CHz5mapvMchdCIKiHF3P1NKJQBckuOpbwLYqLW+yPHat7TWM/P8nEsB/ALAx7XW7zke+zWA6QA2AHhFa/2t8Rrt2d3Pcunqkp6gKe1JpWf+zQFJYmN+AhH5XEG7n2mt86bzKqV+o5S6VGv9ejoovzHGj/pLANtMEE//bNObf1cpFQfwd+O1x3e4prz8IhEZEdm3D3jvPY6GEFGgFZrs1gNgdfr2agD/PsZrWwBsdj6QDv5QSikAqwA8X2B7vCXfBhxUWpYl+8HX1UkwZ4U9IgqwQgP5twHcopR6GUA4fR9KqXql1PfMi5RSVwD4BIB9Wd+/SSl1AsAJABaA/1lge7zFJFitXn1uljSVVk8P0N8vBV84GkJEAVZQspvWehjAZ3M83gfg6477vwJwWY7XfaaQ3+95kYidJR2Pc468mLJHO7LvO6c0OBpCRAHGWuulZFnAxo2SOT00JBXEolEGlkKlUkBLi5RUHRqSfcFHRmSjGsBeD84LJyKqAAzkpebcDQ0ARkclg52mLh6XIA4A27bJhidr18owenOzu20jIioz1lovh0gEqK2V28ePu9uWIIhEgPZ2WVo2MCABvKpKpjB6etxuHRFRWbFHXi533gkcPQosWMDlUFORPQfe0ZH5GCAjH0xsI6IKwx55OcTjUqRkxgw5cjnU5JkVAPG4XTcdsOfDWSudiCoUe+TlEIlIMtboKHDjjew1jsf0tBsagHXrZBTjM5+RdeENDXZQB5jQRkQVj4G8HEwvsatL5nbZaxybCdR1dbIWPJEAfvhDuf3gg7ISAOAFEREROLRefqOjubfRrHRmuDyVkgDd2SkBPRyWXnc8Lklt3d0cRicicmCPvFyiUZkjP3VKepvbtwNPPcVgZIbRzTrwkRE7ac2yMjc82bHDvXYSEXkUe+TlYnqRyaTc37+fSW9A5nx3Z6eMWLS1ScGXZJKjF0RE42CPvNwefBB45RVg9mypSlbpS9Gam6WMbUuL/Ju0tMjjiQTQ2iprwwEmtRER5cFAXm7PPAOcPClffX1SXrQSg5RzSH3nTmDZMrmdSABLl8r9lhY5MqmNiCgvDq27ZeZM4J57JHhVytCxM6HNOaTe3m4vzwMkeHd0AKEQk9qIiMbBHnm5RaPAli2ylKqnR4bXZ8wIdq88V0Lb6KhkpLe0yL9DW5sE9M5O9sCJiCaBgbzcLEuCWnOzBPFK2C/b9L7NxiZmCR4AbN4sFzcAtxwlIpoCBnI3HDggQbyuTiqXOWuIB0UqJdu3AnYCm5kPv+462URmYEAe55ajRERTxkDuhkhEMrV37gS+8hUJaCMjMi8cFPG4vXXrwYPS8wZkGmFkxN61zPTGiYhoSpjs5gbLkjKjS5favdIgJLxlV2cLh+XxREJ656bnHY3KXPjGjcEahSAicgEDuVssCzjvPPu+KRTjZ84dyixLeuGNjfKcyUgHWGKViKiIGMjdFItJoLv5ZllqZfbY9pNkErjlFgngzc2ZWeeWBSxfLrerqtxrIxFRgHGO3E2hELBvnwRBk8Vt5pP90lttbZWh80QCeOEFe2eyri4J6KbGfNAz84mIXMJA7gXHj9u3zXyyXxLfurslee30aUneM/XjnfuFMyOdiKhkOLTuBbGYLMcyenu9PcTuTGoLhaQS28mTktwWidjbkLIXTkRUcgzkXhAKAYcO2Vne+/bJGvPDh91tl9Phw8A118jRmdTmtGSJTAkwmY2IqGw4tO4VJsu7pUWG14eHZZ31Sy95IyCa9e5f+YpcdAB2j5vz4ERErmGP3EtMMJ87V+6/9Zb7e5abYXSzjOy22+Qio7dXjgB74ERELmIg9xrLAnbtkmH2L31J5s+XLCnfOvNkEli50v59Zhj9E5+Qee+ODnuf8NbW8rSJiIjy4tC6F4VCwJ49Mid9+rR83Xuv9IJLLRqVof2zZ6UNzc3ye1tapF2AZKo7j0RE5Br2yL0sHgcuvFBu/+pX5SkYs2CBHM+eld/V0yO9754e+zWhELBjhx3YiYjINQzkXrZokawxr6sDTp2STUg+9SkZ6i5VQG9rk2H9/ftlWJ9LyYiIPI2B3OtCIdn21KwzP31aks8+//mpB3OTwJZMSi+/rc3u7VuWzMkDUmUOYCIbEZGHcY7cDywL2L4dWLMG+PnPgXfekR5zS8vUyrmaBDazlapx8KAE8ZYW4Ngxu1IbK7MREXkWe+R+Yeqyr1ljP5ZIAA0NY2e0O6uwmYz0hgYZLu/uliC9eDFQUyM/b/16mQ/fuJFD6kREPsAeud+0tcm8eSIBzJwJ9PcDCxfK7c9+Fpg9W15XVSUZ6Kb3PTICbNkir3/pJeDuu+W11dV2gZdwWHrkkYi9NpyIiDxNaa3dbsOk1dfX676+Preb4Z5USgL0qVPAI4/kf104LFnoZgvR9eslcA8Nyf32dhlGj0bldW1tnAsnIvIgpdSzWuv6XM9xaN2PTG+5o0OOH/mIPP6hD9mvufxy6bV3dQGjozL/vXatDJubxDmzZWoiIQGeQZyIyHcYyP3MsmQe++hRqcv+yU/az5mRlrlzgZ/+VIL13r1S4GVgQJa0JRLyGs6FExH5FufIg8AUaEkmpQKc1tILf+01GX7/wx/kdQMDwNtvS+/76aeld27mw4mIyJfYIw+SUEiWlO3bByxfbj9+5owc/+IvpCfe0yOv5fpwIiLfY488qNraJMltdFTumyx2Bm4iokBhIA8qy5JkOCIiCjQOrRMREfkYAzkREZGPMZATERH5GAM5ERGRjzGQExER+VhBgVwp9V+UUi8opf6olMpZAzb9uhVKqaRSakAp9YDj8Rql1JH041uUUtMLaQ8REVGlKbRH/jyAvwCwP98LlFIfBPAIgNsBXAugRSl1bfrp7wB4WGtdC+AtAPcU2B4iIqKKUlAg11r/Ums9xmbYAICFAAa01oNa67MAngTwOaWUAvAZAFvTr9sIYFUh7SEiIqo05ZgjvwzAq477Z9KPzQbwttb6/azHc1JKrVFK9Sml+obMNpxEREQVbtzKbkqpBIBLcjz1Ta31vxe/SblprTcA2ADIfuTl+r1EREReNm4g11qHC/wdrwH4hOP+5enHhgFcpJSalu6Vm8eJiIhogsoxtH4MwFXpDPXpAO4C0KO11gD2AvhC+nWrAZSth09ERBQEhS4/u1MpdQbAYgA7lFK70o9/XCm1EwDSve0ogF0AfgngB1rrF9I/4u8BtCqlBiBz5o8V0h4iIqJKo6Rj7C/19fW6r6/P7WYQERGVhVLqWa11znotrOxGRETkYwzkREREPsZATkRE5GO+nCNXSg0BGAGQcrstJWQh2O8PCP57DPr7A/gegyDo7w8Ixnucq7WuzvWELwM5ACil+vJN/AdB0N8fEPz3GPT3B/A9BkHQ3x8Q/PfIoXUiIiIfYyAnIiLyMT8H8g1uN6DEgv7+gOC/x6C/P4DvMQiC/v6AgL9H386RExERkb975ERERBXPF4FcKTVLKbVHKfVy+jgzz+vmKKV2K6V+qZR6USl1RZmbOmUTfY/p135EKXVGKRUrZxsLNZH3qJS6QSl1SCn1glLqF0qpL7rR1slQSq1QSiWVUgNKqQdyPH++UmpL+vkjfvq7NCbwHlvTn7lfKKV+rJSa60Y7p2q89+d43eeVUlop5bsM6Im8R6XUX6b/H19QSv2fcrexUBP4O52jlNqrlDqe/lttcqOdRae19vwXgE4AD6RvPwDgO3le1wvglvTtDwGocrvtxX6P6ee/C+D/AIi53e5iv0cAVwO4Kn374wBeB3CR220f4z19EMArAOYBmA7g5wCuzXrN3wL4l/TtuwBscbvdJXiPy83nDcDf+Ok9TuT9pV/3YQD7ARwGUO92u0vwf3gVgOMAZqbvf8ztdpfgPW4A8Dfp29cC+JXb7S7Gly965AA+B2Bj+vZGAKuyX6CUuhbANK31HgDQWv9Oaz1athYWbtz3CABKqU8BuBjA7vI0q6jGfY9a65e01i+nb/8ngDcA5CyC4BELAQxorQe11mcBPAl5n07O970VwGeVUqqMbSzUuO9Ra73X8Xk7DODyMrexEBP5PwSABwF8B8D/K2fjimQi7/GvATyitX4LALTWb5S5jYWayHvUAD6Svv1RAP9ZxvaVjF8C+cVa69fTt38NCWTZrgbwtlLq/6aHTbqUUh8sXxMLNu57VEp9AMBDAP6unA0roon8P/6JUmoh5Mr6lVI3rACXAXjVcf9M+rGcr9Gyre87kG17/WIi79HpHgA/KmmLimvc96eU+jMAn9Ba7yhnw4poIv+HVwO4Wil1UCl1WCm1omytK46JvMcOAF9Ob7+9E8D95WlaaU1zuwGGUioB4JIcT33TeUdrrZVSuVLtpwFoALAAwGkAWwB8FR7a47wI7/FvAezUWp/xaoeuCO/R/JxLATwBYLXW+o/FbSWVilLqywDqASx1uy3Fkr6A7oacT4JsGmR4fRlkRGW/Uup6rfXbbjaqyFoA/KvW+iGl1GIATyil5vv9HOOZQK61Dud7Tin1G6XUpVrr19Mn+FxDPmcAPKe1Hkx/z9MAFsFDgbwI73ExgAal1N9CcgCmK6V+p7XOm5xTbkV4j1BKfQTADgDf1FofLlFTi+U1AJ9w3L88/Viu15xRSk2DDOkNl6d5RTGR9wilVBhywbZUa/1umdpWDOO9vw8DmA+gN30BfQmAHqVUs9a6r2ytLMxE/g/PADiitX4PwEml1EuQwH6sPE0s2ETe4z0AVgCA1vqQUuoCSB12v00jZPDL0HoPgNXp26sB/HuO1xwDcJFSysynfgbAi2VoW7GM+x611ndrredora+ADK9/30tBfALGfY9KqekAtkHe29Yytm2qjgG4SilVk277XZD36eR8318A8BOdzrbxiXHfo1JqAYBHATT7cG51zPentX5Ha21pra9If/YOQ96nX4I4MLG/06chvXEopSzIUPtgGdtYqIm8x9MAPgsASqlrAFwAYKisrSwFt7PtJvIFmU/8MYCXASQAzEo/Xg/ge47X3QLgFwBOAPhXANPdbnux36Pj9V+F/7LWx32PAL4M4D0Azzm+bnC77eO8ryYAL0Hm8r+ZfuxbkJM9ICeLfwMwAOAogHlut7kE7zEB4DeO/7Met9tczPeX9dpe+CxrfYL/hwoyhfBi+hx6l9ttLsF7vBbAQUhG+3MAbnW7zcX4YmU3IiIiH/PL0DoRERHlwEBORETkYwzkREREPsZATkRE5GMM5ERERD7GQE5ERORjDOREREQ+xkBORETkY/8/ouEj+F/mo3wAAAAASUVORK5CYII=\n",
+                        "text/plain": [
+                            "<Figure size 576x576 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "# First, consider two initial conditions (regular and chaotic)\n",
+                "\n",
+                "count = 1024\n",
+                "\n",
+                "plt.figure(figsize=(8, 8))\n",
+                "\n",
+                "x = torch.tensor([0.50000, 0.0, 0.05, 0.0], dtype=dtype)\n",
+                "orbit = []\n",
+                "for _ in range(count):\n",
+                "    x = mapping(x)\n",
+                "    orbit.append(x)\n",
+                "q, p, *_ = torch.stack(orbit).T\n",
+                "plt.scatter(q, p, s =1, color='blue')\n",
+                "\n",
+                "x = torch.tensor([0.68925, 0.0, 0.10, 0.0], dtype=dtype)\n",
+                "orbit = []\n",
+                "for _ in range(count):\n",
+                "    x = mapping(x)\n",
+                "    orbit.append(x)\n",
+                "q, p, *_ = torch.stack(orbit).T\n",
+                "plt.scatter(q, p, s =1, color='red')\n",
+                "\n",
+                "plt.show()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "3abcd814-9305-4e11-82a8-449c2ffae2db",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAABIYAAAEvCAYAAAAwxMqBAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8qNh9FAAAACXBIWXMAAAsTAAALEwEAmpwYAAAjoklEQVR4nO3dfZBl6V0f9u9vNNOgUSTk7V47saSexoWcRDhlIB1FFE5iA8Gy7PLa8Uug7paVbSfNSnYydtkhQFfhcspdFWzKZFL2KpkyM0HMNZjClk0FBQVhKk5SBXGvIWaFUCFj9egF0GwvKFqaqFfWkz9uj3Zmp9/vPff186k6dfuce+85T2/N3dP97d/ze6q1FgAAAAAWz6VJDwAAAACAyRAMAQAAACwowRAAAADAghIMAQAAACwowRAAAADAghIMAQAAACyoy5MewINWVlba2trapIcBAAAAMDeeffbZ51trjx/13FQFQ2tra9nZ2Zn0MAAAAADmRlXtHvdc51PJqurtVfWRqvpoVX1719cDAAAA4Gw6DYaq6lVJ/naSP5TkLUm+pare0uU1AQAAADibriuG3prko621X26tHST5oSRPdHxNAAAAAM6g62DoDUk+/sD+Jw6PAQAAADBhE1+uvqo2q2qnqnbu3bs36eEAAAAALIyug6FPJnnTA/tvPDz2Ra21m6219dba+uOPH7lyGgAAAAAd6DoY+qdJ3lxVX15VS0m+OcmPdnxNAAAAAM6g02Cotfb5JH8+yQeSfDjJD7fWPtTlNSet309WVpKqwbayMjgGAAAAMG0ud32B1tr7k7y/6+tMg34/eeqp5KWXXj62t5dsbAy+7vUmMy4AAACAo0y8+fQ82dp6OBS67+Bg8BwAAADANBEMjdDduxd7DgAAAGASBEMjtLqafEv6+XRW8oVUvpDKp7OSb0k/jz026dEBAAAAPEwwNEJ33tHPrTyVx7OXSlJJHs9ebmcj7/iNvibUAAAAwFQRDI3Q73v/Vr40jzYZ+pIc5L/9V1v6DAEAAABTRTA0Sic0ElrNXX2GAAAAgKkiGBql1dVjn7qb1bSWVD26razENDMAAABg7ARDo7S9nVy58sjhz2Up35ntY9+2t5dsbAiHAAAAgPESDI1Sr5fcvp0sL6claUnuZTlP5VZ+ML0T33pwED2IAAAAgLG6POkBzJ1eL+n18qpLSWvne6seRAAAAMA4qRjqyAnthkb6HgAAAICLEgx15Jh2Q8daWhq8BwAAAGBcBEMdeaDd0KmWl5NbtwbvAQAAABgXwVBX+v30ttby/AuX0q6tpd3pp7U8tN25MwiF9vaSJ588eil7S9oDAAAAXREMdaHfTzY3k93dQQK0uzvYfyDZ6feTp54ahEJncT88eu1rBUQAAADAaAiGurC1lezvP3xsf/+h9ei3tpKXXjr/qV98MdnYEA4BAAAAwxMMdeG4decfOD7M0vQHBw9lTAAAAAAXIhjqwnHrzj9wfNil6YcJlgAAAAASwVA3treTq1cfPnb16kPr0Z93OftXGjZYAgAAABAMdaHXS27efHit+le/+pGXnHU5+1daWnooYwIAAAC4EMFQl37rt17+em/vkZXJer3k+efzyDL2Ry1pf9/ycnLr1uC9AAAAAMMQDHXluJXJrl8/12nuh0f3A6L7y9ZXHb2trFixDAAAADgbwVBXjusOvbd37uSm30+eemrw1tMIjgAAAICzEgx15aTu0Odca35rK3nppSHHc2hvL9nYEA4BAAAAgqHunNQd+pxrzY96afqDg3NnUwAAAMAcEgx1pdc7fsmxc64138XS9KMOmwAAAIDZIxjq0o0bydWrDx+7evXca81vbydXroxwXEkee2y05wMAAABmj2CoS71ecvNmcu3aoPPztWuD/XOuNd/rJbdvH1+AdBF7expUAwAAwKITDHWt1xuU/KyuDuZvbW1dKHW5v2x9a0dv95ezH4X7K5u99rUCIgAAAJhngqGu9fvJ5mayuztIcHZ3B/sjTlxOCo6qLnbOF18cBEQqigAAAGA+CYa6trWV7O8/fGx/f6zLgo26ebWKIgAAAJgPgqGuHbf81xiXBdvevnjV0ElefDHZ2BAOAQAAwKwSDHXtuHKdLtagP0avlzz9dDfnPjg4erqZKWcAAAAw/QRDXdveHsmS9cN65pnRNqg+i709FUUAAAAwzToLhqrqb1TVL1bVP6+q91XV67u61lQb0ZL1oxrKaSubveY1o73mwcFY2ykBAAAA51CttW5OXPVNSf5xa+3zVfXdSdJa+29Oes/6+nrb2dnpZDycXb+fXL8+qPgZharkC18YzbkAAACA86mqZ1tr60c911nFUGvtf2utff5w96eTvLGrazFax1UW3bmTXLrAv5jW9CACAACAaTSuHkMb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\n",
+                        "text/plain": [
+                            "<Figure size 1440x360 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "# Compute and plot the last gali index at each iteration\n",
+                "# Note, running minimum is appended at each iteration\n",
+                "\n",
+                "plt.figure(figsize=(20, 5))\n",
+                "\n",
+                "x = torch.tensor([0.50000, 0.0, 0.05, 0.0], dtype=dtype, device=device)\n",
+                "vs = torch.eye(4, dtype=dtype, device=device)\n",
+                "out = []\n",
+                "for _ in range(count):\n",
+                "    x, vs = tangent(x, vs)\n",
+                "    res = gali(vs)\n",
+                "    out.append(res if not out else min(res, out[-1]))\n",
+                "out = torch.stack(out)\n",
+                "plt.scatter(range(count), out, color='blue', marker='o')\n",
+                "    \n",
+                "x = torch.tensor([0.68925, 0.0, 0.10, 0.0], dtype=dtype, device=device)\n",
+                "vs = torch.eye(4, dtype=dtype, device=device)\n",
+                "out = []\n",
+                "for _ in range(count):\n",
+                "    x, vs = tangent(x, vs)\n",
+                "    res = gali(vs)\n",
+                "    out.append(res if not out else min(res, out[-1]))\n",
+                "out = torch.stack(out)\n",
+                "plt.scatter(range(count), out, color='red', marker='o')\n",
+                "               \n",
+                "plt.show()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "ce599a3d-c656-408d-8d7d-37f02241decf",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAbsAAAHLCAYAAABRSzbfAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8qNh9FAAAACXBIWXMAAAsTAAALEwEAmpwYAAEAAElEQVR4nOydeXhdVb3+PzuHpGlOk54mTRs70FJaCqW1gGGUqYggsyDiRRQUBBy4gAKKFn7CBRRBFBBEUUGQ4QoIMggyXArIKAHpbSkUSmkp7e0Y0qQnpAnJ/v3xrm/WOqcpKk1LWtb7POc5J3tYe+19Tta73u+0kjRNiYiIiIiI2JRR8mF3ICIiIiIiYn0jkl1ERERExCaPSHYREREREZs8ItlFRERERGzyiGQXEREREbHJI5JdRERERMQmj0h2ERERERF9DkmSXJokyatJkvxvkiR3JUmSW5f2ItlFRERERPRFPAxMTNP048BrwPfXpbFIdhERERERfQ5pmj6Upul77s9ngRHr0l4ku4iIiIiIvo7jgQfWpYHNeqkjEREREREbMT7zmc+ky5cv79U2X3jhhZeBtmDTtWmaXmt/JEnyCFDXw6lT0zS92x0zFXgPuHld+hLJLiIiIiKC5cuX09DQ0KttJknSlqZp/dr2p2m67z85/yvAwcCn0nUs5BzJLiIiIiICSJGA6htIkuQzwHeBvdI0bV3X9iLZRUREREQ49B2yA64C+gEPJ0kC8Gyapl//oI1FsouIiIiI6HNI03Rsb7YXyS4iIiIigr5mxuxtxNSDiIiIiIhNHlHZRURERESwqSu7SHYREREREWzqZBfNmBERERERmzyisouIiIiIICq7iIiIiIiIjRxR2UVEREREEJVdRERERETERo6o7CIiIiIiHDZdZRfJLiIiIiICmTE7P+xOrDdEM2ZERERExCaPqOwiIiIiIogBKhERERERERs5orKLiIiIiGBTV3aR7CIiIiIiHDZdsotmzIiIiIiITR5R2UVEREREsKmbMaOyi4iIiIjY5BGVXUREREQEm7qyi2QXEREREcGmTnbRjBkRERERsckjKruIiIiICKKyi4iIiIiI2MgRlV1EREREhMOmq+wi2UVEREREEM2YERERERERGzmisouIiIiIICq7iIiIiIiIjRxR2UVEREREEJVdRERERETERo6o7CIiIiIi2NSVXSS7iIiIiAiHTZfsohkzIiIiImKTR1R2ERERERFs6mbMqOwiIiIiIjZ5RGUXEREREcGmruwi2UVEREREILLr/LA7sd4QzZgREREREZs8orKLiIiIiGBTN2NGZRcRERERsckjKruIiIiICIdNV9lFsouIiIiIIJoxIyIiIiIiNnJEZRcRERERQVR2ERERERERGzmisouIiIiIoK8puyRJLgAOA7qApcBX0jRd9EHbi8ouIiIiIqIv4tI0TT+epul2wH3A/1uXxqKyi4iIiIigrym7NE2bgz+zqIMfGJHsIiIiIiIcep3sBidJ0hD8fW2aptf+qycnSXIRcCywEpiyLh2JZBcRERERsb6wPE3T+rXtTJLkEaCuh11T0zS9O03TqcDUJEm+D5wC/PCDdiSSXUREREQEH4YZM03Tff/FQ28G7mcdyC4GqERERERE9DkkSTIu+PMw4NV1aS8qu4iIiIgI+lqACnBxkiTjUerBfODr69JYJLuIiIiICPoa2aVp+rnebC+aMSMiIiIiNnlEZRcRERERQV9Tdr2NqOwiIiIiIjZ5RGUXEREREeGw6Sq7SHYREREREUQzZkRERERExEaOqOwiIiIiIojKLiIiIiIiYiNHVHYREREREURlFxERERERsZEjKruIiIiICIfOD7sD6w2R7CIiIiIiiGbMiIiIiIiIjRxR2UVEREREEJVdRERERETERo6o7CIiIiIi2NSVXSS7iIiIiAg2dbKLZsyIiIiIiE0eUdlFRERERBCVXURERERExEaOqOw2ELJJkubTNPmw+xERERGxdmy6yi6S3QZCJLqIiIi+jWjGjNjIkE2S9MPuQ0RERERfQlR2myCiioyIiPj3EZVdRERERETERo2o7CIiIiIiiMouIiIiIiJiI0dUdhERERERbOrKLpJdRERERITDpkt20YwZEREREbHJIyq7iIiIiAg2dTNmVHYfUWSTJI3J5xERER8VRGX3EUVMPI+IiCjEpq3sItlFRERERLCpk100Y0ZEREREbPKIyi4iIiIigqjsIiIiIiIiNnJEZRcRERER4dD5YXdgvSGSXUREREQE0YwZ0Sfx7+bIvd/xtq/43T7HfLyIiIiNHVHZbaT4Z3ly2SRJw2PyaZrYtnBfSGS2rfi8sM3itnrvjiIiIj5cRGUXsRGimMyySZLmR6yp2orPC48PX9ZmPk2T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cSI/XsShjz09t5CcJiJEu52urwTLsogvXJYV9BLk+hUM2VlCS0Uk44lN/wdKSC6B7tOGj/bsRghuhzvdq926EeB02b5nC2AHl4l4VCOp1eLYhhERERGPdnQlSe3kFh/zarhloiF+JhOxix8RERERARzZASqxgkpERERExBGPqOwiIiIiImJtzIiIiIiIiMMdUdlFRERERABR2UVERERERBzWiMouIiIiIiKWC4uIiIiIeHQgmjEjIiIiIiIOY0RlFxERERFxxJsxo7KLiIiIiDjiEZVdRERERARwZPvsItlFRERERMQKKhEREREREYc7orKLiIiIiABigEpERERERMRhjajsIiIiIiKOeJ9dJLuIiIiIiCOe7KIZMyIiIiLiiEdUdhERERERQAxQiYiIiIiIOKwRlV1ERERERPTZRUREREREHO6Iyi4iIiIiAjiyfXaR7CIiIiIiohkzIiIiIiLicEdUdhERERERQFR2ERERERERhzWisouIiIiIoEYMUImIiIiIeBQgmjEjIiIiIiIOY0RlFxERERERUw8iIiIiIiIOd0RlFxEREREBHNkBKlHZRURERETUzZit/BwIkiR5UZIkdyVJMp4kyepg3duTJLk/SZJ7kiR5+t4cLyq7iIiIiIhDEXcCzwc+bxcmSbICeClwHDAHuDpJkmNrtdqE/BrJLiIiIiICOLTMmLVa7Q8ASZKEq84FvlGr1XYDDyZJcj9wEnD9RMeLZsyIiIiIiMMJc4EN5vtGt2xCRGUXEREREcE4XDkIM1p82FKSJDeb75fUarVL9EuSJFcDPRn7XVSr1X7YyguJZBcRERERQa1We8af4Zxn7cdum4D55vs8t2xCRDNmRERERMThhB8BL02SZEqSJI8BlgI37mmnSHYREREREYcckiR5XpIkG4FTgZ8kSXIlQK1Wuwv4FrAG+F/gDXuKxARIarXawbzeiIiIiIiIPzuisouIiIiIOOIRyS4iIiIi4ohHJLuIiIiIiCMekewiIiIiIo54RLKLiIiIiDjiEckuIiIiIuKIRyS7iIiIiIgjHpHsIiIiIiKOePz/1fweHee7lD4AAAAASUVORK5CYII=\n",
+                        "text/plain": [
+                            "<Figure size 576x576 with 2 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "# Compute indicator using all avaliable vectors for a grid of initial conditions\n",
+                "\n",
+                "def gali(vs):\n",
+                "    return torch.linalg.svdvals(vs.nan_to_num()).prod()\n",
+                "\n",
+                "# Set grid\n",
+                "\n",
+                "n1 = 501\n",
+                "n2 = 501\n",
+                "\n",
+                "q1 = torch.linspace(-1.0, +1.0, n1, dtype=dtype, device=device)\n",
+                "q2 = torch.linspace(+0.0, +1.0, n2, dtype=dtype, device=device)\n",
+                "\n",
+                "qs = torch.stack(torch.meshgrid(q1, q2, indexing='ij')).swapaxes(-1, 0).reshape(n1*n2, -1)\n",
+                "ps = torch.full_like(qs, 1.0E-10)\n",
+                "\n",
+                "q1, q2, p1, p2 = torch.hstack([qs, ps]).T\n",
+                "\n",
+                "vs = torch.tensor(n1*n2*[torch.eye(4).tolist()], dtype=dtype, device=device)\n",
+                "qs = torch.stack([q1, p1, q2, p2]).T\n",
+                "\n",
+                "# Set tast\n",
+                "# Perform 512 iterations, compute min of indicator value over the next 64 iterations\n",
+                "\n",
+                "def task(qs, vs, count=512, total=64, level=1.0E-10):\n",
+                "    for _ in range(count):\n",
+                "        qs, vs = tangent(qs, vs)\n",
+                "    out = []\n",
+                "    for _ in range(total):\n",
+                "        qs, vs = tangent(qs, vs)\n",
+                "        out.append(gali(vs))\n",
+                "    return (torch.stack(out).min() + level*torch.sign(qs.norm())).log10()\n",
+                "\n",
+                "# Compute and clean data\n",
+                "\n",
+                "out = torch.vmap(task)(qs, vs)\n",
+                "out = out.nan_to_num(neginf=0.0)\n",
+                "out[(out >= -2.0)*(out != 0.0)] = -2.0\n",
+                "out[out == 0.0] = torch.nan\n",
+                "out = out.reshape(n1, n2)\n",
+                "\n",
+                "# Plot\n",
+                "\n",
+                "plt.figure(figsize=(8, 8))\n",
+                "plt.imshow(\n",
+                "    out.cpu().numpy(),\n",
+                "    vmin=-10.0,\n",
+                "    vmax=-2.0,\n",
+                "    aspect='equal',\n",
+                "    origin='lower',\n",
+                "    cmap='hot', \n",
+                "    interpolation='nearest')\n",
+                "plt.colorbar()\n",
+                "plt.axis('off')\n",
+                "plt.show()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "b1b42a98-fe47-4ae7-9613-114ed5b49e66",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
+                "# Example-11: Closed orbit (dispersion)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "70f1f56c-1877-4291-8a2f-9d75c8d5d249",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# In this example derivatives of closed orbit with respect to momentum deviation are computed"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "43e44d11-1a03-4f8c-a3a7-82df2e4bb4a1",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.evaluate import compare\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "torch.set_printoptions(precision=8, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "0d70fa1d-1104-4f6c-85e1-a623639ce449",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "be0696f0-5b8b-4028-9f3e-4d473175c1b3",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "eb26687c-9b4f-436b-ba87-b2848af36127",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "# Note, here observation poins are locations between elements, lattice start and lattice end\n",
+                "# An observable (closed orbit) is computed at observation points\n",
+                "\n",
+                "# All maps are expected to have identical signature of differentible parameters\n",
+                "# State and momentum deviation in this example\n",
+                "# But each map can have any number of additional args and kwargs after required parameters\n",
+                "\n",
+                "def map_01_02(x, w): return quad(x, w, 0.19, 0.50)\n",
+                "def map_02_03(x, w): return drif(x, w, 0.45)\n",
+                "def map_03_04(x, w): return sext(x, w, 0.00, 0.10)\n",
+                "def map_04_05(x, w): return drif(x, w, 0.45)\n",
+                "def map_05_06(x, w): return bend(x, w, 22.92, 0.015, 0.00, 3.0)\n",
+                "def map_06_07(x, w): return drif(x, w, 0.45)\n",
+                "def map_07_08(x, w): return sext(x, w, 0.00, 0.10)\n",
+                "def map_08_09(x, w): return drif(x, w, 0.45)\n",
+                "def map_09_10(x, w): return quad(x, w, -0.21, 0.50)\n",
+                "def map_10_11(x, w): return quad(x, w, -0.21, 0.50)\n",
+                "def map_11_12(x, w): return drif(x, w, 0.45)\n",
+                "def map_12_13(x, w): return sext(x, w, 0.00, 0.10)\n",
+                "def map_13_14(x, w): return drif(x, w, 0.45)\n",
+                "def map_14_15(x, w): return bend(x, w, 22.92, 0.015, 0.00, 3.0)\n",
+                "def map_15_16(x, w): return drif(x, w, 0.45)\n",
+                "def map_16_17(x, w): return sext(x, w, 0.00, 0.10)\n",
+                "def map_17_18(x, w): return drif(x, w, 0.45)\n",
+                "def map_18_19(x, w): return quad(x, w, 0.19, 0.50)\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02,\n",
+                "    map_02_03,\n",
+                "    map_03_04,\n",
+                "    map_04_05,\n",
+                "    map_05_06,\n",
+                "    map_06_07,\n",
+                "    map_07_08,\n",
+                "    map_08_09,\n",
+                "    map_09_10,\n",
+                "    map_10_11,\n",
+                "    map_11_12,\n",
+                "    map_12_13,\n",
+                "    map_13_14,\n",
+                "    map_14_15,\n",
+                "    map_15_16,\n",
+                "    map_16_17,\n",
+                "    map_17_18,\n",
+                "    map_18_19    \n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, w):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, w)\n",
+                "    return x"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "e4bda838-f9e7-40aa-8cbf-568852ae112b",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# The first step is to compute dynamical fixed point\n",
+                "\n",
+                "# Set initial guess\n",
+                "# Note, in this example zero is a fixed point\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "# Set knobs\n",
+                "\n",
+                "w = torch.tensor([0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "# Find fixed point\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, w, power=1)\n",
+                "\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "c95878f6-0ab7-45ea-b7f2-971c6f682986",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "(0, 0, 0, 0, 0): [0. 0. 0. 0.]\n",
+                        "(0, 0, 0, 0, 1): [1.81613351 0.         0.         0.        ]\n",
+                        "(0, 0, 0, 0, 2): [0.56855511 0.         0.         0.        ]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute parametric closed orbit\n",
+                "\n",
+                "pfp = parametric_fixed_point((2, ), fp, [w], fodo)\n",
+                "chop(pfp)\n",
+                "\n",
+                "# Print series representation\n",
+                "\n",
+                "for key, value in series((4, 1), (0, 2), pfp).items():\n",
+                "    print(f'{key}: {value.cpu().numpy()}')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "81c0b250-6e0c-455f-8884-6686a06ba96e",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n",
+                        "tensor([1.81613351e-03, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00], dtype=torch.float64)\n",
+                        "tensor([1.81670206e-03, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00], dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([1.81670185e-03, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00], dtype=torch.float64)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Check convergence\n",
+                "\n",
+                "print(evaluate(series((4, 1), (0, 0), pfp), [x, w + 1.0E-3]))\n",
+                "print(evaluate(series((4, 1), (0, 1), pfp), [x, w + 1.0E-3]))\n",
+                "print(evaluate(series((4, 1), (0, 2), pfp), [x, w + 1.0E-3]))\n",
+                "print()\n",
+                "\n",
+                "out = fixed_point(16, fodo, x, w + 1.0E-3, power=1)\n",
+                "chop([out])\n",
+                "\n",
+                "print(out)\n",
+                "print()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "022f1ef1-96de-4139-bf64-b6517788184b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Propagate closed orbit\n",
+                "\n",
+                "out = []\n",
+                "\n",
+                "jet = identity((0, 1), fp, parametric=pfp)\n",
+                "out.append(jet)\n",
+                "\n",
+                "for mapping in transport:\n",
+                "    jet = propagate((4, 1), (0, 2), jet, [w], mapping)\n",
+                "    out.append(jet)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "cff7e5c8-d2d5-4903-901a-40811262f87e",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Check periodicity\n",
+                "\n",
+                "print(compare(pfp, jet))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "cae68275-4659-450a-bc95-c309fda3cfad",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "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\n",
+                        "text/plain": [
+                            "<Figure size 1440x360 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "# Plot 1st order dispersion\n",
+                "\n",
+                "pos = [0.00, 0.50, 0.95, 1.05, 1.50, 4.50, 4.95, 5.05, 5.50, 6.00, 6.50, 6.95, 7.05, 7.50, 10.50, 10.95, 11.05, 11.50, 12.00]\n",
+                "res = torch.stack([series((4, 1), (0, 2), jet)[(0, 0, 0, 0, 1)][0] for jet in out])\n",
+                "\n",
+                "plt.figure(figsize=(20, 5))\n",
+                "plt.plot(pos, res.cpu().numpy(), marker='x', color='blue')\n",
+                "plt.show()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "4ebb02ef-1954-4d15-98d5-9a409ad718d6",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "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axQ2om5TeEySpFL3559pdVCDBnDTTWnrxvjx6diaa2adTpKS9deH++6DUaNgzz3hsstg003h3nvTJEVJkkrbEotDMcbZwGmkos5YoG+McXQIoXsIoX3h3fYAxoUQxgPrAFcXPvYH4EpSgWkY0L3wmCRJpWbOHHjwQWjYEC68EHbZJfUUeugh2GijrNNJ0qI1bgz9+8M776Ti0CmnwJZbwtNPp8mKkiSVlhBz7JUmLy8vFhQUZB1DklQGxQgvvAAXXQSjR8P226dVQrvvnnUySVo6836fde0KY8bADjuk32e77ZZ1MklSWRVCGB5jzFvUbSXVkFqSpEy9914qArVvDzNnwlNPzT8mSWVNCLDffmnV4wMPwNSp6ffZfvul7WeSJJUki0OSpDJt3Dg46CDYaafUT+juu9OqoYMPdiy9pLKvShU49tj0++266+DNN2GbbdKxL77IOp0kqbywOCRJKpO++gpOPhm22AJeeQW6d08Tf045BapWzTqdJJWslVZKPdQmTYKzz4bevVNftQsugB9/zDqdJKmsszgkSSpTfvkFunVLzVofeAD+/e90stStG6yyStbpJKl0rbUW3HhjWkl06KHp8iabwA03wF9/ZZ1OklRWWRySJJUJM2fC7bensfRXXZX6bnzySTq29tpZp5OkFatePejVC0aMSNtqL7gANtssHZszJ+t0kqSyxuKQJCmnzZ0LTzyRRjyfeSZsvTUMGwZ9+qRCkSRVZNtsAwMHwpAhsM460KULNG0KL76YJp5JklQcFockSTnr1VeheXM4/HBYbTUYNCgdy1vkAE5JqrhatoT334cnn4Q//4R9903H/ve/rJNJksoCi0OSpJwzYgS0aQOtW8P338Ojj8IHH8BeezmBTJIWJwTo2BHGjoW77krfd9wRDjkk9SiSJGlxLA5JknLGp5/CEUfAttvC8OFw881pVP2RR0IlX7EkqViqVk3N+idOhMsvh5degiZN0rGvv846nSQpF/lWW5KUue++g7POgkaN4Jln4KKLYPLkNK65evWs00lS2bTqqnDFFWmi48knw/33p0mPl18Ov/6adTpJUi6xOCRJyszvv8PVV6cxzHfcAZ07w4QJcM01UKtW1ukkqXxYZx24804YMwb22Qe6d08N/e+8M02ClCTJ4pAkaYWbPRt69oSGDeHSS+Ff/4JRo9Kn2htskHU6SSqf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\n",
+                        "text/plain": [
+                            "<Figure size 1440x360 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "# Plot 2nd order dispersion\n",
+                "\n",
+                "pos = [0.00, 0.50, 0.95, 1.05, 1.50, 4.50, 4.95, 5.05, 5.50, 6.00, 6.50, 6.95, 7.05, 7.50, 10.50, 10.95, 11.05, 11.50, 12.00]\n",
+                "res = torch.stack([series((4, 1), (0, 2), jet)[(0, 0, 0, 0, 2)][0] for jet in out])\n",
+                "\n",
+                "plt.figure(figsize=(20, 5))\n",
+                "plt.plot(pos, res.cpu().numpy(), marker='x', color='blue')\n",
+                "plt.show()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "a85452e8-6cfb-47ef-a434-366de354b268",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
+                "# Example-12: Closed orbit (quadrupole shift)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "ad32fff3-f3da-4bd0-80e5-6ae33b617a50",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.evaluate import compare\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "torch.set_printoptions(precision=6, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "02473f42-5b53-48d1-a478-9e3e1e4d04e9",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "5af703e0-68ed-4dec-a1d4-496aaea2c8cb",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "1d3cb9e4-34ec-46f6-8215-e21743c55323",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, d): \n",
+                "    dxf, dyf, dxd, dyd = d\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    x = slip(x, -dxf, -dyf)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxd, +dyd)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = slip(x, -dxd, -dyd)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxf, +dyf)\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, d):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, d)\n",
+                "    return x"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "b421fbd5-6d20-4531-b0ed-54fa3270fb49",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "fp = fixed_point(16, fodo, x, d, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "bb5b15aa-cf71-4b90-aee5-41b63c29f504",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[-4.621551e-01, 0.000000e+00, 1.165780e+00, 0.000000e+00],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                            "          [0.000000e+00, 3.344042e+00, 0.000000e+00, -4.891066e+00],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute parametric fixed point\n",
+                "\n",
+                "pfp = parametric_fixed_point((1, ), fp, [d], fodo)\n",
+                "chop(pfp)\n",
+                "pfp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "4ec9581a-17f5-46eb-8d17-9d500befb801",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[-4.621551e-01, 0.000000e+00, 1.165780e+00, 0.000000e+00],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                            "          [0.000000e+00, 3.344042e+00, 0.000000e+00, -4.891066e+00],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Propagate parametric fixed point\n",
+                "\n",
+                "out = propagate((4, 4), (0, 1), pfp, [d], fodo)\n",
+                "chop(out)\n",
+                "out"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "5b83a5e1-dbcc-4468-a52b-94aa952c1ef2",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-8.428998e-04, 0.000000e+00, -7.200015e-03, 0.000000e+00], dtype=torch.float64)\n",
+                        "tensor([-8.428998e-04, 0.000000e+00, -7.200015e-03, 0.000000e+00], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Test single random shift\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = 1.0E-3*torch.randn_like(x)\n",
+                "\n",
+                "fp = fixed_point(64, fodo, x, d, power=1, epsilon=1.0E-9)\n",
+                "chop([fp])\n",
+                "\n",
+                "print(fp)\n",
+                "print(evaluate(pfp, [x, d]))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "2f0ebe1d-d86c-454f-ad59-86802a0f58d9",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-2.280223e-05,  0.000000e+00, -3.266640e-05,  0.000000e+00], dtype=torch.float64)\n",
+                        "tensor([1.267704e-03, 0.000000e+00, 5.887239e-03, 0.000000e+00], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Estimate center & spread (tracking)\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = 1.0E-3*torch.randn(8192, 4, dtype=dtype, device=device)\n",
+                "\n",
+                "fp = torch.func.vmap(lambda d: fixed_point(64, fodo, x, d, power=1))(d)\n",
+                "chop([fp])\n",
+                "\n",
+                "print(fp.T.mean(-1))\n",
+                "print(fp.T.std(-1))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "3838c50a-21c7-4a2c-8220-641697a0a905",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-2.510959e-05,  0.000000e+00, -1.240353e-05,  0.000000e+00], dtype=torch.float64)\n",
+                        "tensor([1.260521e-03, 0.000000e+00, 5.920052e-03, 0.000000e+00], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Estimate center & spread (surrogate)\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = 1.0E-3*torch.randn(8192, 4, dtype=dtype, device=device)\n",
+                "\n",
+                "fp = torch.func.vmap(lambda d: evaluate(pfp, [x, d]))(d)\n",
+                "chop([fp])\n",
+                "\n",
+                "print(fp.T.mean(-1))\n",
+                "print(fp.T.std(-1))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "7d4d5f58-b78d-4632-af6d-0955ec51b2c7",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([1.254045e-03, 0.000000e+00, 5.924960e-03, 0.000000e+00], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Estimate spread (error propagation)\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "s = derivative(1, lambda d: evaluate(pfp, [x, d]), d, intermediate=False)\n",
+                "\n",
+                "print((s @ (1.0E-3*torch.eye(4,  dtype=dtype, device=device))**2 @ s.T).diag().sqrt())"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "8eed591e-97f4-4c13-a53b-fc4fb0736995",
+            "metadata": {},
+            "source": [
+                "# Example-13: Closed orbit (sextupole shift)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "e8c85315-a67e-4f13-ad35-8e2136f6b6d1",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.evaluate import compare\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "torch.set_printoptions(precision=6, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "d6b913f4-e7ee-4410-8a97-cf1ac9f52a15",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "3ae4b140-8589-4973-b6f8-d588ecbc8316",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "f22acc90-000b-4e94-baca-a613df54181e",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, d):\n",
+                "    dxsf1, dysf1, dxsd1, dysd1, dxsf2, dysf2, dxsd2, dysd2 = d\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxsf1, +dysf1)\n",
+                "    x = sext(x, [0.0], 0.50, 0.10)\n",
+                "    x = slip(x, -dxsf1, -dysf1)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxsd1, +dysd1)\n",
+                "    x = sext(x, [0.0], -0.50, 0.10)\n",
+                "    x = slip(x, -dxsd1, -dysd1)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxsd2, +dysd2)\n",
+                "    x = sext(x, [0.0], -0.50, 0.10)\n",
+                "    x = slip(x, -dxsd2, -dysd2)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxsf2, +dysf2)\n",
+                "    x = sext(x, [0.0], 0.50, 0.10)\n",
+                "    x = slip(x, -dxsf2, -dysf2)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, d):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, d)\n",
+                "    return x"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "56b58c71-f4ae-44e4-b818-6ba412efb93a",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = torch.tensor([0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "fp = fixed_point(16, fodo, x, d, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "f6fb2e38-d269-4a4f-bf38-31c9de7a887e",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute & check parametric fixed point\n",
+                "# Note, there is no first order contribution from sextupole shifts\n",
+                "\n",
+                "pfp = parametric_fixed_point((2, ), fp, [d], fodo)\n",
+                "out = propagate((4, 8), (0, 2), pfp, [d], fodo)\n",
+                "print(compare(pfp, out))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "f4411bab-734c-45a2-8bbc-0dfaee9d8407",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-5.256659e-07, -4.918902e-08, -2.067269e-06, -5.124183e-08], dtype=torch.float64)\n",
+                        "tensor([-5.246926e-07, -4.909385e-08, -2.075087e-06, -5.138894e-08], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Test for a random shift\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = 1.0E-3*torch.randn(8, dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(64, fodo, x, d, power=1, epsilon=1.0E-9)\n",
+                "\n",
+                "print(fp)\n",
+                "print(evaluate(pfp, [x, d]))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "3cac879f-551a-4ec5-9bf5-d7922d316f06",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-8.407849e-09, -3.266832e-11,  3.976001e-08, -1.611143e-10], dtype=torch.float64)\n",
+                        "tensor([6.868134e-07, 3.121643e-08, 1.807462e-06, 2.967522e-08], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Estimate center & spread (tracking)\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = 1.0E-3*torch.randn(8192, 8, dtype=dtype, device=device)\n",
+                "\n",
+                "fp = torch.func.vmap(lambda d: fixed_point(64, fodo, x, d, power=1))(d)\n",
+                "chop([fp])\n",
+                "\n",
+                "print(fp.T.mean(-1))\n",
+                "print(fp.T.std(-1))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "757522a2-5e28-4141-9e33-29f34fa63c7d",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.156708e-09, 2.567181e-11, 3.218317e-09, 7.290918e-11], dtype=torch.float64)\n",
+                        "tensor([6.811972e-07, 3.105100e-08, 1.816353e-06, 2.926991e-08], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Estimate center & spread (surrogate)\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "d = 1.0E-3*torch.randn(8192, 8, dtype=dtype, device=device)\n",
+                "\n",
+                "fp = torch.func.vmap(lambda d: evaluate(pfp, [x, d]))(d)\n",
+                "chop([fp])\n",
+                "\n",
+                "print(fp.T.mean(-1))\n",
+                "print(fp.T.std(-1))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "81d75dce-4460-47cb-aa13-7f87d0fe0d05",
+            "metadata": {},
+            "source": [
+                "# Example-14: Closed orbit (responce matrix & correction)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "2583e9ab-5501-4f49-b395-f59e9f4c73e7",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# In this example orbit responce matrix is computed\n",
+                "# Quadrupole shifts are introduced and responce matrix is used to correct the orbit at observation locations\n",
+                "\n",
+                "# Correctors are at sextupole centers\n",
+                "# Observation points are at bend centers"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "b0a8970a-837c-4af3-8417-4615d2071ad6",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.evaluate import compare\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "torch.set_printoptions(precision=6, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "b6a506da-4f29-4794-ba37-0e5392536963",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "da6570f1-8968-455a-9938-b797b1821a3a",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=25):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "b17fe3a9-6c67-43f0-bf2b-42ac0a8eb7ee",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, c, d): \n",
+                "    cxsf1, cxsd1, cxsf2, cxsd2, cysf1, cysd1, cysf2, cysd2 = c\n",
+                "    dxf, dyf, dxd, dyd = d\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    x = slip(x, -dxf, -dyf)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = kick(x, cxsf1, cysf1)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 1.5)\n",
+                "    return x\n",
+                "\n",
+                "def map_02_03(x, c, d):\n",
+                "    cxsf1, cxsd1, cxsf2, cxsd2, cysf1, cysd1, cysf2, cysd2 = c\n",
+                "    dxf, dyf, dxd, dyd = d\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 1.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = kick(x, cxsd1, cysd1)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxd, +dyd)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = slip(x, -dxd, -dyd)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = kick(x, cxsd2, cysd2)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 1.5)\n",
+                "    return x\n",
+                "\n",
+                "def map_03_04(x, c, d):\n",
+                "    cxsf1, cxsd1, cxsf2, cxsd2, cysf1, cysd1, cysf2, cysd2 = c\n",
+                "    dxf, dyf, dxd, dyd = d\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.00, 1.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = kick(x, cxsf2, cysf2)\n",
+                "    x = sext(x, [0.0], 0.00, 0.05)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = slip(x, +dxf, +dyf)\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02,\n",
+                "    map_02_03,\n",
+                "    map_03_04\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, c, d):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, c, d)\n",
+                "    return x\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "c = torch.tensor(8*[0.0], dtype=dtype, device=device)\n",
+                "d = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "print(fodo(x, c, d))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "0e69337a-c507-4471-962e-5f69dfb2b8c3",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "c = torch.tensor(8*[0.0], dtype=dtype, device=device)\n",
+                "d = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, c, d, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "02f19aad-3b9c-4497-a4d3-935bbb6b89da",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[7.583253e+00, 5.939607e+00, 7.583253e+00, 5.939607e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                            "          [-4.334732e-01, -9.086786e-02, 4.334732e-01, 9.086786e-02, 0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 1.349234e+01, 2.165892e+01, 1.349234e+01, 2.165892e+01],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, -4.019148e-01, -7.725758e-02, 4.019148e-01, 7.725758e-02]],\n",
+                            "         dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute parametric fixed point\n",
+                "\n",
+                "pfp = parametric_fixed_point((1, ), fp, [c], fodo, d)\n",
+                "chop(pfp)\n",
+                "pfp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "63760982-d712-4ce6-ad69-055c1ce8678b",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[7.583253e+00, 5.939607e+00, 7.583253e+00, 5.939607e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                            "          [-4.334732e-01, -9.086786e-02, 4.334732e-01, 9.086786e-02, 0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 1.349234e+01, 2.165892e+01, 1.349234e+01, 2.165892e+01],\n",
+                            "          [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, -4.019148e-01, -7.725758e-02, 4.019148e-01, 7.725758e-02]],\n",
+                            "         dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Propagate parametric fixed point\n",
+                "\n",
+                "out = propagate((4, 8), (0, 1), pfp, [c], fodo, d)\n",
+                "chop(out)\n",
+                "out"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "f4dd52aa-5eda-4910-962e-d84e18589062",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Orbit derivatives at observation locations\n",
+                "\n",
+                "bag = []\n",
+                "\n",
+                "pfp = propagate((4, 8), (0, 1), pfp, [c], map_01_02, d)\n",
+                "chop(pfp)\n",
+                "bag.append(pfp)\n",
+                "\n",
+                "pfp = propagate((4, 8), (0, 1), pfp, [c], map_02_03, d)\n",
+                "chop(pfp)\n",
+                "bag.append(pfp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "61afd3e6-b21c-4fcb-aceb-d5ea5552fe66",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([[6.221115e+00, 4.042085e+00, 6.753998e+00, 4.569069e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                        "        [6.753998e+00, 4.569069e+00, 6.221115e+00, 4.042085e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00],\n",
+                        "        [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 1.808222e+01, 2.754871e+01, 1.855563e+01, 2.802741e+01],\n",
+                        "        [0.000000e+00, 0.000000e+00, 0.000000e+00, 0.000000e+00, 1.855563e+01, 2.802741e+01, 1.808222e+01, 2.754871e+01]],\n",
+                        "       dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute responce matrix\n",
+                "\n",
+                "def orbit(c, pfp):\n",
+                "    qx, _, qy, _ = evaluate(pfp, [x, c]) \n",
+                "    return torch.stack([qx, qy])\n",
+                "\n",
+                "pfp1, pfp2 = bag\n",
+                "\n",
+                "rx1, ry1 = derivative(1, orbit, c, pfp1, intermediate=False)\n",
+                "rx2, ry2 = derivative(1, orbit, c, pfp2, intermediate=False)\n",
+                "\n",
+                "rm = torch.stack([rx1, rx2, ry1, ry2])\n",
+                "print(rm)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "99e550ce-9345-4582-9ee2-f6d39bd4e237",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-2.161122e-03, -2.161122e-03, -3.001730e-03, -3.001730e-03], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Generate perturbed orbit\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "c = torch.tensor(8*[0.0], dtype=dtype, device=device)\n",
+                "d = torch.tensor([0.001, 0.001, -0.001, 0.001], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, c, d, power=1)\n",
+                "\n",
+                "qx1, _, qy1, _ = map_01_02(fp, c, d)\n",
+                "qx2, _, qy2, _ = map_02_03(map_01_02(fp, c, d), c, d)\n",
+                "\n",
+                "o = torch.stack([qx1, qx2, qy1, qy2])\n",
+                "chop([o])\n",
+                "print(o)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "1394e6ef-4c84-435a-bbce-82b035466e8c",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Correct orbit\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "c = - (torch.linalg.pinv(rm) @ o)\n",
+                "d = torch.tensor([0.001, 0.001, -0.001, 0.001], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, c, d, power=1)\n",
+                "\n",
+                "qx1, _, qy1, _ = map_01_02(fp, c, d)\n",
+                "qx2, _, qy2, _ = map_02_03(map_01_02(fp, c, d), c, d)\n",
+                "\n",
+                "o = torch.stack([qx1, qx2, qy1, qy2])\n",
+                "chop([o])\n",
+                "print(o)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "0e23c026-350b-4d62-82e1-5ddbb49f4573",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
+                "# Example-15: Tune (chromaticity)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "0d6f923d-601e-4736-b214-8e2df57d5918",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "False\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "from twiss.twiss import twiss\n",
+                "\n",
+                "torch.set_printoptions(precision=6, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "e8ef0143-3b64-4487-8a4d-73ef78b0c491",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "1942acce-37c9-4b5c-80e6-9fbd0573816e",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "a69d84a9-7376-4ed6-b669-cd34e56abe50",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, w, k):\n",
+                "    ksf, ksd, ksb = k\n",
+                "    x = quad(x, w, 0.19, 0.50)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = sext(x, w, ksf, 0.10)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = bend(x, w, 22.92, 0.015, ksb, 3.0)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = sext(x, w, ksd, 0.10)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = quad(x, w, -0.21, 0.50)\n",
+                "    x = quad(x, w, -0.21, 0.50)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = sext(x, w, ksd, 0.10)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = bend(x, w, 22.92, 0.015, ksb, 3.0)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = sext(x, w, ksf, 0.10)\n",
+                "    x = drif(x, w, 0.45)\n",
+                "    x = quad(x, w, 0.19, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, d, k):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, d, k)\n",
+                "    return x\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "w = torch.tensor(1*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "print(fodo(x, w, k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "1c148092-c7ba-41b3-b2de-4f0027d02a0e",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "w = torch.tensor(1*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, w, k, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "f5ac8f74-78ac-437d-b5d0-35f7ac1b16a9",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "   tensor([[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]], dtype=torch.float64)],\n",
+                            "  [tensor([[1.816134e+00],\n",
+                            "           [0.000000e+00],\n",
+                            "           [0.000000e+00],\n",
+                            "           [0.000000e+00]], dtype=torch.float64),\n",
+                            "   tensor([[[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]],\n",
+                            "   \n",
+                            "           [[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]],\n",
+                            "   \n",
+                            "           [[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]],\n",
+                            "   \n",
+                            "           [[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]]], dtype=torch.float64)]]]"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute parametric fixed point\n",
+                "\n",
+                "pfp = parametric_fixed_point((1, 1), fp, [w, k], fodo)\n",
+                "chop(pfp)\n",
+                "pfp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "e47fbd61-c250-4f37-8c2c-92d4fe55e6bd",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "   tensor([[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]], dtype=torch.float64)],\n",
+                            "  [tensor([[1.816134e+00],\n",
+                            "           [0.000000e+00],\n",
+                            "           [0.000000e+00],\n",
+                            "           [0.000000e+00]], dtype=torch.float64),\n",
+                            "   tensor([[[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]],\n",
+                            "   \n",
+                            "           [[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]],\n",
+                            "   \n",
+                            "           [[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]],\n",
+                            "   \n",
+                            "           [[0.],\n",
+                            "            [0.],\n",
+                            "            [0.]]], dtype=torch.float64)]]]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Propagate parametric fixed point\n",
+                "\n",
+                "out = propagate((4, 1, 3), (0, 1, 1), pfp, [w, k], fodo)\n",
+                "chop(out)\n",
+                "out"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "d4d080e8-ec1e-41fa-ad29-6c8bddfba185",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Propagate parametric identity (surrogate model for linear dynamics)\n",
+                "\n",
+                "jet = identity((1, 1, 1), fp, parametric=pfp)\n",
+                "jet = propagate((4, 1, 3), (1, 1, 1), jet, [w, k], fodo)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "d64e48f0-a136-478f-99cb-2a0dc8face2c",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute tune\n",
+                "\n",
+                "def tune(w, k):\n",
+                "    m = derivative(1, lambda x: evaluate(jet, [x, w, k]), fp, intermediate=False)\n",
+                "    t, *_ = twiss(m)\n",
+                "    return t\n",
+                "\n",
+                "print(tune(w, k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "3cc1098c-ef11-4ecb-9f21-7f5f71634db2",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[[tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64), tensor([[0., 0., 0.],\n",
+                        "        [0., 0., 0.]], dtype=torch.float64)], [tensor([[-2.343079e-01],\n",
+                        "        [-2.416176e-01]], dtype=torch.float64), tensor([[[3.618782e-01],\n",
+                        "         [8.705079e-02],\n",
+                        "         [5.873074e+00]],\n",
+                        "\n",
+                        "        [[-2.986097e-01],\n",
+                        "         [-4.727344e-01],\n",
+                        "         [-1.106560e+01]]], dtype=torch.float64)]]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute parametric tune\n",
+                "\n",
+                "t = derivative((1, 1), tune, w, k)\n",
+                "\n",
+                "print(t)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "02dd6a3f-856e-44a1-a736-a51279aa6721",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n",
+                        "tensor([2.525452e-01, 1.196688e-01], dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([2.525452e-01, 1.196687e-01], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Check convergence\n",
+                "\n",
+                "print(evaluate(t, [w, k]))\n",
+                "print(evaluate(t, [w + 1.0E-3, k]))\n",
+                "print()\n",
+                "\n",
+                "print(tune(w + 1.0E-3, k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "44d0a4ad-d7d7-46fe-9d34-00343d8bcabf",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n",
+                        "tensor([2.525452e-01, 1.196688e-01], dtype=torch.float64)\n",
+                        "tensor([2.526084e-01, 1.195504e-01], dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([2.526084e-01, 1.195502e-01], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Check convergence\n",
+                "\n",
+                "print(evaluate(t, [w, k]))\n",
+                "print(evaluate(t, [w + 1.0E-3, k]))\n",
+                "print(evaluate(t, [w + 1.0E-3, k + 1.0E-2]))\n",
+                "print()\n",
+                "\n",
+                "print(tune(w + 1.0E-3, k + 1.0E-2))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 13,
+            "id": "b1075e4f-a003-4096-a0d8-5f0c8c39b374",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "(0, 0, 0, 0): tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n",
+                        "(1, 0, 0, 0): tensor([-2.343079e-01, -2.416176e-01], dtype=torch.float64)\n",
+                        "(1, 1, 0, 0): tensor([3.618782e-01, -2.986097e-01], dtype=torch.float64)\n",
+                        "(1, 0, 1, 0): tensor([8.705079e-02, -4.727344e-01], dtype=torch.float64)\n",
+                        "(1, 0, 0, 1): tensor([5.873074e+00, -1.106560e+01], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Series representation\n",
+                "\n",
+                "for key, value in clean(series((1, 3), (1, 1), t)).items():\n",
+                "    print(f'{key}: {value}')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 14,
+            "id": "b53e320f-97ec-4a6d-b224-a6a9d71c4516",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-2.343079e-01, -2.416176e-01], dtype=torch.float64)\n",
+                        "tensor([-2.498002e-16,  2.553513e-15], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set chromaticity to zero\n",
+                "\n",
+                "A = derivative((1, 1), lambda w, k: evaluate(t, [w, k]), w, k, intermediate=False)\n",
+                "b = derivative(1, lambda w, k: evaluate(t, [w, k]), w, k, intermediate=False).flatten()\n",
+                "\n",
+                "print(derivative(1, lambda w: evaluate(t, [w, k]), w, intermediate=False).flatten())\n",
+                "print(derivative(1, lambda w: evaluate(t, [w, - (torch.linalg.pinv(A.squeeze()) @ b)]), w, intermediate=False).flatten())"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 15,
+            "id": "9dd20a0e-5a86-4d33-bb2f-852583a72b9a",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-2.343079e-01, -2.416176e-01], dtype=torch.float64)\n",
+                        "tensor([1.000000e+00, 1.000000e+00], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set chromaticity to one\n",
+                "\n",
+                "A = derivative((1, 1), lambda w, k: evaluate(t, [w, k]), w, k, intermediate=False)\n",
+                "b = -1.0 + derivative(1, lambda w, k: evaluate(t, [w, k]), w, k, intermediate=False).flatten()\n",
+                "\n",
+                "print(derivative(1, lambda w: evaluate(t, [w, k]), w, intermediate=False).flatten())\n",
+                "print(derivative(1, lambda w: evaluate(t, [w, - (torch.linalg.pinv(A.squeeze()) @ b)]), w, intermediate=False).flatten())"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "4e5bec9a-8ca0-4ee4-8daf-3fc4ae4ced3e",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
+                "# Example-16: Tune (responce matrix & correction)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "34e2bb90-1151-46c8-af48-3547ce2e1ec8",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "from twiss.twiss import twiss\n",
+                "\n",
+                "torch.set_printoptions(precision=6, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "5fd86cee-b7a5-4313-ac9e-79fd196ca36e",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "65117f39-b23e-4d8f-ad71-b27367bfef3c",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "2f417785-0148-48e4-a207-9944d1018918",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, k):\n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.0, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.0, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, k):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, k)\n",
+                "    return x\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "print(fodo(x, k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "a2ec343b-0827-4df0-91bb-6dab993fadcf",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, k, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "835bfd5f-0466-422c-9632-0a53ecaba004",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute parametric fixed point\n",
+                "\n",
+                "pfp = parametric_fixed_point((1, ), fp, [k], fodo)\n",
+                "chop(pfp)\n",
+                "pfp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "fa3bf81b-3c99-41d7-9e72-656020d24e69",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Propagate parametric fixed point\n",
+                "\n",
+                "out = propagate((4, 3), (0, 1), pfp, [k], fodo)\n",
+                "chop(out)\n",
+                "out"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "12e6f7b1-98ea-46aa-af37-68d064b7706d",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Propagate parametric identity (surrogate model for linear dynamics)\n",
+                "\n",
+                "jet = identity((1, 1), fp, parametric=pfp)\n",
+                "jet = propagate((4, 3), (1, 1), jet, [k], fodo)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "6d1d9d72-ac01-4016-b716-3e877d58e4aa",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute tune\n",
+                "\n",
+                "def tune(k):\n",
+                "    m = derivative(1, lambda x: evaluate(jet, [x, k]), fp, intermediate=False)\n",
+                "    t, *_ = twiss(m)\n",
+                "    return t\n",
+                "\n",
+                "print(tune(k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "4929b534-0a35-4db5-a7fd-3241bbba02b8",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Compute parametric tune\n",
+                "\n",
+                "t = derivative((1, ), tune, k)"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": null,
-            "id": "68ada124-8f01-4432-b221-8a060ddc04b9",
+            "execution_count": 11,
+            "id": "7730bec7-4b61-4158-b54b-b19afdd38580",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n",
+                        "tensor([2.646746e-01, 9.564416e-02], dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([2.646564e-01, 9.339156e-02], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Check convergence\n",
+                "\n",
+                "print(evaluate(t, [k]))\n",
+                "print(evaluate(t, [k + torch.tensor([5.0E-3, 5.0E-3, 1.0E-3], dtype=dtype, device=device)]))\n",
+                "print()\n",
+                "\n",
+                "print(tune(k + torch.tensor([5.0E-3, 5.0E-3, 1.0E-3], dtype=dtype, device=device)))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "c14a8261-a260-46a7-99cd-781ff07d1f6e",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([[1.217003e+00, 3.230152e-01, 4.195000e+00],\n",
+                        "        [-7.757018e-01, -2.437956e+00, -8.197983e+00]], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Responce matrix\n",
+                "\n",
+                "print(derivative(1, lambda k: evaluate(t, [k]), k, intermediate=False))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 13,
+            "id": "ae0da0a6-9871-4d10-bde8-09710dc97160",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n",
+                        "tensor([2.627666e-01, 1.199040e-01], dtype=torch.float64)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Correct tunes (increase horizontal by 0.01)\n",
+                "\n",
+                "A = derivative(1, lambda k: evaluate(t, [k]), k, intermediate=False)\n",
+                "b = -torch.tensor([0.01, 0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "print(tune(k))\n",
+                "print(tune(-(torch.linalg.pinv(A) @ b)))\n",
+                "print()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "e45a0bb3-6dbc-4c4f-9aee-3e65e1e011a7",
             "metadata": {},
+            "source": [
+                "# Example-17: Tune (spread)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "64adfd8a-c67e-4096-b71c-432890488fa9",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "from twiss.twiss import twiss\n",
+                "\n",
+                "torch.set_printoptions(precision=6, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "f59699d6-947f-4fac-9327-f9a33c587476",
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
-            "source": []
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "043ba457-21bc-485c-ae26-398d51b84e88",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "efb457a6-9b0c-49e5-9c7f-23e7b71185d3",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, k):\n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.0, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.0, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.0, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, k):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, k)\n",
+                "    return x\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "print(fodo(x, k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "7a674c73-751e-431e-b177-a4ed852e815b",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, k, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "88be5819-14c8-44b5-a6eb-60f31490f5ef",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64),\n",
+                            "  tensor([[[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]],\n",
+                            "  \n",
+                            "          [[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]],\n",
+                            "  \n",
+                            "          [[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]],\n",
+                            "  \n",
+                            "          [[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute parametric fixed point\n",
+                "\n",
+                "pfp = parametric_fixed_point((2, ), fp, [k], fodo)\n",
+                "chop(pfp)\n",
+                "pfp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "21e78d86-e754-4a96-ab7e-ca82055202fd",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64),\n",
+                            "  tensor([[[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]],\n",
+                            "  \n",
+                            "          [[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]],\n",
+                            "  \n",
+                            "          [[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]],\n",
+                            "  \n",
+                            "          [[0., 0., 0.],\n",
+                            "           [0., 0., 0.],\n",
+                            "           [0., 0., 0.]]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Propagate parametric fixed point\n",
+                "\n",
+                "out = propagate((4, 3), (0, 2), pfp, [k], fodo)\n",
+                "chop(out)\n",
+                "out"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "f8ca945d-51a8-4a33-a353-957373ea9d45",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Propagate parametric identity (surrogate model for linear dynamics)\n",
+                "\n",
+                "jet = identity((1, 2), fp, parametric=pfp)\n",
+                "jet = propagate((4, 3), (1, 2), jet, [k], fodo)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "8c7a76f9-198e-444d-9cec-2772b562fcea",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527795e-01, 1.199104e-01], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute tune\n",
+                "\n",
+                "def tune(k):\n",
+                "    m = derivative(1, lambda x: evaluate(jet, [x, k]), fp, intermediate=False)\n",
+                "    t, *_ = twiss(m)\n",
+                "    return t\n",
+                "\n",
+                "print(tune(k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "75a24168-d78c-4344-8465-99db88121365",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.528008e-01, 1.197898e-01], dtype=torch.float64)\n",
+                        "tensor([1.984397e-03, 4.095296e-03], dtype=torch.float64)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute tune spread (direct)\n",
+                "\n",
+                "sf = 1.0E-3\n",
+                "sd = 1.0E-3\n",
+                "sb = 1.0E-4\n",
+                "\n",
+                "def wrapper(k):\n",
+                "    t, *_ = twiss(derivative(1, fodo, x, k, intermediate=False))\n",
+                "    return t\n",
+                "\n",
+                "err = torch.tensor([sf, sd, sb])*torch.randn(8192).unsqueeze(1).to(dtype).to(device)\n",
+                "out = torch.func.vmap(wrapper)(err).T\n",
+                "\n",
+                "print(out.mean(-1))\n",
+                "print(out.std(-1))\n",
+                "print()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "fd14777c-8b0c-4171-834f-4b6bcd3b1ad7",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Compute parametric tune\n",
+                "\n",
+                "t = derivative((1, ), tune, k)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "825b1694-45c2-4156-b403-f836e3d04b00",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.527896e-01, 1.198895e-01], dtype=torch.float64)\n",
+                        "tensor([1.943349e-03, 4.000173e-03], dtype=torch.float64)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute tune spread (surrogate)\n",
+                "\n",
+                "sf = 1.0E-3\n",
+                "sd = 1.0E-3\n",
+                "sb = 1.0E-4\n",
+                "\n",
+                "err = torch.tensor([sf, sd, sb])*torch.randn(8192).unsqueeze(1).to(dtype).to(device)\n",
+                "out = torch.func.vmap(lambda k: evaluate(t, [k]))(err).T\n",
+                "\n",
+                "print(out.mean(-1))\n",
+                "print(out.std(-1))\n",
+                "print()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "29cd7b36-7df2-4145-b057-d1c708871dfc",
+            "metadata": {},
+            "source": [
+                "# Example-18: Parametric twiss"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "3e4c3903-481b-4de1-9f3b-54ade0534303",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "from twiss.twiss import twiss\n",
+                "from twiss.twiss import propagate as propagate_twiss\n",
+                "from twiss.convert import wolski_to_cs\n",
+                "\n",
+                "torch.set_printoptions(precision=3, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "d2fd7482-8a02-4433-9865-48e50fa167ec",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "d5a8c2a4-e707-48e6-b611-32283e6810b8",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "f0e309fd-0d4a-4a08-a2a3-8cf4ea352c03",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, k): \n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    return x\n",
+                "\n",
+                "def map_02_03(x, k):\n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.1)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    return x\n",
+                "\n",
+                "def map_03_04(x, k):\n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.1)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02,\n",
+                "    map_02_03,\n",
+                "    map_03_04\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, k):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, k)\n",
+                "    return x\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "print(fodo(x, k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "608c0359-293a-43b8-8d38-6f122c118f8c",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, k, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "566da1db-4fe5-48fd-bde2-c266e5082f7c",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute parametric fixed point\n",
+                "\n",
+                "pfp = parametric_fixed_point((1, ), fp, [k], fodo)\n",
+                "chop(pfp)\n",
+                "pfp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "648fb483-852d-405f-956f-347ab3240d55",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Propagate parametric fixed point\n",
+                "\n",
+                "out = propagate((4, 3), (0, 1), pfp, [k], fodo)\n",
+                "chop(out)\n",
+                "out"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "86ba29c9-e517-45d2-8b77-fd729789c1cd",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Propagate parametric identity (surrogate model for linear dynamics)\n",
+                "\n",
+                "jet = identity((1, 1), fp, parametric=pfp)\n",
+                "jet = propagate((4, 3), (1, 1), jet, [k], fodo)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "b7e8a435-158a-4f96-adff-cfcad2f44253",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.528e-01, 1.199e-01, 8.703e+00, 8.703e+00, 1.553e+01, 1.678e+01, 1.678e+01, 9.586e+00], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute twiss\n",
+                "\n",
+                "# Note, exact or jet one-turn transport can be used\n",
+                "# Other maps can be replaced with jets too\n",
+                "\n",
+                "def fn(k, fodo):\n",
+                "    \n",
+                "    bxs = []\n",
+                "    bys = []\n",
+                "    \n",
+                "    m = derivative(1, fodo, fp, intermediate=False)\n",
+                "    \n",
+                "    t, _, w = twiss(m)\n",
+                "    _, bx, _, by = wolski_to_cs(w)\n",
+                "    \n",
+                "    for mapping in transport:\n",
+                "        w = propagate_twiss(w, derivative(1, mapping, x, k, intermediate=False))\n",
+                "        _, bx, _, by = wolski_to_cs(w)\n",
+                "        bxs.append(bx)\n",
+                "        bys.append(by)\n",
+                "    \n",
+                "    return torch.stack([*t, *bxs, *bys])\n",
+                "\n",
+                "print(fn(k, fodo=lambda x: evaluate(jet, [x, k])))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "f9098db2-d0e7-459d-92ae-eda18d9f3b3d",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[tensor([2.528e-01, 1.199e-01, 8.703e+00, 8.703e+00, 1.553e+01, 1.678e+01, 1.678e+01, 9.586e+00], dtype=torch.float64), tensor([[ 1.217e+00,  3.230e-01,  4.195e+00],\n",
+                        "        [-7.757e-01, -2.438e+00, -8.198e+00],\n",
+                        "        [-3.111e+01, -1.531e+01, -1.101e+02],\n",
+                        "        [-3.111e+01, -1.531e+01, -1.101e+02],\n",
+                        "        [-1.749e+00, -3.120e+01, -1.799e+02],\n",
+                        "        [ 1.153e+02,  3.308e+02,  1.106e+03],\n",
+                        "        [ 1.153e+02,  3.308e+02,  1.106e+03],\n",
+                        "        [ 5.215e+01,  2.146e+02,  6.957e+02]], dtype=torch.float64)]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute parametric derivative using exact map (tune & beta)\n",
+                "\n",
+                "d = derivative((1, ), lambda k: fn(k, fodo=lambda x: fodo(x, k)), k)\n",
+                "\n",
+                "print(d)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "62ac9c73-5b26-4651-8e24-9eb3d676f577",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[tensor([2.528e-01, 1.199e-01, 8.703e+00, 8.703e+00, 1.553e+01, 1.678e+01, 1.678e+01, 9.586e+00], dtype=torch.float64), tensor([[ 1.217e+00,  3.230e-01,  4.195e+00],\n",
+                        "        [-7.757e-01, -2.438e+00, -8.198e+00],\n",
+                        "        [-3.111e+01, -1.531e+01, -1.101e+02],\n",
+                        "        [-3.111e+01, -1.531e+01, -1.101e+02],\n",
+                        "        [-1.749e+00, -3.120e+01, -1.799e+02],\n",
+                        "        [ 1.153e+02,  3.308e+02,  1.106e+03],\n",
+                        "        [ 1.153e+02,  3.308e+02,  1.106e+03],\n",
+                        "        [ 5.215e+01,  2.146e+02,  6.957e+02]], dtype=torch.float64)]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute parametric derivative using jet map (tune & beta)\n",
+                "\n",
+                "d = derivative((1, ), lambda k: fn(k, fodo=lambda x: evaluate(jet, [x, k])), k)\n",
+                "\n",
+                "print(d)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "2255334e-8ccf-49e8-8888-b2b685dd0fa1",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "0.253 0.120 8.703 8.703 15.532 16.780 16.780 9.586\n",
+                        "0.255 0.116 8.645 8.645 15.481 17.337 17.337 9.922\n",
+                        "0.255 0.116 8.646 8.646 15.482 17.366 17.366 9.940\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Check covergence\n",
+                "\n",
+                "dk = torch.tensor([1.0E-3, 1.0E-3, 1.0E-4], dtype=dtype, device=device)\n",
+                "\n",
+                "values = fn(k, fodo=lambda x: fodo(x, k))\n",
+                "print(' '.join([f'{value:.3f}' for value in values.cpu().tolist()]))\n",
+                "\n",
+                "values = evaluate(d, [dk])\n",
+                "print(' '.join([f'{value:.3f}' for value in values.cpu().tolist()]))\n",
+                "\n",
+                "values = fn(k + dk, fodo=lambda x: fodo(x, k + dk))\n",
+                "print(' '.join([f'{value:.3f}' for value in values.cpu().tolist()]))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 13,
+            "id": "654152a0-e66b-4ec1-8716-102b72a9aeac",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([[ 1.217e+00,  3.230e-01,  4.195e+00],\n",
+                        "        [-7.757e-01, -2.438e+00, -8.198e+00],\n",
+                        "        [-3.111e+01, -1.531e+01, -1.101e+02],\n",
+                        "        [-3.111e+01, -1.531e+01, -1.101e+02],\n",
+                        "        [-1.749e+00, -3.120e+01, -1.799e+02],\n",
+                        "        [ 1.153e+02,  3.308e+02,  1.106e+03],\n",
+                        "        [ 1.153e+02,  3.308e+02,  1.106e+03],\n",
+                        "        [ 5.215e+01,  2.146e+02,  6.957e+02]], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Responce matrix\n",
+                "\n",
+                "m = derivative((1, ), lambda k: fn(k, fodo=lambda x: evaluate(jet, [x, k])), k, intermediate=False)\n",
+                "\n",
+                "print(m)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 14,
+            "id": "4b423bb2-1173-42e9-a7ee-779e77d7761f",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.064e-03, -1.258e-03, -4.094e-05], dtype=torch.float64)\n",
+                        "tensor(9.036e-01, dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.000e-03, -1.000e-03, -9.990e-05], dtype=torch.float64)\n",
+                        "tensor(4.251e-02, dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor(8.589e-05, dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor(3.559e-10, dtype=torch.float64)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Correction\n",
+                "\n",
+                "# The target values (tunes and beta functions) are associated with model response matrix\n",
+                "# Given measured values, the goal is to alter knobs to get target values\n",
+                "\n",
+                "# Set target values\n",
+                "\n",
+                "vf = fn(k, fodo=lambda x: fodo(x, k))\n",
+                "\n",
+                "# Set initial solution\n",
+                "\n",
+                "sol = torch.zeros_like(dk)\n",
+                "\n",
+                "# Iterate\n",
+                "\n",
+                "for _ in range(4):\n",
+                "\n",
+                "    # Compute current values and set difference\n",
+                "\n",
+                "    vi = fn(k + dk + sol, fodo=lambda x: evaluate(jet, [x, k + dk + sol]))\n",
+                "\n",
+                "    # Set difference\n",
+                "\n",
+                "    dv = vf - vi\n",
+                "\n",
+                "    # Update solution\n",
+                "\n",
+                "    sol += torch.linalg.pinv(m) @ dv\n",
+                "\n",
+                "    # Verbose\n",
+                "\n",
+                "    print(-dk)\n",
+                "    print(sol)\n",
+                "    print(dv.norm())\n",
+                "    print()\n",
+                "    \n",
+                "    # Continue"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 15,
+            "id": "961c67f7-3585-49d5-b32b-3b8741235952",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Note, similar to tune spread example, it is possible to compute twiss spread\n",
+                "# First order computation can be performed using error propagation\n",
+                "# Or higher order jets can be sampled"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "28236397-30e5-434b-91c1-b7fdd80d0020",
+            "metadata": {},
+            "source": [
+                "# Example-19: Parametric phase advance"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "2383d32c-d2f3-4a53-86fd-f5cad0f49333",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import numpy\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.pfp import fixed_point\n",
+                "from ndtorch.pfp import parametric_fixed_point\n",
+                "\n",
+                "from twiss.twiss import twiss\n",
+                "from twiss.twiss import propagate as propagate_twiss\n",
+                "from twiss.twiss import advance\n",
+                "\n",
+                "torch.set_printoptions(precision=3, sci_mode=True, linewidth=128)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "from matplotlib import pyplot as plt"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "5eefd972-305b-4283-aa5f-26aec1b400f3",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "5b93d925-59de-4f3d-aa1b-39f123af6fc4",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=50):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "bb119a41-088f-4c08-8e3e-9f18bd4d3963",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set transport maps between observation points \n",
+                "\n",
+                "def map_01_02(x, k): \n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    return x\n",
+                "\n",
+                "def map_02_03(x, k):\n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.10)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21 + kqd, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.1)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    return x\n",
+                "\n",
+                "def map_03_04(x, k):\n",
+                "    kqf, kqd, kqb = k\n",
+                "    x = bend(x, [0.0], 22.92, 0.015 + kqb, 0.00, 1.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.00, 0.1)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], 0.19 + kqf, 0.50)\n",
+                "    return x\n",
+                "\n",
+                "transport = [\n",
+                "    map_01_02,\n",
+                "    map_02_03,\n",
+                "    map_03_04\n",
+                "]\n",
+                "\n",
+                "# Define one-turn transport\n",
+                "\n",
+                "def fodo(x, k):\n",
+                "    for mapping in transport:\n",
+                "        x = mapping(x, k)\n",
+                "    return x\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "print(fodo(x, k))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "4562e010-2f28-49ac-b3c2-f3276f64bab9",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute fixed point\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(3*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "fp = fixed_point(16, fodo, x, k, power=1)\n",
+                "print(fp)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "d08f85d3-8e4c-43c0-a101-ba77d2f89b5c",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute parametric fixed point\n",
+                "\n",
+                "pfp = parametric_fixed_point((1, ), fp, [k], fodo)\n",
+                "chop(pfp)\n",
+                "pfp"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "91a8fa30-fbab-4869-ba91-6eeb563ae1a2",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "  tensor([[0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.],\n",
+                            "          [0., 0., 0.]], dtype=torch.float64)]]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Propagate parametric fixed point\n",
+                "\n",
+                "out = propagate((4, 3), (0, 1), pfp, [k], fodo)\n",
+                "chop(out)\n",
+                "out"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "6c1b99c3-e3b6-4f3c-a1ca-72e68d2fb9f2",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Propagate parametric identity (surrogate model for linear dynamics)\n",
+                "\n",
+                "jet = identity((1, 1), fp, parametric=pfp)\n",
+                "jet = propagate((4, 3), (1, 1), jet, [k], fodo)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "3c291b54-e05e-481d-b730-efb83291a148",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([2.528e-01, 1.199e-01, 2.521e-01, 1.084e+00, 2.521e-01, 2.468e-01, 2.599e-01, 2.468e-01], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute phase advance\n",
+                "\n",
+                "# Note, exact or jet one-turn transport can be used\n",
+                "# Other maps can be replaced with jets too\n",
+                "\n",
+                "def fn(k, fodo):\n",
+                "    \n",
+                "    mus = []\n",
+                "    \n",
+                "    m = derivative(1, fodo, fp, intermediate=False)\n",
+                "    \n",
+                "    t, n, _ = twiss(m)\n",
+                "    \n",
+                "    for mapping in transport:\n",
+                "        mu, n = advance(n, derivative(1, mapping, x, k, intermediate=False))\n",
+                "        mus.append(mu)\n",
+                "    \n",
+                "    mus = torch.stack(mus).T\n",
+                "\n",
+                "    return torch.stack([*t, *mus.flatten()])\n",
+                "\n",
+                "print(fn(k, fodo=lambda x: evaluate(jet, [x, k])))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "65210434-411d-464a-a126-50ea5dad6160",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[tensor([2.528e-01, 1.199e-01, 2.521e-01, 1.084e+00, 2.521e-01, 2.468e-01, 2.599e-01, 2.468e-01], dtype=torch.float64), tensor([[1.217e+00, 3.230e-01, 4.195e+00],\n",
+                        "        [-7.757e-01, -2.438e+00, -8.198e+00],\n",
+                        "        [4.458e-01, 4.852e-01, 2.926e+00],\n",
+                        "        [6.755e+00, 1.059e+00, 2.051e+01],\n",
+                        "        [4.458e-01, 4.852e-01, 2.926e+00],\n",
+                        "        [-1.523e+00, -5.303e+00, -1.726e+01],\n",
+                        "        [-1.827e+00, -4.712e+00, -1.699e+01],\n",
+                        "        [-1.523e+00, -5.303e+00, -1.726e+01]], dtype=torch.float64)]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute parametric derivative using exact map (tune & advance)\n",
+                "\n",
+                "d = derivative((1, ), lambda k: fn(k, fodo=lambda x: fodo(x, k)), k)\n",
+                "\n",
+                "print(d)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "b2a73415-1cb4-4f43-a6bc-d99693fcadab",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[tensor([2.528e-01, 1.199e-01, 2.521e-01, 1.084e+00, 2.521e-01, 2.468e-01, 2.599e-01, 2.468e-01], dtype=torch.float64), tensor([[1.217e+00, 3.230e-01, 4.195e+00],\n",
+                        "        [-7.757e-01, -2.438e+00, -8.198e+00],\n",
+                        "        [4.458e-01, 4.852e-01, 2.926e+00],\n",
+                        "        [6.755e+00, 1.059e+00, 2.051e+01],\n",
+                        "        [4.458e-01, 4.852e-01, 2.926e+00],\n",
+                        "        [-1.523e+00, -5.303e+00, -1.726e+01],\n",
+                        "        [-1.827e+00, -4.712e+00, -1.699e+01],\n",
+                        "        [-1.523e+00, -5.303e+00, -1.726e+01]], dtype=torch.float64)]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute parametric derivative using jet map (tune & advance)\n",
+                "\n",
+                "d = derivative((1, ), lambda k: fn(k, fodo=lambda x: evaluate(jet, [x, k])), k)\n",
+                "\n",
+                "print(d)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "38100b72-0f3c-4704-937a-58644a215e86",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "0.253 0.120 0.252 1.084 0.252 0.247 0.260 0.247\n",
+                        "0.255 0.116 0.253 1.094 0.253 0.238 0.252 0.238\n",
+                        "0.255 0.116 0.253 1.094 0.253 0.238 0.251 0.238\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Check covergence\n",
+                "\n",
+                "dk = torch.tensor([1.0E-3, 1.0E-3, 1.0E-4], dtype=dtype, device=device)\n",
+                "\n",
+                "values = fn(k, fodo=lambda x: fodo(x, k))\n",
+                "print(' '.join([f'{value:.3f}' for value in values.cpu().tolist()]))\n",
+                "\n",
+                "values = evaluate(d, [dk])\n",
+                "print(' '.join([f'{value:.3f}' for value in values.cpu().tolist()]))\n",
+                "\n",
+                "values = fn(k + dk, fodo=lambda x: fodo(x, k + dk))\n",
+                "print(' '.join([f'{value:.3f}' for value in values.cpu().tolist()]))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 13,
+            "id": "e36040dd-367b-47a9-884a-a0ccab42d509",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([[1.217e+00, 3.230e-01, 4.195e+00],\n",
+                        "        [-7.757e-01, -2.438e+00, -8.198e+00],\n",
+                        "        [4.458e-01, 4.852e-01, 2.926e+00],\n",
+                        "        [6.755e+00, 1.059e+00, 2.051e+01],\n",
+                        "        [4.458e-01, 4.852e-01, 2.926e+00],\n",
+                        "        [-1.523e+00, -5.303e+00, -1.726e+01],\n",
+                        "        [-1.827e+00, -4.712e+00, -1.699e+01],\n",
+                        "        [-1.523e+00, -5.303e+00, -1.726e+01]], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Responce matrix\n",
+                "\n",
+                "m = derivative((1, ), lambda k: fn(k, fodo=lambda x: evaluate(jet, [x, k])), k, intermediate=False)\n",
+                "\n",
+                "print(m)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 14,
+            "id": "9328e331-744a-4b7d-9e1c-0edb99240c7d",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.043e-03, -1.068e-03, -8.224e-05], dtype=torch.float64)\n",
+                        "tensor(1.846e-02, dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor(2.001e-04, dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor(2.786e-08, dtype=torch.float64)\n",
+                        "\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor([-1.000e-03, -1.000e-03, -1.000e-04], dtype=torch.float64)\n",
+                        "tensor(2.344e-15, dtype=torch.float64)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Correction\n",
+                "\n",
+                "# The target values (tunes and advance functions) are associated with model response matrix\n",
+                "# Given measured values, the goal is to alter knobs to get target values\n",
+                "\n",
+                "# Set target values\n",
+                "\n",
+                "vf = fn(k, fodo=lambda x: fodo(x, k))\n",
+                "\n",
+                "# Set initial solution\n",
+                "\n",
+                "sol = torch.zeros_like(dk)\n",
+                "\n",
+                "# Iterate\n",
+                "\n",
+                "for _ in range(4):\n",
+                "\n",
+                "    # Compute current values and set difference\n",
+                "\n",
+                "    vi = fn(k + dk + sol, fodo=lambda x: evaluate(jet, [x, k + dk + sol]))\n",
+                "\n",
+                "    # Set difference\n",
+                "\n",
+                "    dv = vf - vi\n",
+                "\n",
+                "    # Update solution\n",
+                "\n",
+                "    sol += torch.linalg.pinv(m) @ dv\n",
+                "\n",
+                "    # Verbose\n",
+                "\n",
+                "    print(-dk)\n",
+                "    print(sol)\n",
+                "    print(dv.norm())\n",
+                "    print()\n",
+                "    \n",
+                "    # Continue"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 15,
+            "id": "8c172e35-8002-43ab-9d28-4c6b9610c820",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Note, similar to tune spread example, it is possible to compute advance spread\n",
+                "# First order computation can be performed using error propagation\n",
+                "# Or higher order jets can be sampled"
+            ]
         }
     ],
     "metadata": {
         "colab": {
             "collapsed_sections": [
                 "myt0_gMIOq7b",
                 "5d97819c"
```

### Comparing `ndtorch-0.1.2/pyproject.toml` & `ndtorch-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ndtorch"
-version = "0.1.2"
+version = "0.1.3"
 authors = [{name = "Ivan Morozov", email = "i.a.morozov@inp.nsk.su"}]
 description = "Higher order partial derivatives computation with respect to one or several tensor-like variables, application to nonlinear dynamics"
 readme = "README.MD"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 keywords = ["torch", "derivative"]
 license = {text = "MIT"}
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = ["torch>=2.0.1", "multimethod>=1.9.1"]
 
 [project.optional-dependencies]
 examples = ["jupyter-lab", "numpy", "matplotlib", "twiss"]
```

