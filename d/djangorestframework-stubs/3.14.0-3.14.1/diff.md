# Comparing `tmp/djangorestframework-stubs-3.14.0.tar.gz` & `tmp/djangorestframework-stubs-3.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-stubs-3.14.0.tar", last modified: Thu Apr 27 14:18:07 2023, max compression
+gzip compressed data, was "djangorestframework-stubs-3.14.1.tar", last modified: Fri Jun  2 14:19:49 2023, max compression
```

## Comparing `djangorestframework-stubs-3.14.0.tar` & `djangorestframework-stubs-3.14.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.141746 djangorestframework-stubs-3.14.0/
--rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/LICENSE.txt
--rw-r--r--   0 marti     (1000) marti      (121)     2494 2023-04-27 14:18:07.141746 djangorestframework-stubs-3.14.0/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)     1495 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/README.md
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.125080 djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/
--rw-r--r--   0 marti     (1000) marti      (121)     2494 2023-04-27 14:18:07.000000 djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)     3237 2023-04-27 14:18:07.000000 djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 marti     (1000) marti      (121)        1 2023-04-27 14:18:07.000000 djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 marti     (1000) marti      (121)      214 2023-04-27 14:18:07.000000 djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/requires.txt
--rw-r--r--   0 marti     (1000) marti      (121)       37 2023-04-27 14:18:07.000000 djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.125080 djangorestframework-stubs-3.14.0/mypy_drf_plugin/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/mypy_drf_plugin/__init__.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.128413 djangorestframework-stubs-3.14.0/mypy_drf_plugin/lib/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/mypy_drf_plugin/lib/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     2714 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/mypy_drf_plugin/lib/fullnames.py
--rw-r--r--   0 marti     (1000) marti      (121)      167 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/mypy_drf_plugin/lib/helpers.py
--rw-r--r--   0 marti     (1000) marti      (121)     1880 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/mypy_drf_plugin/main.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.128413 djangorestframework-stubs-3.14.0/mypy_drf_plugin/transformers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/mypy_drf_plugin/transformers/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)      355 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/mypy_drf_plugin/transformers/serializers.py
--rw-r--r--   0 marti     (1000) marti      (121)      207 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/pyproject.toml
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.135079 djangorestframework-stubs-3.14.0/rest_framework-stubs/
--rw-r--r--   0 marti     (1000) marti      (121)      193 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       77 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1115 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authentication.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.135079 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/
--rw-r--r--   0 marti     (1000) marti      (121)       24 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       74 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       73 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.135079 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.135079 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      394 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/management/commands/drf_create_token.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      296 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      196 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/serializers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      417 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/authtoken/views.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1985 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/compat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3265 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1560 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/documentation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3052 2023-04-27 14:17:42.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    23612 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2002 2023-04-27 14:17:42.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/filters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4415 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/generics.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.135079 djangorestframework-stubs-3.14.0/rest_framework-stubs/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.135079 djangorestframework-stubs-3.14.0/rest_framework-stubs/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      384 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/management/commands/generateschema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      737 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/metadata.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1260 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      739 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/negotiation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4964 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/pagination.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1794 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/parsers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3062 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/permissions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6893 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/relations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4382 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/renderers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3302 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/request.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1128 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/response.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      671 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/reverse.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2564 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/routers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.138413 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/
--rw-r--r--   0 marti     (1000) marti      (121)      973 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2814 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/coreapi.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2044 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/generators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      528 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/inspectors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3250 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/openapi.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      261 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      218 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/views.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    12294 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/serializers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4150 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/settings.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2642 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/status.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.138413 djangorestframework-stubs-3.14.0/rest_framework-stubs/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1658 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/templatetags/rest_framework.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5592 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/test.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1126 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/throttling.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      565 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/urlpatterns.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       89 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/urls.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 14:18:07.141746 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       86 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/breadcrumbs.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       54 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/encoders.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      918 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/field_mapping.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      404 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/formatting.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      213 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/html.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      183 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/humanize_datetime.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/json.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      293 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/mediatypes.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      703 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/model_meta.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      280 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/representation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1824 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/serializer_helpers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      145 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2975 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/validators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1169 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/versioning.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4716 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/views.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1835 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.0/rest_framework-stubs/viewsets.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      434 2023-04-27 14:18:07.141746 djangorestframework-stubs-3.14.0/setup.cfg
--rw-r--r--   0 marti     (1000) marti      (121)     2091 2023-04-27 14:17:42.000000 djangorestframework-stubs-3.14.0/setup.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:49.000298 djangorestframework-stubs-3.14.1/
+-rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/LICENSE.txt
+-rw-r--r--   0 marti     (1000) marti      (121)     2444 2023-06-02 14:19:49.000298 djangorestframework-stubs-3.14.1/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)     1495 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/README.md
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.986965 djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/
+-rw-r--r--   0 marti     (1000) marti      (121)     2444 2023-06-02 14:19:48.000000 djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)     3237 2023-06-02 14:19:48.000000 djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 marti     (1000) marti      (121)        1 2023-06-02 14:19:48.000000 djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 marti     (1000) marti      (121)      213 2023-06-02 14:19:48.000000 djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/requires.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       37 2023-06-02 14:19:48.000000 djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.986965 djangorestframework-stubs-3.14.1/mypy_drf_plugin/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/mypy_drf_plugin/__init__.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.986965 djangorestframework-stubs-3.14.1/mypy_drf_plugin/lib/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/mypy_drf_plugin/lib/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2714 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/mypy_drf_plugin/lib/fullnames.py
+-rw-r--r--   0 marti     (1000) marti      (121)      167 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/mypy_drf_plugin/lib/helpers.py
+-rw-r--r--   0 marti     (1000) marti      (121)     1880 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/mypy_drf_plugin/main.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.986965 djangorestframework-stubs-3.14.1/mypy_drf_plugin/transformers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/mypy_drf_plugin/transformers/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)      355 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/mypy_drf_plugin/transformers/serializers.py
+-rw-r--r--   0 marti     (1000) marti      (121)      207 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/pyproject.toml
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.993631 djangorestframework-stubs-3.14.1/rest_framework-stubs/
+-rw-r--r--   0 marti     (1000) marti      (121)      193 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       77 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1115 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authentication.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.996965 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/
+-rw-r--r--   0 marti     (1000) marti      (121)       24 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       74 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       73 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.996965 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.996965 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      394 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/management/commands/drf_create_token.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      296 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      196 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/serializers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      417 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/views.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1985 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/compat.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3273 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1560 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/documentation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3052 2023-04-27 14:17:42.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    23541 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2002 2023-04-27 14:17:42.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/filters.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4415 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/generics.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.996965 djangorestframework-stubs-3.14.1/rest_framework-stubs/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.996965 djangorestframework-stubs-3.14.1/rest_framework-stubs/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      384 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/management/commands/generateschema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      726 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/metadata.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1260 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      739 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/negotiation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4964 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/pagination.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1794 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/parsers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3062 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/permissions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6983 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/relations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4382 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/renderers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3202 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/request.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1128 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/response.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      671 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/reverse.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2564 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/routers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.996965 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/
+-rw-r--r--   0 marti     (1000) marti      (121)      973 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2794 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/coreapi.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2044 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/generators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      528 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/inspectors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3250 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/openapi.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      261 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      218 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/views.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    12294 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/serializers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4150 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/settings.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2642 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/status.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.996965 djangorestframework-stubs-3.14.1/rest_framework-stubs/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1658 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/templatetags/rest_framework.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5592 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/test.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1126 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/throttling.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      565 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/urlpatterns.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       89 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/urls.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:49.000298 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       86 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/breadcrumbs.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       54 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/encoders.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      918 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/field_mapping.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      404 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/formatting.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      213 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/html.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      183 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/humanize_datetime.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/json.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      293 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/mediatypes.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      703 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/model_meta.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      280 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/representation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1774 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/serializer_helpers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      145 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2975 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/validators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1169 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/versioning.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4716 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/views.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1792 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/viewsets.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      434 2023-06-02 14:19:49.000298 djangorestframework-stubs-3.14.1/setup.cfg
+-rw-r--r--   0 marti     (1000) marti      (121)     2041 2023-06-02 14:19:36.000000 djangorestframework-stubs-3.14.1/setup.py
```

### Comparing `djangorestframework-stubs-3.14.0/LICENSE.txt` & `djangorestframework-stubs-3.14.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/PKG-INFO` & `djangorestframework-stubs-3.14.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: djangorestframework-stubs
-Version: 3.14.0
+Version: 3.14.1
 Summary: PEP-484 stubs for django-rest-framework
 Home-page: https://github.com/typeddjango/djangorestframework-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
 Project-URL: Release notes, https://github.com/typeddjango/djangorestframework-stubs/releases
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: compatible-mypy
 Provides-Extra: coreapi
 Provides-Extra: markdown
 License-File: LICENSE.txt
 
 <img src="http://mypy-lang.org/static/mypy_light.svg" alt="mypy logo" width="300px"/>
