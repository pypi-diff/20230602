# Comparing `tmp/drf_pydantic_openapi-0.2.0.tar.gz` & `tmp/drf_pydantic_openapi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_pydantic_openapi-0.2.0.tar", max compression
+gzip compressed data, was "drf_pydantic_openapi-0.3.0.tar", max compression
```

## Comparing `drf_pydantic_openapi-0.2.0.tar` & `drf_pydantic_openapi-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0     1070 2023-04-27 13:44:08.423219 drf_pydantic_openapi-0.2.0/LICENSE
--rw-r--r--   0        0        0     2596 2023-05-09 09:59:45.223778 drf_pydantic_openapi-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-31 10:00:59.144732 drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/__init__.py
--rw-r--r--   0        0        0      164 2023-04-27 14:01:32.336379 drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/apps.py
--rw-r--r--   0        0        0     1456 2023-05-08 13:59:43.276920 drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/errors.py
--rw-r--r--   0        0        0      489 2023-04-27 13:44:28.146816 drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/exception_handler.py
--rw-r--r--   0        0        0     5197 2023-06-01 16:21:12.285971 drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/generator.py
--rw-r--r--   0        0        0     1517 2023-05-23 13:35:05.835776 drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/ref_source.py
--rw-r--r--   0        0        0     4143 2023-05-26 14:34:32.395942 drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/ref_utils.py
--rw-r--r--   0        0        0      815 2023-05-23 13:37:54.105323 drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/settings.py
--rw-r--r--   0        0        0      534 2023-06-01 15:09:21.868622 drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html
--rw-r--r--   0        0        0      256 2023-06-01 11:25:29.626778 drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/urls.py
--rw-r--r--   0        0        0     3794 2023-06-01 16:23:34.093901 drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/utils.py
--rw-r--r--   0        0        0     1223 2023-06-01 16:26:52.458916 drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/views.py
--rw-r--r--   0        0        0     1230 2023-06-01 16:27:42.614620 drf_pydantic_openapi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 drf_pydantic_openapi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-27 13:44:08.423219 drf_pydantic_openapi-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2596 2023-05-09 09:59:45.223778 drf_pydantic_openapi-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 10:00:59.144732 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-27 14:01:32.336379 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/apps.py
+-rw-r--r--   0        0        0     1456 2023-05-08 13:59:43.276920 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/errors.py
+-rw-r--r--   0        0        0      489 2023-04-27 13:44:28.146816 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/exception_handler.py
+-rw-r--r--   0        0        0     5780 2023-06-02 09:32:51.712376 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/generator.py
+-rw-r--r--   0        0        0     2289 2023-06-02 08:27:03.420495 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/patches.py
+-rw-r--r--   0        0        0     1476 2023-06-02 09:32:06.456794 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/path.py
+-rw-r--r--   0        0        0     1517 2023-05-23 13:35:05.835776 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/ref_source.py
+-rw-r--r--   0        0        0     4143 2023-05-26 14:34:32.395942 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/ref_utils.py
+-rw-r--r--   0        0        0      885 2023-06-02 08:31:26.725739 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/settings.py
+-rw-r--r--   0        0        0      435 2023-06-01 16:41:18.204945 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/templates/drf_pydantic_openapi/rapidoc.html
+-rw-r--r--   0        0        0      534 2023-06-01 15:09:21.868622 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html
+-rw-r--r--   0        0        0      256 2023-06-01 11:25:29.626778 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/urls.py
+-rw-r--r--   0        0        0     3938 2023-06-02 09:26:21.617715 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/utils.py
+-rw-r--r--   0        0        0     1720 2023-06-02 09:33:50.952500 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/views.py
+-rw-r--r--   0        0        0     1230 2023-06-02 09:34:18.528242 drf_pydantic_openapi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 drf_pydantic_openapi-0.3.0/PKG-INFO
```

### Comparing `drf_pydantic_openapi-0.2.0/LICENSE` & `drf_pydantic_openapi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.2.0/README.md` & `drf_pydantic_openapi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/errors.py` & `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/errors.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/generator.py` & `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import inspect
+import os
+import re
 from collections import defaultdict
-from dataclasses import dataclass
 from inspect import isclass
-from django.urls import get_resolver
 
