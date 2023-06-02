# Comparing `tmp/django-hydrothings-0.1.5.tar.gz` & `tmp/django-hydrothings-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-hydrothings-0.1.5.tar", last modified: Wed Apr 19 23:19:55 2023, max compression
+gzip compressed data, was "django-hydrothings-0.1.6.tar", last modified: Fri Jun  2 16:22:04 2023, max compression
```

## Comparing `django-hydrothings-0.1.5.tar` & `django-hydrothings-0.1.6.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.410374 django-hydrothings-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-19 23:19:55.410374 django-hydrothings-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-19 23:19:55.410374 django-hydrothings-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.398373 django-hydrothings-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.398373 django-hydrothings-0.1.5/src/django_hydrothings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-19 23:19:55.000000 django-hydrothings-0.1.5/src/django_hydrothings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-19 23:19:55.000000 django-hydrothings-0.1.5/src/django_hydrothings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:19:55.000000 django-hydrothings-0.1.5/src/django_hydrothings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-19 23:19:55.000000 django-hydrothings-0.1.5/src/django_hydrothings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 23:19:55.000000 django-hydrothings-0.1.5/src/django_hydrothings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:19:55.000000 django-hydrothings-0.1.5/src/django_hydrothings.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/backends/frostserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/frostserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/frostserver/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/frostserver/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/frostserver/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/frostserver/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/backends/odm2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/odm2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/odm2/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/odm2/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/odm2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/odm2/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/odm2/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/backends/sensorthings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/sensorthings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/sensorthings/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/sensorthings/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/sensorthings/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/sensorthings/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/components/datastreams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/datastreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/datastreams/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/datastreams/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/components/featuresofinterest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/featuresofinterest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/featuresofinterest/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/featuresofinterest/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/components/historicallocations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/historicallocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/historicallocations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/historicallocations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/components/locations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/locations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/locations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/components/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/observations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/observations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/components/observedproperties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/observedproperties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/observedproperties/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/observedproperties/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/components/root/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/root/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/root/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/root/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/components/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/sensors/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/sensors/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/sensors/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/components/things/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/things/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/things/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/things/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/extras/iso_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.410374 django-hydrothings-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/tests/test_allow_partial_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/tests/test_iso_interval_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/tests/test_iso_time_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/tests/test_metadata_field_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/tests/test_resolve_chained_entity_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/tests/test_sensorthings_abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/tests/test_whitespace_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.182488 django-hydrothings-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.186488 django-hydrothings-0.1.6/src/django_hydrothings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-02 16:22:04.000000 django-hydrothings-0.1.6/src/django_hydrothings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-02 16:22:04.000000 django-hydrothings-0.1.6/src/django_hydrothings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:22:04.000000 django-hydrothings-0.1.6/src/django_hydrothings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 16:22:04.000000 django-hydrothings-0.1.6/src/django_hydrothings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 16:22:04.000000 django-hydrothings-0.1.6/src/django_hydrothings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:22:04.000000 django-hydrothings-0.1.6/src/django_hydrothings.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.186488 django-hydrothings-0.1.6/src/hydrothings/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.186488 django-hydrothings-0.1.6/src/hydrothings/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/backends/frostserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/frostserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/frostserver/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/frostserver/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/frostserver/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/frostserver/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/backends/odm2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/odm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/odm2/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/odm2/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/odm2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/odm2/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/odm2/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/backends/sensorthings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/sensorthings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/sensorthings/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/sensorthings/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/sensorthings/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/sensorthings/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/components/datastreams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/datastreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/datastreams/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/datastreams/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/components/featuresofinterest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/featuresofinterest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/featuresofinterest/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/featuresofinterest/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/components/historicallocations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/historicallocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/historicallocations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/historicallocations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/components/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/locations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/locations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/components/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/observations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/observations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/components/observedproperties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/observedproperties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/observedproperties/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/observedproperties/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/src/hydrothings/components/root/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/root/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/root/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/root/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/src/hydrothings/components/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/sensors/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/sensors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/sensors/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/src/hydrothings/components/things/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/things/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/things/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/things/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/src/hydrothings/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/extras/iso_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/tests/test_allow_partial_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/tests/test_iso_interval_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/tests/test_iso_time_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/tests/test_metadata_field_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/tests/test_resolve_chained_entity_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/tests/test_sensorthings_abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/tests/test_whitespace_validator.py
```

### Comparing `django-hydrothings-0.1.5/LICENSE.txt` & `django-hydrothings-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/README.md` & `django-hydrothings-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/src/django_hydrothings.egg-info/SOURCES.txt` & `django-hydrothings-0.1.6/src/django_hydrothings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/src/hydrothings/backends/frostserver/engine.py` & `django-hydrothings-0.1.6/src/hydrothings/backends/frostserver/engine.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/src/hydrothings/backends/odm2/engine.py` & `django-hydrothings-0.1.6/src/hydrothings/backends/odm2/engine.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/src/hydrothings/backends/sensorthings/engine.py` & `django-hydrothings-0.1.6/src/hydrothings/backends/sensorthings/engine.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/__init__.py` & `django-hydrothings-0.1.6/src/hydrothings/components/__init__.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/datastreams/schemas.py` & `django-hydrothings-0.1.6/src/hydrothings/components/datastreams/schemas.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import TYPE_CHECKING, Literal, List, Union
 from pydantic import Field, AnyHttpUrl
 from ninja import Schema
-from hydrothings.schemas import BaseListResponse, BaseGetResponse, BasePostBody, BasePatchBody, EntityId, NestedEntity
+from hydrothings.schemas import BaseListResponse, BaseGetResponse, BasePostBody, BasePatchBody, EntityId, \
+    NestedEntity
 from hydrothings.validators import allow_partial
 from hydrothings.extras.iso_types import ISOTime, ISOInterval
 
 if TYPE_CHECKING:
     from hydrothings.components.things.schemas import Thing
     from hydrothings.components.sensors.schemas import Sensor
     from hydrothings.components.observedproperties.schemas import ObservedProperty
@@ -65,14 +66,22 @@
 class DatastreamPatchBody(BasePatchBody, DatastreamFields):
     thing: EntityId = Field(..., alias='Thing')
     sensor: EntityId = Field(..., alias='Sensor')
     observed_property: EntityId = Field(..., alias='ObservedProperty')
 
 
 class DatastreamGetResponse(BaseGetResponse, DatastreamFields):
-    thing_link: AnyHttpUrl = Field(..., alias='Thing@iot.navigationLink')
-    sensor_link: AnyHttpUrl = Field(..., alias='Sensor@iot.navigationLink')
-    observed_property_link: AnyHttpUrl = Field(..., alias='ObservedProperty@iot.navigationLink')
+    thing_link: AnyHttpUrl = Field(None, alias='Thing@iot.navigationLink')
+    thing_rel: NestedEntity = Field(None, alias='Thing', nested_class='ThingGetResponse')
+    sensor_link: AnyHttpUrl = Field(None, alias='Sensor@iot.navigationLink')
+    sensor_rel: NestedEntity = Field(None, alias='Sensor', nested_class='SensorGetResponse')
+    observed_property_link: AnyHttpUrl = Field(None, alias='ObservedProperty@iot.navigationLink')
+    observed_property_rel: NestedEntity = Field(
+        None, alias='ObservedProperty',
+        nested_class='ObservedPropertyGetResponse'
+    )
+    observations_link: AnyHttpUrl = Field(None, alias='Observations@iot.navigationLink')
+    observations_rel: List[NestedEntity] = Field(None, alias='Observations', nested_class='ObservationGetResponse')
 
 
 class DatastreamListResponse(BaseListResponse):
-    value: List[DatastreamGetResponse]
+    values: List[DatastreamGetResponse]
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/datastreams/views.py` & `django-hydrothings-0.1.6/src/hydrothings/components/datastreams/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from ninja import Router, Query
 from django.http import HttpResponse
 from hydrothings.engine import SensorThingsRequest
-from hydrothings.schemas import QueryParams
+from hydrothings.schemas import ListQueryParams, GetQueryParams
 from hydrothings.utils import entities_or_404, entity_or_404, generate_response_codes, parse_query_params
 from .schemas import DatastreamPostBody, DatastreamPatchBody, DatastreamListResponse, DatastreamGetResponse
 
 
 router = Router(tags=['Datastreams'])
 
 
 @router.get(
     '/Datastreams',
     response=generate_response_codes('list', DatastreamListResponse),
     by_alias=True,
+    exclude_unset=True,
     url_name='list_datastream'
 )
