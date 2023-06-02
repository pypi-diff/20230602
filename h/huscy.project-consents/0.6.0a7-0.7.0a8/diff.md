# Comparing `tmp/huscy.project_consents-0.6.0a7.tar.gz` & `tmp/huscy.project_consents-0.7.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.project_consents-0.6.0a7.tar", last modified: Thu May 11 13:50:56 2023, max compression
+gzip compressed data, was "huscy.project_consents-0.7.0a8.tar", last modified: Fri Jun  2 13:46:39 2023, max compression
```

## Comparing `huscy.project_consents-0.6.0a7.tar` & `huscy.project_consents-0.7.0a8.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.104585 huscy.project_consents-0.6.0a7/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)    34523 2022-12-05 12:04:00.000000 huscy.project_consents-0.6.0a7/LICENSE
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       39 2023-04-27 11:26:24.000000 huscy.project_consents-0.6.0a7/MANIFEST.in
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-05-11 13:50:56.104585 huscy.project_consents-0.6.0a7/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       19 2022-09-12 13:32:12.000000 huscy.project_consents-0.6.0a7/README.md
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.100585 huscy.project_consents-0.6.0a7/huscy/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.104585 huscy.project_consents-0.6.0a7/huscy/project_consents/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       81 2023-05-11 13:50:39.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      749 2023-05-11 13:50:39.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/admin.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      479 2023-04-21 13:33:05.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/api_urls.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      194 2022-12-05 12:04:00.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/apps.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1007 2023-04-27 11:26:24.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/forms.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.104585 huscy.project_consents-0.6.0a7/huscy/project_consents/migrations/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     3630 2023-05-11 13:50:53.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/migrations/0001_initial.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2022-12-08 10:36:34.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/migrations/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     2352 2023-05-11 13:50:39.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/models.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1304 2023-01-30 14:04:08.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1171 2023-01-24 10:55:08.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/services.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.100585 huscy.project_consents-0.6.0a7/huscy/project_consents/templates/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.104585 huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/
--rw-r--r--   0 lotus     (1000) lotus     (1000)    20480 2023-05-11 09:49:55.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/.project_consent.html.swp
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     6513 2023-05-11 13:50:39.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/project_consent.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      737 2023-04-27 11:26:24.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/projectconsenttoken.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      379 2023-05-11 13:50:39.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/sign_project_consent.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      608 2023-05-11 13:50:39.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/signed_project_consent.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      430 2023-04-27 11:26:24.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/urls.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     4427 2023-05-11 13:50:39.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/views.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1527 2023-01-13 21:29:30.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/viewsets.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.100585 huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-05-11 13:50:56.000000 huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1221 2023-05-11 13:50:56.000000 huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/SOURCES.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2023-05-11 13:50:56.000000 huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/dependency_links.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      115 2023-05-11 13:50:56.000000 huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/requires.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        6 2023-05-11 13:50:56.000000 huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/top_level.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2023-05-11 13:50:56.104585 huscy.project_consents-0.6.0a7/setup.cfg
--rwxrwxr-x   0 lotus     (1000) lotus     (1000)     1673 2023-04-27 11:26:24.000000 huscy.project_consents-0.6.0a7/setup.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.104585 huscy.project_consents-0.6.0a7/tests/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      760 2023-01-30 14:04:08.000000 huscy.project_consents-0.6.0a7/tests/test_project_consent_category_serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      684 2023-01-30 14:04:08.000000 huscy.project_consents-0.6.0a7/tests/test_project_consent_serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     5532 2023-01-24 10:55:08.000000 huscy.project_consents-0.6.0a7/tests/test_viewsets.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-02 13:46:39.001817 huscy.project_consents-0.7.0a8/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    34523 2022-12-08 10:33:28.000000 huscy.project_consents-0.7.0a8/LICENSE
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       39 2023-04-25 13:22:38.000000 huscy.project_consents-0.7.0a8/MANIFEST.in
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1098 2023-06-02 13:46:39.001817 huscy.project_consents-0.7.0a8/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       19 2022-12-08 10:33:28.000000 huscy.project_consents-0.7.0a8/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-02 13:46:38.993817 huscy.project_consents-0.7.0a8/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-02 13:46:38.997817 huscy.project_consents-0.7.0a8/huscy/project_consents/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       81 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      749 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      479 2023-01-13 15:29:15.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      194 2022-12-08 10:33:28.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/apps.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1007 2023-04-25 13:22:38.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/forms.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-02 13:46:38.997817 huscy.project_consents-0.7.0a8/huscy/project_consents/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3678 2023-06-02 13:46:38.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-12-08 10:34:52.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1690 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1215 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1923 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/services.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-02 13:46:38.993817 huscy.project_consents-0.7.0a8/huscy/project_consents/templates/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-02 13:46:38.997817 huscy.project_consents-0.7.0a8/huscy/project_consents/templates/project_consents/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     6710 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/templates/project_consents/project_consent.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      737 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/templates/project_consents/project_consent_token.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      379 2023-05-11 13:38:27.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/templates/project_consents/sign_project_consent.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      870 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/templates/project_consents/signed_project_consent.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      287 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4647 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/views.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1527 2023-01-13 15:29:15.000000 huscy.project_consents-0.7.0a8/huscy/project_consents/viewsets.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-02 13:46:38.997817 huscy.project_consents-0.7.0a8/huscy.project_consents.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1098 2023-06-02 13:46:38.000000 huscy.project_consents-0.7.0a8/huscy.project_consents.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1188 2023-06-02 13:46:38.000000 huscy.project_consents-0.7.0a8/huscy.project_consents.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-06-02 13:46:38.000000 huscy.project_consents-0.7.0a8/huscy.project_consents.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      115 2023-06-02 13:46:38.000000 huscy.project_consents-0.7.0a8/huscy.project_consents.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-06-02 13:46:38.000000 huscy.project_consents-0.7.0a8/huscy.project_consents.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-06-02 13:46:39.001817 huscy.project_consents-0.7.0a8/setup.cfg
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     1673 2023-04-25 13:22:38.000000 huscy.project_consents-0.7.0a8/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-02 13:46:39.001817 huscy.project_consents-0.7.0a8/tests/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      440 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.0a8/tests/test_admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      592 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.0a8/tests/test_models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      760 2023-01-30 13:08:18.000000 huscy.project_consents-0.7.0a8/tests/test_project_consent_category_serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      625 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.0a8/tests/test_project_consent_serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     5522 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.0a8/tests/test_viewsets.py
```

### Comparing `huscy.project_consents-0.6.0a7/LICENSE` & `huscy.project_consents-0.7.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.6.0a7/PKG-INFO` & `huscy.project_consents-0.7.0a8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: huscy.project_consents
-Version: 0.6.0a7
+Version: 0.7.0a8
 Summary: projects_consents
 Home-page: https://bitbucket.org/huscy/project_consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