@@ -31,15 +30,15 @@
 
 [![Build Status](https://travis-ci.com/typeddjango/djangorestframework-stubs.svg?branch=master)](https://travis-ci.com/typeddjango/djangorestframework-stubs)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Gitter](https://badges.gitter.im/mypy-django/Lobby.svg)](https://gitter.im/mypy-django/Lobby)
 
 
 Mypy stubs for [Django REST Framework](https://pypi.org/project/djangorestframework/).
-Supports Python 3.7 and up.
+Supports Python 3.8 and up.
 
 ## Installation
 
 ```bash
 pip install djangorestframework-stubs[compatible-mypy]
 ```
```

### Comparing `djangorestframework-stubs-3.14.0/README.md` & `djangorestframework-stubs-3.14.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [![Build Status](https://travis-ci.com/typeddjango/djangorestframework-stubs.svg?branch=master)](https://travis-ci.com/typeddjango/djangorestframework-stubs)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Gitter](https://badges.gitter.im/mypy-django/Lobby.svg)](https://gitter.im/mypy-django/Lobby)
 
 
 Mypy stubs for [Django REST Framework](https://pypi.org/project/djangorestframework/).
-Supports Python 3.7 and up.
+Supports Python 3.8 and up.
 
 ## Installation
 
 ```bash
 pip install djangorestframework-stubs[compatible-mypy]
 ```
```

### Comparing `djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/PKG-INFO` & `djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: djangorestframework-stubs
-Version: 3.14.0
+Version: 3.14.1
 Summary: PEP-484 stubs for django-rest-framework
 Home-page: https://github.com/typeddjango/djangorestframework-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
 Project-URL: Release notes, https://github.com/typeddjango/djangorestframework-stubs/releases
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: compatible-mypy
 Provides-Extra: coreapi
 Provides-Extra: markdown
 License-File: LICENSE.txt
 
 <img src="http://mypy-lang.org/static/mypy_light.svg" alt="mypy logo" width="300px"/>
@@ -31,15 +30,15 @@
 
 [![Build Status](https://travis-ci.com/typeddjango/djangorestframework-stubs.svg?branch=master)](https://travis-ci.com/typeddjango/djangorestframework-stubs)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Gitter](https://badges.gitter.im/mypy-django/Lobby.svg)](https://gitter.im/mypy-django/Lobby)
 
 
 Mypy stubs for [Django REST Framework](https://pypi.org/project/djangorestframework/).
-Supports Python 3.7 and up.
+Supports Python 3.8 and up.
 
 ## Installation
 
 ```bash
 pip install djangorestframework-stubs[compatible-mypy]
 ```
```

### Comparing `djangorestframework-stubs-3.14.0/djangorestframework_stubs.egg-info/SOURCES.txt` & `djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/mypy_drf_plugin/lib/fullnames.py` & `djangorestframework-stubs-3.14.1/mypy_drf_plugin/lib/fullnames.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/mypy_drf_plugin/main.py` & `djangorestframework-stubs-3.14.1/mypy_drf_plugin/main.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/authentication.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/authentication.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/compat.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/decorators.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/decorators.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -25,28 +25,28 @@
     def put(self, func: _View) -> _View: ...
     def patch(self, func: _View) -> _View: ...
     def delete(self, func: _View) -> _View: ...
     def head(self, func: _View) -> _View: ...
     def options(self, func: _View) -> _View: ...
     def trace(self, func: _View) -> _View: ...
 
-_LOWER_CASE_HTTP_VERBS: TypeAlias = list[
+_LOWER_CASE_HTTP_VERBS: TypeAlias = Sequence[
     Literal[
         "get",
         "post",
         "delete",
         "put",
         "patch",
         "trace",
         "head",
         "options",
     ]
 ]
 
-_MIXED_CASE_HTTP_VERBS: TypeAlias = list[
+_MIXED_CASE_HTTP_VERBS: TypeAlias = Sequence[
     Literal[
         "GET",
         "POST",
         "DELETE",
         "PUT",
         "PATCH",
         "TRACE",
```

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/documentation.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/documentation.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/exceptions.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/fields.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/fields.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import datetime
 import uuid
-from collections import OrderedDict
 from collections.abc import Callable, Generator, Iterable, Mapping, MutableMapping, Sequence
 from decimal import Decimal
 from enum import Enum
 from json import JSONDecoder, JSONEncoder
 from re import Pattern
 from typing import Any, Generic, NoReturn, Protocol, TypeVar
 
@@ -42,18 +41,18 @@
     label: StrOrPromise
     value: str
     display_text: StrOrPromise
 
 def is_simple_callable(obj: Callable) -> bool: ...
 def get_attribute(instance: Any, attrs: list[str] | None) -> Any: ...
 def set_value(dictionary: MutableMapping[str, Any], keys: Sequence[str], value: Any) -> None: ...
-def to_choices_dict(choices: Iterable[Any]) -> OrderedDict: ...
-def flatten_choices_dict(choices: dict[Any, Any]) -> OrderedDict: ...
+def to_choices_dict(choices: Iterable[Any]) -> dict: ...
+def flatten_choices_dict(choices: dict[Any, Any]) -> dict: ...
 def iter_options(
-    grouped_choices: OrderedDict, cutoff: int | None = ..., cutoff_text: StrOrPromise | None = ...
+    grouped_choices: dict, cutoff: int | None = ..., cutoff_text: StrOrPromise | None = ...
 ) -> Generator[Option, None, None]: ...
 def get_error_detail(exc_info: Any) -> Any: ...
 
 REGEX_TYPE: Pattern
 NOT_READ_ONLY_WRITE_ONLY: str
 NOT_READ_ONLY_REQUIRED: str
 NOT_REQUIRED_DEFAULT: str
@@ -450,17 +449,17 @@
         allow_null: bool = ...,
     ): ...
 
 class ChoiceField(Field[str, str | int | tuple[str | int, str | int | tuple], str, Any]):
     html_cutoff: int | None
     html_cutoff_text: StrOrPromise | None
     allow_blank: bool
-    grouped_choices: OrderedDict
+    grouped_choices: dict
     choice_strings_to_values: dict[str, Any]
-    _choices: OrderedDict
+    _choices: dict
     def __init__(
         self,
         choices: Iterable[Any],
         *,
         read_only: bool = ...,
         write_only: bool = ...,
         required: bool = ...,
```

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/filters.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/filters.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/generics.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/generics.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/metadata.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/metadata.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 from rest_framework import serializers
 from rest_framework.request import Request
 from rest_framework.serializers import BaseSerializer
 from rest_framework.utils.field_mapping import ClassLookupDict
 from rest_framework.views import APIView
 
 class BaseMetadata:
-    def determine_metadata(self, request: Request, view: APIView) -> dict[str, Any]: ...
+    def determine_metadata(self, request: Request, view: APIView) -> Any: ...
 
 class SimpleMetadata(BaseMetadata):
     label_lookup: ClassLookupDict[type[serializers.Field], str]
     def determine_actions(self, request: Request, view: APIView) -> dict[str, Any]: ...
     def get_serializer_info(self, serializer: BaseSerializer) -> dict[str, dict[str, Any]]: ...
     def get_field_info(self, field: serializers.Field) -> dict[str, Any]: ...
```

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/mixins.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/mixins.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/negotiation.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/negotiation.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/pagination.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/pagination.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/parsers.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/parsers.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/permissions.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/permissions.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/relations.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/relations.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from collections import OrderedDict
 from collections.abc import Callable, Iterable, Mapping, Sequence
 from typing import Any, Generic, TypeVar
 
 from _typeshed import Self
 from django.db.models import Manager, Model, QuerySet
+from django_stubs_ext import StrOrPromise
 from rest_framework.fields import Field, Option
 from rest_framework.request import Request
 from rest_framework.validators import Validator
 
 def method_overridden(method_name: str, klass: type, instance: Model) -> bool: ...
 
 class ObjectValueError(ValueError): ...
@@ -44,32 +44,32 @@
         html_cutoff_text: str = ...,
         read_only: bool = ...,
         write_only: bool = ...,
         required: bool = ...,
         default: Any = ...,
         initial: Any = ...,
         source: Callable | str = ...,
-        label: str | None = ...,
-        help_text: str = ...,
+        label: StrOrPromise | None = ...,
+        help_text: StrOrPromise = ...,
         allow_null: bool = ...,
         validators: Sequence[Validator[_MT]] | None = ...,
-        error_messages: dict[str, str] | None = ...,
+        error_messages: dict[str, StrOrPromise] | None = ...,
         style: dict[str, str] | None = ...,
     ): ...
     # mypy doesn't accept the typing below, although its accurate to what this class is doing, hence the ignore
     def __new__(cls, *args: Any, **kwargs: Any) -> RelatedField[_MT, _DT, _PT] | ManyRelatedField: ...  # type: ignore
     @classmethod
     def many_init(cls, *args: Any, **kwargs: Any) -> ManyRelatedField: ...
     def get_queryset(self) -> QuerySet[_MT]: ...
     def use_pk_only_optimization(self) -> bool: ...
-    def get_choices(self, cutoff: int | None = ...) -> OrderedDict: ...
+    def get_choices(self, cutoff: int | None = ...) -> dict: ...
     @property
-    def choices(self) -> OrderedDict: ...
+    def choices(self) -> dict: ...
     @property
-    def grouped_choices(self) -> OrderedDict: ...
+    def grouped_choices(self) -> dict: ...
     def iter_options(self) -> Iterable[Option]: ...
     def get_attribute(self, instance: _MT) -> _PT | None: ...  # type: ignore[override]
     def display_value(self, instance: _MT) -> str: ...
 
 class StringRelatedField(RelatedField[_MT, _MT, str]): ...
 
 class PrimaryKeyRelatedField(RelatedField[_MT, _MT, Any]):
@@ -83,19 +83,19 @@
         html_cutoff_text: str = ...,
         read_only: bool = ...,
         write_only: bool = ...,
         required: bool = ...,
         default: Any = ...,
         initial: Any = ...,
         source: Callable | str = ...,
-        label: str | None = ...,
-        help_text: str = ...,
+        label: StrOrPromise | None = ...,
+        help_text: StrOrPromise = ...,
         allow_null: bool = ...,
         validators: Sequence[Validator[_MT]] | None = ...,
-        error_messages: dict[str, str] | None = ...,
+        error_messages: dict[str, StrOrPromise] | None = ...,
         style: dict[str, str] | None = ...,
         pk_field: str | Field | None = ...,
     ): ...
 
 class HyperlinkedRelatedField(RelatedField[_MT, str, Hyperlink]):
     reverse: Callable
     lookup_field: str
@@ -111,19 +111,19 @@
         html_cutoff_text: str = ...,
         read_only: bool = ...,
         write_only: bool = ...,
         required: bool = ...,
         default: Any = ...,
         initial: Any = ...,
         source: Callable | str = ...,
-        label: str | None = ...,
-        help_text: str = ...,
+        label: StrOrPromise | None = ...,
+        help_text: StrOrPromise = ...,
         allow_null: bool = ...,
         validators: Sequence[Validator[_MT]] | None = ...,
-        error_messages: dict[str, str] | None = ...,
+        error_messages: dict[str, StrOrPromise] | None = ...,
         style: dict[str, str] | None = ...,
         view_name: str | None = ...,
         lookup_field: str | None = ...,
         lookup_url_kwarg: str | None = ...,
         format: str | None = ...,
     ): ...
     def get_object(self, view_name: str, *view_args: Any, **view_kwargs: Any) -> _MT: ...
@@ -142,19 +142,19 @@
         html_cutoff_text: str = ...,
         read_only: bool = ...,
         write_only: bool = ...,
         required: bool = ...,
         default: _DT = ...,
         initial: _MT | Callable[[Any], _MT] = ...,
         source: Callable | str = ...,
-        label: str | None = ...,
-        help_text: str = ...,
+        label: StrOrPromise | None = ...,
+        help_text: StrOrPromise = ...,
         allow_null: bool = ...,
         validators: Sequence[Validator[_MT]] | None = ...,
-        error_messages: dict[str, str] | None = ...,
+        error_messages: dict[str, StrOrPromise] | None = ...,
         style: dict[str, str] | None = ...,
         slug_field: str | None = ...,
     ): ...
     def to_internal_value(self, data: Any) -> _MT: ...
     def to_representation(self, value: _MT) -> str: ...
 
 class ManyRelatedField(Field[Sequence[Any], Sequence[Any], list[Any], Any]):
@@ -167,23 +167,23 @@
         self,
         read_only: bool = ...,
         write_only: bool = ...,
         required: bool = ...,
         default: Sequence[Any] = ...,
         initial: Sequence[Any] | Callable[[Any], Sequence[Any]] = ...,
         source: Callable | str = ...,
-        label: str | None = ...,
+        label: StrOrPromise | None = ...,
         help_text: str | None = ...,
         style: dict[str, str] | None = ...,
-        error_messages: dict[str, str] | None = ...,
+        error_messages: dict[str, StrOrPromise] | None = ...,
         validators: Sequence[Validator[Sequence[Any]]] | None = ...,
         allow_null: bool = ...,
         allow_empty: bool = ...,
         child_relation: RelatedField = ...,
     ): ...
     def get_value(self, dictionary: Mapping[Any, Any]) -> list[Any]: ...  # type: ignore[override]
-    def get_choices(self, cutoff: int | None = ...) -> OrderedDict: ...
+    def get_choices(self, cutoff: int | None = ...) -> dict: ...
     @property
-    def choices(self) -> OrderedDict: ...
+    def choices(self) -> dict: ...
     @property
-    def grouped_choices(self) -> OrderedDict: ...
+    def grouped_choices(self) -> dict: ...
     def iter_options(self) -> Iterable[Option]: ...
```

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/renderers.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/renderers.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/request.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/request.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -73,15 +73,11 @@
     def auth(self) -> Token | Any: ...
     @auth.setter
     def auth(self, value: Token | Any) -> None: ...
     @property
     def successful_authenticator(self) -> BaseAuthentication | ForcedAuthentication | None: ...
     def __getattr__(self, attr: str) -> Any: ...
     @property
-    def DATA(self) -> None: ...
-    @property
     def POST(self) -> _ImmutableQueryDict: ...  # type: ignore[override]
     @property
     def FILES(self): ...
-    @property
-    def QUERY_PARAMS(self) -> None: ...
     def force_plaintext_errors(self, value: Any) -> None: ...
```

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/response.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/response.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/reverse.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/reverse.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/routers.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/routers.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/__init__.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/coreapi.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/coreapi.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections import Counter, OrderedDict
+from collections import Counter
 from collections.abc import Iterable, Sequence
 from typing import Any
 
 from rest_framework.compat import coreapi
 from rest_framework.fields import Field
 from rest_framework.request import Request
 from rest_framework.urlpatterns import _AnyURL
@@ -13,15 +13,15 @@
 
 def common_path(paths: Iterable[str]) -> str: ...
 def is_custom_action(action: str) -> bool: ...
 def distribute_links(obj: Any) -> None: ...
 
 INSERT_INTO_COLLISION_FMT: str
 
-class LinkNode(OrderedDict):
+class LinkNode(dict):
     links: list[Any]
     methods_counter: Counter
     def __init__(self) -> None: ...
     def get_available_key(self, preferred_key: str) -> str: ...
 
 def insert_into(target: LinkNode, keys: Sequence[str], value: Any) -> None: ...
```

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/generators.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/generators.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/inspectors.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/inspectors.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/schemas/openapi.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/openapi.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/serializers.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/serializers.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/settings.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/settings.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/status.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/status.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/templatetags/rest_framework.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/templatetags/rest_framework.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/test.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/test.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/throttling.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/throttling.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/urlpatterns.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/urlpatterns.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/field_mapping.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/field_mapping.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/model_meta.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/model_meta.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/utils/serializer_helpers.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/serializer_helpers.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from collections import OrderedDict
 from collections.abc import Iterator, MutableMapping
 from typing import Any
 
 from rest_framework.exceptions import ErrorDetail
 from rest_framework.fields import Field
 from rest_framework.serializers import BaseSerializer
 
-class ReturnDict(OrderedDict):
+class ReturnDict(dict):
     serializer: BaseSerializer
     def __init__(self, serializer: BaseSerializer = ..., *args, **kwargs): ...
     def copy(self) -> ReturnDict: ...
     def __reduce__(self) -> tuple[dict, tuple[dict]]: ...
 
 class ReturnList(list):
     serializer: BaseSerializer
@@ -35,14 +34,14 @@
 
 class NestedBoundField(BoundField):
     def __iter__(self) -> Iterator[str]: ...
     def __getitem__(self, key: str) -> BoundField | NestedBoundField: ...
 
 class BindingDict(MutableMapping[str, Field]):
     serializer: BaseSerializer
-    fields: OrderedDict[str, Field]
+    fields: dict[str, Field]
     def __init__(self, serializer: BaseSerializer): ...
     def __setitem__(self, key: str, field: Field) -> None: ...
     def __getitem__(self, key: str) -> Field: ...
     def __delitem__(self, key: str) -> None: ...
     def __iter__(self) -> Iterator[Field]: ...  # type: ignore[override]
     def __len__(self) -> int: ...
```

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/validators.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/validators.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/versioning.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/versioning.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/views.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/views.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.0/rest_framework-stubs/viewsets.pyi` & `djangorestframework-stubs-3.14.1/rest_framework-stubs/viewsets.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections import OrderedDict
 from collections.abc import Callable
 from typing import Any
 
 from django.http.request import HttpRequest
 from django.http.response import HttpResponseBase
 from rest_framework import generics, mixins, views
 from rest_framework.decorators import ViewSetAction
@@ -32,15 +31,15 @@
     def as_view(
         cls, actions: dict[str, str | ViewSetAction] | None = ..., **initkwargs: Any
     ) -> AsView[GenericView]: ...
     def initialize_request(self, request: HttpRequest, *args: Any, **kwargs: Any) -> Request: ...
     def reverse_action(self, url_name: str, *args: Any, **kwargs: Any) -> str: ...
     @classmethod
     def get_extra_actions(cls) -> list[_ViewFunc]: ...
-    def get_extra_action_url_map(self) -> OrderedDict[str, str]: ...
+    def get_extra_action_url_map(self) -> dict[str, str]: ...
 
 class ViewSet(ViewSetMixin, views.APIView): ...
 class GenericViewSet(ViewSetMixin, generics.GenericAPIView[_MT_co]): ...
 class ReadOnlyModelViewSet(mixins.RetrieveModelMixin, mixins.ListModelMixin, GenericViewSet[_MT_co]): ...
 class ModelViewSet(
     mixins.CreateModelMixin,
     mixins.RetrieveModelMixin,
```

### Comparing `djangorestframework-stubs-3.14.0/setup.py` & `djangorestframework-stubs-3.14.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,48 +17,47 @@
 
 
 with open("README.md") as f:
     readme = f.read()
 
 dependencies = [
     "mypy>=0.991",
-    "django-stubs>=1.13.0",
+    "django-stubs>=4.2.1",
     "typing-extensions>=3.10.0",
     "requests>=2.0.0",
     "types-requests>=0.1.12",
     "types-PyYAML>=5.4.3",
 ]
 
 extras_require = {
-    "compatible-mypy": ["mypy>=1.2.0,<1.3"],
+    "compatible-mypy": ["mypy>=1.3.0,<1.4"],
     "coreapi": ["coreapi>=2.0.0"],
     "markdown": ["types-Markdown>=0.1.5"],
 }
 
 setup(
     name="djangorestframework-stubs",
-    version="3.14.0",
+    version="3.14.1",
     description="PEP-484 stubs for django-rest-framework",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/typeddjango/djangorestframework-stubs",
     author="Maksim Kurnikov",
     author_email="maxim.kurnikov@gmail.com",
     maintainer="Marti Raudsepp",
     maintainer_email="marti@juffo.org",
     license="MIT",
     install_requires=dependencies,
     extras_require=extras_require,
     packages=["rest_framework-stubs", *find_packages(exclude=["scripts"])],
     package_data={"rest_framework-stubs": find_stub_files("rest_framework-stubs")},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Framework :: Django",
     ],
```

