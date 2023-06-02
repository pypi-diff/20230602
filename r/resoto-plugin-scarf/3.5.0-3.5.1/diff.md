# Comparing `tmp/resoto-plugin-scarf-3.5.0.tar.gz` & `tmp/resoto-plugin-scarf-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-scarf-3.5.0.tar", last modified: Fri May 26 18:23:43 2023, max compression
+gzip compressed data, was "resoto-plugin-scarf-3.5.1.tar", last modified: Fri Jun  2 14:55:35 2023, max compression
```

## Comparing `resoto-plugin-scarf-3.5.0.tar` & `resoto-plugin-scarf-3.5.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:43.392379 resoto-plugin-scarf-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:40.000000 resoto-plugin-scarf-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-26 18:23:43.392379 resoto-plugin-scarf-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-26 18:21:40.000000 resoto-plugin-scarf-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 18:21:40.000000 resoto-plugin-scarf-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:43.392379 resoto-plugin-scarf-3.5.0/resoto_plugin_scarf/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-26 18:21:40.000000 resoto-plugin-scarf-3.5.0/resoto_plugin_scarf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-26 18:21:40.000000 resoto-plugin-scarf-3.5.0/resoto_plugin_scarf/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-26 18:21:40.000000 resoto-plugin-scarf-3.5.0/resoto_plugin_scarf/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-26 18:21:40.000000 resoto-plugin-scarf-3.5.0/resoto_plugin_scarf/scarf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:43.392379 resoto-plugin-scarf-3.5.0/resoto_plugin_scarf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-26 18:23:43.000000 resoto-plugin-scarf-3.5.0/resoto_plugin_scarf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-26 18:23:43.000000 resoto-plugin-scarf-3.5.0/resoto_plugin_scarf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:43.000000 resoto-plugin-scarf-3.5.0/resoto_plugin_scarf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-26 18:23:43.000000 resoto-plugin-scarf-3.5.0/resoto_plugin_scarf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:43.000000 resoto-plugin-scarf-3.5.0/resoto_plugin_scarf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 18:23:43.000000 resoto-plugin-scarf-3.5.0/resoto_plugin_scarf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 18:23:43.000000 resoto-plugin-scarf-3.5.0/resoto_plugin_scarf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:23:43.392379 resoto-plugin-scarf-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-26 18:21:40.000000 resoto-plugin-scarf-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:43.392379 resoto-plugin-scarf-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-26 18:21:40.000000 resoto-plugin-scarf-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:35.408630 resoto-plugin-scarf-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:52:52.000000 resoto-plugin-scarf-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-02 14:55:35.408630 resoto-plugin-scarf-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-02 14:52:52.000000 resoto-plugin-scarf-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-02 14:52:52.000000 resoto-plugin-scarf-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:35.404631 resoto-plugin-scarf-3.5.1/resoto_plugin_scarf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-02 14:52:52.000000 resoto-plugin-scarf-3.5.1/resoto_plugin_scarf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-02 14:52:52.000000 resoto-plugin-scarf-3.5.1/resoto_plugin_scarf/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-02 14:52:52.000000 resoto-plugin-scarf-3.5.1/resoto_plugin_scarf/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-02 14:52:52.000000 resoto-plugin-scarf-3.5.1/resoto_plugin_scarf/scarf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:35.408630 resoto-plugin-scarf-3.5.1/resoto_plugin_scarf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-02 14:55:35.000000 resoto-plugin-scarf-3.5.1/resoto_plugin_scarf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-02 14:55:35.000000 resoto-plugin-scarf-3.5.1/resoto_plugin_scarf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:55:35.000000 resoto-plugin-scarf-3.5.1/resoto_plugin_scarf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-02 14:55:35.000000 resoto-plugin-scarf-3.5.1/resoto_plugin_scarf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:54:00.000000 resoto-plugin-scarf-3.5.1/resoto_plugin_scarf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 14:55:35.000000 resoto-plugin-scarf-3.5.1/resoto_plugin_scarf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 14:55:35.000000 resoto-plugin-scarf-3.5.1/resoto_plugin_scarf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:55:35.408630 resoto-plugin-scarf-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:35.408630 resoto-plugin-scarf-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-02 14:52:52.000000 resoto-plugin-scarf-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-scarf-3.5.0/PKG-INFO` & `resoto-plugin-scarf-3.5.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-scarf
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Scarf Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/scarf
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/scarf
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
 
 # Resoto 💜 Scarf
 Scarf Collector Plugin for Resoto
 
 This collector plugin is used to collect data from Scarf. It is used internally at Some Engineering to create metrics about image downloads.
```

### Comparing `resoto-plugin-scarf-3.5.0/README.md` & `resoto-plugin-scarf-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.5.0/resoto_plugin_scarf/__init__.py` & `resoto-plugin-scarf-3.5.1/resoto_plugin_scarf/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.5.0/resoto_plugin_scarf/resources.py` & `resoto-plugin-scarf-3.5.1/resoto_plugin_scarf/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.5.0/resoto_plugin_scarf/scarf.py` & `resoto-plugin-scarf-3.5.1/resoto_plugin_scarf/scarf.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.5.0/resoto_plugin_scarf.egg-info/PKG-INFO` & `resoto-plugin-scarf-3.5.1/resoto_plugin_scarf.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-scarf
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Scarf Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/scarf
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/scarf
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
 
 # Resoto 💜 Scarf
 Scarf Collector Plugin for Resoto
 
 This collector plugin is used to collect data from Scarf. It is used internally at Some Engineering to create metrics about image downloads.
```

