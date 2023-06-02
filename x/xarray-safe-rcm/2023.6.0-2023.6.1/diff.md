# Comparing `tmp/xarray-safe-rcm-2023.6.0.tar.gz` & `tmp/xarray-safe-rcm-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray-safe-rcm-2023.6.0.tar", last modified: Fri Jun  2 09:28:18 2023, max compression
+gzip compressed data, was "xarray-safe-rcm-2023.6.1.tar", last modified: Fri Jun  2 11:48:29 2023, max compression
```

## Comparing `xarray-safe-rcm-2023.6.0.tar` & `xarray-safe-rcm-2023.6.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:18.004341 xarray-safe-rcm-2023.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:17.996341 xarray-safe-rcm-2023.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:17.996341 xarray-safe-rcm-2023.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-02 09:28:18.004341 xarray-safe-rcm-2023.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:17.992341 xarray-safe-rcm-2023.6.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:17.996341 xarray-safe-rcm-2023.6.0/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:17.996341 xarray-safe-rcm-2023.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:18.000341 xarray-safe-rcm-2023.6.0/safe_rcm/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/calibrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:18.000341 xarray-safe-rcm-2023.6.0/safe_rcm/product/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/product/dicttoolz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/product/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/product/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/product/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/product/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:18.000341 xarray-safe-rcm-2023.6.0/safe_rcm/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/tests/test_product_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:28:18.004341 xarray-safe-rcm-2023.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:18.004341 xarray-safe-rcm-2023.6.0/xarray_safe_rcm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-02 09:28:17.000000 xarray-safe-rcm-2023.6.0/xarray_safe_rcm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-02 09:28:17.000000 xarray-safe-rcm-2023.6.0/xarray_safe_rcm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:28:17.000000 xarray-safe-rcm-2023.6.0/xarray_safe_rcm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 09:28:17.000000 xarray-safe-rcm-2023.6.0/xarray_safe_rcm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 09:28:17.000000 xarray-safe-rcm-2023.6.0/xarray_safe_rcm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:48:29.787559 xarray-safe-rcm-2023.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:48:29.783559 xarray-safe-rcm-2023.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:48:29.783559 xarray-safe-rcm-2023.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-02 11:48:29.787559 xarray-safe-rcm-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:48:29.779559 xarray-safe-rcm-2023.6.1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:48:29.783559 xarray-safe-rcm-2023.6.1/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:48:29.783559 xarray-safe-rcm-2023.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:48:29.787559 xarray-safe-rcm-2023.6.1/safe_rcm/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/safe_rcm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/safe_rcm/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/safe_rcm/calibrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/safe_rcm/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:48:29.787559 xarray-safe-rcm-2023.6.1/safe_rcm/product/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/safe_rcm/product/dicttoolz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/safe_rcm/product/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/safe_rcm/product/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/safe_rcm/product/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/safe_rcm/product/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:48:29.787559 xarray-safe-rcm-2023.6.1/safe_rcm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/safe_rcm/tests/test_product_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-02 11:48:09.000000 xarray-safe-rcm-2023.6.1/safe_rcm/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:48:29.787559 xarray-safe-rcm-2023.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:48:29.787559 xarray-safe-rcm-2023.6.1/xarray_safe_rcm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-02 11:48:29.000000 xarray-safe-rcm-2023.6.1/xarray_safe_rcm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-02 11:48:29.000000 xarray-safe-rcm-2023.6.1/xarray_safe_rcm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:48:29.000000 xarray-safe-rcm-2023.6.1/xarray_safe_rcm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-02 11:48:29.000000 xarray-safe-rcm-2023.6.1/xarray_safe_rcm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 11:48:29.000000 xarray-safe-rcm-2023.6.1/xarray_safe_rcm.egg-info/top_level.txt
```

### Comparing `xarray-safe-rcm-2023.6.0/.github/workflows/pypi.yaml` & `xarray-safe-rcm-2023.6.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.6.0/.pre-commit-config.yaml` & `xarray-safe-rcm-2023.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.6.0/LICENSE` & `xarray-safe-rcm-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.6.0/docs/conf.py` & `xarray-safe-rcm-2023.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.6.0/pyproject.toml` & `xarray-safe-rcm-2023.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     "toolz",
     "numpy",
     "xarray",
     "xarray-datatree",
     "lxml",
     "xmlschema",
     "rioxarray",
+    "fsspec",
     "exceptiongroup; python_version < '3.11'",
 ]
 dynamic = ["version"]
 
 [build-system]
 requires = ["setuptools>=64.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
```

### Comparing `xarray-safe-rcm-2023.6.0/safe_rcm/api.py` & `xarray-safe-rcm-2023.6.1/safe_rcm/api.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.6.0/safe_rcm/calibrations.py` & `xarray-safe-rcm-2023.6.1/safe_rcm/calibrations.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.6.0/safe_rcm/manifest.py` & `xarray-safe-rcm-2023.6.1/safe_rcm/manifest.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.6.0/safe_rcm/product/dicttoolz.py` & `xarray-safe-rcm-2023.6.1/safe_rcm/product/dicttoolz.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.6.0/safe_rcm/product/predicates.py` & `xarray-safe-rcm-2023.6.1/safe_rcm/product/predicates.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.6.0/safe_rcm/product/reader.py` & `xarray-safe-rcm-2023.6.1/safe_rcm/product/reader.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.6.0/safe_rcm/product/transformers.py` & `xarray-safe-rcm-2023.6.1/safe_rcm/product/transformers.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.6.0/safe_rcm/product/utils.py` & `xarray-safe-rcm-2023.6.1/safe_rcm/product/utils.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.6.0/safe_rcm/tests/test_product_utils.py` & `xarray-safe-rcm-2023.6.1/safe_rcm/tests/test_product_utils.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.6.0/safe_rcm/xml.py` & `xarray-safe-rcm-2023.6.1/safe_rcm/xml.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.6.0/xarray_safe_rcm.egg-info/SOURCES.txt` & `xarray-safe-rcm-2023.6.1/xarray_safe_rcm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