-def list_datastreams(request: SensorThingsRequest, params: QueryParams = Query(...)):
+def list_datastreams(request: SensorThingsRequest, params: ListQueryParams = Query(...)):
     """
     Get a collection of Datastream entities.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/datastream/properties" target="_blank">\
       Datastream Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/datastream/relations" target="_blank">\
       Datastream Relations</a>
@@ -34,27 +35,33 @@
 
     return entities_or_404(response, DatastreamListResponse)
 
 
 @router.get(
     '/Datastreams({datastream_id})',
     response=generate_response_codes('get', DatastreamGetResponse),
-    by_alias=True
+    by_alias=True,
+    exclude_unset=True
 )
-def get_datastream(request: SensorThingsRequest, datastream_id: str):
+def get_datastream(request: SensorThingsRequest, datastream_id: str, params: GetQueryParams = Query(...)):
     """
     Get a Datastream entity.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/datastream/properties" target="_blank">\
       Datastream Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/datastream/relations" target="_blank">\
       Datastream Relations</a>
     """
 
-    response = request.engine.get(entity_id=datastream_id)
+    response = request.engine.get(
+        entity_id=datastream_id,
+        **parse_query_params(
+            query_params=params.dict()
+        )
+    )
 
     return entity_or_404(response, datastream_id, DatastreamGetResponse)
 
 
 @router.post(
     '/Datastreams',
     response=generate_response_codes('create')
```

#### html2text {}

```diff
@@ -1,32 +1,34 @@
 from ninja import Router, Query from django.http import HttpResponse from
 hydrothings.engine import SensorThingsRequest from hydrothings.schemas import
-QueryParams from hydrothings.utils import entities_or_404, entity_or_404,
-generate_response_codes, parse_query_params from .schemas import
+ListQueryParams, GetQueryParams from hydrothings.utils import entities_or_404,
+entity_or_404, generate_response_codes, parse_query_params from .schemas import
 DatastreamPostBody, DatastreamPatchBody, DatastreamListResponse,
 DatastreamGetResponse router = Router(tags=['Datastreams']) @router.get( '/
 Datastreams', response=generate_response_codes('list', DatastreamListResponse),
-by_alias=True, url_name='list_datastream' ) def list_datastreams(request:
-SensorThingsRequest, params: QueryParams = Query(...)): """ Get a collection of
-Datastream entities. \_Datastream_Properties - \_Datastream_Relations """
-response = request.engine.list( **parse_query_params( query_params=params.dict
-(), entity_chain=request.entity_chain ) ) return entities_or_404(response,
-DatastreamListResponse) @router.get( '/Datastreams({datastream_id})',
-response=generate_response_codes('get', DatastreamGetResponse), by_alias=True )
-def get_datastream(request: SensorThingsRequest, datastream_id: str): """ Get a
-Datastream entity. \_Datastream_Properties - \_Datastream_Relations """
-response = request.engine.get(entity_id=datastream_id) return entity_or_404
-(response, datastream_id, DatastreamGetResponse) @router.post( '/Datastreams',
-response=generate_response_codes('create') ) def create_datastream(request:
-SensorThingsRequest, response: HttpResponse, datastream: DatastreamPostBody):
-""" Create a new Datastream entity. Links: \_Datastream_Properties - \
-Datastream_Relations - \_Create_Entity """ datastream_id =
-request.engine.create( entity_body=datastream ) response['location'] =
-request.engine.get_ref( entity_id=datastream_id ) return 201, None
-@router.patch( '/Datastreams({datastream_id})',
+by_alias=True, exclude_unset=True, url_name='list_datastream' ) def
+list_datastreams(request: SensorThingsRequest, params: ListQueryParams = Query
+(...)): """ Get a collection of Datastream entities. \_Datastream_Properties -
+\_Datastream_Relations """ response = request.engine.list( **parse_query_params
+( query_params=params.dict(), entity_chain=request.entity_chain ) ) return
+entities_or_404(response, DatastreamListResponse) @router.get( '/Datastreams(
+{datastream_id})', response=generate_response_codes('get',
+DatastreamGetResponse), by_alias=True, exclude_unset=True ) def get_datastream
+(request: SensorThingsRequest, datastream_id: str, params: GetQueryParams =
+Query(...)): """ Get a Datastream entity. \_Datastream_Properties - \
+Datastream_Relations """ response = request.engine.get
+( entity_id=datastream_id, **parse_query_params( query_params=params.dict() ) )
+return entity_or_404(response, datastream_id, DatastreamGetResponse)
+@router.post( '/Datastreams', response=generate_response_codes('create') ) def
+create_datastream(request: SensorThingsRequest, response: HttpResponse,
+datastream: DatastreamPostBody): """ Create a new Datastream entity. Links: \
+Datastream_Properties - \_Datastream_Relations - \_Create_Entity """
+datastream_id = request.engine.create( entity_body=datastream ) response
+['location'] = request.engine.get_ref( entity_id=datastream_id ) return 201,
+None @router.patch( '/Datastreams({datastream_id})',
 response=generate_response_codes('update') ) def update_datastream(request:
 SensorThingsRequest, datastream_id: str, datastream: DatastreamPatchBody): """
 Update an existing Datastream entity. Links: \_Datastream_Properties - \
 Datastream_Relations - \_Update_Entity """ request.engine.update
 ( entity_id=datastream_id, entity_body=datastream ) return 204, None
 @router.delete( '/Datastreams({datastream_id})',
 response=generate_response_codes('delete') ) def delete_datastream(request:
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/featuresofinterest/schemas.py` & `django-hydrothings-0.1.6/src/hydrothings/components/featuresofinterest/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,12 +36,13 @@
 
 @allow_partial
 class FeatureOfInterestPatchBody(FeatureOfInterestFields, BasePatchBody):
     pass
 
 
 class FeatureOfInterestGetResponse(BaseGetResponse, FeatureOfInterestFields):
-    observations_link: AnyHttpUrl = Field(..., alias='Observations@iot.navigationLink')
+    observations_link: AnyHttpUrl = Field(None, alias='Observations@iot.navigationLink')
+    observations_rel: List[NestedEntity] = Field(None, alias='Observations', nested_class='ObservationGetResponse')
 
 
 class FeatureOfInterestListResponse(BaseListResponse):
-    value: List[FeatureOfInterestGetResponse]
+    values: List[FeatureOfInterestGetResponse]
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/featuresofinterest/views.py` & `django-hydrothings-0.1.6/src/hydrothings/components/featuresofinterest/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from ninja import Router, Query
 from django.http import HttpResponse
 from hydrothings.engine import SensorThingsRequest
-from hydrothings.schemas import QueryParams
+from hydrothings.schemas import ListQueryParams, GetQueryParams
 from hydrothings.utils import entity_or_404, entities_or_404, generate_response_codes, parse_query_params
 from .schemas import FeatureOfInterestPostBody, FeatureOfInterestPatchBody, FeatureOfInterestListResponse, \
     FeatureOfInterestGetResponse
 
 
 router = Router(tags=['Features Of Interest'])
 
 
 @router.get(
     '/FeaturesOfInterest',
     response=generate_response_codes('list', FeatureOfInterestListResponse),
+    by_alias=True,
+    exclude_unset=True,
     url_name='list_feature_of_interest'
 )
-def list_features_of_interest(request: SensorThingsRequest, params: QueryParams = Query(...)):
+def list_features_of_interest(request: SensorThingsRequest, params: ListQueryParams = Query(...)):
     """
     Get a collection of Feature of Interest entities.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/feature-of-interest/properties" target="_blank">\
       Feature of Interest Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/feature-of-interest/relations" target="_blank">\
       Feature of Interest Relations</a>
@@ -34,27 +36,33 @@
 
     return entities_or_404(response, FeatureOfInterestListResponse)
 
 
 @router.get(
     '/FeaturesOfInterest({feature_of_interest_id})',
     response=generate_response_codes('get', FeatureOfInterestGetResponse),
-    by_alias=True
+    by_alias=True,
+    exclude_unset=True
 )
-def get_feature_of_interest(request, feature_of_interest_id: str):
+def get_feature_of_interest(request, feature_of_interest_id: str, params: GetQueryParams = Query(...)):
     """
     Get a Feature of Interest entity.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/feature-of-interest/properties" target="_blank">\
       Feature of Interest Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/feature-of-interest/relations" target="_blank">\
       Feature of Interest Relations</a>
     """
 
