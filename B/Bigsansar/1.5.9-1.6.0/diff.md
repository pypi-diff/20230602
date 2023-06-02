# Comparing `tmp/Bigsansar-1.5.9.tar.gz` & `tmp/Bigsansar-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-1.5.9.tar", last modified: Mon May 29 11:14:14 2023, max compression
+gzip compressed data, was "Bigsansar-1.6.0.tar", last modified: Fri Jun  2 12:56:26 2023, max compression
```

## Comparing `Bigsansar-1.5.9.tar` & `Bigsansar-1.6.0.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:14.024482 Bigsansar-1.5.9/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.954482 Bigsansar-1.5.9/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3669 2023-05-29 11:14:13.000000 Bigsansar-1.5.9/Bigsansar.egg-info/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13689 2023-05-29 11:14:13.000000 Bigsansar-1.5.9/Bigsansar.egg-info/SOURCES.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-05-29 11:14:13.000000 Bigsansar-1.5.9/Bigsansar.egg-info/dependency_links.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-05-29 11:14:13.000000 Bigsansar-1.5.9/Bigsansar.egg-info/entry_points.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       98 2023-05-29 11:14:13.000000 Bigsansar-1.5.9/Bigsansar.egg-info/requires.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-05-29 11:14:13.000000 Bigsansar-1.5.9/Bigsansar.egg-info/top_level.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-29 06:46:12.000000 Bigsansar-1.5.9/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3669 2023-05-29 11:14:14.024482 Bigsansar-1.5.9/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3080 2023-05-29 09:05:18.000000 Bigsansar-1.5.9/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.954482 Bigsansar-1.5.9/bigsansar/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.954482 Bigsansar-1.5.9/bigsansar/contrib/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.954482 Bigsansar-1.5.9/bigsansar/contrib/account/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/account/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/account/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/account/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.954482 Bigsansar-1.5.9/bigsansar/contrib/account/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/account/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/account/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/account/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.954482 Bigsansar-1.5.9/bigsansar/contrib/account/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/account/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/account/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/account/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.954482 Bigsansar-1.5.9/bigsansar/contrib/advance/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.5.9/bigsansar/contrib/advance/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      291 2023-05-13 03:12:35.000000 Bigsansar-1.5.9/bigsansar/contrib/advance/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      202 2023-05-08 12:23:18.000000 Bigsansar-1.5.9/bigsansar/contrib/advance/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.964482 Bigsansar-1.5.9/bigsansar/contrib/advance/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1000 2023-05-08 12:29:40.000000 Bigsansar-1.5.9/bigsansar/contrib/advance/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-05-13 02:56:41.000000 Bigsansar-1.5.9/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1050 2023-05-13 03:08:43.000000 Bigsansar-1.5.9/bigsansar/contrib/advance/migrations/0003_javascript.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      386 2023-05-13 03:14:07.000000 Bigsansar-1.5.9/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.5.9/bigsansar/contrib/advance/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2023-05-13 04:58:52.000000 Bigsansar-1.5.9/bigsansar/contrib/advance/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-05-08 12:18:38.000000 Bigsansar-1.5.9/bigsansar/contrib/advance/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-05-08 12:18:38.000000 Bigsansar-1.5.9/bigsansar/contrib/advance/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.964482 Bigsansar-1.5.9/bigsansar/contrib/blogs/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/blogs/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      520 2023-05-29 07:20:57.000000 Bigsansar-1.5.9/bigsansar/contrib/blogs/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/blogs/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.964482 Bigsansar-1.5.9/bigsansar/contrib/blogs/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2261 2023-05-29 10:57:40.000000 Bigsansar-1.5.9/bigsansar/contrib/blogs/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 10:57:14.000000 Bigsansar-1.5.9/bigsansar/contrib/blogs/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2106 2023-05-29 08:48:25.000000 Bigsansar-1.5.9/bigsansar/contrib/blogs/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.964482 Bigsansar-1.5.9/bigsansar/contrib/blogs/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-20 12:33:35.000000 Bigsansar-1.5.9/bigsansar/contrib/blogs/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      844 2023-05-27 09:55:49.000000 Bigsansar-1.5.9/bigsansar/contrib/blogs/templatetags/blogs.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/blogs/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/blogs/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.964482 Bigsansar-1.5.9/bigsansar/contrib/sites/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/sites/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1733 2023-05-20 05:28:14.000000 Bigsansar-1.5.9/bigsansar/contrib/sites/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/sites/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3041 2023-05-17 09:58:25.000000 Bigsansar-1.5.9/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.964482 Bigsansar-1.5.9/bigsansar/contrib/sites/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1847 2023-05-02 12:46:38.000000 Bigsansar-1.5.9/bigsansar/contrib/sites/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:46:31.000000 Bigsansar-1.5.9/bigsansar/contrib/sites/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1899 2023-05-17 10:15:27.000000 Bigsansar-1.5.9/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.974482 Bigsansar-1.5.9/bigsansar/contrib/sites/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/sites/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/sites/templatetags/pages.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/sites/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/contrib/sites/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.974482 Bigsansar-1.5.9/bigsansar/core/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/core/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/core/host.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    10679 2023-05-27 06:38:55.000000 Bigsansar-1.5.9/bigsansar/core/init.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/main.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.974482 Bigsansar-1.5.9/bigsansar/management/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.974482 Bigsansar-1.5.9/bigsansar/management/commands/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/management/commands/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.5.9/bigsansar/management/commands/createuser.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.974482 Bigsansar-1.5.9/bigsansar/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.974482 Bigsansar-1.5.9/bigsansar/static/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/static/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.934482 Bigsansar-1.5.9/bigsansar/static/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.934482 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.944482 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.974482 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.974482 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2361 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/codesnippet.js
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.974482 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      532 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/codesnippet.png
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.974482 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1046 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/codesnippet.png
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.994482 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      509 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ar.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      455 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/az.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      512 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/bg.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      452 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ca.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      431 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/cs.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      415 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/da.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      438 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/de-ch.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      435 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/de.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      581 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/el.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/en-au.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/en-gb.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      424 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/en.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      413 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/eo.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/es-mx.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/es.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      411 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/et.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      420 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/eu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      453 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fa.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      479 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fr-ca.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      439 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      471 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/gl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      455 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/he.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      433 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/hr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      434 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/hu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/id.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      468 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/it.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      486 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ja.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      487 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/km.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      451 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ko.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ku.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      441 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/lt.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      431 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/lv.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      415 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/nb.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      407 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/nl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/no.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      440 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/oc.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      418 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/pl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      470 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/pt-br.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      465 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/pt.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      438 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ro.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      478 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ru.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      415 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      446 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sq.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      425 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sr-latn.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      488 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      410 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sv.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      541 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/th.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      428 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/tr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/tt.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      482 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ug.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      502 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/uk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      437 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/vi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      420 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/zh-cn.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      435 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/zh.js
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.944482 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:13.994482 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    29367 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/CHANGES.md
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1498 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4682 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.md
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     7534 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.ru.md
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    30210 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/highlight.pack.js
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:14.004482 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2354 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/arta.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      806 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ascetic.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1719 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1733 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.light.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1744 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1753 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.light.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1743 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.light.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1765 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1774 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.light.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1755 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1764 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.light.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1791 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_paper.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    18198 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_papersq.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1762 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2651 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/default.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1776 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/docco.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1903 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/far.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1582 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/foundation.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1684 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/github.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2162 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/googlecode.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/idea.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1462 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ir_black.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1928 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/magula.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      899 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/mono-blue.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2014 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2336 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai_sublime.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2316 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/obsidian.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1493 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1494 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.light.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1641 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.jpg
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2554 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/railscasts.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1595 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/rainbow.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1983 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      486 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1602 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1602 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_light.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2238 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/sunburst.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1603 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-blue.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1533 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-bright.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1537 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-eighties.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1600 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1429 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1561 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/vs.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2294 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/xcode.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1856 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/zenburn.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    15468 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/plugin.js
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:14.004482 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/samples/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     8267 2023-03-22 09:50:46.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/samples/codesnippet.html
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:14.004482 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:14.004482 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1258 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1165 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:14.014482 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1337 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1654 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1209 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1078 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1514 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1049 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1084 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1103 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      960 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1051 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1250 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1166 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1106 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1195 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1229 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1047 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1064 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1120 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1151 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1178 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1564 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1173 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1206 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1538 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1067 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      916 2021-03-31 11:22:53.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13371 2021-03-31 14:36:18.000000 Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/static/logo.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 11:14:14.024482 Bigsansar-1.5.9/bigsansar/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/templates/404.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/templates/acc_active_email.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1521 2023-05-05 10:08:59.000000 Bigsansar-1.5.9/bigsansar/templates/base.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1326 2023-05-20 05:28:14.000000 Bigsansar-1.5.9/bigsansar/templates/blog_preview.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/templates/default.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/templates/defaultpage.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/templates/parking.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-05-20 05:28:14.000000 Bigsansar-1.5.9/bigsansar/templates/sitemap.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.5.9/bigsansar/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1155 2023-05-20 14:08:47.000000 Bigsansar-1.5.9/bigsansar/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4559 2023-05-20 14:56:48.000000 Bigsansar-1.5.9/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-05-29 11:14:14.024482 Bigsansar-1.5.9/setup.cfg
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2056 2023-05-29 11:12:59.000000 Bigsansar-1.5.9/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.344382 Bigsansar-1.6.0/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.974382 Bigsansar-1.6.0/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3669 2023-06-02 12:56:25.000000 Bigsansar-1.6.0/Bigsansar.egg-info/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13689 2023-06-02 12:56:25.000000 Bigsansar-1.6.0/Bigsansar.egg-info/SOURCES.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-06-02 12:56:25.000000 Bigsansar-1.6.0/Bigsansar.egg-info/dependency_links.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-06-02 12:56:25.000000 Bigsansar-1.6.0/Bigsansar.egg-info/entry_points.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       98 2023-06-02 12:56:25.000000 Bigsansar-1.6.0/Bigsansar.egg-info/requires.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-06-02 12:56:25.000000 Bigsansar-1.6.0/Bigsansar.egg-info/top_level.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-29 06:46:12.000000 Bigsansar-1.6.0/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3669 2023-06-02 12:56:26.344382 Bigsansar-1.6.0/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3080 2023-05-29 09:05:18.000000 Bigsansar-1.6.0/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.974382 Bigsansar-1.6.0/bigsansar/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.974382 Bigsansar-1.6.0/bigsansar/contrib/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.984382 Bigsansar-1.6.0/bigsansar/contrib/account/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/account/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/account/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/account/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.994382 Bigsansar-1.6.0/bigsansar/contrib/account/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/account/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/account/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/account/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.994382 Bigsansar-1.6.0/bigsansar/contrib/account/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/account/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/account/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/account/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.994382 Bigsansar-1.6.0/bigsansar/contrib/advance/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.6.0/bigsansar/contrib/advance/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      291 2023-05-13 03:12:35.000000 Bigsansar-1.6.0/bigsansar/contrib/advance/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      202 2023-05-08 12:23:18.000000 Bigsansar-1.6.0/bigsansar/contrib/advance/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.994382 Bigsansar-1.6.0/bigsansar/contrib/advance/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1000 2023-05-08 12:29:40.000000 Bigsansar-1.6.0/bigsansar/contrib/advance/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-05-13 02:56:41.000000 Bigsansar-1.6.0/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1050 2023-05-13 03:08:43.000000 Bigsansar-1.6.0/bigsansar/contrib/advance/migrations/0003_javascript.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      386 2023-05-13 03:14:07.000000 Bigsansar-1.6.0/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.6.0/bigsansar/contrib/advance/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2023-05-13 04:58:52.000000 Bigsansar-1.6.0/bigsansar/contrib/advance/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-05-08 12:18:38.000000 Bigsansar-1.6.0/bigsansar/contrib/advance/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-05-08 12:18:38.000000 Bigsansar-1.6.0/bigsansar/contrib/advance/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.994382 Bigsansar-1.6.0/bigsansar/contrib/blogs/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/blogs/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      520 2023-05-29 07:20:57.000000 Bigsansar-1.6.0/bigsansar/contrib/blogs/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/blogs/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.994382 Bigsansar-1.6.0/bigsansar/contrib/blogs/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2261 2023-05-29 10:57:40.000000 Bigsansar-1.6.0/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 10:57:14.000000 Bigsansar-1.6.0/bigsansar/contrib/blogs/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2106 2023-05-29 08:48:25.000000 Bigsansar-1.6.0/bigsansar/contrib/blogs/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.994382 Bigsansar-1.6.0/bigsansar/contrib/blogs/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-20 12:33:35.000000 Bigsansar-1.6.0/bigsansar/contrib/blogs/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      927 2023-06-02 12:55:41.000000 Bigsansar-1.6.0/bigsansar/contrib/blogs/templatetags/blogs.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/blogs/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.004382 Bigsansar-1.6.0/bigsansar/contrib/sites/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/sites/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1733 2023-06-02 12:05:41.000000 Bigsansar-1.6.0/bigsansar/contrib/sites/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/sites/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3041 2023-05-17 09:58:25.000000 Bigsansar-1.6.0/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.004382 Bigsansar-1.6.0/bigsansar/contrib/sites/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1847 2023-05-02 12:46:38.000000 Bigsansar-1.6.0/bigsansar/contrib/sites/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:46:31.000000 Bigsansar-1.6.0/bigsansar/contrib/sites/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1899 2023-05-17 10:15:27.000000 Bigsansar-1.6.0/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.014382 Bigsansar-1.6.0/bigsansar/contrib/sites/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/sites/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/sites/templatetags/pages.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/sites/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/contrib/sites/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.014382 Bigsansar-1.6.0/bigsansar/core/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/core/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/core/host.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    10679 2023-05-27 06:38:55.000000 Bigsansar-1.6.0/bigsansar/core/init.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/main.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.014382 Bigsansar-1.6.0/bigsansar/management/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.014382 Bigsansar-1.6.0/bigsansar/management/commands/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/management/commands/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.6.0/bigsansar/management/commands/createuser.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.014382 Bigsansar-1.6.0/bigsansar/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.024382 Bigsansar-1.6.0/bigsansar/static/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/static/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.944383 Bigsansar-1.6.0/bigsansar/static/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.944383 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.954383 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.024382 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.034382 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2361 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/codesnippet.js
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.034382 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      532 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/codesnippet.png
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.034382 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1046 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/codesnippet.png
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.164383 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      509 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ar.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      455 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/az.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      512 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/bg.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      452 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ca.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      431 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/cs.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      415 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/da.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      438 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/de-ch.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      435 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/de.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      581 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/el.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/en-au.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/en-gb.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      424 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/en.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      413 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/eo.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/es-mx.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/es.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      411 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/et.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      420 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/eu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      453 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fa.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      479 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fr-ca.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      439 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      471 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/gl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      455 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/he.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      433 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/hr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      434 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/hu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/id.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      468 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/it.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      486 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ja.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      487 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/km.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      451 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ko.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ku.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      441 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/lt.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      431 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/lv.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      415 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/nb.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      407 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/nl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/no.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      440 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/oc.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      418 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/pl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      470 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/pt-br.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      465 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/pt.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      438 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ro.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      478 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ru.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      415 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      446 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sq.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      425 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sr-latn.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      488 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      410 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sv.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      541 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/th.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      428 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/tr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/tt.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      482 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ug.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      502 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/uk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      437 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/vi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      420 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/zh-cn.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      435 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/zh.js
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:25.954383 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.174383 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    29367 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/CHANGES.md
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1498 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4682 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.md
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     7534 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.ru.md
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    30210 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/highlight.pack.js
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.264382 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2354 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/arta.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      806 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ascetic.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1719 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1733 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.light.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1744 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1753 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.light.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1743 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.light.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1765 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1774 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.light.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1755 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1764 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.light.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1791 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_paper.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    18198 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_papersq.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1762 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2651 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/default.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1776 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/docco.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1903 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/far.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1582 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/foundation.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1684 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/github.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2162 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/googlecode.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/idea.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1462 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ir_black.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1928 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/magula.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      899 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/mono-blue.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2014 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2336 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai_sublime.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2316 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/obsidian.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1493 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1494 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.light.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1641 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.jpg
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2554 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/railscasts.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1595 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/rainbow.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1983 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      486 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1602 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1602 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_light.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2238 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/sunburst.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1603 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-blue.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1533 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-bright.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1537 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-eighties.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1600 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1429 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1561 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/vs.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2294 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/xcode.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1856 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/zenburn.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    15468 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/plugin.js
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.264382 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/samples/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     8267 2023-03-22 09:50:46.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/samples/codesnippet.html
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.274382 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.274382 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1258 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1165 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.324382 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1337 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1654 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1209 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1078 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1514 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1049 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1084 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1103 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      960 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1051 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1250 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1166 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1106 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1195 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1229 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1047 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1064 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1120 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1151 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1178 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1564 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1173 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1206 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1538 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1067 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      916 2021-03-31 11:22:53.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13371 2021-03-31 14:36:18.000000 Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/static/logo.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 12:56:26.344382 Bigsansar-1.6.0/bigsansar/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/templates/404.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/templates/acc_active_email.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1521 2023-05-05 10:08:59.000000 Bigsansar-1.6.0/bigsansar/templates/base.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1326 2023-05-20 05:28:14.000000 Bigsansar-1.6.0/bigsansar/templates/blog_preview.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/templates/default.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/templates/defaultpage.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/templates/parking.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-05-20 05:28:14.000000 Bigsansar-1.6.0/bigsansar/templates/sitemap.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.0/bigsansar/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1155 2023-05-20 14:08:47.000000 Bigsansar-1.6.0/bigsansar/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4445 2023-06-02 12:16:08.000000 Bigsansar-1.6.0/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-06-02 12:56:26.344382 Bigsansar-1.6.0/setup.cfg
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2056 2023-06-02 12:55:55.000000 Bigsansar-1.6.0/setup.py
```

### Comparing `Bigsansar-1.5.9/Bigsansar.egg-info/PKG-INFO` & `Bigsansar-1.6.0/Bigsansar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.5.9
+Version: 1.6.0
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 1.5.9 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 1.6.0 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 bigsansar.com Author: Bikash Pokhrel Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN Project-URL: Bug Tracker, https://github.com/pokhrelb9/
 bigsansar/issues Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django
 flatpages Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `Bigsansar-1.5.9/Bigsansar.egg-info/SOURCES.txt` & `Bigsansar-1.6.0/Bigsansar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/LICENSE` & `Bigsansar-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/PKG-INFO` & `Bigsansar-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.5.9
+Version: 1.6.0
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 1.5.9 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 1.6.0 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 bigsansar.com Author: Bikash Pokhrel Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN Project-URL: Bug Tracker, https://github.com/pokhrelb9/
 bigsansar/issues Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django
 flatpages Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `Bigsansar-1.5.9/README.md` & `Bigsansar-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/contrib/account/forms.py` & `Bigsansar-1.6.0/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/contrib/account/migrations/0001_initial.py` & `Bigsansar-1.6.0/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/contrib/account/models.py` & `Bigsansar-1.6.0/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/contrib/advance/migrations/0001_initial.py` & `Bigsansar-1.6.0/bigsansar/contrib/advance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/contrib/advance/migrations/0003_javascript.py` & `Bigsansar-1.6.0/bigsansar/contrib/advance/migrations/0003_javascript.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/contrib/advance/models.py` & `Bigsansar-1.6.0/bigsansar/contrib/advance/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/contrib/blogs/admin.py` & `Bigsansar-1.6.0/bigsansar/contrib/blogs/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/contrib/blogs/migrations/0001_initial.py` & `Bigsansar-1.6.0/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/contrib/blogs/models.py` & `Bigsansar-1.6.0/bigsansar/contrib/blogs/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/contrib/blogs/templatetags/blogs.py` & `Bigsansar-1.6.0/bigsansar/contrib/blogs/templatetags/blogs.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,26 @@
 
 register = template.Library()
 
 
 @register.simple_tag(takes_context=True)
 def get_blog(context):
     current_site = get_current_site(context['request'])
