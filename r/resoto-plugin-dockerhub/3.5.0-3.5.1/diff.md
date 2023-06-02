# Comparing `tmp/resoto-plugin-dockerhub-3.5.0.tar.gz` & `tmp/resoto-plugin-dockerhub-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-dockerhub-3.5.0.tar", last modified: Fri May 26 18:24:17 2023, max compression
+gzip compressed data, was "resoto-plugin-dockerhub-3.5.1.tar", last modified: Fri Jun  2 14:52:19 2023, max compression
```

## Comparing `resoto-plugin-dockerhub-3.5.0.tar` & `resoto-plugin-dockerhub-3.5.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.630671 resoto-plugin-dockerhub-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:47.000000 resoto-plugin-dockerhub-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-26 18:24:17.630671 resoto-plugin-dockerhub-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-26 18:21:47.000000 resoto-plugin-dockerhub-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 18:21:47.000000 resoto-plugin-dockerhub-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.626671 resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-26 18:21:47.000000 resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 18:21:47.000000 resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-26 18:21:47.000000 resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.630671 resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-26 18:24:17.000000 resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-26 18:24:17.000000 resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:17.000000 resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-26 18:24:17.000000 resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:17.000000 resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 18:24:17.000000 resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-26 18:24:17.000000 resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:24:17.634671 resoto-plugin-dockerhub-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-26 18:21:47.000000 resoto-plugin-dockerhub-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.630671 resoto-plugin-dockerhub-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-26 18:21:47.000000 resoto-plugin-dockerhub-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:19.756030 resoto-plugin-dockerhub-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:49:46.000000 resoto-plugin-dockerhub-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-02 14:52:19.756030 resoto-plugin-dockerhub-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-02 14:49:46.000000 resoto-plugin-dockerhub-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-02 14:49:46.000000 resoto-plugin-dockerhub-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:19.756030 resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-02 14:49:47.000000 resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-02 14:49:47.000000 resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-02 14:49:47.000000 resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:19.756030 resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-02 14:52:19.000000 resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-02 14:52:19.000000 resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:52:19.000000 resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-02 14:52:19.000000 resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:50:47.000000 resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 14:52:19.000000 resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 14:52:19.000000 resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:52:19.756030 resoto-plugin-dockerhub-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:19.756030 resoto-plugin-dockerhub-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-02 14:49:47.000000 resoto-plugin-dockerhub-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-dockerhub-3.5.0/PKG-INFO` & `resoto-plugin-dockerhub-3.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-dockerhub
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Docker Hub Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/dockerhub
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/dockerhub
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
 
 # resoto-plugin-dockerhub
 Docker Hub Collector Plugin for Resoto
 
 This collector plugin is used to collect data from Docker Hub. It is used internally at Some Engineering to create metrics about image downloads.
```

### Comparing `resoto-plugin-dockerhub-3.5.0/README.md` & `resoto-plugin-dockerhub-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub/__init__.py` & `resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub/resources.py` & `resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.5.0/resoto_plugin_dockerhub.egg-info/PKG-INFO` & `resoto-plugin-dockerhub-3.5.1/resoto_plugin_dockerhub.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-dockerhub
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Docker Hub Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/dockerhub
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/dockerhub
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
 
 # resoto-plugin-dockerhub
 Docker Hub Collector Plugin for Resoto
 
 This collector plugin is used to collect data from Docker Hub. It is used internally at Some Engineering to create metrics about image downloads.
```

