# Comparing `tmp/json2csv-1.0.0.tar.gz` & `tmp/json2csv-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json2csv-1.0.0.tar", last modified: Fri Jun  2 09:16:50 2023, max compression
+gzip compressed data, was "json2csv-1.0.1.tar", last modified: Fri Jun  2 09:21:59 2023, max compression
```

## Comparing `json2csv-1.0.0.tar` & `json2csv-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 09:16:50.803963 json2csv-1.0.0/
--rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-06-02 09:16:50.803963 json2csv-1.0.0/PKG-INFO
--rw-r--r--   0 agaba     (1000) agaba     (1000)      790 2023-05-24 13:32:50.000000 json2csv-1.0.0/README.md
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 09:16:50.803963 json2csv-1.0.0/json2csv/
--rw-r--r--   0 agaba     (1000) agaba     (1000)       30 2023-06-02 08:12:43.000000 json2csv-1.0.0/json2csv/__init__.py
--rw-r--r--   0 agaba     (1000) agaba     (1000)      960 2023-06-02 08:53:03.000000 json2csv-1.0.0/json2csv/json2csv.py
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 09:16:50.803963 json2csv-1.0.0/json2csv.egg-info/
--rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-06-02 09:16:50.000000 json2csv-1.0.0/json2csv.egg-info/PKG-INFO
--rw-r--r--   0 agaba     (1000) agaba     (1000)      188 2023-06-02 09:16:50.000000 json2csv-1.0.0/json2csv.egg-info/SOURCES.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-06-02 09:16:50.000000 json2csv-1.0.0/json2csv.egg-info/dependency_links.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-06-02 09:16:50.000000 json2csv-1.0.0/json2csv.egg-info/top_level.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-06-02 09:16:50.803963 json2csv-1.0.0/setup.cfg
--rw-r--r--   0 agaba     (1000) agaba     (1000)      242 2023-06-02 09:16:27.000000 json2csv-1.0.0/setup.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 09:21:59.496031 json2csv-1.0.1/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-06-02 09:21:59.496031 json2csv-1.0.1/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      790 2023-05-24 13:32:50.000000 json2csv-1.0.1/README.md
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 09:21:59.492031 json2csv-1.0.1/json2csv/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       30 2023-06-02 09:20:09.000000 json2csv-1.0.1/json2csv/__init__.py
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      960 2023-06-02 08:53:03.000000 json2csv-1.0.1/json2csv/json2csv.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 09:21:59.496031 json2csv-1.0.1/json2csv.egg-info/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      203 2023-06-02 09:21:59.000000 json2csv-1.0.1/json2csv.egg-info/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      188 2023-06-02 09:21:59.000000 json2csv-1.0.1/json2csv.egg-info/SOURCES.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-06-02 09:21:59.000000 json2csv-1.0.1/json2csv.egg-info/dependency_links.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-06-02 09:21:59.000000 json2csv-1.0.1/json2csv.egg-info/top_level.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-06-02 09:21:59.496031 json2csv-1.0.1/setup.cfg
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      242 2023-06-02 09:21:30.000000 json2csv-1.0.1/setup.py
```

### Comparing `json2csv-1.0.0/README.md` & `json2csv-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `json2csv-1.0.0/json2csv/json2csv.py` & `json2csv-1.0.1/json2csv/json2csv.py`

 * *Files identical despite different names*

