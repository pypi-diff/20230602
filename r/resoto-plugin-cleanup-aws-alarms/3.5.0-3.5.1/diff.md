# Comparing `tmp/resoto-plugin-cleanup-aws-alarms-3.5.0.tar.gz` & `tmp/resoto-plugin-cleanup-aws-alarms-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-aws-alarms-3.5.0.tar", last modified: Fri May 26 18:27:09 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-aws-alarms-3.5.1.tar", last modified: Fri Jun  2 14:49:24 2023, max compression
```

## Comparing `resoto-plugin-cleanup-aws-alarms-3.5.0.tar` & `resoto-plugin-cleanup-aws-alarms-3.5.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:27:09.683095 resoto-plugin-cleanup-aws-alarms-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:24:22.000000 resoto-plugin-cleanup-aws-alarms-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-26 18:27:09.683095 resoto-plugin-cleanup-aws-alarms-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-26 18:24:22.000000 resoto-plugin-cleanup-aws-alarms-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 18:24:22.000000 resoto-plugin-cleanup-aws-alarms-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:27:09.679095 resoto-plugin-cleanup-aws-alarms-3.5.0/resoto_plugin_cleanup_aws_alarms/
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-26 18:24:22.000000 resoto-plugin-cleanup-aws-alarms-3.5.0/resoto_plugin_cleanup_aws_alarms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-26 18:24:22.000000 resoto-plugin-cleanup-aws-alarms-3.5.0/resoto_plugin_cleanup_aws_alarms/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:27:09.683095 resoto-plugin-cleanup-aws-alarms-3.5.0/resoto_plugin_cleanup_aws_alarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-26 18:27:09.000000 resoto-plugin-cleanup-aws-alarms-3.5.0/resoto_plugin_cleanup_aws_alarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-26 18:27:09.000000 resoto-plugin-cleanup-aws-alarms-3.5.0/resoto_plugin_cleanup_aws_alarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:27:09.000000 resoto-plugin-cleanup-aws-alarms-3.5.0/resoto_plugin_cleanup_aws_alarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 18:27:09.000000 resoto-plugin-cleanup-aws-alarms-3.5.0/resoto_plugin_cleanup_aws_alarms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:27:09.000000 resoto-plugin-cleanup-aws-alarms-3.5.0/resoto_plugin_cleanup_aws_alarms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 18:27:09.000000 resoto-plugin-cleanup-aws-alarms-3.5.0/resoto_plugin_cleanup_aws_alarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 18:27:09.000000 resoto-plugin-cleanup-aws-alarms-3.5.0/resoto_plugin_cleanup_aws_alarms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:27:09.683095 resoto-plugin-cleanup-aws-alarms-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-26 18:24:22.000000 resoto-plugin-cleanup-aws-alarms-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:27:09.683095 resoto-plugin-cleanup-aws-alarms-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 18:24:22.000000 resoto-plugin-cleanup-aws-alarms-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:24.633660 resoto-plugin-cleanup-aws-alarms-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:46:29.000000 resoto-plugin-cleanup-aws-alarms-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-02 14:49:24.633660 resoto-plugin-cleanup-aws-alarms-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-02 14:46:29.000000 resoto-plugin-cleanup-aws-alarms-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-02 14:46:29.000000 resoto-plugin-cleanup-aws-alarms-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:24.629660 resoto-plugin-cleanup-aws-alarms-3.5.1/resoto_plugin_cleanup_aws_alarms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-02 14:46:29.000000 resoto-plugin-cleanup-aws-alarms-3.5.1/resoto_plugin_cleanup_aws_alarms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-02 14:46:29.000000 resoto-plugin-cleanup-aws-alarms-3.5.1/resoto_plugin_cleanup_aws_alarms/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:24.633660 resoto-plugin-cleanup-aws-alarms-3.5.1/resoto_plugin_cleanup_aws_alarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-02 14:49:24.000000 resoto-plugin-cleanup-aws-alarms-3.5.1/resoto_plugin_cleanup_aws_alarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-02 14:49:24.000000 resoto-plugin-cleanup-aws-alarms-3.5.1/resoto_plugin_cleanup_aws_alarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:49:24.000000 resoto-plugin-cleanup-aws-alarms-3.5.1/resoto_plugin_cleanup_aws_alarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-02 14:49:24.000000 resoto-plugin-cleanup-aws-alarms-3.5.1/resoto_plugin_cleanup_aws_alarms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:47:41.000000 resoto-plugin-cleanup-aws-alarms-3.5.1/resoto_plugin_cleanup_aws_alarms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:49:24.000000 resoto-plugin-cleanup-aws-alarms-3.5.1/resoto_plugin_cleanup_aws_alarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 14:49:24.000000 resoto-plugin-cleanup-aws-alarms-3.5.1/resoto_plugin_cleanup_aws_alarms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:49:24.633660 resoto-plugin-cleanup-aws-alarms-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:24.633660 resoto-plugin-cleanup-aws-alarms-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-02 14:46:29.000000 resoto-plugin-cleanup-aws-alarms-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-aws-alarms-3.5.0/PKG-INFO` & `resoto-plugin-cleanup-aws-alarms-3.5.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-alarms
-Version: 3.5.0
+Version: 3.5.1
 Summary: AWS Cloudwatch Alarms Cleaner Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_alarms
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_alarms
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
 
 # resoto-plugin-cleanup-aws-alarms
 AWS Cloudwatch Alarms Cleanup Plugin for Resoto
 
 This plugin marks all orphaned AWS CloudWatch Instance Alarms for cleanup.
```

### Comparing `resoto-plugin-cleanup-aws-alarms-3.5.0/README.md` & `resoto-plugin-cleanup-aws-alarms-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-alarms-3.5.0/resoto_plugin_cleanup_aws_alarms/__init__.py` & `resoto-plugin-cleanup-aws-alarms-3.5.1/resoto_plugin_cleanup_aws_alarms/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-alarms-3.5.0/resoto_plugin_cleanup_aws_alarms/config.py` & `resoto-plugin-cleanup-aws-alarms-3.5.1/resoto_plugin_cleanup_aws_alarms/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-alarms-3.5.0/resoto_plugin_cleanup_aws_alarms.egg-info/PKG-INFO` & `resoto-plugin-cleanup-aws-alarms-3.5.1/resoto_plugin_cleanup_aws_alarms.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-alarms
-Version: 3.5.0
+Version: 3.5.1
 Summary: AWS Cloudwatch Alarms Cleaner Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_alarms
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_alarms
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
 
 # resoto-plugin-cleanup-aws-alarms
 AWS Cloudwatch Alarms Cleanup Plugin for Resoto
 
 This plugin marks all orphaned AWS CloudWatch Instance Alarms for cleanup.
```

