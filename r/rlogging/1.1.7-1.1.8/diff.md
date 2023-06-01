# Comparing `tmp/rlogging-1.1.7.tar.gz` & `tmp/rlogging-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlogging-1.1.7.tar", max compression
+gzip compressed data, was "rlogging-1.1.8.tar", max compression
```

## Comparing `rlogging-1.1.7.tar` & `rlogging-1.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1853 2023-06-01 21:59:37.121107 rlogging-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     1465 2023-06-01 21:59:37.121107 rlogging-1.1.7/readme.md
--rw-r--r--   0        0        0       78 2023-06-01 21:59:37.121107 rlogging-1.1.7/rlogging/__init__.py
--rw-r--r--   0        0        0     3199 2023-06-01 21:59:37.121107 rlogging-1.1.7/rlogging/adapters.py
--rw-r--r--   0        0        0      125 2023-06-01 21:59:37.121107 rlogging-1.1.7/rlogging/filters.py
--rw-r--r--   0        0        0     2150 2023-06-01 21:59:37.121107 rlogging-1.1.7/rlogging/formatters.py
--rw-r--r--   0        0        0      990 2023-06-01 21:59:37.121107 rlogging-1.1.7/rlogging/handlers.py
--rw-r--r--   0        0        0        0 2023-06-01 21:59:37.229106 rlogging-1.1.7/rlogging/integration/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 21:59:37.237106 rlogging-1.1.7/rlogging/integration/aiogram/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 21:59:37.241106 rlogging-1.1.7/rlogging/integration/django/__init__.py
--rw-r--r--   0        0        0      727 2023-06-01 21:59:37.121107 rlogging-1.1.7/rlogging/integration/django/adapters.py
--rw-r--r--   0        0        0      125 2023-06-01 21:59:37.121107 rlogging-1.1.7/rlogging/integration/django/admin.py
--rw-r--r--   0        0        0      215 2023-06-01 21:59:37.125107 rlogging-1.1.7/rlogging/integration/django/apps.py
--rw-r--r--   0        0        0        0 2023-06-01 21:59:37.241106 rlogging-1.1.7/rlogging/integration/django/handlers.py
--rw-r--r--   0        0        0     1483 2023-06-01 21:59:37.125107 rlogging-1.1.7/rlogging/integration/django/middleware.py
--rw-r--r--   0        0        0       72 2023-06-01 21:59:37.133107 rlogging-1.1.7/rlogging/integration/django/models.py
--rw-r--r--   0        0        0     2019 2023-06-01 21:59:37.133107 rlogging-1.1.7/rlogging/integration/django/signals.py
--rw-r--r--   0        0        0        0 2023-06-01 21:59:37.241106 rlogging-1.1.7/rlogging/integration/fastapi/__init__.py
--rw-r--r--   0        0        0       50 2023-06-01 21:59:37.133107 rlogging-1.1.7/rlogging/namespaces.py
--rw-r--r--   0        0        0     1542 2023-06-01 21:59:37.133107 rlogging-1.1.7/rlogging/utils.py
--rw-r--r--   0        0        0     2496 1970-01-01 00:00:00.000000 rlogging-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1853 2023-06-01 22:05:36.303549 rlogging-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1465 2023-06-01 22:05:36.303549 rlogging-1.1.8/readme.md
+-rw-r--r--   0        0        0       78 2023-06-01 22:05:36.303549 rlogging-1.1.8/rlogging/__init__.py
+-rw-r--r--   0        0        0     3199 2023-06-01 22:05:36.307549 rlogging-1.1.8/rlogging/adapters.py
+-rw-r--r--   0        0        0      125 2023-06-01 22:05:36.307549 rlogging-1.1.8/rlogging/filters.py
+-rw-r--r--   0        0        0     2173 2023-06-01 22:05:36.307549 rlogging-1.1.8/rlogging/formatters.py
+-rw-r--r--   0        0        0      990 2023-06-01 22:05:36.307549 rlogging-1.1.8/rlogging/handlers.py
+-rw-r--r--   0        0        0        0 2023-06-01 22:05:36.751547 rlogging-1.1.8/rlogging/integration/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 22:05:36.751547 rlogging-1.1.8/rlogging/integration/aiogram/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 22:05:36.751547 rlogging-1.1.8/rlogging/integration/django/__init__.py
+-rw-r--r--   0        0        0      727 2023-06-01 22:05:36.307549 rlogging-1.1.8/rlogging/integration/django/adapters.py
+-rw-r--r--   0        0        0      125 2023-06-01 21:18:55.176675 rlogging-1.1.8/rlogging/integration/django/admin.py
+-rw-r--r--   0        0        0      215 2023-06-01 22:05:36.307549 rlogging-1.1.8/rlogging/integration/django/apps.py
+-rw-r--r--   0        0        0        0 2023-06-01 22:05:36.751547 rlogging-1.1.8/rlogging/integration/django/handlers.py
+-rw-r--r--   0        0        0     1483 2023-06-01 22:05:36.307549 rlogging-1.1.8/rlogging/integration/django/middleware.py
+-rw-r--r--   0        0        0       72 2023-06-01 21:18:55.176675 rlogging-1.1.8/rlogging/integration/django/models.py
+-rw-r--r--   0        0        0     2019 2023-06-01 21:18:55.176675 rlogging-1.1.8/rlogging/integration/django/signals.py
+-rw-r--r--   0        0        0        0 2023-06-01 22:05:36.751547 rlogging-1.1.8/rlogging/integration/fastapi/__init__.py
+-rw-r--r--   0        0        0       50 2023-06-01 21:18:55.184675 rlogging-1.1.8/rlogging/namespaces.py
+-rw-r--r--   0        0        0     1542 2023-06-01 22:05:36.307549 rlogging-1.1.8/rlogging/utils.py
+-rw-r--r--   0        0        0     2496 1970-01-01 00:00:00.000000 rlogging-1.1.8/PKG-INFO
```

### Comparing `rlogging-1.1.7/pyproject.toml` & `rlogging-1.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.7/readme.md` & `rlogging-1.1.8/readme.md`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.7/rlogging/adapters.py` & `rlogging-1.1.8/rlogging/adapters.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.7/rlogging/formatters.py` & `rlogging-1.1.8/rlogging/formatters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import logging
+from typing import Set
 
 from rlogging import utils
 
 
 class RFormatter(logging.Formatter):
     """Кастомный форматер модуля"""
 
@@ -18,15 +19,15 @@
         'exc_info',
         'stack_info',
         'exc_text',
         # 'threadName',
         'thread',
     }
 
-    def __init__(self, include_fields: set[str] = None, exclude_fields: set[str] = None, *args, **kwargs):
+    def __init__(self, include_fields: Set[str] = None, exclude_fields: Set[str] = None, *args, **kwargs):
         super().__init__(*args)
 
         self.include_fields = set(include_fields) if include_fields is not None else None
         self.exclude_fields = set(exclude_fields) if exclude_fields is not None else None
 
         if self.include_fields is None and self.exclude_fields is None:
             self.exclude_fields = self.DEFAULT_EXCLUDE_FIELDS
```

### Comparing `rlogging-1.1.7/rlogging/handlers.py` & `rlogging-1.1.8/rlogging/handlers.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.7/rlogging/integration/django/adapters.py` & `rlogging-1.1.8/rlogging/integration/django/adapters.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.7/rlogging/integration/django/middleware.py` & `rlogging-1.1.8/rlogging/integration/django/middleware.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.7/rlogging/integration/django/signals.py` & `rlogging-1.1.8/rlogging/integration/django/signals.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.7/rlogging/utils.py` & `rlogging-1.1.8/rlogging/utils.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.7/PKG-INFO` & `rlogging-1.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlogging
-Version: 1.1.7
+Version: 1.1.8
 Summary: 
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

