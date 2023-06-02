# Comparing `tmp/django_modshib_certic-0.1.4.tar.gz` & `tmp/django_modshib_certic-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_modshib_certic-0.1.4.tar", max compression
+gzip compressed data, was "django_modshib_certic-0.1.5.tar", max compression
```

## Comparing `django_modshib_certic-0.1.4.tar` & `django_modshib_certic-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-05-19 06:10:59.653227 django_modshib_certic-0.1.4/modshib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-19 06:10:59.654166 django_modshib_certic-0.1.4/modshib/admin.py
--rw-r--r--   0        0        0      146 2023-05-24 09:58:37.360521 django_modshib_certic-0.1.4/modshib/apps.py
--rw-r--r--   0        0        0      400 2023-06-01 08:20:11.702682 django_modshib_certic-0.1.4/modshib/context_processors.py
--rw-r--r--   0        0        0        0 2023-05-19 06:10:59.656283 django_modshib_certic-0.1.4/modshib/migrations/__init__.py
--rw-r--r--   0        0        0       57 2023-05-19 06:10:59.655746 django_modshib_certic-0.1.4/modshib/models.py
--rw-r--r--   0        0        0      896 2023-06-01 14:40:15.254122 django_modshib_certic-0.1.4/modshib/templates/registration/logged_out.html
--rw-r--r--   0        0        0     1334 2023-06-01 08:20:11.703248 django_modshib_certic-0.1.4/modshib/templates/registration/login.html
--rw-r--r--   0        0        0     1012 2023-06-01 08:20:11.704146 django_modshib_certic-0.1.4/modshib/templates/registration/reg_base.html
--rw-r--r--   0        0        0      811 2023-06-01 08:20:11.704836 django_modshib_certic-0.1.4/modshib/templates/registration/sso_fail.html
--rw-r--r--   0        0        0      830 2023-06-01 08:20:11.705098 django_modshib_certic-0.1.4/modshib/templates/registration/sso_no_account.html
--rw-r--r--   0        0        0       60 2023-05-19 06:10:59.655994 django_modshib_certic-0.1.4/modshib/tests.py
--rw-r--r--   0        0        0      117 2023-05-22 09:06:53.828987 django_modshib_certic-0.1.4/modshib/urls.py
--rw-r--r--   0        0        0     2746 2023-06-01 08:20:11.705496 django_modshib_certic-0.1.4/modshib/views.py
--rw-r--r--   0        0        0      550 2023-06-01 14:39:25.560607 django_modshib_certic-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 django_modshib_certic-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.5/modshib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.5/modshib/admin.py
+-rw-r--r--   0        0        0      146 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.5/modshib/apps.py
+-rw-r--r--   0        0        0      400 2023-06-01 08:51:10.568109 django_modshib_certic-0.1.5/modshib/context_processors.py
+-rw-r--r--   0        0        0        0 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.5/modshib/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.5/modshib/models.py
+-rw-r--r--   0        0        0      896 2023-06-02 14:33:23.664664 django_modshib_certic-0.1.5/modshib/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     3065 2023-06-02 15:32:51.152782 django_modshib_certic-0.1.5/modshib/templates/registration/login.html
+-rw-r--r--   0        0        0     1012 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.5/modshib/templates/registration/reg_base.html
+-rw-r--r--   0        0        0      811 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.5/modshib/templates/registration/sso_fail.html
+-rw-r--r--   0        0        0      830 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.5/modshib/templates/registration/sso_no_account.html
+-rw-r--r--   0        0        0       60 2023-05-24 14:07:03.824594 django_modshib_certic-0.1.5/modshib/tests.py
+-rw-r--r--   0        0        0      117 2023-05-24 14:07:03.824594 django_modshib_certic-0.1.5/modshib/urls.py
+-rw-r--r--   0        0        0     2746 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.5/modshib/views.py
+-rw-r--r--   0        0        0      550 2023-06-02 15:33:48.796784 django_modshib_certic-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 django_modshib_certic-0.1.5/PKG-INFO
```

### Comparing `django_modshib_certic-0.1.4/modshib/templates/registration/logged_out.html` & `django_modshib_certic-0.1.5/modshib/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.4/modshib/templates/registration/reg_base.html` & `django_modshib_certic-0.1.5/modshib/templates/registration/reg_base.html`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.4/modshib/templates/registration/sso_fail.html` & `django_modshib_certic-0.1.5/modshib/templates/registration/sso_fail.html`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.4/modshib/templates/registration/sso_no_account.html` & `django_modshib_certic-0.1.5/modshib/templates/registration/sso_no_account.html`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.4/modshib/views.py` & `django_modshib_certic-0.1.5/modshib/views.py`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.4/pyproject.toml` & `django_modshib_certic-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-modshib-CERTIC"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Mickaël Desfrênes <mickael.desfrenes@unicaen.fr>"]
 license = "Cecill-B"
 packages = [
     { include = "modshib"},
 ]
 homepage = "https://www.certic.unicaen.fr"
```

### Comparing `django_modshib_certic-0.1.4/PKG-INFO` & `django_modshib_certic-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-modshib-certic
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Home-page: https://www.certic.unicaen.fr
 License: CECILL-B
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
```

