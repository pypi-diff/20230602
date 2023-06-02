# Comparing `tmp/resoto-plugin-onprem-3.5.0.tar.gz` & `tmp/resoto-plugin-onprem-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-onprem-3.5.0.tar", last modified: Fri May 26 18:26:37 2023, max compression
+gzip compressed data, was "resoto-plugin-onprem-3.5.1.tar", last modified: Fri Jun  2 14:48:44 2023, max compression
```

## Comparing `resoto-plugin-onprem-3.5.0.tar` & `resoto-plugin-onprem-3.5.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:37.762365 resoto-plugin-onprem-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-26 18:26:37.762365 resoto-plugin-onprem-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:37.758365 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:37.758365 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-26 18:26:37.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-26 18:26:37.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:26:37.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 18:26:37.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:26:37.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 18:26:37.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 18:26:37.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:26:37.762365 resoto-plugin-onprem-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:37.758365 resoto-plugin-onprem-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:48:44.068211 resoto-plugin-onprem-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-02 14:48:44.068211 resoto-plugin-onprem-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:48:44.068211 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:48:44.068211 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-02 14:48:44.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-02 14:48:44.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:48:44.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 14:48:44.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:47:08.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 14:48:44.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 14:48:44.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:48:44.068211 resoto-plugin-onprem-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:48:44.068211 resoto-plugin-onprem-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/__init__.py` & `resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/config.py` & `resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/resources.py` & `resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/ssh.py` & `resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/ssh.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.5.0/test/test_config.py` & `resoto-plugin-onprem-3.5.1/test/test_config.py`

 * *Files identical despite different names*