+Description: # project consents
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -20,12 +22,7 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
-License-File: LICENSE
-
-# project consents
-
-
```

### Comparing `huscy.project_consents-0.6.0a7/huscy/project_consents/admin.py` & `huscy.project_consents-0.7.0a8/huscy/project_consents/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class ContactPersonAdmin(admin.ModelAdmin):
     list_display = 'project', 'user', 'email', 'phone'
 
 
 class ProjectConsentAdmin(admin.ModelAdmin):
-    list_display = 'id', '_project', 'consent'
+    list_display = 'id', '_project', 'version'
 
     def _project(self, project_consent):
         return project_consent.project.title
 
 
 class ProjectConsentTokenAdmin(admin.ModelAdmin):
     list_display = 'id', 'project', 'subject', 'created_at'
```

### Comparing `huscy.project_consents-0.6.0a7/huscy/project_consents/forms.py` & `huscy.project_consents-0.7.0a8/huscy/project_consents/forms.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.6.0a7/huscy/project_consents/migrations/0001_initial.py` & `huscy.project_consents-0.7.0a8/huscy/project_consents/migrations/0001_initial.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,77 @@
-# Generated by Django 4.2 on 2023-05-11 13:50
-
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import huscy.project_consents.models
 import phonenumber_field.modelfields
 import uuid
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ('consents', '0001_initial'),
-        ('projects', '0002_alter_membership_options'),
         ('subjects', '0001_squashed_0009_delete_contactold'),
+        ('projects', '0003_project_project_manager_and_more'),
     ]
 
     operations = [
         migrations.CreateModel(
             name='ProjectConsent',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('consent', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, to='consents.consent')),
+                ('text_fragments', models.JSONField()),
+                ('version', models.PositiveIntegerField(default=1)),
                 ('project', models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, to='projects.project')),
             ],
