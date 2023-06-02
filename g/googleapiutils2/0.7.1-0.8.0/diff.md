# Comparing `tmp/googleapiutils2-0.7.1.tar.gz` & `tmp/googleapiutils2-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.7.1.tar", max compression
+gzip compressed data, was "googleapiutils2-0.8.0.tar", max compression
```

## Comparing `googleapiutils2-0.7.1.tar` & `googleapiutils2-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.7.1/LICENSE
--rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.7.1/README.md
--rw-r--r--   0        0        0       96 2023-06-01 17:02:06.802855 googleapiutils2-0.7.1/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.7.1/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.7.1/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.7.1/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.7.1/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1084 2023-06-01 21:02:11.670817 googleapiutils2-0.7.1/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.7.1/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.7.1/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     7442 2023-06-01 21:03:07.412995 googleapiutils2-0.7.1/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    24151 2023-06-01 20:48:26.565632 googleapiutils2-0.7.1/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     5310 2023-06-01 18:17:35.266727 googleapiutils2-0.7.1/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     7497 2023-06-01 20:46:27.789563 googleapiutils2-0.7.1/googleapiutils2/utils.py
--rw-r--r--   0        0        0     1067 2023-06-01 21:03:20.344173 googleapiutils2-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.8.0/LICENSE
+-rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.8.0/README.md
+-rw-r--r--   0        0        0       96 2023-06-01 17:02:06.802855 googleapiutils2-0.8.0/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.8.0/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.8.0/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.8.0/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.8.0/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1084 2023-06-01 21:02:11.670817 googleapiutils2-0.8.0/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.8.0/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.8.0/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     9284 2023-06-02 03:12:44.689458 googleapiutils2-0.8.0/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    32483 2023-06-02 03:13:17.683151 googleapiutils2-0.8.0/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     5211 2023-06-02 00:22:11.187687 googleapiutils2-0.8.0/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     8927 2023-06-02 01:08:13.754688 googleapiutils2-0.8.0/googleapiutils2/utils.py
+-rw-r--r--   0        0        0     1067 2023-06-02 03:17:33.664572 googleapiutils2-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.8.0/PKG-INFO
```

### Comparing `googleapiutils2-0.7.1/LICENSE` & `googleapiutils2-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.7.1/README.md` & `googleapiutils2-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.7.1/googleapiutils2/drive/drive.py` & `googleapiutils2-0.8.0/googleapiutils2/drive/drive.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.7.1/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.8.0/googleapiutils2/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.7.1/googleapiutils2/geocode/misc.py` & `googleapiutils2-0.8.0/googleapiutils2/geocode/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.7.1/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.8.0/googleapiutils2/sheets/misc.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 VERSION = "v4"
 
 DEFAULT_SHEET_NAME = "Sheet1"
 
 DEFAULT_SHEET_SHAPE = (1000, 26)
 
+BASE = 26
+OFFSET = 1
+
 SheetsValues = list[list[Any]] | list[dict[str | Any, Any]]
 
 
 class ValueInputOption(Enum):
     """How the input data should be interpreted."""
 
     # The values the user has entered will not be parsed and will be stored as-is.
@@ -47,147 +50,178 @@
     # Rows are overwritten with the new data.
     overwrite = "OVERWRITE"
 
 
 def format_range_name(
     sheet_name: str | None = None, range_name: str | None = None
 ) -> str:
-    """Format a range name for use in a Google Sheets API request."""
+    """Format a range name for use in a Google Sheets API request.
+    Quotes sheet names if they're not already quoted.
 
+    Args:
+        sheet_name (str | None): The name of the sheet.
+        range_name (str | None): The range name.
+    """
     if sheet_name is not None and range_name is not None:
         if not (sheet_name.startswith("'") and sheet_name.endswith("'")):
             sheet_name = f"'{sheet_name}'"
         return f"{sheet_name}!{range_name}"
     elif range_name is not None:
         return range_name
     elif sheet_name is not None:
         return sheet_name
     else:
         return ""
 
 
-BASE = 26
-OFFSET = 1
-
-
 def int_to_A1(i: int) -> str:
     nums = to_base(i - OFFSET, base=BASE)
     return "".join(map(lambda x: string.ascii_letters[x].upper(), nums))
 
 
 def rc_to_A1(row: int, col: int) -> str:
     t_col = int_to_A1(col) if col is not ... else ""
     t_row = str(row) if row is not ... else ""
