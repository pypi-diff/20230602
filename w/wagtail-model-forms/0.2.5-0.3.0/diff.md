# Comparing `tmp/wagtail-model-forms-0.2.5.tar.gz` & `tmp/wagtail-model-forms-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-model-forms-0.2.5.tar", last modified: Mon May 22 15:07:08 2023, max compression
+gzip compressed data, was "wagtail-model-forms-0.3.0.tar", last modified: Fri Jun  2 08:25:12 2023, max compression
```

## Comparing `wagtail-model-forms-0.2.5.tar` & `wagtail-model-forms-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-22 15:07:08.140406 wagtail-model-forms-0.2.5/
--rw-r--r--   0 robmoorman   (501) staff       (20)     1064 2022-07-18 08:50:50.000000 wagtail-model-forms-0.2.5/LICENSE
--rw-r--r--   0 robmoorman   (501) staff       (20)      175 2022-08-04 10:38:05.000000 wagtail-model-forms-0.2.5/MANIFEST.in
--rw-r--r--   0 robmoorman   (501) staff       (20)      553 2023-05-22 15:07:08.140097 wagtail-model-forms-0.2.5/PKG-INFO
--rw-r--r--   0 robmoorman   (501) staff       (20)       38 2023-05-22 15:07:08.140498 wagtail-model-forms-0.2.5/setup.cfg
--rw-r--r--   0 robmoorman   (501) staff       (20)      996 2023-05-22 15:06:40.000000 wagtail-model-forms-0.2.5/setup.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-22 15:07:08.135020 wagtail-model-forms-0.2.5/src/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-22 15:07:08.138605 wagtail-model-forms-0.2.5/src/wagtail_model_forms/
--rw-r--r--   0 robmoorman   (501) staff       (20)     1160 2022-08-04 13:25:28.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/__init__.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     1056 2022-08-04 15:10:39.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/blocks.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     1431 2023-04-24 09:03:30.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/mixins.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     2892 2022-12-13 09:18:55.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/models.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      390 2022-08-04 15:10:39.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/settings.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-22 15:07:08.135304 wagtail-model-forms-0.2.5/src/wagtail_model_forms/templates/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-22 15:07:08.139259 wagtail-model-forms-0.2.5/src/wagtail_model_forms/templates/wagtail_model_forms/
--rw-r--r--   0 robmoorman   (501) staff       (20)      299 2022-08-04 13:28:34.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/templates/wagtail_model_forms/form.html
--rw-r--r--   0 robmoorman   (501) staff       (20)     1755 2022-08-04 15:10:39.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/templates/wagtail_model_forms/form_submissions_report.html
--rw-r--r--   0 robmoorman   (501) staff       (20)     1347 2023-04-24 09:04:42.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/views.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      928 2023-05-22 15:06:49.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms/wagtail_hooks.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-22 15:07:08.139711 wagtail-model-forms-0.2.5/src/wagtail_model_forms.egg-info/
--rw-r--r--   0 robmoorman   (501) staff       (20)      423 2023-05-22 15:07:08.000000 wagtail-model-forms-0.2.5/src/wagtail_model_forms.egg-info/SOURCES.txt
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:25:12.972526 wagtail-model-forms-0.3.0/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1064 2022-07-18 08:50:50.000000 wagtail-model-forms-0.3.0/LICENSE
+-rw-r--r--   0 robmoorman   (501) staff       (20)      175 2022-08-04 10:38:05.000000 wagtail-model-forms-0.3.0/MANIFEST.in
+-rw-r--r--   0 robmoorman   (501) staff       (20)      718 2023-06-02 08:25:12.972152 wagtail-model-forms-0.3.0/PKG-INFO
+-rw-r--r--   0 robmoorman   (501) staff       (20)       38 2023-06-02 08:25:12.972609 wagtail-model-forms-0.3.0/setup.cfg
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1157 2023-06-02 08:20:58.000000 wagtail-model-forms-0.3.0/setup.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:25:12.964710 wagtail-model-forms-0.3.0/src/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:25:12.970051 wagtail-model-forms-0.3.0/src/wagtail_model_forms/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1160 2023-06-02 07:46:38.000000 wagtail-model-forms-0.3.0/src/wagtail_model_forms/__init__.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1051 2023-06-02 08:20:49.000000 wagtail-model-forms-0.3.0/src/wagtail_model_forms/blocks.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1431 2023-06-02 07:46:38.000000 wagtail-model-forms-0.3.0/src/wagtail_model_forms/mixins.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2885 2023-06-02 08:20:49.000000 wagtail-model-forms-0.3.0/src/wagtail_model_forms/models.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      390 2023-06-02 07:46:38.000000 wagtail-model-forms-0.3.0/src/wagtail_model_forms/settings.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:25:12.965097 wagtail-model-forms-0.3.0/src/wagtail_model_forms/templates/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:25:12.971168 wagtail-model-forms-0.3.0/src/wagtail_model_forms/templates/wagtail_model_forms/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      299 2022-08-04 13:28:34.000000 wagtail-model-forms-0.3.0/src/wagtail_model_forms/templates/wagtail_model_forms/form.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1755 2022-08-04 15:10:39.000000 wagtail-model-forms-0.3.0/src/wagtail_model_forms/templates/wagtail_model_forms/form_submissions_report.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1347 2023-06-02 07:46:38.000000 wagtail-model-forms-0.3.0/src/wagtail_model_forms/views.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      923 2023-06-02 08:20:49.000000 wagtail-model-forms-0.3.0/src/wagtail_model_forms/wagtail_hooks.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:25:12.971777 wagtail-model-forms-0.3.0/src/wagtail_model_forms.egg-info/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      423 2023-06-02 08:25:12.000000 wagtail-model-forms-0.3.0/src/wagtail_model_forms.egg-info/SOURCES.txt
```

### Comparing `wagtail-model-forms-0.2.5/LICENSE` & `wagtail-model-forms-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-model-forms-0.2.5/PKG-INFO` & `wagtail-model-forms-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: wagtail-model-forms
-Version: 0.2.5
+Version: 0.3.0
 Author: R. Moorman <rob@vicktor.nl>
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Operating System :: Unix
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