+            options={
+                'abstract': False,
+            },
+        ),
+        migrations.CreateModel(
+            name='ProjectConsentCategory',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=128)),
+                ('template_text_fragments', models.JSONField()),
+            ],
+            options={
+                'abstract': False,
+            },
         ),
         migrations.CreateModel(
             name='ProjectConsentToken',
             fields=[
                 ('id', models.UUIDField(default=uuid.uuid4, primary_key=True, serialize=False)),
                 ('created_at', models.DateTimeField(auto_now_add=True)),
                 ('created_by', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
                 ('project', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='projects.project')),
                 ('subject', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='subjects.subject')),
             ],
         ),
         migrations.CreateModel(
-            name='ProjectConsentCategory',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('consent_category', models.OneToOneField(on_delete=django.db.models.deletion.PROTECT, to='consents.consentcategory')),
-            ],
-        ),
-        migrations.CreateModel(
             name='ContactPerson',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('email', models.EmailField(blank=True, max_length=254, null=True)),
                 ('phone', phonenumber_field.modelfields.PhoneNumberField(blank=True, max_length=128, null=True, region=None)),
                 ('project', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='projects.project')),
                 ('user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
             ],
         ),
         migrations.CreateModel(
             name='ProjectConsentFile',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('consent_version', models.PositiveIntegerField(default=1)),
-                ('filehandle', models.FileField(upload_to=huscy.project_consents.models.get_consent_file_upload_path)),
+                ('consent_version', models.PositiveIntegerField()),
                 ('created_at', models.DateTimeField(auto_now_add=True)),
-                ('project_consent', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='project_consents.projectconsent')),
+                ('filehandle', models.FileField(upload_to=huscy.project_consents.models.get_project_consent_file_upload_path)),
+                ('consent', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='project_consents.projectconsent')),
                 ('subject', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='subjects.subject')),
             ],
             options={
-                'unique_together': {('project_consent', 'subject', 'consent_version')},
+                'unique_together': {('consent', 'subject', 'consent_version')},
             },
         ),
     ]
```

### Comparing `huscy.project_consents-0.6.0a7/huscy/project_consents/serializer.py` & `huscy.project_consents-0.7.0a8/huscy/project_consents/serializer.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,17 @@
         return create_project_consent_category(**validated_data)
 
     def update(self, project_consent_category, validated_data):
         return update_project_consent_category(project_consent_category, **validated_data)
 
 
 class ProjectConsentSerializer(serializers.ModelSerializer):
-    name = serializers.CharField()
-    text_fragments = serializers.JSONField()
-
     class Meta:
         model = ProjectConsent
-        fields = 'id', 'name', 'project', 'text_fragments'
+        fields = 'id', 'project', 'text_fragments'
         read_only_fields = 'project',
 
     def create(self, validated_data):
         return create_project_consent(**validated_data)
 
     def update(self, project_consent, validated_data):
         return update_project_consent(project_consent, **validated_data)
```

### Comparing `huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/project_consent.html` & `huscy.project_consents-0.7.0a8/huscy/project_consents/templates/project_consents/project_consent.html`

 * *Files 2% similar despite different names*

```diff
@@ -73,69 +73,75 @@
             </p>
 
             {% for text_fragment in consent.text_fragments %}
             {% with template_name="consents/text_fragments/"|add:text_fragment.type|add:".html" %}
             {% include template_name with index=forloop.counter0 %}
             {% endwith %}
             {% endfor %}
+
+            <p class="bigskip">
+                Eine Weitergabe, Speicherung, Auswertung und Nutzung der bei wissenschaftlichen Studien erhobenen Daten erfolgt nach gesetzlichen Bestimmungen und setzt vor Teilnahme an der Studie die folgenden freiwilligen Einwilligungen voraus:
+            </p>
         </div>
 
         <div class="page new_page">
             <form method="post">
                 {% csrf_token %}
                 <input type="hidden" name="form-TOTAL_FORMS" value="2">
                 <input type="hidden" name="form-INITIAL_FORMS" value="0">
 
