# Comparing `tmp/wagtail-analytics-0.4.0.tar.gz` & `tmp/wagtail-analytics-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-analytics-0.4.0.tar", last modified: Wed Mar 15 15:22:20 2023, max compression
+gzip compressed data, was "wagtail-analytics-0.5.0.tar", last modified: Fri Jun  2 08:23:19 2023, max compression
```

## Comparing `wagtail-analytics-0.4.0.tar` & `wagtail-analytics-0.5.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-03-15 15:22:20.470708 wagtail-analytics-0.4.0/
--rw-r--r--   0 robmoorman   (501) staff       (20)      156 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/MANIFEST.in
--rw-r--r--   0 robmoorman   (501) staff       (20)      256 2023-03-15 15:22:20.470159 wagtail-analytics-0.4.0/PKG-INFO
--rw-r--r--   0 robmoorman   (501) staff       (20)       38 2023-03-15 15:22:20.470849 wagtail-analytics-0.4.0/setup.cfg
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-03-15 15:22:20.438478 wagtail-analytics-0.4.0/src/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-03-15 15:22:20.444832 wagtail-analytics-0.4.0/src/wagtail_analytics/
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/__init__.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      298 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/forms.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-03-15 15:22:20.445840 wagtail-analytics-0.4.0/src/wagtail_analytics/lib/
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-03-15 14:49:20.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/lib/__init__.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     7714 2023-03-15 14:52:09.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/lib/analytics.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-03-15 15:22:20.446496 wagtail-analytics-0.4.0/src/wagtail_analytics/locales/
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/locales/.gitkeep
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-03-15 15:22:20.450819 wagtail-analytics-0.4.0/src/wagtail_analytics/migrations/
--rw-r--r--   0 robmoorman   (501) staff       (20)     2484 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/migrations/0001_initial.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      556 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/migrations/0002_analyticssettings_google_site_verification.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      477 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/migrations/0003_analyticssettings_plausible_enabled.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      520 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/migrations/0004_analyticssettings_plausible_domain.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      383 2023-03-15 14:40:10.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/migrations/0005_remove_analyticssettings_google_analytics_view_id.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      612 2023-03-15 15:19:55.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/migrations/0006_analyticssettings_google_analytics_measurement_id.py
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/migrations/__init__.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     2877 2023-03-15 15:19:04.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/models.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      505 2023-03-15 14:40:10.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/settings.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-03-15 15:22:20.440302 wagtail-analytics-0.4.0/src/wagtail_analytics/static/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-03-15 15:22:20.463429 wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/
--rw-r--r--   0 robmoorman   (501) staff       (20)   579244 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/Chart.bundle.js
--rw-r--r--   0 robmoorman   (501) staff       (20)   226227 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/Chart.bundle.min.js
--rw-r--r--   0 robmoorman   (501) staff       (20)      811 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/Chart.css
--rw-r--r--   0 robmoorman   (501) staff       (20)   428366 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/Chart.js
--rw-r--r--   0 robmoorman   (501) staff       (20)      521 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/Chart.min.css
--rw-r--r--   0 robmoorman   (501) staff       (20)   172812 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/Chart.min.js
--rw-r--r--   0 robmoorman   (501) staff       (20)     1088 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/LICENSE.md
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-03-15 15:22:20.464005 wagtail-analytics-0.4.0/src/wagtail_analytics/static/moment/
--rwxr-xr-x   0 robmoorman   (501) staff       (20)    58824 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/static/moment/moment.min.js
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-03-15 15:22:20.466434 wagtail-analytics-0.4.0/src/wagtail_analytics/static/wagtailanalytics/
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/static/wagtailanalytics/.gitkeep
--rw-r--r--   0 robmoorman   (501) staff       (20)       60 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/static/wagtailanalytics/main.css
--rw-r--r--   0 robmoorman   (501) staff       (20)     2357 2023-03-15 15:11:00.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/static/wagtailanalytics/main.js
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-03-15 15:22:20.440716 wagtail-analytics-0.4.0/src/wagtail_analytics/templates/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-03-15 15:22:20.468232 wagtail-analytics-0.4.0/src/wagtail_analytics/templates/wagtail_analytics/
--rw-r--r--   0 robmoorman   (501) staff       (20)      462 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/templates/wagtail_analytics/body.html
--rw-r--r--   0 robmoorman   (501) staff       (20)     2527 2023-03-15 15:10:05.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/templates/wagtail_analytics/dashboard.html
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-03-15 15:22:20.468972 wagtail-analytics-0.4.0/src/wagtail_analytics/templates/wagtail_analytics/edit_handlers/
--rw-r--r--   0 robmoorman   (501) staff       (20)     1029 2023-02-24 13:01:45.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/templates/wagtail_analytics/edit_handlers/sessions.html
--rw-r--r--   0 robmoorman   (501) staff       (20)     1439 2023-03-15 15:19:37.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/templates/wagtail_analytics/head.html
--rw-r--r--   0 robmoorman   (501) staff       (20)      416 2023-03-15 14:53:40.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/types.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     4260 2023-03-15 15:09:59.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/views.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     2689 2023-03-15 14:40:10.000000 wagtail-analytics-0.4.0/src/wagtail_analytics/wagtail_hooks.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-03-15 15:22:20.469559 wagtail-analytics-0.4.0/src/wagtail_analytics.egg-info/
--rw-r--r--   0 robmoorman   (501) staff       (20)     1708 2023-03-15 15:22:20.000000 wagtail-analytics-0.4.0/src/wagtail_analytics.egg-info/SOURCES.txt
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.954166 wagtail-analytics-0.5.0/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      156 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/MANIFEST.in
+-rw-r--r--   0 robmoorman   (501) staff       (20)      672 2023-06-02 08:23:19.953436 wagtail-analytics-0.5.0/PKG-INFO
+-rw-r--r--   0 robmoorman   (501) staff       (20)       38 2023-06-02 08:23:19.954394 wagtail-analytics-0.5.0/setup.cfg
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.924188 wagtail-analytics-0.5.0/src/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.929609 wagtail-analytics-0.5.0/src/wagtail_analytics/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/__init__.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      298 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/forms.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.930307 wagtail-analytics-0.5.0/src/wagtail_analytics/lib/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/lib/__init__.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     7714 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/lib/analytics.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.930672 wagtail-analytics-0.5.0/src/wagtail_analytics/locales/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/locales/.gitkeep
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.935124 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2484 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0001_initial.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      556 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0002_analyticssettings_google_site_verification.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      477 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0003_analyticssettings_plausible_enabled.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      520 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0004_analyticssettings_plausible_domain.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      383 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0005_remove_analyticssettings_google_analytics_view_id.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      612 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0006_analyticssettings_google_analytics_measurement_id.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/__init__.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2878 2023-06-02 08:20:10.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/models.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      505 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/settings.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.925610 wagtail-analytics-0.5.0/src/wagtail_analytics/static/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.946895 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/
+-rw-r--r--   0 robmoorman   (501) staff       (20)   579244 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.bundle.js
+-rw-r--r--   0 robmoorman   (501) staff       (20)   226227 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.bundle.min.js
+-rw-r--r--   0 robmoorman   (501) staff       (20)      811 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.css
+-rw-r--r--   0 robmoorman   (501) staff       (20)   428366 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.js
+-rw-r--r--   0 robmoorman   (501) staff       (20)      521 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.min.css
+-rw-r--r--   0 robmoorman   (501) staff       (20)   172812 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.min.js
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1088 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/LICENSE.md
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.947445 wagtail-analytics-0.5.0/src/wagtail_analytics/static/moment/
+-rwxr-xr-x   0 robmoorman   (501) staff       (20)    58824 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/moment/moment.min.js
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.949945 wagtail-analytics-0.5.0/src/wagtail_analytics/static/wagtailanalytics/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/wagtailanalytics/.gitkeep
+-rw-r--r--   0 robmoorman   (501) staff       (20)       60 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/wagtailanalytics/main.css
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2357 2023-03-15 15:11:00.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/wagtailanalytics/main.js
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.925947 wagtail-analytics-0.5.0/src/wagtail_analytics/templates/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.951737 wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      462 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/body.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2527 2023-03-15 15:10:05.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/dashboard.html
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.952259 wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/edit_handlers/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1029 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/edit_handlers/sessions.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1439 2023-03-15 15:19:37.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/head.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)      416 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/types.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     4248 2023-06-02 08:20:10.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/views.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2684 2023-06-02 08:20:10.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/wagtail_hooks.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.952847 wagtail-analytics-0.5.0/src/wagtail_analytics.egg-info/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1708 2023-06-02 08:23:19.000000 wagtail-analytics-0.5.0/src/wagtail_analytics.egg-info/SOURCES.txt
```

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/lib/analytics.py` & `wagtail-analytics-0.5.0/src/wagtail_analytics/lib/analytics.py`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/migrations/0001_initial.py` & `wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/migrations/0002_analyticssettings_google_site_verification.py` & `wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0002_analyticssettings_google_site_verification.py`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/migrations/0004_analyticssettings_plausible_domain.py` & `wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0004_analyticssettings_plausible_domain.py`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/migrations/0006_analyticssettings_google_analytics_measurement_id.py` & `wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0006_analyticssettings_google_analytics_measurement_id.py`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/models.py` & `wagtail-analytics-0.5.0/src/wagtail_analytics/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 from django.utils.translation import pgettext_lazy
-from wagtail.admin.edit_handlers import FieldPanel, HelpPanel, MultiFieldPanel
-from wagtail.contrib.settings.models import BaseSetting, register_setting
+from wagtail.admin.panels import FieldPanel, HelpPanel, MultiFieldPanel
+from wagtail.contrib.settings.models import BaseSiteSetting, register_setting
 
 from wagtail_analytics import settings
 
 
 @register_setting(icon="view")
-class AnalyticsSettings(BaseSetting):
+class AnalyticsSettings(BaseSiteSetting):
     id = models.AutoField(primary_key=True, auto_created=True, verbose_name="ID")
 
     #: plausible
     plausible_enabled = models.BooleanField(
         verbose_name=_("Plausible Enabled"), default=False
     )
     plausible_domain = models.CharField(
```

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/Chart.bundle.js` & `wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.bundle.js`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/Chart.bundle.min.js` & `wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.bundle.min.js`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/Chart.css` & `wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.css`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/Chart.js` & `wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.js`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/Chart.min.css` & `wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.min.css`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/Chart.min.js` & `wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.min.js`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/static/chart.js/LICENSE.md` & `wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/static/moment/moment.min.js` & `wagtail-analytics-0.5.0/src/wagtail_analytics/static/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/static/wagtailanalytics/main.js` & `wagtail-analytics-0.5.0/src/wagtail_analytics/static/wagtailanalytics/main.js`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/templates/wagtail_analytics/dashboard.html` & `wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/dashboard.html`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/templates/wagtail_analytics/edit_handlers/sessions.html` & `wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/edit_handlers/sessions.html`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/templates/wagtail_analytics/head.html` & `wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/head.html`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/views.py` & `wagtail-analytics-0.5.0/src/wagtail_analytics/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from django.shortcuts import get_object_or_404, redirect
 from django.template.loader import render_to_string
 from django.urls import reverse
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 from django.views import View
 from django.views.generic import TemplateView
