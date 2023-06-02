# Comparing `tmp/flexigurator-0.3.0.tar.gz` & `tmp/flexigurator-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexigurator-0.3.0.tar", max compression
+gzip compressed data, was "flexigurator-0.3.1.tar", max compression
```

## Comparing `flexigurator-0.3.0.tar` & `flexigurator-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-06-02 13:05:36.206512 flexigurator-0.3.0/README.md
--rw-r--r--   0        0        0       69 2023-06-02 13:05:36.206512 flexigurator-0.3.0/flexigurator/__init__.py
--rw-r--r--   0        0        0     1421 2023-06-02 13:05:36.206512 flexigurator-0.3.0/flexigurator/config_patch.py
--rw-r--r--   0        0        0        0 2023-06-02 13:05:36.206512 flexigurator-0.3.0/flexigurator/form/__init__.py
--rw-r--r--   0        0        0     4777 2023-06-02 13:05:36.206512 flexigurator-0.3.0/flexigurator/form/form.py
--rw-r--r--   0        0        0     5790 2023-06-02 13:05:36.206512 flexigurator-0.3.0/flexigurator/form/jinja_templates/config_form.html
--rw-r--r--   0        0        0     3550 2023-06-02 13:05:36.206512 flexigurator-0.3.0/flexigurator/form/jinja_templates/index.html
--rw-r--r--   0        0        0     2481 2023-06-02 13:05:36.206512 flexigurator-0.3.0/flexigurator/placeholder.py
--rw-r--r--   0        0        0     1083 2023-06-02 13:05:36.210512 flexigurator-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      626 1970-01-01 00:00:00.000000 flexigurator-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2373 2023-06-02 13:39:37.460070 flexigurator-0.3.1/README.md
+-rw-r--r--   0        0        0      166 2023-06-02 13:39:37.460070 flexigurator-0.3.1/flexigurator/__init__.py
+-rw-r--r--   0        0        0     1421 2023-06-02 13:39:37.460070 flexigurator-0.3.1/flexigurator/config_patch.py
+-rw-r--r--   0        0        0        0 2023-06-02 13:39:37.460070 flexigurator-0.3.1/flexigurator/form/__init__.py
+-rw-r--r--   0        0        0     4777 2023-06-02 13:39:37.460070 flexigurator-0.3.1/flexigurator/form/form.py
+-rw-r--r--   0        0        0     5790 2023-06-02 13:39:37.460070 flexigurator-0.3.1/flexigurator/form/jinja_templates/config_form.html
+-rw-r--r--   0        0        0     3550 2023-06-02 13:39:37.460070 flexigurator-0.3.1/flexigurator/form/jinja_templates/index.html
+-rw-r--r--   0        0        0     2481 2023-06-02 13:39:37.460070 flexigurator-0.3.1/flexigurator/placeholder.py
+-rw-r--r--   0        0        0     1083 2023-06-02 13:39:37.464070 flexigurator-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2999 1970-01-01 00:00:00.000000 flexigurator-0.3.1/PKG-INFO
```

### Comparing `flexigurator-0.3.0/flexigurator/config_patch.py` & `flexigurator-0.3.1/flexigurator/config_patch.py`

 * *Files identical despite different names*

### Comparing `flexigurator-0.3.0/flexigurator/form/form.py` & `flexigurator-0.3.1/flexigurator/form/form.py`

 * *Files identical despite different names*

### Comparing `flexigurator-0.3.0/flexigurator/form/jinja_templates/config_form.html` & `flexigurator-0.3.1/flexigurator/form/jinja_templates/config_form.html`

 * *Files identical despite different names*

### Comparing `flexigurator-0.3.0/flexigurator/form/jinja_templates/index.html` & `flexigurator-0.3.1/flexigurator/form/jinja_templates/index.html`

 * *Files identical despite different names*

### Comparing `flexigurator-0.3.0/flexigurator/placeholder.py` & `flexigurator-0.3.1/flexigurator/placeholder.py`

 * *Files identical despite different names*

### Comparing `flexigurator-0.3.0/pyproject.toml` & `flexigurator-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flexigurator"
-version = "0.3.0"
+version = "0.3.1"
 description = "Python Configuration solution."
 authors = ["Thomas Bos <thymer.bos217@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^1.10.8"
```