-                Eine Weitergabe, Speicherung, Auswertung und Nutzung der bei wissenschaftlichen Studien erhobenen Daten erfolgt nach gesetzlichen Bestimmungen und setzt vor Teilnahme an der Studie die folgenden freiwilligen Einwilligungen voraus:
-
                 <h2>Einwilligungserklärung zur Teilnahme an der Studie</h2>
                 <h2>{{ project.title }}</h2>
 
                 <ol>
                     <li>Ich wurde über die Studie und deren Wesen, Bedeutung, Tragweite und Risiken aufgeklärt und habe diese Informationen gelesen und verstanden.</li>
                     <li>Mir wurde ausreichend Gelegenheit gegeben, alle offenen Fragen zu klären.</li>
                     <li>Ich habe jederzeit das Recht, weitere Informationen zur Studie zu erfragen.</li>
                     <li>Ich erkläre mich freiwillig bereit, an der Studie teilzunehmen.</li>
                     <li>Ich wurde darauf hingewiesen, dass ich jederzeit von dieser Studienteilnahme zurücktreten kann, ohne dass mir dadurch ein Nachteil entsteht.</li>
                     <li>Eine Ausfertigung der <b>Studieninformation und Einwilligungserklärung</b> habe ich erhalten.</li>
                     <li>Die <b>Erklärungen zum Datenschutz</b> habe ich gelesen und stimme diesen zu.</li>
                     <li>Die Erklärungen zu Zufallsfunden habe ich gelesen und stimme diesen zu.</li>
                 </ol>
 
-                <div class="table-row" style="margin-top: 1.5cm;">
+                <div class="table-row" style="margin-top: 1.2cm;">
                     <div class="table-cell">
                         Versuchsleiter/in:<br>
                         {{ experimenter.get_full_name }}<br><br><br>
                         Leipzig, den {% now "SHORT_DATE_FORMAT" %}
                     </div>
                     <div class="table-cell">
                         Unterschrift Versuchsleiter/in:
                         {% block signature_experimenter %}{{ form.0.signature }}{% endblock signature_experimenter %}
                     </div>
                 </div>
 
-                <div class="table-row" style="margin-top: 1.5cm;">
+                <div class="table-row" style="margin-top: 1.0cm;">
                     <div class="table-cell">
                         Studienteilnehmer/in:<br>
                         {{ subject.contact.display_name }}<br><br>
                         Geburtsdatum:<br>
                         {{ subject.contact.date_of_birth }}<br><br><br>
                         Leipzig, den {% now "SHORT_DATE_FORMAT" %}
                     </div>
                     <div class="table-cell">
                         Unterschrift Studienteilnehmer/in oder gesetzliche/r Vertreter/in*:
                         {% block signature_subject %}{{ form.1.signature }}{% endblock signature_subject %}
                     </div>
                 </div>
 
-                <b>* bei minderjährigen Studienteilnehmer*innen:</b> Als Sorgeberechtigte*r bzw. gesetzliche*r Vertreter*in eines*r minderjährigen Studienteilnehmers*in versichere ich, dass ich auch im Namen des*der zweiten Sorgeberechtigten handle oder alleine sorgeberechtigt bin.
+                <p class="bigskip">
+                    <b>* bei minderjährigen Studienteilnehmer*innen:</b> Als Sorgeberechtigte*r bzw. gesetzliche*r Vertreter*in eines*r minderjährigen Studienteilnehmers*in versichere ich, dass ich auch im Namen des*der zweiten Sorgeberechtigten handle oder alleine sorgeberechtigt bin.
+                </p>
 
+                {% block submit_button %}
                 <div>
                     <button>submit</button>
                 </div>
+                {% endblock submit_button %}
             </form>
         </div>
 
         <script src="{% static 'consents/js/popper.min.js' %}"></script>
         {{ form.media }}
     </body>
 </html>
```

#### html2text {}

```diff
@@ -21,18 +21,18 @@
 { subject.contact.display_name }}, {% elif subject.contact.gender == 1 %} Sehr
 geehrter {{ subject.contact.display_name }}, {% else %} Hallo {
 { subject.contact.display_name }}, {% endif %}
 {% for text_fragment in consent.text_fragments %} {% with
 template_name="consents/text_fragments/"|add:text_fragment.type|add:".html" %}
 {% include template_name with index=forloop.counter0 %} {% endwith %} {% endfor
 %}
