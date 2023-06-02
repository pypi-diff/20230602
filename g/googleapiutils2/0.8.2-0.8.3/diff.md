# Comparing `tmp/googleapiutils2-0.8.2.tar.gz` & `tmp/googleapiutils2-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.8.2.tar", max compression
+gzip compressed data, was "googleapiutils2-0.8.3.tar", max compression
```

## Comparing `googleapiutils2-0.8.2.tar` & `googleapiutils2-0.8.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.8.2/LICENSE
--rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.8.2/README.md
--rw-r--r--   0        0        0      119 2023-06-02 03:26:51.461760 googleapiutils2-0.8.2/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.8.2/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.8.2/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.8.2/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.8.2/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-02 03:24:36.559913 googleapiutils2-0.8.2/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.8.2/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.8.2/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     9284 2023-06-02 03:12:44.689458 googleapiutils2-0.8.2/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    32483 2023-06-02 03:13:17.683151 googleapiutils2-0.8.2/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     5211 2023-06-02 00:22:11.187687 googleapiutils2-0.8.2/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     8927 2023-06-02 01:08:13.754688 googleapiutils2-0.8.2/googleapiutils2/utils.py
--rw-r--r--   0        0        0     1067 2023-06-02 03:32:18.471503 googleapiutils2-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.8.3/LICENSE
+-rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.8.3/README.md
+-rw-r--r--   0        0        0      119 2023-06-02 03:26:51.461760 googleapiutils2-0.8.3/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.8.3/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.8.3/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.8.3/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.8.3/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-02 03:24:36.559913 googleapiutils2-0.8.3/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.8.3/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.8.3/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     9284 2023-06-02 03:12:44.689458 googleapiutils2-0.8.3/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    33125 2023-06-02 03:53:11.173456 googleapiutils2-0.8.3/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     5211 2023-06-02 00:22:11.187687 googleapiutils2-0.8.3/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     8927 2023-06-02 01:08:13.754688 googleapiutils2-0.8.3/googleapiutils2/utils.py
+-rw-r--r--   0        0        0     1067 2023-06-02 03:53:56.464685 googleapiutils2-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.8.3/PKG-INFO
```

### Comparing `googleapiutils2-0.8.2/LICENSE` & `googleapiutils2-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.2/README.md` & `googleapiutils2-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.2/googleapiutils2/drive/drive.py` & `googleapiutils2-0.8.3/googleapiutils2/drive/drive.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.2/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.8.3/googleapiutils2/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.2/googleapiutils2/geocode/misc.py` & `googleapiutils2-0.8.3/googleapiutils2/geocode/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.2/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.8.3/googleapiutils2/sheets/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.2/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.8.3/googleapiutils2/sheets/sheets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,98 @@
 from __future__ import annotations
-from collections import defaultdict
 
 import logging
 import operator
 import time
+from collections import defaultdict
 from typing import *
 
 import pandas as pd
 from cachetools import TTLCache, cachedmethod
 from google.oauth2.credentials import Credentials
 from googleapiclient import discovery
 
 from ..utils import THROTTLE_TIME, hex_to_rgb, nested_defaultdict, parse_file_id
 from .misc import (
     DEFAULT_SHEET_NAME,
     DEFAULT_SHEET_SHAPE,
     VERSION,
+    A1_to_slices,
     InsertDataOption,
     SheetSlice,
     SheetSliceT,
     SheetsValues,
     ValueInputOption,
     ValueRenderOption,
     split_sheet_range,
-    A1_to_slices,
 )
 
 if TYPE_CHECKING:
     from googleapiclient._apis.drive.v3.resources import File
     from googleapiclient._apis.sheets.v4.resources import (
         AppendValuesResponse,
         BatchUpdateSpreadsheetRequest,
+        BatchUpdateSpreadsheetResponse,
         BatchUpdateValuesRequest,
         BatchUpdateValuesResponse,
+        CellFormat,
         ClearValuesResponse,
         CopySheetToAnotherSpreadsheetRequest,
+        Request,
         Sheet,
         SheetProperties,
         SheetsResource,
         Spreadsheet,
         SpreadsheetProperties,
+        TextFormat,
         UpdateValuesResponse,
         ValueRange,
-        CellFormat,
-        TextFormat,
     )
 
 logger = logging.getLogger(__name__)
 
 SheetsRange = str | SheetSliceT | Any
 
 
 class Sheets:
     def __init__(self, creds: Credentials, throttle_time: float = THROTTLE_TIME):
         self.creds = creds
         self.service: SheetsResource = discovery.build(  # type: ignore
             "sheets", VERSION, credentials=self.creds
         )
