# Comparing `tmp/cvxcovariance-0.0.7.tar.gz` & `tmp/cvxcovariance-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxcovariance-0.0.7.tar", max compression
+gzip compressed data, was "cvxcovariance-0.0.8.tar", max compression
```

## Comparing `cvxcovariance-0.0.7.tar` & `cvxcovariance-0.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11375 2023-06-02 01:05:02.456010 cvxcovariance-0.0.7/LICENSE
--rw-r--r--   0        0        0     6749 2023-06-02 01:05:02.456010 cvxcovariance-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-06-02 01:05:02.484010 cvxcovariance-0.0.7/cvx/covariance/__init__.py
--rw-r--r--   0        0        0     9179 2023-06-02 01:05:02.484010 cvxcovariance-0.0.7/cvx/covariance/combination.py
--rw-r--r--   0        0        0     6706 2023-06-02 01:05:02.484010 cvxcovariance-0.0.7/cvx/covariance/ewma.py
--rw-r--r--   0        0        0     1863 2023-06-02 01:05:02.484010 cvxcovariance-0.0.7/cvx/covariance/regularization.py
--rw-r--r--   0        0        0      645 2023-06-02 01:05:31.691910 cvxcovariance-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     7347 1970-01-01 00:00:00.000000 cvxcovariance-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-06-02 03:58:14.021217 cvxcovariance-0.0.8/LICENSE
+-rw-r--r--   0        0        0     6749 2023-06-02 03:58:14.021217 cvxcovariance-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 03:58:14.045217 cvxcovariance-0.0.8/cvx/covariance/__init__.py
+-rw-r--r--   0        0        0     9179 2023-06-02 03:58:14.045217 cvxcovariance-0.0.8/cvx/covariance/combination.py
+-rw-r--r--   0        0        0     6706 2023-06-02 03:58:14.045217 cvxcovariance-0.0.8/cvx/covariance/ewma.py
+-rw-r--r--   0        0        0     1863 2023-06-02 03:58:14.045217 cvxcovariance-0.0.8/cvx/covariance/regularization.py
+-rw-r--r--   0        0        0      645 2023-06-02 03:58:42.481428 cvxcovariance-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     7347 1970-01-01 00:00:00.000000 cvxcovariance-0.0.8/PKG-INFO
```

### Comparing `cvxcovariance-0.0.7/LICENSE` & `cvxcovariance-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxcovariance-0.0.7/README.md` & `cvxcovariance-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cvxcovariance-0.0.7/cvx/covariance/combination.py` & `cvxcovariance-0.0.8/cvx/covariance/combination.py`

 * *Files identical despite different names*

### Comparing `cvxcovariance-0.0.7/cvx/covariance/ewma.py` & `cvxcovariance-0.0.8/cvx/covariance/ewma.py`

 * *Files identical despite different names*

### Comparing `cvxcovariance-0.0.7/cvx/covariance/regularization.py` & `cvxcovariance-0.0.8/cvx/covariance/regularization.py`

 * *Files identical despite different names*

### Comparing `cvxcovariance-0.0.7/pyproject.toml` & `cvxcovariance-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxcovariance"
-version = "v0.0.7"             # Don't touch, leave at 0.0.0
+version = "v0.0.8"             # Don't touch, leave at 0.0.0
 description = "..."
 authors = ["Kasper Johansson", "Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/cov_pred_finance"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxcovariance-0.0.7/PKG-INFO` & `cvxcovariance-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxcovariance
-Version: 0.0.7
+Version: 0.0.8
 Summary: ...
 Home-page: https://github.com/cvxgrp/cov_pred_finance
 Author: Kasper Johansson
 Requires-Python: >=3.8.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

