# Comparing `tmp/hotjar-data-wrapper-0.1.2.tar.gz` & `tmp/hotjar-data-wrapper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotjar-data-wrapper-0.1.2.tar", last modified: Sun May 21 20:43:23 2023, max compression
+gzip compressed data, was "hotjar-data-wrapper-0.1.3.tar", last modified: Fri Jun  2 19:31:35 2023, max compression
```

## Comparing `hotjar-data-wrapper-0.1.2.tar` & `hotjar-data-wrapper-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,14 @@
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:43:23.774341 hotjar-data-wrapper-0.1.2/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       96 2023-05-21 18:21:37.000000 hotjar-data-wrapper-0.1.2/.gitignore
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.2/CODEOWNERS
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.2/LICENSE
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      820 2023-05-21 20:40:00.000000 hotjar-data-wrapper-0.1.2/Makefile
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3076 2023-05-21 20:43:23.773692 hotjar-data-wrapper-0.1.2/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1517 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.2/README.md
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      981 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.2/example.py
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:43:23.756844 hotjar-data-wrapper-0.1.2/hotjar_data_wrapper/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       45 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.2/hotjar_data_wrapper/__init__.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     6077 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.2/hotjar_data_wrapper/hotjar_api.py
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:43:23.766406 hotjar-data-wrapper-0.1.2/hotjar_data_wrapper/hotjar_data_wrapper.egg-info/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3076 2023-05-21 20:43:23.000000 hotjar-data-wrapper-0.1.2/hotjar_data_wrapper/hotjar_data_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      538 2023-05-21 20:43:23.000000 hotjar-data-wrapper-0.1.2/hotjar_data_wrapper/hotjar_data_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 20:43:23.000000 hotjar-data-wrapper-0.1.2/hotjar_data_wrapper/hotjar_data_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       99 2023-05-21 20:43:23.000000 hotjar-data-wrapper-0.1.2/hotjar_data_wrapper/hotjar_data_wrapper.egg-info/requires.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 20:43:23.000000 hotjar-data-wrapper-0.1.2/hotjar_data_wrapper/hotjar_data_wrapper.egg-info/top_level.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      894 2023-05-21 20:43:07.000000 hotjar-data-wrapper-0.1.2/pyproject.toml
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:43:23.772682 hotjar-data-wrapper-0.1.2/requirements/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       29 2023-05-21 18:18:40.000000 hotjar-data-wrapper-0.1.2/requirements/dev.in
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2777 2023-05-21 20:40:30.000000 hotjar-data-wrapper-0.1.2/requirements/dev.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       13 2023-05-21 18:18:31.000000 hotjar-data-wrapper-0.1.2/requirements/main.in
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      412 2023-05-21 20:40:25.000000 hotjar-data-wrapper-0.1.2/requirements/main.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       38 2023-05-21 20:43:23.774487 hotjar-data-wrapper-0.1.2/setup.cfg
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:31:35.594656 hotjar-data-wrapper-0.1.3/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.3/LICENSE
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      302 2023-06-02 19:31:35.594845 hotjar-data-wrapper-0.1.3/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1517 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.3/README.md
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:31:35.588717 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:27:46.000000 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper/__init__.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     6077 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper/hotjar_api.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:31:35.593960 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper.egg-info/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      302 2023-06-02 19:31:35.000000 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      274 2023-06-02 19:31:35.000000 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-02 19:31:35.000000 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       20 2023-06-02 19:31:35.000000 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      423 2023-06-02 19:31:35.597125 hotjar-data-wrapper-0.1.3/setup.cfg
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       36 2023-06-02 19:25:41.000000 hotjar-data-wrapper-0.1.3/setup.py
```

### Comparing `hotjar-data-wrapper-0.1.2/LICENSE` & `hotjar-data-wrapper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hotjar-data-wrapper-0.1.2/README.md` & `hotjar-data-wrapper-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hotjar-data-wrapper-0.1.2/hotjar_data_wrapper/hotjar_api.py` & `hotjar-data-wrapper-0.1.3/hotjar_data_wrapper/hotjar_api.py`

 * *Files identical despite different names*

