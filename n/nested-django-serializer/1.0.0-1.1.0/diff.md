# Comparing `tmp/nested_django_serializer-1.0.0.tar.gz` & `tmp/nested_django_serializer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nested_django_serializer-1.0.0.tar", last modified: Fri Jun  2 02:19:47 2023, max compression
+gzip compressed data, was "nested_django_serializer-1.1.0.tar", last modified: Fri Jun  2 17:37:08 2023, max compression
```

## Comparing `nested_django_serializer-1.0.0.tar` & `nested_django_serializer-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 cschneider  (1000) cschneider  (1000)        0 2023-06-02 02:19:47.273273 nested_django_serializer-1.0.0/
--rwxr-xr-x   0 cschneider  (1000) cschneider  (1000)       33 2023-06-01 16:02:47.000000 nested_django_serializer-1.0.0/AUTHORS
--rwxr-xr-x   0 cschneider  (1000) cschneider  (1000)     1630 2023-06-01 16:02:47.000000 nested_django_serializer-1.0.0/LICENSE
--rw-rw-r--   0 cschneider  (1000) cschneider  (1000)      843 2023-06-02 02:19:47.273273 nested_django_serializer-1.0.0/PKG-INFO
--rwxr-xr-x   0 cschneider  (1000) cschneider  (1000)      168 2023-06-01 14:42:50.000000 nested_django_serializer-1.0.0/README.md
-drwxrwxr-x   0 cschneider  (1000) cschneider  (1000)        0 2023-06-02 02:19:47.273273 nested_django_serializer-1.0.0/nested_django_serializer/
--rw-rw-r--   0 cschneider  (1000) cschneider  (1000)        0 2023-06-02 01:45:17.000000 nested_django_serializer-1.0.0/nested_django_serializer/__init__.py
-drwxrwxr-x   0 cschneider  (1000) cschneider  (1000)        0 2023-06-02 02:19:47.273273 nested_django_serializer-1.0.0/nested_django_serializer/django/
--rwxr-xr-x   0 cschneider  (1000) cschneider  (1000)        0 2023-06-01 11:28:24.000000 nested_django_serializer-1.0.0/nested_django_serializer/django/__init__.py
-drwxrwxr-x   0 cschneider  (1000) cschneider  (1000)        0 2023-06-02 02:19:47.273273 nested_django_serializer-1.0.0/nested_django_serializer/django/serializers/
--rwxr-xr-x   0 cschneider  (1000) cschneider  (1000)       22 2023-06-01 14:53:17.000000 nested_django_serializer-1.0.0/nested_django_serializer/django/serializers/__init__.py
--rwxr-xr-x   0 cschneider  (1000) cschneider  (1000)     3035 2023-06-01 13:23:12.000000 nested_django_serializer-1.0.0/nested_django_serializer/django/serializers/base.py
--rwxr-xr-x   0 cschneider  (1000) cschneider  (1000)      752 2023-06-01 14:53:17.000000 nested_django_serializer-1.0.0/nested_django_serializer/django/serializers/json.py
--rwxr-xr-x   0 cschneider  (1000) cschneider  (1000)     5858 2023-06-01 14:53:17.000000 nested_django_serializer-1.0.0/nested_django_serializer/django/serializers/python.py
-drwxrwxr-x   0 cschneider  (1000) cschneider  (1000)        0 2023-06-02 02:19:47.273273 nested_django_serializer-1.0.0/nested_django_serializer.egg-info/
--rw-rw-r--   0 cschneider  (1000) cschneider  (1000)      843 2023-06-02 02:19:47.000000 nested_django_serializer-1.0.0/nested_django_serializer.egg-info/PKG-INFO
--rw-rw-r--   0 cschneider  (1000) cschneider  (1000)      568 2023-06-02 02:19:47.000000 nested_django_serializer-1.0.0/nested_django_serializer.egg-info/SOURCES.txt
--rw-rw-r--   0 cschneider  (1000) cschneider  (1000)        1 2023-06-02 02:19:47.000000 nested_django_serializer-1.0.0/nested_django_serializer.egg-info/dependency_links.txt
--rw-rw-r--   0 cschneider  (1000) cschneider  (1000)        7 2023-06-02 02:19:47.000000 nested_django_serializer-1.0.0/nested_django_serializer.egg-info/requires.txt
--rw-rw-r--   0 cschneider  (1000) cschneider  (1000)       25 2023-06-02 02:19:47.000000 nested_django_serializer-1.0.0/nested_django_serializer.egg-info/top_level.txt
--rw-rw-r--   0 cschneider  (1000) cschneider  (1000)       38 2023-06-02 02:19:47.273273 nested_django_serializer-1.0.0/setup.cfg
--rwxr-xr-x   0 cschneider  (1000) cschneider  (1000)     1033 2023-06-02 02:19:22.000000 nested_django_serializer-1.0.0/setup.py
+drwxrwxr-x   0 cschneider  (1002) cschneider  (1002)        0 2023-06-02 17:37:08.274000 nested_django_serializer-1.1.0/
+-rwxrwxr-x   0 cschneider  (1002) cschneider  (1002)       33 2023-06-02 15:12:09.000000 nested_django_serializer-1.1.0/AUTHORS
+-rwxrwxr-x   0 cschneider  (1002) cschneider  (1002)     1630 2023-06-02 15:12:09.000000 nested_django_serializer-1.1.0/LICENSE
+-rw-rw-r--   0 cschneider  (1002) cschneider  (1002)     3584 2023-06-02 17:37:08.274000 nested_django_serializer-1.1.0/PKG-INFO
+-rwxrwxr-x   0 cschneider  (1002) cschneider  (1002)     2873 2023-06-02 17:04:07.000000 nested_django_serializer-1.1.0/README.md
+drwxrwxr-x   0 cschneider  (1002) cschneider  (1002)        0 2023-06-02 17:37:08.274000 nested_django_serializer-1.1.0/nested_django_serializer/
+-rw-rw-r--   0 cschneider  (1002) cschneider  (1002)        0 2023-06-02 15:12:09.000000 nested_django_serializer-1.1.0/nested_django_serializer/__init__.py
+drwxrwxr-x   0 cschneider  (1002) cschneider  (1002)        0 2023-06-02 17:37:08.274000 nested_django_serializer-1.1.0/nested_django_serializer/django/
+-rwxrwxr-x   0 cschneider  (1002) cschneider  (1002)        0 2023-06-02 15:12:09.000000 nested_django_serializer-1.1.0/nested_django_serializer/django/__init__.py
+drwxrwxr-x   0 cschneider  (1002) cschneider  (1002)        0 2023-06-02 17:37:08.274000 nested_django_serializer-1.1.0/nested_django_serializer/django/serializers/
+-rwxrwxr-x   0 cschneider  (1002) cschneider  (1002)       22 2023-06-02 15:12:09.000000 nested_django_serializer-1.1.0/nested_django_serializer/django/serializers/__init__.py
+-rwxrwxr-x   0 cschneider  (1002) cschneider  (1002)     3035 2023-06-02 15:12:09.000000 nested_django_serializer-1.1.0/nested_django_serializer/django/serializers/base.py
+-rwxrwxr-x   0 cschneider  (1002) cschneider  (1002)      752 2023-06-02 15:12:09.000000 nested_django_serializer-1.1.0/nested_django_serializer/django/serializers/json.py
+-rwxrwxr-x   0 cschneider  (1002) cschneider  (1002)     5858 2023-06-02 15:12:09.000000 nested_django_serializer-1.1.0/nested_django_serializer/django/serializers/python.py
+drwxrwxr-x   0 cschneider  (1002) cschneider  (1002)        0 2023-06-02 17:37:08.274000 nested_django_serializer-1.1.0/nested_django_serializer.egg-info/
+-rw-rw-r--   0 cschneider  (1002) cschneider  (1002)     3584 2023-06-02 17:37:08.000000 nested_django_serializer-1.1.0/nested_django_serializer.egg-info/PKG-INFO
+-rw-rw-r--   0 cschneider  (1002) cschneider  (1002)      568 2023-06-02 17:37:08.000000 nested_django_serializer-1.1.0/nested_django_serializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 cschneider  (1002) cschneider  (1002)        1 2023-06-02 17:37:08.000000 nested_django_serializer-1.1.0/nested_django_serializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 cschneider  (1002) cschneider  (1002)        7 2023-06-02 17:37:08.000000 nested_django_serializer-1.1.0/nested_django_serializer.egg-info/requires.txt
+-rw-rw-r--   0 cschneider  (1002) cschneider  (1002)       25 2023-06-02 17:37:08.000000 nested_django_serializer-1.1.0/nested_django_serializer.egg-info/top_level.txt
+-rw-rw-r--   0 cschneider  (1002) cschneider  (1002)       38 2023-06-02 17:37:08.274000 nested_django_serializer-1.1.0/setup.cfg
+-rwxrwxr-x   0 cschneider  (1002) cschneider  (1002)     1133 2023-06-02 15:18:18.000000 nested_django_serializer-1.1.0/setup.py
```

### Comparing `nested_django_serializer-1.0.0/LICENSE` & `nested_django_serializer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nested_django_serializer-1.0.0/nested_django_serializer/django/serializers/base.py` & `nested_django_serializer-1.1.0/nested_django_serializer/django/serializers/base.py`

 * *Files identical despite different names*

### Comparing `nested_django_serializer-1.0.0/nested_django_serializer/django/serializers/json.py` & `nested_django_serializer-1.1.0/nested_django_serializer/django/serializers/json.py`

 * *Files identical despite different names*

### Comparing `nested_django_serializer-1.0.0/nested_django_serializer/django/serializers/python.py` & `nested_django_serializer-1.1.0/nested_django_serializer/django/serializers/python.py`

 * *Files identical despite different names*

### Comparing `nested_django_serializer-1.0.0/nested_django_serializer.egg-info/SOURCES.txt` & `nested_django_serializer-1.1.0/nested_django_serializer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nested_django_serializer-1.0.0/setup.py` & `nested_django_serializer-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import nested_django_serializer.django.serializers
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="nested_django_serializer",
-    version="1.0.0",
+    version="1.1.0",
     author="Colton Schneider",
     description="Modifies the Django serializer such that it fully serializes foreign key relations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=(
         "nested_django_serializer",
         "nested_django_serializer.django",
@@ -25,9 +25,12 @@
         "License :: OSI Approved :: MIT License",
         "Topic :: Utilities",
         "Framework :: Django"
     ],
     python_requires=">=3.8",
     install_requires=["django"],
     license="MIT",
-    keywords="django json serializer"
+    keywords="django json serializer",
+    project_urls={
+        "Github": "https://github.com/colton305/nested-django-serializer"
+    }
 )
```

