# Comparing `tmp/mono-dense-keras-0.0.6rc2.tar.gz` & `tmp/mono-dense-keras-0.0.6rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mono-dense-keras-0.0.6rc2.tar", last modified: Fri Jun  2 14:10:10 2023, max compression
+gzip compressed data, was "mono-dense-keras-0.0.6rc3.tar", last modified: Fri Jun  2 14:14:31 2023, max compression
```

## Comparing `mono-dense-keras-0.0.6rc2.tar` & `mono-dense-keras-0.0.6rc3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:10:10.739577 mono-dense-keras-0.0.6rc2/
--rw-r--r--   0 davor     (1000) davor     (1000)    20848 2022-09-02 19:27:53.000000 mono-dense-keras-0.0.6rc2/LICENSE
--rw-rw-r--   0 davor     (1000) davor     (1000)      111 2022-08-18 19:39:58.000000 mono-dense-keras-0.0.6rc2/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)     7659 2023-06-02 14:10:10.739577 mono-dense-keras-0.0.6rc2/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)     6546 2023-06-01 08:50:38.000000 mono-dense-keras-0.0.6rc2/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:10:10.735577 mono-dense-keras-0.0.6rc2/mono_dense_keras/
--rw-rw-r--   0 davor     (1000) davor     (1000)      463 2023-06-02 14:08:39.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:10:10.739577 mono-dense-keras-0.0.6rc2/mono_dense_keras/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-02 13:55:48.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    23910 2023-06-02 14:08:39.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras/_components/mono_dense_layer.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    10897 2023-06-02 14:08:39.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras/_modidx.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    14065 2023-06-02 14:08:39.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras/experiments.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      288 2023-06-02 13:55:48.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras/helpers.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:10:10.739577 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/
--rw-r--r--   0 davor     (1000) davor     (1000)     7659 2023-06-02 14:10:10.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/PKG-INFO
--rw-r--r--   0 davor     (1000) davor     (1000)      539 2023-06-02 14:10:10.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/SOURCES.txt
--rw-r--r--   0 davor     (1000) davor     (1000)        1 2023-06-02 14:10:10.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/dependency_links.txt
--rw-r--r--   0 davor     (1000) davor     (1000)       54 2023-06-02 14:10:10.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/entry_points.txt
--rw-r--r--   0 davor     (1000) davor     (1000)        1 2022-12-06 04:51:35.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/not-zip-safe
--rw-r--r--   0 davor     (1000) davor     (1000)      224 2023-06-02 14:10:10.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/requires.txt
--rw-r--r--   0 davor     (1000) davor     (1000)       17 2023-06-02 14:10:10.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/top_level.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)      969 2023-06-02 14:09:59.000000 mono-dense-keras-0.0.6rc2/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-02 14:10:10.739577 mono-dense-keras-0.0.6rc2/setup.cfg
--rw-rw-r--   0 davor     (1000) davor     (1000)     3093 2023-06-02 14:08:39.000000 mono-dense-keras-0.0.6rc2/setup.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:14:31.598461 mono-dense-keras-0.0.6rc3/
+-rw-r--r--   0 davor     (1000) davor     (1000)    20848 2022-09-02 19:27:53.000000 mono-dense-keras-0.0.6rc3/LICENSE
+-rw-rw-r--   0 davor     (1000) davor     (1000)      111 2022-08-18 19:39:58.000000 mono-dense-keras-0.0.6rc3/MANIFEST.in
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10344 2023-06-02 14:14:31.598461 mono-dense-keras-0.0.6rc3/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)     9231 2023-06-02 14:13:16.000000 mono-dense-keras-0.0.6rc3/README.md
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:14:31.598461 mono-dense-keras-0.0.6rc3/mono_dense_keras/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      463 2023-06-02 14:14:28.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:14:31.598461 mono-dense-keras-0.0.6rc3/mono_dense_keras/_components/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-02 14:14:28.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras/_components/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    23910 2023-06-02 14:14:28.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras/_components/mono_dense_layer.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10897 2023-06-02 14:14:28.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras/_modidx.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    14065 2023-06-02 14:14:28.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras/experiments.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      288 2023-06-02 14:14:28.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras/helpers.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:14:31.598461 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/
+-rw-r--r--   0 davor     (1000) davor     (1000)    10344 2023-06-02 14:14:31.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/PKG-INFO
+-rw-r--r--   0 davor     (1000) davor     (1000)      539 2023-06-02 14:14:31.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/SOURCES.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)        1 2023-06-02 14:14:31.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/dependency_links.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)       54 2023-06-02 14:14:31.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/entry_points.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)        1 2022-12-06 04:51:35.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/not-zip-safe
+-rw-r--r--   0 davor     (1000) davor     (1000)      224 2023-06-02 14:14:31.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/requires.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)       17 2023-06-02 14:14:31.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/top_level.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)      969 2023-06-02 14:14:19.000000 mono-dense-keras-0.0.6rc3/settings.ini
+-rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-02 14:14:31.598461 mono-dense-keras-0.0.6rc3/setup.cfg
+-rw-rw-r--   0 davor     (1000) davor     (1000)     3093 2023-06-02 14:08:39.000000 mono-dense-keras-0.0.6rc3/setup.py
```

### Comparing `mono-dense-keras-0.0.6rc2/LICENSE` & `mono-dense-keras-0.0.6rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc2/mono_dense_keras/_components/mono_dense_layer.py` & `mono-dense-keras-0.0.6rc3/mono_dense_keras/_components/mono_dense_layer.py`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc2/mono_dense_keras/_modidx.py` & `mono-dense-keras-0.0.6rc3/mono_dense_keras/_modidx.py`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc2/mono_dense_keras/experiments.py` & `mono-dense-keras-0.0.6rc3/mono_dense_keras/experiments.py`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/SOURCES.txt` & `mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc2/settings.ini` & `mono-dense-keras-0.0.6rc3/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = mono-dense-keras
 lib_name = %(repo)s
-version = 0.0.6rc2
+version = 0.0.6rc3
 min_python = 3.7
 license = cc
 
 ### nbdev ###
 doc_path = _docs
 lib_path = mono_dense_keras
 nbs_path = nbs
```

### Comparing `mono-dense-keras-0.0.6rc2/setup.py` & `mono-dense-keras-0.0.6rc3/setup.py`

 * *Files identical despite different names*