-
     return f"{t_col}{t_row}"
 
 
-def A1_to_rc(a1: str | int) -> tuple[int, int | None]:
-    finder = lambda x: string.ascii_letters.find(x) + OFFSET
+def A1_to_int(a1: str) -> int:
+    base = len(
+        string.ascii_uppercase
+    )  # The base for this operation is 26 (letters in the alphabet)
+    a1 = a1.upper()
+    result = 0
+    for i, c in enumerate(a1[::-1]):
+        result += (string.ascii_uppercase.index(c) + 1) * (base**i)
+    return result
 
-    if isinstance(a1, int) or a1 is ...:
-        return a1, None
 
-    a1 = a1.lower()
-    if ":" in a1:
-        row, col = a1.split(":")
-        return finder(row), finder(col)
-    else:
-        new_row = finder(a1)
-        return new_row, new_row
+def A1_to_rc(a1: str) -> tuple[int | None, int | None]:
+    col_part = "".join(filter(str.isalpha, a1))
+    row_part = "".join(filter(str.isdigit, a1))
 
+    col = A1_to_int(col_part) if col_part else None  # return None if no column part
+    row = int(row_part) if row_part else None  # return None if no row part
 
-def slices_to_A1(row_ix: slice, col_ix: slice) -> tuple[str, str]:
-    return (
-        rc_to_A1(row_ix.start, col_ix.start),
-        rc_to_A1(row_ix.stop, col_ix.stop),
-    )
+    return row, col
 
 
-def normalize_ix(ix: slice, length: int) -> slice:
-    handle_negative = lambda x: x + length + 1 if isinstance(x, int) and x < 0 else x
-    handle_str = lambda x: A1_to_rc(x)[0] if isinstance(x, str) else x
+def split_sheet_range(range_name: Any) -> tuple[str, str]:
+    range_name = str(range_name)
 
-    start, stop = ix.start, ix.stop
+    if "!" in range_name:
+        sheet_name, range_name = range_name.split("!")
+        return sheet_name, range_name
 
-    start, stop = handle_str(start), handle_str(stop)
+    if ":" in range_name:
+        return DEFAULT_SHEET_NAME, range_name
+    else:
+        return range_name, ""
 
-    none_stop = start is not None and stop is None
-    ellipsis_stop = stop is ... and not start is ...
 
-    if none_stop or ellipsis_stop:
-        stop = length
+def A1_to_slices(
+    a1: str, shape: tuple[int, int] = DEFAULT_SHEET_SHAPE
+) -> tuple[slice, slice]:
+    # Parse sheet and range
+    _, range_name = split_sheet_range(a1)
+
+    if not range_name:  # The entire sheet is the range
+        return slice(1, shape[0]), slice(1, shape[1])
+
+    if ":" in range_name:  # Range is specified
+        start_a1, end_a1 = range_name.split(":")
+    else:  # Only a single cell is specified
+        start_a1, end_a1 = range_name, range_name
+
+    # Convert A1 notation to row and column indices
+    start_row, start_col = A1_to_rc(start_a1)
+    end_row, end_col = A1_to_rc(end_a1)
+
+    # If start indices are not specified, set them to 1
+    start_row = start_row if start_row is not None and start_row is not ... else 1
+    start_col = start_col if start_col is not None else 1
+
+    # If end indices are not specified, set them to the maximum row/column
+    end_row = end_row if end_row is not None else shape[0]
+    end_col = end_col if end_col is not None else shape[1]
 
-    start, stop = handle_negative(start), handle_negative(stop)
+    return slice(start_row, end_row), slice(start_col, end_col)
 
-    return slice(start, stop, ix.step)
 
+def slices_to_A1(row_ix: slice, col_ix: slice) -> tuple[str, str]:
+    return (
+        rc_to_A1(row_ix.start, col_ix.start),
+        rc_to_A1(row_ix.stop, col_ix.stop),
+    )
 
-def to_slice(
-    *slices: slice | int | EllipsisType, shape: tuple[int, ...] | None = None
-) -> tuple[slice, ...]:
-    def inner(ix: slice | int | EllipsisType) -> slice:
+
+def expand_slices(
+    row_ix: slice | int | EllipsisType,
+    col_ix: slice | int | EllipsisType,
+    shape: tuple[int, int] = DEFAULT_SHEET_SHAPE,
+) -> str | None:
+    # TODO! optimize row ellipsis and col ellipsis types
+    # TODO! like 1:1, B:B, etc.
+
+    def to_slice(ix: slice | int) -> slice:
         if isinstance(ix, slice):
             return ix
