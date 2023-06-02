# Comparing `tmp/netbox-unacceptable-events-0.1.3.tar.gz` & `tmp/netbox-unacceptable-events-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-unacceptable-events-0.1.3.tar", last modified: Thu Jan 19 22:40:09 2023, max compression
+gzip compressed data, was "netbox-unacceptable-events-0.1.4.tar", last modified: Fri Jun  2 09:08:57 2023, max compression
```

## Comparing `netbox-unacceptable-events-0.1.3.tar` & `netbox-unacceptable-events-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-19 22:40:09.475416 netbox-unacceptable-events-0.1.3/
--rw-rw-r--   0 user      (1000) user      (1000)    11357 2023-01-16 15:39:22.000000 netbox-unacceptable-events-0.1.3/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       34 2023-01-17 08:39:39.000000 netbox-unacceptable-events-0.1.3/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)      972 2023-01-19 22:40:09.475416 netbox-unacceptable-events-0.1.3/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      306 2023-01-18 07:35:37.000000 netbox-unacceptable-events-0.1.3/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-19 22:40:09.471416 netbox-unacceptable-events-0.1.3/netbox_unacceptable_events.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      972 2023-01-19 22:40:09.000000 netbox-unacceptable-events-0.1.3/netbox_unacceptable_events.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1039 2023-01-19 22:40:09.000000 netbox-unacceptable-events-0.1.3/netbox_unacceptable_events.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-01-19 22:40:09.000000 netbox-unacceptable-events-0.1.3/netbox_unacceptable_events.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-01-17 07:10:02.000000 netbox-unacceptable-events-0.1.3/netbox_unacceptable_events.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-01-19 22:40:09.000000 netbox-unacceptable-events-0.1.3/netbox_unacceptable_events.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-19 22:40:09.475416 netbox-unacceptable-events-0.1.3/ptuevents/
--rw-rw-r--   0 user      (1000) user      (1000)      404 2023-01-17 08:39:52.000000 netbox-unacceptable-events-0.1.3/ptuevents/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-19 22:40:09.475416 netbox-unacceptable-events-0.1.3/ptuevents/api/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-24 15:50:18.000000 netbox-unacceptable-events-0.1.3/ptuevents/api/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5004 2023-01-18 07:20:21.000000 netbox-unacceptable-events-0.1.3/ptuevents/api/serializers.py
--rw-rw-r--   0 user      (1000) user      (1000)      500 2023-01-17 13:07:51.000000 netbox-unacceptable-events-0.1.3/ptuevents/api/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     1442 2023-01-19 22:25:09.000000 netbox-unacceptable-events-0.1.3/ptuevents/api/views.py
--rw-rw-r--   0 user      (1000) user      (1000)     1817 2023-01-19 22:26:06.000000 netbox-unacceptable-events-0.1.3/ptuevents/filtersets.py
--rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-01-19 22:16:54.000000 netbox-unacceptable-events-0.1.3/ptuevents/forms.py
--rw-rw-r--   0 user      (1000) user      (1000)     1665 2023-01-19 21:37:38.000000 netbox-unacceptable-events-0.1.3/ptuevents/graphql.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-19 22:40:09.475416 netbox-unacceptable-events-0.1.3/ptuevents/migrations/
--rw-rw-r--   0 user      (1000) user      (1000)     5433 2023-01-17 13:35:06.000000 netbox-unacceptable-events-0.1.3/ptuevents/migrations/0001_initial.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-17 13:35:06.000000 netbox-unacceptable-events-0.1.3/ptuevents/migrations/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4736 2023-01-17 14:01:17.000000 netbox-unacceptable-events-0.1.3/ptuevents/models.py
--rw-rw-r--   0 user      (1000) user      (1000)     1223 2023-01-17 13:21:59.000000 netbox-unacceptable-events-0.1.3/ptuevents/navigation.py
--rw-rw-r--   0 user      (1000) user      (1000)     2179 2023-01-17 13:49:46.000000 netbox-unacceptable-events-0.1.3/ptuevents/tables.py
--rw-rw-r--   0 user      (1000) user      (1000)     3877 2023-01-17 14:20:24.000000 netbox-unacceptable-events-0.1.3/ptuevents/template_content.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-19 22:40:09.471416 netbox-unacceptable-events-0.1.3/ptuevents/templates/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-19 22:40:09.475416 netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/
--rw-rw-r--   0 user      (1000) user      (1000)      604 2023-01-19 22:10:16.000000 netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/appsystem_assignment_edit.html
--rw-rw-r--   0 user      (1000) user      (1000)     1395 2023-01-17 14:25:11.000000 netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/appsystem_panel.html
--rw-rw-r--   0 user      (1000) user      (1000)     1419 2023-01-17 14:07:22.000000 netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/ptappsystem.html
--rw-rw-r--   0 user      (1000) user      (1000)      748 2023-01-17 13:09:14.000000 netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/ptuevent.html
--rw-rw-r--   0 user      (1000) user      (1000)      600 2023-01-17 13:42:03.000000 netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/ptuevent_assignment_edit.html
--rw-rw-r--   0 user      (1000) user      (1000)     1502 2023-01-17 13:38:27.000000 netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/ptuevent_panel.html
--rw-rw-r--   0 user      (1000) user      (1000)      708 2023-01-17 11:14:00.000000 netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/ptueventrelation.html
--rw-rw-r--   0 user      (1000) user      (1000)     3081 2023-01-17 13:21:06.000000 netbox-unacceptable-events-0.1.3/ptuevents/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     5741 2023-01-17 14:28:01.000000 netbox-unacceptable-events-0.1.3/ptuevents/views.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-01-19 22:40:09.475416 netbox-unacceptable-events-0.1.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1014 2023-01-19 22:39:54.000000 netbox-unacceptable-events-0.1.3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:08:57.868792 netbox-unacceptable-events-0.1.4/
+-rw-rw-r--   0 user      (1000) user      (1000)    11357 2023-01-16 15:39:22.000000 netbox-unacceptable-events-0.1.4/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       34 2023-01-17 08:39:39.000000 netbox-unacceptable-events-0.1.4/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)      972 2023-06-02 09:08:57.868792 netbox-unacceptable-events-0.1.4/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      306 2023-01-18 07:35:37.000000 netbox-unacceptable-events-0.1.4/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:08:57.860792 netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      972 2023-06-02 09:08:57.000000 netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1039 2023-06-02 09:08:57.000000 netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-02 09:08:57.000000 netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-01-17 07:10:02.000000 netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-06-02 09:08:57.000000 netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:08:57.864792 netbox-unacceptable-events-0.1.4/ptuevents/
+-rw-rw-r--   0 user      (1000) user      (1000)      404 2023-01-17 08:39:52.000000 netbox-unacceptable-events-0.1.4/ptuevents/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:08:57.864792 netbox-unacceptable-events-0.1.4/ptuevents/api/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-24 15:50:18.000000 netbox-unacceptable-events-0.1.4/ptuevents/api/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5004 2023-01-18 07:20:21.000000 netbox-unacceptable-events-0.1.4/ptuevents/api/serializers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      500 2023-01-17 13:07:51.000000 netbox-unacceptable-events-0.1.4/ptuevents/api/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1442 2023-01-19 22:25:09.000000 netbox-unacceptable-events-0.1.4/ptuevents/api/views.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1817 2023-01-19 22:26:06.000000 netbox-unacceptable-events-0.1.4/ptuevents/filtersets.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1582 2023-05-26 10:25:54.000000 netbox-unacceptable-events-0.1.4/ptuevents/forms.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1665 2023-01-19 21:37:38.000000 netbox-unacceptable-events-0.1.4/ptuevents/graphql.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:08:57.868792 netbox-unacceptable-events-0.1.4/ptuevents/migrations/
+-rw-rw-r--   0 user      (1000) user      (1000)     5433 2023-01-17 13:35:06.000000 netbox-unacceptable-events-0.1.4/ptuevents/migrations/0001_initial.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-17 13:35:06.000000 netbox-unacceptable-events-0.1.4/ptuevents/migrations/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4736 2023-05-26 08:55:41.000000 netbox-unacceptable-events-0.1.4/ptuevents/models.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1223 2023-01-17 13:21:59.000000 netbox-unacceptable-events-0.1.4/ptuevents/navigation.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2179 2023-01-17 13:49:46.000000 netbox-unacceptable-events-0.1.4/ptuevents/tables.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3877 2023-01-17 14:20:24.000000 netbox-unacceptable-events-0.1.4/ptuevents/template_content.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:08:57.860792 netbox-unacceptable-events-0.1.4/ptuevents/templates/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:08:57.868792 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/
+-rw-rw-r--   0 user      (1000) user      (1000)      604 2023-01-19 22:10:16.000000 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/appsystem_assignment_edit.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1395 2023-01-17 14:25:11.000000 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/appsystem_panel.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1419 2023-01-17 14:07:22.000000 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptappsystem.html
+-rw-rw-r--   0 user      (1000) user      (1000)      748 2023-01-17 13:09:14.000000 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptuevent.html
+-rw-rw-r--   0 user      (1000) user      (1000)      600 2023-01-17 13:42:03.000000 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptuevent_assignment_edit.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1502 2023-01-17 13:38:27.000000 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptuevent_panel.html
+-rw-rw-r--   0 user      (1000) user      (1000)      708 2023-01-17 11:14:00.000000 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptueventrelation.html
+-rw-rw-r--   0 user      (1000) user      (1000)     3081 2023-01-17 13:21:06.000000 netbox-unacceptable-events-0.1.4/ptuevents/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5741 2023-01-17 14:28:01.000000 netbox-unacceptable-events-0.1.4/ptuevents/views.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-02 09:08:57.868792 netbox-unacceptable-events-0.1.4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1014 2023-06-02 07:56:30.000000 netbox-unacceptable-events-0.1.4/setup.py
```

### Comparing `netbox-unacceptable-events-0.1.3/LICENSE` & `netbox-unacceptable-events-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/PKG-INFO` & `netbox-unacceptable-events-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-unacceptable-events
-Version: 0.1.3
+Version: 0.1.4
 Summary: Netbox plugin. Assign devices and virtual machines and application systems to information security unacceptable events
 Download-URL: https://pypi.org/project/netbox-unacceptable-events/
 Author: Oleg Senchenko
 Author-email: senchenkoob@mail.ru
 Maintainer: Oleg Senchenko
 Maintainer-email: senchenkoob@mail.ru
 License: MIT
