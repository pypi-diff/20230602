# Comparing `tmp/django-ipghrms-settingsapp-1.0.tar.gz` & `tmp/django-ipghrms-settingsapp-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ipghrms-settingsapp-1.0.tar", last modified: Mon Mar 27 15:19:37 2023, max compression
+gzip compressed data, was "django-ipghrms-settingsapp-1.1.tar", last modified: Sat Jun  3 21:32:18 2023, max compression
```

## Comparing `django-ipghrms-settingsapp-1.0.tar` & `django-ipghrms-settingsapp-1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 15:19:37.674622 django-ipghrms-settingsapp-1.0/
--rw-rw-rw-   0        0        0     1070 2023-03-27 15:14:06.000000 django-ipghrms-settingsapp-1.0/LICENSE
--rw-rw-rw-   0        0        0       80 2023-03-27 14:31:32.000000 django-ipghrms-settingsapp-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      986 2023-03-27 15:19:37.675818 django-ipghrms-settingsapp-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      531 2023-03-27 14:31:40.000000 django-ipghrms-settingsapp-1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-27 15:19:37.605978 django-ipghrms-settingsapp-1.0/django_ipghrms_settingsapp.egg-info/
--rw-rw-rw-   0        0        0      986 2023-03-27 15:19:37.000000 django-ipghrms-settingsapp-1.0/django_ipghrms_settingsapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1078 2023-03-27 15:19:37.000000 django-ipghrms-settingsapp-1.0/django_ipghrms_settingsapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 15:19:37.000000 django-ipghrms-settingsapp-1.0/django_ipghrms_settingsapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-27 15:19:37.000000 django-ipghrms-settingsapp-1.0/django_ipghrms_settingsapp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-27 15:19:37.645011 django-ipghrms-settingsapp-1.0/settings_app/
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:31.000000 django-ipghrms-settingsapp-1.0/settings_app/__init__.py
--rw-rw-rw-   0        0        0      318 2023-02-02 13:27:21.000000 django-ipghrms-settingsapp-1.0/settings_app/admin.py
--rw-rw-rw-   0        0        0      155 2022-10-18 10:39:31.000000 django-ipghrms-settingsapp-1.0/settings_app/apps.py
--rw-rw-rw-   0        0        0      683 2023-03-07 10:23:00.000000 django-ipghrms-settingsapp-1.0/settings_app/decorators.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:19:37.657801 django-ipghrms-settingsapp-1.0/settings_app/migrations/
--rw-rw-rw-   0        0        0     1263 2023-02-02 13:21:11.000000 django-ipghrms-settingsapp-1.0/settings_app/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      612 2023-02-02 13:27:50.000000 django-ipghrms-settingsapp-1.0/settings_app/migrations/0002_ipginfo_user.py
--rw-rw-rw-   0        0        0      425 2023-02-02 13:31:02.000000 django-ipghrms-settingsapp-1.0/settings_app/migrations/0003_alter_ipginfo_mobile.py
--rw-rw-rw-   0        0        0      507 2023-02-24 00:50:18.000000 django-ipghrms-settingsapp-1.0/settings_app/migrations/0004_ipginfo_cop.py
--rw-rw-rw-   0        0        0        0 2023-02-02 13:21:11.000000 django-ipghrms-settingsapp-1.0/settings_app/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:19:37.673079 django-ipghrms-settingsapp-1.0/settings_app/migrations/__pycache__/
--rw-rw-rw-   0        0        0     1099 2023-02-02 13:21:20.000000 django-ipghrms-settingsapp-1.0/settings_app/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-rw-rw-   0        0        0      778 2023-02-02 13:27:57.000000 django-ipghrms-settingsapp-1.0/settings_app/migrations/__pycache__/0002_ipginfo_user.cpython-310.pyc
--rw-rw-rw-   0        0        0      611 2023-02-02 13:31:11.000000 django-ipghrms-settingsapp-1.0/settings_app/migrations/__pycache__/0003_alter_ipginfo_mobile.cpython-310.pyc
--rw-rw-rw-   0        0        0      692 2023-02-24 00:50:28.000000 django-ipghrms-settingsapp-1.0/settings_app/migrations/__pycache__/0004_ipginfo_cop.cpython-310.pyc
--rw-rw-rw-   0        0        0      150 2023-02-02 13:21:11.000000 django-ipghrms-settingsapp-1.0/settings_app/migrations/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1593 2023-02-24 00:49:51.000000 django-ipghrms-settingsapp-1.0/settings_app/models.py
--rw-rw-rw-   0        0        0       60 2022-10-18 10:39:31.000000 django-ipghrms-settingsapp-1.0/settings_app/tests.py
--rw-rw-rw-   0        0        0     7663 2023-03-15 10:13:29.000000 django-ipghrms-settingsapp-1.0/settings_app/upload_utils.py
--rw-rw-rw-   0        0        0     1005 2023-03-16 00:00:38.000000 django-ipghrms-settingsapp-1.0/settings_app/user_utils.py
--rw-rw-rw-   0        0        0     2346 2022-12-15 07:06:35.000000 django-ipghrms-settingsapp-1.0/settings_app/utils.py
--rw-rw-rw-   0        0        0     1587 2022-10-18 10:39:31.000000 django-ipghrms-settingsapp-1.0/settings_app/utils_print.py
--rw-rw-rw-   0        0        0       63 2022-10-18 10:39:31.000000 django-ipghrms-settingsapp-1.0/settings_app/views.py
--rw-rw-rw-   0        0        0      518 2023-03-27 15:19:37.677823 django-ipghrms-settingsapp-1.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-settingsapp-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 21:32:18.173858 django-ipghrms-settingsapp-1.1/
+-rw-rw-rw-   0        0        0     1070 2023-03-27 15:14:06.000000 django-ipghrms-settingsapp-1.1/LICENSE
+-rw-rw-rw-   0        0        0       80 2023-03-27 14:31:32.000000 django-ipghrms-settingsapp-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1007 2023-06-03 21:32:18.174858 django-ipghrms-settingsapp-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      531 2023-03-27 14:31:40.000000 django-ipghrms-settingsapp-1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-03 21:32:18.082032 django-ipghrms-settingsapp-1.1/django_ipghrms_settingsapp.egg-info/
+-rw-rw-rw-   0        0        0     1007 2023-06-03 21:32:18.000000 django-ipghrms-settingsapp-1.1/django_ipghrms_settingsapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1078 2023-06-03 21:32:18.000000 django-ipghrms-settingsapp-1.1/django_ipghrms_settingsapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 21:32:18.000000 django-ipghrms-settingsapp-1.1/django_ipghrms_settingsapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 21:32:18.000000 django-ipghrms-settingsapp-1.1/django_ipghrms_settingsapp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 21:32:18.138630 django-ipghrms-settingsapp-1.1/settings_app/
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:31.000000 django-ipghrms-settingsapp-1.1/settings_app/__init__.py
+-rw-rw-rw-   0        0        0      318 2023-02-02 13:27:21.000000 django-ipghrms-settingsapp-1.1/settings_app/admin.py
+-rw-rw-rw-   0        0        0      155 2022-10-18 10:39:31.000000 django-ipghrms-settingsapp-1.1/settings_app/apps.py
+-rw-rw-rw-   0        0        0      683 2023-03-07 10:23:00.000000 django-ipghrms-settingsapp-1.1/settings_app/decorators.py
+drwxrwxrwx   0        0        0        0 2023-06-03 21:32:18.165863 django-ipghrms-settingsapp-1.1/settings_app/migrations/
+-rw-rw-rw-   0        0        0     1263 2023-02-02 13:21:11.000000 django-ipghrms-settingsapp-1.1/settings_app/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      612 2023-02-02 13:27:50.000000 django-ipghrms-settingsapp-1.1/settings_app/migrations/0002_ipginfo_user.py
+-rw-rw-rw-   0        0        0      425 2023-02-02 13:31:02.000000 django-ipghrms-settingsapp-1.1/settings_app/migrations/0003_alter_ipginfo_mobile.py
+-rw-rw-rw-   0        0        0      507 2023-02-24 00:50:18.000000 django-ipghrms-settingsapp-1.1/settings_app/migrations/0004_ipginfo_cop.py
+-rw-rw-rw-   0        0        0        0 2023-02-02 13:21:11.000000 django-ipghrms-settingsapp-1.1/settings_app/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 21:32:18.173858 django-ipghrms-settingsapp-1.1/settings_app/migrations/__pycache__/
+-rw-rw-rw-   0        0        0     1099 2023-02-02 13:21:20.000000 django-ipghrms-settingsapp-1.1/settings_app/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-rw-rw-   0        0        0      778 2023-02-02 13:27:57.000000 django-ipghrms-settingsapp-1.1/settings_app/migrations/__pycache__/0002_ipginfo_user.cpython-310.pyc
+-rw-rw-rw-   0        0        0      611 2023-02-02 13:31:11.000000 django-ipghrms-settingsapp-1.1/settings_app/migrations/__pycache__/0003_alter_ipginfo_mobile.cpython-310.pyc
+-rw-rw-rw-   0        0        0      692 2023-02-24 00:50:28.000000 django-ipghrms-settingsapp-1.1/settings_app/migrations/__pycache__/0004_ipginfo_cop.cpython-310.pyc
+-rw-rw-rw-   0        0        0      150 2023-02-02 13:21:11.000000 django-ipghrms-settingsapp-1.1/settings_app/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1593 2023-02-24 00:49:51.000000 django-ipghrms-settingsapp-1.1/settings_app/models.py
+-rw-rw-rw-   0        0        0       60 2022-10-18 10:39:31.000000 django-ipghrms-settingsapp-1.1/settings_app/tests.py
+-rw-rw-rw-   0        0        0     7663 2023-03-15 10:13:29.000000 django-ipghrms-settingsapp-1.1/settings_app/upload_utils.py
+-rw-rw-rw-   0        0        0     1005 2023-03-16 00:00:38.000000 django-ipghrms-settingsapp-1.1/settings_app/user_utils.py
+-rw-rw-rw-   0        0        0     2346 2022-12-15 07:06:35.000000 django-ipghrms-settingsapp-1.1/settings_app/utils.py
+-rw-rw-rw-   0        0        0     1587 2022-10-18 10:39:31.000000 django-ipghrms-settingsapp-1.1/settings_app/utils_print.py
+-rw-rw-rw-   0        0        0       63 2022-10-18 10:39:31.000000 django-ipghrms-settingsapp-1.1/settings_app/views.py
+-rw-rw-rw-   0        0        0      518 2023-06-03 21:32:18.175855 django-ipghrms-settingsapp-1.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-settingsapp-1.1/setup.py
```

### Comparing `django-ipghrms-settingsapp-1.0/LICENSE` & `django-ipghrms-settingsapp-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/PKG-INFO` & `django-ipghrms-settingsapp-1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-settingsapp
-Version: 1.0
+Version: 1.1
 Summary: Django IPG HRMS APP settings_app
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
 
 
@@ -36,7 +37,8 @@
 
 3. Run ``python manage.py migrate`` to create settings_app model
 
 4. Another Apps Need for this Apps::
     4.1. custom::
     4.2. employee::
     4.3. user
