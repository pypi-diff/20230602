# Comparing `tmp/quranallsbuforuni-0.0.1.tar.gz` & `tmp/quranallsbuforuni-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quranallsbuforuni-0.0.1.tar", last modified: Thu Jun  1 22:45:06 2023, max compression
+gzip compressed data, was "quranallsbuforuni-0.0.2.tar", last modified: Thu Jun  1 23:14:56 2023, max compression
```

## Comparing `quranallsbuforuni-0.0.1.tar` & `quranallsbuforuni-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 22:45:06.003471 quranallsbuforuni-0.0.1/
--rw-rw-rw-   0        0        0      315 2023-06-01 22:45:06.003471 quranallsbuforuni-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-01 22:45:05.991469 quranallsbuforuni-0.0.1/quranallsbuforuni/
--rw-rw-rw-   0        0        0       50 2023-06-01 22:44:51.000000 quranallsbuforuni-0.0.1/quranallsbuforuni/__init__.py
--rw-rw-rw-   0        0        0   743998 2023-06-01 22:37:36.000000 quranallsbuforuni-0.0.1/quranallsbuforuni/module1.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:45:06.001471 quranallsbuforuni-0.0.1/quranallsbuforuni.egg-info/
--rw-rw-rw-   0        0        0      315 2023-06-01 22:45:05.000000 quranallsbuforuni-0.0.1/quranallsbuforuni.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-01 22:45:05.000000 quranallsbuforuni-0.0.1/quranallsbuforuni.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 22:45:05.000000 quranallsbuforuni-0.0.1/quranallsbuforuni.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-01 22:45:05.000000 quranallsbuforuni-0.0.1/quranallsbuforuni.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 22:45:06.003471 quranallsbuforuni-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      528 2023-06-01 22:44:31.000000 quranallsbuforuni-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 23:14:56.729354 quranallsbuforuni-0.0.2/
+-rw-rw-rw-   0        0        0      315 2023-06-01 23:14:56.729354 quranallsbuforuni-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-01 23:14:56.717344 quranallsbuforuni-0.0.2/quranallsbuforuni/
+-rw-rw-rw-   0        0        0       99 2023-06-01 23:14:41.000000 quranallsbuforuni-0.0.2/quranallsbuforuni/__init__.py
+-rw-rw-rw-   0        0        0   743998 2023-06-01 22:37:36.000000 quranallsbuforuni-0.0.2/quranallsbuforuni/module1.py
+-rw-rw-rw-   0        0        0   744515 2023-06-01 23:14:30.000000 quranallsbuforuni-0.0.2/quranallsbuforuni/module2.py
+drwxrwxrwx   0        0        0        0 2023-06-01 23:14:56.727361 quranallsbuforuni-0.0.2/quranallsbuforuni.egg-info/
+-rw-rw-rw-   0        0        0      315 2023-06-01 23:14:56.000000 quranallsbuforuni-0.0.2/quranallsbuforuni.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-06-01 23:14:56.000000 quranallsbuforuni-0.0.2/quranallsbuforuni.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 23:14:56.000000 quranallsbuforuni-0.0.2/quranallsbuforuni.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-01 23:14:56.000000 quranallsbuforuni-0.0.2/quranallsbuforuni.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 23:14:56.729354 quranallsbuforuni-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      528 2023-06-01 23:14:46.000000 quranallsbuforuni-0.0.2/setup.py
```

### Comparing `quranallsbuforuni-0.0.1/quranallsbuforuni/module1.py` & `quranallsbuforuni-0.0.2/quranallsbuforuni/module1.py`

 * *Files identical despite different names*

### Comparing `quranallsbuforuni-0.0.1/setup.py` & `quranallsbuforuni-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Quran SBU All'
 LONG_DESCRIPTION = 'First Python Package'
 
 # Setting up
 setup(
     name="quranallsbuforuni",
     version=VERSION,
```