```

### Comparing `netbox-unacceptable-events-0.1.3/netbox_unacceptable_events.egg-info/PKG-INFO` & `netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-unacceptable-events
-Version: 0.1.3
+Version: 0.1.4
 Summary: Netbox plugin. Assign devices and virtual machines and application systems to information security unacceptable events
 Download-URL: https://pypi.org/project/netbox-unacceptable-events/
 Author: Oleg Senchenko
 Author-email: senchenkoob@mail.ru
 Maintainer: Oleg Senchenko
 Maintainer-email: senchenkoob@mail.ru
 License: MIT
```

### Comparing `netbox-unacceptable-events-0.1.3/netbox_unacceptable_events.egg-info/SOURCES.txt` & `netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/api/serializers.py` & `netbox-unacceptable-events-0.1.4/ptuevents/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/api/views.py` & `netbox-unacceptable-events-0.1.4/ptuevents/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/filtersets.py` & `netbox-unacceptable-events-0.1.4/ptuevents/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/forms.py` & `netbox-unacceptable-events-0.1.4/ptuevents/forms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from netbox.forms import NetBoxModelForm
 from tenancy.models import Tenant
 from pyrsistent import v
 from .models import PTUEvent, PTUEventRelation, PTUEventAssignment, PTAppSystem, PTAppSystemAssignment
 from utilities.forms.fields import CommentField