+        elif isinstance(ix, str):
+            ix = A1_to_int(ix)
+            return slice(ix, ix)
         elif isinstance(ix, int):
             return slice(ix, ix)
-        elif isinstance(ix, str):
-            return slice(*A1_to_rc(ix))
         elif ix is ...:
             return slice(..., ...)
         else:
-            raise TypeError(f"Invalid type: {type(ix)}")
-
-    ixs = map(inner, slices)
-
-    if shape is None:
-        return tuple(ixs)
+            raise TypeError("Indices must be slices or integers.")
 
-    return tuple((normalize_ix(ix, shape[n]) for n, ix in enumerate(ixs)))
-
-
-def expand_slices(
-    row_ix: slice | int, col_ix: slice | int, shape: tuple[int, int] | None
-) -> list[str | None]:
-    row_ix, col_ix = to_slice(row_ix, col_ix, shape=shape)
-    row_ix, col_ix = slices_to_A1(row_ix, col_ix)
-    range_name = f"{row_ix}:{col_ix}" if row_ix != "" and col_ix != "" else None
+    def normalize_ix(slc: slice, max_dim: int) -> slice:
+        start, stop, step = slc.start, slc.stop, slc.step
+        # handle None
+        start = 1 if start is None else start
+        stop = max_dim if stop is None else stop
+        # check if A1 notation is used
+        start = A1_to_int(start) if isinstance(start, str) else start
+        stop = A1_to_int(stop) if isinstance(stop, str) else stop
+        # handle ellipsis
+        start = 1 if start is ... else start
+        stop = max_dim if stop is ... else stop
+        # handle negative indices
+        start = max_dim + start if start < 0 else start
+        stop = max_dim + stop if stop < 0 else stop
+        return slice(start, stop, step)
+
+    row_ix, col_ix = to_slice(row_ix), to_slice(col_ix)  # type: ignore
+    row_ix, col_ix = normalize_ix(row_ix, shape[0]), normalize_ix(col_ix, shape[1])  # type: ignore
+    row_ix, col_ix = slices_to_A1(row_ix, col_ix)  # type: ignore
 
