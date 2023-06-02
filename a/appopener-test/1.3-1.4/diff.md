# Comparing `tmp/appopener_test-1.3.tar.gz` & `tmp/appopener_test-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appopener_test-1.3.tar", last modified: Fri Jun  2 15:37:52 2023, max compression
+gzip compressed data, was "appopener_test-1.4.tar", last modified: Fri Jun  2 15:57:21 2023, max compression
```

## Comparing `appopener_test-1.3.tar` & `appopener_test-1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 15:37:52.117653 appopener_test-1.3/
--rw-rw-rw-   0        0        0     3850 2023-06-02 15:37:52.117653 appopener_test-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 15:37:52.101836 appopener_test-1.3/appopener_test/
--rw-rw-rw-   0        0        0      416 2023-06-02 14:58:04.000000 appopener_test-1.3/appopener_test/__init__.py
--rw-rw-rw-   0        0        0       62 2023-06-02 14:32:02.000000 appopener_test-1.3/appopener_test/__main__.py
--rw-rw-rw-   0        0        0     2704 2023-06-02 15:37:43.000000 appopener_test-1.3/appopener_test/check.py
--rw-rw-rw-   0        0        0      827 2023-06-02 14:32:02.000000 appopener_test-1.3/appopener_test/commands.py
--rw-rw-rw-   0        0        0     1294 2023-06-02 15:36:30.000000 appopener_test-1.3/appopener_test/old_style.py
--rw-rw-rw-   0        0        0     7421 2023-06-02 14:41:38.000000 appopener_test-1.3/appopener_test/update_list.py
-drwxrwxrwx   0        0        0        0 2023-06-02 15:37:52.117653 appopener_test-1.3/appopener_test.egg-info/
--rw-rw-rw-   0        0        0     3850 2023-06-02 15:37:51.000000 appopener_test-1.3/appopener_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-06-02 15:37:51.000000 appopener_test-1.3/appopener_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 15:37:51.000000 appopener_test-1.3/appopener_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 15:37:51.000000 appopener_test-1.3/appopener_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-02 15:37:51.000000 appopener_test-1.3/appopener_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 15:37:52.117653 appopener_test-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-06-02 14:35:00.000000 appopener_test-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:57:21.347142 appopener_test-1.4/
+-rw-rw-rw-   0        0        0     3850 2023-06-02 15:57:21.342309 appopener_test-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 15:57:21.313181 appopener_test-1.4/appopener_test/
+-rw-rw-rw-   0        0        0      911 2023-06-02 15:56:39.000000 appopener_test-1.4/appopener_test/__init__.py
+-rw-rw-rw-   0        0        0       62 2023-06-02 14:32:02.000000 appopener_test-1.4/appopener_test/__main__.py
+-rw-rw-rw-   0        0        0     2704 2023-06-02 15:37:43.000000 appopener_test-1.4/appopener_test/check.py
+-rw-rw-rw-   0        0        0      827 2023-06-02 14:32:02.000000 appopener_test-1.4/appopener_test/commands.py
+-rw-rw-rw-   0        0        0     1294 2023-06-02 15:36:30.000000 appopener_test-1.4/appopener_test/old_style.py
+-rw-rw-rw-   0        0        0     7421 2023-06-02 14:41:38.000000 appopener_test-1.4/appopener_test/update_list.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:57:21.334057 appopener_test-1.4/appopener_test.egg-info/
+-rw-rw-rw-   0        0        0     3850 2023-06-02 15:57:21.000000 appopener_test-1.4/appopener_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-06-02 15:57:21.000000 appopener_test-1.4/appopener_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 15:57:21.000000 appopener_test-1.4/appopener_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 15:57:21.000000 appopener_test-1.4/appopener_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-02 15:57:21.000000 appopener_test-1.4/appopener_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 15:57:21.347142 appopener_test-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2023-06-02 14:35:00.000000 appopener_test-1.4/setup.py
```

### Comparing `appopener_test-1.3/PKG-INFO` & `appopener_test-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appopener_test
-Version: 1.3
+Version: 1.4
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `appopener_test-1.3/appopener_test/check.py` & `appopener_test-1.4/appopener_test/check.py`

 * *Files identical despite different names*

### Comparing `appopener_test-1.3/appopener_test/commands.py` & `appopener_test-1.4/appopener_test/commands.py`

 * *Files identical despite different names*

### Comparing `appopener_test-1.3/appopener_test/old_style.py` & `appopener_test-1.4/appopener_test/old_style.py`

 * *Files identical despite different names*

### Comparing `appopener_test-1.3/appopener_test/update_list.py` & `appopener_test-1.4/appopener_test/update_list.py`

 * *Files identical despite different names*

### Comparing `appopener_test-1.3/appopener_test.egg-info/PKG-INFO` & `appopener_test-1.4/appopener_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appopener-test
-Version: 1.3
+Version: 1.4
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `appopener_test-1.3/setup.py` & `appopener_test-1.4/setup.py`

 * *Files identical despite different names*

