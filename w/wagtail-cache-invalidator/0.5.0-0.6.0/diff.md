# Comparing `tmp/wagtail-cache-invalidator-0.5.0.tar.gz` & `tmp/wagtail-cache-invalidator-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-cache-invalidator-0.5.0.tar", last modified: Thu Apr 13 12:34:49 2023, max compression
+gzip compressed data, was "wagtail-cache-invalidator-0.6.0.tar", last modified: Fri Jun  2 08:24:28 2023, max compression
```

## Comparing `wagtail-cache-invalidator-0.5.0.tar` & `wagtail-cache-invalidator-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-13 12:34:49.846361 wagtail-cache-invalidator-0.5.0/
--rw-r--r--   0 robmoorman   (501) staff       (20)      164 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.5.0/MANIFEST.in
--rw-r--r--   0 robmoorman   (501) staff       (20)      285 2023-04-13 12:34:49.845875 wagtail-cache-invalidator-0.5.0/PKG-INFO
--rw-r--r--   0 robmoorman   (501) staff       (20)       38 2023-04-13 12:34:49.846499 wagtail-cache-invalidator-0.5.0/setup.cfg
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-13 12:34:49.836440 wagtail-cache-invalidator-0.5.0/src/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-13 12:34:49.841432 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/
--rw-r--r--   0 robmoorman   (501) staff       (20)       87 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/__init__.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      178 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/admin_urls.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      406 2022-08-19 11:53:10.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/apps.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      547 2022-11-25 13:22:25.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/forms.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-13 12:34:49.844411 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/
--rw-r--r--   0 robmoorman   (501) staff       (20)     1550 2023-04-13 11:29:31.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/0001_initial.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     1807 2023-04-13 11:29:31.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/0002_cachesettings.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      559 2023-04-13 11:29:31.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/0003_purgecachesite.py
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/__init__.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     3746 2023-04-13 11:48:09.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/models.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      200 2023-04-13 11:37:45.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/settings.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     1033 2023-04-13 12:24:47.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/signal_handlers.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      356 2023-04-13 11:37:51.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/signals.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-13 12:34:49.836924 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/templates/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-13 12:34:49.844790 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/templates/ wagtailcacheinvalidator/
--rw-r--r--   0 robmoorman   (501) staff       (20)     2051 2022-11-25 13:12:14.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/templates/ wagtailcacheinvalidator/purge.html
--rw-r--r--   0 robmoorman   (501) staff       (20)     1107 2023-04-13 11:57:44.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/utils.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     1623 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/views.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     2652 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/wagtail_hooks.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-13 12:34:49.845395 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator.egg-info/
--rw-r--r--   0 robmoorman   (501) staff       (20)      784 2023-04-13 12:34:49.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator.egg-info/SOURCES.txt
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:24:28.424623 wagtail-cache-invalidator-0.6.0/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      164 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.6.0/MANIFEST.in
+-rw-r--r--   0 robmoorman   (501) staff       (20)      701 2023-06-02 08:24:28.424308 wagtail-cache-invalidator-0.6.0/PKG-INFO
+-rw-r--r--   0 robmoorman   (501) staff       (20)       38 2023-06-02 08:24:28.424703 wagtail-cache-invalidator-0.6.0/setup.cfg
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:24:28.413756 wagtail-cache-invalidator-0.6.0/src/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:24:28.420920 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/
+-rw-r--r--   0 robmoorman   (501) staff       (20)       87 2023-06-01 15:17:21.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/__init__.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      178 2023-06-01 15:17:21.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/admin_urls.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      406 2023-06-01 15:17:21.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/apps.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      547 2023-06-01 15:17:21.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/forms.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:24:28.423121 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/migrations/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1550 2023-06-01 15:17:21.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/migrations/0001_initial.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1807 2023-06-01 15:17:21.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/migrations/0002_cachesettings.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      559 2023-06-01 15:17:21.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/migrations/0003_purgecachesite.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-06-01 15:17:21.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/migrations/__init__.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     3742 2023-06-02 08:20:20.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/models.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      200 2023-06-01 15:17:21.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/settings.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1028 2023-06-02 08:20:20.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/signal_handlers.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      356 2023-06-01 15:17:21.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/signals.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:24:28.414404 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/templates/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:24:28.423431 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/templates/ wagtailcacheinvalidator/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2051 2022-11-25 13:12:14.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/templates/ wagtailcacheinvalidator/purge.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1107 2023-06-01 15:17:21.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/utils.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1618 2023-06-02 08:20:20.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/views.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2647 2023-06-02 08:20:20.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/wagtail_hooks.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:24:28.423967 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator.egg-info/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      784 2023-06-02 08:24:28.000000 wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator.egg-info/SOURCES.txt
```

### Comparing `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/forms.py` & `wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/0001_initial.py` & `wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/0002_cachesettings.py` & `wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/migrations/0002_cachesettings.py`

 * *Files identical despite different names*

### Comparing `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/0003_purgecachesite.py` & `wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/migrations/0003_purgecachesite.py`

 * *Files identical despite different names*

### Comparing `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/models.py` & `wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import uuid
 
 from django.conf import settings
 from django.db import models
 from django.db.models.signals import m2m_changed
 from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
