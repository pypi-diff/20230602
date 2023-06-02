# Comparing `tmp/roxbot-0.2.0.tar.gz` & `tmp/roxbot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roxbot-0.2.0.tar", last modified: Fri Jun  2 11:19:13 2023, max compression
+gzip compressed data, was "roxbot-0.3.0.tar", last modified: Fri Jun  2 16:42:03 2023, max compression
```

## Comparing `roxbot-0.2.0.tar` & `roxbot-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:19:13.414440 roxbot-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-06-02 11:19:04.000000 roxbot-0.2.0/LICENCE
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-02 11:19:13.414440 roxbot-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-06-02 11:19:04.000000 roxbot-0.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-02 11:19:13.414440 roxbot-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-02 11:19:04.000000 roxbot-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:19:13.409441 roxbot-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:19:13.411440 roxbot-0.2.0/src/roxbot/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-02 11:19:04.000000 roxbot-0.2.0/src/roxbot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-02 11:19:04.000000 roxbot-0.2.0/src/roxbot/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5874 2023-06-02 11:19:04.000000 roxbot-0.2.0/src/roxbot/gps.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-06-02 11:19:04.000000 roxbot-0.2.0/src/roxbot/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     5020 2023-06-02 11:19:04.000000 roxbot-0.2.0/src/roxbot/vectors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:19:13.413441 roxbot-0.2.0/src/roxbot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-02 11:19:13.000000 roxbot-0.2.0/src/roxbot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      431 2023-06-02 11:19:13.000000 roxbot-0.2.0/src/roxbot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 11:19:13.000000 roxbot-0.2.0/src/roxbot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-02 11:19:13.000000 roxbot-0.2.0/src/roxbot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-02 11:19:13.000000 roxbot-0.2.0/src/roxbot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-02 11:19:13.000000 roxbot-0.2.0/src/roxbot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:19:13.414440 roxbot-0.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-02 11:19:04.000000 roxbot-0.2.0/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2780 2023-06-02 11:19:04.000000 roxbot-0.2.0/tests/test_gps.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-02 11:19:04.000000 roxbot-0.2.0/tests/test_interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2781 2023-06-02 11:19:04.000000 roxbot-0.2.0/tests/test_vectors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:42:03.532494 roxbot-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-06-02 16:41:54.000000 roxbot-0.3.0/LICENCE
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-02 16:42:03.533494 roxbot-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-06-02 16:41:54.000000 roxbot-0.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-02 16:42:03.533494 roxbot-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-02 16:41:54.000000 roxbot-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:42:03.528494 roxbot-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:42:03.530494 roxbot-0.3.0/src/roxbot/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-02 16:41:54.000000 roxbot-0.3.0/src/roxbot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-02 16:41:54.000000 roxbot-0.3.0/src/roxbot/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5874 2023-06-02 16:41:54.000000 roxbot-0.3.0/src/roxbot/gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-06-02 16:41:54.000000 roxbot-0.3.0/src/roxbot/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4913 2023-06-02 16:41:54.000000 roxbot-0.3.0/src/roxbot/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-06-02 16:41:54.000000 roxbot-0.3.0/src/roxbot/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5020 2023-06-02 16:41:54.000000 roxbot-0.3.0/src/roxbot/vectors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:42:03.531494 roxbot-0.3.0/src/roxbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-02 16:42:03.000000 roxbot-0.3.0/src/roxbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      513 2023-06-02 16:42:03.000000 roxbot-0.3.0/src/roxbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 16:42:03.000000 roxbot-0.3.0/src/roxbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-02 16:42:03.000000 roxbot-0.3.0/src/roxbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-02 16:42:03.000000 roxbot-0.3.0/src/roxbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-02 16:42:03.000000 roxbot-0.3.0/src/roxbot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:42:03.532494 roxbot-0.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-02 16:41:54.000000 roxbot-0.3.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2780 2023-06-02 16:41:54.000000 roxbot-0.3.0/tests/test_gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-02 16:41:54.000000 roxbot-0.3.0/tests/test_interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2070 2023-06-02 16:41:54.000000 roxbot-0.3.0/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2023-06-02 16:41:54.000000 roxbot-0.3.0/tests/test_trike.py
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2023-06-02 16:41:54.000000 roxbot-0.3.0/tests/test_vectors.py
```

### Comparing `roxbot-0.2.0/LICENCE` & `roxbot-0.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `roxbot-0.2.0/README.md` & `roxbot-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `roxbot-0.2.0/setup.py` & `roxbot-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.2.0/src/roxbot/gps.py` & `roxbot-0.3.0/src/roxbot/gps.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.2.0/src/roxbot/vectors.py` & `roxbot-0.3.0/src/roxbot/vectors.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.2.0/tests/test_gps.py` & `roxbot-0.3.0/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.2.0/tests/test_vectors.py` & `roxbot-0.3.0/tests/test_vectors.py`

 * *Files identical despite different names*