-        self.sheets: SheetsResource.SpreadsheetsResource = self.service.spreadsheets()
+        self.spreadsheets: SheetsResource.SpreadsheetsResource = (
+            self.service.spreadsheets()
+        )
         self.throttle_time = throttle_time
 
         self._cache: TTLCache = TTLCache(maxsize=128, ttl=80)
 
         self._batched_data: DefaultDict[
             str, dict[str | Any, SheetsValues]
         ] = defaultdict(dict)
         self._prev_time: Optional[float] = None
 
+    def batch_update_spreadsheet(
+        self,
+        spreadsheet_id: str,
+        body: BatchUpdateSpreadsheetRequest,
+        **kwargs: Any,
+    ) -> BatchUpdateSpreadsheetResponse:
+        """Executes a batch update spreadsheet request.
+
+        Args:
+            spreadsheet_id (str): The spreadsheet to update.
+            body (BatchUpdateSpreadsheetRequest): The request body.
+            **kwargs: Additional arguments to pass to self.sheets.batchUpdate.
+        """
+        spreadsheet_id = parse_file_id(spreadsheet_id)
+        return self.spreadsheets.batchUpdate(
+            spreadsheetId=spreadsheet_id, body=body, **kwargs
+        ).execute()
+
     def create(
         self,
         title: str,
         sheet_names: list[str] | None = None,
         body: Spreadsheet | None = None,  # type: ignore
     ):
         body: Spreadsheet = nested_defaultdict(body if body else {})  # type: ignore
@@ -78,15 +100,15 @@
 
         body["properties"]["title"] = title  # type: ignore
         for n, sheet_name in enumerate(sheet_names):
             body["sheets"][n]["properties"]["title"] = sheet_name  # type: ignore
 
         body["sheets"] = list(body["sheets"].values())  # type: ignore
 
-        return self.sheets.create(body=body).execute()  # type: ignore
+        return self.spreadsheets.create(body=body).execute()  # type: ignore
 
     def copy_to(
         self,
         from_spreadsheet_id: str,
         from_sheet_id: int,
         to_spreadsheet_id: str,
     ):
@@ -102,29 +124,29 @@
             parse_file_id(to_spreadsheet_id),
         )
         body: CopySheetToAnotherSpreadsheetRequest = {
             "destinationSpreadsheetId": to_spreadsheet_id
         }
 
         return (
-            self.sheets.sheets()
+            self.spreadsheets.sheets()
             .copyTo(  # type: ignore
                 spreadsheetId=from_spreadsheet_id,
                 sheetId=from_sheet_id,
                 body=body,
             )
             .execute()
         )
 
     def get_spreadsheet(
         self,
         spreadsheet_id: str,
     ) -> Spreadsheet:
         spreadsheet_id = parse_file_id(spreadsheet_id)
-        return self.sheets.get(spreadsheetId=spreadsheet_id).execute()
+        return self.spreadsheets.get(spreadsheetId=spreadsheet_id).execute()
 
     def get(
         self,
         spreadsheet_id: str,
         name: str | None = None,
         sheet_id: int | None = None,
     ) -> Sheet:
@@ -169,17 +191,15 @@
                     "updateSheetProperties": {
                         "properties": {"sheetId": sheet_id, "title": new_name},
                         "fields": "title",
                     }
                 }
             ]
         }
-        return self.sheets.batchUpdate(
-            spreadsheetId=spreadsheet_id, body=body
-        ).execute()
+        return self.batch_update_spreadsheet(spreadsheet_id=spreadsheet_id, body=body)
 
     def add(
         self,
         spreadsheet_id: str,
         names: str | list[str],
         rows: int = 1000,
         cols: int = 26,
@@ -218,19 +238,19 @@
                 {
                     "addSheet": make_body(name),
                 }
                 for name in names
             ],
         }
 
-        return self.sheets.batchUpdate(
-            spreadsheetId=spreadsheet_id,
+        return self.batch_update_spreadsheet(
+            spreadsheet_id=spreadsheet_id,
             body=body,
             **kwargs,
-        ).execute()
+        )
 
     def delete(
         self,
         spreadsheet_id: str,
         sheet_id: int,
         **kwargs: Any,
     ):
