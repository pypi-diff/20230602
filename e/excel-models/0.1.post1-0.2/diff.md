# Comparing `tmp/excel-models-0.1.post1.tar.gz` & `tmp/excel-models-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel-models-0.1.post1.tar", last modified: Wed May 17 03:02:33 2023, max compression
+gzip compressed data, was "excel-models-0.2.tar", last modified: Fri Jun  2 18:01:14 2023, max compression
```

## Comparing `excel-models-0.1.post1.tar` & `excel-models-0.2.tar`

### file list

```diff
@@ -1,47 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:02:33.325576 excel-models-0.1.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-17 03:02:26.000000 excel-models-0.1.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-17 03:02:33.325576 excel-models-0.1.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-17 03:02:26.000000 excel-models-0.1.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:02:33.321576 excel-models-0.1.post1/excel_models/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:02:33.321576 excel-models-0.1.post1/excel_models/columns/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/columns/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/columns/_inst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/columns/basic_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/columns/collection_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/db.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:02:33.325576 excel-models-0.1.post1/excel_models/tables/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/tables/_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/tables/_inst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:02:33.325576 excel-models-0.1.post1/excel_models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/utils/class_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/utils/descriptors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:02:33.325576 excel-models-0.1.post1/excel_models/validators/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-17 03:02:19.000000 excel-models-0.1.post1/excel_models/validators/comparisons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:02:33.321576 excel-models-0.1.post1/excel_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-17 03:02:33.000000 excel-models-0.1.post1/excel_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-17 03:02:33.000000 excel-models-0.1.post1/excel_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 03:02:33.000000 excel-models-0.1.post1/excel_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-17 03:02:33.000000 excel-models-0.1.post1/excel_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 03:02:33.000000 excel-models-0.1.post1/excel_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:02:33.325576 excel-models-0.1.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-17 03:02:19.000000 excel-models-0.1.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:02:33.325576 excel-models-0.1.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-17 03:02:19.000000 excel-models-0.1.post1/tests/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-17 03:02:19.000000 excel-models-0.1.post1/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-17 03:02:19.000000 excel-models-0.1.post1/tests/test_cell_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-17 03:02:19.000000 excel-models-0.1.post1/tests/test_cell_access_many.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-17 03:02:19.000000 excel-models-0.1.post1/tests/test_cell_access_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-17 03:02:19.000000 excel-models-0.1.post1/tests/test_custom_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-17 03:02:19.000000 excel-models-0.1.post1/tests/test_custom_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-17 03:02:19.000000 excel-models-0.1.post1/tests/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-17 03:02:19.000000 excel-models-0.1.post1/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-17 03:02:19.000000 excel-models-0.1.post1/tests/test_model_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-17 03:02:19.000000 excel-models-0.1.post1/tests/test_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-17 03:02:19.000000 excel-models-0.1.post1/tests/test_open_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.333166 excel-models-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-02 18:01:07.000000 excel-models-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-02 18:01:14.333166 excel-models-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-02 18:01:07.000000 excel-models-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models/column_inst/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/column_inst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/column_inst/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/column_inst/_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/column_inst/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/column_inst/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/column_inst/remainder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models/columns/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/columns/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/columns/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/columns/_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/columns/basic_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/columns/collection_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/columns/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/models/_std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/tables/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/tables/_inst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/tables/_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/utils/assignable_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/utils/class_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/utils/descriptors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/validators/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-02 18:01:04.000000 excel-models-0.2/excel_models/validators/comparisons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.329166 excel-models-0.2/excel_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-02 18:01:14.000000 excel-models-0.2/excel_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-02 18:01:14.000000 excel-models-0.2/excel_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:01:14.000000 excel-models-0.2/excel_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-02 18:01:14.000000 excel-models-0.2/excel_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 18:01:14.000000 excel-models-0.2/excel_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 18:01:14.333166 excel-models-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-02 18:01:04.000000 excel-models-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:01:14.333166 excel-models-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_cell_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_cell_access_many.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_cell_access_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_custom_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_custom_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_model_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-02 18:01:04.000000 excel-models-0.2/tests/test_open_modes.py
```

### Comparing `excel-models-0.1.post1/LICENSE` & `excel-models-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `excel-models-0.1.post1/PKG-INFO` & `excel-models-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-models
-Version: 0.1.post1
+Version: 0.2
 Summary: Model-style Excel File Accessor
 Home-page: https://github.com/MichaelKim0407/excel-models
 Author: Zheng Jin
 Author-email: mkim0407@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `excel-models-0.1.post1/README.md` & `excel-models-0.2/README.md`

 * *Files identical despite different names*

### Comparing `excel-models-0.1.post1/excel_models/columns/_inst.py` & `excel-models-0.2/excel_models/column_inst/_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,76 +1,59 @@
 import typing
