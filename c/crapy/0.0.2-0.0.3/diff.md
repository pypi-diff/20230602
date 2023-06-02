# Comparing `tmp/crapy-0.0.2.tar.gz` & `tmp/crapy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crapy-0.0.2.tar", last modified: Fri Aug 23 03:00:58 2019, max compression
+gzip compressed data, was "crapy-0.0.3.tar", max compression
```

## Comparing `crapy-0.0.2.tar` & `crapy-0.0.3.tar`

### file list

```diff
@@ -1,4 +1,8 @@
--rw-r--r--   0        0        0      110 2019-08-23 02:56:39.847268 crapy-0.0.2/crapy.py
--rw-r--r--   0        0        0      287 2019-08-23 02:59:19.105946 crapy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      376 1970-01-01 00:00:00.000000 crapy-0.0.2/setup.py
--rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 crapy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      296 2023-06-02 14:08:41.254279 crapy-0.0.3/README.md
+-rw-r--r--   0        0        0      247 2023-06-02 14:47:10.662011 crapy-0.0.3/crapy/__about__.py
+-rw-r--r--   0        0        0      823 2023-06-02 14:36:26.231391 crapy-0.0.3/crapy/__init__.py
+-rw-r--r--   0        0        0      466 2023-06-02 14:48:06.237931 crapy-0.0.3/crapy/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-02 13:35:42.933197 crapy-0.0.3/crapy/py.typed
+-rw-r--r--   0        0        0     1157 2023-06-02 14:36:26.229966 crapy-0.0.3/crapy/third_party.py
+-rw-r--r--   0        0        0     4189 2023-06-02 14:46:41.460182 crapy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 crapy-0.0.3/PKG-INFO
```