+from django.urls import get_resolver
 from openapi_schema_pydantic import (
     Info,
     MediaType,
     OpenAPI,
     Operation,
     PathItem,
     RequestBody,
@@ -16,46 +17,45 @@
 from openapi_schema_pydantic.util import (
     PydanticSchema,
     construct_open_api_with_schema_class,
 )
 from pydantic import BaseModel
 from rest_framework.schemas.generators import BaseSchemaGenerator
 
-from .utils import (
-    Docstring,
-    ParameterLocation,
-    get_view_version,
-)
-
-
-@dataclass
-class Path:
-    """
-    Container for application api paths
-    """
-
-    name: str
-    method: str
-    view: callable
+from .path import Path
+from .settings import config
+from .utils import Docstring, ParameterLocation, get_view_version, method_mapping
 
 
 class Document(BaseSchemaGenerator):
-    def __init__(self, api_version: str, *args, **kwargs) -> None:
+    def __init__(self, api_version: str, tag_path_regex: str | None, *args, **kwargs) -> None:
         self.api_version = api_version
+        self.tag_path_regex = tag_path_regex
         self.openapi = OpenAPI(info=Info(title="test", version="3.0.0"), paths={})
         self.responses = {}
-        self.method_mapping = {
-            "get": "retrieve",
-            "post": "create",
-            "put": "update",
-            "patch": "partial_update",
-            "delete": "destroy",
-        }
         super().__init__(*args, **kwargs)
 
+    @property
+    def _tag_path_regex(self):
+        # Get path prefix regex
+        return self.tag_path_regex if self.tag_path_regex else config.tag_path_regex
+
+    def find_path_prefix(self, view_endpoints):
+        if self._tag_path_regex is None:
+            non_trivial_prefix = len(set([view.__class__ for _, _, view in view_endpoints])) > 1
+            if non_trivial_prefix:
+                path_prefix = os.path.commonpath([path for path, _, _ in view_endpoints])
+                path_prefix = re.escape(path_prefix)  # guard for RE special chars in path
+            else:
+                path_prefix = "/"
+        else:
+            path_prefix = self._tag_path_regex
+
+        return path_prefix
+
     def generate_responses(self, docstring, view_func):
         response = {}
         handler_signature = inspect.signature(view_func)
         return_type = handler_signature.return_annotation
         docs = getattr(view_func, "docs_metadata", None)
         if docs:
             if response_model := docs.response:
@@ -76,21 +76,19 @@
                 description = ""
                 if docstring and (returns := docstring.returns.get(error.__name__)):
                     description = returns.description
                 response["200"] = Response(
                     description=description,
                     content={"application/json": MediaType(schema=schema)},
                 )
-            else:
-                print("No type found")
         return response
 
-    def generate_operation(self, path: str, method: str, view) -> Operation | None:
-        method = method.lower()
-        view_func = getattr(view, method, getattr(view, self.method_mapping[method], None))
+    def generate_operation(self, path: Path) -> Operation | None:
+        method = path.method.lower()
+        view_func = getattr(path.view, method, getattr(path.view, method_mapping[method], None))
 
         if not view_func:
             return
 
         request_body = None
 
         docs = getattr(view_func, "docs_metadata", None)
@@ -104,43 +102,51 @@
 
         parameters = []
         if docs and (path_param := docs.generate_parameter(ParameterLocation.PATH)):
             parameters.append(path_param)
         if docs and (query_param := docs.generate_parameter(ParameterLocation.QUERY)):
             parameters.append(query_param)
 
-        path_name = path.replace("/", "_")
-
         return Operation(
-            operation_id=f"{method}_{path_name}_operation",
+            operation_id=path.get_operation_id(),
             requestBody=request_body,
+            tags=path.get_tags(),
             responses=self.generate_responses(docstring, view_func),
             summary=docstring.short_description if docstring else "",
             description=docstring.long_description if docstring else "",
             parameters=parameters,
         )
 
     def generate_docs(self, paths: list[Path]):
         docs = PathItem()
         for path in paths:
-            if operation := self.generate_operation(path.name, path.method, path.view):
+            if operation := self.generate_operation(path):
                 setattr(docs, path.method.lower(), operation)
         return docs
 
     def get_schema(self, request=None, public=False):
         self._initialise_endpoints()
         _, view_endpoints = self._get_paths_and_endpoints(request)
         paths = defaultdict(list)
+        path_prefix = self.find_path_prefix(view_endpoints)
+
         for path, method, view in view_endpoints:
             if self.api_version:
                 # resolver required by NamespaceVersioning
                 view.request.resolver_match = get_resolver().resolve(path)
                 if get_view_version(view) != self.api_version:
                     continue
-            paths[path].append(Path(name=path, method=method, view=view))
+            paths[path].append(
+                Path(
+                    path=path,
+                    path_prefix=path_prefix,
+                    method=method,
+                    view=view,
+                )
+            )
 
         for path in paths.keys():
             docs = self.generate_docs(paths[path])
             self.openapi.paths[path] = docs
 
         self.openapi = construct_open_api_with_schema_class(self.openapi)
         return self.openapi.json(by_alias=True, exclude_none=True)
```

### Comparing `drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/ref_source.py` & `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/ref_source.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/ref_utils.py` & `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/ref_utils.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/settings.py` & `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pydantic import BaseModel, Field
 
 from .ref_source import RefSource
 
 
 class Config(BaseModel):
     ref_sources: dict[str, RefSource] = Field(default={}, alias="REF_SOURCES")
+    tag_path_regex: str = Field(default=None, alias="TAG_PATH_REGEX")
 
     def get_source(self, name: str) -> RefSource | None:
         """Find source by given source name"""
         if ref_source := self.ref_sources.get(name):
             try:
                 ref_source.init()
                 return ref_source
```

### Comparing `drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html` & `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/utils.py` & `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 from openapi_schema_pydantic import Parameter, Schema
 from openapi_schema_pydantic.util import PydanticSchema
 from pydantic import BaseModel
 from rest_framework import exceptions
 
 from .errors import HttpError
 
+method_mapping = {
+    "get": "retrieve",
+    "post": "create",
+    "put": "update",
+    "patch": "partial_update",
+    "delete": "destroy",
+}
+
 _builtin_openapi_map = {
     builtins.bool: "boolean",
     builtins.str: "string",
     builtins.int: "integer",
     builtins.float: "number",
 }
```

### Comparing `drf_pydantic_openapi-0.2.0/drf_pydantic_openapi/views.py` & `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,32 +6,45 @@
 from rest_framework.reverse import reverse
 from rest_framework.views import APIView
 
 from .generator import Document
 
 
 class DrfPydanticSchemaView(APIView):
-    # TODO: get these from settings
     authentication_classes = {}
     permission_classes = {}
     api_version = None
+    tag_path_regex = None
 
     def get(self, request, *args, **kwargs):
         version = self.api_version
         if hasattr(request, "version"):
             version = request.version
 
-        document = Document(api_version=version)
+        document = Document(api_version=version, tag_path_regex=self.tag_path_regex)
         schema = document.get_schema(request=request)
         return Response(json.loads(schema), headers={"Cache-Control": "no-cache, no-store, must-revalidate"})
 
 
 class DrfPydanticRedocView(TemplateView):
     api_version = None
     template_name = "drf_pydantic_openapi/redoc.html"
     url_name = "dpo_schema"
 
     def get_context_data(self, **kwargs: Any) -> Dict[str, Any]:
         context = super().get_context_data(**kwargs)
         schema_url = f"{self.api_version}:{self.url_name}" if self.api_version else self.url_name
         context["schema_url"] = reverse(schema_url)
         return context
+
+
+class DrfPydanticRapidocView(TemplateView):
+    api_version = None
+    template_name = "drf_pydantic_openapi/rapidoc.html"
+    url_name = "dpo_schema"
+    rapidoc_settings = {}
+
+    def get_context_data(self, **kwargs: Any) -> Dict[str, Any]:
+        context = super().get_context_data(**kwargs)
+        schema_url = f"{self.api_version}:{self.url_name}" if self.api_version else self.url_name
+        context["schema_url"] = reverse(schema_url)
+        return context
```

### Comparing `drf_pydantic_openapi-0.2.0/pyproject.toml` & `drf_pydantic_openapi-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-pydantic-openapi"
-version = "0.2.0"
+version = "0.3.0"
 description = "OpenAPI (v3) schema generation via Pydantic models using Django REST Framework."
 authors = ["iKlotho <umutkahrimanedu@gmail.com>"]
 readme = "README.md"
 packages = [{include = "drf_pydantic_openapi"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `drf_pydantic_openapi-0.2.0/PKG-INFO` & `drf_pydantic_openapi-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-pydantic-openapi
-Version: 0.2.0
+Version: 0.3.0
 Summary: OpenAPI (v3) schema generation via Pydantic models using Django REST Framework.
 Author: iKlotho
 Author-email: umutkahrimanedu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

