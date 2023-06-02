# Comparing `tmp/django-mermaid-0.0.6.tar.gz` & `tmp/django-mermaid-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mermaid-0.0.6.tar", last modified: Wed May 24 18:29:13 2023, max compression
+gzip compressed data, was "django-mermaid-0.0.7.tar", last modified: Fri Jun  2 16:54:28 2023, max compression
```

## Comparing `django-mermaid-0.0.6.tar` & `django-mermaid-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:29:13.909531 django-mermaid-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 18:29:01.000000 django-mermaid-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-24 18:29:13.909531 django-mermaid-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-24 18:29:01.000000 django-mermaid-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 18:29:01.000000 django-mermaid-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-24 18:29:13.909531 django-mermaid-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-24 18:29:01.000000 django-mermaid-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:29:13.905531 django-mermaid-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:29:13.905531 django-mermaid-0.0.6/src/django_mermaid/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 18:29:01.000000 django-mermaid-0.0.6/src/django_mermaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-24 18:29:01.000000 django-mermaid-0.0.6/src/django_mermaid/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:29:13.909531 django-mermaid-0.0.6/src/django_mermaid/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-24 18:29:01.000000 django-mermaid-0.0.6/src/django_mermaid/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-24 18:29:01.000000 django-mermaid-0.0.6/src/django_mermaid/templatetags/mermaid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:29:13.905531 django-mermaid-0.0.6/src/django_mermaid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-24 18:29:13.000000 django-mermaid-0.0.6/src/django_mermaid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-24 18:29:13.000000 django-mermaid-0.0.6/src/django_mermaid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:29:13.000000 django-mermaid-0.0.6/src/django_mermaid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:29:13.000000 django-mermaid-0.0.6/src/django_mermaid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 18:29:13.000000 django-mermaid-0.0.6/src/django_mermaid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 18:29:13.000000 django-mermaid-0.0.6/src/django_mermaid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:54:28.000728 django-mermaid-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-02 16:54:17.000000 django-mermaid-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 16:54:17.000000 django-mermaid-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-02 16:54:28.000728 django-mermaid-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-02 16:54:17.000000 django-mermaid-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-02 16:54:17.000000 django-mermaid-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-02 16:54:28.000728 django-mermaid-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 16:54:17.000000 django-mermaid-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:54:27.996728 django-mermaid-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:54:28.000728 django-mermaid-0.0.7/src/django_mermaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 16:54:17.000000 django-mermaid-0.0.7/src/django_mermaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-02 16:54:17.000000 django-mermaid-0.0.7/src/django_mermaid/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:54:27.996728 django-mermaid-0.0.7/src/django_mermaid/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:54:27.996728 django-mermaid-0.0.7/src/django_mermaid/static/mermaid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:54:28.000728 django-mermaid-0.0.7/src/django_mermaid/static/mermaid/9.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:54:17.000000 django-mermaid-0.0.7/src/django_mermaid/static/mermaid/9.4.3/mermaid.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:54:28.000728 django-mermaid-0.0.7/src/django_mermaid/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-02 16:54:17.000000 django-mermaid-0.0.7/src/django_mermaid/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-02 16:54:17.000000 django-mermaid-0.0.7/src/django_mermaid/templatetags/mermaid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:54:28.000728 django-mermaid-0.0.7/src/django_mermaid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-02 16:54:27.000000 django-mermaid-0.0.7/src/django_mermaid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-02 16:54:27.000000 django-mermaid-0.0.7/src/django_mermaid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:54:27.000000 django-mermaid-0.0.7/src/django_mermaid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:54:27.000000 django-mermaid-0.0.7/src/django_mermaid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 16:54:27.000000 django-mermaid-0.0.7/src/django_mermaid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 16:54:27.000000 django-mermaid-0.0.7/src/django_mermaid.egg-info/top_level.txt
```

### Comparing `django-mermaid-0.0.6/LICENSE` & `django-mermaid-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mermaid-0.0.6/PKG-INFO` & `django-mermaid-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mermaid
-Version: 0.0.6
+Version: 0.0.7
 Summary: Django template tag for rendering mermaid diagrams.
 Home-page: https://github.com/pysnippet/django-mermaid
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Keywords: python,django,mermaid,tag,graph,jinja,diagram,template
 Platform: unix
```

### Comparing `django-mermaid-0.0.6/README.md` & `django-mermaid-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `django-mermaid-0.0.6/setup.cfg` & `django-mermaid-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-mermaid-0.0.6/src/django_mermaid/apps.py` & `django-mermaid-0.0.7/src/django_mermaid/apps.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-from distutils import dir_util
-from os import stat
-from os.path import dirname
-from os.path import exists
-from os.path import join
+import pathlib
 from urllib.request import urlretrieve
 
 from django.apps import AppConfig
 from django.conf import settings
 
 from .templatetags import DEFAULT_VERSION
 
@@ -14,13 +10,15 @@
 class MermaidConfig(AppConfig):
     name = "django_mermaid"
 
     def ready(self):
         """Download mermaid.js from CDN if not already present"""
         version = getattr(settings, "MERMAID_VERSION", DEFAULT_VERSION)
         cdn = "https://cdnjs.cloudflare.com/ajax/libs/mermaid/%s/mermaid.min.js" % version
-        static_dir = join(dirname(__file__), "static")
-        mermaid_dir = join(static_dir, "mermaid", version)
-        if not exists(join(mermaid_dir, "mermaid.js")) or \
-                stat(join(mermaid_dir, "mermaid.js")).st_size == 0:
-            dir_util.create_tree(mermaid_dir, ["mermaid.js"])
-            urlretrieve(cdn, join(mermaid_dir, "mermaid.js"))
+        current_dir = pathlib.Path(__file__).parent
+        static_dir = current_dir / "static"
+        mermaid_dir = static_dir / "mermaid" / version
+        mermaid_js = mermaid_dir / "mermaid.js"
+        if not mermaid_js.exists() or \
+               mermaid_js.stat().st_size == 0:
+            mermaid_dir.mkdir(parents=True, exist_ok=True)
+            urlretrieve(cdn, str(mermaid_js))
```

### Comparing `django-mermaid-0.0.6/src/django_mermaid/templatetags/mermaid.py` & `django-mermaid-0.0.7/src/django_mermaid/templatetags/mermaid.py`

 * *Files identical despite different names*

### Comparing `django-mermaid-0.0.6/src/django_mermaid.egg-info/PKG-INFO` & `django-mermaid-0.0.7/src/django_mermaid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mermaid
-Version: 0.0.6
+Version: 0.0.7
 Summary: Django template tag for rendering mermaid diagrams.
 Home-page: https://github.com/pysnippet/django-mermaid
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Keywords: python,django,mermaid,tag,graph,jinja,diagram,template
 Platform: unix
```