-{% csrf_token %}   Eine Weitergabe, Speicherung, Auswertung und Nutzung der bei
-wissenschaftlichen Studien erhobenen Daten erfolgt nach gesetzlichen
-Bestimmungen und setzt vor Teilnahme an der Studie die folgenden freiwilligen
-Einwilligungen voraus:
+Eine Weitergabe, Speicherung, Auswertung und Nutzung der bei wissenschaftlichen
+Studien erhobenen Daten erfolgt nach gesetzlichen Bestimmungen und setzt vor
+Teilnahme an der Studie die folgenden freiwilligen Einwilligungen voraus:
+{% csrf_token %}
 ***** EinwilligungserklÃ¤rung zur Teilnahme an der Studie *****
 ***** {{ project.title }} *****
    1. Ich wurde Ã¼ber die Studie und deren Wesen, Bedeutung, Tragweite und
       Risiken aufgeklÃ¤rt und habe diese Informationen gelesen und verstanden.
    2. Mir wurde ausreichend Gelegenheit gegeben, alle offenen Fragen zu
       klÃ¤ren.
    3. Ich habe jederzeit das Recht, weitere Informationen zur Studie zu
@@ -62,9 +62,11 @@
 Leipzig, den {% now "SHORT_DATE_FORMAT" %}
 Unterschrift Studienteilnehmer/in oder gesetzliche/r Vertreter/in*: {% block
 signature_subject %}{{ form.1.signature }}{% endblock signature_subject %}
 * bei minderjÃ¤hrigen Studienteilnehmer*innen: Als Sorgeberechtigte*r bzw.
 gesetzliche*r Vertreter*in eines*r minderjÃ¤hrigen Studienteilnehmers*in
 versichere ich, dass ich auch im Namen des*der zweiten Sorgeberechtigten handle
 oder alleine sorgeberechtigt bin.
+{% block submit_button %}
 submit
+{% endblock submit_button %}
  {{ form.media }}
