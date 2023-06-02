# Comparing `tmp/dataverse_api-0.2.2.tar.gz` & `tmp/dataverse_api-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse_api-0.2.2.tar", max compression
+gzip compressed data, was "dataverse_api-0.2.3.tar", max compression
```

## Comparing `dataverse_api-0.2.2.tar` & `dataverse_api-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       61 2023-05-12 18:28:06.104392 dataverse_api-0.2.2/dataverse_api/__init__.py
--rw-r--r--   0        0        0    24199 2023-05-30 13:41:54.658389 dataverse_api-0.2.2/dataverse_api/dataverse.py
--rw-r--r--   0        0        0     8295 2023-05-30 13:41:54.659390 dataverse_api-0.2.2/dataverse_api/utils.py
--rw-r--r--   0        0        0     1093 2023-05-12 18:09:25.896155 dataverse_api-0.2.2/LICENSE
--rw-r--r--   0        0        0      801 2023-05-30 14:37:37.603132 dataverse_api-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3977 2023-05-30 13:41:54.655391 dataverse_api-0.2.2/README.md
--rw-r--r--   0        0        0     4528 1970-01-01 00:00:00.000000 dataverse_api-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-05-12 18:28:06.104392 dataverse_api-0.2.3/dataverse_api/__init__.py
+-rw-r--r--   0        0        0    24522 2023-06-02 12:47:02.784360 dataverse_api-0.2.3/dataverse_api/dataverse.py
+-rw-r--r--   0        0        0     9719 2023-06-02 12:46:37.380533 dataverse_api-0.2.3/dataverse_api/utils.py
+-rw-r--r--   0        0        0     1093 2023-05-12 18:09:25.896155 dataverse_api-0.2.3/LICENSE
+-rw-r--r--   0        0        0      801 2023-06-02 12:48:47.990615 dataverse_api-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3977 2023-05-30 13:41:54.655391 dataverse_api-0.2.3/README.md
+-rw-r--r--   0        0        0     4528 1970-01-01 00:00:00.000000 dataverse_api-0.2.3/PKG-INFO
```

### Comparing `dataverse_api-0.2.2/dataverse_api/dataverse.py` & `dataverse_api-0.2.3/dataverse_api/dataverse.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     batch_command,
     batch_id_generator,
     chunk_data,
     convert_data,
     expand_headers,
     extract_batch_response_data,
     extract_key,
+    find_invalid_columns,
     parse_entity_metadata,
 )
 
 log = logging.getLogger()
 logging.basicConfig(level=logging.INFO)
 
 
@@ -380,15 +381,15 @@
           - data: Data that forms the basis for update into Dataverse.
           - key_columns: If validation is not enabled, provide primary column or
             columns that form an alternate key
 
         >>> data={"col1":"abc", "col2":"dac", "col3":69}
         >>> table.update_single_value(data, key_columns={"col1","col2"})
         """
-        key_columns = key_columns or self._validate_payload(data, write_mode=True)
+        key_columns = key_columns or self._validate_payload(data, mode="update")
 
         if key_columns is None and not self._validate:
             raise DataverseError("Key column(s) must be specified.")
 
         data, row_key = extract_key(data=data, key_columns=key_columns)
 
         if len(data) > 1:
@@ -433,15 +434,15 @@
 
         Alternatively, updating different columns per data row:
 
         >>> data=[{"col1":"foo", "col2":2}, {"col1":"bar", "col3":5}]
         >>> table.upsert_single_column(data, key_columns="col1", liberal=True)
         """
         data = convert_data(data)
