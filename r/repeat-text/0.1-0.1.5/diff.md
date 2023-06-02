# Comparing `tmp/repeat_text-0.1.tar.gz` & `tmp/repeat_text-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repeat_text-0.1.tar", last modified: Fri Jun  2 20:34:55 2023, max compression
+gzip compressed data, was "repeat_text-0.1.5.tar", last modified: Fri Jun  2 20:44:38 2023, max compression
```

## Comparing `repeat_text-0.1.tar` & `repeat_text-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 20:34:55.906585 repeat_text-0.1/
--rw-r--r--   0 runner    (1000) runner    (1000)       53 2023-06-02 20:34:55.906585 repeat_text-0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 20:34:55.906585 repeat_text-0.1/repeat_text.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)       53 2023-06-02 20:34:55.000000 repeat_text-0.1/repeat_text.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      235 2023-06-02 20:34:55.000000 repeat_text-0.1/repeat_text.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 20:34:55.000000 repeat_text-0.1/repeat_text.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       49 2023-06-02 20:34:55.000000 repeat_text-0.1/repeat_text.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-06-02 20:34:55.000000 repeat_text-0.1/repeat_text.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-06-02 20:34:55.000000 repeat_text-0.1/repeat_text.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      682 2023-06-02 20:33:36.000000 repeat_text-0.1/repeat_text.py
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-02 20:34:55.906585 repeat_text-0.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      274 2023-06-02 20:33:55.000000 repeat_text-0.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 20:44:38.442238 repeat_text-0.1.5/
+-rw-r--r--   0 runner    (1000) runner    (1000)       55 2023-06-02 20:44:38.442238 repeat_text-0.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 20:44:38.442238 repeat_text-0.1.5/repeat_text.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)       55 2023-06-02 20:44:38.000000 repeat_text-0.1.5/repeat_text.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      235 2023-06-02 20:44:38.000000 repeat_text-0.1.5/repeat_text.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 20:44:38.000000 repeat_text-0.1.5/repeat_text.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       49 2023-06-02 20:44:38.000000 repeat_text-0.1.5/repeat_text.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-06-02 20:44:38.000000 repeat_text-0.1.5/repeat_text.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-06-02 20:44:38.000000 repeat_text-0.1.5/repeat_text.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      682 2023-06-02 20:33:36.000000 repeat_text-0.1.5/repeat_text.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-02 20:44:38.442238 repeat_text-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      276 2023-06-02 20:44:17.000000 repeat_text-0.1.5/setup.py
```

### Comparing `repeat_text-0.1/repeat_text.py` & `repeat_text-0.1.5/repeat_text.py`

 * *Files identical despite different names*

