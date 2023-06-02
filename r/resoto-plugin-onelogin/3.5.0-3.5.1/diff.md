# Comparing `tmp/resoto-plugin-onelogin-3.5.0.tar.gz` & `tmp/resoto-plugin-onelogin-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-onelogin-3.5.0.tar", last modified: Fri May 26 18:23:26 2023, max compression
+gzip compressed data, was "resoto-plugin-onelogin-3.5.1.tar", last modified: Fri Jun  2 14:54:23 2023, max compression
```

## Comparing `resoto-plugin-onelogin-3.5.0.tar` & `resoto-plugin-onelogin-3.5.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:26.737770 resoto-plugin-onelogin-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:38.000000 resoto-plugin-onelogin-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-26 18:23:26.737770 resoto-plugin-onelogin-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-26 18:21:38.000000 resoto-plugin-onelogin-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 18:21:38.000000 resoto-plugin-onelogin-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:26.737770 resoto-plugin-onelogin-3.5.0/resoto_plugin_onelogin/
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-26 18:21:38.000000 resoto-plugin-onelogin-3.5.0/resoto_plugin_onelogin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-26 18:21:38.000000 resoto-plugin-onelogin-3.5.0/resoto_plugin_onelogin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:26.737770 resoto-plugin-onelogin-3.5.0/resoto_plugin_onelogin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-26 18:23:26.000000 resoto-plugin-onelogin-3.5.0/resoto_plugin_onelogin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-26 18:23:26.000000 resoto-plugin-onelogin-3.5.0/resoto_plugin_onelogin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:26.000000 resoto-plugin-onelogin-3.5.0/resoto_plugin_onelogin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-26 18:23:26.000000 resoto-plugin-onelogin-3.5.0/resoto_plugin_onelogin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:26.000000 resoto-plugin-onelogin-3.5.0/resoto_plugin_onelogin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 18:23:26.000000 resoto-plugin-onelogin-3.5.0/resoto_plugin_onelogin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 18:23:26.000000 resoto-plugin-onelogin-3.5.0/resoto_plugin_onelogin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:23:26.741770 resoto-plugin-onelogin-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-26 18:21:38.000000 resoto-plugin-onelogin-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:26.737770 resoto-plugin-onelogin-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-26 18:21:38.000000 resoto-plugin-onelogin-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:23.494231 resoto-plugin-onelogin-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:50:52.000000 resoto-plugin-onelogin-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-02 14:54:23.494231 resoto-plugin-onelogin-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-02 14:50:52.000000 resoto-plugin-onelogin-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-02 14:50:52.000000 resoto-plugin-onelogin-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:23.494231 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin/
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-02 14:50:52.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-02 14:50:52.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:23.494231 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-02 14:54:23.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-02 14:54:23.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:54:23.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-02 14:54:23.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:52:19.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 14:54:23.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:54:23.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:54:23.494231 resoto-plugin-onelogin-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:23.494231 resoto-plugin-onelogin-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-02 14:50:52.000000 resoto-plugin-onelogin-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-onelogin-3.5.0/PKG-INFO` & `resoto-plugin-onelogin-3.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onelogin
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto OneLogin Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/onelogin
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/onelogin
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
 
 # resoto-plugin-onelogin
 OneLogin collector plugin for Resoto
 
 This plugin collects OneLogin users as cloud resources and adds them to the Resoto graph for use by other plugins.
```

### Comparing `resoto-plugin-onelogin-3.5.0/resoto_plugin_onelogin/__init__.py` & `resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onelogin-3.5.0/resoto_plugin_onelogin.egg-info/PKG-INFO` & `resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onelogin
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto OneLogin Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/onelogin
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/onelogin
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
 
 # resoto-plugin-onelogin
 OneLogin collector plugin for Resoto
 
 This plugin collects OneLogin users as cloud resources and adds them to the Resoto graph for use by other plugins.
```