-from functools import cached_property
 
 from openpyxl.cell import Cell
-from openpyxl.utils import get_column_letter
 
-from ._base import TColumnDef
-from ..tables import TTable
+from excel_models.typing import AbstractColumn, TTable, TColumnDef, ColumnValue
 
 
-class ExcelColumn(typing.Generic[TTable, TColumnDef]):
+class BaseExcelColumn(AbstractColumn):
     def __init__(
             self,
             table: TTable,
             column_def: TColumnDef,
-            col_num: int,
     ):
         self.table = table
         self.column_def = column_def
-        self.col_num = col_num
 
-    @cached_property
-    def col_letter(self) -> str:
-        return get_column_letter(self.col_num)
+    def check(self) -> None:
+        pass
 
     def __eq__(self, other: typing.Self) -> bool:
-        if other is None or not isinstance(other, ExcelColumn):
+        if other is None or not isinstance(other, BaseExcelColumn):
             return False
 
         return (
                 self.table == other.table
                 and self.column_def == other.column_def
-                and self.col_num == other.col_num
         )
 
-    def __getitem__(self, idx: int | slice):
+    def __getitem__(self, idx: int | slice) -> ColumnValue | list[ColumnValue]:
         if isinstance(idx, slice):
             return [
                 self.column_def.__get__(row)
                 for row in self.table[idx]
             ]
 
         return self.column_def.__get__(self.table[idx])
 
-    def __iter__(self) -> typing.Iterator:
+    def __iter__(self) -> typing.Iterator[ColumnValue]:
         for row in self.table:
             yield self.column_def.__get__(row)
 
-    def __setitem__(self, idx: int | slice, value):
+    def __setitem__(self, idx: int | slice, value: ColumnValue) -> None:
         if isinstance(idx, slice):
             for row, v in zip(self.table[idx], value, strict=True):
                 self.column_def.__set__(row, v)
             return
 
         self.column_def.__set__(self.table[idx], value)
 
-    def __delitem__(self, idx: int | slice):
+    def __delitem__(self, idx: int | slice) -> None:
         if isinstance(idx, slice):
             for row in self.table[idx]:
                 self.column_def.__delete__(row)
             return
 
         self.column_def.__delete__(self.table[idx])
 
-    def cell(self, row_num: int) -> Cell:
-        return self.table.cell(row_num, self.col_num)
-
     def cell0(self, idx: int) -> Cell:
         return self.cell(self.table.get_row_num(idx))
-
-    @property
-    def cells(self) -> typing.Sequence[Cell]:
-        return self.table.ws[self.col_letter][self.table.get_row_num(-1):]
-
-
-TColumn = typing.TypeVar('TColumn', bound=ExcelColumn)
```

### Comparing `excel-models-0.1.post1/excel_models/columns/basic_types.py` & `excel-models-0.2/excel_models/columns/basic_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from datetime import datetime
 
-from ._base import Column
+from excel_models.typing import CellValue, ColumnValue
+from ._std import Column
 
 
 class BaseTypedColumn(Column):
-    def _convert_to_python(self, value):
+    def _convert_to_python(self, raw: CellValue) -> ColumnValue:
         raise NotImplementedError  # pragma: no cover
 
-    def _to_python(self, value):
-        if value is None:
+    def to_python(self, raw: CellValue) -> ColumnValue:
+        if raw is None:
             return None
-        return self._convert_to_python(value)
+        return self._convert_to_python(raw)
 
-    def _convert_from_python(self, value):
+    def _convert_from_python(self, value: ColumnValue) -> CellValue:
         raise NotImplementedError  # pragma: no cover
 
-    def _from_python(self, value):
+    def from_python(self, value: ColumnValue) -> CellValue:
         if value is None:
             return None
         return self._convert_from_python(value)
 
 
 class BaseSimpleTypeColumn(BaseTypedColumn):
-    def _convert(self, value):
+    def _convert(self, value: CellValue | ColumnValue) -> ColumnValue | CellValue:
         raise NotImplementedError  # pragma: no cover
 