-from utilities.forms import (
-    BootstrapMixin, DynamicModelChoiceField)
+from utilities.forms import BootstrapMixin
+from utilities.forms.fields import DynamicModelChoiceField
 from django import forms
 
 
 class PTUEventForm(NetBoxModelForm):
     class Meta:
         model = PTUEvent
         fields = ('name', 'description', 'comments')
```

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/graphql.py` & `netbox-unacceptable-events-0.1.4/ptuevents/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/migrations/0001_initial.py` & `netbox-unacceptable-events-0.1.4/ptuevents/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/models.py` & `netbox-unacceptable-events-0.1.4/ptuevents/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         # return 'reskrel'
         return self.name
 
     def get_absolute_url(self):
         return reverse('plugins:ptuevents:ptueventrelation', args=[self.pk])
 
 
-class PTUEventAssignment(WebhooksMixin, ChangeLoggedModel):
+class PTUEventAssignment(ChangeLoggedModel, WebhooksMixin):
     content_type = models.ForeignKey(
         to=ContentType,
         on_delete=models.CASCADE
     )
     object_id = models.PositiveBigIntegerField()
     object = GenericForeignKey(
         ct_field='content_type',
@@ -121,15 +121,15 @@
         return reverse('plugins:ptuevents:ptappsystem', args=[self.pk])
 
     class Meta:
         ordering = ['name']
         verbose_name_plural = 'Application systems'
 
 
-class PTAppSystemAssignment(WebhooksMixin, ChangeLoggedModel):
+class PTAppSystemAssignment(ChangeLoggedModel, WebhooksMixin):
     content_type = models.ForeignKey(
         to=ContentType,
         on_delete=models.CASCADE
     )
     object_id = models.PositiveBigIntegerField()
     object = GenericForeignKey(
         ct_field='content_type',
```

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/navigation.py` & `netbox-unacceptable-events-0.1.4/ptuevents/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/tables.py` & `netbox-unacceptable-events-0.1.4/ptuevents/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/template_content.py` & `netbox-unacceptable-events-0.1.4/ptuevents/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/appsystem_assignment_edit.html` & `netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/appsystem_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/appsystem_panel.html` & `netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/appsystem_panel.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/ptappsystem.html` & `netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptappsystem.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/ptuevent.html` & `netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptuevent.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/ptuevent_assignment_edit.html` & `netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptuevent_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/ptuevent_panel.html` & `netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptuevent_panel.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/templates/ptuevents/ptueventrelation.html` & `netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptueventrelation.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/urls.py` & `netbox-unacceptable-events-0.1.4/ptuevents/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/ptuevents/views.py` & `netbox-unacceptable-events-0.1.4/ptuevents/views.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.3/setup.py` & `netbox-unacceptable-events-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='netbox-unacceptable-events',
-    version='0.1.3',
+    version='0.1.4',
     description='Netbox plugin. Assign devices and virtual machines and application systems to information security unacceptable events',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
     download_url='https://pypi.org/project/netbox-unacceptable-events/',
     packages=find_packages(),
     include_package_data=True,
```

