# Comparing `tmp/pocketbase-0.8.1.tar.gz` & `tmp/pocketbase-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketbase-0.8.1.tar", max compression
+gzip compressed data, was "pocketbase-0.8.2.tar", max compression
```

## Comparing `pocketbase-0.8.1.tar` & `pocketbase-0.8.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     2253 2023-04-27 00:23:48.651889 pocketbase-0.8.1/README.md
--rw-r--r--   0        0        0      304 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/__init__.py
--rw-r--r--   0        0        0     4763 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/client.py
--rw-r--r--   0        0        0      199 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/__init__.py
--rw-r--r--   0        0        0      363 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/admin.py
--rw-r--r--   0        0        0     1296 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/collection.py
--rw-r--r--   0        0        0      486 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/external_auth.py
--rw-r--r--   0        0        0      390 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/file_upload.py
--rw-r--r--   0        0        0      767 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/log_request.py
--rw-r--r--   0        0        0      797 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/record.py
--rw-r--r--   0        0        0      108 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/utils/__init__.py
--rw-r--r--   0        0        0      880 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/utils/base_model.py
--rw-r--r--   0        0        0      313 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/utils/list_result.py
--rw-r--r--   0        0        0      293 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/utils/schema_field.py
--rw-r--r--   0        0        0      292 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/__init__.py
--rw-r--r--   0        0        0     4906 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/admin_service.py
--rw-r--r--   0        0        0     1118 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/collection_service.py
--rw-r--r--   0        0        0     2048 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/log_service.py
--rw-r--r--   0        0        0     5186 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/realtime_service.py
--rw-r--r--   0        0        0     9534 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/record_service.py
--rw-r--r--   0        0        0     1517 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/settings_service.py
--rw-r--r--   0        0        0      123 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/utils/__init__.py
--rw-r--r--   0        0        0     3460 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/utils/base_crud_service.py
--rw-r--r--   0        0        0      178 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/utils/base_service.py
--rw-r--r--   0        0        0     1941 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/utils/crud_service.py
--rw-r--r--   0        0        0     4032 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/utils/sse.py
--rw-r--r--   0        0        0       88 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/stores/__init__.py
--rw-r--r--   0        0        0     1278 2023-04-27 00:23:48.655889 pocketbase-0.8.1/pocketbase/stores/base_auth_store.py
--rw-r--r--   0        0        0     1785 2023-04-27 00:23:48.655889 pocketbase-0.8.1/pocketbase/stores/local_auth_store.py
--rw-r--r--   0        0        0     1011 2023-04-27 00:23:48.655889 pocketbase-0.8.1/pocketbase/utils.py
--rw-r--r--   0        0        0     1605 2023-04-27 00:23:48.655889 pocketbase-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 pocketbase-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      321 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/__init__.py
+-rw-r--r--   0        0        0     4973 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/client.py
+-rw-r--r--   0        0        0      205 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/models/__init__.py
+-rw-r--r--   0        0        0      379 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/models/admin.py
+-rw-r--r--   0        0        0     1342 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/models/collection.py
+-rw-r--r--   0        0        0      503 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/models/external_auth.py
+-rw-r--r--   0        0        0      404 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/models/file_upload.py
+-rw-r--r--   0        0        0      794 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/models/log_request.py
+-rw-r--r--   0        0        0      737 2023-06-02 12:35:50.426099 pocketbase-0.8.2/pocketbase/models/record.py
+-rw-r--r--   0        0        0      111 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/models/utils/__init__.py
+-rw-r--r--   0        0        0      913 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/models/utils/base_model.py
+-rw-r--r--   0        0        0      327 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/models/utils/list_result.py
+-rw-r--r--   0        0        0      307 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/models/utils/schema_field.py
+-rw-r--r--   0        0        0      298 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/services/__init__.py
+-rw-r--r--   0        0        0     5049 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/services/admin_service.py
+-rw-r--r--   0        0        0     1154 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/services/collection_service.py
+-rw-r--r--   0        0        0     2108 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/services/log_service.py
+-rw-r--r--   0        0        0     5337 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/services/realtime_service.py
+-rw-r--r--   0        0        0     9809 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/services/record_service.py
+-rw-r--r--   0        0        0     1569 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/services/settings_service.py
+-rw-r--r--   0        0        0      126 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/services/utils/__init__.py
+-rw-r--r--   0        0        0     3560 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/services/utils/base_crud_service.py
+-rw-r--r--   0        0        0      187 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/services/utils/base_service.py
+-rw-r--r--   0        0        0     1992 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/services/utils/crud_service.py
+-rw-r--r--   0        0        0     4171 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/services/utils/sse.py
+-rw-r--r--   0        0        0       90 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/stores/__init__.py
+-rw-r--r--   0        0        0     1322 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/stores/base_auth_store.py
+-rw-r--r--   0        0        0     1846 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/stores/local_auth_store.py
+-rw-r--r--   0        0        0     1047 2023-05-20 14:02:20.608038 pocketbase-0.8.2/pocketbase/utils.py
+-rw-r--r--   0        0        0     1659 2023-06-02 12:36:43.594811 pocketbase-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     2339 2023-05-20 14:02:20.608038 pocketbase-0.8.2/README.md
+-rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 pocketbase-0.8.2/PKG-INFO
```

### Comparing `pocketbase-0.8.1/README.md` & `pocketbase-0.8.2/README.md`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-# PocketBase Python SDK
-
-[![Tests](https://github.com/vaphes/pocketbase/actions/workflows/tests.yml/badge.svg)](https://github.com/vaphes/pocketbase/actions/workflows/tests.yml)
-
-Python client SDK for the <a href="https://pocketbase.io/">PocketBase</a> backend.
-
-This is in early development, and at first is just a translation of <a href="https://github.com/pocketbase/js-sdk">the javascript lib</a> using <a href="https://github.com/encode/httpx/">HTTPX</a>.
-
----
-
-## Installation
-
-Install PocketBase using PIP:
-
-```shell
-python3 -m pip install pocketbase
-```
-
-## Usage
-
-The rule of thumb here is just to use it as you would <a href="https://github.com/pocketbase/js-sdk">the javascript lib</a>, but in a pythonic way of course!
-
-```python
-from pocketbase import PocketBase  # Client also works the same
-from pocketbase.client import FileUpload
-
-client = PocketBase('http://127.0.0.1:8090')
-
-# authenticate as regular user
-user_data = client.collection("users").auth_with_password(
-    "user@example.com", "0123456789")
-
-# or as admin
-admin_data = client.admins.auth_with_password("test@example.com", "0123456789")
-
-# list and filter "example" collection records
-result = client.collection("example").get_list(
-    1, 20, {"filter": 'status = true && created > "2022-08-01 10:00:00"'})
-
-# create record and upload file to image field
-result = client.collection("example").create(
-    {
-        "status": "true",
-        "image": FileUpload(("image.png", open("image.png", "rb"))),
-    })
-
-# and much more...
-```
-> More detailed API docs and copy-paste examples could be found in the [API documentation for each service](https://pocketbase.io/docs/api-authentication). Just remember to 'pythonize it' 🙃.
-
-## Development
-
-These are the requirements for local development:
-
-* Python 3.7+
-* Poetry (https://python-poetry.org/)
-
-You can install locally:
-
-```shell
-poetry install
-```
-
-Or can build and generate a package:
-
-```shell
-poetry build
-```
-
-But if you are using only PIP, use this command:
-
-```shell
-python3 -m pip install -e .
-```
-
-## Tests
-
-To execute the tests use this command:
-
-```
-poetry run pytest
-```
-
-## License
-
-The PocketBase Python SDK is <a href="https://github.com/vaphes/pocketbase/blob/master/LICENCE.txt">MIT licensed</a> code.
+# PocketBase Python SDK
+
+[![Tests](https://github.com/vaphes/pocketbase/actions/workflows/tests.yml/badge.svg)](https://github.com/vaphes/pocketbase/actions/workflows/tests.yml)
+
+Python client SDK for the <a href="https://pocketbase.io/">PocketBase</a> backend.
+
+This is in early development, and at first is just a translation of <a href="https://github.com/pocketbase/js-sdk">the javascript lib</a> using <a href="https://github.com/encode/httpx/">HTTPX</a>.
+
+---
+
+## Installation
+
+Install PocketBase using PIP:
+
+```shell
+python3 -m pip install pocketbase
+```
+
+## Usage
+
+The rule of thumb here is just to use it as you would <a href="https://github.com/pocketbase/js-sdk">the javascript lib</a>, but in a pythonic way of course!
+
+```python
+from pocketbase import PocketBase  # Client also works the same
+from pocketbase.client import FileUpload
+
+client = PocketBase('http://127.0.0.1:8090')
+
+# authenticate as regular user
+user_data = client.collection("users").auth_with_password(
+    "user@example.com", "0123456789")
+
+# or as admin
+admin_data = client.admins.auth_with_password("test@example.com", "0123456789")
+
+# list and filter "example" collection records
+result = client.collection("example").get_list(
+    1, 20, {"filter": 'status = true && created > "2022-08-01 10:00:00"'})
+
+# create record and upload file to image field
+result = client.collection("example").create(
+    {
+        "status": "true",
+        "image": FileUpload(("image.png", open("image.png", "rb"))),
+    })
+
+# and much more...
+```
+> More detailed API docs and copy-paste examples could be found in the [API documentation for each service](https://pocketbase.io/docs/api-authentication). Just remember to 'pythonize it' 🙃.
+
+## Development
+
+These are the requirements for local development:
+
+* Python 3.7+
+* Poetry (https://python-poetry.org/)
+
+You can install locally:
+
+```shell
+poetry install
+```
+
+Or can build and generate a package:
+
+```shell
+poetry build
+```
+
+But if you are using only PIP, use this command:
+
+```shell
+python3 -m pip install -e .
+```
+
+## Tests
+
+To execute the tests use this command:
+
+```
+poetry run pytest
+```
+
+## License
+
+The PocketBase Python SDK is <a href="https://github.com/vaphes/pocketbase/blob/master/LICENCE.txt">MIT licensed</a> code.
```

