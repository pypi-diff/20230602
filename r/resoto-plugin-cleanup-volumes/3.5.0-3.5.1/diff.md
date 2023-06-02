# Comparing `tmp/resoto-plugin-cleanup-volumes-3.5.0.tar.gz` & `tmp/resoto-plugin-cleanup-volumes-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-volumes-3.5.0.tar", last modified: Fri May 26 18:23:21 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-volumes-3.5.1.tar", last modified: Fri Jun  2 14:53:56 2023, max compression
```

## Comparing `resoto-plugin-cleanup-volumes-3.5.0.tar` & `resoto-plugin-cleanup-volumes-3.5.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:21.432283 resoto-plugin-cleanup-volumes-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:38.000000 resoto-plugin-cleanup-volumes-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-26 18:23:21.432283 resoto-plugin-cleanup-volumes-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-26 18:21:38.000000 resoto-plugin-cleanup-volumes-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:21:38.000000 resoto-plugin-cleanup-volumes-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:21.432283 resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes/
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-26 18:21:38.000000 resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-26 18:21:38.000000 resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:21.432283 resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-26 18:23:21.000000 resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-26 18:23:21.000000 resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:21.000000 resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-26 18:23:21.000000 resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:21.000000 resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:23:21.000000 resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 18:23:21.000000 resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:23:21.432283 resoto-plugin-cleanup-volumes-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-26 18:21:38.000000 resoto-plugin-cleanup-volumes-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:21.432283 resoto-plugin-cleanup-volumes-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-26 18:21:38.000000 resoto-plugin-cleanup-volumes-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:56.153997 resoto-plugin-cleanup-volumes-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:51:11.000000 resoto-plugin-cleanup-volumes-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-02 14:53:56.157997 resoto-plugin-cleanup-volumes-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-02 14:51:11.000000 resoto-plugin-cleanup-volumes-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-02 14:51:11.000000 resoto-plugin-cleanup-volumes-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:56.153997 resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-02 14:51:11.000000 resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-02 14:51:11.000000 resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:56.153997 resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-02 14:53:56.000000 resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-02 14:53:56.000000 resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:53:56.000000 resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-02 14:53:56.000000 resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:52:17.000000 resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:53:56.000000 resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-02 14:53:56.000000 resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:53:56.157997 resoto-plugin-cleanup-volumes-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:56.153997 resoto-plugin-cleanup-volumes-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-02 14:51:11.000000 resoto-plugin-cleanup-volumes-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-volumes-3.5.0/PKG-INFO` & `resoto-plugin-cleanup-volumes-3.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-volumes
-Version: 3.5.0
+Version: 3.5.1
 Summary: Volume Cleaner Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_volumes
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_volumes
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
 
 # resoto-plugin-cleanup-volumes
 Volume cleanup plugin for Resoto
 
 This plugin cleans up storage volumes.
```

### Comparing `resoto-plugin-cleanup-volumes-3.5.0/README.md` & `resoto-plugin-cleanup-volumes-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes/__init__.py` & `resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes/config.py` & `resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO` & `resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-volumes
-Version: 3.5.0
+Version: 3.5.1
 Summary: Volume Cleaner Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_volumes
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_volumes
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
 
 # resoto-plugin-cleanup-volumes
 Volume cleanup plugin for Resoto
 
 This plugin cleans up storage volumes.
```

### Comparing `resoto-plugin-cleanup-volumes-3.5.0/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-volumes-3.5.1/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 resoto_plugin_cleanup_volumes/__init__.py
 resoto_plugin_cleanup_volumes/config.py
 resoto_plugin_cleanup_volumes.egg-info/PKG-INFO
 resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt
 resoto_plugin_cleanup_volumes.egg-info/dependency_links.txt
 resoto_plugin_cleanup_volumes.egg-info/entry_points.txt
 resoto_plugin_cleanup_volumes.egg-info/not-zip-safe
```

