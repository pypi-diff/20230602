# Comparing `tmp/chater-1.0.1.tar.gz` & `tmp/chater-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chater-1.0.1.tar", last modified: Fri Jun  2 16:03:45 2023, max compression
+gzip compressed data, was "chater-1.0.2.tar", last modified: Fri Jun  2 16:28:37 2023, max compression
```

## Comparing `chater-1.0.1.tar` & `chater-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:03:45.028993 chater-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-02 16:03:35.000000 chater-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-02 16:03:45.028993 chater-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-02 16:03:35.000000 chater-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:03:45.028993 chater-1.0.1/chater/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-02 16:03:35.000000 chater-1.0.1/chater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:03:45.028993 chater-1.0.1/chater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-02 16:03:45.000000 chater-1.0.1/chater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-02 16:03:45.000000 chater-1.0.1/chater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:03:45.000000 chater-1.0.1/chater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 16:03:45.000000 chater-1.0.1/chater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 16:03:45.000000 chater-1.0.1/chater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:03:45.028993 chater-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-02 16:03:35.000000 chater-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:28:37.395574 chater-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-02 16:28:27.000000 chater-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-02 16:28:37.395574 chater-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-02 16:28:27.000000 chater-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:28:37.391574 chater-1.0.2/chater/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-02 16:28:27.000000 chater-1.0.2/chater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:28:37.395574 chater-1.0.2/chater/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:28:37.395574 chater-1.0.2/chater/api/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/abstract/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/abstract/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/stream_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-02 16:28:27.000000 chater-1.0.2/chater/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:28:37.391574 chater-1.0.2/chater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-02 16:28:37.000000 chater-1.0.2/chater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-02 16:28:37.000000 chater-1.0.2/chater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:28:37.000000 chater-1.0.2/chater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 16:28:37.000000 chater-1.0.2/chater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 16:28:37.000000 chater-1.0.2/chater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:28:37.395574 chater-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-02 16:28:27.000000 chater-1.0.2/setup.py
```

### Comparing `chater-1.0.1/LICENSE` & `chater-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chater-1.0.1/README.md` & `chater-1.0.2/README.md`

 * *Files identical despite different names*

