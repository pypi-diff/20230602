# Comparing `tmp/django-models-logging-2.3.tar.gz` & `tmp/django-models-logging-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-models-logging-2.3.tar", last modified: Thu Apr 27 12:41:45 2023, max compression
+gzip compressed data, was "django-models-logging-2.3.1.tar", last modified: Fri Jun  2 07:22:41 2023, max compression
```

## Comparing `django-models-logging-2.3.tar` & `django-models-logging-2.3.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.889213 django-models-logging-2.3/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1066 2023-04-27 12:40:48.000000 django-models-logging-2.3/LICENSE
--rw-rw-r--   0 legion    (1000) legion    (1000)     1185 2023-04-27 12:41:45.885213 django-models-logging-2.3/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)     3279 2023-04-27 12:40:48.000000 django-models-logging-2.3/README.md
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.885213 django-models-logging-2.3/django_models_logging.egg-info/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1185 2023-04-27 12:41:45.000000 django-models-logging-2.3/django_models_logging.egg-info/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)     1315 2023-04-27 12:41:45.000000 django-models-logging-2.3/django_models_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-04-27 12:41:45.000000 django-models-logging-2.3/django_models_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       28 2023-04-27 12:41:45.000000 django-models-logging-2.3/django_models_logging.egg-info/requires.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       15 2023-04-27 12:41:45.000000 django-models-logging-2.3/django_models_logging.egg-info/top_level.txt
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.885213 django-models-logging-2.3/models_logging/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1880 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     9573 2023-04-27 12:40:50.000000 django-models-logging-2.3/models_logging/admin.py
--rw-rw-r--   0 legion    (1000) legion    (1000)      335 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/apps.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     2864 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/helpers.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.885213 django-models-logging-2.3/models_logging/management/
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.885213 django-models-logging-2.3/models_logging/management/commands/
--rw-rw-r--   0 legion    (1000) legion    (1000)        0 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/management/commands/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     1182 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/management/commands/delete_changes.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     1158 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/middleware.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.885213 django-models-logging-2.3/models_logging/migrations/
--rw-rw-r--   0 legion    (1000) legion    (1000)     3356 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/migrations/0001_initial.py
--rw-rw-r--   0 legion    (1000) legion    (1000)      595 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/migrations/0002_auto_20161012_2025.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     2995 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/migrations/0003_auto_20170726_1552.py
--rw-rw-r--   0 legion    (1000) legion    (1000)      510 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/migrations/0004_auto_20171124_1445.py
--rw-rw-r--   0 legion    (1000) legion    (1000)      945 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/migrations/0005_auto_20200804_1305.py
--rw-rw-r--   0 legion    (1000) legion    (1000)      443 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/migrations/0006_auto_20211020_2036.py
--rw-rw-r--   0 legion    (1000) legion    (1000)      490 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/migrations/0007_migrate_old_fields.py
--rw-rw-r--   0 legion    (1000) legion    (1000)      566 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/migrations/0008_change_extras.py
--rw-rw-r--   0 legion    (1000) legion    (1000)        0 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/migrations/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     6563 2023-04-27 12:40:50.000000 django-models-logging-2.3/models_logging/models.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     1272 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/settings.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     1124 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/setup.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     1333 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/signals.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.885213 django-models-logging-2.3/models_logging/templates/
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.885213 django-models-logging-2.3/models_logging/templates/models_logging/
--rw-rw-r--   0 legion    (1000) legion    (1000)      349 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/templates/models_logging/change_form.html
--rw-rw-r--   0 legion    (1000) legion    (1000)     2824 2023-04-27 12:40:50.000000 django-models-logging-2.3/models_logging/templates/models_logging/object_history.html
--rw-rw-r--   0 legion    (1000) legion    (1000)     1538 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/templates/models_logging/revert_changes_confirmation.html
--rw-rw-r--   0 legion    (1000) legion    (1000)     2167 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/templates/models_logging/revert_revision_confirmation.html
--rw-rw-r--   0 legion    (1000) legion    (1000)     2929 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/utils.py
--rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-04-27 12:41:45.889213 django-models-logging-2.3/setup.cfg
--rw-rw-r--   0 legion    (1000) legion    (1000)     1545 2023-04-27 12:40:50.000000 django-models-logging-2.3/setup.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-02 07:22:41.359576 django-models-logging-2.3.1/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1066 2023-04-27 12:48:57.000000 django-models-logging-2.3.1/LICENSE
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1187 2023-06-02 07:22:41.359576 django-models-logging-2.3.1/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)     3279 2023-04-27 12:48:57.000000 django-models-logging-2.3.1/README.md
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-02 07:22:41.359576 django-models-logging-2.3.1/django_models_logging.egg-info/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1187 2023-06-02 07:22:41.000000 django-models-logging-2.3.1/django_models_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1315 2023-06-02 07:22:41.000000 django-models-logging-2.3.1/django_models_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-02 07:22:41.000000 django-models-logging-2.3.1/django_models_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       28 2023-06-02 07:22:41.000000 django-models-logging-2.3.1/django_models_logging.egg-info/requires.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       15 2023-06-02 07:22:41.000000 django-models-logging-2.3.1/django_models_logging.egg-info/top_level.txt
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-02 07:22:41.359576 django-models-logging-2.3.1/models_logging/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1884 2023-06-02 07:19:20.000000 django-models-logging-2.3.1/models_logging/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     9573 2023-04-27 12:48:57.000000 django-models-logging-2.3.1/models_logging/admin.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)      335 2023-04-27 12:48:57.000000 django-models-logging-2.3.1/models_logging/apps.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2864 2023-04-27 12:48:57.000000 django-models-logging-2.3.1/models_logging/helpers.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-02 07:22:41.359576 django-models-logging-2.3.1/models_logging/management/
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-02 07:22:41.359576 django-models-logging-2.3.1/models_logging/management/commands/
+-rw-rw-r--   0 legion    (1000) legion    (1000)        0 2023-01-05 14:55:39.000000 django-models-logging-2.3.1/models_logging/management/commands/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1182 2023-01-05 14:55:39.000000 django-models-logging-2.3.1/models_logging/management/commands/delete_changes.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1158 2023-04-27 12:48:57.000000 django-models-logging-2.3.1/models_logging/middleware.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-02 07:22:41.359576 django-models-logging-2.3.1/models_logging/migrations/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     3356 2023-01-05 14:55:39.000000 django-models-logging-2.3.1/models_logging/migrations/0001_initial.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)      595 2023-01-05 14:55:39.000000 django-models-logging-2.3.1/models_logging/migrations/0002_auto_20161012_2025.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2995 2023-01-05 14:55:39.000000 django-models-logging-2.3.1/models_logging/migrations/0003_auto_20170726_1552.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)      510 2023-01-05 14:55:39.000000 django-models-logging-2.3.1/models_logging/migrations/0004_auto_20171124_1445.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)      945 2023-04-27 12:48:57.000000 django-models-logging-2.3.1/models_logging/migrations/0005_auto_20200804_1305.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)      443 2023-01-05 14:55:39.000000 django-models-logging-2.3.1/models_logging/migrations/0006_auto_20211020_2036.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)      490 2023-04-27 12:48:57.000000 django-models-logging-2.3.1/models_logging/migrations/0007_migrate_old_fields.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)      566 2023-04-27 12:48:57.000000 django-models-logging-2.3.1/models_logging/migrations/0008_change_extras.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)        0 2023-01-05 14:55:39.000000 django-models-logging-2.3.1/models_logging/migrations/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     6563 2023-04-27 12:48:57.000000 django-models-logging-2.3.1/models_logging/models.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1272 2023-04-27 12:48:57.000000 django-models-logging-2.3.1/models_logging/settings.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1124 2023-04-27 12:48:57.000000 django-models-logging-2.3.1/models_logging/setup.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1333 2023-04-27 12:48:57.000000 django-models-logging-2.3.1/models_logging/signals.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-02 07:22:41.359576 django-models-logging-2.3.1/models_logging/templates/
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-02 07:22:41.359576 django-models-logging-2.3.1/models_logging/templates/models_logging/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      349 2023-01-05 14:55:39.000000 django-models-logging-2.3.1/models_logging/templates/models_logging/change_form.html
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2824 2023-04-27 12:40:50.000000 django-models-logging-2.3.1/models_logging/templates/models_logging/object_history.html
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1538 2023-01-05 14:55:39.000000 django-models-logging-2.3.1/models_logging/templates/models_logging/revert_changes_confirmation.html
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2167 2023-01-05 14:55:39.000000 django-models-logging-2.3.1/models_logging/templates/models_logging/revert_revision_confirmation.html
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2929 2023-04-27 12:48:57.000000 django-models-logging-2.3.1/models_logging/utils.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-02 07:22:41.359576 django-models-logging-2.3.1/setup.cfg
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1547 2023-06-02 07:19:36.000000 django-models-logging-2.3.1/setup.py
```

### Comparing `django-models-logging-2.3/LICENSE` & `django-models-logging-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/PKG-INFO` & `django-models-logging-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-models-logging
-Version: 2.3
+Version: 2.3.1
 Summary: Add logging of models from save, delete signals
 Home-page: https://github.com/legion-an/django-models-logging
 Author: legion
 Author-email: legion.andrey.89@gmail.com
 License: MIT
 Keywords: django logging,django history,django logging models,django history models
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-models-logging-2.3/README.md` & `django-models-logging-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/django_models_logging.egg-info/PKG-INFO` & `django-models-logging-2.3.1/django_models_logging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-models-logging
-Version: 2.3
+Version: 2.3.1
 Summary: Add logging of models from save, delete signals
 Home-page: https://github.com/legion-an/django-models-logging
 Author: legion
 Author-email: legion.andrey.89@gmail.com
 License: MIT
 Keywords: django logging,django history,django logging models,django history models
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-models-logging-2.3/django_models_logging.egg-info/SOURCES.txt` & `django-models-logging-2.3.1/django_models_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/__init__.py` & `django-models-logging-2.3.1/models_logging/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     @property
     def user_id(self):
         if self.request:
             from models_logging.models import Change
 
             user = self.request.user
