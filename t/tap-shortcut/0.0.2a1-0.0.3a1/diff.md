# Comparing `tmp/tap_shortcut-0.0.2a1.tar.gz` & `tmp/tap_shortcut-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_shortcut-0.0.2a1.tar", max compression
+gzip compressed data, was "tap_shortcut-0.0.3a1.tar", max compression
```

## Comparing `tap_shortcut-0.0.2a1.tar` & `tap_shortcut-0.0.3a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-04-11 06:41:11.321362 tap_shortcut-0.0.2a1/LICENSE
--rw-r--r--   0        0        0     2571 2023-04-11 06:41:11.321362 tap_shortcut-0.0.2a1/README.md
--rw-r--r--   0        0        0     1630 2023-04-11 06:41:29.625494 tap_shortcut-0.0.2a1/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-11 06:41:11.325362 tap_shortcut-0.0.2a1/tap_shortcut/__init__.py
--rw-r--r--   0        0        0     1004 2023-04-11 06:41:11.325362 tap_shortcut-0.0.2a1/tap_shortcut/client.py
--rw-r--r--   0        0        0     2299 2023-04-11 06:41:11.325362 tap_shortcut-0.0.2a1/tap_shortcut/streams.py
--rw-r--r--   0        0        0     3640 2023-04-11 06:41:11.325362 tap_shortcut-0.0.2a1/tap_shortcut/tap.py
--rw-r--r--   0        0        0     3519 1970-01-01 00:00:00.000000 tap_shortcut-0.0.2a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-02 03:12:14.242133 tap_shortcut-0.0.3a1/LICENSE
+-rw-r--r--   0        0        0     2571 2023-06-02 03:12:14.242133 tap_shortcut-0.0.3a1/README.md
+-rw-r--r--   0        0        0     2195 2023-06-02 03:12:36.842876 tap_shortcut-0.0.3a1/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-06-02 03:12:14.246133 tap_shortcut-0.0.3a1/tap_shortcut/__init__.py
+-rw-r--r--   0        0        0     1039 2023-06-02 03:12:14.246133 tap_shortcut-0.0.3a1/tap_shortcut/client.py
+-rw-r--r--   0        0        0     2559 2023-06-02 03:12:14.246133 tap_shortcut-0.0.3a1/tap_shortcut/streams.py
+-rw-r--r--   0        0        0     3634 2023-06-02 03:12:14.246133 tap_shortcut-0.0.3a1/tap_shortcut/tap.py
+-rw-r--r--   0        0        0     3519 1970-01-01 00:00:00.000000 tap_shortcut-0.0.3a1/PKG-INFO
```

### Comparing `tap_shortcut-0.0.2a1/LICENSE` & `tap_shortcut-0.0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.0.2a1/README.md` & `tap_shortcut-0.0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.0.2a1/tap_shortcut/client.py` & `tap_shortcut-0.0.3a1/tap_shortcut/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """REST client handling, including ShortcutStream base class."""
+from __future__ import annotations
 
 from singer_sdk import RESTStream
 from singer_sdk.authenticators import APIKeyAuthenticator
 
 
 class ShortcutStream(RESTStream):
     """Shortcut stream class."""
```

### Comparing `tap_shortcut-0.0.2a1/tap_shortcut/streams.py` & `tap_shortcut-0.0.3a1/tap_shortcut/streams.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 """Stream type classes for tap-shortcut."""
 
 from __future__ import annotations
 
 from tap_shortcut.client import ShortcutStream
 
+__all__ = [
+    "Categories",
+    "Epics",
+    "Files",
+    "Groups",
+    "Iterations",
+    "Labels",
+    "Members",
+    "Milestones",
+    "Projects",
+    "ProjectStories",
+    "Repositories",
+    "Workflows",
+]
+
 
 class Members(ShortcutStream):
     """Members stream."""
 
     name = "members"
     path = "/api/v3/members"
     primary_keys = ["id"]
@@ -16,15 +31,19 @@
 class Projects(ShortcutStream):
     """Projects stream."""
 
     name = "projects"
     path = "/api/v3/projects"
     primary_keys = ["id"]
 
