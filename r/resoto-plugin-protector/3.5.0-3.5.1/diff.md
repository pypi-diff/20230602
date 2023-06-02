# Comparing `tmp/resoto-plugin-protector-3.5.0.tar.gz` & `tmp/resoto-plugin-protector-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-protector-3.5.0.tar", last modified: Fri May 26 18:26:41 2023, max compression
+gzip compressed data, was "resoto-plugin-protector-3.5.1.tar", last modified: Fri Jun  2 14:48:49 2023, max compression
```

## Comparing `resoto-plugin-protector-3.5.0.tar` & `resoto-plugin-protector-3.5.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:41.756013 resoto-plugin-protector-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:25:04.000000 resoto-plugin-protector-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-26 18:26:41.756013 resoto-plugin-protector-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-26 18:25:04.000000 resoto-plugin-protector-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:25:04.000000 resoto-plugin-protector-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:41.756013 resoto-plugin-protector-3.5.0/resoto_plugin_protector/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-26 18:25:04.000000 resoto-plugin-protector-3.5.0/resoto_plugin_protector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-26 18:25:04.000000 resoto-plugin-protector-3.5.0/resoto_plugin_protector/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:41.756013 resoto-plugin-protector-3.5.0/resoto_plugin_protector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-26 18:26:41.000000 resoto-plugin-protector-3.5.0/resoto_plugin_protector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-26 18:26:41.000000 resoto-plugin-protector-3.5.0/resoto_plugin_protector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:26:41.000000 resoto-plugin-protector-3.5.0/resoto_plugin_protector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 18:26:41.000000 resoto-plugin-protector-3.5.0/resoto_plugin_protector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:26:41.000000 resoto-plugin-protector-3.5.0/resoto_plugin_protector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:26:41.000000 resoto-plugin-protector-3.5.0/resoto_plugin_protector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-26 18:26:41.000000 resoto-plugin-protector-3.5.0/resoto_plugin_protector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:26:41.760013 resoto-plugin-protector-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-26 18:25:04.000000 resoto-plugin-protector-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:41.756013 resoto-plugin-protector-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-26 18:25:04.000000 resoto-plugin-protector-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:48:49.196018 resoto-plugin-protector-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:46:02.000000 resoto-plugin-protector-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-02 14:48:49.196018 resoto-plugin-protector-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-02 14:46:02.000000 resoto-plugin-protector-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-02 14:46:02.000000 resoto-plugin-protector-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:48:49.196018 resoto-plugin-protector-3.5.1/resoto_plugin_protector/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-02 14:46:02.000000 resoto-plugin-protector-3.5.1/resoto_plugin_protector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-02 14:46:02.000000 resoto-plugin-protector-3.5.1/resoto_plugin_protector/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:48:49.196018 resoto-plugin-protector-3.5.1/resoto_plugin_protector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-02 14:48:49.000000 resoto-plugin-protector-3.5.1/resoto_plugin_protector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-02 14:48:49.000000 resoto-plugin-protector-3.5.1/resoto_plugin_protector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:48:49.000000 resoto-plugin-protector-3.5.1/resoto_plugin_protector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 14:48:49.000000 resoto-plugin-protector-3.5.1/resoto_plugin_protector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:47:08.000000 resoto-plugin-protector-3.5.1/resoto_plugin_protector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:48:49.000000 resoto-plugin-protector-3.5.1/resoto_plugin_protector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 14:48:49.000000 resoto-plugin-protector-3.5.1/resoto_plugin_protector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:48:49.196018 resoto-plugin-protector-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:48:49.196018 resoto-plugin-protector-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-02 14:46:02.000000 resoto-plugin-protector-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-protector-3.5.0/PKG-INFO` & `resoto-plugin-protector-3.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-protector
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Protector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/protector
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/protector
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
 
 # resoto-plugin-protector
 Protector Plugin for Resoto
 
 This plugin protects important resources from deletion by Resoto.
```

### Comparing `resoto-plugin-protector-3.5.0/README.md` & `resoto-plugin-protector-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.5.0/resoto_plugin_protector/__init__.py` & `resoto-plugin-protector-3.5.1/resoto_plugin_protector/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.5.0/resoto_plugin_protector/config.py` & `resoto-plugin-protector-3.5.1/resoto_plugin_protector/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.5.0/resoto_plugin_protector.egg-info/PKG-INFO` & `resoto-plugin-protector-3.5.1/resoto_plugin_protector.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-protector
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Protector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/protector
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/protector
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
 
 # resoto-plugin-protector
 Protector Plugin for Resoto
 
 This plugin protects important resources from deletion by Resoto.
```