### Comparing `pocketbase-0.8.1/pocketbase/client.py` & `pocketbase-0.8.2/pocketbase/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,138 +1,140 @@
-from __future__ import annotations
-
-from typing import Any, Dict
-from urllib.parse import quote, urlencode
-
-import httpx
-
-from pocketbase.models import FileUpload
-from pocketbase.models.record import Record
-from pocketbase.services.admin_service import AdminService
-from pocketbase.services.collection_service import CollectionService
-from pocketbase.services.log_service import LogService
-from pocketbase.services.realtime_service import RealtimeService
-from pocketbase.services.record_service import RecordService
-from pocketbase.services.settings_service import SettingsService
-from pocketbase.stores.base_auth_store import BaseAuthStore
-from pocketbase.utils import ClientResponseError
-
-
-class Client:
-    base_url: str
-    lang: str
-    auth_store: BaseAuthStore
-    settings: SettingsService
-    admins: AdminService
-    records: Record
-    collections: CollectionService
-    records: RecordService
-    logs: LogService
-    realtime: RealtimeService
-    record_service: Dict[str, RecordService]
-
-    def __init__(
-        self,
-        base_url: str = "/",
-        lang: str = "en-US",
-        auth_store: BaseAuthStore | None = None,
-    ) -> None:
-        self.base_url = base_url
-        self.lang = lang
-        self.auth_store = auth_store or BaseAuthStore()  # LocalAuthStore()
-        # services
-        self.admins = AdminService(self)
-        self.collections = CollectionService(self)
-        self.logs = LogService(self)
-        self.settings = SettingsService(self)
-        self.realtime = RealtimeService(self)
-        self.record_service = {}
-
-    def collection(self, id_or_name: str) -> RecordService:
-        """Returns the RecordService associated to the specified collection."""
-        if id_or_name not in self.record_service:
-            self.record_service[id_or_name] = RecordService(self, id_or_name)
-        return self.record_service[id_or_name]
-
-    def send(self, path: str, req_config: dict[str:Any]) -> Any:
-        """Sends an api http request."""
-        config = {"method": "GET"}
-        config.update(req_config)
-        # check if Authorization header can be added
-        if self.auth_store.token and (
-            "headers" not in config or "Authorization" not in config["headers"]
-        ):
-            config["headers"] = config.get("headers", {})
-            config["headers"].update({"Authorization": self.auth_store.token})
-        # build url + path
-        url = self.build_url(path)
-        # send the request
-        method = config.get("method", "GET")
-        params = config.get("params", None)
-        headers = config.get("headers", None)
-        body = config.get("body", None)
-        # handle requests including files as multipart:
-        data = {}
-        files = ()
-        for k, v in (body if isinstance(body, dict) else {}).items():
-            if isinstance(v, FileUpload):
-                files += v.get(k)
-            else:
-                data[k] = v
-        if len(files) > 0:
-            # discard body, switch to multipart encoding
-            body = None
-        else:
-            # discard files+data (do not use multipart encoding)
-            files = None
-            data = None
-        try:
-            response = httpx.request(
-                method=method,
-                url=url,
-                params=params,
-                headers=headers,
-                json=body,
-                data=data,
-                files=files,
-                timeout=120,
-            )
-        except Exception as e:
-            raise ClientResponseError(
-                f"General request error. Original error: {e}",
-                original_error=e,
-            )
-        try:
-            data = response.json()
-        except Exception:
-            data = None
-        if response.status_code >= 400:
-            raise ClientResponseError(
-                f"Response error. Status code:{response.status_code}",
-                url=response.url,
-                status=response.status_code,
-                data=data,
-            )
-        return data
-
-    def get_file_url(self, record: Record, filename: str, query_params: dict):
-        parts = [
-            "api",
-            "files",
-            quote(record.collection_id or record.collection_name),
-            quote(record.id),
-            quote(filename),
-        ]
-        result = self.build_url("/".join(parts))
-        if len(query_params) != 0:
-            params: str = urlencode(query_params)
-            result += "&" if "?" in result else "?"
-            result += params
-        return result
-
-    def build_url(self, path: str) -> str:
-        url = self.base_url
-        if not self.base_url.endswith("/"):
-            url += "/"
-        if path.startswith("/"):
-            path = path[1:]
-        return url + path
+from __future__ import annotations
+
+from typing import Any, Dict
+from urllib.parse import quote, urlencode
+
+import httpx
+
+from pocketbase.models import FileUpload
+from pocketbase.models.record import Record
+from pocketbase.services.admin_service import AdminService
+from pocketbase.services.collection_service import CollectionService
+from pocketbase.services.log_service import LogService
+from pocketbase.services.realtime_service import RealtimeService
+from pocketbase.services.record_service import RecordService
+from pocketbase.services.settings_service import SettingsService
+from pocketbase.stores.base_auth_store import BaseAuthStore
+from pocketbase.utils import ClientResponseError
+
+
+class Client:
+    base_url: str
+    lang: str
+    auth_store: BaseAuthStore
+    settings: SettingsService
+    admins: AdminService
+    records: Record
+    collections: CollectionService
+    records: RecordService
+    logs: LogService
+    realtime: RealtimeService
+    record_service: Dict[str, RecordService]
+
+    def __init__(
+        self,
+        base_url: str = "/",
+        lang: str = "en-US",
+        auth_store: BaseAuthStore | None = None,
+        timeout: float = 120,
+    ) -> None:
+        self.base_url = base_url
+        self.lang = lang
+        self.auth_store = auth_store or BaseAuthStore()  # LocalAuthStore()
+        self.timeout = timeout
+        # services
+        self.admins = AdminService(self)
+        self.collections = CollectionService(self)
+        self.logs = LogService(self)
+        self.settings = SettingsService(self)
+        self.realtime = RealtimeService(self)
+        self.record_service = {}
+
+    def collection(self, id_or_name: str) -> RecordService:
+        """Returns the RecordService associated to the specified collection."""
+        if id_or_name not in self.record_service:
+            self.record_service[id_or_name] = RecordService(self, id_or_name)
+        return self.record_service[id_or_name]
+
+    def send(self, path: str, req_config: dict[str:Any]) -> Any:
+        """Sends an api http request."""
+        config = {"method": "GET"}
+        config.update(req_config)
+        # check if Authorization header can be added
+        if self.auth_store.token and (
+            "headers" not in config or "Authorization" not in config["headers"]
+        ):
+            config["headers"] = config.get("headers", {})
+            config["headers"].update({"Authorization": self.auth_store.token})
+        # build url + path
+        url = self.build_url(path)
+        # send the request
+        method = config.get("method", "GET")
+        params = config.get("params", None)
+        headers = config.get("headers", None)
+        body = config.get("body", None)
+        # handle requests including files as multipart:
+        data = {}
+        files = ()
+        for k, v in (body if isinstance(body, dict) else {}).items():
+            if isinstance(v, FileUpload):
+                files += v.get(k)
+            else:
+                data[k] = v
+        if len(files) > 0:
+            # discard body, switch to multipart encoding
+            body = None
+        else:
+            # discard files+data (do not use multipart encoding)
+            files = None
+            data = None
+        try:
+            response = httpx.request(
+                method=method,
+                url=url,
+                params=params,
+                headers=headers,
+                json=body,
+                data=data,
+                files=files,
+                timeout=self.timeout,
+            )
+        except Exception as e:
+            raise ClientResponseError(
+                f"General request error. Original error: {e}",
+                original_error=e,
+            )
+        try:
+            data = response.json()
+        except Exception:
+            data = None
+        if response.status_code >= 400:
+            raise ClientResponseError(
+                f"Response error. Status code:{response.status_code}",
+                url=response.url,
+                status=response.status_code,
+                data=data,
+            )
+        return data
+
+    def get_file_url(self, record: Record, filename: str, query_params: dict):
+        parts = [
+            "api",
+            "files",
+            quote(record.collection_id or record.collection_name),
+            quote(record.id),
+            quote(filename),
+        ]
+        result = self.build_url("/".join(parts))
+        if len(query_params) != 0:
+            params: str = urlencode(query_params)
+            result += "&" if "?" in result else "?"
+            result += params
+        return result
+
+    def build_url(self, path: str) -> str:
+        url = self.base_url
+        if not self.base_url.endswith("/"):
+            url += "/"
+        if path.startswith("/"):
+            path = path[1:]
+        return url + path
```

### Comparing `pocketbase-0.8.1/pocketbase/models/utils/base_model.py` & `pocketbase-0.8.2/pocketbase/models/utils/base_model.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from __future__ import annotations
-
-from abc import ABC
-import datetime
-
-from pocketbase.utils import to_datetime
-
-
-class BaseModel(ABC):
-    id: str
-    created: str | datetime.datetime
-    updated: str | datetime.datetime
-
-    def __init__(self, data: dict = {}) -> None:
-        super().__init__()
-        self.load(data)
-
-    def __str__(self) -> str:
-        return f"<{self.__class__.__name__}: {self.id}>"
-
-    def __repr__(self) -> str:
-        return self.__str__()
-
-    def load(self, data: dict) -> None:
-        """Loads `data` into the current model."""
-        self.id = data.pop("id", "")
-        self.created = to_datetime(data.pop("created", ""))
-        self.updated = to_datetime(data.pop("updated", ""))
-
-    @property
-    def is_new(self) -> bool:
-        """Returns whether the current loaded data represent a stored db record."""
-        return not self.id
+from __future__ import annotations
+
+from abc import ABC
+import datetime
+
+from pocketbase.utils import to_datetime
+
+
+class BaseModel(ABC):
+    id: str
+    created: str | datetime.datetime
+    updated: str | datetime.datetime
+
+    def __init__(self, data: dict = {}) -> None:
+        super().__init__()
+        self.load(data)
+
+    def __str__(self) -> str:
+        return f"<{self.__class__.__name__}: {self.id}>"
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
+    def load(self, data: dict) -> None:
+        """Loads `data` into the current model."""
+        self.id = data.pop("id", "")
+        self.created = to_datetime(data.pop("created", ""))
+        self.updated = to_datetime(data.pop("updated", ""))
+
+    @property
+    def is_new(self) -> bool:
+        """Returns whether the current loaded data represent a stored db record."""
+        return not self.id
```

### Comparing `pocketbase-0.8.1/pocketbase/services/admin_service.py` & `pocketbase-0.8.2/pocketbase/services/admin_service.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-from __future__ import annotations
-
-from pocketbase.models.utils.base_model import BaseModel
-from pocketbase.services.utils.crud_service import CrudService
-from pocketbase.models.admin import Admin
-
-
-class AdminAuthResponse:
-    token: str
-    admin: Admin
-
-    def __init__(self, token: str, admin: Admin, **kwargs) -> None:
-        self.token = token
-        self.admin = admin
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-
-
-class AdminService(CrudService):
-    def decode(self, data: dict) -> BaseModel:
-        return Admin(data)
-
-    def base_crud_path(self) -> str:
-        return "/api/admins"
-
-    def update(self, id: str, body_params: dict, query_params: dict) -> BaseModel:
-        """
-        If the current `client.auth_store.model` matches with the updated id,
-        then on success the `client.auth_store.model` will be updated with the result.
-        """
-        item = super(AdminService).update(id, body_params)
-        try:
-            if (
-                self.client.auth_store.model.collection_id is not None
-                and item.id == self.client.auth_store.model.id
-            ):
-                self.client.auth_store.save(self.client.auth_store.token, item)
-        except:
-            pass
-        return item
-
-    def delete(self, id: str, body_params: dict, query_params: dict) -> BaseModel:
-        """
-        If the current `client.auth_store.model` matches with the deleted id,
-        then on success the `client.auth_store` will be cleared.
-        """
-        item = super(AdminService).delete(id, body_params)
-        try:
-            if (
-                self.client.auth_store.model.collection_id is not None
-                and item.id == self.client.auth_store.model.id
-            ):
-                self.client.auth_store.save(self.client.auth_store.token, item)
-        except:
-            pass
-        return item
-
-    def auth_response(self, response_data: dict) -> AdminAuthResponse:
-        """Prepare successful authorize response."""
-        admin = self.decode(response_data.pop("admin", {}))
-        token = response_data.pop("token", "")
-        if token and admin:
-            self.client.auth_store.save(token, admin)
-        return AdminAuthResponse(token=token, admin=admin, **response_data)
-
-    def auth_with_password(
-        self, email: str, password: str, body_params: dict = {}, query_params: dict = {}
-    ) -> AdminAuthResponse:
-        """
-        Authenticate an admin account with its email and password
-        and returns a new admin token and data.
-
-        On success this method automatically updates the client's AuthStore data.
-        """
-        body_params.update({"identity": email, "password": password})
-        response_data = self.client.send(
-            self.base_crud_path() + "/auth-with-password",
-            {
-                "method": "POST",
-                "params": query_params,
-                "body": body_params,
-                "headers": {"Authorization": ""},
-            },
-        )
-        return self.auth_response(response_data)
-
-    def authRefresh(
-        self, body_params: dict = {}, query_params: dict = {}
-    ) -> AdminAuthResponse:
-        """
-        Refreshes the current admin authenticated instance and
-        returns a new token and admin data.
-
-        On success this method automatically updates the client's AuthStore data.
-        """
-        return self.auth_response(
-            self.client.send(
-                self.base_crud_path() + "/auth-refresh",
-                {"method": "POST", "params": query_params, "body": body_params},
-            )
-        )
-
-    def requestPasswordReset(
-        self, email: str, body_params: dict = {}, query_params: dict = {}
-    ) -> bool:
-        """Sends admin password reset request."""
-        body_params.update({"email": email})
-        self.client.send(
-            self.base_crud_path() + "/request-password-reset",
-            {
-                "method": "POST",
-                "params": query_params,
-                "body": body_params,
-            },
-        )
-        return True
-
-    def confirmPasswordReset(
-        self,
-        password_reset_token: str,
-        password: str,
-        password_confirm: str,
-        body_params: dict = {},
-        query_params: dict = {},
-    ) -> AdminAuthResponse:
-        """Confirms admin password reset request."""
-        body_params.update(
-            {
-                "token": password_reset_token,
-                "password": password,
-                "passwordConfirm": password_confirm,
-            }
-        )
-        return self.auth_response(
-            self.client.send(
-                self.base_crud_path() + "/confirm-password-reset",
-                {
-                    "method": "POST",
-                    "params": query_params,
-                    "body": body_params,
-                },
-            )
-        )
+from __future__ import annotations
+
+from pocketbase.models.utils.base_model import BaseModel
+from pocketbase.services.utils.crud_service import CrudService
+from pocketbase.models.admin import Admin
+
+
+class AdminAuthResponse:
+    token: str
+    admin: Admin
+
+    def __init__(self, token: str, admin: Admin, **kwargs) -> None:
+        self.token = token
+        self.admin = admin
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
+
+class AdminService(CrudService):
+    def decode(self, data: dict) -> BaseModel:
+        return Admin(data)
+
+    def base_crud_path(self) -> str:
+        return "/api/admins"
+
+    def update(self, id: str, body_params: dict, query_params: dict) -> BaseModel:
+        """
+        If the current `client.auth_store.model` matches with the updated id,
+        then on success the `client.auth_store.model` will be updated with the result.
+        """
+        item = super(AdminService).update(id, body_params)
+        try:
+            if (
+                self.client.auth_store.model.collection_id is not None
+                and item.id == self.client.auth_store.model.id
+            ):
+                self.client.auth_store.save(self.client.auth_store.token, item)
+        except:
+            pass
+        return item
+
+    def delete(self, id: str, body_params: dict, query_params: dict) -> BaseModel:
+        """
+        If the current `client.auth_store.model` matches with the deleted id,
+        then on success the `client.auth_store` will be cleared.
+        """
+        item = super(AdminService).delete(id, body_params)
+        try:
+            if (
+                self.client.auth_store.model.collection_id is not None
+                and item.id == self.client.auth_store.model.id
+            ):
+                self.client.auth_store.save(self.client.auth_store.token, item)
+        except:
+            pass
+        return item
+
+    def auth_response(self, response_data: dict) -> AdminAuthResponse:
+        """Prepare successful authorize response."""
+        admin = self.decode(response_data.pop("admin", {}))
+        token = response_data.pop("token", "")
+        if token and admin:
+            self.client.auth_store.save(token, admin)
+        return AdminAuthResponse(token=token, admin=admin, **response_data)
+
+    def auth_with_password(
+        self, email: str, password: str, body_params: dict = {}, query_params: dict = {}
+    ) -> AdminAuthResponse:
+        """
+        Authenticate an admin account with its email and password
+        and returns a new admin token and data.
+
+        On success this method automatically updates the client's AuthStore data.
+        """
+        body_params.update({"identity": email, "password": password})
+        response_data = self.client.send(
+            self.base_crud_path() + "/auth-with-password",
+            {
+                "method": "POST",
+                "params": query_params,
+                "body": body_params,
+                "headers": {"Authorization": ""},
+            },
+        )
+        return self.auth_response(response_data)
+
+    def authRefresh(
+        self, body_params: dict = {}, query_params: dict = {}
+    ) -> AdminAuthResponse:
+        """
+        Refreshes the current admin authenticated instance and
+        returns a new token and admin data.
+
+        On success this method automatically updates the client's AuthStore data.
+        """
+        return self.auth_response(
+            self.client.send(
+                self.base_crud_path() + "/auth-refresh",
+                {"method": "POST", "params": query_params, "body": body_params},
+            )
+        )
+
+    def requestPasswordReset(
+        self, email: str, body_params: dict = {}, query_params: dict = {}
+    ) -> bool:
+        """Sends admin password reset request."""
+        body_params.update({"email": email})
+        self.client.send(
+            self.base_crud_path() + "/request-password-reset",
+            {
+                "method": "POST",
+                "params": query_params,
+                "body": body_params,
+            },
+        )
+        return True
+
+    def confirmPasswordReset(
+        self,
+        password_reset_token: str,
+        password: str,
+        password_confirm: str,
+        body_params: dict = {},
+        query_params: dict = {},
+    ) -> AdminAuthResponse:
+        """Confirms admin password reset request."""
+        body_params.update(
+            {
+                "token": password_reset_token,
+                "password": password,
+                "passwordConfirm": password_confirm,
+            }
+        )
+        return self.auth_response(
+            self.client.send(
+                self.base_crud_path() + "/confirm-password-reset",
+                {
+                    "method": "POST",
+                    "params": query_params,
+                    "body": body_params,
+                },
+            )
+        )
```

### Comparing `pocketbase-0.8.1/pocketbase/services/collection_service.py` & `pocketbase-0.8.2/pocketbase/services/collection_service.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from __future__ import annotations
-
-from pocketbase.services.utils.crud_service import CrudService
-from pocketbase.models.utils.base_model import BaseModel
-from pocketbase.models.collection import Collection
-
-
-class CollectionService(CrudService):
-    def decode(self, data: dict) -> BaseModel:
-        return Collection(data)
-
-    def base_crud_path(self) -> str:
-        return "/api/collections"
-
-    def import_collections(
-        self,
-        collections: list,
-        delete_missing: bool = False,
-        query_params: dict = {},
-    ) -> bool:
-        """
-        Imports the provided collections.
-
-        If `delete_missing` is `True`, all local collections and schema fields,
-        that are not present in the imported configuration, WILL BE DELETED
-        (including their related records data)!
-        """
-        self.client.send(
-            self.base_crud_path() + "/import",
-            {
-                "method": "PUT",
-                "params": query_params,
-                "body": {"collections": collections, "deleteMissing": delete_missing},
-            },
-        )
-        return True
+from __future__ import annotations
+
+from pocketbase.services.utils.crud_service import CrudService
+from pocketbase.models.utils.base_model import BaseModel
+from pocketbase.models.collection import Collection
+
+
+class CollectionService(CrudService):
+    def decode(self, data: dict) -> BaseModel:
+        return Collection(data)
+
+    def base_crud_path(self) -> str:
+        return "/api/collections"
+
+    def import_collections(
+        self,
+        collections: list,
+        delete_missing: bool = False,
+        query_params: dict = {},
+    ) -> bool:
+        """
+        Imports the provided collections.
+
+        If `delete_missing` is `True`, all local collections and schema fields,
+        that are not present in the imported configuration, WILL BE DELETED
+        (including their related records data)!
+        """
+        self.client.send(
+            self.base_crud_path() + "/import",
+            {
+                "method": "PUT",
+                "params": query_params,
+                "body": {"collections": collections, "deleteMissing": delete_missing},
+            },
+        )
+        return True
```

### Comparing `pocketbase-0.8.1/pocketbase/services/log_service.py` & `pocketbase-0.8.2/pocketbase/services/log_service.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from __future__ import annotations
-
-from dataclasses import dataclass
-from typing import Union
-from urllib.parse import quote
-import datetime
-
-from pocketbase.services.utils.base_service import BaseService
-from pocketbase.models.utils.list_result import ListResult
-from pocketbase.models.log_request import LogRequest
-from pocketbase.utils import to_datetime
-
-
-@dataclass
-class HourlyStats:
-    total: int
-    date: Union[str, datetime.datetime]
-
-
-class LogService(BaseService):
-    def get_request_list(
-        self, page: int = 1, per_page: int = 30, query_params: dict = {}
-    ) -> ListResult:
-        """Returns paginated logged requests list."""
-        query_params.update({"page": page, "perPage": per_page})
-        response_data = self.client.send(
-            "/api/logs/requests",
-            {"method": "GET", "params": query_params},
-        )
-        items: list[LogRequest] = []
-        if "items" in response_data:
-            response_data["items"] = response_data["items"] or []
-            for item in response_data["items"]:
-                items.append(LogRequest(item))
-        return ListResult(
-            response_data.get("page", 1),
-            response_data.get("perPage", 0),
-            response_data.get("totalItems", 0),
-            response_data.get("totalPages", 0),
-            items,
-        )
-
-    def get_request(self, id: str, query_params: dict = {}) -> LogRequest:
-        """Returns a single logged request by its id."""
-        return LogRequest(
-            self.client.send(
-                "/api/logs/requests/" + quote(id),
-                {"method": "GET", "params": query_params},
-            )
-        )
-
-    def get_requests_stats(self, query_params: dict = {}) -> list[HourlyStats]:
-        """Returns request logs statistics."""
-        return [
-            HourlyStats(total=stat["total"], date=to_datetime(stat["date"]))
-            for stat in self.client.send(
-                "/api/logs/requests/stats",
-                {"method": "GET", "params": query_params},
-            )
-        ]
+from __future__ import annotations
+
+from dataclasses import dataclass
+from typing import Union
+from urllib.parse import quote
+import datetime
+
+from pocketbase.services.utils.base_service import BaseService
+from pocketbase.models.utils.list_result import ListResult
+from pocketbase.models.log_request import LogRequest
+from pocketbase.utils import to_datetime
+
+
+@dataclass
+class HourlyStats:
+    total: int
+    date: Union[str, datetime.datetime]
+
+
+class LogService(BaseService):
+    def get_request_list(
+        self, page: int = 1, per_page: int = 30, query_params: dict = {}
+    ) -> ListResult:
+        """Returns paginated logged requests list."""
+        query_params.update({"page": page, "perPage": per_page})
+        response_data = self.client.send(
+            "/api/logs/requests",
+            {"method": "GET", "params": query_params},
+        )
+        items: list[LogRequest] = []
+        if "items" in response_data:
+            response_data["items"] = response_data["items"] or []
+            for item in response_data["items"]:
+                items.append(LogRequest(item))
+        return ListResult(
+            response_data.get("page", 1),
+            response_data.get("perPage", 0),
+            response_data.get("totalItems", 0),
+            response_data.get("totalPages", 0),
+            items,
+        )
+
+    def get_request(self, id: str, query_params: dict = {}) -> LogRequest:
+        """Returns a single logged request by its id."""
+        return LogRequest(
+            self.client.send(
+                "/api/logs/requests/" + quote(id),
+                {"method": "GET", "params": query_params},
+            )
+        )
+
+    def get_requests_stats(self, query_params: dict = {}) -> list[HourlyStats]:
+        """Returns request logs statistics."""
+        return [
+            HourlyStats(total=stat["total"], date=to_datetime(stat["date"]))
+            for stat in self.client.send(
+                "/api/logs/requests/stats",
+                {"method": "GET", "params": query_params},
+            )
+        ]
```

### Comparing `pocketbase-0.8.1/pocketbase/services/realtime_service.py` & `pocketbase-0.8.2/pocketbase/services/realtime_service.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-from __future__ import annotations
-
-from typing import Callable, List
-import dataclasses
-import json
-
-from pocketbase.services.utils.base_service import BaseService
-from pocketbase.services.utils.sse import Event, SSEClient
-from pocketbase.models.record import Record
-
-
-@dataclasses.dataclass
-class MessageData:
-    action: str
-    record: Record
-
-
-class RealtimeService(BaseService):
-    subscriptions: dict
-    client_id: str = ""
-    event_source: SSEClient | None = None
-
-    def __init__(self, client) -> None:
-        super().__init__(client)
-        self.subscriptions = {}
-        self.client_id = ""
-        self.event_source = None
-
-    def subscribe(
-        self, subscription: str, callback: Callable[[MessageData], None]
-    ) -> None:
-        """Inits the sse connection (if not already) and register the subscription."""
-        # unsubscribe existing
-        if subscription in self.subscriptions and self.event_source:
-            self.event_source.remove_event_listener(subscription, callback)
-        # register subscription
-        self.subscriptions[subscription] = self._make_subscription(callback)
-        if not self.event_source:
-            self._connect()
-        elif self.client_id:
-            self._submit_subscriptions()
-
-    def unsubscribe_by_prefix(self, subscription_prefix: str):
-        """
-        Unsubscribe from all subscriptions starting with the provided prefix.
-
-        This method is no-op if there are no active subscriptions with the provided prefix.
-
-        The related sse connection will be autoclosed if after the
-        unsubscribe operation there are no active subscriptions left.
-        """
-        to_unsubscribe = []
-        for sub in self.subscriptions:
-            if sub.startswith(subscription_prefix):
-                to_unsubscribe.append(sub)
-        if len(to_unsubscribe) == 0:
-            return
-        return self.unsubscribe(*to_unsubscribe)
-
-    def unsubscribe(self, subscriptions: List[str] | None = None) -> None:
-        """
-        Unsubscribe from a subscription.
-
-        If the `subscriptions` argument is not set,
-        then the client will unsubscribe from all registered subscriptions.
-
-        The related sse connection will be autoclosed if after the
-        unsubscribe operations there are no active subscriptions left.
-        """
-        if not subscriptions or len(subscriptions) == 0:
-            # remove all subscriptions
-            self._remove_subscription_listeners()
-            self.subscriptions = {}
-        else:
-            # remove each passed subscription
-            found = False
-            for sub in self.subscriptions:
-                found = True
-                self.event_source.remove_event_listener(sub, self.subscriptions[sub])
-                self.subscriptions.pop(sub)
-            if not found:
-                return
-
-        if self.client_id:
-            self._submit_subscriptions()
-
-        # no more subscriptions -> close the sse connection
-        if not self.subscriptions:
-            self._disconnect()
-
-    def _make_subscription(
-        self, callback: Callable[[MessageData], None]
-    ) -> Callable[[Event], None]:
-        def listener(event: Event) -> None:
-            data = json.loads(event.data)
-            if "record" in data and "action" in data:
-                callback(
-                    MessageData(
-                        action=data["action"],
-                        record=Record(
-                            data=data["record"],
-                        ),
-                    )
-                )
-
-        return listener
-
-    def _submit_subscriptions(self) -> bool:
-        self._add_subscription_listeners()
-        self.client.send(
-            "/api/realtime",
-            {
-                "method": "POST",
-                "body": {
-                    "clientId": self.client_id,
-                    "subscriptions": list(self.subscriptions.keys()),
-                },
-            },
-        )
-        return True
-
-    def _add_subscription_listeners(self) -> None:
-        if not self.event_source:
-            return
-        self._remove_subscription_listeners()
-        for subscription, callback in self.subscriptions.items():
-            self.event_source.add_event_listener(subscription, callback)
-
-    def _remove_subscription_listeners(self) -> None:
-        if not self.event_source:
-            return
-        for subscription, callback in self.subscriptions.items():
-            self.event_source.remove_event_listener(subscription, callback)
-
-    def _connect_handler(self, event: Event) -> None:
-        self.client_id = event.id
-        self._submit_subscriptions()
-
-    def _connect(self) -> None:
-        self._disconnect()
-        self.event_source = SSEClient(self.client.build_url("/api/realtime"))
-        self.event_source.add_event_listener("PB_CONNECT", self._connect_handler)
-
-    def _disconnect(self) -> None:
-        self._remove_subscription_listeners()
-        self.client_id = ""
-        if not self.event_source:
-            return
-        self.event_source.remove_event_listener("PB_CONNECT", self._connect_handler)
-        self.event_source.close()
-        self.event_source = None
+from __future__ import annotations
+
+from typing import Callable, List
+import dataclasses
+import json
+
+from pocketbase.services.utils.base_service import BaseService
+from pocketbase.services.utils.sse import Event, SSEClient
+from pocketbase.models.record import Record
+
+
+@dataclasses.dataclass
+class MessageData:
+    action: str
+    record: Record
+
+
+class RealtimeService(BaseService):
+    subscriptions: dict
+    client_id: str = ""
+    event_source: SSEClient | None = None
+
+    def __init__(self, client) -> None:
+        super().__init__(client)
+        self.subscriptions = {}
+        self.client_id = ""
+        self.event_source = None
+
+    def subscribe(
+        self, subscription: str, callback: Callable[[MessageData], None]
+    ) -> None:
+        """Inits the sse connection (if not already) and register the subscription."""
+        # unsubscribe existing
+        if subscription in self.subscriptions and self.event_source:
+            self.event_source.remove_event_listener(subscription, callback)
+        # register subscription
+        self.subscriptions[subscription] = self._make_subscription(callback)
+        if not self.event_source:
+            self._connect()
+        elif self.client_id:
+            self._submit_subscriptions()
+
+    def unsubscribe_by_prefix(self, subscription_prefix: str):
+        """
+        Unsubscribe from all subscriptions starting with the provided prefix.
+
+        This method is no-op if there are no active subscriptions with the provided prefix.
+
+        The related sse connection will be autoclosed if after the
+        unsubscribe operation there are no active subscriptions left.
+        """
+        to_unsubscribe = []
+        for sub in self.subscriptions:
+            if sub.startswith(subscription_prefix):
+                to_unsubscribe.append(sub)
+        if len(to_unsubscribe) == 0:
+            return
+        return self.unsubscribe(*to_unsubscribe)
+
+    def unsubscribe(self, subscriptions: List[str] | None = None) -> None:
+        """
+        Unsubscribe from a subscription.
+
+        If the `subscriptions` argument is not set,
+        then the client will unsubscribe from all registered subscriptions.
+
+        The related sse connection will be autoclosed if after the
+        unsubscribe operations there are no active subscriptions left.
+        """
+        if not subscriptions or len(subscriptions) == 0:
+            # remove all subscriptions
+            self._remove_subscription_listeners()
+            self.subscriptions = {}
+        else:
+            # remove each passed subscription
+            found = False
+            for sub in self.subscriptions:
+                found = True
+                self.event_source.remove_event_listener(sub, self.subscriptions[sub])
+                self.subscriptions.pop(sub)
+            if not found:
+                return
+
+        if self.client_id:
+            self._submit_subscriptions()
+
+        # no more subscriptions -> close the sse connection
+        if not self.subscriptions:
+            self._disconnect()
+
+    def _make_subscription(
+        self, callback: Callable[[MessageData], None]
+    ) -> Callable[[Event], None]:
+        def listener(event: Event) -> None:
+            data = json.loads(event.data)
+            if "record" in data and "action" in data:
+                callback(
+                    MessageData(
+                        action=data["action"],
+                        record=Record(
+                            data=data["record"],
+                        ),
+                    )
+                )
+
+        return listener
+
+    def _submit_subscriptions(self) -> bool:
+        self._add_subscription_listeners()
+        self.client.send(
+            "/api/realtime",
+            {
+                "method": "POST",
+                "body": {
+                    "clientId": self.client_id,
+                    "subscriptions": list(self.subscriptions.keys()),
+                },
+            },
+        )
+        return True
+
+    def _add_subscription_listeners(self) -> None:
+        if not self.event_source:
+            return
+        self._remove_subscription_listeners()
+        for subscription, callback in self.subscriptions.items():
+            self.event_source.add_event_listener(subscription, callback)
+
+    def _remove_subscription_listeners(self) -> None:
+        if not self.event_source:
+            return
+        for subscription, callback in self.subscriptions.items():
+            self.event_source.remove_event_listener(subscription, callback)
+
+    def _connect_handler(self, event: Event) -> None:
+        self.client_id = event.id
+        self._submit_subscriptions()
+
+    def _connect(self) -> None:
+        self._disconnect()
+        self.event_source = SSEClient(self.client.build_url("/api/realtime"))
+        self.event_source.add_event_listener("PB_CONNECT", self._connect_handler)
+
+    def _disconnect(self) -> None:
+        self._remove_subscription_listeners()
+        self.client_id = ""
+        if not self.event_source:
+            return
+        self.event_source.remove_event_listener("PB_CONNECT", self._connect_handler)
+        self.event_source.close()
+        self.event_source = None
```

### Comparing `pocketbase-0.8.1/pocketbase/services/record_service.py` & `pocketbase-0.8.2/pocketbase/services/record_service.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,275 +1,275 @@
-from __future__ import annotations
-from dataclasses import dataclass
-from typing import List
-
-from urllib.parse import quote, urlencode
-from pocketbase.services.realtime_service import Callable, MessageData
-
-from pocketbase.models.utils.base_model import BaseModel
-from pocketbase.models.record import Record
-from pocketbase.services.utils.crud_service import CrudService
-from pocketbase.utils import camel_to_snake
-
-
-class RecordAuthResponse:
-    token: str
-    record: Record
-
-    def __init__(self, token: str, record: Record, **kwargs) -> None:
-        self.token = token
-        self.record = record
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-
-
-@dataclass
-class AuthProviderInfo:
-    name: str
-    state: str
-    code_verifier: str
-    code_challenge: str
-    code_challenge_method: str
-    auth_url: str
-
-
-@dataclass
-class AuthMethodsList:
-    username_password: bool
-    email_password: bool
-    auth_providers: list[AuthProviderInfo]
-
-
-class RecordService(CrudService):
-    collection_id_or_name: str
-
-    def __init__(self, client, collection_id_or_name) -> None:
-        super().__init__(client)
-        self.collection_id_or_name = collection_id_or_name
-
-    def decode(self, data: dict) -> BaseModel:
-        return Record(data)
-
-    def base_crud_path(self) -> str:
-        return self.base_collection_path() + "/records"
-
-    def base_collection_path(self) -> str:
-        """Returns the current collection service base path."""
-        return "/api/collections/" + quote(self.collection_id_or_name)
-
-    def get_file_url(
-        self, record: Record, filename: str, query_params: dict = {}
-    ) -> str:
-        """Builds and returns an absolute record file url."""
-        base_url = self.client.base_url
-        if base_url.endswith("/"):
-            base_url = base_url[:-1]
-        result = f"{base_url}/api/files/{record.collection_id}/{record.id}/{filename}"
-        if query_params:
-            result += "?" + urlencode(query_params)
-        return result
-
-    def subscribe(self, callback: Callable[[MessageData], None]):
-        """Subscribe to realtime changes of any record from the collection."""
-        return self.client.realtime.subscribe(self.collection_id_or_name, callback)
-
-    def subscribeOne(self, record_id: str, callback: Callable[[MessageData], None]):
-        """Subscribe to the realtime changes of a single record in the collection."""
-        return self.client.realtime.subscribe(
-            self.collection_id_or_name + "/" + record_id, callback
-        )
-
-    def unsubscribe(self, *record_ids: List[str]):
-        """Subscribe to the realtime changes of a single record in the collection."""
-        if record_ids and len(record_ids) == 0:
-            subs = []
-            for id in record_ids:
-                subs.append(self.collection_id_or_name + "/" + id)
-            return self.client.realtime.unsubscribe(*subs)
-        return self.client.realtime.subscribe_by_prefix(self.collection_id_or_name)
-
-    def update(self, id: str, body_params: dict = {}, query_params: dict = {}):
-        """
-        If the current `client.auth_store.model` matches with the updated id, then
-        on success the `client.auth_store.model` will be updated with the result.
-        """
-        item = super().update(id, body_params)  # super(Record).update
-        try:
-            if (
-                self.client.auth_store.model.collection_id is not None
-                and item.id == self.client.auth_store.model.id
-            ):
-                self.client.auth_store.save(self.client.auth_store.token, item)
-        except:
-            pass
-        return item
-
-    def delete(self, id: str, body_params: dict = {}, query_params: dict = {}):
-        """
-        If the current `client.auth_store.model` matches with the deleted id,
-        then on success the `client.auth_store` will be cleared.
-        """
-        success = super().delete(id, body_params)  # super(Record).delete
-        try:
-            if (
-                success
-                and self.client.auth_store.model.collection_id is not None
-                and id == self.client.auth_store.model.id
-            ):
-                self.client.auth_store.clear()
-        except:
-            pass
-        return success
-
-    def auth_response(self, response_data: dict) -> RecordAuthResponse:
-        """Prepare successful collection authorization response."""
-        record = self.decode(response_data.pop("record", {}))
-        token = response_data.pop("token", "")
-        if token and record:
-            self.client.auth_store.save(token, record)
-        return RecordAuthResponse(token=token, record=record, **response_data)
-
-    def list_auth_methods(self, query_params: str = {}):
-        """Returns all available collection auth methods."""
-        response_data = self.client.send(
-            self.base_collection_path() + "/auth-methods",
-            {"method": "GET", "params": query_params},
-        )
-        username_password = response_data.pop("usernamePassword", False)
-        email_password = response_data.pop("emailPassword", False)
-
-        def apply_pythonic_keys(ap):
-            pythonic_keys_ap = {
-                camel_to_snake(key).replace("@", ""): value for key, value in ap.items()
-            }
-            return pythonic_keys_ap
-
-        auth_providers = [
-            AuthProviderInfo(**auth_provider)
-            for auth_provider in map(
-                apply_pythonic_keys, response_data.get("authProviders", [])
-            )
-        ]
-        return AuthMethodsList(username_password, email_password, auth_providers)
-
-    def auth_with_password(
-        self,
-        username_or_email: str,
-        password: str,
-        body_params: dict = {},
-        query_params: dict = {},
-    ) -> RecordAuthResponse:
-        """
-        Authenticate a single auth collection record via its username/email and password.
-
-        On success, this method also automatically updates
-        the client's AuthStore data and returns:
-        - the authentication token
-        - the authenticated record model
-        """
-        body_params.update({"identity": username_or_email, "password": password})
-        response_data = self.client.send(
-            self.base_collection_path() + "/auth-with-password",
-            {
-                "method": "POST",
-                "params": query_params,
-                "body": body_params,
-                "headers": {"Authorization": ""},
-            },
-        )
-        return self.auth_response(response_data)
-
-    def auth_with_oauth2(
-        self,
-        provider: str,
-        code: str,
-        code_verifier: str,
-        redirct_url: str,
-        create_data={},
-        body_params={},
-        query_params={},
-    ):
-        """
-        Authenticate a single auth collection record with OAuth2.
-
-        On success, this method also automatically updates
-        the client's AuthStore data and returns:
-        - the authentication token
-        - the authenticated record model
-        - the OAuth2 account data (eg. name, email, avatar, etc.)
-        """
-        body_params.update(
-            {
-                "provider": provider,
-                "code": code,
-                "codeVerifier": code_verifier,
-                "redirectUrl": redirct_url,
-                "createData": create_data,
-            }
-        )
-        response_data = self.client.send(
-            self.base_collection_path() + "/auth-with-oauth2",
-            {
-                "method": "POST",
-                "params": query_params,
-                "body": body_params,
-            },
-        )
-        return self.auth_response(response_data)
-
-    def authRefresh(
-        self, body_params: dict = {}, query_params: dict = {}
-    ) -> RecordAuthResponse:
-        """
-        Refreshes the current authenticated record instance and
-        returns a new token and record data.
-
-        On success this method also automatically updates the client's AuthStore.
-        """
-        return self.auth_response(
-            self.client.send(
-                self.base_collection_path() + "/auth-refresh",
-                {"method": "POST", "params": query_params, "body": body_params},
-            )
-        )
-
-    def requestPasswordReset(
-        self, email: str, body_params: dict = {}, query_params: dict = {}
-    ) -> bool:
-        """Sends auth record password reset request."""
-        body_params.update({"email": email})
-        self.client.send(
-            self.base_collection_path() + "/request-password-reset",
-            {
-                "method": "POST",
-                "params": query_params,
-                "body": body_params,
-            },
-        )
-        return True
-
-    def confirmPasswordReset(
-        self,
-        password_reset_token: str,
-        password: str,
-        password_confirm: str,
-        body_params: dict = {},
-        query_params: dict = {},
-    ) -> RecordAuthResponse:
-        """Confirms auth record password reset reque"""
-        body_params.update(
-            {
-                "token": password_reset_token,
-                "password": password,
-                "passwordConfirm": password_confirm,
-            }
-        )
-        return self.auth_response(
-            self.client.send(
-                self.base_collection_path() + "/confirm-password-reset",
-                {
-                    "method": "POST",
-                    "params": query_params,
-                    "body": body_params,
-                },
-            )
-        )
+from __future__ import annotations
+from dataclasses import dataclass
+from typing import List
+
+from urllib.parse import quote, urlencode
+from pocketbase.services.realtime_service import Callable, MessageData
+
+from pocketbase.models.utils.base_model import BaseModel
+from pocketbase.models.record import Record
+from pocketbase.services.utils.crud_service import CrudService
+from pocketbase.utils import camel_to_snake
+
+
+class RecordAuthResponse:
+    token: str
+    record: Record
+
+    def __init__(self, token: str, record: Record, **kwargs) -> None:
+        self.token = token
+        self.record = record
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
+
+@dataclass
+class AuthProviderInfo:
+    name: str
+    state: str
+    code_verifier: str
+    code_challenge: str
+    code_challenge_method: str
+    auth_url: str
+
+
+@dataclass
+class AuthMethodsList:
+    username_password: bool
+    email_password: bool
+    auth_providers: list[AuthProviderInfo]
+
+
+class RecordService(CrudService):
+    collection_id_or_name: str
+
+    def __init__(self, client, collection_id_or_name) -> None:
+        super().__init__(client)
+        self.collection_id_or_name = collection_id_or_name
+
+    def decode(self, data: dict) -> BaseModel:
+        return Record(data)
+
+    def base_crud_path(self) -> str:
+        return self.base_collection_path() + "/records"
+
+    def base_collection_path(self) -> str:
+        """Returns the current collection service base path."""
+        return "/api/collections/" + quote(self.collection_id_or_name)
+
+    def get_file_url(
+        self, record: Record, filename: str, query_params: dict = {}
+    ) -> str:
+        """Builds and returns an absolute record file url."""
+        base_url = self.client.base_url
+        if base_url.endswith("/"):
+            base_url = base_url[:-1]
+        result = f"{base_url}/api/files/{record.collection_id}/{record.id}/{filename}"
+        if query_params:
+            result += "?" + urlencode(query_params)
+        return result
+
+    def subscribe(self, callback: Callable[[MessageData], None]):
+        """Subscribe to realtime changes of any record from the collection."""
+        return self.client.realtime.subscribe(self.collection_id_or_name, callback)
+
+    def subscribeOne(self, record_id: str, callback: Callable[[MessageData], None]):
+        """Subscribe to the realtime changes of a single record in the collection."""
+        return self.client.realtime.subscribe(
+            self.collection_id_or_name + "/" + record_id, callback
+        )
+
+    def unsubscribe(self, *record_ids: List[str]):
+        """Subscribe to the realtime changes of a single record in the collection."""
+        if record_ids and len(record_ids) == 0:
+            subs = []
+            for id in record_ids:
+                subs.append(self.collection_id_or_name + "/" + id)
+            return self.client.realtime.unsubscribe(*subs)
+        return self.client.realtime.subscribe_by_prefix(self.collection_id_or_name)
+
+    def update(self, id: str, body_params: dict = {}, query_params: dict = {}):
+        """
+        If the current `client.auth_store.model` matches with the updated id, then
+        on success the `client.auth_store.model` will be updated with the result.
+        """
+        item = super().update(id, body_params)  # super(Record).update
+        try:
+            if (
+                self.client.auth_store.model.collection_id is not None
+                and item.id == self.client.auth_store.model.id
+            ):
+                self.client.auth_store.save(self.client.auth_store.token, item)
+        except:
+            pass
+        return item
+
+    def delete(self, id: str, body_params: dict = {}, query_params: dict = {}):
+        """
+        If the current `client.auth_store.model` matches with the deleted id,
+        then on success the `client.auth_store` will be cleared.
+        """
+        success = super().delete(id, body_params)  # super(Record).delete
+        try:
+            if (
+                success
+                and self.client.auth_store.model.collection_id is not None
+                and id == self.client.auth_store.model.id
+            ):
+                self.client.auth_store.clear()
+        except:
+            pass
+        return success
+
+    def auth_response(self, response_data: dict) -> RecordAuthResponse:
+        """Prepare successful collection authorization response."""
+        record = self.decode(response_data.pop("record", {}))
+        token = response_data.pop("token", "")
+        if token and record:
+            self.client.auth_store.save(token, record)
+        return RecordAuthResponse(token=token, record=record, **response_data)
+
+    def list_auth_methods(self, query_params: str = {}):
+        """Returns all available collection auth methods."""
+        response_data = self.client.send(
+            self.base_collection_path() + "/auth-methods",
+            {"method": "GET", "params": query_params},
+        )
+        username_password = response_data.pop("usernamePassword", False)
+        email_password = response_data.pop("emailPassword", False)
+
+        def apply_pythonic_keys(ap):
+            pythonic_keys_ap = {
+                camel_to_snake(key).replace("@", ""): value for key, value in ap.items()
+            }
+            return pythonic_keys_ap
+
+        auth_providers = [
+            AuthProviderInfo(**auth_provider)
+            for auth_provider in map(
+                apply_pythonic_keys, response_data.get("authProviders", [])
+            )
+        ]
+        return AuthMethodsList(username_password, email_password, auth_providers)
+
+    def auth_with_password(
+        self,
+        username_or_email: str,
+        password: str,
+        body_params: dict = {},
+        query_params: dict = {},
+    ) -> RecordAuthResponse:
+        """
+        Authenticate a single auth collection record via its username/email and password.
+
+        On success, this method also automatically updates
+        the client's AuthStore data and returns:
+        - the authentication token
+        - the authenticated record model
+        """
+        body_params.update({"identity": username_or_email, "password": password})
+        response_data = self.client.send(
+            self.base_collection_path() + "/auth-with-password",
+            {
+                "method": "POST",
+                "params": query_params,
+                "body": body_params,
+                "headers": {"Authorization": ""},
+            },
+        )
+        return self.auth_response(response_data)
+
+    def auth_with_oauth2(
+        self,
+        provider: str,
+        code: str,
+        code_verifier: str,
+        redirct_url: str,
+        create_data={},
+        body_params={},
+        query_params={},
+    ):
+        """
+        Authenticate a single auth collection record with OAuth2.
+
+        On success, this method also automatically updates
+        the client's AuthStore data and returns:
+        - the authentication token
+        - the authenticated record model
+        - the OAuth2 account data (eg. name, email, avatar, etc.)
+        """
+        body_params.update(
+            {
+                "provider": provider,
+                "code": code,
+                "codeVerifier": code_verifier,
+                "redirectUrl": redirct_url,
+                "createData": create_data,
+            }
+        )
+        response_data = self.client.send(
+            self.base_collection_path() + "/auth-with-oauth2",
+            {
+                "method": "POST",
+                "params": query_params,
+                "body": body_params,
+            },
+        )
+        return self.auth_response(response_data)
+
+    def authRefresh(
+        self, body_params: dict = {}, query_params: dict = {}
+    ) -> RecordAuthResponse:
+        """
+        Refreshes the current authenticated record instance and
+        returns a new token and record data.
+
+        On success this method also automatically updates the client's AuthStore.
+        """
+        return self.auth_response(
+            self.client.send(
+                self.base_collection_path() + "/auth-refresh",
+                {"method": "POST", "params": query_params, "body": body_params},
+            )
+        )
+
+    def requestPasswordReset(
+        self, email: str, body_params: dict = {}, query_params: dict = {}
+    ) -> bool:
+        """Sends auth record password reset request."""
+        body_params.update({"email": email})
+        self.client.send(
+            self.base_collection_path() + "/request-password-reset",
+            {
+                "method": "POST",
+                "params": query_params,
+                "body": body_params,
+            },
+        )
+        return True
+
+    def confirmPasswordReset(
+        self,
+        password_reset_token: str,
+        password: str,
+        password_confirm: str,
+        body_params: dict = {},
+        query_params: dict = {},
+    ) -> RecordAuthResponse:
+        """Confirms auth record password reset reque"""
+        body_params.update(
+            {
+                "token": password_reset_token,
+                "password": password,
+                "passwordConfirm": password_confirm,
+            }
+        )
+        return self.auth_response(
+            self.client.send(
+                self.base_collection_path() + "/confirm-password-reset",
+                {
+                    "method": "POST",
+                    "params": query_params,
+                    "body": body_params,
+                },
+            )
+        )
```

### Comparing `pocketbase-0.8.1/pocketbase/services/settings_service.py` & `pocketbase-0.8.2/pocketbase/services/settings_service.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from __future__ import annotations
-
-from pocketbase.services.utils.base_service import BaseService
-
-
-class SettingsService(BaseService):
-    def get_all(self, query_params: dict = {}) -> dict:
-        """Fetch all available app settings."""
-        return self.client.send(
-            "/api/settings",
-            {"method": "GET", "params": query_params},
-        )
-
-    def update(self, body_params: dict = {}, query_params: dict = {}) -> dict:
-        """Bulk updates app settings."""
-        return self.client.send(
-            "/api/settings",
-            {
-                "method": "PATCH",
-                "params": query_params,
-                "body": body_params,
-            },
-        )
-
-    def test_s3(self, query_params: dict = {}) -> bool:
-        """Performs a S3 storage connection test."""
-        self.client.send(
-            "/api/settings/test/s3",
-            {"method": "POST", "params": query_params},
-        )
-        return True
-
-    def test_email(
-        self, to_email: str, email_template: str, query_params: dict = {}
-    ) -> bool:
-        """
-        Sends a test email.
-
-        The possible `email_template` values are:
-        - verification
-        - password-reset
-        - email-change
-        """
-        self.client.send(
-            "/api/settings/test/email",
-            {
-                "method": "POST",
-                "params": query_params,
-                "body": {"email": to_email, "template": email_template},
-            },
-        )
-        return True
+from __future__ import annotations
+
+from pocketbase.services.utils.base_service import BaseService
+
+
+class SettingsService(BaseService):
+    def get_all(self, query_params: dict = {}) -> dict:
+        """Fetch all available app settings."""
+        return self.client.send(
+            "/api/settings",
+            {"method": "GET", "params": query_params},
+        )
+
+    def update(self, body_params: dict = {}, query_params: dict = {}) -> dict:
+        """Bulk updates app settings."""
+        return self.client.send(
+            "/api/settings",
+            {
+                "method": "PATCH",
+                "params": query_params,
+                "body": body_params,
+            },
+        )
+
+    def test_s3(self, query_params: dict = {}) -> bool:
+        """Performs a S3 storage connection test."""
+        self.client.send(
+            "/api/settings/test/s3",
+            {"method": "POST", "params": query_params},
+        )
+        return True
+
+    def test_email(
+        self, to_email: str, email_template: str, query_params: dict = {}
+    ) -> bool:
+        """
+        Sends a test email.
+
+        The possible `email_template` values are:
+        - verification
+        - password-reset
+        - email-change
+        """
+        self.client.send(
+            "/api/settings/test/email",
+            {
+                "method": "POST",
+                "params": query_params,
+                "body": {"email": to_email, "template": email_template},
+            },
+        )
+        return True
```

### Comparing `pocketbase-0.8.1/pocketbase/services/utils/sse.py` & `pocketbase-0.8.2/pocketbase/services/utils/sse.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-from __future__ import annotations
-
-from typing import Callable
-import dataclasses
-import threading
-
-import httpx
-
-
-@dataclasses.dataclass
-class Event:
-    """Representation of an event"""
-
-    id: str = ""
-    event: str = "message"
-    data: str = ""
-    retry: int | None = None
-
-
-class EventLoop(threading.Thread):
-    FIELD_SEPARATOR = ":"
-
-    def __init__(
-        self,
-        url: str,
-        method: str = "GET",
-        headers: dict | None = None,
-        payload: dict | None = None,
-        encoding="utf-8",
-        listeners: dict[str, Callable] | None = None,
-        **kwargs,
-    ):
-        threading.Thread.__init__(self, **kwargs)
-        self.kill = False
-        self.client = httpx.Client()
-        self.url = url
-        self.method = method
-        self.headers = headers
-        self.payload = payload
-        self.encoding = encoding
-        self.listeners = listeners or {}
-
-    def _read(self):
-        """Read the incoming event source stream and yield event chunks"""
-        data = b""
-        with self.client.stream(
-            self.method,
-            self.url,
-            headers=self.headers,
-            data=self.payload,
-            timeout=None,
-        ) as r:
-            for chunk in r.iter_bytes():
-                for line in chunk.splitlines(True):
-                    data += line
-                    if data.endswith((b"\r\r", b"\n\n", b"\r\n\r\n")):
-                        yield data
-                        data = b""
-            if data:
-                yield data
-
-    def _events(self):
-        for chunk in self._read():
-            event = Event()
-            for line in chunk.splitlines():
-                line = line.decode(self.encoding)
-                if not line.strip() or line.startswith(self.FIELD_SEPARATOR):
-                    continue
-                data = line.split(self.FIELD_SEPARATOR, 1)
-                field = data[0]
-                if field not in event.__dict__:
-                    continue
-                if len(data) > 1:
-                    if data[1].startswith(" "):
-                        value = data[1][1:]
-                    else:
-                        value = data[1]
-                else:
-                    value = ""
-                if field == "data":
-                    event.data += value + "\n"
-                else:
-                    setattr(event, field, value)
-            if not event.data:
-                continue
-            if event.data.endswith("\n"):
-                event.data = event.data[0:-1]
-            event.event = event.event or "message"
-            yield event
-
-    def run(self):
-        for event in self._events():
-            if self.kill:
-                break
-            if event.event in self.listeners:
-                self.listeners[event.event](event)
-
-
-class SSEClient:
-    """Implementation of a server side event client"""
-
-    _listeners: dict = {}
-    _loop_thread: threading.Thread | None = None
-
-    def __init__(
-        self,
-        url: str,
-        method: str = "GET",
-        headers: dict | None = None,
-        payload: dict | None = None,
-        encoding="utf-8",
-    ) -> None:
-        self._listeners = {}
-        self._loop_thread = EventLoop(
-            url=url,
-            method=method,
-            headers=headers,
-            payload=payload,
-            encoding=encoding,
-            listeners=self._listeners,
-            name="loop",
-        )
-        self._loop_thread.daemon = True
-        self._loop_thread.start()
-
-    def add_event_listener(self, event: str, callback: Callable[[Event], None]) -> None:
-        self._listeners[event] = callback
-        self._loop_thread.listeners = self._listeners
-
-    def remove_event_listener(
-        self, event: str, callback: Callable[[Event], None]
-    ) -> None:
-        if event in self._listeners:
-            self._listeners.pop(event)
-            self._loop_thread.listeners = self._listeners
-
-    def close(self) -> None:
-        # TODO: does not work like this
-        self._loop_thread.kill = True
+from __future__ import annotations
+
+from typing import Callable
+import dataclasses
+import threading
+
+import httpx
+
+
+@dataclasses.dataclass
+class Event:
+    """Representation of an event"""
+
+    id: str = ""
+    event: str = "message"
+    data: str = ""
+    retry: int | None = None
+
+
+class EventLoop(threading.Thread):
+    FIELD_SEPARATOR = ":"
+
+    def __init__(
+        self,
+        url: str,
+        method: str = "GET",
+        headers: dict | None = None,
+        payload: dict | None = None,
+        encoding="utf-8",
+        listeners: dict[str, Callable] | None = None,
+        **kwargs,
+    ):
+        threading.Thread.__init__(self, **kwargs)
+        self.kill = False
+        self.client = httpx.Client()
+        self.url = url
+        self.method = method
+        self.headers = headers
+        self.payload = payload
+        self.encoding = encoding
+        self.listeners = listeners or {}
+
+    def _read(self):
+        """Read the incoming event source stream and yield event chunks"""
+        data = b""
+        with self.client.stream(
+            self.method,
+            self.url,
+            headers=self.headers,
+            data=self.payload,
+            timeout=None,
+        ) as r:
+            for chunk in r.iter_bytes():
+                for line in chunk.splitlines(True):
+                    data += line
+                    if data.endswith((b"\r\r", b"\n\n", b"\r\n\r\n")):
+                        yield data
+                        data = b""
+            if data:
+                yield data
+
+    def _events(self):
+        for chunk in self._read():
+            event = Event()
+            for line in chunk.splitlines():
+                line = line.decode(self.encoding)
+                if not line.strip() or line.startswith(self.FIELD_SEPARATOR):
+                    continue
+                data = line.split(self.FIELD_SEPARATOR, 1)
+                field = data[0]
+                if field not in event.__dict__:
+                    continue
+                if len(data) > 1:
+                    if data[1].startswith(" "):
+                        value = data[1][1:]
+                    else:
+                        value = data[1]
+                else:
+                    value = ""
+                if field == "data":
+                    event.data += value + "\n"
+                else:
+                    setattr(event, field, value)
+            if not event.data:
+                continue
+            if event.data.endswith("\n"):
+                event.data = event.data[0:-1]
+            event.event = event.event or "message"
+            yield event
+
+    def run(self):
+        for event in self._events():
+            if self.kill:
+                break
+            if event.event in self.listeners:
+                self.listeners[event.event](event)
+
+
+class SSEClient:
+    """Implementation of a server side event client"""
+
+    _listeners: dict = {}
+    _loop_thread: threading.Thread | None = None
+
+    def __init__(
+        self,
+        url: str,
+        method: str = "GET",
+        headers: dict | None = None,
+        payload: dict | None = None,
+        encoding="utf-8",
+    ) -> None:
+        self._listeners = {}
+        self._loop_thread = EventLoop(
+            url=url,
+            method=method,
+            headers=headers,
+            payload=payload,
+            encoding=encoding,
+            listeners=self._listeners,
+            name="loop",
+        )
+        self._loop_thread.daemon = True
+        self._loop_thread.start()
+
+    def add_event_listener(self, event: str, callback: Callable[[Event], None]) -> None:
+        self._listeners[event] = callback
+        self._loop_thread.listeners = self._listeners
+
+    def remove_event_listener(
+        self, event: str, callback: Callable[[Event], None]
+    ) -> None:
+        if event in self._listeners:
+            self._listeners.pop(event)
+            self._loop_thread.listeners = self._listeners
+
+    def close(self) -> None:
+        # TODO: does not work like this
+        self._loop_thread.kill = True
```

### Comparing `pocketbase-0.8.1/pocketbase/stores/base_auth_store.py` & `pocketbase-0.8.2/pocketbase/stores/base_auth_store.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from __future__ import annotations
-
-from abc import ABC
-
-from pocketbase.models.admin import Admin
-from pocketbase.models.record import Record
-
-
-class BaseAuthStore(ABC):
-    """
-    Base AuthStore class that is intended to be extended by all other
-    PocketBase AuthStore implementations.
-    """
-
-    base_token: str
-    base_model: Record | Admin | None
-
-    def __init__(
-        self, base_token: str = "", base_model: Record | Admin | None = None
-    ) -> None:
-        super().__init__()
-        self.base_token = base_token
-        self.base_model = base_model
-
-    @property
-    def token(self) -> str | None:
-        """Retrieves the stored token (if any)."""
-        return self.base_token
-
-    @property
-    def model(self) -> Record | Admin | None:
-        """Retrieves the stored model data (if any)."""
-        return self.base_model
-
-    def save(self, token: str = "", model: Record | Admin | None = None) -> None:
-        """Saves the provided new token and model data in the auth store."""
-
-        self.base_token = token if token else ""
-        self.base_model = model if model else None
-
-    def clear(self) -> None:
-        """Removes the stored token and model data form the auth store."""
-        self.base_token = None
-        self.base_model = None
+from __future__ import annotations
+
+from abc import ABC
+
+from pocketbase.models.admin import Admin
+from pocketbase.models.record import Record
+
+
+class BaseAuthStore(ABC):
+    """
+    Base AuthStore class that is intended to be extended by all other
+    PocketBase AuthStore implementations.
+    """
+
+    base_token: str
+    base_model: Record | Admin | None
+
+    def __init__(
+        self, base_token: str = "", base_model: Record | Admin | None = None
+    ) -> None:
+        super().__init__()
+        self.base_token = base_token
+        self.base_model = base_model
+
+    @property
+    def token(self) -> str | None:
+        """Retrieves the stored token (if any)."""
+        return self.base_token
+
+    @property
+    def model(self) -> Record | Admin | None:
+        """Retrieves the stored model data (if any)."""
+        return self.base_model
+
+    def save(self, token: str = "", model: Record | Admin | None = None) -> None:
+        """Saves the provided new token and model data in the auth store."""
+
+        self.base_token = token if token else ""
+        self.base_model = model if model else None
+
+    def clear(self) -> None:
+        """Removes the stored token and model data form the auth store."""
+        self.base_token = None
+        self.base_model = None
```

### Comparing `pocketbase-0.8.1/pocketbase/stores/local_auth_store.py` & `pocketbase-0.8.2/pocketbase/stores/local_auth_store.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from __future__ import annotations
-
-from typing import Any
-import pickle
-import os
-
-from pocketbase.stores.base_auth_store import BaseAuthStore
-from pocketbase.models.record import Record
-from pocketbase.models.admin import Admin
-
-
-class LocalAuthStore(BaseAuthStore):
-    filename: str
-    filepath: str
-
-    def __init__(
-        self,
-        filename: str = "pocketbase_auth.data",
-        filepath: str = "",
-        base_token: str = "",
-        base_model: Record | Admin | None = None,
-    ) -> None:
-        super().__init__(base_token, base_model)
-        self.filename = filename
-        self.filepath = filepath
-        self.complete_filepath = os.path.join(filepath, filename)
-
-    @property
-    def token(self) -> str:
-        data = self._storage_get(self.complete_filepath)
-        if not data or "token" not in data:
-            return None
-        return data["token"]
-
-    @property
-    def model(self) -> Record | Admin | None:
-        data = self._storage_get(self.complete_filepath)
-        if not data or "model" not in data:
-            return None
-        return data["model"]
-
-    def save(self, token: str = "", model: Record | Admin | None = None) -> None:
-        self._storage_set(self.complete_filepath, {"token": token, "model": model})
-        super().save(token, model)
-
-    def clear(self) -> None:
-        self._storage_remove(self.complete_filepath)
-        super().clear()
-
-    def _storage_set(self, key: str, value: Any) -> None:
-        with open(key, "wb") as f:
-            pickle.dump(value, f)
-
-    def _storage_get(self, key: str) -> Any:
-        with open(key, "rb") as f:
-            value = pickle.load(f)
-        return value
-
-    def _storage_remove(self, key: str) -> None:
-        if os.path.exists(key):
-            os.remove(key)
+from __future__ import annotations
+
+from typing import Any
+import pickle
+import os
+
+from pocketbase.stores.base_auth_store import BaseAuthStore
+from pocketbase.models.record import Record
+from pocketbase.models.admin import Admin
+
+
+class LocalAuthStore(BaseAuthStore):
+    filename: str
+    filepath: str
+
+    def __init__(
+        self,
+        filename: str = "pocketbase_auth.data",
+        filepath: str = "",
+        base_token: str = "",
+        base_model: Record | Admin | None = None,
+    ) -> None:
+        super().__init__(base_token, base_model)
+        self.filename = filename
+        self.filepath = filepath
+        self.complete_filepath = os.path.join(filepath, filename)
+
+    @property
+    def token(self) -> str:
+        data = self._storage_get(self.complete_filepath)
+        if not data or "token" not in data:
+            return None
+        return data["token"]
+
+    @property
+    def model(self) -> Record | Admin | None:
+        data = self._storage_get(self.complete_filepath)
+        if not data or "model" not in data:
+            return None
+        return data["model"]
+
+    def save(self, token: str = "", model: Record | Admin | None = None) -> None:
+        self._storage_set(self.complete_filepath, {"token": token, "model": model})
+        super().save(token, model)
+
+    def clear(self) -> None:
+        self._storage_remove(self.complete_filepath)
+        super().clear()
+
+    def _storage_set(self, key: str, value: Any) -> None:
+        with open(key, "wb") as f:
+            pickle.dump(value, f)
+
+    def _storage_get(self, key: str) -> Any:
+        with open(key, "rb") as f:
+            value = pickle.load(f)
+        return value
+
+    def _storage_remove(self, key: str) -> None:
+        if os.path.exists(key):
+            os.remove(key)
```

### Comparing `pocketbase-0.8.1/pyproject.toml` & `pocketbase-0.8.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-[project]
-name = "pocketbase"
-description = "PocketBase SDK for python."
-requires-python = ">=3.7"
-license = "MIT"
-authors = [
-    { name = "Vithor Jaeger", email = "vaphes@gmail.com" },
-    { name = "Max Amling", email = "max-amling@web.de" },
-]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Intended Audience :: Developers",
-]
-keywords = "pocketbase sdk"
-dependencies = ["httpx>=0.23.0"]
-dynamic = ["readme", "version"]
-
-[project.urls]
-"Homepage" = "https://github.com/vaphes/pocketbase"
-"Source" = "https://github.com/vaphes/pocketbase"
-"Bug Tracker" = "https://github.com/vaphes/pocketbase/issues"
-
-[tool.poetry]
-name = "pocketbase"
-version = "0.8.1"
-description = "PocketBase SDK for python."
-authors = ["Vithor Jaeger <vaphes@gmail.com>"]
-readme = "README.md"
-homepage = "https://github.com/vaphes/pocketbase"
-repository = "https://github.com/vaphes/pocketbase"
-keywords = ["pocketbase", "sdk"]
-
-[tool.poetry.urls]
-"Bug Tracker" = "https://github.com/vaphes/pocketbase/issues"
-
-[tool.poetry.dependencies]
-python = "^3.7"
-httpx = "^0.23.0"
-
-[tool.poetry.group.dev.dependencies]
-flake8 = "^5.0.4"
-pytest = "^7.1.3"
-black = {version = "^22.8.0", allow-prereleases = true}
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[project]
+name = "pocketbase"
+description = "PocketBase SDK for python."
+requires-python = ">=3.7"
+license = "MIT"
+authors = [
+    { name = "Vithor Jaeger", email = "vaphes@gmail.com" },
+    { name = "Max Amling", email = "max-amling@web.de" },
+]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Intended Audience :: Developers",
+]
+keywords = "pocketbase sdk"
+dependencies = ["httpx>=0.23.0"]
+dynamic = ["readme", "version"]
+
+[project.urls]
+"Homepage" = "https://github.com/vaphes/pocketbase"
+"Source" = "https://github.com/vaphes/pocketbase"
+"Bug Tracker" = "https://github.com/vaphes/pocketbase/issues"
+
+[tool.poetry]
+name = "pocketbase"
+version = "0.8.2"
+description = "PocketBase SDK for python."
+authors = ["Vithor Jaeger <vaphes@gmail.com>"]
+readme = "README.md"
+homepage = "https://github.com/vaphes/pocketbase"
+repository = "https://github.com/vaphes/pocketbase"
+keywords = ["pocketbase", "sdk"]
+
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/vaphes/pocketbase/issues"
+
+[tool.poetry.dependencies]
+python = "^3.7"
+httpx = "^0.23.0"
+
+[tool.poetry.group.dev.dependencies]
+flake8 = "^5.0.4"
+pytest = "^7.1.3"
+black = {version = "^22.8.0", allow-prereleases = true}
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pocketbase-0.8.1/PKG-INFO` & `pocketbase-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketbase
-Version: 0.8.1
+Version: 0.8.2
 Summary: PocketBase SDK for python.
 Home-page: https://github.com/vaphes/pocketbase
 Keywords: pocketbase,sdk
 Author: Vithor Jaeger
 Author-email: vaphes@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pocketbase Version: 0.8.1 Summary: PocketBase SDK
+Metadata-Version: 2.1 Name: pocketbase Version: 0.8.2 Summary: PocketBase SDK
 for python. Home-page: https://github.com/vaphes/pocketbase Keywords:
 pocketbase,sdk Author: Vithor Jaeger Author-email: vaphes@gmail.com Requires-
 Python: >=3.7,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: httpx (>=0.23.0,<0.24.0) Project-URL: Bug
```