```

### Comparing `huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/projectconsenttoken.html` & `huscy.project_consents-0.7.0a8/huscy/project_consents/templates/project_consents/project_consent_token.html`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.6.0a7/huscy/project_consents/views.py` & `huscy.project_consents-0.7.0a8/huscy/project_consents/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,50 @@
+import re
+import string
+import unicodedata
+
 from django.core.files.uploadedfile import SimpleUploadedFile
-from django.db import transaction
+from django.contrib.auth.mixins import LoginRequiredMixin
 from django.forms import formset_factory
 from django.http import HttpResponse, HttpResponseRedirect
 from django.shortcuts import get_object_or_404
 from django.template.loader import get_template
 from django.urls import reverse
 from django.views import generic
 from weasyprint import HTML
 
-from huscy.consents.models import Consent
 from huscy.consents.forms import SignatureForm
-from huscy.consents.views import CreateConsentView, SignConsentView
+from huscy.consents.views import SignConsentView
 from huscy.project_consents.forms import TokenForm
-from huscy.project_consents.models import ProjectConsent, ProjectConsentFile, ProjectConsentToken
-from huscy.projects.models import Project
+from huscy.project_consents.models import ProjectConsentFile, ProjectConsentToken
 
 
-class CreateProjectConsentView(CreateConsentView):
+def sanitize_string(_string):
+    # replace umlauts
+    _string = re.sub('[ä]', 'ae', _string)
+    _string = re.sub('[Ä]', 'Ae', _string)
+    _string = re.sub('[ö]', 'oe', _string)
+    _string = re.sub('[Ö]', 'Oe', _string)
+    _string = re.sub('[ü]', 'ue', _string)
+    _string = re.sub('[Ü]', 'Ue', _string)
+    _string = re.sub('[ß]', 'ss', _string)
 
-    def dispatch(self, request, *args, **kwargs):
-        self.project = get_object_or_404(Project, pk=self.kwargs['project_id'])
-        return super().dispatch(request, *args, **kwargs)
+    # remove accents
+    _string = ''.join(c for c in unicodedata.normalize('NFKD', _string)
+                      if not unicodedata.combining(c))
 
-    @transaction.atomic
-    def post(self, request, *args, **kwargs):
-        response = super().post(self, request, *args, **kwargs)
-        consent = Consent.objects.latest('id')
-        ProjectConsent.objects.create(consent=consent, project=self.project)
-        return response
+    # remove punctuation
+    _string = _string.translate(str.maketrans('', '', string.punctuation))
 
-    def get_success_url(self):
-        return reverse('consent-created')
+    return _string
 
 
-class CreateTokenView(generic.FormView):
+class CreateTokenView(LoginRequiredMixin, generic.FormView):
     form_class = TokenForm
-    template_name = 'project_consents/projectconsenttoken.html'
+    template_name = 'project_consents/project_consent_token.html'
 
     def get_form_kwargs(self):
         form_kwargs = super().get_form_kwargs()
         form_kwargs['user'] = self.request.user
         return form_kwargs
 
     def form_valid(self, form):
@@ -52,58 +57,68 @@
             '{}?token={}'.format(reverse('create-project-consent-token'), token.id)
         )
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         if 'token' in self.request.GET:
             token = get_object_or_404(ProjectConsentToken, pk=self.request.GET.get('token'))
-            context['sign_project_consent_url'] = '{protocol}://{host}{url}'.format(
-                protocol=self.request.scheme,
-                host=self.request.get_host(),
-                url=reverse('sign-project-consent', kwargs=dict(token=token.id))
-            )
+
+            protocol = self.request.scheme,
+            host = self.request.get_host(),
+            url = reverse('sign-project-consent', kwargs=dict(token=token.id))
+
+            context['sign_project_consent_url'] = f'{protocol}://{host}{url}'
         return context
 
 
 class SignProjectConsentView(SignConsentView):
     form_class = formset_factory(SignatureForm, extra=2)
     template_name = 'project_consents/sign_project_consent.html'
 
     def dispatch(self, request, *args, **kwargs):
         self.token = get_object_or_404(ProjectConsentToken, pk=self.kwargs['token'])
-        self.consent = self.token.project.projectconsent.consent  # required by parent class
+        self.project = self.token.project
+        self.subject = self.token.subject
+        self.consent = self.project.projectconsent  # required by parent class
         return super(SignConsentView, self).dispatch(request, *args, **kwargs)
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context['experimenter'] = self.token.created_by
-        context['project'] = self.token.project
-        context['subject'] = self.token.subject
+        context['project'] = self.project
+        context['subject'] = self.subject
         return context
 
     def form_valid(self, form):
         html_template = get_template('project_consents/signed_project_consent.html')
 
         custom_data = dict((key, value)
                            for key, value in self.request.POST.items()
                            if key.startswith('textfragment'))
         rendered_html = html_template.render({
             'consent': self.consent,
             'custom_data': custom_data,
             'experimenter': self.token.created_by,
             'form': form,
-            'subject': self.token.subject,
+            'project': self.project,
+            'subject': self.subject,
         })
         content = HTML(string=rendered_html, base_url=self.request.build_absolute_uri()).write_pdf()
+
+        filename = '_'.join([
+            *sanitize_string(self.subject.contact.display_name).split(),
+            self.subject.contact.date_of_birth.strftime("%Y%m%d")
+        ]) + '.pdf'
         filehandle = SimpleUploadedFile(
-            name='filehandle',
+            name=filename,
             content=content,
             content_type='application/pdf'
         )
         ProjectConsentFile.objects.create(
+            consent=self.consent,
             consent_version=self.consent.version,
             filehandle=filehandle,
-            project_consent=self.token.project.projectconsent,
-            subject=self.token.subject
+            subject=self.subject
         )
         self.token.delete()
+
         return HttpResponse(content, content_type="application/pdf")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `huscy.project_consents-0.6.0a7/huscy/project_consents/viewsets.py` & `huscy.project_consents-0.7.0a8/huscy/project_consents/viewsets.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/PKG-INFO` & `huscy.project_consents-0.7.0a8/huscy.project_consents.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: huscy.project-consents
-Version: 0.6.0a7
+Version: 0.7.0a8
 Summary: projects_consents
 Home-page: https://bitbucket.org/huscy/project_consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
+Description: # project consents
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -20,12 +22,7 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
-License-File: LICENSE
-
-# project consents
-
-
```

### Comparing `huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/SOURCES.txt` & `huscy.project_consents-0.7.0a8/huscy.project_consents.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 huscy/project_consents/serializer.py
 huscy/project_consents/services.py
 huscy/project_consents/urls.py
 huscy/project_consents/views.py
 huscy/project_consents/viewsets.py
 huscy/project_consents/migrations/0001_initial.py
 huscy/project_consents/migrations/__init__.py
-huscy/project_consents/templates/project_consents/.project_consent.html.swp
 huscy/project_consents/templates/project_consents/project_consent.html
-huscy/project_consents/templates/project_consents/projectconsenttoken.html
+huscy/project_consents/templates/project_consents/project_consent_token.html
 huscy/project_consents/templates/project_consents/sign_project_consent.html
 huscy/project_consents/templates/project_consents/signed_project_consent.html