-from wagtail.admin.edit_handlers import HelpPanel, ObjectList, TabbedInterface
-from wagtail.core.models import Page, Site
+from wagtail.admin.panels import HelpPanel, ObjectList, TabbedInterface
+from wagtail.models import Page, Site
 
 from wagtail_analytics import settings as wagtail_analytics_settings
 from wagtail_analytics.forms import SiteSwitchForm
 from wagtail_analytics.lib.analytics import GoogleAnalyticsAPIClient, PlausibleAPIClient
 from wagtail_analytics.models import AnalyticsSettings
```

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics/wagtail_hooks.py` & `wagtail-analytics-0.5.0/src/wagtail_analytics/wagtail_hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.templatetags.static import static
 from django.urls import include, path, re_path, reverse
 from django.utils.html import format_html, format_html_join
 from django.utils.translation import gettext_lazy as _
+from wagtail import hooks
 from wagtail.admin.menu import Menu, MenuItem, SubmenuMenuItem
-from wagtail.core import hooks
 
 from wagtail_analytics import settings as wagtail_analytics_settings
 from wagtail_analytics import views
 
 wagtail_analytics_menu = Menu(
     register_hook_name="register_wagtail_analytics_menu_item",
     construct_hook_name="construct_wagtail_analytics_menu",
```

### Comparing `wagtail-analytics-0.4.0/src/wagtail_analytics.egg-info/SOURCES.txt` & `wagtail-analytics-0.5.0/src/wagtail_analytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

