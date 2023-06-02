# Comparing `tmp/drakaina-0.7.0b4.tar.gz` & `tmp/drakaina-0.7.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drakaina-0.7.0b4.tar", max compression
+gzip compressed data, was "drakaina-0.7.0b6.tar", max compression
```

## Comparing `drakaina-0.7.0b4.tar` & `drakaina-0.7.0b6.tar`

### file list

```diff
@@ -1,41 +1,28 @@
--rw-r--r--   0        0        0     9270 2023-05-30 13:55:11.975948 drakaina-0.7.0b4/drakaina/__init__.py
--rw-r--r--   0        0        0     1494 2023-01-27 12:48:38.216236 drakaina-0.7.0b4/drakaina/asgi.py
--rw-r--r--   0        0        0     3699 2023-02-13 13:22:12.183448 drakaina-0.7.0b4/drakaina/client/__init__.py
--rw-r--r--   0        0        0     6158 2022-07-08 05:47:38.000000 drakaina-0.7.0b4/drakaina/client/base.py
--rw-r--r--   0        0        0     1832 2022-07-08 05:47:38.000000 drakaina-0.7.0b4/drakaina/client/http.py
--rw-r--r--   0        0        0    11280 2023-01-27 12:55:37.114745 drakaina-0.7.0b4/drakaina/client/tcp.py
--rw-r--r--   0        0        0     8797 2022-07-08 05:47:38.000000 drakaina-0.7.0b4/drakaina/client/websocket.py
--rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.0b4/drakaina/contrib/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.0b4/drakaina/contrib/django/__init__.py
--rw-r--r--   0        0        0     6132 2023-04-11 08:46:20.669302 drakaina-0.7.0b4/drakaina/contrib/django/middleware.py
--rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.0b4/drakaina/contrib/django/views.py
--rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.0b4/drakaina/contrib/jwt/__init__.py
--rw-r--r--   0        0        0      348 2023-03-10 11:02:10.213372 drakaina-0.7.0b4/drakaina/contrib/jwt/errors.py
--rw-r--r--   0        0        0     8847 2023-05-30 13:55:11.976951 drakaina-0.7.0b4/drakaina/contrib/jwt/middleware.py
--rw-r--r--   0        0        0      911 2023-05-29 22:21:28.708378 drakaina-0.7.0b4/drakaina/contrib/jwt/types.py
--rw-r--r--   0        0        0    18201 2023-05-30 13:55:11.977951 drakaina-0.7.0b4/drakaina/contrib/jwt/utils.py
--rw-r--r--   0        0        0     4115 2023-05-28 21:21:43.059480 drakaina-0.7.0b4/drakaina/drakaina_openapi.py
--rw-r--r--   0        0        0     1327 2023-05-11 09:46:59.367413 drakaina-0.7.0b4/drakaina/exceptions.py
--rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.0b4/drakaina/middleware/__init__.py
--rw-r--r--   0        0        0     1370 2023-05-29 22:21:28.722375 drakaina-0.7.0b4/drakaina/middleware/base.py
--rw-r--r--   0        0        0     7364 2023-05-30 13:55:11.978951 drakaina-0.7.0b4/drakaina/middleware/cors.py
--rw-r--r--   0        0        0     1967 2023-05-30 13:55:11.980056 drakaina-0.7.0b4/drakaina/middleware/exception.py
--rw-r--r--   0        0        0      430 2023-04-13 16:28:59.822156 drakaina-0.7.0b4/drakaina/middleware/gzip.py
--rw-r--r--   0        0        0      983 2023-04-04 11:19:41.525282 drakaina-0.7.0b4/drakaina/middleware/logging.py
--rw-r--r--   0        0        0     1072 2023-05-29 22:42:27.401282 drakaina-0.7.0b4/drakaina/middleware/request_wrapper.py
--rw-r--r--   0        0        0    12285 2023-05-30 13:55:11.980056 drakaina-0.7.0b4/drakaina/registries.py
--rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.0b4/drakaina/rpc_protocols/__init__.py
--rw-r--r--   0        0        0     7317 2023-05-30 13:55:11.981055 drakaina-0.7.0b4/drakaina/rpc_protocols/base.py
--rw-r--r--   0        0        0    20624 2023-05-30 13:55:11.982509 drakaina-0.7.0b4/drakaina/rpc_protocols/jsonrpc20.py
--rw-r--r--   0        0        0      200 2023-01-09 10:12:10.047554 drakaina-0.7.0b4/drakaina/rsgi.py
--rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.0b4/drakaina/serializers.py
--rw-r--r--   0        0        0    11142 2023-01-27 12:51:42.029067 drakaina-0.7.0b4/drakaina/tcp.py
--rw-r--r--   0        0        0    22700 2023-05-30 13:55:11.982509 drakaina-0.7.0b4/drakaina/types.py
--rw-r--r--   0        0        0     3625 2023-05-30 13:55:11.983500 drakaina-0.7.0b4/drakaina/utils.py
--rw-r--r--   0        0        0      162 2023-01-25 16:44:10.299855 drakaina-0.7.0b4/drakaina/ws.py
--rw-r--r--   0        0        0     8212 2023-05-30 13:55:11.984506 drakaina-0.7.0b4/drakaina/wsgi.py
--rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.0b4/LICENSE
--rw-r--r--   0        0        0     2595 2023-05-30 13:55:11.984506 drakaina-0.7.0b4/pyproject.toml
--rw-r--r--   0        0        0     5200 2023-05-30 13:55:11.974952 drakaina-0.7.0b4/README.md
--rw-r--r--   0        0        0     6671 1970-01-01 00:00:00.000000 drakaina-0.7.0b4/setup.py
--rw-r--r--   0        0        0     6892 1970-01-01 00:00:00.000000 drakaina-0.7.0b4/PKG-INFO
+-rw-r--r--   0        0        0     9270 2023-06-02 11:15:23.718906 drakaina-0.7.0b6/drakaina/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.0b6/drakaina/contrib/__init__.py
+-rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.0b6/drakaina/contrib/django/__init__.py
+-rw-r--r--   0        0        0     6267 2023-06-01 12:00:05.542467 drakaina-0.7.0b6/drakaina/contrib/django/middleware.py
+-rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.0b6/drakaina/contrib/django/views.py
+-rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.0b6/drakaina/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0      348 2023-03-10 11:02:10.213372 drakaina-0.7.0b6/drakaina/contrib/jwt/errors.py
+-rw-r--r--   0        0        0     8847 2023-06-02 11:15:23.719893 drakaina-0.7.0b6/drakaina/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0      911 2023-05-29 22:21:28.708378 drakaina-0.7.0b6/drakaina/contrib/jwt/types.py
+-rw-r--r--   0        0        0    18201 2023-06-02 11:15:23.720890 drakaina-0.7.0b6/drakaina/contrib/jwt/utils.py
+-rw-r--r--   0        0        0     1327 2023-05-11 09:46:59.367413 drakaina-0.7.0b6/drakaina/exceptions.py
+-rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.0b6/drakaina/middleware/__init__.py
+-rw-r--r--   0        0        0     1370 2023-05-29 22:21:28.722375 drakaina-0.7.0b6/drakaina/middleware/base.py
+-rw-r--r--   0        0        0     7364 2023-06-02 11:15:23.721960 drakaina-0.7.0b6/drakaina/middleware/cors.py
+-rw-r--r--   0        0        0     1967 2023-06-02 11:15:23.721960 drakaina-0.7.0b6/drakaina/middleware/exception.py
+-rw-r--r--   0        0        0     1072 2023-05-29 22:42:27.401282 drakaina-0.7.0b6/drakaina/middleware/request_wrapper.py
+-rw-r--r--   0        0        0    12337 2023-06-02 11:15:23.722960 drakaina-0.7.0b6/drakaina/registries.py
+-rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.0b6/drakaina/rpc_protocols/__init__.py
+-rw-r--r--   0        0        0     7317 2023-06-02 11:15:23.722960 drakaina-0.7.0b6/drakaina/rpc_protocols/base.py
+-rw-r--r--   0        0        0    13954 2023-06-02 11:15:23.723959 drakaina-0.7.0b6/drakaina/rpc_protocols/jsonrpc20.py
+-rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.0b6/drakaina/serializers.py
+-rw-r--r--   0        0        0    30834 2023-06-02 11:15:23.724958 drakaina-0.7.0b6/drakaina/types.py
+-rw-r--r--   0        0        0     3625 2023-06-02 11:15:23.725965 drakaina-0.7.0b6/drakaina/utils.py
+-rw-r--r--   0        0        0     8212 2023-06-02 11:15:23.726959 drakaina-0.7.0b6/drakaina/wsgi.py
+-rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.0b6/LICENSE
+-rw-r--r--   0        0        0     2672 2023-06-02 10:50:25.172544 drakaina-0.7.0b6/pyproject.toml
+-rw-r--r--   0        0        0     5366 2023-06-02 11:15:23.718906 drakaina-0.7.0b6/README.md
+-rw-r--r--   0        0        0     7010 1970-01-01 00:00:00.000000 drakaina-0.7.0b6/PKG-INFO
```

### Comparing `drakaina-0.7.0b4/drakaina/__init__.py` & `drakaina-0.7.0b6/drakaina/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/drakaina/contrib/django/__init__.py` & `drakaina-0.7.0b6/drakaina/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/drakaina/contrib/django/middleware.py` & `drakaina-0.7.0b6/drakaina/contrib/django/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Optional
 from typing import Protocol
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.http import HttpRequest
 from django.http import HttpResponse
