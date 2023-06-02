# Comparing `tmp/resoto-plugin-digitalocean-k8s-3.5.0.tar.gz` & `tmp/resoto-plugin-digitalocean-k8s-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-digitalocean-k8s-3.5.0.tar", last modified: Fri May 26 18:23:45 2023, max compression
+gzip compressed data, was "resoto-plugin-digitalocean-k8s-3.5.1.tar", last modified: Fri Jun  2 14:56:51 2023, max compression
```

## Comparing `resoto-plugin-digitalocean-k8s-3.5.0.tar` & `resoto-plugin-digitalocean-k8s-3.5.1.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:45.668591 resoto-plugin-digitalocean-k8s-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-26 18:23:45.668591 resoto-plugin-digitalocean-k8s-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:45.664591 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:45.668591 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-26 18:23:45.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-26 18:23:45.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:45.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 18:23:45.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:45.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:23:45.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-26 18:23:45.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:23:45.668591 resoto-plugin-digitalocean-k8s-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:45.668591 resoto-plugin-digitalocean-k8s-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/test/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:51.853901 resoto-plugin-digitalocean-k8s-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:53:11.000000 resoto-plugin-digitalocean-k8s-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-02 14:56:51.853901 resoto-plugin-digitalocean-k8s-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-02 14:53:11.000000 resoto-plugin-digitalocean-k8s-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-02 14:53:11.000000 resoto-plugin-digitalocean-k8s-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:51.853901 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-02 14:53:11.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:51.853901 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-02 14:56:51.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-02 14:56:51.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:56:51.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-02 14:56:51.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:54:21.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 14:56:51.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-02 14:56:51.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:56:51.857901 resoto-plugin-digitalocean-k8s-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:51.853901 resoto-plugin-digitalocean-k8s-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:11.000000 resoto-plugin-digitalocean-k8s-3.5.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-02 14:53:11.000000 resoto-plugin-digitalocean-k8s-3.5.1/test/test_collector.py
```

### Comparing `resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s/__init__.py` & `resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-k8s-3.5.0/test/test_collector.py` & `resoto-plugin-digitalocean-k8s-3.5.1/test/test_collector.py`

 * *Files identical despite different names*

