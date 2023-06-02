# Comparing `tmp/appopener_test-1.1.tar.gz` & `tmp/appopener_test-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appopener_test-1.1.tar", last modified: Fri Jun  2 15:11:22 2023, max compression
+gzip compressed data, was "appopener_test-1.2.tar", last modified: Fri Jun  2 15:28:39 2023, max compression
```

## Comparing `appopener_test-1.1.tar` & `appopener_test-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 15:11:22.230567 appopener_test-1.1/
--rw-rw-rw-   0        0        0     3850 2023-06-02 15:11:22.229499 appopener_test-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 15:11:22.209890 appopener_test-1.1/appopener_test/
--rw-rw-rw-   0        0        0      416 2023-06-02 14:58:04.000000 appopener_test-1.1/appopener_test/__init__.py
--rw-rw-rw-   0        0        0       62 2023-06-02 14:32:02.000000 appopener_test-1.1/appopener_test/__main__.py
--rw-rw-rw-   0        0        0     2704 2023-06-02 15:10:34.000000 appopener_test-1.1/appopener_test/check.py
--rw-rw-rw-   0        0        0      827 2023-06-02 14:32:02.000000 appopener_test-1.1/appopener_test/commands.py
--rw-rw-rw-   0        0        0      534 2023-06-02 15:08:42.000000 appopener_test-1.1/appopener_test/old_style.py
--rw-rw-rw-   0        0        0     7421 2023-06-02 14:41:38.000000 appopener_test-1.1/appopener_test/update_list.py
-drwxrwxrwx   0        0        0        0 2023-06-02 15:11:22.227049 appopener_test-1.1/appopener_test.egg-info/
--rw-rw-rw-   0        0        0     3850 2023-06-02 15:11:22.000000 appopener_test-1.1/appopener_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-06-02 15:11:22.000000 appopener_test-1.1/appopener_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 15:11:22.000000 appopener_test-1.1/appopener_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 15:11:22.000000 appopener_test-1.1/appopener_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-02 15:11:22.000000 appopener_test-1.1/appopener_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 15:11:22.230567 appopener_test-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-06-02 14:35:00.000000 appopener_test-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:28:39.617519 appopener_test-1.2/
+-rw-rw-rw-   0        0        0     3850 2023-06-02 15:28:39.611445 appopener_test-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 15:28:39.588196 appopener_test-1.2/appopener_test/
+-rw-rw-rw-   0        0        0      416 2023-06-02 14:58:04.000000 appopener_test-1.2/appopener_test/__init__.py
+-rw-rw-rw-   0        0        0       62 2023-06-02 14:32:02.000000 appopener_test-1.2/appopener_test/__main__.py
+-rw-rw-rw-   0        0        0     2704 2023-06-02 15:28:28.000000 appopener_test-1.2/appopener_test/check.py
+-rw-rw-rw-   0        0        0      827 2023-06-02 14:32:02.000000 appopener_test-1.2/appopener_test/commands.py
+-rw-rw-rw-   0        0        0     1114 2023-06-02 15:27:37.000000 appopener_test-1.2/appopener_test/old_style.py
+-rw-rw-rw-   0        0        0     7421 2023-06-02 14:41:38.000000 appopener_test-1.2/appopener_test/update_list.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:28:39.611445 appopener_test-1.2/appopener_test.egg-info/
+-rw-rw-rw-   0        0        0     3850 2023-06-02 15:28:39.000000 appopener_test-1.2/appopener_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-06-02 15:28:39.000000 appopener_test-1.2/appopener_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 15:28:39.000000 appopener_test-1.2/appopener_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 15:28:39.000000 appopener_test-1.2/appopener_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-02 15:28:39.000000 appopener_test-1.2/appopener_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 15:28:39.617519 appopener_test-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2023-06-02 14:35:00.000000 appopener_test-1.2/setup.py
```

### Comparing `appopener_test-1.1/PKG-INFO` & `appopener_test-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appopener_test
-Version: 1.1
+Version: 1.2
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `appopener_test-1.1/appopener_test/check.py` & `appopener_test-1.2/appopener_test/check.py`

 * *Files identical despite different names*

### Comparing `appopener_test-1.1/appopener_test/commands.py` & `appopener_test-1.2/appopener_test/commands.py`

 * *Files identical despite different names*

### Comparing `appopener_test-1.1/appopener_test/update_list.py` & `appopener_test-1.2/appopener_test/update_list.py`

 * *Files identical despite different names*

### Comparing `appopener_test-1.1/appopener_test.egg-info/PKG-INFO` & `appopener_test-1.2/appopener_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appopener-test
-Version: 1.1
+Version: 1.2
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `appopener_test-1.1/setup.py` & `appopener_test-1.2/setup.py`

 * *Files identical despite different names*

