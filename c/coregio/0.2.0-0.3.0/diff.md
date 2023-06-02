# Comparing `tmp/coregio-0.2.0.tar.gz` & `tmp/coregio-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coregio-0.2.0.tar", last modified: Fri Jun  2 12:56:04 2023, max compression
+gzip compressed data, was "coregio-0.3.0.tar", last modified: Fri Jun  2 13:19:25 2023, max compression
```

## Comparing `coregio-0.2.0.tar` & `coregio-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:56:04.118136 coregio-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 12:56:04.118136 coregio-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:56:04.114136 coregio-0.2.0/coregio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 12:55:54.000000 coregio-0.2.0/coregio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-06-02 12:55:54.000000 coregio-0.2.0/coregio/registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-02 12:55:54.000000 coregio-0.2.0/coregio/registry_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-02 12:55:54.000000 coregio-0.2.0/coregio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:56:04.114136 coregio-0.2.0/coregio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 12:56:04.000000 coregio-0.2.0/coregio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-02 12:56:04.000000 coregio-0.2.0/coregio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 12:56:04.000000 coregio-0.2.0/coregio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 12:56:04.000000 coregio-0.2.0/coregio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 12:56:04.000000 coregio-0.2.0/coregio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-02 12:55:54.000000 coregio-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 12:56:04.118136 coregio-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:56:04.118136 coregio-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-06-02 12:55:54.000000 coregio-0.2.0/tests/test_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-02 12:55:54.000000 coregio-0.2.0/tests/test_registry_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-02 12:55:54.000000 coregio-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:25.646465 coregio-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 13:19:25.646465 coregio-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:25.646465 coregio-0.3.0/coregio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:16.000000 coregio-0.3.0/coregio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-06-02 13:19:16.000000 coregio-0.3.0/coregio/registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-02 13:19:16.000000 coregio-0.3.0/coregio/registry_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-02 13:19:16.000000 coregio-0.3.0/coregio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:25.646465 coregio-0.3.0/coregio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 13:19:25.000000 coregio-0.3.0/coregio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-02 13:19:25.000000 coregio-0.3.0/coregio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:19:25.000000 coregio-0.3.0/coregio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 13:19:25.000000 coregio-0.3.0/coregio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 13:19:25.000000 coregio-0.3.0/coregio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-02 13:19:16.000000 coregio-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 13:19:25.646465 coregio-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:19:25.646465 coregio-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-06-02 13:19:16.000000 coregio-0.3.0/tests/test_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-02 13:19:16.000000 coregio-0.3.0/tests/test_registry_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-02 13:19:16.000000 coregio-0.3.0/tests/test_utils.py
```

### Comparing `coregio-0.2.0/coregio/registry_api.py` & `coregio-0.3.0/coregio/registry_api.py`

 * *Files identical despite different names*

### Comparing `coregio-0.2.0/coregio/registry_auth.py` & `coregio-0.3.0/coregio/registry_auth.py`

 * *Files identical despite different names*

### Comparing `coregio-0.2.0/coregio/utils.py` & `coregio-0.3.0/coregio/utils.py`

 * *Files identical despite different names*

### Comparing `coregio-0.2.0/pyproject.toml` & `coregio-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "coregio"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python container registry API library."
 authors = [{ name = "Ales Raszka", email = "araszka@redhat.com" }]
 dependencies = []
 requires-python = ">=3.10"
 readme = "README.md"
 license = { text = "MIT" }
 [project.optional-dependencies]
```

### Comparing `coregio-0.2.0/tests/test_registry_api.py` & `coregio-0.3.0/tests/test_registry_api.py`

 * *Files identical despite different names*

### Comparing `coregio-0.2.0/tests/test_registry_auth.py` & `coregio-0.3.0/tests/test_registry_auth.py`

 * *Files identical despite different names*

