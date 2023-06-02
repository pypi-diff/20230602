# Comparing `tmp/HaplyHAPI-1.0.0.tar.gz` & `tmp/HaplyHAPI-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HaplyHAPI-1.0.0.tar", last modified: Fri Jun  2 15:49:51 2023, max compression
+gzip compressed data, was "HaplyHAPI-1.0.1.tar", last modified: Fri Jun  2 17:15:10 2023, max compression
```

## Comparing `HaplyHAPI-1.0.0.tar` & `HaplyHAPI-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:49:51.882096 HaplyHAPI-1.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:49:51.882096 HaplyHAPI-1.0.0/HaplyHAPI.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-06-02 15:49:51.000000 HaplyHAPI-1.0.0/HaplyHAPI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-02 15:49:51.000000 HaplyHAPI-1.0.0/HaplyHAPI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 15:49:51.000000 HaplyHAPI-1.0.0/HaplyHAPI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-02 15:49:51.000000 HaplyHAPI-1.0.0/HaplyHAPI.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-02 15:49:51.000000 HaplyHAPI-1.0.0/HaplyHAPI.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      316 2023-06-02 15:49:51.882096 HaplyHAPI-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-06-02 15:48:22.000000 HaplyHAPI-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 15:49:51.882096 HaplyHAPI-1.0.0/hapi/
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-02 15:48:22.000000 HaplyHAPI-1.0.0/hapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23649 2023-06-02 15:48:22.000000 HaplyHAPI-1.0.0/hapi/hapi.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-02 15:48:22.000000 HaplyHAPI-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 15:49:51.882096 HaplyHAPI-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-02 15:48:22.000000 HaplyHAPI-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:15:10.900745 HaplyHAPI-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)     2541 2023-06-02 17:15:10.896745 HaplyHAPI-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2320 2023-06-02 17:14:54.000000 HaplyHAPI-1.0.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-02 17:14:54.000000 HaplyHAPI-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 17:15:10.900745 HaplyHAPI-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-06-02 17:14:54.000000 HaplyHAPI-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:15:10.896745 HaplyHAPI-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:15:10.896745 HaplyHAPI-1.0.1/src/HaplyHAPI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2541 2023-06-02 17:15:10.000000 HaplyHAPI-1.0.1/src/HaplyHAPI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2023-06-02 17:15:10.000000 HaplyHAPI-1.0.1/src/HaplyHAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 17:15:10.000000 HaplyHAPI-1.0.1/src/HaplyHAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-02 17:15:10.000000 HaplyHAPI-1.0.1/src/HaplyHAPI.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-02 17:15:10.000000 HaplyHAPI-1.0.1/src/HaplyHAPI.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    23649 2023-06-02 17:14:54.000000 HaplyHAPI-1.0.1/src/HaplyHAPI.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-02 17:14:54.000000 HaplyHAPI-1.0.1/src/__init__.py
```

### Comparing `HaplyHAPI-1.0.0/hapi/hapi.py` & `HaplyHAPI-1.0.1/src/HaplyHAPI.py`

 * *Files identical despite different names*