-    def _convert_to_python(self, value):
-        return self._convert(value)
+    def _convert_to_python(self, raw: CellValue) -> ColumnValue:
+        return self._convert(raw)
 
-    def _convert_from_python(self, value):
+    def _convert_from_python(self, value: ColumnValue) -> CellValue:
         return self._convert(value)
 
 
 class StringColumn(BaseSimpleTypeColumn):
     _convert = str
```

### Comparing `excel-models-0.1.post1/excel_models/db.py` & `excel-models-0.2/excel_models/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
-import typing
 from functools import cached_property
 
 from openpyxl.reader.excel import load_workbook
 from openpyxl.workbook import Workbook
 
-from .utils.class_collector import CollectorMeta, ListCollector
+from excel_models.typing import AbstractDB, TTableDef
+from excel_models.utils.class_collector import CollectorMeta, ListCollector
 
 
-class ExcelDB(metaclass=CollectorMeta):
-    tables: ListCollector['TTableDef'] = ListCollector()
+class ExcelDB(AbstractDB, metaclass=CollectorMeta):
+    tables: ListCollector[TTableDef] = ListCollector()
 
     MODE_OPEN = 'o'  # open an existing file; FileNotFoundError
     MODE_CREATE = 'n'  # create a new file; FileExistsError
     MODE_OVERWRITE = 'w'  # overwrite and existing file; FileNotFoundError
     MODE_OPEN_CREATE = 'a'  # open an existing file; create a new file
     MODE_CREATE_OVERWRITE = 'x'  # create a new file; overwrite an existing file
 
@@ -22,15 +22,15 @@
             filename: str,
             *,
             mode: str = MODE_OPEN_CREATE,
     ):
         self.filename = filename
         self.mode = mode
 
-        self.ws_cache = {}
+        self.tables_cache = {}
 
     @cached_property
     def wb(self) -> Workbook:
         if os.path.exists(self.filename):
             if self.mode in (self.MODE_OPEN, self.MODE_OPEN_CREATE):
                 return load_workbook(self.filename)
             elif self.mode in (self.MODE_OVERWRITE, self.MODE_CREATE_OVERWRITE):
@@ -44,13 +44,7 @@
                 raise FileNotFoundError(self.filename)
 
     def save_as(self, filename: str):
         self.wb.save(filename)
 
     def save(self):
         self.save_as(self.filename)
-
-
-TDB = typing.TypeVar('TDB', bound=ExcelDB)
-
-if typing.TYPE_CHECKING:
-    from .tables import TTableDef
```

### Comparing `excel-models-0.1.post1/excel_models/models.py` & `excel-models-0.2/excel_models/models/_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 import typing
 
 from openpyxl.cell import Cell
 from returns import returns
 
-from .utils.class_collector import CollectorMeta, ListCollector
+from excel_models.typing import AbstractModel, TColumnDef, TTableDef, TTable, ColumnValue
+from excel_models.utils.class_collector import CollectorMeta, ListCollector
 
 
-class ExcelModel(metaclass=CollectorMeta):
-    columns: ListCollector['TColumnDef'] = ListCollector()
+class BaseExcelModel(AbstractModel, metaclass=CollectorMeta):
+    column_defs: ListCollector[TColumnDef] = ListCollector()
+    table_def_class: typing.Type[TTableDef]  # assign in subclass
 
     @classmethod
-    def as_table(
-            cls,
-            *,
-            table_def_class: typing.Type['TTableDef'] = None,
-            **kwargs,
-    ) -> 'TTableDef':
-        if table_def_class is None:
-            from .tables import ExcelTableDefinition
-            table_def_class = ExcelTableDefinition
-        return table_def_class(cls, **kwargs)
+    def as_table(cls, **table_def_kwargs) -> TTableDef:
+        return cls.table_def_class(model=cls, **table_def_kwargs)
 
     def __init__(
             self,
-            table: 'TTable',
+            table: TTable,
             idx: int,
             row_num: int,
     ):
         self.table = table
         self.idx = idx
         self.row_num = row_num
 
         self.values_cache = {}
 
     def __eq__(self, other: typing.Self) -> bool:
-        if other is None or not isinstance(other, ExcelModel):
+        if other is None or not isinstance(other, BaseExcelModel):
             return False
 
         return (
                 self.table == other.table
                 and self.idx == other.idx
                 and self.row_num == other.row_num
         )
