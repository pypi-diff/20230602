# Comparing `tmp/rlogging-1.1.5.tar.gz` & `tmp/rlogging-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlogging-1.1.5.tar", max compression
+gzip compressed data, was "rlogging-1.1.6.tar", max compression
```

## Comparing `rlogging-1.1.5.tar` & `rlogging-1.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1399 2023-06-01 21:18:55.176675 rlogging-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1465 2023-06-01 21:18:55.176675 rlogging-1.1.5/readme.md
--rw-r--r--   0        0        0       78 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/__init__.py
--rw-r--r--   0        0        0     3176 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/adapters.py
--rw-r--r--   0        0        0      125 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/filters.py
--rw-r--r--   0        0        0     2150 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/formatters.py
--rw-r--r--   0        0        0      990 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/handlers.py
--rw-r--r--   0        0        0        0 2023-06-01 21:38:16.119018 rlogging-1.1.5/rlogging/integration/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 21:38:16.119018 rlogging-1.1.5/rlogging/integration/aiogram/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 21:38:16.119018 rlogging-1.1.5/rlogging/integration/django/__init__.py
--rw-r--r--   0        0        0      727 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/integration/django/adapters.py
--rw-r--r--   0        0        0      125 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/integration/django/admin.py
--rw-r--r--   0        0        0      215 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/integration/django/apps.py
--rw-r--r--   0        0        0        0 2023-06-01 21:38:16.119018 rlogging-1.1.5/rlogging/integration/django/handlers.py
--rw-r--r--   0        0        0     1483 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/integration/django/middleware.py
--rw-r--r--   0        0        0       72 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/integration/django/models.py
--rw-r--r--   0        0        0     2019 2023-06-01 21:18:55.176675 rlogging-1.1.5/rlogging/integration/django/signals.py
--rw-r--r--   0        0        0        0 2023-06-01 21:38:16.119018 rlogging-1.1.5/rlogging/integration/fastapi/__init__.py
--rw-r--r--   0        0        0       50 2023-06-01 21:18:55.184675 rlogging-1.1.5/rlogging/namespaces.py
--rw-r--r--   0        0        0     1542 2023-06-01 21:18:55.184675 rlogging-1.1.5/rlogging/utils.py
--rw-r--r--   0        0        0     2496 1970-01-01 00:00:00.000000 rlogging-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1853 2023-06-01 21:52:25.714866 rlogging-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1465 2023-06-01 21:18:35.680770 rlogging-1.1.6/readme.md
+-rw-r--r--   0        0        0       78 2023-06-01 21:18:35.680770 rlogging-1.1.6/rlogging/__init__.py
+-rw-r--r--   0        0        0     3192 2023-06-01 21:52:25.714866 rlogging-1.1.6/rlogging/adapters.py
+-rw-r--r--   0        0        0      125 2023-06-01 21:18:35.680770 rlogging-1.1.6/rlogging/filters.py
+-rw-r--r--   0        0        0     2150 2023-06-01 21:18:35.680770 rlogging-1.1.6/rlogging/formatters.py
+-rw-r--r--   0        0        0      990 2023-06-01 21:18:35.680770 rlogging-1.1.6/rlogging/handlers.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:55:40.822062 rlogging-1.1.6/rlogging/integration/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:55:40.822062 rlogging-1.1.6/rlogging/integration/aiogram/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:55:40.822062 rlogging-1.1.6/rlogging/integration/django/__init__.py
+-rw-r--r--   0        0        0      727 2023-06-01 21:18:35.680770 rlogging-1.1.6/rlogging/integration/django/adapters.py
+-rw-r--r--   0        0        0      125 2023-06-01 21:18:35.680770 rlogging-1.1.6/rlogging/integration/django/admin.py
+-rw-r--r--   0        0        0      215 2023-06-01 21:18:35.680770 rlogging-1.1.6/rlogging/integration/django/apps.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:55:40.822062 rlogging-1.1.6/rlogging/integration/django/handlers.py
+-rw-r--r--   0        0        0     1483 2023-06-01 21:18:35.680770 rlogging-1.1.6/rlogging/integration/django/middleware.py
+-rw-r--r--   0        0        0       72 2023-06-01 21:18:35.684770 rlogging-1.1.6/rlogging/integration/django/models.py
+-rw-r--r--   0        0        0     2019 2023-06-01 21:18:35.684770 rlogging-1.1.6/rlogging/integration/django/signals.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:55:40.822062 rlogging-1.1.6/rlogging/integration/fastapi/__init__.py
+-rw-r--r--   0        0        0       50 2023-06-01 21:18:35.684770 rlogging-1.1.6/rlogging/namespaces.py
+-rw-r--r--   0        0        0     1542 2023-06-01 21:18:35.684770 rlogging-1.1.6/rlogging/utils.py
+-rw-r--r--   0        0        0     2496 1970-01-01 00:00:00.000000 rlogging-1.1.6/PKG-INFO
```

### Comparing `rlogging-1.1.5/pyproject.toml` & `rlogging-1.1.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -40,15 +40,42 @@
 line_length = 120
 
 [tool.ruff]
 select = ["A", "B", "C", "E", "F", "I", "UP"]
 fixable = ["A", "B", "C", "D", "E", "F", "I", "UP"]
 ignore = ["UP004", "D100", "D101", "D102", "D103", "D104", "D107", "D400", "D415"]
 line-length = 120