@@ -247,19 +267,19 @@
                 {
                     "deleteSheet": {
                         "sheetId": sheet_id,
                     },
                 },
             ],
         }
-        return self.sheets.batchUpdate(
-            spreadsheetId=spreadsheet_id,
+        return self.batch_update_spreadsheet(
+            spreadsheet_id=spreadsheet_id,
             body=body,
             **kwargs,
-        ).execute()
+        )
 
     def values(
         self,
         spreadsheet_id: str,
         range_name: SheetsRange = DEFAULT_SHEET_NAME,
         value_render_option: ValueRenderOption = ValueRenderOption.unformatted,
         **kwargs: Any,
@@ -270,15 +290,15 @@
             spreadsheet_id (str): The spreadsheet ID.
             range_name (SheetsRange, optional): The range to get values from. Defaults to DEFAULT_SHEET_NAME.
             value_render_option (ValueRenderOption, optional): The value render option. Defaults to ValueRenderOption.unformatted.
         """
         spreadsheet_id = parse_file_id(spreadsheet_id)
         range_name = str(range_name)
         return (
-            self.sheets.values()
+            self.spreadsheets.values()
             .get(
                 spreadsheetId=spreadsheet_id,
                 range=range_name,
                 valueRenderOption=value_render_option.value,
                 **kwargs,
             )
             .execute()
@@ -377,15 +397,15 @@
         spreadsheet_id = parse_file_id(spreadsheet_id)
         range_name = str(range_name)
         values = self._process_sheets_values(
             spreadsheet_id, range_name, values, align_columns
         )
 
         return (
-            self.sheets.values()
+            self.spreadsheets.values()
             .update(
                 spreadsheetId=spreadsheet_id,
                 range=range_name,
                 body={"values": values},  # type: ignore
                 valueInputOption=value_input_option.value,
             )
             .execute()
@@ -413,15 +433,15 @@
         ]
 
         body: BatchUpdateValuesRequest = {
             "valueInputOption": value_input_option.value,
             "data": new_data,
         }
         return (
-            self.sheets.values()
+            self.spreadsheets.values()
             .batchUpdate(
                 spreadsheetId=spreadsheet_id,
                 body=body,
             )
             .execute()
         )
 
@@ -526,15 +546,15 @@
                 range_name=range_name,
                 values=values,
                 align_columns=align_columns,
             )
         }
 
         return (
-            self.sheets.values()
+            self.spreadsheets.values()
             .append(
                 spreadsheetId=spreadsheet_id,
                 range=range_name,
                 body=body,
                 insertDataOption=insert_data_option.value,
                 valueInputOption=value_input_option.value,
             )
@@ -552,15 +572,15 @@
             spreadsheet_id (str): The spreadsheet to update.
             range_name (SheetsRange): The range to clear.
         """
         spreadsheet_id = parse_file_id(spreadsheet_id)
         range_name = str(range_name)
 
         return (
-            self.sheets.values()
+            self.spreadsheets.values()
             .clear(spreadsheetId=spreadsheet_id, range=range_name)
             .execute()
         )
 
     def resize(
         self,
         spreadsheet_id: str,
@@ -591,17 +611,15 @@
                             },
                         },
                         "fields": "gridProperties.rowCount,gridProperties.columnCount",
                     }
                 }
             ]
         }
-        return self.sheets.batchUpdate(
-            spreadsheetId=spreadsheet_id, body=body
-        ).execute()
+        return self.batch_update_spreadsheet(spreadsheet_id=spreadsheet_id, body=body)
 
     def clear_formatting(self, spreadsheet_id: str, sheet_name: str):
         """Clears all formatting from a sheet.
 
         Args:
             spreadsheet_id (str): The spreadsheet to update.
             sheet_name (str): The name of the sheet to clear formatting from.
@@ -617,17 +635,15 @@
                             "sheetId": sheet_id,
                         },
                         "fields": "userEnteredFormat",
                     }
                 }
             ]
         }
-        return self.sheets.batchUpdate(
-            spreadsheetId=spreadsheet_id, body=body
-        ).execute()
+        return self.batch_update_spreadsheet(spreadsheet_id=spreadsheet_id, body=body)
 
     def reset_sheet(
         self,
         spreadsheet_id: str,
         sheet_name: str,
     ):
         """Resets a sheet back to a default state. This includes clearing all values and formatting.
