# Comparing `tmp/aspectify-0.0.1.tar.gz` & `tmp/aspectify-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aspectify-0.0.1.tar", last modified: Mon May 29 07:49:18 2023, max compression
+gzip compressed data, was "aspectify-0.0.2.tar", last modified: Fri Jun  2 06:38:25 2023, max compression
```

## Comparing `aspectify-0.0.1.tar` & `aspectify-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-05-29 07:49:18.173232 aspectify-0.0.1/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     7048 2023-05-29 07:08:03.000000 aspectify-0.0.1/LICENSE
--rw-rw-r--   0 ruescog   (1008) ruescog   (1011)      111 2023-04-27 10:12:58.000000 aspectify-0.0.1/MANIFEST.in
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     1261 2023-05-29 07:49:18.173232 aspectify-0.0.1/PKG-INFO
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      296 2023-05-29 07:42:33.000000 aspectify-0.0.1/README.md
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-05-29 07:49:18.173232 aspectify-0.0.1/aspectify/
--rw-r--r--   0 ruescog   (1008) ruescog   (1011)       22 2023-05-29 07:42:30.000000 aspectify-0.0.1/aspectify/__init__.py
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      369 2023-05-29 07:42:30.000000 aspectify-0.0.1/aspectify/_modidx.py
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      142 2023-05-29 07:42:30.000000 aspectify-0.0.1/aspectify/core.py
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-05-29 07:49:18.173232 aspectify-0.0.1/aspectify.egg-info/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     1261 2023-05-29 07:49:18.000000 aspectify-0.0.1/aspectify.egg-info/PKG-INFO
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      344 2023-05-29 07:49:18.000000 aspectify-0.0.1/aspectify.egg-info/SOURCES.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-05-29 07:49:18.000000 aspectify-0.0.1/aspectify.egg-info/dependency_links.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       61 2023-05-29 07:49:18.000000 aspectify-0.0.1/aspectify.egg-info/entry_points.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-05-29 07:48:24.000000 aspectify-0.0.1/aspectify.egg-info/not-zip-safe
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        7 2023-05-29 07:49:18.000000 aspectify-0.0.1/aspectify.egg-info/requires.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       10 2023-05-29 07:49:18.000000 aspectify-0.0.1/aspectify.egg-info/top_level.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      969 2023-05-29 07:42:18.000000 aspectify-0.0.1/settings.ini
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       38 2023-05-29 07:49:18.173232 aspectify-0.0.1/setup.cfg
--rw-rw-r--   0 ruescog   (1008) ruescog   (1011)     2596 2023-04-27 10:12:58.000000 aspectify-0.0.1/setup.py
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 06:38:25.096353 aspectify-0.0.2/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     7048 2023-05-29 07:08:03.000000 aspectify-0.0.2/LICENSE
+-rw-rw-r--   0 ruescog   (1008) ruescog   (1011)      111 2023-04-27 10:12:58.000000 aspectify-0.0.2/MANIFEST.in
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     6787 2023-06-02 06:38:25.096353 aspectify-0.0.2/PKG-INFO
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     4758 2023-06-01 07:25:52.000000 aspectify-0.0.2/README.md
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 06:38:25.092353 aspectify-0.0.2/aspectify/
+-rw-r--r--   0 ruescog   (1008) ruescog   (1011)       22 2023-06-02 06:37:48.000000 aspectify-0.0.2/aspectify/__init__.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     1537 2023-06-02 06:37:48.000000 aspectify-0.0.2/aspectify/_modidx.py
+-rw-r--r--   0 ruescog   (1008) ruescog   (1011)     6490 2023-06-02 06:37:48.000000 aspectify-0.0.2/aspectify/aop.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      142 2023-05-29 07:42:30.000000 aspectify-0.0.2/aspectify/core.py
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 06:38:25.096353 aspectify-0.0.2/aspectify.egg-info/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     6787 2023-06-02 06:38:25.000000 aspectify-0.0.2/aspectify.egg-info/PKG-INFO
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      361 2023-06-02 06:38:25.000000 aspectify-0.0.2/aspectify.egg-info/SOURCES.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-06-02 06:38:25.000000 aspectify-0.0.2/aspectify.egg-info/dependency_links.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       61 2023-06-02 06:38:25.000000 aspectify-0.0.2/aspectify.egg-info/entry_points.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-05-29 07:48:24.000000 aspectify-0.0.2/aspectify.egg-info/not-zip-safe
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        7 2023-06-02 06:38:25.000000 aspectify-0.0.2/aspectify.egg-info/requires.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       10 2023-06-02 06:38:25.000000 aspectify-0.0.2/aspectify.egg-info/top_level.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      802 2023-06-02 06:32:55.000000 aspectify-0.0.2/settings.ini
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       38 2023-06-02 06:38:25.096353 aspectify-0.0.2/setup.cfg
+-rw-rw-r--   0 ruescog   (1008) ruescog   (1011)     2596 2023-04-27 10:12:58.000000 aspectify-0.0.2/setup.py
```

### Comparing `aspectify-0.0.1/LICENSE` & `aspectify-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aspectify-0.0.1/setup.py` & `aspectify-0.0.2/setup.py`

 * *Files identical despite different names*