-    def get_child_context(self, record: dict, context: dict | None) -> dict:
+    def get_child_context(
+        self,
+        record: dict,
+        context: dict | None,  # noqa: ARG002
+    ) -> dict:
         """Return a dictionary of child context.
 
         Args:
             record: A dictionary of the record.
             context: A dictionary of the context.
 
         Returns:
```

### Comparing `tap_shortcut-0.0.2a1/tap_shortcut/tap.py` & `tap_shortcut-0.0.3a1/tap_shortcut/tap.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,56 @@
 """Shortcut tap class."""
+from __future__ import annotations
 
 from copy import deepcopy
-from typing import Any, Dict, List, Type, Union
+from typing import TYPE_CHECKING, Any
 
 import requests
 from singer_sdk import RESTStream, Stream, Tap
 from singer_sdk import typing as th
 from singer_sdk._singerlib import resolve_schema_references
 from toolz.dicttoolz import get_in
 
-from tap_shortcut.client import ShortcutStream
-from tap_shortcut.streams import (
-    Categories,
-    Epics,
-    Files,
-    Groups,
-    Iterations,
-    Labels,
-    Members,
-    Milestones,
-    Projects,
-    ProjectStories,
-    Repositories,
-    Workflows,
-)
-
-STREAM_TYPES: List[Type[ShortcutStream]] = [
-    Categories,
-    Epics,
-    Files,
-    Groups,
-    Iterations,
-    Labels,
-    Members,
-    Milestones,
-    Projects,
-    ProjectStories,
-    Repositories,
-    Workflows,
+from tap_shortcut import streams
+
+if TYPE_CHECKING:
+    from tap_shortcut.client import ShortcutStream
+
+STREAM_TYPES: list[type[ShortcutStream]] = [
+    streams.Categories,
+    streams.Epics,
+    streams.Files,
+    streams.Groups,
+    streams.Iterations,
+    streams.Labels,
+    streams.Members,
+    streams.Milestones,
+    streams.Projects,
+    streams.ProjectStories,
+    streams.Repositories,
+    streams.Workflows,
 ]
 
 OPENAPI_URL = "https://developer.shortcut.com/api/rest/v3/shortcut.swagger.json"
 
 
-def handle_x_nullable(schema: Dict[str, Any]) -> Dict[str, Any]:
+def handle_x_nullable(schema: dict[str, Any]) -> dict[str, Any]:
     """Resolve x-nullable properties to standard JSON Schema nullable type.
 
     Args:
         schema: A JSON Schema dictionary.
 
     Returns:
         A new JSON Schema dictionary with 'x-nullable' resolved to [<type>, "null"].
     """
     result = deepcopy(schema)
 
     if "object" in result["type"]:
         for prop, prop_schema in result.get("properties", {}).items():
-            prop_type: Union[str, List[str]] = prop_schema.get("type", [])
+            prop_type: str | list[str] = prop_schema.get("type", [])
             types = [prop_type] if isinstance(prop_type, str) else prop_type
             nullable: bool = prop_schema.get("x-nullable", False)
 
             if nullable:
                 prop_schema["type"] = [*types, "null"]
 
             result["properties"][prop] = handle_x_nullable(prop_schema)
@@ -93,30 +83,31 @@
 
         Returns:
             OpenAPI schema.
 
         Raises:
             RuntimeError: If the OpenAPI schema cannot be retrieved.
         """
-        response = requests.get(OPENAPI_URL)
+        response = requests.get(OPENAPI_URL, timeout=30)
         try:
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
-            raise RuntimeError(f"Error retrieving OpenAPI schema ({err})") from err
+            msg = f"Error retrieving OpenAPI schema ({err})"
+            raise RuntimeError(msg) from err
 
         return response.json()
 
-    def discover_streams(self) -> List[Stream]:
+    def discover_streams(self) -> list[Stream]:
         """Return a list of discovered streams.
 
         Returns:
             A list of Shortcut streams.
         """
         openapi_schema = self.get_openapi_schema()
-        streams: List[RESTStream] = []
+        streams: list[RESTStream] = []
 
         for stream_type in STREAM_TYPES:
             schema = get_in(
                 keys=[
                     "paths",
                     stream_type.path,
                     "get",
```

### Comparing `tap_shortcut-0.0.2a1/PKG-INFO` & `tap_shortcut-0.0.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tap-shortcut
-Version: 0.0.2a1
+Version: 0.0.3a1
 Summary: `tap-shortcut` is a Singer tap for Shortcut, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-shortcut
 License: Apache-2.0
 Keywords: ELT,singer.io,Shortcut
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: singer-sdk (==0.23.0)
+Requires-Dist: singer-sdk (==0.27.0)
 Requires-Dist: toolz (==0.12.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-shortcut#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-shortcut
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: tap-shortcut Version: 0.0.2a1 Summary: `tap-
+Metadata-Version: 2.1 Name: tap-shortcut Version: 0.0.3a1 Summary: `tap-
 shortcut` is a Singer tap for Shortcut, built with the Meltano SDK for Singer
 Taps. Home-page: https://github.com/edgarrmondragon/tap-shortcut License:
 Apache-2.0 Keywords: ELT,singer.io,Shortcut Author: Edgar RamÃ­rez-MondragÃ³n
 Author-email: edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: singer-sdk (==0.23.0) Requires-Dist: toolz (==0.12.0) Project-
+Requires-Dist: singer-sdk (==0.27.0) Requires-Dist: toolz (==0.12.0) Project-
 URL: Documentation, https://github.com/edgarrmondragon/tap-shortcut#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-shortcut
 Description-Content-Type: text/markdown
                                 # tap-shortcut
                        [pre-commit.ci_status] [License]
       Singer tap for Shortcut. Built with the [Meltano Tap SDK](https://
                        sdk.meltano.com) for Singer Taps.
```