-target-version = "py37"
+target-version = "py38"
 
-[tool.ruff.mccabe]
-max-complexity = 10
+[tool.coverage.run]
+omit = [
+    "*/tests/*",
+    "install-poetry.py"
+]
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.coverage.report]
+exclude_lines = [
+    "pragma: no cover",
+    "def __repr__",
+    "raise AssertionError",
+    "raise NotImplementedError",
+    "if __name__ == .__main__.:",
+]
+
+[tool.pytest.ini_options]
+addopts = "-vvs --tb=short"
+xfail_strict = true
+testpaths = [
+    "tests",
+    "integration",
+]
+python_files = [
+    "tests/*.py",
+    "test_*.py"
+]
+filterwarnings = [
+    "ignore::DeprecationWarning",
+    "ignore:Module already imported:pytest.PytestWarning"
+]
+
+[tool.mypy]
+python_version = 3.8
```

### Comparing `rlogging-1.1.5/readme.md` & `rlogging-1.1.6/readme.md`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.5/rlogging/adapters.py` & `rlogging-1.1.6/rlogging/adapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import inspect
 import logging
 import sys
 import uuid
 from types import FrameType
-from typing import Any
+from typing import Any, Optional
 
 
 class RLoggerAdapter(logging.LoggerAdapter):
     """Путь логирования
 
     Создание логов, через флоу позволяет обоготить их
 
     """
 
     flow_id: uuid.UUID
 
-    def __init__(self, logger: logging.Logger, extra: dict | None = None) -> None:
+    def __init__(self, logger: logging.Logger, extra: Optional[dict] = None) -> None:
         extra = extra if extra is not None else {}
 
         super().__init__(logger, extra)
 
         self.flow_id = uuid.uuid1()
 
     def _extra_update(self, kwargs: dict, extra: dict):
         kwargs['extra'] = extra | kwargs.get('extra', {})
 
     def get_frame(self, stacklevel: int = 41) -> FrameType:
         return sys._getframe(5)
 
-    def get_class_info(self) -> dict | None:
+    def get_class_info(self) -> Optional[dict]:
         frame = self.get_frame()
         obj = frame.f_locals.get('self')
 
         if obj is None:
             return None
 
         module = inspect.getmodule(obj.__class__)
```

### Comparing `rlogging-1.1.5/rlogging/formatters.py` & `rlogging-1.1.6/rlogging/formatters.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.5/rlogging/handlers.py` & `rlogging-1.1.6/rlogging/handlers.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.5/rlogging/integration/django/adapters.py` & `rlogging-1.1.6/rlogging/integration/django/adapters.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.5/rlogging/integration/django/middleware.py` & `rlogging-1.1.6/rlogging/integration/django/middleware.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.5/rlogging/integration/django/signals.py` & `rlogging-1.1.6/rlogging/integration/django/signals.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.5/rlogging/utils.py` & `rlogging-1.1.6/rlogging/utils.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.5/PKG-INFO` & `rlogging-1.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlogging
-Version: 1.1.5
+Version: 1.1.6
 Summary: 
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