@@ -46,24 +40,24 @@
     def __bool__(self) -> bool:
         for cell in self.cells:
             if cell.value is not None:
                 return True
         return False
 
     @returns(dict)
-    def as_dict(self) -> dict[str, typing.Any]:
-        for column in self.columns:
-            yield column.name, column.__get__(self)
+    def as_dict(self) -> dict[str, ColumnValue]:
+        for column_def in self.column_defs:
+            yield column_def.name, column_def.__get__(self)
 
     def set_dict(
             self,
-            mapping: typing.Mapping[str, typing.Any] = None,
+            mapping: typing.Mapping[str, ColumnValue] = None,
             /,
             **kwargs,
-    ):
+    ) -> None:
         if mapping is not None:
             for k, v in mapping.items():
                 setattr(self, k, v)
         for k, v in kwargs.items():
             setattr(self, k, v)
 
     def cell(self, col_num: int) -> Cell:
@@ -73,15 +67,8 @@
         return self.cell(col_idx + 1)
 
     def cella(self, attr: str) -> Cell:
         return self.cell(getattr(self.table, attr).col_num)
 
     @property
     def cells(self) -> typing.Sequence[Cell]:
-        return self.table.ws[self.row_num]
-
-
-TModel = typing.TypeVar('TModel', bound=ExcelModel)
-
-if typing.TYPE_CHECKING:
-    from .tables import TTableDef, TTable
-    from .columns import TColumnDef
+        return self.table.row(self.row_num)
```

### Comparing `excel-models-0.1.post1/excel_models/tables/_def.py` & `excel-models-0.2/excel_models/tables/_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,98 +1,84 @@
 import typing
 
 from openpyxl.worksheet.worksheet import Worksheet
 
