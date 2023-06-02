# Comparing `tmp/resoto-plugin-random-3.5.0.tar.gz` & `tmp/resoto-plugin-random-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-random-3.5.0.tar", last modified: Fri May 26 18:23:16 2023, max compression
+gzip compressed data, was "resoto-plugin-random-3.5.1.tar", last modified: Fri Jun  2 14:52:52 2023, max compression
```

## Comparing `resoto-plugin-random-3.5.0.tar` & `resoto-plugin-random-3.5.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:16.345168 resoto-plugin-random-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:35.000000 resoto-plugin-random-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-26 18:23:16.345168 resoto-plugin-random-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-26 18:21:35.000000 resoto-plugin-random-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:21:35.000000 resoto-plugin-random-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:16.345168 resoto-plugin-random-3.5.0/resoto_plugin_random/
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-05-26 18:21:35.000000 resoto-plugin-random-3.5.0/resoto_plugin_random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-26 18:21:35.000000 resoto-plugin-random-3.5.0/resoto_plugin_random/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-26 18:21:35.000000 resoto-plugin-random-3.5.0/resoto_plugin_random/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:16.345168 resoto-plugin-random-3.5.0/resoto_plugin_random.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-26 18:23:16.000000 resoto-plugin-random-3.5.0/resoto_plugin_random.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-26 18:23:16.000000 resoto-plugin-random-3.5.0/resoto_plugin_random.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:16.000000 resoto-plugin-random-3.5.0/resoto_plugin_random.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 18:23:16.000000 resoto-plugin-random-3.5.0/resoto_plugin_random.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:16.000000 resoto-plugin-random-3.5.0/resoto_plugin_random.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:23:16.000000 resoto-plugin-random-3.5.0/resoto_plugin_random.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 18:23:16.000000 resoto-plugin-random-3.5.0/resoto_plugin_random.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:23:16.345168 resoto-plugin-random-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-26 18:21:35.000000 resoto-plugin-random-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:16.345168 resoto-plugin-random-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-26 18:21:35.000000 resoto-plugin-random-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:52.476053 resoto-plugin-random-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:49:39.000000 resoto-plugin-random-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-02 14:52:52.476053 resoto-plugin-random-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-02 14:49:39.000000 resoto-plugin-random-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-02 14:49:39.000000 resoto-plugin-random-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:52.476053 resoto-plugin-random-3.5.1/resoto_plugin_random/
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-02 14:49:39.000000 resoto-plugin-random-3.5.1/resoto_plugin_random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-02 14:49:39.000000 resoto-plugin-random-3.5.1/resoto_plugin_random/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-06-02 14:49:39.000000 resoto-plugin-random-3.5.1/resoto_plugin_random/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:52.476053 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-02 14:52:52.000000 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-02 14:52:52.000000 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:52:52.000000 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 14:52:52.000000 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:50:58.000000 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:52:52.000000 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 14:52:52.000000 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:52:52.480053 resoto-plugin-random-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:52.476053 resoto-plugin-random-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-02 14:49:39.000000 resoto-plugin-random-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-random-3.5.0/PKG-INFO` & `resoto-plugin-random-3.5.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-random
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Random Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/random
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/random
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # resoto-plugin-random
 Random Cloud Collector for Resoto
 
 Creates a plausible pseudo-random cloud based on a configurable seed.
```

### Comparing `resoto-plugin-random-3.5.0/README.md` & `resoto-plugin-random-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-random-3.5.0/resoto_plugin_random/__init__.py` & `resoto-plugin-random-3.5.1/resoto_plugin_random/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-random-3.5.0/resoto_plugin_random/resources.py` & `resoto-plugin-random-3.5.1/resoto_plugin_random/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-random-3.5.0/resoto_plugin_random.egg-info/PKG-INFO` & `resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-random
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Random Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/random
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/random
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # resoto-plugin-random
 Random Cloud Collector for Resoto
 
 Creates a plausible pseudo-random cloud based on a configurable seed.
```

