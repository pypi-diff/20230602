# Comparing `tmp/django_freeman-0.1.0.tar.gz` & `tmp/django_freeman-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_freeman-0.1.0.tar", max compression
+gzip compressed data, was "django_freeman-0.1.1.tar", max compression
```

## Comparing `django_freeman-0.1.0.tar` & `django_freeman-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1080 2023-04-09 09:54:37.352354 django_freeman-0.1.0/LICENSE
--rw-r--r--   0        0        0       16 2023-04-09 09:54:37.352354 django_freeman-0.1.0/README.md
--rw-r--r--   0        0        0      114 2023-04-09 09:54:37.352354 django_freeman-0.1.0/freeman/__init__.py
--rw-r--r--   0        0        0      865 2023-04-09 09:54:37.352354 django_freeman-0.1.0/freeman/middlewares/errorhandling.py
--rw-r--r--   0        0        0     2051 2023-04-09 09:54:37.352354 django_freeman-0.1.0/freeman/middlewares/picking.py
--rw-r--r--   0        0        0     7673 2023-04-09 11:58:27.831801 django_freeman-0.1.0/freeman/models/abstract.py
--rw-r--r--   0        0        0      135 2023-04-09 09:54:37.356353 django_freeman-0.1.0/freeman/models/types.py
--rw-r--r--   0        0        0      614 2023-04-09 09:54:37.356353 django_freeman-0.1.0/freeman/utils/dsa.py
--rw-r--r--   0        0        0    24527 2023-04-14 10:48:34.591574 django_freeman-0.1.0/freeman/utils/dto.py
--rw-r--r--   0        0        0     1487 2023-04-14 08:12:32.587787 django_freeman-0.1.0/freeman/utils/exceptions.py
--rw-r--r--   0        0        0      983 2023-04-09 09:54:37.356353 django_freeman-0.1.0/freeman/utils/models.py
--rw-r--r--   0        0        0     1740 2023-04-09 09:54:37.356353 django_freeman-0.1.0/freeman/utils/picking.py
--rw-r--r--   0        0        0     5251 2023-04-09 09:54:37.356353 django_freeman-0.1.0/freeman/utils/query.py
--rw-r--r--   0        0        0     2778 2023-04-14 10:31:57.192412 django_freeman-0.1.0/freeman/utils/strings.py
--rw-r--r--   0        0        0      211 2023-04-09 09:54:37.356353 django_freeman-0.1.0/freeman/utils/typecheck.py
--rw-r--r--   0        0        0      499 2023-04-14 11:00:15.452285 django_freeman-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 django_freeman-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-04-09 09:54:37.352354 django_freeman-0.1.1/LICENSE
+-rw-r--r--   0        0        0       16 2023-04-09 09:54:37.352354 django_freeman-0.1.1/README.md
+-rw-r--r--   0        0        0      114 2023-04-09 09:54:37.352354 django_freeman-0.1.1/freeman/__init__.py
+-rw-r--r--   0        0        0      865 2023-04-09 09:54:37.352354 django_freeman-0.1.1/freeman/middlewares/errorhandling.py
+-rw-r--r--   0        0        0     1991 2023-06-02 17:45:43.235906 django_freeman-0.1.1/freeman/middlewares/picking.py
+-rw-r--r--   0        0        0     7547 2023-05-29 07:06:56.957703 django_freeman-0.1.1/freeman/models/abstract.py
+-rw-r--r--   0        0        0      135 2023-04-09 09:54:37.356353 django_freeman-0.1.1/freeman/models/types.py
+-rw-r--r--   0        0        0      111 2023-06-02 17:48:54.252370 django_freeman-0.1.1/freeman/settings.py
+-rw-r--r--   0        0        0      614 2023-04-09 09:54:37.356353 django_freeman-0.1.1/freeman/utils/dsa.py
+-rw-r--r--   0        0        0    24527 2023-04-14 10:48:34.591574 django_freeman-0.1.1/freeman/utils/dto.py
+-rw-r--r--   0        0        0     1487 2023-04-14 08:12:32.587787 django_freeman-0.1.1/freeman/utils/exceptions.py
+-rw-r--r--   0        0        0      590 2023-06-02 17:07:41.522792 django_freeman-0.1.1/freeman/utils/funcache.py
+-rw-r--r--   0        0        0      983 2023-04-09 09:54:37.356353 django_freeman-0.1.1/freeman/utils/models.py
+-rw-r--r--   0        0        0     1740 2023-04-09 09:54:37.356353 django_freeman-0.1.1/freeman/utils/picking.py
+-rw-r--r--   0        0        0     5266 2023-06-02 17:28:15.422988 django_freeman-0.1.1/freeman/utils/query.py
+-rw-r--r--   0        0        0     2778 2023-04-14 10:31:57.192412 django_freeman-0.1.1/freeman/utils/strings.py
+-rw-r--r--   0        0        0      211 2023-04-09 09:54:37.356353 django_freeman-0.1.1/freeman/utils/typecheck.py
+-rw-r--r--   0        0        0      519 2023-06-02 17:38:39.381922 django_freeman-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 django_freeman-0.1.1/PKG-INFO
```

### Comparing `django_freeman-0.1.0/LICENSE` & `django_freeman-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_freeman-0.1.0/freeman/middlewares/errorhandling.py` & `django_freeman-0.1.1/freeman/middlewares/errorhandling.py`

 * *Files identical despite different names*

### Comparing `django_freeman-0.1.0/freeman/middlewares/picking.py` & `django_freeman-0.1.1/freeman/middlewares/picking.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import json
 import typing
 from django.http import HttpResponse, HttpRequest
 from freeman.utils.picking import pick
