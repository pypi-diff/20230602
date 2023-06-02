# Comparing `tmp/taskanalytics-data-wrapper-0.1.3.tar.gz` & `tmp/taskanalytics-data-wrapper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskanalytics-data-wrapper-0.1.3.tar", last modified: Sun May 21 20:37:56 2023, max compression
+gzip compressed data, was "taskanalytics-data-wrapper-0.1.5.tar", last modified: Fri Jun  2 19:16:57 2023, max compression
```

## Comparing `taskanalytics-data-wrapper-0.1.3.tar` & `taskanalytics-data-wrapper-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,14 @@
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:37:56.172299 taskanalytics-data-wrapper-0.1.3/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       85 2023-05-21 18:14:07.000000 taskanalytics-data-wrapper-0.1.3/.gitignore
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.3/CODEOWNERS
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.3/LICENSE
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      820 2023-05-21 20:33:58.000000 taskanalytics-data-wrapper-0.1.3/Makefile
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4994 2023-05-21 20:37:56.171248 taskanalytics-data-wrapper-0.1.3/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3362 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.3/README.md
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2321 2023-05-21 18:11:27.000000 taskanalytics-data-wrapper-0.1.3/example.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      969 2023-05-21 20:37:36.000000 taskanalytics-data-wrapper-0.1.3/pyproject.toml
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:37:56.148591 taskanalytics-data-wrapper-0.1.3/requirements/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       43 2023-05-21 18:03:20.000000 taskanalytics-data-wrapper-0.1.3/requirements/dev.in
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2831 2023-05-21 20:34:36.000000 taskanalytics-data-wrapper-0.1.3/requirements/dev.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       13 2023-05-21 18:03:07.000000 taskanalytics-data-wrapper-0.1.3/requirements/main.in
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      412 2023-05-21 20:34:30.000000 taskanalytics-data-wrapper-0.1.3/requirements/main.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       38 2023-05-21 20:37:56.172554 taskanalytics-data-wrapper-0.1.3/setup.cfg
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:37:56.162451 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       59 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/__init__.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5217 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_api.py
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:37:56.169201 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4994 2023-05-21 20:37:56.000000 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      629 2023-05-21 20:37:56.000000 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 20:37:56.000000 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       99 2023-05-21 20:37:56.000000 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/requires.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 20:37:56.000000 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:16:57.812790 taskanalytics-data-wrapper-0.1.5/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.5/LICENSE
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      357 2023-06-02 19:16:57.812936 taskanalytics-data-wrapper-0.1.5/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3362 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.5/README.md
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      478 2023-06-02 19:16:57.814629 taskanalytics-data-wrapper-0.1.5/setup.cfg
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       36 2023-06-02 19:04:15.000000 taskanalytics-data-wrapper-0.1.5/setup.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:16:57.808730 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 18:58:55.000000 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper/__init__.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5217 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper/taskanalytics_api.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:16:57.812186 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper.egg-info/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      357 2023-06-02 19:16:57.000000 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      323 2023-06-02 19:16:57.000000 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-02 19:16:57.000000 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       27 2023-06-02 19:16:57.000000 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper.egg-info/top_level.txt
```

### Comparing `taskanalytics-data-wrapper-0.1.3/LICENSE` & `taskanalytics-data-wrapper-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `taskanalytics-data-wrapper-0.1.3/README.md` & `taskanalytics-data-wrapper-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_api.py` & `taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper/taskanalytics_api.py`

 * *Files identical despite different names*

