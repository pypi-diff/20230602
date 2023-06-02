# Comparing `tmp/django-proemail-template-0.1.9.tar.gz` & `tmp/django-proemail-template-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-proemail-template-0.1.9.tar", last modified: Tue Apr  5 14:13:52 2022, max compression
+gzip compressed data, was "django-proemail-template-0.2.0.tar", last modified: Fri Jun  2 16:19:26 2023, max compression
```

## Comparing `django-proemail-template-0.1.9.tar` & `django-proemail-template-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 teppss     (501) staff       (20)        0 2022-04-05 14:13:52.871744 django-proemail-template-0.1.9/
-drwxr-xr-x   0 teppss     (501) staff       (20)        0 2022-04-05 14:13:52.870109 django-proemail-template-0.1.9/EmailTemplate/
--rw-r--r--   0 teppss     (501) staff       (20)        0 2022-04-05 14:10:09.000000 django-proemail-template-0.1.9/EmailTemplate/__init__.py
--rw-r--r--   0 teppss     (501) staff       (20)      390 2022-04-05 14:12:50.000000 django-proemail-template-0.1.9/EmailTemplate/admin.py
-drwxr-xr-x   0 teppss     (501) staff       (20)        0 2022-04-05 14:13:52.871080 django-proemail-template-0.1.9/EmailTemplate/migrations/
--rw-r--r--   0 teppss     (501) staff       (20)     1232 2022-04-05 14:05:32.000000 django-proemail-template-0.1.9/EmailTemplate/migrations/0001_initial.py
--rw-r--r--   0 teppss     (501) staff       (20)      445 2022-04-05 14:05:32.000000 django-proemail-template-0.1.9/EmailTemplate/migrations/0002_auto_20190719_1354.py
--rw-r--r--   0 teppss     (501) staff       (20)      482 2022-04-05 14:05:32.000000 django-proemail-template-0.1.9/EmailTemplate/migrations/0003_auto_20190719_1358.py
--rw-r--r--   0 teppss     (501) staff       (20)      445 2022-04-05 14:05:32.000000 django-proemail-template-0.1.9/EmailTemplate/migrations/0004_auto_20210226_0911.py
--rw-r--r--   0 teppss     (501) staff       (20)      637 2022-04-05 14:12:58.000000 django-proemail-template-0.1.9/EmailTemplate/migrations/0005_emailtemplate_bcc_emailtemplate_cc.py
--rw-r--r--   0 teppss     (501) staff       (20)        0 2022-04-05 14:05:32.000000 django-proemail-template-0.1.9/EmailTemplate/migrations/__init__.py
--rw-r--r--   0 teppss     (501) staff       (20)     3334 2022-04-05 14:11:16.000000 django-proemail-template-0.1.9/EmailTemplate/models.py
--rw-r--r--   0 teppss     (501) staff       (20)      449 2021-02-26 09:04:46.000000 django-proemail-template-0.1.9/EmailTemplate/tests.py
--rw-r--r--   0 teppss     (501) staff       (20)       63 2018-11-14 15:29:47.000000 django-proemail-template-0.1.9/EmailTemplate/views.py
--rw-r--r--   0 teppss     (501) staff       (20)     1065 2019-07-12 02:22:08.000000 django-proemail-template-0.1.9/LICENSE
--rw-r--r--   0 teppss     (501) staff       (20)       60 2019-07-12 02:22:08.000000 django-proemail-template-0.1.9/MANIFEST.in
--rw-r--r--   0 teppss     (501) staff       (20)     1803 2022-04-05 14:13:52.871624 django-proemail-template-0.1.9/PKG-INFO
--rw-r--r--   0 teppss     (501) staff       (20)      979 2020-02-01 09:44:20.000000 django-proemail-template-0.1.9/README.rst
-drwxr-xr-x   0 teppss     (501) staff       (20)        0 2022-04-05 14:13:52.871474 django-proemail-template-0.1.9/django_proemail_template.egg-info/
--rw-r--r--   0 teppss     (501) staff       (20)     1803 2022-04-05 14:13:52.000000 django-proemail-template-0.1.9/django_proemail_template.egg-info/PKG-INFO
--rw-r--r--   0 teppss     (501) staff       (20)      652 2022-04-05 14:13:52.000000 django-proemail-template-0.1.9/django_proemail_template.egg-info/SOURCES.txt
--rw-r--r--   0 teppss     (501) staff       (20)        1 2022-04-05 14:13:52.000000 django-proemail-template-0.1.9/django_proemail_template.egg-info/dependency_links.txt
--rw-r--r--   0 teppss     (501) staff       (20)       14 2022-04-05 14:13:52.000000 django-proemail-template-0.1.9/django_proemail_template.egg-info/top_level.txt
--rw-r--r--   0 teppss     (501) staff       (20)       38 2022-04-05 14:13:52.871780 django-proemail-template-0.1.9/setup.cfg
--rw-r--r--   0 teppss     (501) staff       (20)     1191 2022-04-05 14:13:38.000000 django-proemail-template-0.1.9/setup.py
+drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:19:26.748662 django-proemail-template-0.2.0/
+drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:19:26.746585 django-proemail-template-0.2.0/EmailTemplate/
+-rw-r--r--   0 teppss     (501) staff       (20)        0 2022-04-05 14:10:09.000000 django-proemail-template-0.2.0/EmailTemplate/__init__.py
+-rw-r--r--   0 teppss     (501) staff       (20)      718 2023-06-02 16:17:24.000000 django-proemail-template-0.2.0/EmailTemplate/admin.py
+drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:19:26.747950 django-proemail-template-0.2.0/EmailTemplate/migrations/
+-rw-r--r--   0 teppss     (501) staff       (20)     1232 2022-04-05 14:05:32.000000 django-proemail-template-0.2.0/EmailTemplate/migrations/0001_initial.py
+-rw-r--r--   0 teppss     (501) staff       (20)      445 2022-04-05 14:05:32.000000 django-proemail-template-0.2.0/EmailTemplate/migrations/0002_auto_20190719_1354.py
+-rw-r--r--   0 teppss     (501) staff       (20)      482 2022-04-05 14:05:32.000000 django-proemail-template-0.2.0/EmailTemplate/migrations/0003_auto_20190719_1358.py
+-rw-r--r--   0 teppss     (501) staff       (20)      445 2022-04-05 14:05:32.000000 django-proemail-template-0.2.0/EmailTemplate/migrations/0004_auto_20210226_0911.py
+-rw-r--r--   0 teppss     (501) staff       (20)      637 2022-04-05 14:12:58.000000 django-proemail-template-0.2.0/EmailTemplate/migrations/0005_emailtemplate_bcc_emailtemplate_cc.py
+-rw-r--r--   0 teppss     (501) staff       (20)        0 2022-04-05 14:05:32.000000 django-proemail-template-0.2.0/EmailTemplate/migrations/__init__.py
+-rw-r--r--   0 teppss     (501) staff       (20)     5468 2023-06-02 16:16:34.000000 django-proemail-template-0.2.0/EmailTemplate/models.py
+-rw-r--r--   0 teppss     (501) staff       (20)      449 2021-02-26 09:04:46.000000 django-proemail-template-0.2.0/EmailTemplate/tests.py
+-rw-r--r--   0 teppss     (501) staff       (20)       63 2018-11-14 15:29:47.000000 django-proemail-template-0.2.0/EmailTemplate/views.py
+-rw-r--r--   0 teppss     (501) staff       (20)     1065 2019-07-12 02:22:08.000000 django-proemail-template-0.2.0/LICENSE
+-rw-r--r--   0 teppss     (501) staff       (20)       60 2022-05-19 14:16:14.000000 django-proemail-template-0.2.0/MANIFEST.in
+-rw-r--r--   0 teppss     (501) staff       (20)     1783 2023-06-02 16:19:26.748546 django-proemail-template-0.2.0/PKG-INFO
+-rw-r--r--   0 teppss     (501) staff       (20)      979 2020-02-01 09:44:20.000000 django-proemail-template-0.2.0/README.rst
+drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:19:26.748372 django-proemail-template-0.2.0/django_proemail_template.egg-info/
+-rw-r--r--   0 teppss     (501) staff       (20)     1783 2023-06-02 16:19:26.000000 django-proemail-template-0.2.0/django_proemail_template.egg-info/PKG-INFO
+-rw-r--r--   0 teppss     (501) staff       (20)      652 2023-06-02 16:19:26.000000 django-proemail-template-0.2.0/django_proemail_template.egg-info/SOURCES.txt
+-rw-r--r--   0 teppss     (501) staff       (20)        1 2023-06-02 16:19:26.000000 django-proemail-template-0.2.0/django_proemail_template.egg-info/dependency_links.txt
+-rw-r--r--   0 teppss     (501) staff       (20)       14 2023-06-02 16:19:26.000000 django-proemail-template-0.2.0/django_proemail_template.egg-info/top_level.txt
+-rw-r--r--   0 teppss     (501) staff       (20)       38 2023-06-02 16:19:26.748702 django-proemail-template-0.2.0/setup.cfg
+-rw-r--r--   0 teppss     (501) staff       (20)     1191 2023-06-02 16:18:14.000000 django-proemail-template-0.2.0/setup.py
```

### Comparing `django-proemail-template-0.1.9/EmailTemplate/migrations/0001_initial.py` & `django-proemail-template-0.2.0/EmailTemplate/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.1.9/EmailTemplate/migrations/0005_emailtemplate_bcc_emailtemplate_cc.py` & `django-proemail-template-0.2.0/EmailTemplate/migrations/0005_emailtemplate_bcc_emailtemplate_cc.py`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.1.9/LICENSE` & `django-proemail-template-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.1.9/PKG-INFO` & `django-proemail-template-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-proemail-template
-Version: 0.1.9
+Version: 0.2.0
 Summary: A simple Django app to send emails
 Home-page: https://github.com/iwalucas/django-email-template/
 Author: Lucas
 Author-email: teppss@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -55,9 +54,7 @@
 
 And send it from any code::
 
     EmailTemplate.send('default', {
         'object': your_model_instance,
     })
     
-
-
```

### Comparing `django-proemail-template-0.1.9/README.rst` & `django-proemail-template-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.1.9/django_proemail_template.egg-info/PKG-INFO` & `django-proemail-template-0.2.0/django_proemail_template.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-proemail-template
-Version: 0.1.9
+Version: 0.2.0
 Summary: A simple Django app to send emails
 Home-page: https://github.com/iwalucas/django-email-template/
 Author: Lucas
 Author-email: teppss@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -55,9 +54,7 @@
 
 And send it from any code::
 
     EmailTemplate.send('default', {
         'object': your_model_instance,
     })
     
-
-
```

### Comparing `django-proemail-template-0.1.9/django_proemail_template.egg-info/SOURCES.txt` & `django-proemail-template-0.2.0/django_proemail_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.1.9/setup.py` & `django-proemail-template-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-proemail-template',
-    version='0.1.9',
+    version='0.2.0',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A simple Django app to send emails',
     long_description=README,
     url='https://github.com/iwalucas/django-email-template/',
     author='Lucas',
```