+
```

### Comparing `django-ipghrms-settingsapp-1.0/README.rst` & `django-ipghrms-settingsapp-1.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/django_ipghrms_settingsapp.egg-info/PKG-INFO` & `django-ipghrms-settingsapp-1.1/django_ipghrms_settingsapp.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-settingsapp
-Version: 1.0
+Version: 1.1
 Summary: Django IPG HRMS APP settings_app
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
 
 
@@ -36,7 +37,8 @@
 
 3. Run ``python manage.py migrate`` to create settings_app model
 
 4. Another Apps Need for this Apps::
     4.1. custom::
     4.2. employee::
     4.3. user
+
```

### Comparing `django-ipghrms-settingsapp-1.0/django_ipghrms_settingsapp.egg-info/SOURCES.txt` & `django-ipghrms-settingsapp-1.1/django_ipghrms_settingsapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/settings_app/decorators.py` & `django-ipghrms-settingsapp-1.1/settings_app/decorators.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/settings_app/migrations/0001_initial.py` & `django-ipghrms-settingsapp-1.1/settings_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/settings_app/migrations/0002_ipginfo_user.py` & `django-ipghrms-settingsapp-1.1/settings_app/migrations/0002_ipginfo_user.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/settings_app/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-ipghrms-settingsapp-1.1/settings_app/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/settings_app/migrations/__pycache__/0002_ipginfo_user.cpython-310.pyc` & `django-ipghrms-settingsapp-1.1/settings_app/migrations/__pycache__/0002_ipginfo_user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/settings_app/migrations/__pycache__/0003_alter_ipginfo_mobile.cpython-310.pyc` & `django-ipghrms-settingsapp-1.1/settings_app/migrations/__pycache__/0003_alter_ipginfo_mobile.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/settings_app/migrations/__pycache__/0004_ipginfo_cop.cpython-310.pyc` & `django-ipghrms-settingsapp-1.1/settings_app/migrations/__pycache__/0004_ipginfo_cop.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/settings_app/models.py` & `django-ipghrms-settingsapp-1.1/settings_app/models.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/settings_app/upload_utils.py` & `django-ipghrms-settingsapp-1.1/settings_app/upload_utils.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/settings_app/user_utils.py` & `django-ipghrms-settingsapp-1.1/settings_app/user_utils.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/settings_app/utils.py` & `django-ipghrms-settingsapp-1.1/settings_app/utils.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/settings_app/utils_print.py` & `django-ipghrms-settingsapp-1.1/settings_app/utils_print.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-settingsapp-1.0/setup.cfg` & `django-ipghrms-settingsapp-1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 6970 6768 726d   = django-ipghrm
 00000020: 732d 7365 7474 696e 6773 6170 700d 0a76  s-settingsapp..v
-00000030: 6572 7369 6f6e 203d 2031 2e30 0d0a 6175  ersion = 1.0..au
+00000030: 6572 7369 6f6e 203d 2031 2e31 0d0a 6175  ersion = 1.1..au
 00000040: 7468 6f72 203d 204b 696e 6f73 0d0a 6175  thor = Kinos..au
 00000050: 7468 6f72 5f65 6d61 696c 203d 2069 6e66  thor_email = inf
 00000060: 6f40 6b69 6e6f 732e 746c 0d0a 6d61 696e  o@kinos.tl..main
 00000070: 7461 696e 6572 203d 206b 696e 6f73 0d0a  tainer = kinos..
 00000080: 6d61 696e 7461 696e 6572 5f65 6d61 696c  maintainer_email
 00000090: 203d 2069 6e66 6f40 6b69 6e6f 732e 746c   = info@kinos.tl
 000000a0: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description =
```