+from django.utils.functional import SimpleLazyObject
 from django.utils.module_loading import import_string
 
 from drakaina import ENV_AUTH_PAYLOAD
 from drakaina import ENV_AUTH_SCOPES
 from drakaina import ENV_IS_AUTHENTICATED
 from drakaina import ENV_USER_ID
 from drakaina.contrib import django as default_settings
@@ -123,15 +124,17 @@
                     )
 
             setattr(request, ENV_USER_ID, payload[self.user_id_field])
             setattr(request, ENV_IS_AUTHENTICATED, True)
             setattr(request, ENV_AUTH_PAYLOAD, payload)
 
             if callable(self.get_user):
-                request.user = self.get_user(request, payload)
+                request.user = SimpleLazyObject(
+                    lambda: self.get_user(request, payload),
+                )
             if callable(self.get_scopes):
                 setattr(
                     request,
                     ENV_AUTH_SCOPES,
                     self.get_scopes(request, payload),
                 )
 
@@ -167,14 +170,14 @@
         self,
         request: HttpRequest,
         payload: dict[str, Any],
     ) -> Optional[UserModel]:
         user_id = payload.get(self.user_id_field)
         if user_id is None:
             return getattr(request, "user", None)
-        return UserModel.objects.get(pk=user_id)
+        return UserModel._default_manager.get(pk=user_id)  # noqa
 
     def _error_response(self, error: Exception) -> HttpResponse:
         return HttpResponse(
             content=self._rpc_handler.get_raw_error(error),
             content_type=self._rpc_handler.content_type,
         )
