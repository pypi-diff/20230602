# Comparing `tmp/resoto-plugin-slack-3.5.0.tar.gz` & `tmp/resoto-plugin-slack-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-slack-3.5.0.tar", last modified: Fri May 26 18:23:23 2023, max compression
+gzip compressed data, was "resoto-plugin-slack-3.5.1.tar", last modified: Fri Jun  2 14:51:59 2023, max compression
```

## Comparing `resoto-plugin-slack-3.5.0.tar` & `resoto-plugin-slack-3.5.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:23.553272 resoto-plugin-slack-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:37.000000 resoto-plugin-slack-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-26 18:23:23.553272 resoto-plugin-slack-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-26 18:21:37.000000 resoto-plugin-slack-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 18:21:37.000000 resoto-plugin-slack-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:23.553272 resoto-plugin-slack-3.5.0/resoto_plugin_slack/
--rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-05-26 18:21:37.000000 resoto-plugin-slack-3.5.0/resoto_plugin_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 18:21:37.000000 resoto-plugin-slack-3.5.0/resoto_plugin_slack/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-26 18:21:37.000000 resoto-plugin-slack-3.5.0/resoto_plugin_slack/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:23.553272 resoto-plugin-slack-3.5.0/resoto_plugin_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-26 18:23:23.000000 resoto-plugin-slack-3.5.0/resoto_plugin_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-26 18:23:23.000000 resoto-plugin-slack-3.5.0/resoto_plugin_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:23.000000 resoto-plugin-slack-3.5.0/resoto_plugin_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-26 18:23:23.000000 resoto-plugin-slack-3.5.0/resoto_plugin_slack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:23.000000 resoto-plugin-slack-3.5.0/resoto_plugin_slack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 18:23:23.000000 resoto-plugin-slack-3.5.0/resoto_plugin_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 18:23:23.000000 resoto-plugin-slack-3.5.0/resoto_plugin_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:23:23.553272 resoto-plugin-slack-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-26 18:21:37.000000 resoto-plugin-slack-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:23.553272 resoto-plugin-slack-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-26 18:21:37.000000 resoto-plugin-slack-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:59.359762 resoto-plugin-slack-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:49:15.000000 resoto-plugin-slack-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-02 14:51:59.359762 resoto-plugin-slack-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 14:49:15.000000 resoto-plugin-slack-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-02 14:49:15.000000 resoto-plugin-slack-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:59.355762 resoto-plugin-slack-3.5.1/resoto_plugin_slack/
+-rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-06-02 14:49:15.000000 resoto-plugin-slack-3.5.1/resoto_plugin_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-02 14:49:15.000000 resoto-plugin-slack-3.5.1/resoto_plugin_slack/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-02 14:49:15.000000 resoto-plugin-slack-3.5.1/resoto_plugin_slack/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:59.359762 resoto-plugin-slack-3.5.1/resoto_plugin_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-02 14:51:59.000000 resoto-plugin-slack-3.5.1/resoto_plugin_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-02 14:51:59.000000 resoto-plugin-slack-3.5.1/resoto_plugin_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:51:59.000000 resoto-plugin-slack-3.5.1/resoto_plugin_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-02 14:51:59.000000 resoto-plugin-slack-3.5.1/resoto_plugin_slack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:50:20.000000 resoto-plugin-slack-3.5.1/resoto_plugin_slack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-02 14:51:59.000000 resoto-plugin-slack-3.5.1/resoto_plugin_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 14:51:59.000000 resoto-plugin-slack-3.5.1/resoto_plugin_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:51:59.359762 resoto-plugin-slack-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:59.359762 resoto-plugin-slack-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-02 14:49:15.000000 resoto-plugin-slack-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-slack-3.5.0/PKG-INFO` & `resoto-plugin-slack-3.5.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-slack
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Slack Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/slack
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/slack
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
 
 # resoto-plugin-slack
 Slack collector for Resoto
```

### Comparing `resoto-plugin-slack-3.5.0/resoto_plugin_slack/__init__.py` & `resoto-plugin-slack-3.5.1/resoto_plugin_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-slack-3.5.0/resoto_plugin_slack/resources.py` & `resoto-plugin-slack-3.5.1/resoto_plugin_slack/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-slack-3.5.0/resoto_plugin_slack.egg-info/PKG-INFO` & `resoto-plugin-slack-3.5.1/resoto_plugin_slack.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-slack
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Slack Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/slack
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/slack
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
 
 # resoto-plugin-slack
 Slack collector for Resoto
```

