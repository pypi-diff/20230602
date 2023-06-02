# Comparing `tmp/json2csv-0.0.7.tar.gz` & `tmp/json2csv-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json2csv-0.0.7.tar", last modified: Wed May 24 14:37:26 2023, max compression
+gzip compressed data, was "json2csv-0.0.8.tar", last modified: Fri Jun  2 08:14:42 2023, max compression
```

## Comparing `json2csv-0.0.7.tar` & `json2csv-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 14:37:26.196527 json2csv-0.0.7/
--rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-05-24 14:37:26.196527 json2csv-0.0.7/PKG-INFO
--rw-r--r--   0 agaba     (1000) agaba     (1000)      790 2023-05-24 13:32:50.000000 json2csv-0.0.7/README.md
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 14:37:26.196527 json2csv-0.0.7/json2csv/
--rw-r--r--   0 agaba     (1000) agaba     (1000)       39 2023-05-24 14:35:02.000000 json2csv-0.0.7/json2csv/__init__.py
--rw-r--r--   0 agaba     (1000) agaba     (1000)      950 2023-05-24 13:32:04.000000 json2csv-0.0.7/json2csv/json2csv.py
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-24 14:37:26.196527 json2csv-0.0.7/json2csv.egg-info/
--rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-05-24 14:37:26.000000 json2csv-0.0.7/json2csv.egg-info/PKG-INFO
--rw-r--r--   0 agaba     (1000) agaba     (1000)      188 2023-05-24 14:37:26.000000 json2csv-0.0.7/json2csv.egg-info/SOURCES.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-05-24 14:37:26.000000 json2csv-0.0.7/json2csv.egg-info/dependency_links.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-05-24 14:37:26.000000 json2csv-0.0.7/json2csv.egg-info/top_level.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-05-24 14:37:26.196527 json2csv-0.0.7/setup.cfg
--rw-r--r--   0 agaba     (1000) agaba     (1000)      242 2023-05-24 14:34:32.000000 json2csv-0.0.7/setup.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 08:14:42.156694 json2csv-0.0.8/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-06-02 08:14:42.156694 json2csv-0.0.8/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      790 2023-05-24 13:32:50.000000 json2csv-0.0.8/README.md
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 08:14:42.156694 json2csv-0.0.8/json2csv/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       30 2023-06-02 08:12:43.000000 json2csv-0.0.8/json2csv/__init__.py
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      950 2023-05-24 13:32:04.000000 json2csv-0.0.8/json2csv/json2csv.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 08:14:42.156694 json2csv-0.0.8/json2csv.egg-info/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-06-02 08:14:42.000000 json2csv-0.0.8/json2csv.egg-info/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      188 2023-06-02 08:14:42.000000 json2csv-0.0.8/json2csv.egg-info/SOURCES.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-06-02 08:14:42.000000 json2csv-0.0.8/json2csv.egg-info/dependency_links.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-06-02 08:14:42.000000 json2csv-0.0.8/json2csv.egg-info/top_level.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-06-02 08:14:42.156694 json2csv-0.0.8/setup.cfg
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      242 2023-06-02 08:13:13.000000 json2csv-0.0.8/setup.py
```

### Comparing `json2csv-0.0.7/README.md` & `json2csv-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `json2csv-0.0.7/json2csv/json2csv.py` & `json2csv-0.0.8/json2csv/json2csv.py`

 * *Files identical despite different names*