```

### Comparing `drakaina-0.7.0b4/drakaina/contrib/django/views.py` & `drakaina-0.7.0b6/drakaina/contrib/django/views.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/drakaina/contrib/jwt/middleware.py` & `drakaina-0.7.0b6/drakaina/contrib/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/drakaina/contrib/jwt/types.py` & `drakaina-0.7.0b6/drakaina/contrib/jwt/types.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/drakaina/contrib/jwt/utils.py` & `drakaina-0.7.0b6/drakaina/contrib/jwt/utils.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/drakaina/exceptions.py` & `drakaina-0.7.0b6/drakaina/exceptions.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/drakaina/middleware/base.py` & `drakaina-0.7.0b6/drakaina/middleware/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/drakaina/middleware/cors.py` & `drakaina-0.7.0b6/drakaina/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/drakaina/middleware/exception.py` & `drakaina-0.7.0b6/drakaina/middleware/exception.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/drakaina/middleware/request_wrapper.py` & `drakaina-0.7.0b6/drakaina/middleware/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/drakaina/registries.py` & `drakaina-0.7.0b6/drakaina/registries.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
                 "Method names that begin with 'rpc.' are reserved for "
                 "rpc internal methods and extensions and MUST NOT be used "
                 "for anything else.",
             )
 
         # Inspection of the procedure interface and its documentation.
         schema = self.inspect_procedure(procedure, metadata)