-    get_pages_filter = post.objects.filter(domain__domain=current_site)
+    get_pages_filter = post.objects.filter(domain__domain=current_site).order_by('-id')[:10]
 
     return get_pages_filter
 
 
 @register.simple_tag(takes_context=True)
 def get_blog_object(context):
     get_path_args = context['request'].get_full_path().rsplit('/', 1)[1]
     dd = get_path_args.split('?')[0]
     current_site = get_current_site(context['request'])
-    db = domains.objects.get(domain=current_site)
-    get_blog_objects = post.objects.get(domain=db, slug=dd)
+    try:
+        db = domains.objects.get(domain=current_site)
+        get_blog_objects = post.objects.get(domain=db, slug=dd)
 
-    return get_blog_objects
+    except:
+        pass
+
+    else:
+        return get_blog_objects
```

### Comparing `Bigsansar-1.5.9/bigsansar/contrib/sites/admin.py` & `Bigsansar-1.6.0/bigsansar/contrib/sites/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/contrib/sites/forms.py` & `Bigsansar-1.6.0/bigsansar/contrib/sites/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/contrib/sites/migrations/0001_initial.py` & `Bigsansar-1.6.0/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/contrib/sites/models.py` & `Bigsansar-1.6.0/bigsansar/contrib/sites/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/core/__init__.py` & `Bigsansar-1.6.0/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/core/init.py` & `Bigsansar-1.6.0/bigsansar/core/init.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/management/commands/createuser.py` & `Bigsansar-1.6.0/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/codesnippet.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/codesnippet.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/codesnippet.png` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/codesnippet.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/codesnippet.png` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/codesnippet.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/bg.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/bg.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/el.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/el.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/th.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/th.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/CHANGES.md` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/CHANGES.md`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/LICENSE` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.md` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.md`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.ru.md` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.ru.md`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/highlight.pack.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/arta.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/arta.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ascetic.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ascetic.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.dark.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.light.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.light.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.dark.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.light.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.light.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.dark.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.light.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.light.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.dark.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.light.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.light.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.dark.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.light.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.light.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_paper.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_paper.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_papersq.png` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_papersq.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/dark.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/default.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/default.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/docco.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/docco.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/far.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/far.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/foundation.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/foundation.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/github.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/github.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/googlecode.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/googlecode.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/idea.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/idea.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ir_black.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ir_black.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/magula.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/magula.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/mono-blue.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/mono-blue.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai_sublime.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai_sublime.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/obsidian.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/obsidian.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.dark.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.light.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.light.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.jpg` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.jpg`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/railscasts.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/railscasts.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/rainbow.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/rainbow.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_dark.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_light.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_light.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/sunburst.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/sunburst.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-blue.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-blue.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-bright.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-bright.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-eighties.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-eighties.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/vs.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/vs.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/xcode.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/xcode.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/zenburn.css` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/zenburn.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/plugin.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/plugin.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/samples/codesnippet.html` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/samples/codesnippet.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js` & `Bigsansar-1.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/logo.png` & `Bigsansar-1.6.0/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/static/style.css` & `Bigsansar-1.6.0/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/templates/404.html` & `Bigsansar-1.6.0/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/templates/base.html` & `Bigsansar-1.6.0/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/templates/blog_preview.html` & `Bigsansar-1.6.0/bigsansar/templates/blog_preview.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/templates/default.html` & `Bigsansar-1.6.0/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/templates/defaultpage.html` & `Bigsansar-1.6.0/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/templates/parking.html` & `Bigsansar-1.6.0/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/urls.py` & `Bigsansar-1.6.0/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.5.9/bigsansar/views.py` & `Bigsansar-1.6.0/bigsansar/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,16 @@
     default_page = 'defaultpage.html'
     try:
         current_site = get_current_site(request)
         db = domains.objects.get(domain=current_site)
         get_pagename = path.strip('/')
         page = pages.objects.get(domain=db, slug=get_pagename)
         total = db.visitor + 1
-        pagetotal = page.visitor + 1
         domains.objects.filter(pk=db.id).update(visitor=total)
-        pages.objects.filter(domain=db, slug=get_pagename).update(visitor=pagetotal)
+        
 
     except:
         return render(request, '404.html')
     
     else:
          
          asp = 'templates/' + str(db.domain) + '/' + page.slug + '.html'
```

### Comparing `Bigsansar-1.5.9/setup.py` & `Bigsansar-1.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="1.5.9",
+    version="1.6.0",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bigsansar.com",
     project_urls={
```