-from django.conf import settings
-
-FREEMAN_PICK_PARAM_NAME = getattr(settings, "FREEMAN_PICK_PARAM_NAME", "pick")
+from freeman.settings import FREEMAN_PICK_PARAM_NAME
 
 
 class FreemanPickMiddleware:
     """
     Middleware that modifies the response of views by picking specific fields from JSON content.
 
     This middleware expects responses with a "Content-Type" header of "application/json".
```

### Comparing `django_freeman-0.1.0/freeman/models/abstract.py` & `django_freeman-0.1.1/freeman/models/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,14 @@
 
 
 class AbstractSharedModel(models.Model):
     id = models.UUIDField(default=uuid.uuid4, primary_key=True, editable=False)
     date_created = models.DateTimeField(auto_now_add=True, editable=False)
     last_updated = models.DateTimeField(auto_now_add=True, editable=False)
 
-    USE_GET_FUNCTIONS = True
-    USE_INSERT_FUNCTIONS = True
-    USE_UPDATE_FUNCTIONS = True
-    USE_DELETE_FUNCTIONS = True
-
     class Meta:
         abstract = True
 
     def serialize(self) -> DotDict:
         """
         Turns a model into a JSON serializable data. Must be overridden by the subclass.
```

### Comparing `django_freeman-0.1.0/freeman/utils/dsa.py` & `django_freeman-0.1.1/freeman/utils/dsa.py`

 * *Files identical despite different names*

### Comparing `django_freeman-0.1.0/freeman/utils/dto.py` & `django_freeman-0.1.1/freeman/utils/dto.py`

 * *Files identical despite different names*

### Comparing `django_freeman-0.1.0/freeman/utils/exceptions.py` & `django_freeman-0.1.1/freeman/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_freeman-0.1.0/freeman/utils/models.py` & `django_freeman-0.1.1/freeman/utils/models.py`

 * *Files identical despite different names*

### Comparing `django_freeman-0.1.0/freeman/utils/picking.py` & `django_freeman-0.1.1/freeman/utils/picking.py`

 * *Files identical despite different names*

### Comparing `django_freeman-0.1.0/freeman/utils/query.py` & `django_freeman-0.1.1/freeman/utils/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # it is treated as a field name and the search continues recursively on its corresponding value.
 # The Q objects created for each criterion are then combined using the _or
 # and _and conjunctions, or negated using the _not conjunction,
 # to create the final Q object that represents the entire search query.
 
 import typing
 from functools import reduce
+from .funcache import cached
 from django.db.models import Q
 from collections.abc import Sequence
 
-
 ConjunctionTypes: typing.TypeAlias = (
     typing.Literal["_or"] | typing.Literal["_and"] | typing.Literal["_not"]
 )
 CriterionTypes: typing.TypeAlias = (
     typing.Literal["_eq"]
     | typing.Literal["_neq"]
     | typing.Literal["_gt"]
@@ -98,15 +98,15 @@
 
 
 class QueryStructureError(BaseException):
     pass
 
 
 # make query func
-# TODO: cache function
+@cached()
 def makeQuery(query: dict[str, typing.Any], **kwargs: str) -> Q:
     # Get parent field name, if any
     parent: str = kwargs.get("parent", "")
 
     # Initialize list to store Q objects for each criterion
     res: list[Q] = []
```

### Comparing `django_freeman-0.1.0/freeman/utils/strings.py` & `django_freeman-0.1.1/freeman/utils/strings.py`

 * *Files identical despite different names*

### Comparing `django_freeman-0.1.0/PKG-INFO` & `django_freeman-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-freeman
-Version: 0.1.0
+Version: 0.1.1
 Summary: Collections of functions and helpers that helps speed up development of your django project
 License: MIT
 Author: rubbiekelvin
 Author-email: rubbiekelvinvoltsman@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

