# Comparing `tmp/resoto-plugin-github-3.5.0.tar.gz` & `tmp/resoto-plugin-github-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-github-3.5.0.tar", last modified: Fri May 26 18:26:40 2023, max compression
+gzip compressed data, was "resoto-plugin-github-3.5.1.tar", last modified: Fri Jun  2 14:50:14 2023, max compression
```

## Comparing `resoto-plugin-github-3.5.0.tar` & `resoto-plugin-github-3.5.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:40.061689 resoto-plugin-github-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:24:21.000000 resoto-plugin-github-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-26 18:26:40.061689 resoto-plugin-github-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 18:24:21.000000 resoto-plugin-github-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-26 18:24:21.000000 resoto-plugin-github-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:40.061689 resoto-plugin-github-3.5.0/resoto_plugin_github/
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-05-26 18:24:21.000000 resoto-plugin-github-3.5.0/resoto_plugin_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-26 18:24:21.000000 resoto-plugin-github-3.5.0/resoto_plugin_github/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-05-26 18:24:21.000000 resoto-plugin-github-3.5.0/resoto_plugin_github/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:40.061689 resoto-plugin-github-3.5.0/resoto_plugin_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-26 18:26:40.000000 resoto-plugin-github-3.5.0/resoto_plugin_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-26 18:26:40.000000 resoto-plugin-github-3.5.0/resoto_plugin_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:26:40.000000 resoto-plugin-github-3.5.0/resoto_plugin_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 18:26:40.000000 resoto-plugin-github-3.5.0/resoto_plugin_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:26:40.000000 resoto-plugin-github-3.5.0/resoto_plugin_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-26 18:26:40.000000 resoto-plugin-github-3.5.0/resoto_plugin_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 18:26:40.000000 resoto-plugin-github-3.5.0/resoto_plugin_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:26:40.065689 resoto-plugin-github-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-26 18:24:21.000000 resoto-plugin-github-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:40.061689 resoto-plugin-github-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-26 18:24:21.000000 resoto-plugin-github-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:50:14.171762 resoto-plugin-github-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:47:32.000000 resoto-plugin-github-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-02 14:50:14.171762 resoto-plugin-github-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 14:47:32.000000 resoto-plugin-github-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-02 14:47:32.000000 resoto-plugin-github-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:50:14.167761 resoto-plugin-github-3.5.1/resoto_plugin_github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-02 14:47:32.000000 resoto-plugin-github-3.5.1/resoto_plugin_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-02 14:47:32.000000 resoto-plugin-github-3.5.1/resoto_plugin_github/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-06-02 14:47:32.000000 resoto-plugin-github-3.5.1/resoto_plugin_github/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:50:14.171762 resoto-plugin-github-3.5.1/resoto_plugin_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-02 14:50:14.000000 resoto-plugin-github-3.5.1/resoto_plugin_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-02 14:50:14.000000 resoto-plugin-github-3.5.1/resoto_plugin_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:50:14.000000 resoto-plugin-github-3.5.1/resoto_plugin_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 14:50:14.000000 resoto-plugin-github-3.5.1/resoto_plugin_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:48:38.000000 resoto-plugin-github-3.5.1/resoto_plugin_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 14:50:14.000000 resoto-plugin-github-3.5.1/resoto_plugin_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 14:50:14.000000 resoto-plugin-github-3.5.1/resoto_plugin_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:50:14.171762 resoto-plugin-github-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:50:14.171762 resoto-plugin-github-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-02 14:47:32.000000 resoto-plugin-github-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-github-3.5.0/PKG-INFO` & `resoto-plugin-github-3.5.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-github
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Github Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/github
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/github
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
 
 # resoto-plugin-github (WIP)
 GitHub Collector Plugin for Resoto
```

### Comparing `resoto-plugin-github-3.5.0/resoto_plugin_github/__init__.py` & `resoto-plugin-github-3.5.1/resoto_plugin_github/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-github-3.5.0/resoto_plugin_github/config.py` & `resoto-plugin-github-3.5.1/resoto_plugin_github/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-github-3.5.0/resoto_plugin_github/resources.py` & `resoto-plugin-github-3.5.1/resoto_plugin_github/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-github-3.5.0/resoto_plugin_github.egg-info/PKG-INFO` & `resoto-plugin-github-3.5.1/resoto_plugin_github.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-github
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Github Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/github
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/github
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
 
 # resoto-plugin-github (WIP)
 GitHub Collector Plugin for Resoto
```