-    response = request.engine.get(entity_id=feature_of_interest_id)
+    response = request.engine.get(
+        entity_id=feature_of_interest_id,
+        **parse_query_params(
+            query_params=params.dict()
+        )
+    )
 
     return entity_or_404(response, feature_of_interest_id, FeatureOfInterestGetResponse)
 
 
 @router.post(
     '/FeaturesOfInterest',
     response=generate_response_codes('create')
```

#### html2text {}

```diff
@@ -1,27 +1,29 @@
 from ninja import Router, Query from django.http import HttpResponse from
 hydrothings.engine import SensorThingsRequest from hydrothings.schemas import
-QueryParams from hydrothings.utils import entity_or_404, entities_or_404,
-generate_response_codes, parse_query_params from .schemas import
-FeatureOfInterestPostBody, FeatureOfInterestPatchBody,
+ListQueryParams, GetQueryParams from hydrothings.utils import entity_or_404,
+entities_or_404, generate_response_codes, parse_query_params from .schemas
+import FeatureOfInterestPostBody, FeatureOfInterestPatchBody,
 FeatureOfInterestListResponse, \ FeatureOfInterestGetResponse router = Router
 (tags=['Features Of Interest']) @router.get( '/FeaturesOfInterest',
 response=generate_response_codes('list', FeatureOfInterestListResponse),
-url_name='list_feature_of_interest' ) def list_features_of_interest(request:
-SensorThingsRequest, params: QueryParams = Query(...)): """ Get a collection of
-Feature of Interest entities. \_Feature_of_Interest_Properties - \_Feature_of
-Interest_Relations """ response = request.engine.list( **parse_query_params
-( query_params=params.dict(), entity_chain=request.entity_chain ) ) return
-entities_or_404(response, FeatureOfInterestListResponse) @router.get( '/
-FeaturesOfInterest({feature_of_interest_id})', response=generate_response_codes
-('get', FeatureOfInterestGetResponse), by_alias=True ) def
-get_feature_of_interest(request, feature_of_interest_id: str): """ Get a
-Feature of Interest entity. \_Feature_of_Interest_Properties - \_Feature_of
-Interest_Relations """ response = request.engine.get
-(entity_id=feature_of_interest_id) return entity_or_404(response,
+by_alias=True, exclude_unset=True, url_name='list_feature_of_interest' ) def
+list_features_of_interest(request: SensorThingsRequest, params: ListQueryParams
+= Query(...)): """ Get a collection of Feature of Interest entities. \_Feature
+of_Interest_Properties - \_Feature_of_Interest_Relations """ response =
+request.engine.list( **parse_query_params( query_params=params.dict(),
+entity_chain=request.entity_chain ) ) return entities_or_404(response,
+FeatureOfInterestListResponse) @router.get( '/FeaturesOfInterest(
+{feature_of_interest_id})', response=generate_response_codes('get',
+FeatureOfInterestGetResponse), by_alias=True, exclude_unset=True ) def
+get_feature_of_interest(request, feature_of_interest_id: str, params:
+GetQueryParams = Query(...)): """ Get a Feature of Interest entity. \_Feature
+of_Interest_Properties - \_Feature_of_Interest_Relations """ response =
+request.engine.get( entity_id=feature_of_interest_id, **parse_query_params
+( query_params=params.dict() ) ) return entity_or_404(response,
 feature_of_interest_id, FeatureOfInterestGetResponse) @router.post( '/
 FeaturesOfInterest', response=generate_response_codes('create') ) def
 create_feature_of_interest( request: SensorThingsRequest, response:
 HttpResponse, feature_of_interest: FeatureOfInterestPostBody ): """ Create a
 new Feature of Interest entity. Links: \_Feature_of_Interest_Properties - \
 Feature_of_Interest_Relations - \_Create_Entity """ feature_of_interest_id =
 request.engine.create( entity_body=feature_of_interest ) response['location'] =
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/historicallocations/schemas.py` & `django-hydrothings-0.1.6/src/hydrothings/components/historicallocations/schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,13 +35,19 @@
 @allow_partial
 class HistoricalLocationPatchBody(HistoricalLocationFields, BasePatchBody):
     thing: EntityId = Field(..., alias='Thing')
     locations: List[EntityId] = Field(..., alias='Locations')
 
 
 class HistoricalLocationGetResponse(BaseGetResponse, HistoricalLocationFields):
-    thing_link: AnyHttpUrl = Field(..., alias='Thing@iot.navigationLink')
-    historical_locations_link: AnyHttpUrl = Field(..., alias='Locations@iot.navigationLink')
+    thing_link: AnyHttpUrl = Field(None, alias='Thing@iot.navigationLink')
+    thing_rel: NestedEntity = Field(None, alias='Thing', nested_class='ThingGetResponse')
+    historical_locations_link: AnyHttpUrl = Field(None, alias='HistoricalLocations@iot.navigationLink')
+    historical_locations_rel: List[NestedEntity] = Field(
+        None,
+        alias='HistoricalLocations',
+        nested_class='HistoricalLocationsGetResponse'
+    )
 
 
 class HistoricalLocationListResponse(BaseListResponse):
-    value: List[HistoricalLocationGetResponse]
+    values: List[HistoricalLocationGetResponse]
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/historicallocations/views.py` & `django-hydrothings-0.1.6/src/hydrothings/components/historicallocations/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from ninja import Router, Query
 from django.http import HttpResponse
 from hydrothings.engine import SensorThingsRequest
-from hydrothings.schemas import QueryParams
+from hydrothings.schemas import ListQueryParams, GetQueryParams
 from hydrothings.utils import entity_or_404, entities_or_404, generate_response_codes, parse_query_params
 from .schemas import HistoricalLocationPostBody, HistoricalLocationPatchBody, HistoricalLocationListResponse, \
     HistoricalLocationGetResponse
 
 
 router = Router(tags=['Historical Locations'])
 
 
 @router.get(
     '/HistoricalLocations',
     response=generate_response_codes('list', HistoricalLocationListResponse),
     by_alias=True,
+    exclude_unset=True,
     url_name='list_historical_location'
 )
-def list_historical_locations(request: SensorThingsRequest, params: QueryParams = Query(...)):
+def list_historical_locations(request: SensorThingsRequest, params: ListQueryParams = Query(...)):
     """
     Get a collection of Historical Location entities.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/historical-location/properties" target="_blank">\
       Historical Location Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/historical-location/relations" target="_blank">\
       Historical Location Relations</a>
@@ -35,28 +36,37 @@
 
     return entities_or_404(response, HistoricalLocationListResponse)
 
 
 @router.get(
     '/HistoricalLocations({historical_location_id})',
     response=generate_response_codes('get', HistoricalLocationGetResponse),
-    by_alias=True
+    by_alias=True,
+    exclude_unset=True
 )
-def get_historical_location(request: SensorThingsRequest, historical_location_id: str):
+def get_historical_location(
+        request: SensorThingsRequest,
+        historical_location_id: str,
+        params: GetQueryParams = Query(...)
+):
     """
     Get a Historical Location entity.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/historical-location/properties" target="_blank">\
       Historical Location Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/historical-location/relations" target="_blank">\
       Historical Location Relations</a>
     """
 
-    response = request.engine.get(entity_id=historical_location_id)
-
+    response = request.engine.get(
+        entity_id=historical_location_id,
+        **parse_query_params(
+            query_params=params.dict()
+        )
+    )
     return entity_or_404(response, historical_location_id, HistoricalLocationGetResponse)
 
 
 @router.post(
     '/HistoricalLocations',
     response=generate_response_codes('create')
 )
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
 from ninja import Router, Query from django.http import HttpResponse from
 hydrothings.engine import SensorThingsRequest from hydrothings.schemas import
-QueryParams from hydrothings.utils import entity_or_404, entities_or_404,
-generate_response_codes, parse_query_params from .schemas import
-HistoricalLocationPostBody, HistoricalLocationPatchBody,
+ListQueryParams, GetQueryParams from hydrothings.utils import entity_or_404,
+entities_or_404, generate_response_codes, parse_query_params from .schemas
+import HistoricalLocationPostBody, HistoricalLocationPatchBody,
 HistoricalLocationListResponse, \ HistoricalLocationGetResponse router = Router
 (tags=['Historical Locations']) @router.get( '/HistoricalLocations',
 response=generate_response_codes('list', HistoricalLocationListResponse),
-by_alias=True, url_name='list_historical_location' ) def
-list_historical_locations(request: SensorThingsRequest, params: QueryParams =
-Query(...)): """ Get a collection of Historical Location entities. \_Historical
-Location_Properties - \_Historical_Location_Relations """ response =
+by_alias=True, exclude_unset=True, url_name='list_historical_location' ) def
+list_historical_locations(request: SensorThingsRequest, params: ListQueryParams
+= Query(...)): """ Get a collection of Historical Location entities. \
+Historical_Location_Properties - \_Historical_Location_Relations """ response =
 request.engine.list( **parse_query_params( query_params=params.dict(),
 entity_chain=request.entity_chain ) ) return entities_or_404(response,
 HistoricalLocationListResponse) @router.get( '/HistoricalLocations(
 {historical_location_id})', response=generate_response_codes('get',
-HistoricalLocationGetResponse), by_alias=True ) def get_historical_location
-(request: SensorThingsRequest, historical_location_id: str): """ Get a
-Historical Location entity. \_Historical_Location_Properties - \_Historical
-Location_Relations """ response = request.engine.get
-(entity_id=historical_location_id) return entity_or_404(response,
-historical_location_id, HistoricalLocationGetResponse) @router.post( '/
-HistoricalLocations', response=generate_response_codes('create') ) def
+HistoricalLocationGetResponse), by_alias=True, exclude_unset=True ) def
+get_historical_location( request: SensorThingsRequest, historical_location_id:
+str, params: GetQueryParams = Query(...) ): """ Get a Historical Location
+entity. \_Historical_Location_Properties - \_Historical_Location_Relations """
+response = request.engine.get( entity_id=historical_location_id,
+**parse_query_params( query_params=params.dict() ) ) return entity_or_404
+(response, historical_location_id, HistoricalLocationGetResponse) @router.post
+( '/HistoricalLocations', response=generate_response_codes('create') ) def
 create_historical_location( request: SensorThingsRequest, response:
 HttpResponse, historical_location: HistoricalLocationPostBody ): """ Create a
 new Historical Location entity. Links: \_Historical_Location_Properties - \
 Historical_Location_Relations - \_Create_Entity """ historical_location_id =
 request.engine.create( entity_body=historical_location ) response['location'] =
 request.engine.get_ref( entity_id=historical_location_id ) return 201, None
 @router.patch( '/HistoricalLocations({historical_location_id})',
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/locations/schemas.py` & `django-hydrothings-0.1.6/src/hydrothings/components/locations/schemas.py`

 * *Files 17% similar despite different names*

```diff
@@ -42,13 +42,19 @@
 @allow_partial
 class LocationPatchBody(LocationFields, BasePatchBody):
     things: List[EntityId] = Field([], alias='Things')
     historical_locations: List[EntityId] = Field([], alias='HistoricalLocations')
 
 
 class LocationGetResponse(BaseGetResponse, LocationFields):
-    things_link: AnyHttpUrl = Field(..., alias='Things@iot.navigationLink')
-    historical_locations_link: AnyHttpUrl = Field(..., alias='HistoricalLocations@iot.navigationLink')
+    things_link: AnyHttpUrl = Field(None, alias='Things@iot.navigationLink')
+    things_rel: List[NestedEntity] = Field(None, alias='Things', nested_class='ThingGetResponse')
+    historical_locations_link: AnyHttpUrl = Field(None, alias='HistoricalLocations@iot.navigationLink')
+    historical_locations_rel: List[NestedEntity] = Field(
+        None,
+        alias='HistoricalLocations',
+        nested_class='HistoricalLocationGetResponse'
+    )
 
 
 class LocationListResponse(BaseListResponse):
-    value: List[LocationGetResponse]
+    values: List[LocationGetResponse]
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/locations/views.py` & `django-hydrothings-0.1.6/src/hydrothings/components/locations/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from ninja import Router, Query
 from django.http import HttpResponse
 from hydrothings.engine import SensorThingsRequest
-from hydrothings.schemas import QueryParams
+from hydrothings.schemas import ListQueryParams, GetQueryParams
 from hydrothings.utils import entity_or_404, entities_or_404, generate_response_codes, parse_query_params
 from .schemas import LocationPostBody, LocationPatchBody, LocationListResponse, LocationGetResponse
 
 
 router = Router(tags=['Locations'])
 
 
 @router.get(
     '/Locations',
     response=generate_response_codes('list', LocationListResponse),
     by_alias=True,
+    exclude_unset=True,
     url_name='list_location'
 )
-def list_locations(request: SensorThingsRequest, params: QueryParams = Query(...)):
+def list_locations(request: SensorThingsRequest, params: ListQueryParams = Query(...)):
     """
     Get a collection of Location entities.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/location/properties" target="_blank">\
       Location Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/location/relations" target="_blank">\
       Location Relations</a>
@@ -34,27 +35,33 @@
 
     return entities_or_404(response, LocationListResponse)
 
 
 @router.get(
     '/Locations({location_id})',
     response=generate_response_codes('get', LocationGetResponse),
-    by_alias=True
+    by_alias=True,
+    exclude_unset=True
 )
-def get_location(request: SensorThingsRequest, location_id: str):
+def get_location(request: SensorThingsRequest, location_id: str, params: GetQueryParams = Query(...)):
     """
     Get a Location entity.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/location/properties" target="_blank">\
       Location Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/location/relations" target="_blank">\
       Location Relations</a>
     """
 
-    response = request.engine.get(entity_id=location_id)
+    response = request.engine.get(
+        entity_id=location_id,
+        **parse_query_params(
+            query_params=params.dict()
+        )
+    )
 
     return entity_or_404(response, location_id, LocationGetResponse)
 
 
 @router.post(
     '/Locations',
     response=generate_response_codes('create')
```

#### html2text {}

```diff
@@ -1,25 +1,27 @@
 from ninja import Router, Query from django.http import HttpResponse from
 hydrothings.engine import SensorThingsRequest from hydrothings.schemas import
-QueryParams from hydrothings.utils import entity_or_404, entities_or_404,
-generate_response_codes, parse_query_params from .schemas import
-LocationPostBody, LocationPatchBody, LocationListResponse, LocationGetResponse
-router = Router(tags=['Locations']) @router.get( '/Locations',
-response=generate_response_codes('list', LocationListResponse), by_alias=True,
-url_name='list_location' ) def list_locations(request: SensorThingsRequest,
-params: QueryParams = Query(...)): """ Get a collection of Location entities. \
-Location_Properties - \_Location_Relations """ response = request.engine.list
-( **parse_query_params( query_params=params.dict(),
-entity_chain=request.entity_chain ) ) return entities_or_404(response,
-LocationListResponse) @router.get( '/Locations({location_id})',
-response=generate_response_codes('get', LocationGetResponse), by_alias=True )
-def get_location(request: SensorThingsRequest, location_id: str): """ Get a
-Location entity. \_Location_Properties - \_Location_Relations """ response =
-request.engine.get(entity_id=location_id) return entity_or_404(response,
-location_id, LocationGetResponse) @router.post( '/Locations',
+ListQueryParams, GetQueryParams from hydrothings.utils import entity_or_404,
+entities_or_404, generate_response_codes, parse_query_params from .schemas
+import LocationPostBody, LocationPatchBody, LocationListResponse,
+LocationGetResponse router = Router(tags=['Locations']) @router.get( '/
+Locations', response=generate_response_codes('list', LocationListResponse),
+by_alias=True, exclude_unset=True, url_name='list_location' ) def
+list_locations(request: SensorThingsRequest, params: ListQueryParams = Query
+(...)): """ Get a collection of Location entities. \_Location_Properties - \
+Location_Relations """ response = request.engine.list( **parse_query_params
+( query_params=params.dict(), entity_chain=request.entity_chain ) ) return
+entities_or_404(response, LocationListResponse) @router.get( '/Locations(
+{location_id})', response=generate_response_codes('get', LocationGetResponse),
+by_alias=True, exclude_unset=True ) def get_location(request:
+SensorThingsRequest, location_id: str, params: GetQueryParams = Query(...)):
+""" Get a Location entity. \_Location_Properties - \_Location_Relations """
+response = request.engine.get( entity_id=location_id, **parse_query_params
+( query_params=params.dict() ) ) return entity_or_404(response, location_id,
+LocationGetResponse) @router.post( '/Locations',
 response=generate_response_codes('create') ) def create_location(request:
 SensorThingsRequest, response: HttpResponse, location: LocationPostBody): """
 Create a new Location entity. Links: \_Location_Properties - \_Location
 Relations - \_Create_Entity """ location_id = request.engine.create
 ( entity_body=location ) response['location'] = request.engine.get_ref
 ( entity_id=location_id ) return 201, None @router.patch( '/Locations(
 {location_id})', response=generate_response_codes('update') ) def
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/observations/schemas.py` & `django-hydrothings-0.1.6/src/hydrothings/components/observations/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TYPE_CHECKING, Literal, Union, List
 from pydantic import Field, AnyHttpUrl
 from ninja import Schema
 from hydrothings.schemas import BaseListResponse, BaseGetResponse, BasePostBody, BasePatchBody, EntityId, \
-    NestedEntity, QueryParams
+    NestedEntity, ListQueryParams
 from hydrothings.extras.iso_types import ISOTime, ISOInterval
 from hydrothings.validators import allow_partial
 
 if TYPE_CHECKING:
     from hydrothings.components.datastreams.schemas import Datastream
     from hydrothings.components.featuresofinterest.schemas import FeatureOfInterest
 
@@ -78,30 +78,36 @@
 @allow_partial
 class ObservationPatchBody(BasePatchBody, ObservationFields):
     datastream: EntityId = Field(..., alias='Datastream')
     feature_of_interest: EntityId = Field(..., alias='FeatureOfInterest')
 
 
 class ObservationGetResponse(ObservationFields, BaseGetResponse):
-    datastream_link: AnyHttpUrl = Field(..., alias='Datastream@iot.navigationLink')
-    feature_of_interest_link: AnyHttpUrl = Field(..., alias='FeatureOfInterest@iot.navigationLink')
+    datastream_link: AnyHttpUrl = Field(None, alias='Datastream@iot.navigationLink')
+    datastream_rel: NestedEntity = Field(None, alias='Datastream', nested_class='DatastreamGetResponse')
+    feature_of_interest_link: AnyHttpUrl = Field(None, alias='FeatureOfInterest@iot.navigationLink')
+    feature_of_interest_rel: NestedEntity = Field(
+        None,
+        alias='FeatureOfInterest',
+        nested_class='FeatureOfInterestGetResponse'
+    )
 
     class Config:
         allow_population_by_field_name = True
 
 
 class ObservationListResponse(BaseListResponse):
     value: List[ObservationGetResponse]
 
     class Config:
         allow_population_by_field_name = True
 
 
 class ObservationDataArrayResponse(BaseListResponse):
-    value: List[ObservationDataArray]
+    values: List[ObservationDataArray]
 
     class Config:
         allow_population_by_field_name = True
 
 
-class ObservationParams(QueryParams):
+class ObservationParams(ListQueryParams):
     result_format: Union[observationResultFormats, None] = Field(None, alias='$resultFormat')
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/observations/utils.py` & `django-hydrothings-0.1.6/src/hydrothings/components/observations/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,26 +46,26 @@
     else:
         selected_fields = [
             field for field in fields if field[0] in ['result_time', 'result']
         ]
 
     datastream_url_template = f'{request.scheme}://{request.get_host()}{request.path[:-12]}Datastreams'
 
-    response['value'] = [
+    response['values'] = [
         {
             'datastream': f'{datastream_url_template}({datastream_id})',
             'components': [
                 field[1] for field in selected_fields
             ],
             'data_array': [
                 [
                     observation[field[0]] for field in selected_fields
                 ] for observation in observations
             ]
-        } for datastream_id, observations in groupby(response['value'], key=lambda x: x['datastream_id'])
+        } for datastream_id, observations in groupby(response['values'], key=lambda x: x['datastream_id'])
     ]
 
     return response
 
 
 def parse_data_array(
         observation: List[ObservationDataArray]
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/observations/views.py` & `django-hydrothings-0.1.6/src/hydrothings/components/observations/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from ninja import Router, Query
 from typing import Union, List
 from django.http import HttpResponse
 from hydrothings.engine import SensorThingsRequest
+from hydrothings.schemas import GetQueryParams
 from hydrothings.utils import entity_or_404, entities_or_404, generate_response_codes, parse_query_params
 from .schemas import ObservationPostBody, ObservationPatchBody, ObservationListResponse, ObservationGetResponse, \
     ObservationParams, ObservationDataArrayResponse, ObservationDataArrayBody
 from .utils import convert_to_data_array, parse_data_array
 
 
 router = Router(tags=['Observations'])
 
 
 @router.get(
     '/Observations',
     response=generate_response_codes('list', Union[ObservationListResponse, ObservationDataArrayResponse]),
     by_alias=True,
     url_name='list_observation',
-    exclude_none=True
+    exclude_unset=True
 )
 def list_observations(request: SensorThingsRequest, params: ObservationParams = Query(...)):
     """
     Get a collection of Observation entities.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/observation/properties" target="_blank">\
       Observation Properties</a> -
@@ -45,28 +46,33 @@
     else:
         return entities_or_404(response, ObservationListResponse)
 
 
 @router.get(
     '/Observations({observation_id})',
     response=generate_response_codes('get', ObservationGetResponse),
-    by_alias=True
+    by_alias=True,
+    exclude_unset=True
 )
-def get_observation(request: SensorThingsRequest, observation_id: str):
+def get_observation(request: SensorThingsRequest, observation_id: str, params: GetQueryParams = Query(...)):
     """
     Get an Observation entity.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/observation/properties" target="_blank">\
       Observation Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/observation/relations" target="_blank">\
       Observation Relations</a>
     """
 
-    response = request.engine.get(entity_id=observation_id)
-
+    response = request.engine.get(
+        entity_id=observation_id,
+        **parse_query_params(
+            query_params=params.dict()
+        )
+    )
     return entity_or_404(response, observation_id, ObservationGetResponse)
 
 
 @router.post(
     '/Observations',
     response=generate_response_codes('create')
 )
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/observedproperties/schemas.py` & `django-hydrothings-0.1.6/src/hydrothings/components/observedproperties/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,12 +31,13 @@
 
 @allow_partial
 class ObservedPropertyPatchBody(BasePatchBody, ObservedPropertyFields):
     pass
 
 
 class ObservedPropertyGetResponse(ObservedPropertyFields, BaseGetResponse):
-    datastreams_link: AnyHttpUrl = Field(..., alias='Datastreams@iot.navigationLink')
+    datastreams_link: AnyHttpUrl = Field(None, alias='Datastreams@iot.navigationLink')
+    datastreams_rel: List[NestedEntity] = Field(None, alias='Datastreams', nested_class='DatastreamGetResponse')
 
 
 class ObservedPropertyListResponse(BaseListResponse):
-    value: List[ObservedPropertyGetResponse]
+    values: List[ObservedPropertyGetResponse]
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/observedproperties/views.py` & `django-hydrothings-0.1.6/src/hydrothings/components/observedproperties/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from ninja import Router, Query
 from django.http import HttpResponse
 from hydrothings.engine import SensorThingsRequest
-from hydrothings.schemas import QueryParams
+from hydrothings.schemas import ListQueryParams, GetQueryParams
 from hydrothings.utils import entity_or_404, entities_or_404, generate_response_codes, parse_query_params
 from .schemas import ObservedPropertyPostBody, ObservedPropertyPatchBody, ObservedPropertyListResponse, \
     ObservedPropertyGetResponse
 
 
 router = Router(tags=['Observed Properties'])
 
 
 @router.get(
     '/ObservedProperties',
     response=generate_response_codes('list', ObservedPropertyListResponse),
     by_alias=True,
     url_name='list_observed_property',
-    exclude_none=True
+    exclude_unset=True
 )
-def list_observed_properties(request: SensorThingsRequest, params: QueryParams = Query(...)):
+def list_observed_properties(request: SensorThingsRequest, params: ListQueryParams = Query(...)):
     """
     Get a collection of Observed Property entities.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/observed-property/properties" target="_blank">\
       Observed Property Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/observed-property/relations" target="_blank">\
       Observed Property Relations</a>
@@ -36,27 +36,33 @@
 
     return entities_or_404(response, ObservedPropertyListResponse)
 
 
 @router.get(
     '/ObservedProperties({observed_property_id})',
     response=generate_response_codes('get', ObservedPropertyGetResponse),
-    by_alias=True
+    by_alias=True,
+    exclude_unset=True
 )
-def get_observed_property(request, observed_property_id: str):
+def get_observed_property(request, observed_property_id: str, params: GetQueryParams = Query(...)):
     """
     Get an Observed Property entity.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/observed-property/properties" target="_blank">\
       Observed Property Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/observed-property/relations" target="_blank">\
       Observed Property Relations</a>
     """
 
-    response = request.engine.get(entity_id=observed_property_id)
+    response = request.engine.get(
+        entity_id=observed_property_id,
+        **parse_query_params(
+            query_params=params.dict()
+        )
+    )
 
     return entity_or_404(response, observed_property_id, ObservedPropertyGetResponse)
 
 
 @router.post(
     '/ObservedProperties',
     response=generate_response_codes('create')
```

#### html2text {}

```diff
@@ -1,28 +1,30 @@
 from ninja import Router, Query from django.http import HttpResponse from
 hydrothings.engine import SensorThingsRequest from hydrothings.schemas import
-QueryParams from hydrothings.utils import entity_or_404, entities_or_404,
-generate_response_codes, parse_query_params from .schemas import
-ObservedPropertyPostBody, ObservedPropertyPatchBody,
+ListQueryParams, GetQueryParams from hydrothings.utils import entity_or_404,
+entities_or_404, generate_response_codes, parse_query_params from .schemas
+import ObservedPropertyPostBody, ObservedPropertyPatchBody,
 ObservedPropertyListResponse, \ ObservedPropertyGetResponse router = Router
 (tags=['Observed Properties']) @router.get( '/ObservedProperties',
 response=generate_response_codes('list', ObservedPropertyListResponse),
-by_alias=True, url_name='list_observed_property', exclude_none=True ) def
-list_observed_properties(request: SensorThingsRequest, params: QueryParams =
-Query(...)): """ Get a collection of Observed Property entities. \_Observed
+by_alias=True, url_name='list_observed_property', exclude_unset=True ) def
+list_observed_properties(request: SensorThingsRequest, params: ListQueryParams
+= Query(...)): """ Get a collection of Observed Property entities. \_Observed
 Property_Properties - \_Observed_Property_Relations """ response =
 request.engine.list( **parse_query_params( query_params=params.dict(),
 entity_chain=request.entity_chain ) ) return entities_or_404(response,
 ObservedPropertyListResponse) @router.get( '/ObservedProperties(
 {observed_property_id})', response=generate_response_codes('get',
-ObservedPropertyGetResponse), by_alias=True ) def get_observed_property
-(request, observed_property_id: str): """ Get an Observed Property entity. \
-Observed_Property_Properties - \_Observed_Property_Relations """ response =
-request.engine.get(entity_id=observed_property_id) return entity_or_404
-(response, observed_property_id, ObservedPropertyGetResponse) @router.post( '/
+ObservedPropertyGetResponse), by_alias=True, exclude_unset=True ) def
+get_observed_property(request, observed_property_id: str, params:
+GetQueryParams = Query(...)): """ Get an Observed Property entity. \_Observed
+Property_Properties - \_Observed_Property_Relations """ response =
+request.engine.get( entity_id=observed_property_id, **parse_query_params
+( query_params=params.dict() ) ) return entity_or_404(response,
+observed_property_id, ObservedPropertyGetResponse) @router.post( '/
 ObservedProperties', response=generate_response_codes('create') ) def
 create_observed_property( request: SensorThingsRequest, response: HttpResponse,
 observed_property: ObservedPropertyPostBody ): """ Create a new Observed
 Property entity. Links: \_Observed_Property_Properties - \_Observed_Property
 Relations - \_Create_Entity """ observed_property_id = request.engine.create
 ( entity_body=observed_property ) response['location'] = request.engine.get_ref
 ( entity_id=observed_property_id ) return 201, None @router.patch( '/
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/root/views.py` & `django-hydrothings-0.1.6/src/hydrothings/components/root/views.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/sensors/schemas.py` & `django-hydrothings-0.1.6/src/hydrothings/components/sensors/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,11 +43,12 @@
 @allow_partial
 class SensorPatchBody(BasePatchBody, SensorFields):
     pass
 
 
 class SensorGetResponse(SensorFields, BaseGetResponse):
     datastreams_link: AnyHttpUrl = Field(..., alias='Datastreams@iot.navigationLink')
+    datastreams_rel: List[NestedEntity] = Field(None, alias='Datastreams', nested_class='DatastreamGetResponse')
 
 
 class SensorListResponse(BaseListResponse):
-    value: List[SensorGetResponse]
+    values: List[SensorGetResponse]
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/sensors/utils.py` & `django-hydrothings-0.1.6/src/hydrothings/components/sensors/utils.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/sensors/views.py` & `django-hydrothings-0.1.6/src/hydrothings/components/sensors/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from ninja import Router, Query
 from django.http import HttpResponse
 from hydrothings.engine import SensorThingsRequest
-from hydrothings.schemas import QueryParams
+from hydrothings.schemas import ListQueryParams, GetQueryParams
 from hydrothings.utils import entity_or_404, entities_or_404, generate_response_codes, parse_query_params
 from .schemas import SensorPostBody, SensorPatchBody, SensorListResponse, SensorGetResponse
 
 
 router = Router(tags=['Sensors'])
 
 
 @router.get(
     '/Sensors',
     response=generate_response_codes('list', SensorListResponse),
     by_alias=True,
     url_name='list_sensor',
-    exclude_none=True
+    exclude_unset=True
 )
-def list_sensors(request, params: QueryParams = Query(...)):
+def list_sensors(request, params: ListQueryParams = Query(...)):
     """
     Get a collection of Sensor entities.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/sensor/properties" target="_blank">\
       Sensor Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/sensor/relations" target="_blank">\
       Sensor Relations</a>
@@ -34,27 +34,33 @@
     )
     return entities_or_404(response, SensorListResponse)
 
 
 @router.get(
     '/Sensors({sensor_id})',
     response=generate_response_codes('get', SensorGetResponse),
-    by_alias=True
+    by_alias=True,
+    exclude_unset=True
 )
-def get_sensor(request, sensor_id: str):
+def get_sensor(request, sensor_id: str, params: GetQueryParams = Query(...)):
     """
     Get a Sensor entity.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/sensor/properties" target="_blank">\
       Sensor Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/sensor/relations" target="_blank">\
       Sensor Relations</a>
     """
 
-    response = request.engine.get(entity_id=sensor_id)
+    response = request.engine.get(
+        entity_id=sensor_id,
+        **parse_query_params(
+            query_params=params.dict()
+        )
+    )
 
     return entity_or_404(response, sensor_id, SensorGetResponse)
 
 
 @router.post(
     '/Sensors',
     response=generate_response_codes('create')
```

#### html2text {}

```diff
@@ -1,31 +1,33 @@
 from ninja import Router, Query from django.http import HttpResponse from
 hydrothings.engine import SensorThingsRequest from hydrothings.schemas import
-QueryParams from hydrothings.utils import entity_or_404, entities_or_404,
-generate_response_codes, parse_query_params from .schemas import
-SensorPostBody, SensorPatchBody, SensorListResponse, SensorGetResponse router =
-Router(tags=['Sensors']) @router.get( '/Sensors',
+ListQueryParams, GetQueryParams from hydrothings.utils import entity_or_404,
+entities_or_404, generate_response_codes, parse_query_params from .schemas
+import SensorPostBody, SensorPatchBody, SensorListResponse, SensorGetResponse
+router = Router(tags=['Sensors']) @router.get( '/Sensors',
 response=generate_response_codes('list', SensorListResponse), by_alias=True,
-url_name='list_sensor', exclude_none=True ) def list_sensors(request, params:
-QueryParams = Query(...)): """ Get a collection of Sensor entities. \_Sensor
-Properties - \_Sensor_Relations """ response = request.engine.list
+url_name='list_sensor', exclude_unset=True ) def list_sensors(request, params:
+ListQueryParams = Query(...)): """ Get a collection of Sensor entities. \
+Sensor_Properties - \_Sensor_Relations """ response = request.engine.list
 ( **parse_query_params( query_params=params.dict(),
 entity_chain=request.entity_chain ) ) return entities_or_404(response,
 SensorListResponse) @router.get( '/Sensors({sensor_id})',
-response=generate_response_codes('get', SensorGetResponse), by_alias=True ) def
-get_sensor(request, sensor_id: str): """ Get a Sensor entity. \_Sensor
-Properties - \_Sensor_Relations """ response = request.engine.get
-(entity_id=sensor_id) return entity_or_404(response, sensor_id,
-SensorGetResponse) @router.post( '/Sensors', response=generate_response_codes
-('create') ) def create_sensor(request: SensorThingsRequest, response:
-HttpResponse, sensor: SensorPostBody): """ Create a new Sensor entity. Links: \
-Sensor_Properties - \_Sensor_Relations - \_Create_Entity """ sensor_id =
-request.engine.create( entity_body=sensor ) response['location'] =
-request.engine.get_ref( entity_id=sensor_id ) return 201, None @router.patch
-( '/Sensors({sensor_id})', response=generate_response_codes('update') ) def
-update_sensor(request: SensorThingsRequest, sensor_id: str, sensor:
-SensorPatchBody): """ Update an existing Sensor entity. Links: \_Sensor
-Properties - \_Sensor_Relations - \_Update_Entity """ request.engine.update
-( entity_id=sensor_id, entity_body=sensor ) return 204, None @router.delete( '/
-Sensors({sensor_id})', response=generate_response_codes('delete') ) def
-delete_sensor(request, sensor_id: str): """ Delete a Sensor entity. Links: \
-Delete_Entity """ request.engine.delete( entity_id=sensor_id ) return 204, None
+response=generate_response_codes('get', SensorGetResponse), by_alias=True,
+exclude_unset=True ) def get_sensor(request, sensor_id: str, params:
+GetQueryParams = Query(...)): """ Get a Sensor entity. \_Sensor_Properties - \
+Sensor_Relations """ response = request.engine.get( entity_id=sensor_id,
+**parse_query_params( query_params=params.dict() ) ) return entity_or_404
+(response, sensor_id, SensorGetResponse) @router.post( '/Sensors',
+response=generate_response_codes('create') ) def create_sensor(request:
+SensorThingsRequest, response: HttpResponse, sensor: SensorPostBody): """
+Create a new Sensor entity. Links: \_Sensor_Properties - \_Sensor_Relations - \
+Create_Entity """ sensor_id = request.engine.create( entity_body=sensor )
+response['location'] = request.engine.get_ref( entity_id=sensor_id ) return
+201, None @router.patch( '/Sensors({sensor_id})',
+response=generate_response_codes('update') ) def update_sensor(request:
+SensorThingsRequest, sensor_id: str, sensor: SensorPatchBody): """ Update an
+existing Sensor entity. Links: \_Sensor_Properties - \_Sensor_Relations - \
+Update_Entity """ request.engine.update( entity_id=sensor_id,
+entity_body=sensor ) return 204, None @router.delete( '/Sensors({sensor_id})',
+response=generate_response_codes('delete') ) def delete_sensor(request,
+sensor_id: str): """ Delete a Sensor entity. Links: \_Delete_Entity """
+request.engine.delete( entity_id=sensor_id ) return 204, None
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/things/schemas.py` & `django-hydrothings-0.1.6/src/hydrothings/components/things/schemas.py`

 * *Files 18% similar despite different names*

```diff
@@ -43,18 +43,25 @@
 
 @allow_partial
 class ThingPatchBody(BasePatchBody, ThingFields):
     locations: List[EntityId] = Field([], alias='Locations')
 
 
 class ThingGetResponse(ThingFields, BaseGetResponse):
-    locations_link: AnyHttpUrl = Field(..., alias='Locations@iot.navigationLink')
-    historical_locations_link: AnyHttpUrl = Field(..., alias='HistoricalLocations@iot.navigationLink')
-    datastreams_link: AnyHttpUrl = Field(..., alias='Datastreams@iot.navigationLink')
+    locations_link: AnyHttpUrl = Field(None, alias='Locations@iot.navigationLink')
+    locations_rel: List[NestedEntity] = Field(None, alias='Locations', nested_class='LocationGetResponse')
+    historical_locations_link: AnyHttpUrl = Field(None, alias='HistoricalLocations@iot.navigationLink')
+    historical_locations_rel: List[NestedEntity] = Field(
+        None,
+        alias='HistoricalLocations',
+        nested_class='HistoricalLocationGetResponse'
+    )
+    datastreams_link: AnyHttpUrl = Field(None, alias='Datastreams@iot.navigationLink')
+    datastreams_rel: List[NestedEntity] = Field(None, alias='Datastreams', nested_class='DatastreamGetResponse')
 
 
 class ThingListResponse(BaseListResponse):
-    value: List[ThingGetResponse]
+    values: List[ThingGetResponse]
 
 
 class ThingGetResponseODM(ThingGetResponse):
     properties: str
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/components/things/views.py` & `django-hydrothings-0.1.6/src/hydrothings/components/things/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from ninja import Router, Query
 from django.http import HttpResponse
 from hydrothings.engine import SensorThingsRequest
-from hydrothings.schemas import QueryParams
+from hydrothings.schemas import ListQueryParams, GetQueryParams
 from hydrothings.utils import entity_or_404, entities_or_404, generate_response_codes, parse_query_params
 from .schemas import ThingPostBody, ThingPatchBody, ThingListResponse, ThingGetResponse
 
 
 router = Router(tags=['Things'])
 
 
 @router.get(
     '/Things',
     response=generate_response_codes('list', ThingListResponse),
     by_alias=True,
     url_name='list_thing',
-    exclude_none=True
+    exclude_unset=True
 )
-def list_things(request: SensorThingsRequest, params: QueryParams = Query(...)):
+def list_things(request: SensorThingsRequest, params: ListQueryParams = Query(...)):
     """
     Get a collection of Thing entities.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/thing/properties" target="_blank">\
       Thing Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/thing/relations" target="_blank">\
       Thing Relations</a>
@@ -35,28 +35,33 @@
 
     return entities_or_404(response, ThingListResponse)
 
 
 @router.get(
     '/Things({thing_id})',
     response=generate_response_codes('get', ThingGetResponse),
-    by_alias=True
+    by_alias=True,
+    exclude_unset=True
 )
-def get_thing(request: SensorThingsRequest, thing_id: str):
+def get_thing(request: SensorThingsRequest, thing_id: str, params: GetQueryParams = Query(...)):
     """
     Get a Thing entity.
 
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/thing/properties" target="_blank">\
       Thing Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/thing/relations" target="_blank">\
       Thing Relations</a>
     """
 
-    response = request.engine.get(entity_id=thing_id)
-
+    response = request.engine.get(
+        entity_id=thing_id,
+        **parse_query_params(
+            query_params=params.dict()
+        )
+    )
     return entity_or_404(response, thing_id, ThingGetResponse)
 
 
 @router.post(
     '/Things',
     response=generate_response_codes('create')
 )
```

#### html2text {}

```diff
@@ -1,31 +1,33 @@
 from ninja import Router, Query from django.http import HttpResponse from
 hydrothings.engine import SensorThingsRequest from hydrothings.schemas import
-QueryParams from hydrothings.utils import entity_or_404, entities_or_404,
-generate_response_codes, parse_query_params from .schemas import ThingPostBody,
-ThingPatchBody, ThingListResponse, ThingGetResponse router = Router(tags=
-['Things']) @router.get( '/Things', response=generate_response_codes('list',
-ThingListResponse), by_alias=True, url_name='list_thing', exclude_none=True )
-def list_things(request: SensorThingsRequest, params: QueryParams = Query
-(...)): """ Get a collection of Thing entities. \_Thing_Properties - \_Thing
-Relations """ response = request.engine.list( **parse_query_params
-( query_params=params.dict(), entity_chain=request.entity_chain ) ) return
-entities_or_404(response, ThingListResponse) @router.get( '/Things(
-{thing_id})', response=generate_response_codes('get', ThingGetResponse),
-by_alias=True ) def get_thing(request: SensorThingsRequest, thing_id: str): """
-Get a Thing entity. \_Thing_Properties - \_Thing_Relations """ response =
-request.engine.get(entity_id=thing_id) return entity_or_404(response, thing_id,
-ThingGetResponse) @router.post( '/Things', response=generate_response_codes
-('create') ) def create_thing(request: SensorThingsRequest, response:
-HttpResponse, thing: ThingPostBody): """ Create a new Thing entity. Links: \
-Thing_Properties - \_Thing_Relations - \_Create_Entity """ thing_id =
-request.engine.create( entity_body=thing ) response['location'] =
-request.engine.get_ref( entity_id=thing_id ) return 201, None @router.patch( '/
-Things({thing_id})', response=generate_response_codes('update') ) def
-update_thing(request: SensorThingsRequest, thing_id: str, thing:
-ThingPatchBody): """ Update an existing Thing entity. Links: \_Thing_Properties
-- \_Thing_Relations - \_Update_Entity """ request.engine.update
+ListQueryParams, GetQueryParams from hydrothings.utils import entity_or_404,
+entities_or_404, generate_response_codes, parse_query_params from .schemas
+import ThingPostBody, ThingPatchBody, ThingListResponse, ThingGetResponse
+router = Router(tags=['Things']) @router.get( '/Things',
+response=generate_response_codes('list', ThingListResponse), by_alias=True,
+url_name='list_thing', exclude_unset=True ) def list_things(request:
+SensorThingsRequest, params: ListQueryParams = Query(...)): """ Get a
+collection of Thing entities. \_Thing_Properties - \_Thing_Relations """
+response = request.engine.list( **parse_query_params( query_params=params.dict
+(), entity_chain=request.entity_chain ) ) return entities_or_404(response,
+ThingListResponse) @router.get( '/Things({thing_id})',
+response=generate_response_codes('get', ThingGetResponse), by_alias=True,
+exclude_unset=True ) def get_thing(request: SensorThingsRequest, thing_id: str,
+params: GetQueryParams = Query(...)): """ Get a Thing entity. \_Thing
+Properties - \_Thing_Relations """ response = request.engine.get
+( entity_id=thing_id, **parse_query_params( query_params=params.dict() ) )
+return entity_or_404(response, thing_id, ThingGetResponse) @router.post( '/
+Things', response=generate_response_codes('create') ) def create_thing(request:
+SensorThingsRequest, response: HttpResponse, thing: ThingPostBody): """ Create
+a new Thing entity. Links: \_Thing_Properties - \_Thing_Relations - \_Create
+Entity """ thing_id = request.engine.create( entity_body=thing ) response
+['location'] = request.engine.get_ref( entity_id=thing_id ) return 201, None
+@router.patch( '/Things({thing_id})', response=generate_response_codes
+('update') ) def update_thing(request: SensorThingsRequest, thing_id: str,
+thing: ThingPatchBody): """ Update an existing Thing entity. Links: \_Thing
+Properties - \_Thing_Relations - \_Update_Entity """ request.engine.update
 ( entity_id=thing_id, entity_body=thing ) return 204, None @router.delete( '/
 Things({thing_id})', response=generate_response_codes('delete') ) def
 delete_thing(request: SensorThingsRequest, thing_id: str): """ Delete a Thing
 entity. Links: \_Delete_Entity """ request.engine.delete( entity_id=thing_id )
 return 204, None
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/engine.py` & `django-hydrothings-0.1.6/src/hydrothings/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from uuid import UUID
 from pydantic.fields import SHAPE_LIST
 from typing import Union, Tuple, List, Optional
 from django.http import HttpRequest
 from hydrothings import components as component_schemas
 from hydrothings import settings
 from hydrothings.schemas import BasePostBody, BasePatchBody
+from hydrothings.utils import lookup_component
 
 
 class SensorThingsAbstractEngine(metaclass=ABCMeta):
     """
     Abstract base class for a SensorThings engine.
 
     A SensorThings API must be linked to a SensorThings engine to perform database operations. This class defines all
@@ -19,32 +20,42 @@
     scheme: str
     host: str
     path: str
     version: str
     component: str
     component_path: str
 
-    def get_ref(self, entity_id: Union[str, None] = None, related_component: Union[str, None] = None) -> str:
+    def get_ref(
+            self,
+            entity_id: Union[str, None] = None,
+            related_component: Union[str, None] = None,
+            override_component: Union[str, None] = None
+    ) -> str:
         """
         Builds a reference URL for a given entity.
 
         Parameters
         ----------
         entity_id : str
             The ID of the entity.
         related_component : str
             The related component to be appended to the ref URL.
+        override_component : str
+            A value used to override the base component in the URL.
 
         Returns
         -------
         str
             The entity's reference URL.
         """
 
-        ref_url = f'{self.scheme}://{self.host}{self.path}'
+        if override_component is not None:
+            override_component = '/' + lookup_component(override_component, 'camel_singular', 'camel_plural')
+
+        ref_url = f'{self.scheme}://{self.host}{override_component if override_component is not None else self.path}'
 
         if entity_id is not None:
             ref_url = f'{ref_url}({entity_id})'
 
         if related_component is not None:
             ref_url = f'{ref_url}/{related_component}'
 
@@ -206,25 +217,28 @@
         """
 
         pass
 
     @abstractmethod
     def get(
             self,
-            entity_id: str
+            entity_id: str,
+            expand
     ) -> Optional[dict]:
         """
         Abstract method for handling GET entity requests.
 
         This method should return a dictionary representing an entity with the given entity ID.
 
         Parameters
         ----------
         entity_id : str
             The ID of the entity to be returned.
+        expand
+            Represents related components whose fields should be included in the response.
 
         Returns
         -------
         dict
             A dictionary object representing the SensorThings GET entity response.
         """
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/extras/iso_types.py` & `django-hydrothings-0.1.6/src/hydrothings/extras/iso_types.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/src/hydrothings/main.py` & `django-hydrothings-0.1.6/src/hydrothings/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                     if view_func.__annotations__.get(component):
                         for field, schema in component_settings.component_schema.__fields__.items():
                             view_func.__annotations__[component].__fields__[field] = schema
 
                     if response_schema:
                         if operation_method == 'list':
                             for field, schema in component_settings.component_schema.__fields__.items():
-                                response_schema.__fields__['value'].type_.__fields__[field] = schema
+                                response_schema.__fields__['values'].type_.__fields__[field] = schema
 
                         elif operation_method == 'get':
                             for field, schema in component_settings.component_schema.__fields__.items():
                                 response_schema.__fields__[field] = schema
 
                 authorization_callbacks = getattr(endpoint_settings.get(operation_method), 'authorization', [])
 
@@ -135,14 +135,15 @@
                 else:
                     authorization_callbacks = []
 
                 (getattr(st_router, operation.methods[0].lower())(
                     path.replace('(', f'({self.id_qualifier}').replace(')', f'{self.id_qualifier})'),
                     response=generate_response_codes(operation_method, response_schema),
                     deprecated=getattr(endpoint_settings.get(operation_method), 'deprecated', False),
+                    exclude_unset=True,
                     by_alias=True,
                     **{
                         'auth': endpoint_settings[operation_method].authentication
                         for _ in range(1) if getattr(endpoint_settings.get(operation_method), 'authentication', None)
                     }
                 ))(self._apply_authorization(view_func, authorization_callbacks))
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/middleware.py` & `django-hydrothings-0.1.6/src/hydrothings/middleware.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/src/hydrothings/schemas.py` & `django-hydrothings-0.1.6/src/hydrothings/schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,30 +58,33 @@
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
 
 class BaseListResponse(Schema):
     count: Union[int, None] = Field(None, alias='@iot.count')
-    value: list = []
+    values: list = []
     next_link: Union[AnyHttpUrl, None] = Field(None, alias='@iot.nextLink')
 
     class Config:
         allow_population_by_field_name = True
 
 
 class BaseGetResponse(Schema):
     id: UUID = Field(..., alias='@iot.id')
     self_link: AnyHttpUrl = Field(..., alias='@iot.selfLink')
 
     class Config:
         allow_population_by_field_name = True
 
 
-class QueryParams(Schema):
+class GetQueryParams(Schema):
+    expand: str = Field(None, alias='$expand')
+
+
+class ListQueryParams(GetQueryParams):
     filters: str = Field(None, alias='$filter')
     count: bool = Field(None, alias='$count')
     order_by: str = Field(None, alias='$orderby')
     skip: int = Field(0, alias='$skip')
     top: int = Field(None, alias='$top')
     select: str = Field(None, alias='$select')
-    expand: str = Field(None, alias='$expand')
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/settings.py` & `django-hydrothings-0.1.6/src/hydrothings/settings.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/src/hydrothings/utils.py` & `django-hydrothings-0.1.6/src/hydrothings/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import inspect
+import hydrothings.components as core_components
 import hydrothings.schemas as core_schemas
 from ninja import Schema
 from odata_query.grammar import ODataParser, ODataLexer
 from django.http import HttpResponse
 from pydantic import HttpUrl
 from typing import Literal, Union, List
 from requests import Response
@@ -104,26 +105,35 @@
         return response
 
     new_model = response_model.__new__(response_model)
 
     fields_values = {}
 
     for name, field in response_model.__fields__.items():
-        if name in response.keys():
+        if name.endswith('_rel') and name in response.keys():
+            if isinstance(response[name], list):
+                fields_values[name] = [
+                    serialize_response(
+                        entity, getattr(core_components, field.field_info.extra.get('nested_class'))
+                    ) for entity in response[name]
+                ]
+            else:
+                fields_values[name] = serialize_response(
+                    response[name], getattr(core_components, field.field_info.extra.get('nested_class'))
+                )
+        elif name in response.keys():
             if isinstance(response[name], list):
                 fields_values[name] = [
                     serialize_response(fv, field.type_)
                     for fv in response[name]
                 ]
             elif inspect.isclass(field.type_) and issubclass(field.type_, Schema):
                 fields_values[name] = serialize_response(response[name], field.type_)
             else:
                 fields_values[name] = response[name]
-        elif not field.required:
-            fields_values[name] = field.get_default()
 
     object.__setattr__(new_model, '__dict__', fields_values)
     _fields_set = set(response.keys())
     object.__setattr__(new_model, '__fields_set__', _fields_set)
 
     new_model._init_private_attributes()
 
@@ -174,25 +184,22 @@
 
     Returns
     -------
     dict
         A dictionary containing all parsed query parameters.
     """
 
-    lexer = ODataLexer()
-    parser = ODataParser()
-
     if entity_chain:
         if query_params.get('filters'):
             query_params['filters'] += f' and {entity_chain[-1][0]}/id eq {entity_chain[-1][1]}'
         else:
             query_params['filters'] = f'{entity_chain[-1][0]}/id eq {entity_chain[-1][1]}'
 
     if query_params.get('filters'):
-        query_params['filters'] = parser.parse(lexer.tokenize(query_params['filters']))
+        query_params['filters'] = tokenize_filters(query_params['filters'])
 
     if sort_datastream is True:
         if query_params.get('order_by'):
             query_params['order_by'] += ', Datastreams/id'
         else:
             query_params['order_by'] = 'Datastreams/id'
 
@@ -200,8 +207,68 @@
         query_params['order_by'] = [
             {
                 'field': order_field.strip().split(' ')[0],
                 'direction': 'desc' if order_field.strip().endswith('desc') else 'asc'
             } for order_field in query_params['order_by'].split(',')
         ]
 
+    if query_params.get('expand'):
+        expanded_entities = [
+            tokenize_expansion(entity)
+            for entity in query_params['expand'].split(',')
+        ]
+
+        query_params['expand'] = expanded_entities
+
     return query_params
+
+
+def tokenize_filters(filter_string):
+    """"""
+
+    lexer = ODataLexer()
+    parser = ODataParser()
+
+    return parser.parse(lexer.tokenize(filter_string))
+
+
+def tokenize_expansion(entity):
+    """"""
+
+    nav_props = entity.split('/')
+
+    if len(nav_props) == 0:
+        return None
+
+    nav_prop = nav_props[0]
+    filter_search = re.findall(r'\(.*?\)', nav_prop)
+
+    if filter_search and '$filter=' in filter_search[0]:
+        nav_prop = nav_prop.split('(')[0]
+        filters = tokenize_filters(filter_search[0][1:-1].replace('$filter=', ''))
+    else:
+        filters = None
+
+    if len(nav_props) > 1:
+        child_props = [tokenize_expansion('/'.join(nav_props[1:]))]
+    else:
+        child_props = []
+
+    try:
+        nav_prop = lookup_component(
+            input_value=nav_prop,
+            input_type='camel_plural',
+            output_type='camel_singular'
+        )
+        array = True
+    except:
+        array = False
+
+    return {
+        'component': nav_prop,
+        'array': array,
+        'select': None,
+        'filters': filters,
+        'order_by': None,
+        'pagination': None,
+        'children': child_props
+    }
```

### Comparing `django-hydrothings-0.1.5/src/hydrothings/validators.py` & `django-hydrothings-0.1.6/src/hydrothings/validators.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/tests/test_allow_partial_decorator.py` & `django-hydrothings-0.1.6/tests/test_allow_partial_decorator.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/tests/test_iso_interval_type.py` & `django-hydrothings-0.1.6/tests/test_iso_interval_type.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/tests/test_iso_time_type.py` & `django-hydrothings-0.1.6/tests/test_iso_time_type.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/tests/test_metadata_field_validator.py` & `django-hydrothings-0.1.6/tests/test_metadata_field_validator.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/tests/test_resolve_chained_entity_url.py` & `django-hydrothings-0.1.6/tests/test_resolve_chained_entity_url.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/tests/test_sensorthings_abstract_engine.py` & `django-hydrothings-0.1.6/tests/test_sensorthings_abstract_engine.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.5/tests/test_whitespace_validator.py` & `django-hydrothings-0.1.6/tests/test_whitespace_validator.py`

 * *Files identical despite different names*

