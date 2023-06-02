# Comparing `tmp/django-iubenda-web-0.0.7.tar.gz` & `tmp/django-iubenda-web-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-iubenda-web-0.0.7.tar", last modified: Fri Jun  2 13:55:08 2023, max compression
+gzip compressed data, was "django-iubenda-web-0.0.8.tar", last modified: Fri Jun  2 14:05:11 2023, max compression
```

## Comparing `django-iubenda-web-0.0.7.tar` & `django-iubenda-web-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:55:08.435339 django-iubenda-web-0.0.7/
--rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/LICENSE
--rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 13:55:08.435532 django-iubenda-web-0.0.7/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)       47 2023-06-02 13:20:05.000000 django-iubenda-web-0.0.7/README.md
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:55:08.427413 django-iubenda-web-0.0.7/django_iubenda/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/__init__.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:55:08.430967 django-iubenda-web-0.0.7/django_iubenda/core/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/core/__init__.py
--rw-r--r--   0 shadmod    (501) admin       (80)       63 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/core/admin.py
--rw-r--r--   0 shadmod    (501) admin       (80)      159 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/core/apps.py
--rw-r--r--   0 shadmod    (501) admin       (80)       57 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/core/models.py
--rw-r--r--   0 shadmod    (501) admin       (80)       63 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/core/views.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:55:08.432279 django-iubenda-web-0.0.7/django_iubenda/tests/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/tests/__init__.py
--rw-r--r--   0 shadmod    (501) admin       (80)       60 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/tests/tests.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:55:08.434843 django-iubenda-web-0.0.7/django_iubenda_web.egg-info/
--rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 13:55:08.000000 django-iubenda-web-0.0.7/django_iubenda_web.egg-info/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)      442 2023-06-02 13:55:08.000000 django-iubenda-web-0.0.7/django_iubenda_web.egg-info/SOURCES.txt
--rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-02 13:55:08.000000 django-iubenda-web-0.0.7/django_iubenda_web.egg-info/dependency_links.txt
--rw-r--r--   0 shadmod    (501) admin       (80)       15 2023-06-02 13:55:08.000000 django-iubenda-web-0.0.7/django_iubenda_web.egg-info/top_level.txt
--rw-r--r--   0 shadmod    (501) admin       (80)       79 2023-06-02 13:55:08.436466 django-iubenda-web-0.0.7/setup.cfg
--rw-r--r--   0 shadmod    (501) admin       (80)     1072 2023-06-02 13:53:07.000000 django-iubenda-web-0.0.7/setup.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 14:05:11.923584 django-iubenda-web-0.0.8/
+-rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.8/LICENSE
+-rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 14:05:11.923739 django-iubenda-web-0.0.8/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)       47 2023-06-02 13:20:05.000000 django-iubenda-web-0.0.8/README.md
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 14:05:11.915645 django-iubenda-web-0.0.8/django_iubenda/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.8/django_iubenda/__init__.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 14:05:11.919458 django-iubenda-web-0.0.8/django_iubenda/core/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.8/django_iubenda/core/__init__.py
+-rw-r--r--   0 shadmod    (501) admin       (80)       63 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.8/django_iubenda/core/admin.py
+-rw-r--r--   0 shadmod    (501) admin       (80)      159 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.8/django_iubenda/core/apps.py
+-rw-r--r--   0 shadmod    (501) admin       (80)       57 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.8/django_iubenda/core/models.py
+-rw-r--r--   0 shadmod    (501) admin       (80)       63 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.8/django_iubenda/core/views.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 14:05:11.920573 django-iubenda-web-0.0.8/django_iubenda/tests/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.8/django_iubenda/tests/__init__.py
+-rw-r--r--   0 shadmod    (501) admin       (80)       60 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.8/django_iubenda/tests/tests.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 14:05:11.923177 django-iubenda-web-0.0.8/django_iubenda_web.egg-info/
+-rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 14:05:11.000000 django-iubenda-web-0.0.8/django_iubenda_web.egg-info/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)      442 2023-06-02 14:05:11.000000 django-iubenda-web-0.0.8/django_iubenda_web.egg-info/SOURCES.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-02 14:05:11.000000 django-iubenda-web-0.0.8/django_iubenda_web.egg-info/dependency_links.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       15 2023-06-02 14:05:11.000000 django-iubenda-web-0.0.8/django_iubenda_web.egg-info/top_level.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       79 2023-06-02 14:05:11.924260 django-iubenda-web-0.0.8/setup.cfg
+-rw-r--r--   0 shadmod    (501) admin       (80)     1036 2023-06-02 14:03:34.000000 django-iubenda-web-0.0.8/setup.py
```

### Comparing `django-iubenda-web-0.0.7/LICENSE` & `django-iubenda-web-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-iubenda-web-0.0.7/PKG-INFO` & `django-iubenda-web-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-iubenda-web
-Version: 0.0.7
+Version: 0.0.8
 Summary: Iubenda integration for web application
 Home-page: https://github.com/shadMod/django_iubenda
-Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.7.tar.gz
+Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.8.tar.gz
 Author: ShadMod
 Author-email: support@shadmod.it
 License: Iubenda integration for web application
 Keywords: Django iubenda
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `django-iubenda-web-0.0.7/django_iubenda_web.egg-info/PKG-INFO` & `django-iubenda-web-0.0.8/django_iubenda_web.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-iubenda-web
-Version: 0.0.7
+Version: 0.0.8
 Summary: Iubenda integration for web application
 Home-page: https://github.com/shadMod/django_iubenda
-Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.7.tar.gz
+Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.8.tar.gz
 Author: ShadMod
 Author-email: support@shadmod.it
 License: Iubenda integration for web application
 Keywords: Django iubenda
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `django-iubenda-web-0.0.7/setup.py` & `django-iubenda-web-0.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from distutils.core import setup
 
 setup(
     name="django-iubenda-web",
-    version="0.0.7",
+    version="0.0.8",
     license="Iubenda integration for web application",
     description="Iubenda integration for web application",
     author="ShadMod",
     author_email="support@shadmod.it",
     url="https://github.com/shadMod/django_iubenda",
-    download_url="https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.7.tar.gz",
+    download_url="https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.8.tar.gz",
     packages=[
         "django_iubenda",
         "django_iubenda.core",
-        "django_iubenda.templates",
         "django_iubenda.tests",
     ],
     keywords=[
         "Django iubenda",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
```

