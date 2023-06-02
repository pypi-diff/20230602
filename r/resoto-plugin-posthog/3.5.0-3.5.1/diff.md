# Comparing `tmp/resoto-plugin-posthog-3.5.0.tar.gz` & `tmp/resoto-plugin-posthog-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-posthog-3.5.0.tar", last modified: Fri May 26 18:26:51 2023, max compression
+gzip compressed data, was "resoto-plugin-posthog-3.5.1.tar", last modified: Fri Jun  2 14:53:29 2023, max compression
```

## Comparing `resoto-plugin-posthog-3.5.0.tar` & `resoto-plugin-posthog-3.5.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:51.730023 resoto-plugin-posthog-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:24:52.000000 resoto-plugin-posthog-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-26 18:26:51.730023 resoto-plugin-posthog-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-26 18:24:52.000000 resoto-plugin-posthog-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 18:24:52.000000 resoto-plugin-posthog-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:51.730023 resoto-plugin-posthog-3.5.0/resoto_plugin_posthog/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-26 18:24:52.000000 resoto-plugin-posthog-3.5.0/resoto_plugin_posthog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-26 18:24:52.000000 resoto-plugin-posthog-3.5.0/resoto_plugin_posthog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-26 18:24:52.000000 resoto-plugin-posthog-3.5.0/resoto_plugin_posthog/posthog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-26 18:24:52.000000 resoto-plugin-posthog-3.5.0/resoto_plugin_posthog/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:51.730023 resoto-plugin-posthog-3.5.0/resoto_plugin_posthog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-26 18:26:51.000000 resoto-plugin-posthog-3.5.0/resoto_plugin_posthog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-26 18:26:51.000000 resoto-plugin-posthog-3.5.0/resoto_plugin_posthog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:26:51.000000 resoto-plugin-posthog-3.5.0/resoto_plugin_posthog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-26 18:26:51.000000 resoto-plugin-posthog-3.5.0/resoto_plugin_posthog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:26:51.000000 resoto-plugin-posthog-3.5.0/resoto_plugin_posthog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 18:26:51.000000 resoto-plugin-posthog-3.5.0/resoto_plugin_posthog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 18:26:51.000000 resoto-plugin-posthog-3.5.0/resoto_plugin_posthog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:26:51.730023 resoto-plugin-posthog-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-26 18:24:52.000000 resoto-plugin-posthog-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:51.730023 resoto-plugin-posthog-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 18:24:52.000000 resoto-plugin-posthog-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:29.812331 resoto-plugin-posthog-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:50:46.000000 resoto-plugin-posthog-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-02 14:53:29.812331 resoto-plugin-posthog-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-02 14:50:46.000000 resoto-plugin-posthog-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-02 14:50:46.000000 resoto-plugin-posthog-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:29.812331 resoto-plugin-posthog-3.5.1/resoto_plugin_posthog/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-02 14:50:46.000000 resoto-plugin-posthog-3.5.1/resoto_plugin_posthog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-02 14:50:46.000000 resoto-plugin-posthog-3.5.1/resoto_plugin_posthog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-02 14:50:46.000000 resoto-plugin-posthog-3.5.1/resoto_plugin_posthog/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-02 14:50:46.000000 resoto-plugin-posthog-3.5.1/resoto_plugin_posthog/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:29.812331 resoto-plugin-posthog-3.5.1/resoto_plugin_posthog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-02 14:53:29.000000 resoto-plugin-posthog-3.5.1/resoto_plugin_posthog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-02 14:53:29.000000 resoto-plugin-posthog-3.5.1/resoto_plugin_posthog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:53:29.000000 resoto-plugin-posthog-3.5.1/resoto_plugin_posthog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-02 14:53:29.000000 resoto-plugin-posthog-3.5.1/resoto_plugin_posthog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:51:52.000000 resoto-plugin-posthog-3.5.1/resoto_plugin_posthog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 14:53:29.000000 resoto-plugin-posthog-3.5.1/resoto_plugin_posthog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 14:53:29.000000 resoto-plugin-posthog-3.5.1/resoto_plugin_posthog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:53:29.812331 resoto-plugin-posthog-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:29.812331 resoto-plugin-posthog-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-02 14:50:46.000000 resoto-plugin-posthog-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-posthog-3.5.0/PKG-INFO` & `resoto-plugin-posthog-3.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-posthog
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Posthog Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/posthog
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/posthog
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
 
 # resoto-plugin-posthog
 Posthog Collector Plugin for Resoto
 
 This collector plugin is used to collect data from Posthog. It is used internally at Some Engineering to create metrics about resoto installations and usage.
```

### Comparing `resoto-plugin-posthog-3.5.0/README.md` & `resoto-plugin-posthog-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.5.0/resoto_plugin_posthog/__init__.py` & `resoto-plugin-posthog-3.5.1/resoto_plugin_posthog/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.5.0/resoto_plugin_posthog/posthog.py` & `resoto-plugin-posthog-3.5.1/resoto_plugin_posthog/posthog.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.5.0/resoto_plugin_posthog/resources.py` & `resoto-plugin-posthog-3.5.1/resoto_plugin_posthog/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.5.0/resoto_plugin_posthog.egg-info/PKG-INFO` & `resoto-plugin-posthog-3.5.1/resoto_plugin_posthog.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-posthog
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Posthog Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/posthog
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/posthog
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
 
 # resoto-plugin-posthog
 Posthog Collector Plugin for Resoto
 
 This collector plugin is used to collect data from Posthog. It is used internally at Some Engineering to create metrics about resoto installations and usage.
```

### Comparing `resoto-plugin-posthog-3.5.0/resoto_plugin_posthog.egg-info/SOURCES.txt` & `resoto-plugin-posthog-3.5.1/resoto_plugin_posthog.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 resoto_plugin_posthog/__init__.py
 resoto_plugin_posthog/config.py
 resoto_plugin_posthog/posthog.py
 resoto_plugin_posthog/resources.py
 resoto_plugin_posthog.egg-info/PKG-INFO
 resoto_plugin_posthog.egg-info/SOURCES.txt
 resoto_plugin_posthog.egg-info/dependency_links.txt
```

