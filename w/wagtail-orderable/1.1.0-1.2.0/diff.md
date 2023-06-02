# Comparing `tmp/wagtail-orderable-1.1.0.tar.gz` & `tmp/wagtail-orderable-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-orderable-1.1.0.tar", last modified: Sat Aug 27 12:18:51 2022, max compression
+gzip compressed data, was "wagtail-orderable-1.2.0.tar", last modified: Fri Jun  2 16:14:24 2023, max compression
```

## Comparing `wagtail-orderable-1.1.0.tar` & `wagtail-orderable-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 12:18:51.587241 wagtail-orderable-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-08-27 12:18:43.000000 wagtail-orderable-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-27 12:18:43.000000 wagtail-orderable-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-08-27 12:18:51.587241 wagtail-orderable-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3842 2022-08-27 12:18:43.000000 wagtail-orderable-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-27 12:18:51.587241 wagtail-orderable-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1898 2022-08-27 12:18:43.000000 wagtail-orderable-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 12:18:51.587241 wagtail-orderable-1.1.0/wagtail_orderable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-08-27 12:18:51.000000 wagtail-orderable-1.1.0/wagtail_orderable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-08-27 12:18:51.000000 wagtail-orderable-1.1.0/wagtail_orderable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 12:18:51.000000 wagtail-orderable-1.1.0/wagtail_orderable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-27 12:18:51.000000 wagtail-orderable-1.1.0/wagtail_orderable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-27 12:18:51.000000 wagtail-orderable-1.1.0/wagtail_orderable.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 12:18:51.587241 wagtail-orderable-1.1.0/wagtailorderable/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-27 12:18:43.000000 wagtail-orderable-1.1.0/wagtailorderable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 12:18:51.587241 wagtail-orderable-1.1.0/wagtailorderable/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-08-27 12:18:50.000000 wagtail-orderable-1.1.0/wagtailorderable/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 12:18:51.587241 wagtail-orderable-1.1.0/wagtailorderable/modeladmin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-27 12:18:43.000000 wagtail-orderable-1.1.0/wagtailorderable/modeladmin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12931 2022-08-27 12:18:43.000000 wagtail-orderable-1.1.0/wagtailorderable/modeladmin/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-08-27 12:18:43.000000 wagtail-orderable-1.1.0/wagtailorderable/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-08-27 12:18:43.000000 wagtail-orderable-1.1.0/wagtailorderable/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 12:18:51.583241 wagtail-orderable-1.1.0/wagtailorderable/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 12:18:51.583241 wagtail-orderable-1.1.0/wagtailorderable/static/wagtailorderable/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 12:18:51.583241 wagtail-orderable-1.1.0/wagtailorderable/static/wagtailorderable/modeladmin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 12:18:51.587241 wagtail-orderable-1.1.0/wagtailorderable/static/wagtailorderable/modeladmin/css/
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-08-27 12:18:43.000000 wagtail-orderable-1.1.0/wagtailorderable/static/wagtailorderable/modeladmin/css/orderablemixin.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 12:18:51.587241 wagtail-orderable-1.1.0/wagtailorderable/static/wagtailorderable/modeladmin/js/
--rw-r--r--   0 runner    (1001) docker     (121)     3300 2022-08-27 12:18:43.000000 wagtail-orderable-1.1.0/wagtailorderable/static/wagtailorderable/modeladmin/js/orderablemixin.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:14:24.582219 wagtail-orderable-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-02 16:14:13.000000 wagtail-orderable-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-02 16:14:13.000000 wagtail-orderable-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-02 16:14:24.582219 wagtail-orderable-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-02 16:14:13.000000 wagtail-orderable-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-02 16:14:24.582219 wagtail-orderable-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-02 16:14:13.000000 wagtail-orderable-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:14:24.578219 wagtail-orderable-1.2.0/wagtail_orderable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-02 16:14:24.000000 wagtail-orderable-1.2.0/wagtail_orderable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-02 16:14:24.000000 wagtail-orderable-1.2.0/wagtail_orderable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:14:24.000000 wagtail-orderable-1.2.0/wagtail_orderable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 16:14:24.000000 wagtail-orderable-1.2.0/wagtail_orderable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 16:14:24.000000 wagtail-orderable-1.2.0/wagtail_orderable.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:14:24.582219 wagtail-orderable-1.2.0/wagtailorderable/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 16:14:13.000000 wagtail-orderable-1.2.0/wagtailorderable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:14:24.582219 wagtail-orderable-1.2.0/wagtailorderable/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-02 16:14:23.000000 wagtail-orderable-1.2.0/wagtailorderable/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:14:24.582219 wagtail-orderable-1.2.0/wagtailorderable/modeladmin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:14:13.000000 wagtail-orderable-1.2.0/wagtailorderable/modeladmin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-06-02 16:14:13.000000 wagtail-orderable-1.2.0/wagtailorderable/modeladmin/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-02 16:14:13.000000 wagtail-orderable-1.2.0/wagtailorderable/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-02 16:14:13.000000 wagtail-orderable-1.2.0/wagtailorderable/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:14:24.578219 wagtail-orderable-1.2.0/wagtailorderable/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:14:24.578219 wagtail-orderable-1.2.0/wagtailorderable/static/wagtailorderable/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:14:24.578219 wagtail-orderable-1.2.0/wagtailorderable/static/wagtailorderable/modeladmin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:14:24.582219 wagtail-orderable-1.2.0/wagtailorderable/static/wagtailorderable/modeladmin/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-02 16:14:13.000000 wagtail-orderable-1.2.0/wagtailorderable/static/wagtailorderable/modeladmin/css/orderablemixin.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:14:24.582219 wagtail-orderable-1.2.0/wagtailorderable/static/wagtailorderable/modeladmin/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-02 16:14:13.000000 wagtail-orderable-1.2.0/wagtailorderable/static/wagtailorderable/modeladmin/js/orderablemixin.js
```

### Comparing `wagtail-orderable-1.1.0/LICENSE.txt` & `wagtail-orderable-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail-orderable-1.1.0/PKG-INFO` & `wagtail-orderable-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: wagtail-orderable
-Version: 1.1.0
+Version: 1.2.0
 Summary: Orderable support for Wagtail
 Home-page: https://github.com/elton2048/wagtail-orderable
 Author: Elton Lee & Andy Babic
 Author-email: elton2048@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: zlib/libpng License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 License-File: LICENSE.txt
 
 Provides drag-and-drop support ordering support to the ModelAdmin listing view.
