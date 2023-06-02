# Comparing `tmp/laproxy-1.0.1.tar.gz` & `tmp/laproxy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laproxy-1.0.1.tar", max compression
+gzip compressed data, was "laproxy-1.0.2.tar", max compression
```

## Comparing `laproxy-1.0.1.tar` & `laproxy-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      406 2023-06-02 08:55:27.653001 laproxy-1.0.1/laproxy/__init__.py
--rw-r--r--   0        0        0     5086 2023-06-02 08:55:27.653001 laproxy-1.0.1/laproxy/_http.py
--rw-r--r--   0        0        0      501 2023-06-02 08:55:27.653001 laproxy-1.0.1/laproxy/_laproxy.py
--rw-r--r--   0        0        0     2898 2023-06-02 08:55:27.653001 laproxy-1.0.1/laproxy/_tcp.py
--rw-r--r--   0        0        0        0 2023-06-02 08:55:27.653001 laproxy-1.0.1/laproxy/py.typed
--rw-r--r--   0        0        0      484 2023-06-02 08:55:27.653001 laproxy-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 laproxy-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      406 2023-06-02 09:55:34.707128 laproxy-1.0.2/laproxy/__init__.py
+-rw-r--r--   0        0        0     5086 2023-06-02 09:55:34.707128 laproxy-1.0.2/laproxy/_http.py
+-rw-r--r--   0        0        0      501 2023-06-02 09:55:34.707128 laproxy-1.0.2/laproxy/_laproxy.py
+-rw-r--r--   0        0        0     2898 2023-06-02 09:55:34.707128 laproxy-1.0.2/laproxy/_tcp.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:55:34.707128 laproxy-1.0.2/laproxy/py.typed
+-rw-r--r--   0        0        0      485 2023-06-02 09:55:34.707128 laproxy-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 laproxy-1.0.2/PKG-INFO
```

### Comparing `laproxy-1.0.1/laproxy/_http.py` & `laproxy-1.0.2/laproxy/_http.py`

 * *Files identical despite different names*

### Comparing `laproxy-1.0.1/laproxy/_tcp.py` & `laproxy-1.0.2/laproxy/_tcp.py`

 * *Files identical despite different names*