-        key_columns = key_columns or self._validate_payload(data, write_mode=True)
+        key_columns = key_columns or self._validate_payload(data, mode="update")
 
         if key_columns is None and not self._validate:
             raise DataverseError("Key column(s) must be specified.")
 
         if not all(len(row) == 1 for row in data):
             raise DataverseError(
                 "Only one data column can be passed. Use `upsert` instead."
@@ -479,15 +480,15 @@
             columns that form an alternate key, to ensure data can be inserted.
 
         >>> data={"col1":"abc", "col2":"dac", "col3":69, "col4":"Foo"}
         >>> table.upsert(data, key_columns={"col1","col2"})
         """
         data = convert_data(data)
         # Validation just run to make sure appropriate keys are present
-        self._validate_payload(data, write_mode=True)
+        self._validate_payload(data, mode="create")
 
         log.info(f"Performing insert of {len(data)} elements into {self.schema.name}.")
 
         # Converting to Batch Commands
         batch_data = self._prepare_batch_data(data=data, mode="POST")
 
         self._client.batch_operation(batch_data)
@@ -506,15 +507,15 @@
           - key_columns: If validation is not enabled, provide primary column or
             columns that form an alternate key for identifying rows uniquely.
 
         >>> data={"col1":"abc", "col2":"dac", "col3":69, "col4":"Foo"}
         >>> table.upsert(data, key_columns={"col1","col2"})
         """
         data = convert_data(data)
-        key_columns = key_columns or self._validate_payload(data, write_mode=True)
+        key_columns = key_columns or self._validate_payload(data, mode="upsert")
 
         log.info(f"Performing upsert of {len(data)} elements into {self.schema.name}.")
 
         if key_columns is None and not self._validate:
             raise DataverseError("Key column(s) must be specified.")
 
         batch_data = self._prepare_batch_data(
@@ -565,23 +566,29 @@
                 output.append(DataverseBatchCommand(uri=uri, mode=mode, data=row))
 
         return output
 
     def _validate_payload(
         self,
         data: list[dict],
-        write_mode: Optional[bool] = False,
+        mode: Optional[Literal["insert", "update", "upsert"]] = None,
     ) -> Optional[set[str]]:
         """
         Used to validate write/update/upsert data payload
         against the parsed Entity schema. If validation is set to False,
         it will not return a key or alter the supplied data.
 
         Returns a set of key column(s) to use if succesful.
 
+        Args:
+          - data: The data that will be validated according to Schema.
+          - mode: The optional validation mode parameter that must be set
+            to `"create"` if writing new data to Dataverse and `"update"`
+            if performing updates to Dataverse.
+
         Raises DataverseError if:
           - Column names in payload are not found in schema
           - No key or alternate key can be formed from columns (if write_mode = True)
         """
         if not self._validate:
             log.info("Data validation not performed.")
             return None
@@ -593,53 +600,57 @@
 
         # Getting a set of all columns present in all rows of data
         complete_columns = {k for k in self.schema.columns.keys()}
         for row in data:
             contains_values = {k for k, v in row.items() if v is not None}
             complete_columns = complete_columns.intersection(contains_values)
 
-        data_columns, complete_columns = set(data_columns), set(complete_columns)
-
         # Checking column names against schema
         if not data_columns.issubset(self.schema.columns):
             bad_columns = list(data_columns.difference(self.schema.columns))
             raise DataverseError(
                 (
                     "Found bad payload columns not present "
                     + f"in table schema: {' '.join(bad_columns)}"
                 )
             )
 
-        if not write_mode:
+        if mode is None:
             log.info(
                 "Data validation completed - all columns valid according to schema."
             )
             return None
 
         # Checking for available keys against schema
         if self.schema.key in complete_columns:
-            log.info("Data validation completed. Key column present in all rows.")
-            return set(self.schema.key)
+            log.info("Key column present in all rows, using as key.")
+            key = {self.schema.key}
         elif self.schema.altkeys:
             # Checking if any valid altkeys can be formed from columns
             # Preferring shortest possible altkeys
             for altkey in sorted(self.schema.altkeys, key=len):
                 if altkey.issubset(complete_columns):
                     log.info(
-                        (
-                            "Data validation completed. A consistent"
-                            + " alternate key can be formed from all rows."
-                        )
+                        ("A consistent alternate key can be formed from all rows.")
                     )
-                    return altkey
+                    key = altkey
         else:
             raise DataverseError(
-                "No columns in payload to form primary key or any alternate key."
+                "No columns in payload to form consistent primary or alternate key."
             )
 
+        find_invalid_columns(
+            key_columns=key,
+            data_columns=data_columns,
+            schema_columns=self.schema.columns,
+            mode=mode,
+        )
+
+        return key
+
     def read(self, select: Optional[list[str]] = None, page_size: Optional[int] = None):
         """
         Reads entity.
 
         TODO: Support advanced query params: select, expand, filter, orderby, top
         TODO: Support paging if server responds with
         """
```

### Comparing `dataverse_api-0.2.2/dataverse_api/utils.py` & `dataverse_api-0.2.3/dataverse_api/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import json
+import logging
 from collections.abc import Iterator
 from dataclasses import dataclass
 from textwrap import dedent
-from typing import Any, Optional, Union
+from typing import Any, Literal, Optional, Union
 from uuid import uuid4
 
 import pandas as pd
 
+log = logging.getLogger()
+
 
 @dataclass
 class DataverseBatchCommand:
     uri: str
     mode: str
     data: Optional[dict[str, Any]] = None
 
@@ -158,15 +161,15 @@
       - List of alternate key column combinations as sets.
     """
     keys: list[set] = list()
 
     items: list[dict] = keys_metadata["value"]
     for item in items:
         try:
-            keys.append(set(item["KeyAttributes"]))
+            keys.append(set(item["KeyAttributes"]))  # KeyAttributes is a List
         except KeyError:
             raise DataverseError("Payload does not contain the necessary columns.")
 
     return keys
 
 
 def chunk_data(
@@ -248,15 +251,17 @@
     Returns a tuple with two elements:
       - 0: A modified data dict where any key columns are removed
       - 1: A string that contains the Dataverse specification
         row identifier
     """
     data = data.copy()
     key_elements = []
-    for col in set(key_columns):
+    if type(key_columns) == str:
+        key_columns = {key_columns}
+    for col in key_columns:
         key_value = data.pop(col).__repr__()  # Need repr to capture strings properly
         key_elements.append(f"{col}={key_value}")
     return (data, ",".join(key_elements))
 
 
 def batch_id_generator() -> str:
     """Simply creates a unique string."""
@@ -281,7 +286,45 @@
 
         {row.mode} {api_url}{row.uri} HTTP/1.1
         Content-Type: application/json{'; type=entry' if row.mode=="POST" else""}
 
         {json.dumps(row.data)}
         """
     return dedent(row_command)
+
+
+def find_invalid_columns(
+    key_columns: set[str],
+    data_columns: set[str],
+    schema_columns: dict[str, DataverseColumn],
+    mode: Literal["create", "update", "upsert"],
+):
+    """
+    Simple function to isolate columns passed in data as attributes
+    invalid for passing in create or update.
+
+    Args:
+      - key_columns: Set of key column(s) to be ignored
+      - data_columns: The data columns passed from user
+      - schema_columns: The data columns available in schema
+    """
+    baddies = set()
+    for col in data_columns:
+        if col in key_columns:
+            continue
+
+        create = schema_columns[col].can_create
+        update = schema_columns[col].can_update
+
+        if not create and mode == "create":
+            baddies.add(col)
+        elif not update and mode == "update":
+            baddies.add(col)
+        elif (create ^ update) and mode == "upsert":  # XOR: if only one is true
+            baddies.add(col)
+
+    if baddies and (mode in ["create", "update"]):
+        cols = ", ".join(sorted(baddies))
+        raise DataverseError(f"Found columns not valid for {mode}: {cols}")
+
+    if baddies and mode == "upsert":
+        log.warning(f"Found columns that may throw errors in upsert: {cols}")
```

### Comparing `dataverse_api-0.2.2/LICENSE` & `dataverse_api-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.2.2/pyproject.toml` & `dataverse_api-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataverse-api"
-version = "0.2.2"
+version = "0.2.3"
 description = "Abstraction layer for interacting with Microsoft Dataverse in Python. Supports batch operations!"
 authors = ["Marcus Risanger <69350948+MarcusRisanger@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 msal = "^1.22.0"
```

### Comparing `dataverse_api-0.2.2/README.md` & `dataverse_api-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.2.2/PKG-INFO` & `dataverse_api-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-api
-Version: 0.2.2
+Version: 0.2.3
 Summary: Abstraction layer for interacting with Microsoft Dataverse in Python. Supports batch operations!
 Author: Marcus Risanger
 Author-email: 69350948+MarcusRisanger@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