-from wagtail.admin.edit_handlers import (
+from wagtail.admin.panels import (
     FieldPanel,
     MultiFieldPanel,
     ObjectList,
     TabbedInterface,
 )
-from wagtail.contrib.settings.models import BaseSetting, register_setting
-from wagtail.core.models import Site
+from wagtail.contrib.settings.models import BaseSiteSetting, register_setting
+from wagtail.models import Site
 
 from wagtail_cache_invalidator import signals
 from wagtail_cache_invalidator.settings import ASYNC
 from wagtail_cache_invalidator.utils import purge_urls_from_cache
 
 PURGE_ALL_HELP_TXT = _("Purge all cache for this site when pages are (un)published")
 
@@ -31,15 +31,15 @@
             result += ":{}".format(self.port)
         if self.is_default_site:
             result += " [{}]".format(_("default"))
         return result
 
 
 @register_setting
-class CacheSettings(BaseSetting):
+class CacheSettings(BaseSiteSetting):
     purge_all = models.BooleanField(
         verbose_name=_("purge all"), default=False, help_text=PURGE_ALL_HELP_TXT
     )
 
     cloudfront_enabled = models.BooleanField(verbose_name=_("enabled"), default=False)
     cloudfront_distribution_id = models.CharField(
         verbose_name=_("distribution ID"), max_length=255
```

### Comparing `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/signal_handlers.py` & `wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/signal_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.apps import apps
-from wagtail.core.signals import page_published, page_unpublished
+from wagtail.signals import page_published, page_unpublished
 
 from wagtail_cache_invalidator import signals
 from wagtail_cache_invalidator.settings import ASYNC
 from wagtail_cache_invalidator.utils import purge_page_from_cache
 
 
 def page_published_signal_handler(instance, **kwargs):
```

### Comparing `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/templates/ wagtailcacheinvalidator/purge.html` & `wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/templates/ wagtailcacheinvalidator/purge.html`

 * *Files identical despite different names*

### Comparing `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/utils.py` & `wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/views.py` & `wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.contrib import messages
 from django.http import HttpResponseRedirect
 from django.template.response import TemplateResponse
 from django.utils import timezone
 from django.utils.translation import gettext as _
 from wagtail.admin.auth import permission_required
-from wagtail.core.models import Site
+from wagtail.models import Site
 
 from wagtail_cache_invalidator.forms import PurgeForm
 from wagtail_cache_invalidator.models import InvalidationRequest
 
 
 @permission_required("wagtailcacheinvalidator.add_invalidationrequest")
 def purge(request):
```

### Comparing `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/wagtail_hooks.py` & `wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator/wagtail_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from django.contrib.auth.models import Permission
 from django.urls import include, path, reverse
 from django.utils.translation import gettext_lazy as _
+from wagtail import hooks
 from wagtail.admin.menu import Menu, MenuItem, SubmenuMenuItem
 from wagtail.contrib.modeladmin.helpers.permission import PermissionHelper
 from wagtail.contrib.modeladmin.options import (
     ModelAdmin,
     ModelAdminGroup,
     modeladmin_register,
 )
-from wagtail.core import hooks
 
 from wagtail_cache_invalidator.models import InvalidationRequest
 
 
 @hooks.register("register_admin_urls")
 def register_admin_urls():
     return [
```

### Comparing `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator.egg-info/SOURCES.txt` & `wagtail-cache-invalidator-0.6.0/src/wagtail_cache_invalidator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

