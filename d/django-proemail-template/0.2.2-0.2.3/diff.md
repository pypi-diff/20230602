# Comparing `tmp/django-proemail-template-0.2.2.tar.gz` & `tmp/django-proemail-template-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-proemail-template-0.2.2.tar", last modified: Fri Jun  2 16:23:55 2023, max compression
+gzip compressed data, was "django-proemail-template-0.2.3.tar", last modified: Fri Jun  2 16:26:23 2023, max compression
```

## Comparing `django-proemail-template-0.2.2.tar` & `django-proemail-template-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:23:55.568999 django-proemail-template-0.2.2/
-drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:23:55.567078 django-proemail-template-0.2.2/EmailTemplate/
--rw-r--r--   0 teppss     (501) staff       (20)        0 2022-04-05 14:10:09.000000 django-proemail-template-0.2.2/EmailTemplate/__init__.py
--rw-r--r--   0 teppss     (501) staff       (20)      706 2023-06-02 16:23:37.000000 django-proemail-template-0.2.2/EmailTemplate/admin.py
-drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:23:55.568319 django-proemail-template-0.2.2/EmailTemplate/migrations/
--rw-r--r--   0 teppss     (501) staff       (20)     1232 2022-04-05 14:05:32.000000 django-proemail-template-0.2.2/EmailTemplate/migrations/0001_initial.py
--rw-r--r--   0 teppss     (501) staff       (20)      445 2022-04-05 14:05:32.000000 django-proemail-template-0.2.2/EmailTemplate/migrations/0002_auto_20190719_1354.py
--rw-r--r--   0 teppss     (501) staff       (20)      482 2022-04-05 14:05:32.000000 django-proemail-template-0.2.2/EmailTemplate/migrations/0003_auto_20190719_1358.py
--rw-r--r--   0 teppss     (501) staff       (20)      445 2022-04-05 14:05:32.000000 django-proemail-template-0.2.2/EmailTemplate/migrations/0004_auto_20210226_0911.py
--rw-r--r--   0 teppss     (501) staff       (20)      637 2022-04-05 14:12:58.000000 django-proemail-template-0.2.2/EmailTemplate/migrations/0005_emailtemplate_bcc_emailtemplate_cc.py
--rw-r--r--   0 teppss     (501) staff       (20)        0 2022-04-05 14:05:32.000000 django-proemail-template-0.2.2/EmailTemplate/migrations/__init__.py
--rw-r--r--   0 teppss     (501) staff       (20)     5468 2023-06-02 16:16:34.000000 django-proemail-template-0.2.2/EmailTemplate/models.py
--rw-r--r--   0 teppss     (501) staff       (20)      449 2021-02-26 09:04:46.000000 django-proemail-template-0.2.2/EmailTemplate/tests.py
--rw-r--r--   0 teppss     (501) staff       (20)       63 2018-11-14 15:29:47.000000 django-proemail-template-0.2.2/EmailTemplate/views.py
--rw-r--r--   0 teppss     (501) staff       (20)     1065 2019-07-12 02:22:08.000000 django-proemail-template-0.2.2/LICENSE
--rw-r--r--   0 teppss     (501) staff       (20)       60 2022-05-19 14:16:14.000000 django-proemail-template-0.2.2/MANIFEST.in
--rw-r--r--   0 teppss     (501) staff       (20)     1803 2023-06-02 16:23:55.568884 django-proemail-template-0.2.2/PKG-INFO
--rw-r--r--   0 teppss     (501) staff       (20)      979 2020-02-01 09:44:20.000000 django-proemail-template-0.2.2/README.rst
-drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:23:55.568729 django-proemail-template-0.2.2/django_proemail_template.egg-info/
--rw-r--r--   0 teppss     (501) staff       (20)     1803 2023-06-02 16:23:55.000000 django-proemail-template-0.2.2/django_proemail_template.egg-info/PKG-INFO
--rw-r--r--   0 teppss     (501) staff       (20)      652 2023-06-02 16:23:55.000000 django-proemail-template-0.2.2/django_proemail_template.egg-info/SOURCES.txt
--rw-r--r--   0 teppss     (501) staff       (20)        1 2023-06-02 16:23:55.000000 django-proemail-template-0.2.2/django_proemail_template.egg-info/dependency_links.txt
--rw-r--r--   0 teppss     (501) staff       (20)       14 2023-06-02 16:23:55.000000 django-proemail-template-0.2.2/django_proemail_template.egg-info/top_level.txt
--rw-r--r--   0 teppss     (501) staff       (20)       38 2023-06-02 16:23:55.569033 django-proemail-template-0.2.2/setup.cfg
--rw-r--r--   0 teppss     (501) staff       (20)     1191 2023-06-02 16:23:49.000000 django-proemail-template-0.2.2/setup.py
+drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:26:23.831401 django-proemail-template-0.2.3/
+drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:26:23.829312 django-proemail-template-0.2.3/EmailTemplate/
+-rw-r--r--   0 teppss     (501) staff       (20)        0 2022-04-05 14:10:09.000000 django-proemail-template-0.2.3/EmailTemplate/__init__.py
+-rw-r--r--   0 teppss     (501) staff       (20)      706 2023-06-02 16:23:37.000000 django-proemail-template-0.2.3/EmailTemplate/admin.py
+drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:26:23.830647 django-proemail-template-0.2.3/EmailTemplate/migrations/
+-rw-r--r--   0 teppss     (501) staff       (20)     1232 2022-04-05 14:05:32.000000 django-proemail-template-0.2.3/EmailTemplate/migrations/0001_initial.py
+-rw-r--r--   0 teppss     (501) staff       (20)      445 2022-04-05 14:05:32.000000 django-proemail-template-0.2.3/EmailTemplate/migrations/0002_auto_20190719_1354.py
+-rw-r--r--   0 teppss     (501) staff       (20)      482 2022-04-05 14:05:32.000000 django-proemail-template-0.2.3/EmailTemplate/migrations/0003_auto_20190719_1358.py
+-rw-r--r--   0 teppss     (501) staff       (20)      445 2022-04-05 14:05:32.000000 django-proemail-template-0.2.3/EmailTemplate/migrations/0004_auto_20210226_0911.py
+-rw-r--r--   0 teppss     (501) staff       (20)      637 2022-04-05 14:12:58.000000 django-proemail-template-0.2.3/EmailTemplate/migrations/0005_emailtemplate_bcc_emailtemplate_cc.py
+-rw-r--r--   0 teppss     (501) staff       (20)        0 2022-04-05 14:05:32.000000 django-proemail-template-0.2.3/EmailTemplate/migrations/__init__.py
+-rw-r--r--   0 teppss     (501) staff       (20)     5468 2023-06-02 16:16:34.000000 django-proemail-template-0.2.3/EmailTemplate/models.py
+-rw-r--r--   0 teppss     (501) staff       (20)      449 2021-02-26 09:04:46.000000 django-proemail-template-0.2.3/EmailTemplate/tests.py
+-rw-r--r--   0 teppss     (501) staff       (20)       63 2018-11-14 15:29:47.000000 django-proemail-template-0.2.3/EmailTemplate/views.py
+-rw-r--r--   0 teppss     (501) staff       (20)     1065 2019-07-12 02:22:08.000000 django-proemail-template-0.2.3/LICENSE
+-rw-r--r--   0 teppss     (501) staff       (20)       60 2022-05-19 14:16:14.000000 django-proemail-template-0.2.3/MANIFEST.in
+-rw-r--r--   0 teppss     (501) staff       (20)     1803 2023-06-02 16:26:23.831287 django-proemail-template-0.2.3/PKG-INFO
+-rw-r--r--   0 teppss     (501) staff       (20)      979 2020-02-01 09:44:20.000000 django-proemail-template-0.2.3/README.rst
+drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:26:23.831120 django-proemail-template-0.2.3/django_proemail_template.egg-info/
+-rw-r--r--   0 teppss     (501) staff       (20)     1803 2023-06-02 16:26:23.000000 django-proemail-template-0.2.3/django_proemail_template.egg-info/PKG-INFO
+-rw-r--r--   0 teppss     (501) staff       (20)      652 2023-06-02 16:26:23.000000 django-proemail-template-0.2.3/django_proemail_template.egg-info/SOURCES.txt
+-rw-r--r--   0 teppss     (501) staff       (20)        1 2023-06-02 16:26:23.000000 django-proemail-template-0.2.3/django_proemail_template.egg-info/dependency_links.txt
+-rw-r--r--   0 teppss     (501) staff       (20)       14 2023-06-02 16:26:23.000000 django-proemail-template-0.2.3/django_proemail_template.egg-info/top_level.txt
+-rw-r--r--   0 teppss     (501) staff       (20)       38 2023-06-02 16:26:23.831436 django-proemail-template-0.2.3/setup.cfg
+-rw-r--r--   0 teppss     (501) staff       (20)     1191 2023-06-02 16:26:20.000000 django-proemail-template-0.2.3/setup.py
```

### Comparing `django-proemail-template-0.2.2/EmailTemplate/admin.py` & `django-proemail-template-0.2.3/EmailTemplate/admin.py`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.2.2/EmailTemplate/migrations/0001_initial.py` & `django-proemail-template-0.2.3/EmailTemplate/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.2.2/EmailTemplate/migrations/0005_emailtemplate_bcc_emailtemplate_cc.py` & `django-proemail-template-0.2.3/EmailTemplate/migrations/0005_emailtemplate_bcc_emailtemplate_cc.py`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.2.2/EmailTemplate/models.py` & `django-proemail-template-0.2.3/EmailTemplate/models.py`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.2.2/LICENSE` & `django-proemail-template-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.2.2/PKG-INFO` & `django-proemail-template-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-proemail-template
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple Django app to send emails
 Home-page: https://github.com/iwalucas/django-email-template/
 Author: Lucas
 Author-email: teppss@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-proemail-template-0.2.2/README.rst` & `django-proemail-template-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.2.2/django_proemail_template.egg-info/PKG-INFO` & `django-proemail-template-0.2.3/django_proemail_template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-proemail-template
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple Django app to send emails
 Home-page: https://github.com/iwalucas/django-email-template/
 Author: Lucas
 Author-email: teppss@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-proemail-template-0.2.2/django_proemail_template.egg-info/SOURCES.txt` & `django-proemail-template-0.2.3/django_proemail_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.2.2/setup.py` & `django-proemail-template-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-proemail-template',
-    version='0.2.2',
+    version='0.2.3',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A simple Django app to send emails',
     long_description=README,
     url='https://github.com/iwalucas/django-email-template/',
     author='Lucas',
```

