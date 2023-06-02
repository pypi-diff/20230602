# Comparing `tmp/cmdsave-1.0.1.tar.gz` & `tmp/cmdsave-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdsave-1.0.1.tar", last modified: Fri Jun  2 18:54:10 2023, max compression
+gzip compressed data, was "cmdsave-1.0.2.tar", last modified: Fri Jun  2 19:02:00 2023, max compression
```

## Comparing `cmdsave-1.0.1.tar` & `cmdsave-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 18:54:10.139725 cmdsave-1.0.1/
--rw-rw-rw-   0        0        0       54 2023-06-02 18:54:10.138729 cmdsave-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1741 2023-06-02 18:44:34.000000 cmdsave-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 18:54:10.131746 cmdsave-1.0.1/cmdsave/
--rw-rw-rw-   0        0        0     4419 2023-06-02 16:19:57.000000 cmdsave-1.0.1/cmdsave/cmdsave.py
-drwxrwxrwx   0        0        0        0 2023-06-02 18:54:10.137730 cmdsave-1.0.1/cmdsave.egg-info/
--rw-rw-rw-   0        0        0       54 2023-06-02 18:54:09.000000 cmdsave-1.0.1/cmdsave.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-02 18:54:10.000000 cmdsave-1.0.1/cmdsave.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 18:54:09.000000 cmdsave-1.0.1/cmdsave.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-02 18:54:09.000000 cmdsave-1.0.1/cmdsave.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-06-02 18:54:09.000000 cmdsave-1.0.1/cmdsave.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 18:54:09.000000 cmdsave-1.0.1/cmdsave.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 18:54:10.139725 cmdsave-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      369 2023-06-02 18:54:02.000000 cmdsave-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:02:00.502120 cmdsave-1.0.2/
+-rw-rw-rw-   0        0        0     1909 2023-06-02 19:02:00.502120 cmdsave-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1741 2023-06-02 18:44:34.000000 cmdsave-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 19:02:00.488156 cmdsave-1.0.2/cmdsave/
+-rw-rw-rw-   0        0        0     4419 2023-06-02 16:19:57.000000 cmdsave-1.0.2/cmdsave/cmdsave.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:02:00.501123 cmdsave-1.0.2/cmdsave.egg-info/
+-rw-rw-rw-   0        0        0     1909 2023-06-02 19:02:00.000000 cmdsave-1.0.2/cmdsave.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-02 19:02:00.000000 cmdsave-1.0.2/cmdsave.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 19:02:00.000000 cmdsave-1.0.2/cmdsave.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-02 19:02:00.000000 cmdsave-1.0.2/cmdsave.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2023-06-02 19:02:00.000000 cmdsave-1.0.2/cmdsave.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 19:02:00.000000 cmdsave-1.0.2/cmdsave.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 19:02:00.502120 cmdsave-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      606 2023-06-02 19:01:53.000000 cmdsave-1.0.2/setup.py
```

### Comparing `cmdsave-1.0.1/README.md` & `cmdsave-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cmdsave-1.0.1/cmdsave/cmdsave.py` & `cmdsave-1.0.2/cmdsave/cmdsave.py`

 * *Files identical despite different names*

