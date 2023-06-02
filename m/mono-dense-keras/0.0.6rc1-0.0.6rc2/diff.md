# Comparing `tmp/mono-dense-keras-0.0.6rc1.tar.gz` & `tmp/mono-dense-keras-0.0.6rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mono-dense-keras-0.0.6rc1.tar", last modified: Fri May 26 14:28:10 2023, max compression
+gzip compressed data, was "mono-dense-keras-0.0.6rc2.tar", last modified: Fri Jun  2 14:10:10 2023, max compression
```

## Comparing `mono-dense-keras-0.0.6rc1.tar` & `mono-dense-keras-0.0.6rc2.tar`

### file list

```diff
@@ -1,28 +1,24 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/
--rw-r--r--   0 davor     (1000) davor     (1000)    20848 2022-09-02 19:27:53.000000 mono-dense-keras-0.0.6rc1/LICENSE
--rw-rw-r--   0 davor     (1000) davor     (1000)      111 2022-08-18 19:39:58.000000 mono-dense-keras-0.0.6rc1/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)     7659 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)     6546 2023-05-26 14:19:35.000000 mono-dense-keras-0.0.6rc1/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/airt/
--rw-r--r--   0 davor     (1000) davor     (1000)       22 2022-09-03 17:11:42.000000 mono-dense-keras-0.0.6rc1/airt/__init__.py
--rw-r--r--   0 davor     (1000) davor     (1000)     1275 2022-09-03 17:11:04.000000 mono-dense-keras-0.0.6rc1/airt/_modidx.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/airt/keras/
--rw-r--r--   0 davor     (1000) davor     (1000)        0 2022-09-03 17:11:01.000000 mono-dense-keras-0.0.6rc1/airt/keras/__init__.py
--rw-r--r--   0 davor     (1000) davor     (1000)     3906 2022-09-03 17:11:01.000000 mono-dense-keras-0.0.6rc1/airt/keras/layers.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/mono_dense_keras/
--rw-rw-r--   0 davor     (1000) davor     (1000)      472 2023-05-26 14:27:26.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/mono_dense_keras/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-05-26 14:27:26.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    10318 2023-05-26 14:27:26.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras/_components/mono_dense_layer.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     4050 2023-05-26 14:27:26.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras/_modidx.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/
--rw-r--r--   0 davor     (1000) davor     (1000)     7659 2023-05-26 14:28:10.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/PKG-INFO
--rw-r--r--   0 davor     (1000) davor     (1000)      556 2023-05-26 14:28:10.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/SOURCES.txt
--rw-r--r--   0 davor     (1000) davor     (1000)        1 2023-05-26 14:28:10.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/dependency_links.txt
--rw-r--r--   0 davor     (1000) davor     (1000)       54 2023-05-26 14:28:10.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/entry_points.txt
--rw-r--r--   0 davor     (1000) davor     (1000)        1 2022-12-06 04:51:35.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/not-zip-safe
--rw-r--r--   0 davor     (1000) davor     (1000)      219 2023-05-26 14:28:10.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/requires.txt
--rw-r--r--   0 davor     (1000) davor     (1000)       22 2023-05-26 14:28:10.000000 mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/top_level.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)      969 2023-05-26 14:27:16.000000 mono-dense-keras-0.0.6rc1/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-05-26 14:28:10.871570 mono-dense-keras-0.0.6rc1/setup.cfg
--rw-rw-r--   0 davor     (1000) davor     (1000)     3081 2023-05-26 14:25:56.000000 mono-dense-keras-0.0.6rc1/setup.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:10:10.739577 mono-dense-keras-0.0.6rc2/
+-rw-r--r--   0 davor     (1000) davor     (1000)    20848 2022-09-02 19:27:53.000000 mono-dense-keras-0.0.6rc2/LICENSE
+-rw-rw-r--   0 davor     (1000) davor     (1000)      111 2022-08-18 19:39:58.000000 mono-dense-keras-0.0.6rc2/MANIFEST.in
+-rw-rw-r--   0 davor     (1000) davor     (1000)     7659 2023-06-02 14:10:10.739577 mono-dense-keras-0.0.6rc2/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)     6546 2023-06-01 08:50:38.000000 mono-dense-keras-0.0.6rc2/README.md
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:10:10.735577 mono-dense-keras-0.0.6rc2/mono_dense_keras/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      463 2023-06-02 14:08:39.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:10:10.739577 mono-dense-keras-0.0.6rc2/mono_dense_keras/_components/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-02 13:55:48.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras/_components/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    23910 2023-06-02 14:08:39.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras/_components/mono_dense_layer.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10897 2023-06-02 14:08:39.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras/_modidx.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    14065 2023-06-02 14:08:39.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras/experiments.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      288 2023-06-02 13:55:48.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras/helpers.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:10:10.739577 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/
+-rw-r--r--   0 davor     (1000) davor     (1000)     7659 2023-06-02 14:10:10.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/PKG-INFO
+-rw-r--r--   0 davor     (1000) davor     (1000)      539 2023-06-02 14:10:10.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/SOURCES.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)        1 2023-06-02 14:10:10.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/dependency_links.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)       54 2023-06-02 14:10:10.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/entry_points.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)        1 2022-12-06 04:51:35.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/not-zip-safe
+-rw-r--r--   0 davor     (1000) davor     (1000)      224 2023-06-02 14:10:10.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/requires.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)       17 2023-06-02 14:10:10.000000 mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/top_level.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)      969 2023-06-02 14:09:59.000000 mono-dense-keras-0.0.6rc2/settings.ini
+-rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-02 14:10:10.739577 mono-dense-keras-0.0.6rc2/setup.cfg
+-rw-rw-r--   0 davor     (1000) davor     (1000)     3093 2023-06-02 14:08:39.000000 mono-dense-keras-0.0.6rc2/setup.py
```

### Comparing `mono-dense-keras-0.0.6rc1/LICENSE` & `mono-dense-keras-0.0.6rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc1/PKG-INFO` & `mono-dense-keras-0.0.6rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mono-dense-keras
-Version: 0.0.6rc1
+Version: 0.0.6rc2
 Summary: Monotonic Dense Layer implemented in Keras
 Home-page: https://github.com/airtai/mono-dense-keras
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/mono-dense-keras/issues
 Project-URL: CI, https://github.com/airtai/mono-dense-keras/actions
