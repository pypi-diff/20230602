# Comparing `tmp/mongopasswordmanager-1.0.0.tar.gz` & `tmp/mongopasswordmanager-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongopasswordmanager-1.0.0.tar", last modified: Fri Jun  2 15:58:01 2023, max compression
+gzip compressed data, was "mongopasswordmanager-1.0.1.tar", last modified: Fri Jun  2 16:00:27 2023, max compression
```

## Comparing `mongopasswordmanager-1.0.0.tar` & `mongopasswordmanager-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 15:58:01.704739 mongopasswordmanager-1.0.0/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      230 2023-06-02 15:58:01.700739 mongopasswordmanager-1.0.0/PKG-INFO
--rwxrwxr-x   0 praveen   (1000) praveen   (1000)     7277 2023-06-01 15:11:43.000000 mongopasswordmanager-1.0.0/README.md
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 15:58:01.700739 mongopasswordmanager-1.0.0/mongopasswordmanager.egg-info/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      230 2023-06-02 15:58:01.000000 mongopasswordmanager-1.0.0/mongopasswordmanager.egg-info/PKG-INFO
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      237 2023-06-02 15:58:01.000000 mongopasswordmanager-1.0.0/mongopasswordmanager.egg-info/SOURCES.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 15:58:01.000000 mongopasswordmanager-1.0.0/mongopasswordmanager.egg-info/dependency_links.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       46 2023-06-02 15:58:01.000000 mongopasswordmanager-1.0.0/mongopasswordmanager.egg-info/requires.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 15:58:01.000000 mongopasswordmanager-1.0.0/mongopasswordmanager.egg-info/top_level.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-02 15:58:01.704739 mongopasswordmanager-1.0.0/setup.cfg
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      464 2023-06-02 15:57:42.000000 mongopasswordmanager-1.0.0/setup.py
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:00:27.234400 mongopasswordmanager-1.0.1/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      230 2023-06-02 16:00:27.234400 mongopasswordmanager-1.0.1/PKG-INFO
+-rwxrwxr-x   0 praveen   (1000) praveen   (1000)     7277 2023-06-01 15:11:43.000000 mongopasswordmanager-1.0.1/README.md
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:00:27.234400 mongopasswordmanager-1.0.1/mongopasswordmanager.egg-info/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      230 2023-06-02 16:00:27.000000 mongopasswordmanager-1.0.1/mongopasswordmanager.egg-info/PKG-INFO
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      237 2023-06-02 16:00:27.000000 mongopasswordmanager-1.0.1/mongopasswordmanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 16:00:27.000000 mongopasswordmanager-1.0.1/mongopasswordmanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       46 2023-06-02 16:00:27.000000 mongopasswordmanager-1.0.1/mongopasswordmanager.egg-info/requires.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 16:00:27.000000 mongopasswordmanager-1.0.1/mongopasswordmanager.egg-info/top_level.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-02 16:00:27.234400 mongopasswordmanager-1.0.1/setup.cfg
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      533 2023-06-02 16:00:20.000000 mongopasswordmanager-1.0.1/setup.py
```

### Comparing `mongopasswordmanager-1.0.0/README.md` & `mongopasswordmanager-1.0.1/README.md`

 * *Files identical despite different names*