@@ -646,15 +662,15 @@
     def _create_format_body(
         sheet_id: int,
         start_row: int,
         start_col: int,
         cell_format: CellFormat,
         end_row: int | None = None,
         end_col: int | None = None,
-    ) -> BatchUpdateSpreadsheetRequest:
+    ) -> Request:
         """Creates a batch update request body for formatting a range of cells.
         The ranges herein are 1-indexed.
 
         Args:
             sheet_id (int): The ID of the sheet to format.
             start_row (int): The starting row of the range to format.
             start_col (int): The starting column of the range to format.
@@ -662,31 +678,27 @@
             end_row (int, optional): The ending row of the range to format. Defaults to None.
             end_col (int, optional): The ending column of the range to format. Defaults to None.
         """
         end_row = end_row if end_row is not None else start_row + 1
         end_col = end_col if end_col is not None else start_col + 1
 
         return {
-            "requests": [
-                {
-                    "repeatCell": {
-                        "range": {
-                            "sheetId": sheet_id,
-                            "startRowIndex": start_row - 1,
-                            "endRowIndex": end_row,
-                            "startColumnIndex": start_col - 1,
-                            "endColumnIndex": end_col,
-                        },
-                        "cell": {
-                            "userEnteredFormat": cell_format,
-                        },
-                        "fields": f"userEnteredFormat",
-                    }
-                }
-            ]
+            "repeatCell": {
+                "range": {
+                    "sheetId": sheet_id,
+                    "startRowIndex": start_row - 1,
+                    "endRowIndex": end_row,
+                    "startColumnIndex": start_col - 1,
+                    "endColumnIndex": end_col,
+                },
+                "cell": {
+                    "userEnteredFormat": cell_format,
+                },
+                "fields": f"userEnteredFormat",
+            }
         }
 
     @staticmethod
     def _create_cell_format(
         bold: bool | None = None,
         italic: bool | None = None,
         underline: bool | None = None,
@@ -763,26 +775,27 @@
         shape = (
             properties["gridProperties"]["rowCount"],
             properties["gridProperties"]["columnCount"],
         )
 
         row_slc, col_slc = A1_to_slices(range_name, shape=shape)
 
-        body = self._create_format_body(
-            sheet_id,
-            start_row=row_slc.start,
-            end_row=row_slc.stop,
-            start_col=col_slc.start,
-            end_col=col_slc.stop,
-            cell_format=cell_format,
-        )
-
-        return self.sheets.batchUpdate(
-            spreadsheetId=spreadsheet_id, body=body
-        ).execute()
+        body: BatchUpdateSpreadsheetRequest = {
+            "requests": [
+                self._create_format_body(
+                    sheet_id,
+                    start_row=row_slc.start,
+                    end_row=row_slc.stop,
+                    start_col=col_slc.start,
+                    end_col=col_slc.stop,
+                    cell_format=cell_format,
+                )
+            ]
+        }
+        return self.batch_update_spreadsheet(spreadsheet_id=spreadsheet_id, body=body)
 
     @staticmethod
     def to_frame(values: ValueRange, **kwargs: Any) -> pd.DataFrame | None:
         """Converts a ValueRange to a DataFrame.
 
         Useful for working with the data in Pandas after a call to sheets.values().
         If one of the keyword arguments to the dataframe is "columns",
```

### Comparing `googleapiutils2-0.8.2/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.8.3/googleapiutils2/sheets/sheets_value_range.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.2/googleapiutils2/utils.py` & `googleapiutils2-0.8.3/googleapiutils2/utils.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.2/pyproject.toml` & `googleapiutils2-0.8.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.8.2"
+version = "0.8.3"
 description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 
 readme = "README.md"
 keywords = ["google", "googleapi", "googleapiutils2"]
 license = "MIT"
 repository = "https://github.com/mkbabb/googleapiutils2"
```

### Comparing `googleapiutils2-0.8.2/PKG-INFO` & `googleapiutils2-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleapiutils2
-Version: 0.8.2
+Version: 0.8.3
 Summary: Wrapper for Google's Python API.
 Home-page: https://github.com/mkbabb/googleapiutils2
 License: MIT
 Keywords: google,googleapi,googleapiutils2
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
```