```

### Comparing `mono-dense-keras-0.0.6rc1/README.md` & `mono-dense-keras-0.0.6rc2/README.md`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc1/mono_dense_keras.egg-info/PKG-INFO` & `mono-dense-keras-0.0.6rc2/mono_dense_keras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mono-dense-keras
-Version: 0.0.6rc1
+Version: 0.0.6rc2
 Summary: Monotonic Dense Layer implemented in Keras
 Home-page: https://github.com/airtai/mono-dense-keras
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/mono-dense-keras/issues
 Project-URL: CI, https://github.com/airtai/mono-dense-keras/actions
```

### Comparing `mono-dense-keras-0.0.6rc1/settings.ini` & `mono-dense-keras-0.0.6rc2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = mono-dense-keras
 lib_name = %(repo)s
-version = 0.0.6rc1
+version = 0.0.6rc2
 min_python = 3.7
 license = cc
 
 ### nbdev ###
 doc_path = _docs
 lib_path = mono_dense_keras
 nbs_path = nbs
```

### Comparing `mono-dense-keras-0.0.6rc1/setup.py` & `mono-dense-keras-0.0.6rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,26 @@
 min_python = cfg['min_python']
 lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
 
 requirements = ["tensorflow>=2.10.0"]
     
 dev_requirements = [
     "keras-tuner[bayesian]==1.3.5",
-    "nbdev_mkdocs==0.5.0",
+    "nbdev_mkdocs==0.5.1",
     "pytest==7.3.1",
     "pandas>=1.3.5",
     "nbqa==1.7.0",
     "black==23.3.0",
     "isort==5.12.0",
     "matplotlib==3.7.1",
     "seaborn==0.12.2",
     "mypy==1.3.0",
     "bandit==1.7.5",
     "semgrep==1.23.0",
+    "tqdm",
 ]
 
 project_urls = {
    'Bug Tracker': cfg['git_url'] + '/issues',
    'CI': cfg['git_url'] + '/actions',
    'Documentation': 'https://mono-dense-keras.airt.ai/',
 #    'Tutorial': 'https://colab.research.google.com/github/airtai/fastkafka/blob/main/nbs/guides/Guide_00_FastKafka_Demo.ipynb'
```