-from ..db import ExcelDB
-from ..models import TModel
-from ..utils.descriptors import BasePropertyDescriptor
+from excel_models.typing import AbstractTableDefinition, TDB, TTable
+from excel_models.utils.descriptors import BasePropertyDescriptor
 
 
-class ExcelTableDefinition(
-    BasePropertyDescriptor[ExcelDB],
-    typing.Generic[TModel],
+class BaseExcelTableDefinition(
+    BasePropertyDescriptor[TDB],
+    AbstractTableDefinition,
 ):
+    table_class: typing.Type[TTable]  # assign in subclass
     title_row: int = 1
-
-    def __init__(
-            self,
-            model: typing.Type[TModel],
-            *,
-            table_class: typing.Type['TTable'] = None,
-            **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.model = model
-        if table_class is None:
-            from ._inst import ExcelTable
-            table_class = ExcelTable
-        self.table_class: typing.Type['TTable'] = table_class
+    trim: bool = False
 
     def _add_to_class(self):
+        super()._add_to_class()
         self.obj_type.tables.append(self)
 
-    _f_initialize = None
+    def make_table(self, db: TDB, ws: Worksheet) -> TTable:
+        return self.table_class(db, self, ws)
 
-    def _initialize_title_row(self, db: ExcelDB, ws: Worksheet):
-        for i, column in enumerate(self.model.columns):
-            ws.cell(self.title_row, i + 1, column.name)
+    _f_initialize = None
 
-    def _initialize_default(self, db: ExcelDB, ws: Worksheet):
+    def _initialize_default(self, db: TDB, table: TTable):
         pass
 
     @property
-    def _initialize_method(self):
+    def _initialize_method(self) -> typing.Callable:
         if self._f_initialize is None:
             return self._initialize_default
         else:
             return self._f_initialize
 
-    def initialize(self, db: ExcelDB, ws: Worksheet):
-        self._initialize_title_row(db, ws)
-        self._initialize_method(db, ws)  # noqa: pycharm
+    def _initialize(self, db: TDB, table: TTable):
+        self._initialize_method(db, table)
 
     def initializer(self, f_initialize):
         self._f_initialize = f_initialize
         return self
 
-    def _get_default(self, db: ExcelDB) -> Worksheet:
+    def _get_default(self, db: TDB) -> TTable:
         if self.name in db.wb:
-            return db.wb[self.name]
+            ws = db.wb[self.name]
+            table = self.make_table(db, ws)
+            if self.trim:
+                table.trim()
+            table.find_columns()
         else:
             ws = db.wb.create_sheet(self.name)
-            self.initialize(db, ws)
-            return ws
-
-    def _get(self, db: ExcelDB) -> 'TTable':
-        if self.attr not in db.ws_cache:
-            ws = self._get_method(db)
-            db.ws_cache[self.attr] = ws
-        ws = db.ws_cache[self.attr]
-        return self.table_class(db, self, ws)
+            table = self.make_table(db, ws)
+            table.init_columns()
+            self._initialize(db, table)
+        return table
+
+    def _get(self, db: TDB) -> TTable:
+        if self.attr not in db.tables_cache:
+            table = self._get_method(db)
+            db.tables_cache[self.attr] = table
+        return db.tables_cache[self.attr]
 
-    def _set_default(self, db: ExcelDB, ws: Worksheet) -> Worksheet:
+    def _set_default(self, db: TDB, table: TTable | Worksheet) -> TTable:
         if self.name in db.wb:
             del db.wb[self.name]
+        if isinstance(table, Worksheet):
+            ws = table
+        else:
+            ws = table.ws
         copy: Worksheet = db.wb.copy_worksheet(ws)
         copy.title = self.name
-        return copy
+        return self.make_table(db, copy)
 
-    def _set(self, db: ExcelDB, ws: typing.Union[Worksheet, 'TTable']):
-        from ._inst import ExcelTable
-        if isinstance(ws, ExcelTable):
-            ws = ws.ws
-        copy = self._set_method(db, ws)
-        db.ws_cache[self.attr] = copy
+    def _set(self, db: TDB, table: TTable | Worksheet):
+        copy = self._set_method(db, table)
+        db.tables_cache[self.attr] = copy
 
-    def _delete_default(self, db: ExcelDB):
+    def _delete_default(self, db: TDB):
         del db.wb[self.name]
 
-    def _delete(self, db: ExcelDB):
+    def _delete(self, db: TDB):
         if self.attr in db.__dict__:
-            del db.ws_cache[self.attr]
+            del db.tables_cache[self.attr]
         self._delete_method(db)
-
-
-TTableDef = typing.TypeVar('TTableDef', bound=ExcelTableDefinition)
-
-if typing.TYPE_CHECKING:
-    from ._inst import TTable
```

### Comparing `excel-models-0.1.post1/excel_models/utils/class_collector.py` & `excel-models-0.2/excel_models/utils/class_collector.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.1.post1/excel_models/utils/descriptors.py` & `excel-models-0.2/excel_models/utils/descriptors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import typing
 
 Object = typing.TypeVar('Object')
 ObjectType = typing.Type[Object]
 
 
 class BasePropertyDescriptor(typing.Generic[Object]):
+    name: str = None
+
     def __init__(self, **kwargs):
-        self.name = None
         for k, v in kwargs.items():
             setattr(self, k, v)
 
     def _add_to_class(self):
         pass  # pragma: no cover
 
     def __set_name__(self, obj_type: ObjectType, attr: str):
```

### Comparing `excel-models-0.1.post1/excel_models/validators/comparisons.py` & `excel-models-0.2/excel_models/validators/comparisons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from . import AbstractValueValidator
-from ..exceptions import ValidationError
+from excel_models.exceptions import ValidationError
+from ._base import AbstractValueValidator
 
 
 class AbstractComparisonValidator(AbstractValueValidator):
     skip_none = False
 
     def _compare(self, value) -> bool:
         raise NotImplementedError  # pragma: no cover
```

### Comparing `excel-models-0.1.post1/excel_models.egg-info/PKG-INFO` & `excel-models-0.2/excel_models.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-models
-Version: 0.1.post1
+Version: 0.2
 Summary: Model-style Excel File Accessor
 Home-page: https://github.com/MichaelKim0407/excel-models
 Author: Zheng Jin
 Author-email: mkim0407@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `excel-models-0.1.post1/excel_models.egg-info/SOURCES.txt` & `excel-models-0.2/excel_models.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,52 @@
 LICENSE
 README.md
 setup.py
 excel_models/__init__.py
 excel_models/db.py
 excel_models/exceptions.py
-excel_models/models.py
+excel_models/typing.py
 excel_models.egg-info/PKG-INFO
 excel_models.egg-info/SOURCES.txt
 excel_models.egg-info/dependency_links.txt
 excel_models.egg-info/requires.txt
 excel_models.egg-info/top_level.txt
+excel_models/column_inst/__init__.py
+excel_models/column_inst/_base.py
+excel_models/column_inst/_std.py
+excel_models/column_inst/array.py
+excel_models/column_inst/map.py
+excel_models/column_inst/remainder.py
 excel_models/columns/__init__.py
 excel_models/columns/_base.py
-excel_models/columns/_inst.py
+excel_models/columns/_container.py
+excel_models/columns/_std.py
 excel_models/columns/basic_types.py
 excel_models/columns/collection_types.py
+excel_models/columns/multi.py
+excel_models/models/__init__.py
+excel_models/models/_base.py
+excel_models/models/_std.py
 excel_models/tables/__init__.py
-excel_models/tables/_def.py
+excel_models/tables/_base.py
 excel_models/tables/_inst.py
+excel_models/tables/_std.py
 excel_models/utils/__init__.py
+excel_models/utils/assignable_property.py
 excel_models/utils/class_collector.py
+excel_models/utils/collections.py
 excel_models/utils/descriptors.py
 excel_models/validators/__init__.py
+excel_models/validators/_base.py
 excel_models/validators/comparisons.py
+tests/test_alias.py
 tests/test_bool.py
 tests/test_caching.py
 tests/test_cell_access.py
 tests/test_cell_access_many.py
 tests/test_cell_access_raw.py
 tests/test_custom_column.py
 tests/test_custom_table.py
 tests/test_eq.py
-tests/test_filter.py
 tests/test_model_inheritance.py
 tests/test_new.py
 tests/test_open_modes.py
```

### Comparing `excel-models-0.1.post1/setup.py` & `excel-models-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.1.post1/tests/test_caching.py` & `excel-models-0.2/tests/test_caching.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
 
 def test_get(db, tmp_excel_data):
     user = db.users[0]
     assert user.id == tmp_excel_data[0][0]
     assert user.name == tmp_excel_data[0][1]
     # if we update the cells directly, cached columns should not reflect the changes
-    db.wb['users'].cell(2, 1).value = '10'
-    db.wb['users'].cell(2, 2).value = 'A'
+    db.users.cell(2, 1).value = '10'
+    db.users.cell(2, 2).value = 'A'
     assert user.id == '10'
     assert user.name == tmp_excel_data[0][1]
 
 
 def test_set(db):
     user = db.users[0]
     user.name = 'B'
     assert user.name == 'B'
-    assert db.wb['users'].cell(2, 2).value == 'B'
+    assert db.users.cell(2, 2).value == 'B'
 
 
 def test_del(db):
     user = db.users[0]
     del user.name
     assert 'name' not in user.__dict__
-    assert db.wb['users'].cell(2, 2).value is None
+    assert db.users.cell(2, 2).value is None
```

### Comparing `excel-models-0.1.post1/tests/test_cell_access.py` & `excel-models-0.2/tests/test_cell_access.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,26 +28,26 @@
     col = db.users.name
     assert (col[0], col[1], col[2]) == tuple(x[1] for x in tmp_excel_data)
 
 
 def test_set_by_row(db):
     row = db.users[1]
     row.name = 'Chris'
-    assert db.wb['users'].cell(3, 2).value == 'Chris'
+    assert db.users.cell(3, 2).value == 'Chris'
 
 
 def test_set_by_col(db):
     col = db.users.name
     col[1] = 'Chris'
-    assert db.wb['users'].cell(3, 2).value == 'Chris'
+    assert db.users.cell(3, 2).value == 'Chris'
 
 
 def test_del_by_row(db):
     row = db.users[2]
     del row.name
-    assert db.wb['users'].cell(4, 2).value is None
+    assert db.users.cell(4, 2).value is None
 
 
 def test_del_by_col(db):
     col = db.users.name
     del col[2]
-    assert db.wb['users'].cell(4, 2).value is None
+    assert db.users.cell(4, 2).value is None
```

### Comparing `excel-models-0.1.post1/tests/test_cell_access_many.py` & `excel-models-0.2/tests/test_cell_access_many.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,31 +34,31 @@
 
 def test_row_as_dict(db, tmp_excel_columns, tmp_excel_data):
     assert db.users[0].as_dict() == dict(zip(tmp_excel_columns, tmp_excel_data[0]))
 
 
 def test_row_set_dict(db):
     db.users[0].set_dict({'name': 'Chris'})
-    assert db.wb['users'].cell(2, 2).value == 'Chris'
+    assert db.users.cell(2, 2).value == 'Chris'
     db.users[1].set_dict(name='Carol')
-    assert db.wb['users'].cell(3, 2).value == 'Carol'
+    assert db.users.cell(3, 2).value == 'Carol'
 
 
 def test_column_iter(db, tmp_excel_data):
     for name, data in zip(db.users.name, tmp_excel_data, strict=True):
         assert name == data[1]
 
 
 def test_column_slice(db, tmp_excel_data):
     assert db.users.name[:-1] == [data[1] for data in tmp_excel_data[:-1]]
 
 
 def test_column_slice_set(db):
     db.users.name[:2] = ('Chris', 'Carol')
-    assert db.wb['users'].cell(2, 2).value == 'Chris'
-    assert db.wb['users'].cell(3, 2).value == 'Carol'
+    assert db.users.cell(2, 2).value == 'Chris'
+    assert db.users.cell(3, 2).value == 'Carol'
 
 
 def test_column_slice_del(db):
     del db.users.name[1:]
-    assert db.wb['users'].cell(3, 2).value is None
-    assert db.wb['users'].cell(4, 2).value is None
+    assert db.users.cell(3, 2).value is None
+    assert db.users.cell(4, 2).value is None
```

### Comparing `excel-models-0.1.post1/tests/test_cell_access_raw.py` & `excel-models-0.2/tests/test_cell_access_raw.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,44 @@
 def test_table_cell(db):
     cell = db.users.cell(1, 1)
     assert isinstance(cell, Cell)
     assert cell.row == 1
     assert cell.column == 1
 
 
+def test_table_row(db):
+    cells = db.users.row(2)
+    assert isinstance(cells, (list, tuple))
+    assert len(cells) == 2
+    for col, cell in enumerate(cells, start=1):
+        assert isinstance(cell, Cell)
+        assert cell.row == 2
+        assert cell.column == col
+
+
+def test_table_col(db):
+    cells = db.users.col(1)
+    assert isinstance(cells, (list, tuple))
+    assert len(cells) == 4
+    for row, cell in enumerate(cells, start=1):
+        assert isinstance(cell, Cell)
+        assert cell.row == row
+        assert cell.column == 1
+
+
+def test_table_col_data_only(db):
+    cells = db.users.col(1, data_only=True)
+    assert isinstance(cells, (list, tuple))
+    assert len(cells) == 3
+    for row, cell in enumerate(cells, start=2):
+        assert isinstance(cell, Cell)
+        assert cell.row == row
+        assert cell.column == 1
+
+
 def test_row_cell(db):
     cell = db.users[1].cell(2)
     assert isinstance(cell, Cell)
     assert cell.row == 3
     assert cell.column == 2
 
 
@@ -48,20 +78,18 @@
     assert cell.column == 1
 
 
 def test_row_cells(db):
     cells = db.users[0].cells
     assert isinstance(cells, (list, tuple))
     assert len(cells) == 2
-    assert isinstance(cells[0], Cell)
-    assert cells[0].row == 2
-    assert cells[0].column == 1
-    assert isinstance(cells[1], Cell)
-    assert cells[1].row == 2
-    assert cells[1].column == 2
+    for col, cell in enumerate(cells, start=1):
+        assert isinstance(cell, Cell)
+        assert cell.row == 2
+        assert cell.column == col
 
 
 def test_col_cell(db):
     cell = db.users.id.cell(3)
     assert isinstance(cell, Cell)
     assert cell.row == 3
     assert cell.column == 1
@@ -74,16 +102,11 @@
     assert cell.column == 2
 
 
 def test_col_cells(db):
     cells = db.users.name.cells
     assert isinstance(cells, (list, tuple))
     assert len(cells) == 3
-    assert isinstance(cells[0], Cell)
-    assert cells[0].row == 2
-    assert cells[0].column == 2
-    assert isinstance(cells[1], Cell)
-    assert cells[1].row == 3
-    assert cells[1].column == 2
-    assert isinstance(cells[2], Cell)
-    assert cells[2].row == 4
-    assert cells[2].column == 2
+    for row, cell in enumerate(cells, start=2):
+        assert isinstance(cell, Cell)
+        assert cell.row == row
+        assert cell.column == 2
```

### Comparing `excel-models-0.1.post1/tests/test_custom_column.py` & `excel-models-0.2/tests/test_custom_column.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import pytest
-from openpyxl.cell import Cell
 
 from excel_models.columns import Column
 from excel_models.db import ExcelDB
 from excel_models.models import ExcelModel
 
 
 @pytest.fixture()
 def excel(lazy_init_excel):
     return lazy_init_excel('users', 'name', 'John\nDoe', None, 'Bob', 1.5)
 
 
 class User(ExcelModel):
     @Column()
-    def name(self, cell: Cell):
-        if cell.value is None or cell.value == '':
+    def name(self):
+        raw = self._get_name(self)
+        if raw is None or raw == '':
             return []
-        return cell.value.split('\n')
+        return raw.split('\n')
+
+    _get_name = name.get_raw
+    _set_name = name.set_raw
 
     @name.setter
-    def name(self, value, cell: Cell):
+    def name(self, value):
         if not value:
-            cell.value = ''
+            self._set_name(self, '')
             return
-        cell.value = '\n'.join(value)
+        self._set_name(self, '\n'.join(value))
 
     @name.deleter
-    def name(self, cell: Cell):
-        cell.value = ''
+    def name(self):
+        self._set_name(self, '')
 
     @name.error_handler
-    def name(self, cell: Cell, ex: Exception):
-        return [str(cell.value)]
+    def name(self, ex: Exception):
+        return [str(self._get_name(self))]
 
 
 class MyDB(ExcelDB):
     users = User.as_table()
 
 
 @pytest.fixture()
@@ -45,13 +48,13 @@
 
 def test_get(db):
     assert db.users.name[:] == [['John', 'Doe'], [], ['Bob'], ['1.5']]
 
 
 def test_set(db):
     db.users[1].name = ['Chris']
-    assert db.wb['users'].cell(3, 1).value == 'Chris'
+    assert db.users.cell(3, 1).value == 'Chris'
 
 
 def test_del(db):
     del db.users[2].name
-    assert db.wb['users'].cell(4, 1).value == ''
+    assert db.users.cell(4, 1).value == ''
```

### Comparing `excel-models-0.1.post1/tests/test_eq.py` & `excel-models-0.2/tests/test_eq.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 @pytest.fixture()
 def db(tmp_excel_file):
     return MyDB(tmp_excel_file)
 
 
 def test_table_eq(db):
-    assert db.users is not db.users
+    assert db.users is db.users  # tables are cached
     assert db.users == db.users
     assert db.users != db.accounts
 
 
 def test_row_eq(db):
     users = db.users
     assert users[0] is not users[0]
```

### Comparing `excel-models-0.1.post1/tests/test_model_inheritance.py` & `excel-models-0.2/tests/test_model_inheritance.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,34 +19,34 @@
 
 @pytest.fixture()
 def db(tmp_excel_file):
     return MyDB(tmp_excel_file)
 
 
 def test_model_columns():
-    assert len(User.columns) == 2
-    assert [column.name for column in User.columns] == ['id', 'name']
+    assert len(User.column_defs) == 2
+    assert [column_def.name for column_def in User.column_defs] == ['id', 'name']
 
 
 def test_get_by_row(db, tmp_excel_data):
     assert db.users[0].id == tmp_excel_data[0][0]
     assert db.users[0].name == tmp_excel_data[0][1]
 
 
 def test_get_by_col(db, tmp_excel_data):
     assert db.users.id[1] == tmp_excel_data[1][0]
     assert db.users.name[1] == tmp_excel_data[1][1]
 
 
 def test_set_by_row(db):
     db.users[2].id = 100
-    assert db.wb['users'].cell(4, 1).value == 100
+    assert db.users.cell(4, 1).value == 100
     db.users[2].name = 'Chris'
-    assert db.wb['users'].cell(4, 2).value == 'Chris'
+    assert db.users.cell(4, 2).value == 'Chris'
 
 
 def test_set_by_col(db):
     db.users.id[:2] = 50, 51
-    assert db.wb['users'].cell(2, 1).value == 50
-    assert db.wb['users'].cell(3, 1).value == 51
+    assert db.users.cell(2, 1).value == 50
+    assert db.users.cell(3, 1).value == 51
     db.users.name[3] = 'Lucy'
-    assert db.wb['users'].cell(5, 2).value == 'Lucy'
+    assert db.users.cell(5, 2).value == 'Lucy'
```

### Comparing `excel-models-0.1.post1/tests/test_new.py` & `excel-models-0.2/tests/test_new.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.1.post1/tests/test_open_modes.py` & `excel-models-0.2/tests/test_open_modes.py`

 * *Files identical despite different names*

