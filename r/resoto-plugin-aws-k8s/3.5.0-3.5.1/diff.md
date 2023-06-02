# Comparing `tmp/resoto-plugin-aws-k8s-3.5.0.tar.gz` & `tmp/resoto-plugin-aws-k8s-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-aws-k8s-3.5.0.tar", last modified: Fri May 26 18:24:18 2023, max compression
+gzip compressed data, was "resoto-plugin-aws-k8s-3.5.1.tar", last modified: Fri Jun  2 14:57:25 2023, max compression
```

## Comparing `resoto-plugin-aws-k8s-3.5.0.tar` & `resoto-plugin-aws-k8s-3.5.1.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:18.445371 resoto-plugin-aws-k8s-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-26 18:24:18.445371 resoto-plugin-aws-k8s-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:18.441372 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:18.441372 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-26 18:24:18.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-26 18:24:18.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:18.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 18:24:18.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:18.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:24:18.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 18:24:18.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:24:18.445371 resoto-plugin-aws-k8s-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:18.445371 resoto-plugin-aws-k8s-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/test/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:25.795444 resoto-plugin-aws-k8s-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:53:44.000000 resoto-plugin-aws-k8s-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-02 14:57:25.795444 resoto-plugin-aws-k8s-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-02 14:53:44.000000 resoto-plugin-aws-k8s-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-02 14:53:44.000000 resoto-plugin-aws-k8s-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:25.795444 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-02 14:53:44.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:25.795444 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-02 14:57:25.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-02 14:57:25.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:57:25.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-02 14:57:25.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:54:57.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 14:57:25.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-02 14:57:25.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:57:25.795444 resoto-plugin-aws-k8s-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:25.795444 resoto-plugin-aws-k8s-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:44.000000 resoto-plugin-aws-k8s-3.5.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 14:53:44.000000 resoto-plugin-aws-k8s-3.5.1/test/test_collector.py
```

### Comparing `resoto-plugin-aws-k8s-3.5.0/PKG-INFO` & `resoto-plugin-aws-k8s-3.5.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws-k8s
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto AWS-K8s Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/aws_k8s
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws_k8s
+Keywords: aws,k8s
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
+Provides-Extra: dev
 
 # resoto-plugin-aws-k8s
 AWS - K8s Collector Plugin for Resoto: link together your AWS and k8s cluster resources.
```

### Comparing `resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s/__init__.py` & `resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/PKG-INFO` & `resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws-k8s
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto AWS-K8s Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/aws_k8s
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws_k8s
+Keywords: aws,k8s
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
+Provides-Extra: dev
 
 # resoto-plugin-aws-k8s
 AWS - K8s Collector Plugin for Resoto: link together your AWS and k8s cluster resources.
```

### Comparing `resoto-plugin-aws-k8s-3.5.0/test/test_collector.py` & `resoto-plugin-aws-k8s-3.5.1/test/test_collector.py`

 * *Files identical despite different names*

