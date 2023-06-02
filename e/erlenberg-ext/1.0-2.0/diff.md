# Comparing `tmp/erlenberg_ext-1.0.tar.gz` & `tmp/erlenberg_ext-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlenberg_ext-1.0.tar", last modified: Fri Jun  2 10:27:37 2023, max compression
+gzip compressed data, was "erlenberg_ext-2.0.tar", last modified: Fri Jun  2 12:20:42 2023, max compression
```

## Comparing `erlenberg_ext-1.0.tar` & `erlenberg_ext-2.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 10:27:37.380166 erlenberg_ext-1.0/
--rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)     1094 2022-12-10 23:42:16.000000 erlenberg_ext-1.0/LICENSE
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)      935 2023-06-02 10:27:37.381166 erlenberg_ext-1.0/PKG-INFO
--rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)      558 2023-06-02 09:37:20.000000 erlenberg_ext-1.0/README.md
-drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 10:27:37.380166 erlenberg_ext-1.0/erlenberg_ext/
--rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)       33 2023-06-02 09:19:40.000000 erlenberg_ext-1.0/erlenberg_ext/__init__.py
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)     1397 2023-06-02 09:18:42.000000 erlenberg_ext-1.0/erlenberg_ext/simpleCrypt.py
-drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 10:27:37.380166 erlenberg_ext-1.0/erlenberg_ext.egg-info/
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)      935 2023-06-02 10:27:37.000000 erlenberg_ext-1.0/erlenberg_ext.egg-info/PKG-INFO
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)      281 2023-06-02 10:27:37.000000 erlenberg_ext-1.0/erlenberg_ext.egg-info/SOURCES.txt
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)        1 2023-06-02 10:27:37.000000 erlenberg_ext-1.0/erlenberg_ext.egg-info/dependency_links.txt
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)       13 2023-06-02 10:27:37.000000 erlenberg_ext-1.0/erlenberg_ext.egg-info/requires.txt
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)       14 2023-06-02 10:27:37.000000 erlenberg_ext-1.0/erlenberg_ext.egg-info/top_level.txt
--rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)      104 2022-12-10 21:33:18.000000 erlenberg_ext-1.0/pyproject.toml
--rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)      499 2023-06-02 10:27:37.381166 erlenberg_ext-1.0/setup.cfg
+drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 12:20:42.247770 erlenberg_ext-2.0/
+-rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)     1094 2022-12-10 23:42:16.000000 erlenberg_ext-2.0/LICENSE
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)      935 2023-06-02 12:20:42.247770 erlenberg_ext-2.0/PKG-INFO
+-rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)      558 2023-06-02 09:37:20.000000 erlenberg_ext-2.0/README.md
+drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 12:20:42.246770 erlenberg_ext-2.0/erlenberg_ext/
+-rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)       33 2023-06-02 09:19:40.000000 erlenberg_ext-2.0/erlenberg_ext/__init__.py
+drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 12:20:42.247770 erlenberg_ext-2.0/erlenberg_ext/cryptScriptGenerator/
+-rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)       51 2023-06-02 11:49:55.000000 erlenberg_ext-2.0/erlenberg_ext/cryptScriptGenerator/__init__.py
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)     3002 2023-04-21 13:05:05.000000 erlenberg_ext-2.0/erlenberg_ext/cryptScriptGenerator/__main__.py
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)     1397 2023-06-02 09:18:42.000000 erlenberg_ext-2.0/erlenberg_ext/simpleCrypt.py
+drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 12:20:42.247770 erlenberg_ext-2.0/erlenberg_ext.egg-info/
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)      935 2023-06-02 12:20:42.000000 erlenberg_ext-2.0/erlenberg_ext.egg-info/PKG-INFO
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)      415 2023-06-02 12:20:42.000000 erlenberg_ext-2.0/erlenberg_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)        1 2023-06-02 12:20:42.000000 erlenberg_ext-2.0/erlenberg_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)      104 2023-06-02 12:20:42.000000 erlenberg_ext-2.0/erlenberg_ext.egg-info/entry_points.txt
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)       13 2023-06-02 12:20:42.000000 erlenberg_ext-2.0/erlenberg_ext.egg-info/requires.txt
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)       14 2023-06-02 12:20:42.000000 erlenberg_ext-2.0/erlenberg_ext.egg-info/top_level.txt
+-rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)      104 2022-12-10 21:33:18.000000 erlenberg_ext-2.0/pyproject.toml
+-rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)      629 2023-06-02 12:20:42.248771 erlenberg_ext-2.0/setup.cfg
```

### Comparing `erlenberg_ext-1.0/LICENSE` & `erlenberg_ext-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erlenberg_ext-1.0/PKG-INFO` & `erlenberg_ext-2.0/erlenberg_ext.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: erlenberg_ext
-Version: 1.0
+Name: erlenberg-ext
+Version: 2.0
 Summary: Some personal librarys for python (extended)
 Author: Tizian Erlenberg
 Author-email: mail@erlenberg.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `erlenberg_ext-1.0/README.md` & `erlenberg_ext-2.0/README.md`

 * *Files identical despite different names*

### Comparing `erlenberg_ext-1.0/erlenberg_ext/simpleCrypt.py` & `erlenberg_ext-2.0/erlenberg_ext/simpleCrypt.py`

 * *Files identical despite different names*

### Comparing `erlenberg_ext-1.0/erlenberg_ext.egg-info/PKG-INFO` & `erlenberg_ext-2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: erlenberg-ext
-Version: 1.0
+Name: erlenberg_ext
+Version: 2.0
 Summary: Some personal librarys for python (extended)
 Author: Tizian Erlenberg
 Author-email: mail@erlenberg.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