+tests/test_admin.py
+tests/test_models.py
 tests/test_project_consent_category_serializer.py
 tests/test_project_consent_serializer.py
 tests/test_viewsets.py
```

### Comparing `huscy.project_consents-0.6.0a7/setup.py` & `huscy.project_consents-0.7.0a8/setup.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.6.0a7/tests/test_project_consent_category_serializer.py` & `huscy.project_consents-0.7.0a8/tests/test_project_consent_category_serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.6.0a7/tests/test_project_consent_serializer.py` & `huscy.project_consents-0.7.0a8/tests/test_project_consent_serializer.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 from huscy.project_consents.serializer import ProjectConsentSerializer
 
 pytestmark = pytest.mark.django_db
 
 
 def test_project_consent_serializer_input_data(text_fragments):
-    data = dict(name='consent name', text_fragments=text_fragments)
+    data = dict(text_fragments=text_fragments)
     serializer = ProjectConsentSerializer(data=data)
     assert serializer.is_valid()
 
 
 def test_project_consent_serializer_output_data(project_consent):
     serializer = ProjectConsentSerializer(project_consent)
     assert serializer.data == {
         "id": project_consent.id,
-        "name": project_consent.name,
         "project": project_consent.project.id,
         "text_fragments": project_consent.text_fragments,
     }
```

### Comparing `huscy.project_consents-0.6.0a7/tests/test_viewsets.py` & `huscy.project_consents-0.7.0a8/tests/test_viewsets.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     create_membership(project, user)
 
 
 @when('I try to create a project consent', target_fixture='request_result')
 def create_project_consent(client, project, paragraph):
     return client.post(
         reverse('projectconsent-list', kwargs=dict(project_pk=project.pk)),
-        data=dict(name='consent name', text_fragments=[paragraph]),
+        data=dict(text_fragments=[paragraph]),
         format='json'
     )
 
 
 @when('I try to create a project consent category', target_fixture='request_result')
 def create_project_consent_category(client, text_fragments):
     return client.post(
@@ -99,26 +99,27 @@
 
 
 @when('I try to list project consent categories', target_fixture='request_result')
 def list_project_consent_categories(client):
     return client.get(reverse('projectconsentcategory-list'))
 
 
-@when('I try to partial update a project consent', target_fixture='request_result')
-def partial_update_project_consent(client, project, project_consent):
+@when('I try to patch a project consent category', target_fixture='request_result')
+def partial_update_project_consent_category(client, project_consent_category):
     return client.patch(
-        reverse('projectconsent-detail', kwargs=dict(project_pk=project.pk, pk=project_consent.pk)),
-        data=dict(name='new consent name')
+        reverse('projectconsentcategory-detail', kwargs=dict(pk=project_consent_category.pk))
     )
 
 
-@when('I try to patch a project consent category', target_fixture='request_result')
-def patch_project_consent_category(client, project_consent_category):
+@when('I try to partial update a project consent', target_fixture='request_result')
+def partial_update_project_consent(client, project, project_consent, checkbox):
     return client.patch(
-        reverse('projectconsentcategory-detail', kwargs=dict(pk=project_consent_category.pk))
+        reverse('projectconsent-detail', kwargs=dict(project_pk=project.pk, pk=project_consent.pk)),
+        data=dict(text_fragments=[checkbox]),
+        format='json'
     )
 
 
 @when('I try to retrieve a project consent', target_fixture='request_result')
 def retrieve_project_consent(client, project, project_consent):
     return client.get(
         reverse('projectconsent-detail', kwargs=dict(project_pk=project.pk, pk=project_consent.pk))
@@ -129,18 +130,18 @@
 def retrieve_project_consent_category(client, project_consent_category):
     return client.get(
         reverse('projectconsentcategory-detail', kwargs=dict(pk=project_consent_category.pk))
     )
 
 
 @when('I try to update a project consent', target_fixture='request_result')
-def update_project_consent(client, project, project_consent):
+def update_project_consent(client, project, project_consent, paragraph):
     return client.put(
         reverse('projectconsent-detail', kwargs=dict(project_pk=project.pk, pk=project_consent.pk)),
-        data=dict(name='new consent name', text_fragments=project_consent.text_fragments),
+        data=dict(text_fragments=[paragraph]),
         format='json'
     )
 
 
 @when('I try to update a project consent category', target_fixture='request_result')
 def update_project_consent_category(client, project_consent_category):
     return client.put(
```

