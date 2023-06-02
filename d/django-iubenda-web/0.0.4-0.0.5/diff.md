# Comparing `tmp/django-iubenda-web-0.0.4.tar.gz` & `tmp/django-iubenda-web-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-iubenda-web-0.0.4.tar", last modified: Fri Jun  2 13:28:36 2023, max compression
+gzip compressed data, was "django-iubenda-web-0.0.5.tar", last modified: Fri Jun  2 13:36:24 2023, max compression
```

## Comparing `django-iubenda-web-0.0.4.tar` & `django-iubenda-web-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:28:36.237087 django-iubenda-web-0.0.4/
--rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.4/LICENSE
--rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 13:28:36.237238 django-iubenda-web-0.0.4/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)       47 2023-06-02 13:20:05.000000 django-iubenda-web-0.0.4/README.md
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:28:36.235397 django-iubenda-web-0.0.4/django_iubenda/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.4/django_iubenda/__init__.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:28:36.236741 django-iubenda-web-0.0.4/django_iubenda_web.egg-info/
--rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 13:28:36.000000 django-iubenda-web-0.0.4/django_iubenda_web.egg-info/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)      231 2023-06-02 13:28:36.000000 django-iubenda-web-0.0.4/django_iubenda_web.egg-info/SOURCES.txt
--rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-02 13:28:36.000000 django-iubenda-web-0.0.4/django_iubenda_web.egg-info/dependency_links.txt
--rw-r--r--   0 shadmod    (501) admin       (80)       15 2023-06-02 13:28:36.000000 django-iubenda-web-0.0.4/django_iubenda_web.egg-info/top_level.txt
--rw-r--r--   0 shadmod    (501) admin       (80)       79 2023-06-02 13:28:36.237756 django-iubenda-web-0.0.4/setup.cfg
--rw-r--r--   0 shadmod    (501) admin       (80)      958 2023-06-02 13:28:06.000000 django-iubenda-web-0.0.4/setup.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:36:24.528112 django-iubenda-web-0.0.5/
+-rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.5/LICENSE
+-rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 13:36:24.528307 django-iubenda-web-0.0.5/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)       47 2023-06-02 13:20:05.000000 django-iubenda-web-0.0.5/README.md
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:36:24.527593 django-iubenda-web-0.0.5/django_iubenda_web.egg-info/
+-rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 13:36:24.000000 django-iubenda-web-0.0.5/django_iubenda_web.egg-info/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)      204 2023-06-02 13:36:24.000000 django-iubenda-web-0.0.5/django_iubenda_web.egg-info/SOURCES.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-02 13:36:24.000000 django-iubenda-web-0.0.5/django_iubenda_web.egg-info/dependency_links.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       15 2023-06-02 13:36:24.000000 django-iubenda-web-0.0.5/django_iubenda_web.egg-info/top_level.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       79 2023-06-02 13:36:24.528855 django-iubenda-web-0.0.5/setup.cfg
+-rw-r--r--   0 shadmod    (501) admin       (80)      958 2023-06-02 13:35:36.000000 django-iubenda-web-0.0.5/setup.py
```

### Comparing `django-iubenda-web-0.0.4/LICENSE` & `django-iubenda-web-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-iubenda-web-0.0.4/PKG-INFO` & `django-iubenda-web-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-iubenda-web
-Version: 0.0.4
+Version: 0.0.5
 Summary: Iubenda integration for web application
 Home-page: https://github.com/shadMod/django_iubenda
-Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.4.tar.gz
+Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.5.tar.gz
 Author: ShadMod
 Author-email: support@shadmod.it
 License: Iubenda integration for web application
 Keywords: Django iubenda
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `django-iubenda-web-0.0.4/django_iubenda_web.egg-info/PKG-INFO` & `django-iubenda-web-0.0.5/django_iubenda_web.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-iubenda-web
-Version: 0.0.4
+Version: 0.0.5
 Summary: Iubenda integration for web application
 Home-page: https://github.com/shadMod/django_iubenda
-Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.4.tar.gz
+Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.5.tar.gz
 Author: ShadMod
 Author-email: support@shadmod.it
 License: Iubenda integration for web application
 Keywords: Django iubenda
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `django-iubenda-web-0.0.4/setup.py` & `django-iubenda-web-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
     name="django-iubenda-web",
     packages=["django_iubenda"],
-    version="0.0.4",
+    version="0.0.5",
     license="Iubenda integration for web application",
     description="Iubenda integration for web application",
     author="ShadMod",
     author_email="support@shadmod.it",
     url="https://github.com/shadMod/django_iubenda",
-    download_url="https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.4.tar.gz",
+    download_url="https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.5.tar.gz",
     keywords=[
         "Django iubenda",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
```

