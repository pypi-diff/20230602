# Comparing `tmp/wombo-0.1.0.tar.gz` & `tmp/wombo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wombo-0.1.0.tar", max compression
+gzip compressed data, was "wombo-0.1.1.tar", max compression
```

## Comparing `wombo-0.1.0.tar` & `wombo-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-06-02 14:02:35.382424 wombo-0.1.0/LICENSE
--rw-r--r--   0        0        0        7 2023-06-02 14:02:35.382424 wombo-0.1.0/README.md
--rw-r--r--   0        0        0      319 2023-06-02 14:22:31.106424 wombo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-06-02 14:20:19.386424 wombo-0.1.0/wombo/__init__.py
--rw-r--r--   0        0        0     4118 2023-06-02 14:20:48.810424 wombo-0.1.0/wombo/async_dream.py
--rw-r--r--   0        0        0     2851 2023-06-02 14:21:31.050424 wombo-0.1.0/wombo/dream.py
--rw-r--r--   0        0        0     3274 2023-06-02 14:21:55.846424 wombo-0.1.0/wombo/urls.py
--rw-r--r--   0        0        0      488 1970-01-01 00:00:00.000000 wombo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-02 14:02:35.382424 wombo-0.1.1/LICENSE
+-rw-r--r--   0        0        0       26 2023-06-02 14:29:16.110424 wombo-0.1.1/README.md
+-rw-r--r--   0        0        0      319 2023-06-02 14:29:00.950424 wombo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-06-02 14:20:19.386424 wombo-0.1.1/wombo/__init__.py
+-rw-r--r--   0        0        0     4118 2023-06-02 14:20:48.810424 wombo-0.1.1/wombo/async_dream.py
+-rw-r--r--   0        0        0     2851 2023-06-02 14:21:31.050424 wombo-0.1.1/wombo/dream.py
+-rw-r--r--   0        0        0     3274 2023-06-02 14:21:55.846424 wombo-0.1.1/wombo/urls.py
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 wombo-0.1.1/PKG-INFO
```

### Comparing `wombo-0.1.0/LICENSE` & `wombo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wombo-0.1.0/wombo/async_dream.py` & `wombo-0.1.1/wombo/async_dream.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.0/wombo/dream.py` & `wombo-0.1.1/wombo/dream.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.0/wombo/urls.py` & `wombo-0.1.1/wombo/urls.py`

 * *Files identical despite different names*