-    return range_name
+    return f"{row_ix}:{col_ix}" if row_ix != "" and col_ix != "" else None  # type: ignore
 
 
-def parse_sheets_ixs(
-    ixs: str | tuple[Any, ...], shape: tuple[int, int] | None
+def parse_sheet_slice_ixs(
+    ixs: str | tuple[Any, ...], shape: tuple[int, int] = DEFAULT_SHEET_SHAPE
 ) -> tuple[str | None, str | None]:
     match ixs:
+        # sheet name and a string range
         case str(sheet_name), str(range_name):
             return sheet_name, range_name
+        # only a sheet name
         case str(sheet_name):
             return sheet_name, None
+        # sheet name name, row, and column indices
         case str(sheet_name), row_ix, col_ix:
             return sheet_name, expand_slices(row_ix, col_ix, shape=shape)
+        # row and column indices
         case row_ix, col_ix:
             return None, expand_slices(row_ix, col_ix, shape=shape)
         case _:
             raise IndexError(f"Invalid index: {ixs}")
 
 
-def reverse_sheet_range(range_name: Any) -> tuple[str, str]:
-    range_name = str(range_name)
-
-    if "!" in range_name:
-        sheet_name, range_name = range_name.split("!")
-        return sheet_name, range_name
-
-    if ":" in range_name:
-        return DEFAULT_SHEET_NAME, range_name
-    else:
-        return range_name, ""
-
-
 @dataclass(frozen=True)
 class SheetSliceT:
     """For better indexing of a Sheet-like object, e.g. a Google Sheet.
     Allows you to index into a sheet using numpy-like syntax.
 
     The forms a slice index can take are:
         SheetSlice[sheet_name, row_ix, col_ix]
@@ -230,15 +264,15 @@
 
     def __getitem__(self, ixs: str | tuple[Any, ...]) -> SheetSliceT:
         if isinstance(ixs, SheetSliceT):
             return ixs
         if isinstance(ixs, tuple) and not len(ixs):
             raise IndexError("Empty index")
 
-        sheet_name, range_name = parse_sheets_ixs(ixs, shape=self.shape)
+        sheet_name, range_name = parse_sheet_slice_ixs(ixs, shape=self.shape)
         return SheetSliceT(
             sheet_name if sheet_name is not None else self.sheet_name,
             range_name if range_name is not None else self.range_name,
             self.shape,
         )
```

### Comparing `googleapiutils2-0.7.1/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.8.0/googleapiutils2/sheets/sheets.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 from typing import *
 
 import pandas as pd
 from cachetools import TTLCache, cachedmethod
 from google.oauth2.credentials import Credentials
 from googleapiclient import discovery
 
-from ..utils import THROTTLE_TIME, nested_defaultdict, parse_file_id
+from ..utils import THROTTLE_TIME, hex_to_rgb, nested_defaultdict, parse_file_id
 from .misc import (
     DEFAULT_SHEET_NAME,
+    DEFAULT_SHEET_SHAPE,
     VERSION,
     InsertDataOption,
     SheetSlice,
     SheetSliceT,
     SheetsValues,
     ValueInputOption,
     ValueRenderOption,
-    reverse_sheet_range,
+    split_sheet_range,
+    A1_to_slices,
 )
 
 if TYPE_CHECKING:
     from googleapiclient._apis.drive.v3.resources import File
     from googleapiclient._apis.sheets.v4.resources import (
         AppendValuesResponse,
         BatchUpdateSpreadsheetRequest,
@@ -36,14 +38,16 @@
         Sheet,
         SheetProperties,
         SheetsResource,
         Spreadsheet,
         SpreadsheetProperties,
         UpdateValuesResponse,
         ValueRange,
+        CellFormat,
+        TextFormat,
     )
 
 logger = logging.getLogger(__name__)
 
 SheetsRange = str | SheetSliceT | Any
 
 
@@ -119,32 +123,35 @@
         return self.sheets.get(spreadsheetId=spreadsheet_id).execute()
 
     def get(
         self,
         spreadsheet_id: str,
         name: str | None = None,
         sheet_id: int | None = None,
-    ) -> Sheet | None:
+    ) -> Sheet:
         """Get a sheet from a spreadsheet. Either the name or the ID of the sheet must be provided.
 
         Args:
             spreadsheet_id (str): The ID of the spreadsheet containing the sheet to get.
             name (str, optional): The name of the sheet to get. Defaults to None.
             sheet_id (int, optional): The ID of the sheet to get. Defaults to None.
         """
         spreadsheet_id = parse_file_id(spreadsheet_id)
         spreadsheet = self.get_spreadsheet(spreadsheet_id)
 
+        if name is not None and name.startswith("'") and name.endswith("'"):
+            name = name[1:-1]
+
         for sheet in spreadsheet["sheets"]:
             if sheet_id is not None and sheet["properties"]["sheetId"] == sheet_id:
                 return sheet
             if name is not None and sheet["properties"]["title"] == name:
                 return sheet
 
-        return None
+        raise ValueError(f"Sheet {name or sheet_id} not found in spreadsheet.")
 
     def rename(
         self,
         spreadsheet_id: str,
         sheet_id: int,
         new_name: str,
     ):
@@ -302,27 +309,27 @@
             rows (list[dict[SheetsRange, Any]]): The rows to update.
             align_columns (bool, optional): Whether to align the columns with the header. Defaults to True.
         """
         if not align_columns:
             logger.debug("align_columns is False, skipping column alignment")
             return [list(row.values()) for row in rows]
 
-        sheet_name, _ = reverse_sheet_range(range_name)
+        sheet_name, _ = split_sheet_range(range_name)
         header = self._header(spreadsheet_id, sheet_name)
         header = pd.Index(header).astype(str)
 
         frame = pd.DataFrame(rows)
         frame = frame.reindex(
             list(rows[0].keys()), axis=1
         )  # preserve the insertion order
         frame.index = frame.index.astype(str)
 
         if len(diff := frame.columns.difference(header)):
             header = header.append(diff)
-            sheet_name, _ = reverse_sheet_range(range_name)
+            sheet_name, _ = split_sheet_range(range_name)
             self.update(
                 spreadsheet_id,
                 SheetSlice[sheet_name, 1, ...],
                 [header.tolist()],
             )
             self._cache[(spreadsheet_id, sheet_name)] = list(header)
 
@@ -550,14 +557,233 @@
 
         return (
             self.sheets.values()
             .clear(spreadsheetId=spreadsheet_id, range=range_name)
             .execute()
         )
 
+    def resize(
+        self,
+        spreadsheet_id: str,
+        sheet_name: str,
+        rows: int = DEFAULT_SHEET_SHAPE[0],
+        cols: int = DEFAULT_SHEET_SHAPE[1],
+    ):
+        """Resizes a sheet to the given number of rows and columns.
+
+        Args:
+            spreadsheet_id (str): The spreadsheet to update.
+            sheet_name (str): The name of the sheet to resize.
+            rows (int, optional): The number of rows to resize to. Defaults to DEFAULT_SHEET_SHAPE[0].
+            cols (int, optional): The number of columns to resize to. Defaults to DEFAULT_SHEET_SHAPE[1].
+        """
+        spreadsheet_id = parse_file_id(spreadsheet_id)
+
+        sheet_id = self.get(spreadsheet_id, name=sheet_name)["properties"]["sheetId"]
+        body: BatchUpdateSpreadsheetRequest = {
+            "requests": [
+                {
+                    "updateSheetProperties": {
+                        "properties": {
+                            "sheetId": sheet_id,
+                            "gridProperties": {
+                                "rowCount": rows,
+                                "columnCount": cols,
+                            },
+                        },
+                        "fields": "gridProperties.rowCount,gridProperties.columnCount",
+                    }
+                }
+            ]
+        }
+        return self.sheets.batchUpdate(
+            spreadsheetId=spreadsheet_id, body=body
+        ).execute()
+
+    def clear_formatting(self, spreadsheet_id: str, sheet_name: str):
+        """Clears all formatting from a sheet.
+
+        Args:
+            spreadsheet_id (str): The spreadsheet to update.
+            sheet_name (str): The name of the sheet to clear formatting from.
+        """
+        spreadsheet_id = parse_file_id(spreadsheet_id)
+
+        sheet_id = self.get(spreadsheet_id, name=sheet_name)["properties"]["sheetId"]
+        body: BatchUpdateSpreadsheetRequest = {
+            "requests": [
+                {
+                    "updateCells": {
+                        "range": {
+                            "sheetId": sheet_id,
+                        },
+                        "fields": "userEnteredFormat",
+                    }
+                }
+            ]
+        }
+        return self.sheets.batchUpdate(
+            spreadsheetId=spreadsheet_id, body=body
+        ).execute()
+
+    def reset_sheet(
+        self,
+        spreadsheet_id: str,
+        sheet_name: str,
+    ):
+        """Resets a sheet back to a default state. This includes clearing all values and formatting.
+
+        Args:
+            spreadsheet_id (str): The spreadsheet to update.
+            sheet_name (str): The name of the sheet to reset.
+        """
+        # first clear all of the values, and set the bounds of the sheet to have 26 columns, and 1000 rows
+        self.clear(spreadsheet_id, sheet_name)
+        self.resize(spreadsheet_id, sheet_name, rows=1000, cols=26)
+        # then clear all of the formatting
+        self.clear_formatting(spreadsheet_id, sheet_name)
+
+    @staticmethod
+    def _create_format_body(
+        sheet_id: int,
+        start_row: int,
+        start_col: int,
+        cell_format: CellFormat,
+        end_row: int | None = None,
+        end_col: int | None = None,
+    ) -> BatchUpdateSpreadsheetRequest:
+        """Creates a batch update request body for formatting a range of cells.
+        The ranges herein are 1-indexed.
+
+        Args:
+            sheet_id (int): The ID of the sheet to format.
+            start_row (int): The starting row of the range to format.
+            start_col (int): The starting column of the range to format.
+            cell_format (CellFormat): The format to apply to the range.
+            end_row (int, optional): The ending row of the range to format. Defaults to None.
+            end_col (int, optional): The ending column of the range to format. Defaults to None.
+        """
+        end_row = end_row if end_row is not None else start_row + 1
+        end_col = end_col if end_col is not None else start_col + 1
+
+        return {
+            "requests": [
+                {
+                    "repeatCell": {
+                        "range": {
+                            "sheetId": sheet_id,
+                            "startRowIndex": start_row - 1,
+                            "endRowIndex": end_row,
+                            "startColumnIndex": start_col - 1,
+                            "endColumnIndex": end_col,
+                        },
+                        "cell": {
+                            "userEnteredFormat": cell_format,
+                        },
+                        "fields": f"userEnteredFormat",
+                    }
+                }
+            ]
+        }
+
+    @staticmethod
+    def _create_cell_format(
+        bold: bool | None = None,
+        italic: bool | None = None,
+        underline: bool | None = None,
+        strikethrough: bool | None = None,
+        font_size: int | None = None,
+        font_family: str | None = None,
+        text_color: str | None = None,
+        background_color: str | None = None,
+        cell_format: CellFormat | None = None,
+    ) -> CellFormat:
+        text_format: TextFormat = {}
+        if bold is not None:
+            text_format["bold"] = bold
+        if italic is not None:
+            text_format["italic"] = italic
+        if underline is not None:
+            text_format["underline"] = underline
+        if strikethrough is not None:
+            text_format["strikethrough"] = strikethrough
+        if font_size is not None:
+            text_format["fontSize"] = font_size
+        if font_family is not None:
+            text_format["fontFamily"] = font_family
+        if text_color is not None:
+            text_format["foregroundColor"] = hex_to_rgb(text_color)
+
+        cell_format_dict: CellFormat = {}
+        if background_color is not None:
+            cell_format_dict["backgroundColor"] = hex_to_rgb(background_color)
+        if cell_format is not None:
+            cell_format_dict.update(cell_format)
+
+        return {"textFormat": text_format, **cell_format_dict}  # type: ignore
+
+    def format(
+        self,
+        spreadsheet_id: str,
+        range_name: SheetsRange,
+        bold: bool | None = None,
+        italic: bool | None = None,
+        underline: bool | None = None,
+        strikethrough: bool | None = None,
+        font_size: int | None = None,
+        font_family: str | None = None,
+        text_color: str | None = None,
+        background_color: str | None = None,
+        cell_format: CellFormat | None = None,
+    ):
+        """Formats a range of cells in a spreadsheet.
+
+        Args:
+            spreadsheet_id (str): The spreadsheet to update.
+            range_name (str): The range to format.
+            ...
+            cell_format (CellFormat, optional): A cell format to merge with the default format. Defaults to None.
+        """
+        spreadsheet_id = parse_file_id(spreadsheet_id)
+        cell_format = self._create_cell_format(
+            bold=bold,
+            italic=italic,
+            underline=underline,
+            strikethrough=strikethrough,
+            font_size=font_size,
+            font_family=font_family,
+            text_color=text_color,
+            background_color=background_color,
+            cell_format=cell_format,
+        )
+
+        sheet_name, range_name = split_sheet_range(str(range_name))  # type: ignore
+
+        properties = self.get(spreadsheet_id, sheet_name)["properties"]
+        sheet_id = properties["sheetId"]
+        shape = (
+            properties["gridProperties"]["rowCount"],
+            properties["gridProperties"]["columnCount"],
+        )
+
+        row_slc, col_slc = A1_to_slices(range_name, shape=shape)
+
+        body = self._create_format_body(
+            sheet_id,
+            start_row=row_slc.start,
+            end_row=row_slc.stop,
+            start_col=col_slc.start,
+            end_col=col_slc.stop,
+            cell_format=cell_format,
+        )
+
+        return self.sheets.batchUpdate(
+            spreadsheetId=spreadsheet_id, body=body
+        ).execute()
+
     @staticmethod
     def to_frame(values: ValueRange, **kwargs: Any) -> pd.DataFrame | None:
         """Converts a ValueRange to a DataFrame.
 
         Useful for working with the data in Pandas after a call to sheets.values().
         If one of the keyword arguments to the dataframe is "columns",
         the first row of the values will be used as the column names, aligned to the data.
```

### Comparing `googleapiutils2-0.7.1/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.8.0/googleapiutils2/sheets/sheets_value_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,22 +68,21 @@
     def header(self) -> list[str]:
         return self.sheets._header(
             spreadsheet_id=self.spreadsheet_id, sheet_name=self.sheet_name
         )
 
     @cachedmethod(operator.attrgetter("_cache"))
     def shape(self) -> tuple[int, int]:
-        for sheet in self.sheets.get_spreadsheet(self.spreadsheet_id).get("sheets", []):
-            properties = sheet.get("properties", {})
-            if properties.get("title") == self.sheet_name:
-                grid_properties = properties.get("gridProperties", {})
-                return (
-                    grid_properties.get("rowCount", 0),
-                    grid_properties.get("columnCount", 0),
-                )
+        sheet = self.sheets.get(self.spreadsheet_id, name=self.sheet_name)
+        if sheet is not None:
+            grid_properties = sheet.get("properties", {}).get("gridProperties", {})
+            return (
+                grid_properties.get("rowCount", 0),
+                grid_properties.get("columnCount", 0),
+            )
         return DEFAULT_SHEET_SHAPE
 
     @cachedmethod(operator.attrgetter("_cache"))
     def sheet_id(self) -> int:
         for sheet in self.sheets.get_spreadsheet(self.spreadsheet_id).get("sheets", []):
             properties = sheet.get("properties", {})
             if properties.get("title") == self.sheet_name:
```

### Comparing `googleapiutils2-0.7.1/googleapiutils2/utils.py` & `googleapiutils2-0.8.0/googleapiutils2/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 
 FilePath = str | Path
 
 if TYPE_CHECKING:
     from googleapiclient._apis.drive.v3.resources import File
-    from googleapiclient._apis.sheets.v4.resources import Spreadsheet
+    from googleapiclient._apis.sheets.v4.resources import Spreadsheet, Color
 
 
 THROTTLE_TIME = 30
 
 SCOPES = [
     "https://www.googleapis.com/auth/spreadsheets",
     "https://www.googleapis.com/auth/drive.file",
@@ -34,14 +34,38 @@
 
 
 TOKEN_PATH = "auth/token.pickle"
 CONFIG_PATH = "auth/credentials.json"
 
 
 class GoogleMimeTypes(Enum):
+    """Enum representing the MIME types used by Google Drive API.
+
+    Each member of this enum represents a MIME type used by Google Drive API.
+    These MIME types are used to identify the type of a file or folder in Google Drive.
+
+    Attributes:
+        audio (str): MIME type for audio files.
+        docs (str): MIME type for Google Docs files.
+        drive_sdk (str): MIME type for Google Drive SDK files.
+        drawing (str): MIME type for Google Drawings files.
+        file (str): MIME type for generic files.
+        folder (str): MIME type for folders.
+        form (str): MIME type for Google Forms files.
+        fusiontable (str): MIME type for Google Fusion Tables files.
+        jam (str): MIME type for Google Jamboard files.
+        map (str): MIME type for Google My Maps files.
+        photo (str): MIME type for Google Photos files.
+        slides (str): MIME type for Google Slides files.
+        script (str): MIME type for Google Apps Script files.
+        shortcut (str): MIME type for Google Drive shortcut files.
+        site (str): MIME type for Google Sites files.
+        sheets (str): MIME type for Google Sheets files.
+    """
+
     audio = "application/vnd.google-apps.audio"
     docs = "application/vnd.google-apps.document"
     drive_sdk = "application/vnd.google-apps.drive-sdk"
     drawing = "application/vnd.google-apps.drawing"
     file = "application/vnd.google-apps.file"
     folder = "application/vnd.google-apps.folder"
     form = "application/vnd.google-apps.form"
@@ -86,14 +110,24 @@
     cab = "application/cab"
     php = "application/x-httpd-php"
     json = "application/vnd.google-apps.script+json"
 
     default = "application/octet-stream"
 
 
+def hex_to_rgb(hex_code: str) -> Color:
+    """Converts a hex color code to RGB."""
+    hex_code = hex_code.lstrip("#")
+    return {
+        "red": int(hex_code[:2], 16),
+        "green": int(hex_code[2:4], 16),
+        "blue": int(hex_code[4:], 16),
+    }
+
+
 def url_components(url: str) -> dict[str, List[str]]:
     return urllib.parse.parse_qs(urllib.parse.urlparse(url).query)
 
 
 def update_url_params(url: str, params: dict) -> str:
     url_obj = urllib.parse.urlparse(url)
     params.update(urllib.parse.parse_qsl(url_obj.query))
```

### Comparing `googleapiutils2-0.7.1/pyproject.toml` & `googleapiutils2-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.7.1"
+version = "0.8.0"
 description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 
 readme = "README.md"
 keywords = ["google", "googleapi", "googleapiutils2"]
 license = "MIT"
 repository = "https://github.com/mkbabb/googleapiutils2"
```

### Comparing `googleapiutils2-0.7.1/PKG-INFO` & `googleapiutils2-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleapiutils2
-Version: 0.7.1
+Version: 0.8.0
 Summary: Wrapper for Google's Python API.
 Home-page: https://github.com/mkbabb/googleapiutils2
 License: MIT
 Keywords: google,googleapi,googleapiutils2
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
```