+        schema["name"] = procedure_name
 
         self.__register_callable(
             func=procedure,
             name=procedure_name,
             provide_request=provide_request,
             schema=schema,
             metadata=metadata,
@@ -138,16 +139,16 @@
             May contain additional information about the signature or
             documentation about the procedure.
         :return:
             Returns the schema for the given procedure filled with
             the found data.
 
         """
-        if "doc_schema" in metadata:
-            schema = metadata["doc_schema"]
+        if "method_schema" in metadata:
+            schema = metadata["method_schema"]
         else:
             schema = MethodSchema(parameters=OrderedDict(), result={})
 
         if callable(parse_doc):
             docstring = parse_doc(getattr(procedure, "__doc__", ""))
             docstring.params_dict = {p.arg_name: p for p in docstring.params}
             if docstring.short_description:
@@ -274,15 +275,15 @@
         # applied once
         _func = func
         while _func is not None:
             setattr(_func, RPC_REGISTRY, self)
             setattr(_func, RPC_REGISTERED, True)
             setattr(_func, RPC_NAME, name)
             setattr(_func, RPC_PROVIDE_REQUEST, provide_request)
-            setattr(_func, RPC_SCHEMA, schema)
+            setattr(_func, RPC_SCHEMA, schema or {})
             setattr(_func, RPC_META, metadata or {})
             # If it's a wrapped function
             _func = getattr(_func, "__wrapped__", None)
 
         self._remote_procedures[name] = func
 
     def replace(
```

### Comparing `drakaina-0.7.0b4/drakaina/rpc_protocols/base.py` & `drakaina-0.7.0b6/drakaina/rpc_protocols/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/drakaina/rpc_protocols/jsonrpc20.py` & `drakaina-0.7.0b6/drakaina/rpc_protocols/jsonrpc20.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from copy import deepcopy
+from functools import partial
 from typing import Any
 from typing import ClassVar
 
 from drakaina.exceptions import AuthenticationFailedError
 from drakaina.exceptions import BadRequestError
 from drakaina.exceptions import DeserializationError
 from drakaina.exceptions import ForbiddenError
@@ -282,15 +283,15 @@
         self.openapi_schema_template = (
             openapi if openapi is not None else DEFAULT_OPENAPI_SCHEMA
         )
         self.__openapi_schema = None
 
         if allow_service_discovery:
             self.registry.register_rpc_extension(
-                extension_procedure=self.rpc_discover,
+                extension_procedure=partial(rpc_discover, protocol=self),
                 extension_name="rpc.discover",
             )
 
     def handle(
         self,
         rpc_request: JSONRPCRequest,
         request: Any | None = None,
@@ -389,94 +390,38 @@
             return InternalError(message=str(err), id=request_id).as_dict()
 
         if request_id is None:
             return None
 
         return dict(jsonrpc="2.0", result=result, id=request_id)
 
-    def rpc_discover(self) -> dict[str, Any]:
-        """Returns an OpenRPC schema as a description of this service.
-
-        :return:
-
-        """
-        if self.schema_url is not None:
-            self._validate_rpc_url()
-            schema = {"$ref": self.schema_url}
-        else:
-            schema = self.openrpc_schema()
-
-        return {"name": "OpenRPC Schema", "schema": schema}
-
     def openrpc_schema(self) -> ORPC.OpenRPC:
         """Implementation of OpenRPC specification.
 
         https://spec.open-rpc.org/
 
         """
         if not self.__openrpc_schema:
             openrpc: ORPC.OpenRPC = deepcopy(self.openrpc_schema_template)
+            if not isinstance(openrpc.get("methods"), list):
+                openrpc["methods"] = []
 
             for method_name, procedure_ in self.registry.items():
                 procedure = unwrap_func(procedure_)
                 try:
                     method_schema: MethodSchema = getattr(procedure, RPC_SCHEMA)
                 except AttributeError:
-                    break
+                    continue
 
-                method = ORPC.Method(
-                    name=method_name,
-                    params=[],
-                    result={},
-                    deprecated=method_schema.get("deprecated", False),
+                openrpc["methods"].append(
+                    ORPC.method_by_schema(
+                        method_schema,
+                        default_name=method_name,
+                    ),
                 )
-                if "short_description" in method_schema:
-                    method["summary"] = method_schema["short_description"]
-                if "description" in method_schema:
-                    method["description"] = method_schema["description"]
-
-                # Fill parameters schema
-                parameters = method_schema.get("parameters", {})
-                for param_name, parameter in parameters.items():
-                    cd_param = ORPC.ContentDescriptor(
-                        name=parameter.get("name", param_name),
-                        schema=ORPC.Schema(),
-                        required=parameter.get("required", False),
-                        deprecated=parameter.get("deprecated", False),
-                    )
-                    if "type" in parameter:
-                        cd_param["schema"]["type"] = ORPC.type_mapping(
-                            parameter["type"],
-                        )
-                    if "default" in parameter:
-                        cd_param["schema"]["default"] = parameter["default"]
-                    if "description" in parameter:
-                        cd_param["summary"] = parameter["description"]
-                        cd_param["description"] = parameter["description"]
-
-                    method["params"].append(cd_param)
-
-                # Fill result schema
-                if "result" in method_schema:
-                    result_schema = method_schema["result"]
-                    cd_result = ORPC.ContentDescriptor(
-                        name=result_schema.get("name", "result"),
-                        schema=ORPC.Schema(),
-                    )
-                    if "type" in result_schema:
-                        cd_result["schema"]["type"] = ORPC.type_mapping(
-                            result_schema.get("type"),
-                        )
-                    if "description" in result_schema:
-                        cd_result["summary"] = result_schema["description"]
-                        cd_result["description"] = result_schema["description"]
-
-                    method["result"] = cd_result
-
-                openrpc["methods"].append(method)
 
             self.__openrpc_schema = openrpc
         return self.__openrpc_schema
 
     def openapi_schema(self) -> dict:
         """Implementation of OpenAPI specification.
 
@@ -487,126 +432,40 @@
             openapi: OAPI.OpenAPI = deepcopy(self.openapi_schema_template)
 
             for method_name, procedure_ in self.registry.items():
                 procedure = unwrap_func(procedure_)
                 try:
                     method_schema: MethodSchema = getattr(procedure, RPC_SCHEMA)
                 except AttributeError:
-                    break
+                    continue
 
                 path_name = self.schema_url + "#" + method_name
-                operation = OAPI.Operation(
-                    operationId=method_name,
-                    parameters=[],
-                    deprecated=method_schema.get("deprecated", False),
-                )
-                if "short_description" in method_schema:
-                    operation["summary"] = method_schema["short_description"]
-                if "description" in method_schema:
-                    operation["description"] = method_schema["description"]
-
-                # Fill request body
-                parameters = method_schema.get("parameters", {}).items()
-                media = OAPI.MediaType(
-                    schema=OAPI.Schema(
-                        type="object",
-                        properties={
-                            "jsonrpc": {
-                                "type": "string",
-                                "description": "Protocol version",
-                            },
-                            "method": {
-                                "type": "string",
-                                "description": "Procedure (method) name",
-                            },
-                            "params": {
-                                "type": "object",
-                                "properties": {
-                                    param_name: {
-                                        "default": parameter.get("default", ""),
-                                        "description": parameter.get(
-                                            "description",
-                                            "",
-                                        ),
-                                        "deprecated": parameter.get(
-                                            "deprecated",
-                                            False,
-                                        ),
-                                    }
-                                    for param_name, parameter in parameters
-                                },
-                            },
-                            "id": {
-                                "type": "string",
-                            },
-                        },
-                        required=["jsonrpc", "method"],
-                    ),
-                )
-                if "example" in method_schema:
-                    media["example"] = method_schema["example"]
-                if "examples" in method_schema:
-                    media["examples"] = method_schema["examples"]
-                operation["requestBody"] = OAPI.RequestBody(
-                    content={"application/json": media},
-                    description="JSON-RPC 2.0 Request Object",
-                    required=True,
-                )
-
-                # Fill result schema
-                if "result" in method_schema:
-                    result_schema = method_schema["result"]
-
-                    media = OAPI.MediaType(
-                        schema=OAPI.Schema(
-                            type="object",
-                            properties=dict(
-                                jsonrpc=dict(type="string", default="2.0"),
-                                result=dict(),
-                                id=dict(type="string"),
-                            ),
-                        ),
-                    )
-                    if "type" in result_schema:
-                        media["schema"]["type"] = OAPI.type_mapping(
-                            result_schema.get("type"),
-                        )
-                    if "description" in result_schema:
-                        media["schema"]["description"] = result_schema[
-                            "description"
-                        ]
-                    if "example" in result_schema:
-                        media["example"] = result_schema["example"]
-                    if "examples" in result_schema:
-                        media["examples"] = result_schema["examples"]
-                else:
-                    # If returns type is NoneType
-                    media = OAPI.MediaType(
-                        schema=OAPI.Schema(
-                            type="object",
-                            properties=dict(
-                                jsonrpc=dict(type="string", default="2.0"),
-                                result=dict(type="null"),
-                                id=dict(type="string"),
-                            ),
-                        ),
-                    )
-                operation["responses"] = OAPI.Responses(
-                    **{
-                        "200": OAPI.Response(
-                            description="JSON-RPC 2.0 Response Object",
-                            content={"application/json": media},
-                        ),
-                    },
+                operation = OAPI.operation_by_schema(
+                    method_schema,
+                    default_name=method_name,
                 )
-
                 openapi["paths"][path_name] = OAPI.PathItem(post=operation)
 
             self.__openapi_schema = openapi
         return self.__openapi_schema
 
     def _validate_rpc_url(self):
         assert bool(self.schema_url), (
             "To use service description schemes, "
             "you must specify the URL responsible for processing "
             "RPC requests."
         )
+
+
+def rpc_discover(protocol: JsonRPCv2) -> dict[str, Any]:
+    """Returns an OpenRPC schema as a description of this service.
+
+    :return: OpenRPC Schema.
+
+    """
+    if protocol.schema_url is not None:
+        protocol._validate_rpc_url()  # noqa
+        schema = {"$ref": protocol.schema_url}
+    else:
+        schema = protocol.openrpc_schema()
+
+    return schema
```

### Comparing `drakaina-0.7.0b4/drakaina/serializers.py` & `drakaina-0.7.0b6/drakaina/serializers.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/drakaina/utils.py` & `drakaina-0.7.0b6/drakaina/utils.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/drakaina/wsgi.py` & `drakaina-0.7.0b6/drakaina/wsgi.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/LICENSE` & `drakaina-0.7.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b4/pyproject.toml` & `drakaina-0.7.0b6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drakaina"
-version = "0.7.0-beta.4"
+version = "0.7.0-beta.6"
 description = "Module for simple RPC service implementation"
 authors = ["Aleksey Terentyev <terentyev.a@pm.me>"]
 license = "Apache License 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
@@ -49,19 +49,21 @@
 pytest = "^7.3.1"
 ujson = "^5.7.0"
 pyjwt = "^2.7.0"
 django = ">=3.2"
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.2.1"
+pytest-cov = "^4.1.0"
 httpx = "^0.23.3"
 
 [tool.pytest.ini_options]
 cache_dir = ".pytest_cache"
 testpaths = "tests"
+addopts = "-vl --cov=drakaina --tb=auto --capture=sys"
 
 [tool.ruff]
 # Enable Pyflakes `E` and `F` codes by default.
 select = ["E", "F"]
 ignore = []
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
```

### Comparing `drakaina-0.7.0b4/README.md` & `drakaina-0.7.0b6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 ![Drakaina](content/drakaina.png "Drakaina"){width=200px height=205px}
 
 [![image](https://img.shields.io/pypi/v/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![image](https://img.shields.io/pypi/l/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![image](https://img.shields.io/pypi/pyversions/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
+[![OpenRPC](https://img.shields.io/endpoint?url=https%3A%2F%2Fgitlab.com%2Ftau_lex%2Fdrakaina%2F-%2Fraw%2Fmain%2Fcontent%2Fopenrpc-badge.json)](https://open-rpc.org)
 [![libera manifesto](https://img.shields.io/badge/libera-manifesto-lightgrey.svg)](https://liberamanifesto.com)
 
 ❗ WIP ❗
 
 Framework for simple RPC service implementation.
 
 
 ## Quickstart
 
-Drakaina may be installed via `pip` and requires Python 3.7 or higher :
+Drakaina may be installed via `pip` and requires Python 3.8 or higher :
 
 ```shell
 pip install drakaina
 ```
 
 A minimal Drakaina example is:
```

### Comparing `drakaina-0.7.0b4/PKG-INFO` & `drakaina-0.7.0b6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drakaina
-Version: 0.7.0b4
+Version: 0.7.0b6
 Summary: Module for simple RPC service implementation
 Home-page: https://gitlab.com/tau_lex/drakaina
 License: Apache-2.0
 Keywords: rpc,jsonrpc,openrpc
 Author: Aleksey Terentyev
 Author-email: terentyev.a@pm.me
 Requires-Python: >=3.8,<4.0
@@ -14,15 +14,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Provides-Extra: docs
 Provides-Extra: jwt
 Provides-Extra: msgpack
 Provides-Extra: orjson
@@ -42,24 +41,25 @@
 ![Drakaina](content/drakaina.png "Drakaina"){width=200px height=205px}
 
 [![image](https://img.shields.io/pypi/v/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![image](https://img.shields.io/pypi/l/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![image](https://img.shields.io/pypi/pyversions/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
+[![OpenRPC](https://img.shields.io/endpoint?url=https%3A%2F%2Fgitlab.com%2Ftau_lex%2Fdrakaina%2F-%2Fraw%2Fmain%2Fcontent%2Fopenrpc-badge.json)](https://open-rpc.org)
 [![libera manifesto](https://img.shields.io/badge/libera-manifesto-lightgrey.svg)](https://liberamanifesto.com)
 
 ❗ WIP ❗
 
 Framework for simple RPC service implementation.
 
 
 ## Quickstart
 
-Drakaina may be installed via `pip` and requires Python 3.7 or higher :
+Drakaina may be installed via `pip` and requires Python 3.8 or higher :
 
 ```shell
 pip install drakaina
 ```
 
 A minimal Drakaina example is:
```

