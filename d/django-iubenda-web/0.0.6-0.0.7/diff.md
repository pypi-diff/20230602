# Comparing `tmp/django-iubenda-web-0.0.6.tar.gz` & `tmp/django-iubenda-web-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-iubenda-web-0.0.6.tar", last modified: Fri Jun  2 13:41:05 2023, max compression
+gzip compressed data, was "django-iubenda-web-0.0.7.tar", last modified: Fri Jun  2 13:55:08 2023, max compression
```

## Comparing `django-iubenda-web-0.0.6.tar` & `django-iubenda-web-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,22 @@
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:41:05.935315 django-iubenda-web-0.0.6/
--rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.6/LICENSE
--rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 13:41:05.935457 django-iubenda-web-0.0.6/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)       47 2023-06-02 13:20:05.000000 django-iubenda-web-0.0.6/README.md
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:41:05.934953 django-iubenda-web-0.0.6/django_iubenda_web.egg-info/
--rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 13:41:05.000000 django-iubenda-web-0.0.6/django_iubenda_web.egg-info/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)      204 2023-06-02 13:41:05.000000 django-iubenda-web-0.0.6/django_iubenda_web.egg-info/SOURCES.txt
--rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-02 13:41:05.000000 django-iubenda-web-0.0.6/django_iubenda_web.egg-info/dependency_links.txt
--rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-02 13:41:05.000000 django-iubenda-web-0.0.6/django_iubenda_web.egg-info/top_level.txt
--rw-r--r--   0 shadmod    (501) admin       (80)       79 2023-06-02 13:41:05.935958 django-iubenda-web-0.0.6/setup.cfg
--rw-r--r--   0 shadmod    (501) admin       (80)     1012 2023-06-02 13:41:00.000000 django-iubenda-web-0.0.6/setup.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:55:08.435339 django-iubenda-web-0.0.7/
+-rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/LICENSE
+-rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 13:55:08.435532 django-iubenda-web-0.0.7/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)       47 2023-06-02 13:20:05.000000 django-iubenda-web-0.0.7/README.md
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:55:08.427413 django-iubenda-web-0.0.7/django_iubenda/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/__init__.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:55:08.430967 django-iubenda-web-0.0.7/django_iubenda/core/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/core/__init__.py
+-rw-r--r--   0 shadmod    (501) admin       (80)       63 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/core/admin.py
+-rw-r--r--   0 shadmod    (501) admin       (80)      159 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/core/apps.py
+-rw-r--r--   0 shadmod    (501) admin       (80)       57 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/core/models.py
+-rw-r--r--   0 shadmod    (501) admin       (80)       63 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/core/views.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:55:08.432279 django-iubenda-web-0.0.7/django_iubenda/tests/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/tests/__init__.py
+-rw-r--r--   0 shadmod    (501) admin       (80)       60 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.7/django_iubenda/tests/tests.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:55:08.434843 django-iubenda-web-0.0.7/django_iubenda_web.egg-info/
+-rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 13:55:08.000000 django-iubenda-web-0.0.7/django_iubenda_web.egg-info/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)      442 2023-06-02 13:55:08.000000 django-iubenda-web-0.0.7/django_iubenda_web.egg-info/SOURCES.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-02 13:55:08.000000 django-iubenda-web-0.0.7/django_iubenda_web.egg-info/dependency_links.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       15 2023-06-02 13:55:08.000000 django-iubenda-web-0.0.7/django_iubenda_web.egg-info/top_level.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       79 2023-06-02 13:55:08.436466 django-iubenda-web-0.0.7/setup.cfg
+-rw-r--r--   0 shadmod    (501) admin       (80)     1072 2023-06-02 13:53:07.000000 django-iubenda-web-0.0.7/setup.py
```

### Comparing `django-iubenda-web-0.0.6/LICENSE` & `django-iubenda-web-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-iubenda-web-0.0.6/PKG-INFO` & `django-iubenda-web-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-iubenda-web
-Version: 0.0.6
+Version: 0.0.7
 Summary: Iubenda integration for web application
 Home-page: https://github.com/shadMod/django_iubenda
-Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.6.tar.gz
+Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.7.tar.gz
 Author: ShadMod
 Author-email: support@shadmod.it
 License: Iubenda integration for web application
 Keywords: Django iubenda
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `django-iubenda-web-0.0.6/django_iubenda_web.egg-info/PKG-INFO` & `django-iubenda-web-0.0.7/django_iubenda_web.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-iubenda-web
-Version: 0.0.6
+Version: 0.0.7
 Summary: Iubenda integration for web application
 Home-page: https://github.com/shadMod/django_iubenda
-Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.6.tar.gz
+Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.7.tar.gz
 Author: ShadMod
 Author-email: support@shadmod.it
 License: Iubenda integration for web application
 Keywords: Django iubenda
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `django-iubenda-web-0.0.6/setup.py` & `django-iubenda-web-0.0.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-from setuptools import setup, find_packages
+from distutils.core import setup
 
 setup(
     name="django-iubenda-web",
-    packages=find_packages(include=("django_iubenda", "django_iubenda.*")),
-    version="0.0.6",
+    version="0.0.7",
     license="Iubenda integration for web application",
     description="Iubenda integration for web application",
     author="ShadMod",
     author_email="support@shadmod.it",
     url="https://github.com/shadMod/django_iubenda",
-    download_url="https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.6.tar.gz",
+    download_url="https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.7.tar.gz",
+    packages=[
+        "django_iubenda",
+        "django_iubenda.core",
+        "django_iubenda.templates",
+        "django_iubenda.tests",
+    ],
     keywords=[
         "Django iubenda",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
```