```

### Comparing `wagtail-orderable-1.1.0/README.md` & `wagtail-orderable-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -94,14 +94,21 @@
 ```shell
 python manage.py collectstatic
 ```
 in your project.
 
 ### Change Log
 
+1.2.0
+---
+- Updated documentation for wagtail 4.0 support
+- Updated workflow action versions
+- Allow wagtail v4.1+ (drops ability to use on a wagtail site version earlier than v4.1)
+- Allow Wagtail v5 and Django v4.2
+
 1.1.0
 ---
 - Extending `Orderable` is no more mandatory if you want to use your own order field (#27)
 - Add `Orderable.get_sort_order_max()` to get the max "order" when instance is being created (#27)
 - Fix keeping current filters when sorting was reset (#27)
 - Fix class names (`get_extra_class_names_for_field_col` parameters were inverted) (#27)
 - Fix CSS which had SCSS syntax (#27)
```

### Comparing `wagtail-orderable-1.1.0/setup.py` & `wagtail-orderable-1.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,35 +3,36 @@
 import subprocess
 
 from wagtailorderable import __version__
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 INSTALL_REQUIRES = [
-    "wagtail>=2.15",
+    "wagtail>=4.1",
 ]
 
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     "Framework :: Django",
     "Framework :: Django :: 3.2",
-    "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     'License :: OSI Approved :: zlib/libpng License',
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Framework :: Wagtail",
-    "Framework :: Wagtail :: 2",
-    "Framework :: Wagtail :: 3",
+    "Framework :: Wagtail :: 4",
+    "Framework :: Wagtail :: 5",
 ]
 
 class VerifyVersionCommand(install):
     """Custom command to verify that the git tag matches our version"""
     description = 'verify that the git tag matches our version'
 
     def run(self):
```

### Comparing `wagtail-orderable-1.1.0/wagtail_orderable.egg-info/PKG-INFO` & `wagtail-orderable-1.2.0/wagtail_orderable.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: wagtail-orderable
-Version: 1.1.0
+Version: 1.2.0
 Summary: Orderable support for Wagtail
 Home-page: https://github.com/elton2048/wagtail-orderable
 Author: Elton Lee & Andy Babic
 Author-email: elton2048@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: zlib/libpng License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 License-File: LICENSE.txt
 
 Provides drag-and-drop support ordering support to the ModelAdmin listing view.
```

### Comparing `wagtail-orderable-1.1.0/wagtail_orderable.egg-info/SOURCES.txt` & `wagtail-orderable-1.2.0/wagtail_orderable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-orderable-1.1.0/wagtailorderable/modeladmin/mixins.py` & `wagtail-orderable-1.2.0/wagtailorderable/modeladmin/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail-orderable-1.1.0/wagtailorderable/models.py` & `wagtail-orderable-1.2.0/wagtailorderable/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-orderable-1.1.0/wagtailorderable/signals.py` & `wagtail-orderable-1.2.0/wagtailorderable/signals.py`

 * *Files identical despite different names*

### Comparing `wagtail-orderable-1.1.0/wagtailorderable/static/wagtailorderable/modeladmin/js/orderablemixin.js` & `wagtail-orderable-1.2.0/wagtailorderable/static/wagtailorderable/modeladmin/js/orderablemixin.js`

 * *Files identical despite different names*

