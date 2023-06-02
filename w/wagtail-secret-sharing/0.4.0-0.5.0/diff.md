# Comparing `tmp/wagtail-secret-sharing-0.4.0.tar.gz` & `tmp/wagtail-secret-sharing-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-secret-sharing-0.4.0.tar", last modified: Mon Oct 17 07:15:17 2022, max compression
+gzip compressed data, was "wagtail-secret-sharing-0.5.0.tar", last modified: Fri Jun  2 08:24:51 2023, max compression
```

## Comparing `wagtail-secret-sharing-0.4.0.tar` & `wagtail-secret-sharing-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-10-17 07:15:17.051317 wagtail-secret-sharing-0.4.0/
--rw-r--r--   0 robmoorman   (501) staff       (20)     1064 2022-07-18 08:50:50.000000 wagtail-secret-sharing-0.4.0/LICENSE
--rw-r--r--   0 robmoorman   (501) staff       (20)      178 2022-07-18 08:50:50.000000 wagtail-secret-sharing-0.4.0/MANIFEST.in
--rw-r--r--   0 robmoorman   (501) staff       (20)      556 2022-10-17 07:15:17.050962 wagtail-secret-sharing-0.4.0/PKG-INFO
--rw-r--r--   0 robmoorman   (501) staff       (20)       38 2022-10-17 07:15:17.051458 wagtail-secret-sharing-0.4.0/setup.cfg
--rw-r--r--   0 robmoorman   (501) staff       (20)     1031 2022-10-17 07:14:52.000000 wagtail-secret-sharing-0.4.0/setup.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-10-17 07:15:17.045258 wagtail-secret-sharing-0.4.0/src/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-10-17 07:15:17.048242 wagtail-secret-sharing-0.4.0/src/wagtail_secret_sharing/
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-07-18 08:50:50.000000 wagtail-secret-sharing-0.4.0/src/wagtail_secret_sharing/__init__.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     3520 2022-08-11 14:00:23.000000 wagtail-secret-sharing-0.4.0/src/wagtail_secret_sharing/models.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      152 2022-08-09 12:41:59.000000 wagtail-secret-sharing-0.4.0/src/wagtail_secret_sharing/settings.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-10-17 07:15:17.045599 wagtail-secret-sharing-0.4.0/src/wagtail_secret_sharing/templates/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-10-17 07:15:17.049864 wagtail-secret-sharing-0.4.0/src/wagtail_secret_sharing/templates/wagtail_secret_sharing/
--rw-r--r--   0 robmoorman   (501) staff       (20)      686 2022-08-11 14:00:23.000000 wagtail-secret-sharing-0.4.0/src/wagtail_secret_sharing/templates/wagtail_secret_sharing/create.html
--rw-r--r--   0 robmoorman   (501) staff       (20)       98 2022-07-18 08:50:50.000000 wagtail-secret-sharing-0.4.0/src/wagtail_secret_sharing/templates/wagtail_secret_sharing/retrieve.html
--rw-r--r--   0 robmoorman   (501) staff       (20)      367 2022-08-11 14:00:23.000000 wagtail-secret-sharing-0.4.0/src/wagtail_secret_sharing/templates/wagtail_secret_sharing/view.html
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-10-17 07:15:17.050446 wagtail-secret-sharing-0.4.0/src/wagtail_secret_sharing.egg-info/
--rw-r--r--   0 robmoorman   (501) staff       (20)      359 2022-10-17 07:15:17.000000 wagtail-secret-sharing-0.4.0/src/wagtail_secret_sharing.egg-info/SOURCES.txt
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:24:51.151977 wagtail-secret-sharing-0.5.0/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1064 2022-07-18 08:50:50.000000 wagtail-secret-sharing-0.5.0/LICENSE
+-rw-r--r--   0 robmoorman   (501) staff       (20)      178 2022-07-18 08:50:50.000000 wagtail-secret-sharing-0.5.0/MANIFEST.in
+-rw-r--r--   0 robmoorman   (501) staff       (20)      754 2023-06-02 08:24:51.151435 wagtail-secret-sharing-0.5.0/PKG-INFO
+-rw-r--r--   0 robmoorman   (501) staff       (20)       38 2023-06-02 08:24:51.152087 wagtail-secret-sharing-0.5.0/setup.cfg
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1224 2023-06-02 08:21:29.000000 wagtail-secret-sharing-0.5.0/setup.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:24:51.145700 wagtail-secret-sharing-0.5.0/src/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:24:51.148491 wagtail-secret-sharing-0.5.0/src/wagtail_secret_sharing/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-06-02 07:41:52.000000 wagtail-secret-sharing-0.5.0/src/wagtail_secret_sharing/__init__.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     3515 2023-06-02 08:20:30.000000 wagtail-secret-sharing-0.5.0/src/wagtail_secret_sharing/models.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      152 2023-06-02 07:41:52.000000 wagtail-secret-sharing-0.5.0/src/wagtail_secret_sharing/settings.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:24:51.146017 wagtail-secret-sharing-0.5.0/src/wagtail_secret_sharing/templates/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:24:51.150347 wagtail-secret-sharing-0.5.0/src/wagtail_secret_sharing/templates/wagtail_secret_sharing/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      686 2022-08-11 14:00:23.000000 wagtail-secret-sharing-0.5.0/src/wagtail_secret_sharing/templates/wagtail_secret_sharing/create.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)       98 2022-07-18 08:50:50.000000 wagtail-secret-sharing-0.5.0/src/wagtail_secret_sharing/templates/wagtail_secret_sharing/retrieve.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)      367 2022-08-11 14:00:23.000000 wagtail-secret-sharing-0.5.0/src/wagtail_secret_sharing/templates/wagtail_secret_sharing/view.html
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:24:51.150916 wagtail-secret-sharing-0.5.0/src/wagtail_secret_sharing.egg-info/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      359 2023-06-02 08:24:51.000000 wagtail-secret-sharing-0.5.0/src/wagtail_secret_sharing.egg-info/SOURCES.txt
```

### Comparing `wagtail-secret-sharing-0.4.0/LICENSE` & `wagtail-secret-sharing-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-secret-sharing-0.4.0/PKG-INFO` & `wagtail-secret-sharing-0.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: wagtail-secret-sharing
-Version: 0.4.0
+Version: 0.5.0
 Author: R. Moorman <rob@vicktor.nl>
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Operating System :: Unix
+Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `wagtail-secret-sharing-0.4.0/setup.py` & `wagtail-secret-sharing-0.5.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,29 +10,34 @@
     "pytest",
     "pytest-cov",
     "pytest-django",
 ]
 
 setup(
     name="wagtail-secret-sharing",
-    version="0.4.0",
+    version="0.5.0",
     description="",
     author="R. Moorman <rob@vicktor.nl>",
     install_requires=install_requires,
     tests_requires=tests_requires,
     extras_require={"test": tests_requires},
     package_dir={"": "src"},
     packages=find_packages("src"),
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Django",
         "Operating System :: Unix",
+        "Framework :: Wagtail",
+        "Framework :: Wagtail :: 3",
+        "Framework :: Wagtail :: 4",
+        "Framework :: Wagtail :: 5",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `wagtail-secret-sharing-0.4.0/src/wagtail_secret_sharing/models.py` & `wagtail-secret-sharing-0.5.0/src/wagtail_secret_sharing/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from django.template.response import TemplateResponse
 from django.utils.crypto import get_random_string
 from django_secret_sharing import settings as django_secret_sharing_settings
 from django_secret_sharing.exceptions import SecretNotFound
 from django_secret_sharing.forms import CreateSecretForm
 from django_secret_sharing.utils import create_secret, get_secret_by_url_part
 from wagtail.contrib.routable_page.models import RoutablePageMixin, route
-from wagtail.core.models import Page
+from wagtail.models import Page
 
 
 class AbstractSecretsPage(RoutablePageMixin, Page):
     create_page_template = "wagtail_secret_sharing/create.html"
     retrieve_page_template = "wagtail_secret_sharing/retrieve.html"
     view_page_template = "wagtail_secret_sharing/view.html"
```

### Comparing `wagtail-secret-sharing-0.4.0/src/wagtail_secret_sharing/templates/wagtail_secret_sharing/create.html` & `wagtail-secret-sharing-0.5.0/src/wagtail_secret_sharing/templates/wagtail_secret_sharing/create.html`

 * *Files identical despite different names*