### Comparing `wagtail-model-forms-0.2.5/setup.py` & `wagtail-model-forms-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,29 +10,33 @@
     "pytest",
     "pytest-cov",
     "pytest-django",
 ]
 
 setup(
     name="wagtail-model-forms",
-    version="0.2.5",
+    version="0.3.0",
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

### Comparing `wagtail-model-forms-0.2.5/src/wagtail_model_forms/__init__.py` & `wagtail-model-forms-0.3.0/src/wagtail_model_forms/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail-model-forms-0.2.5/src/wagtail_model_forms/blocks.py` & `wagtail-model-forms-0.3.0/src/wagtail_model_forms/blocks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from wagtail.core import blocks
+from wagtail import blocks
 from wagtail.snippets.blocks import SnippetChooserBlock
 
 from wagtail_model_forms.settings import FORM_MODEL
 
 
 class AbstractFormBlock(blocks.StructBlock):
     form = SnippetChooserBlock(FORM_MODEL)
```

### Comparing `wagtail-model-forms-0.2.5/src/wagtail_model_forms/mixins.py` & `wagtail-model-forms-0.3.0/src/wagtail_model_forms/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail-model-forms-0.2.5/src/wagtail_model_forms/models.py` & `wagtail-model-forms-0.3.0/src/wagtail_model_forms/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db import models
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 from modelcluster.fields import ParentalKey
 from modelcluster.models import ClusterableModel
-from wagtail.admin.edit_handlers import (
+from wagtail.admin.panels import (
     FieldPanel,
     InlinePanel,
     ObjectList,
     TabbedInterface,
 )
 from wagtail.contrib.forms.forms import FormBuilder
 from wagtail.contrib.forms.models import (
```

### Comparing `wagtail-model-forms-0.2.5/src/wagtail_model_forms/templates/wagtail_model_forms/form_submissions_report.html` & `wagtail-model-forms-0.3.0/src/wagtail_model_forms/templates/wagtail_model_forms/form_submissions_report.html`

 * *Files identical despite different names*

### Comparing `wagtail-model-forms-0.2.5/src/wagtail_model_forms/views.py` & `wagtail-model-forms-0.3.0/src/wagtail_model_forms/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-model-forms-0.2.5/src/wagtail_model_forms/wagtail_hooks.py` & `wagtail-model-forms-0.3.0/src/wagtail_model_forms/wagtail_hooks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.urls import path, reverse
+from wagtail import hooks
 from wagtail.admin.menu import MenuItem
-from wagtail.core import hooks
 
 from wagtail_model_forms.settings import REPORTS
 from wagtail_model_forms.views import FormSubmissionReportView
 
 
 class ReportsMenuItem(MenuItem):
     def is_shown(self, request):
```