-            return user.pk if user and type(user) == Change.user_field_model() and user.is_authenticated else None
+            return user.pk if user and isinstance(user, Change.user_field_model()) and user.is_authenticated else None
 
     def put_change_to_stack(self, change: "Change"):
         key = (change.object_id, change.content_type.pk)
         existing_change = self.stack_changes.get(key)
         if existing_change:
             # If the object changes several times during the request, we need to properly track the changed fields
             for k, v in change.changed_data.items():
```

### Comparing `django-models-logging-2.3/models_logging/admin.py` & `django-models-logging-2.3.1/models_logging/admin.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/helpers.py` & `django-models-logging-2.3.1/models_logging/helpers.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/management/commands/delete_changes.py` & `django-models-logging-2.3.1/models_logging/management/commands/delete_changes.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/middleware.py` & `django-models-logging-2.3.1/models_logging/middleware.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/migrations/0001_initial.py` & `django-models-logging-2.3.1/models_logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/migrations/0002_auto_20161012_2025.py` & `django-models-logging-2.3.1/models_logging/migrations/0002_auto_20161012_2025.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/migrations/0003_auto_20170726_1552.py` & `django-models-logging-2.3.1/models_logging/migrations/0003_auto_20170726_1552.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/migrations/0005_auto_20200804_1305.py` & `django-models-logging-2.3.1/models_logging/migrations/0005_auto_20200804_1305.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/migrations/0008_change_extras.py` & `django-models-logging-2.3.1/models_logging/migrations/0008_change_extras.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/models.py` & `django-models-logging-2.3.1/models_logging/models.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/settings.py` & `django-models-logging-2.3.1/models_logging/settings.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/setup.py` & `django-models-logging-2.3.1/models_logging/setup.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/signals.py` & `django-models-logging-2.3.1/models_logging/signals.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/templates/models_logging/object_history.html` & `django-models-logging-2.3.1/models_logging/templates/models_logging/object_history.html`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/templates/models_logging/revert_changes_confirmation.html` & `django-models-logging-2.3.1/models_logging/templates/models_logging/revert_changes_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/templates/models_logging/revert_revision_confirmation.html` & `django-models-logging-2.3.1/models_logging/templates/models_logging/revert_revision_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/models_logging/utils.py` & `django-models-logging-2.3.1/models_logging/utils.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.3/setup.py` & `django-models-logging-2.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 files = ["templates/models_logging/*", "migrations/*", "management/commands/*"]
 
 setup(
     name='django-models-logging',
-    version='2.3',
+    version='2.3.1',
     packages=['models_logging'],
     url='https://github.com/legion-an/django-models-logging',
     package_data={'models_logging' : files},
     license='MIT',
     author='legion',
     author_email='legion.andrey.89@gmail.com',
     description='Add logging of models from save, delete signals',
```

