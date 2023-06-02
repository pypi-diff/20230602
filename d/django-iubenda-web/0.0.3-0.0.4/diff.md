# Comparing `tmp/django-iubenda-web-0.0.3.tar.gz` & `tmp/django-iubenda-web-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-iubenda-web-0.0.3.tar", last modified: Fri Jun  2 13:21:13 2023, max compression
+gzip compressed data, was "django-iubenda-web-0.0.4.tar", last modified: Fri Jun  2 13:28:36 2023, max compression
```

## Comparing `django-iubenda-web-0.0.3.tar` & `django-iubenda-web-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:21:13.821665 django-iubenda-web-0.0.3/
--rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.3/LICENSE
--rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 13:21:13.821810 django-iubenda-web-0.0.3/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)       47 2023-06-02 13:20:05.000000 django-iubenda-web-0.0.3/README.md
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:21:13.821342 django-iubenda-web-0.0.3/django_iubenda_web.egg-info/
--rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 13:21:13.000000 django-iubenda-web-0.0.3/django_iubenda_web.egg-info/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)      204 2023-06-02 13:21:13.000000 django-iubenda-web-0.0.3/django_iubenda_web.egg-info/SOURCES.txt
--rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-02 13:21:13.000000 django-iubenda-web-0.0.3/django_iubenda_web.egg-info/dependency_links.txt
--rw-r--r--   0 shadmod    (501) admin       (80)       15 2023-06-02 13:21:13.000000 django-iubenda-web-0.0.3/django_iubenda_web.egg-info/top_level.txt
--rw-r--r--   0 shadmod    (501) admin       (80)       79 2023-06-02 13:21:13.822306 django-iubenda-web-0.0.3/setup.cfg
--rw-r--r--   0 shadmod    (501) admin       (80)      958 2023-06-02 13:20:31.000000 django-iubenda-web-0.0.3/setup.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:28:36.237087 django-iubenda-web-0.0.4/
+-rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.4/LICENSE
+-rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 13:28:36.237238 django-iubenda-web-0.0.4/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)       47 2023-06-02 13:20:05.000000 django-iubenda-web-0.0.4/README.md
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:28:36.235397 django-iubenda-web-0.0.4/django_iubenda/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-02 12:36:33.000000 django-iubenda-web-0.0.4/django_iubenda/__init__.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-02 13:28:36.236741 django-iubenda-web-0.0.4/django_iubenda_web.egg-info/
+-rw-r--r--   0 shadmod    (501) admin       (80)      841 2023-06-02 13:28:36.000000 django-iubenda-web-0.0.4/django_iubenda_web.egg-info/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)      231 2023-06-02 13:28:36.000000 django-iubenda-web-0.0.4/django_iubenda_web.egg-info/SOURCES.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-02 13:28:36.000000 django-iubenda-web-0.0.4/django_iubenda_web.egg-info/dependency_links.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       15 2023-06-02 13:28:36.000000 django-iubenda-web-0.0.4/django_iubenda_web.egg-info/top_level.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       79 2023-06-02 13:28:36.237756 django-iubenda-web-0.0.4/setup.cfg
+-rw-r--r--   0 shadmod    (501) admin       (80)      958 2023-06-02 13:28:06.000000 django-iubenda-web-0.0.4/setup.py
```

### Comparing `django-iubenda-web-0.0.3/LICENSE` & `django-iubenda-web-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-iubenda-web-0.0.3/PKG-INFO` & `django-iubenda-web-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-iubenda-web
-Version: 0.0.3
+Version: 0.0.4
 Summary: Iubenda integration for web application
 Home-page: https://github.com/shadMod/django_iubenda
-Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.3.tar.gz
+Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.4.tar.gz
 Author: ShadMod
 Author-email: support@shadmod.it
 License: Iubenda integration for web application
 Keywords: Django iubenda
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `django-iubenda-web-0.0.3/django_iubenda_web.egg-info/PKG-INFO` & `django-iubenda-web-0.0.4/django_iubenda_web.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-iubenda-web
-Version: 0.0.3
+Version: 0.0.4
 Summary: Iubenda integration for web application
 Home-page: https://github.com/shadMod/django_iubenda
-Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.3.tar.gz
+Download-URL: https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.4.tar.gz
 Author: ShadMod
 Author-email: support@shadmod.it
 License: Iubenda integration for web application
 Keywords: Django iubenda
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `django-iubenda-web-0.0.3/setup.py` & `django-iubenda-web-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
     name="django-iubenda-web",
     packages=["django_iubenda"],
-    version="0.0.3",
+    version="0.0.4",
     license="Iubenda integration for web application",
     description="Iubenda integration for web application",
     author="ShadMod",
     author_email="support@shadmod.it",
     url="https://github.com/shadMod/django_iubenda",
-    download_url="https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.3.tar.gz",
+    download_url="https://github.com/shadMod/django_iubenda/archive/refs/tags/0.0.4.tar.gz",
     keywords=[
         "Django iubenda",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
```

