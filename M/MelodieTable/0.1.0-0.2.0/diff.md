# Comparing `tmp/MelodieTable-0.1.0-py3-none-any.whl.zip` & `tmp/MelodieTable-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 8164 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat       85 b- defN 23-Apr-30 08:51 MelodieTable/__init__.py
--rw-rw-rw-  2.0 fat     5965 b- defN 23-May-03 10:30 MelodieTable/reader_writer.py
--rw-rw-rw-  2.0 fat     1945 b- defN 23-May-02 14:55 MelodieTable/table_base.py
--rw-rw-rw-  2.0 fat     4748 b- defN 23-May-02 15:14 MelodieTable/table_general.py
--rw-rw-rw-  2.0 fat     4164 b- defN 23-Apr-30 08:51 MelodieTable/table_pyam.py
--rw-rw-rw-  2.0 fat     1092 b- defN 23-May-09 13:02 MelodieTable-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      209 b- defN 23-May-09 13:02 MelodieTable-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-09 13:02 MelodieTable-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       67 b- defN 23-May-09 13:02 MelodieTable-0.1.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-May-09 13:02 MelodieTable-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      927 b- defN 23-May-09 13:02 MelodieTable-0.1.0.dist-info/RECORD
-11 files, 19307 bytes uncompressed, 6580 bytes compressed:  65.9%
+Zip file size: 10042 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      163 b- defN 23-May-30 12:51 MelodieTable/__init__.py
+-rw-rw-rw-  2.0 fat     6128 b- defN 23-May-09 14:56 MelodieTable/reader_writer.py
+-rw-rw-rw-  2.0 fat     2800 b- defN 23-May-30 13:33 MelodieTable/table_base.py
+-rw-rw-rw-  2.0 fat     3104 b- defN 23-May-30 12:01 MelodieTable/table_general.py
+-rw-rw-rw-  2.0 fat     6645 b- defN 23-May-31 11:04 MelodieTable/table_objects.py
+-rw-rw-rw-  2.0 fat     4077 b- defN 23-May-30 12:19 MelodieTable/table_pyam.py
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Jun-02 02:28 MelodieTable-0.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      160 b- defN 23-Jun-02 02:28 MelodieTable-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-02 02:28 MelodieTable-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       66 b- defN 23-Jun-02 02:28 MelodieTable-0.2.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-02 02:28 MelodieTable-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1014 b- defN 23-Jun-02 02:28 MelodieTable-0.2.0.dist-info/RECORD
+12 files, 25354 bytes uncompressed, 8324 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -6,29 +6,32 @@
 
 Filename: MelodieTable/table_base.py
 Comment: 
 
 Filename: MelodieTable/table_general.py
 Comment: 
 
+Filename: MelodieTable/table_objects.py
+Comment: 
+
 Filename: MelodieTable/table_pyam.py
 Comment: 
 
-Filename: MelodieTable-0.1.0.dist-info/LICENSE
+Filename: MelodieTable-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: MelodieTable-0.1.0.dist-info/METADATA
+Filename: MelodieTable-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: MelodieTable-0.1.0.dist-info/WHEEL
+Filename: MelodieTable-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: MelodieTable-0.1.0.dist-info/entry_points.txt
+Filename: MelodieTable-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: MelodieTable-0.1.0.dist-info/top_level.txt
+Filename: MelodieTable-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: MelodieTable-0.1.0.dist-info/RECORD
+Filename: MelodieTable-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## MelodieTable/__init__.py

```diff
@@ -1,3 +1,5 @@
-from .table_general import *
+from .table_base import column_meta
+from .table_objects import *
+from .table_general import GeneralTable
 from .table_pyam import *
 from .reader_writer import *
```

## MelodieTable/reader_writer.py

```diff
@@ -175,12 +175,17 @@
         self.engine = engine
 
     def write_table(self, table_name: str, columns, data:List[Dict]):
         stat_cls = get_stat_cls(table_name, columns)
         insp = inspect(self.engine)
         if not insp.has_table(table_name):
             stat_cls.__table__.create(bind=self.engine)
-        self.engine.execute(
-            stat_cls.__table__.insert(),
-            data
-        )
+        # self.engine.execute(
+        #     stat_cls.__table__.insert(),
+        #     data
+        # )
+        with self.engine.connect() as conn:
+            conn.execute(
+                stat_cls.__table__.insert(),
+                data
+            )
```

## MelodieTable/table_base.py

```diff
@@ -1,27 +1,58 @@
-from typing import Callable, List, Tuple
+from dataclasses import dataclass
+from sqlalchemy.types import BigInteger, Text, TypeEngine, Float, Boolean
+from typing import Callable, Dict, List, Optional, Tuple, TypeVar, Type, Any
+
+pytypes_to_satypes: Dict[Type, Type[TypeEngine]] = {
+    int: BigInteger,
+    str: Text,
+    float: Float,
+    bool: Boolean
+}
+
+
+@dataclass
+class ColumnMeta:
+    column_name: str
+    dtype: Optional[TypeEngine]
+
+    def __post_init__(self):
+        assert isinstance(
+            self.dtype, TypeEngine) or self.dtype is None, self.dtype
+
+
+def column_meta(col_name: str, dtype: Optional[TypeEngine] = None) -> Any:
+    o = ColumnMeta(col_name, dtype)
+    return o
 
 
 class RowBase:
     def payload_to_str(self):
         return f"{self.__dict__}"
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} {self.payload_to_str()}>"
 
 
-class TableBase:
+class TableBase():
 
-    class IatIndicer:
+    class IatObjectsIndicer:
         def __init__(self, data: List) -> None:
             self.data = data
 
         def __getitem__(self, indices):
             return getattr(self.data[indices[0]], indices[1])
 
+    class IatDictsIndicer:
+        def __init__(self, data: List) -> None:
+            self.data = data
+
+        def __getitem__(self, indices):
+            return self.data[indices[0]][indices[1]]
+
     def __init__(self) -> None:
         self.data: List[object] = []
 
     def __len__(self):
         return len(self.data)
 
     def create_empty(self):
@@ -59,8 +90,8 @@
         new_data = self.find_all(query)
         new_table = self.create_same_schemed_empty()
         new_table.data = new_data
         return new_table
 
     @property
     def iat(self):
-        return TableBase.IatIndicer(self.data)
+        return TableBase.IatObjectsIndicer(self.data)
```

## MelodieTable/table_general.py

```diff
@@ -1,133 +1,98 @@
-from typing import Callable, List, Tuple, Type, Union, Dict
+from typing import Callable, List, Optional, Tuple, Type, Union, Dict
 from sqlalchemy import Column
 from sqlalchemy.types import TypeEngine
 from sqlalchemy.orm import declarative_base
 from .reader_writer import TableReader, TableWriter, DatabaseConnector
 from .table_base import TableBase, RowBase
 
 Base = declarative_base()
 
 VEC_TEMPLATE = """
 def vectorize_template(obj):
     return [{exprs}]
 """
 
 
-class TableRow(RowBase):
-    def __init__(self, **kwargs) -> None:
-        for k, v in kwargs.items():
-            setattr(self, k, v)
+RowType = Dict[str, TypeEngine]
 
-    @staticmethod
-    def vectorizer(attrs: List[str]) -> Callable[[List[str]], str]:
-        exprs = ",".join(['obj.'+attr for attr in attrs])
-        code = VEC_TEMPLATE.format(exprs=exprs)
-        vars = {}
-        exec(code, None, vars)
-        return vars["vectorize_template"]
-
-
-RowType = Union[Type, Dict[str, TypeEngine]]
 
+class GeneralTable(TableBase):
+    data: List[dict]
 
-class Table(TableBase):
-    def __init__(self, name: str, row_type: RowType) -> None:
+    def __init__(self, row_type: RowType) -> None:
         super().__init__()
-        self.name = name
-        self.row_cls: Type = None
         self._db_model_cls: Type = None
         self.row_types: Dict[str, Column] = {}
 
-        if callable(row_type):
-            self.row_cls = row_type
-        elif isinstance(row_type, dict):
-            self.row_cls = TableRow
-            for prop_name, prop_value in row_type.items():
-                self.row_types[prop_name] = Column(prop_value)
-        else:
-            raise NotImplementedError(
-                f"Cannot recognize table row type {type(row_type)}")
+        for prop_name, prop_value in row_type.items():
+            self.row_types[prop_name] = Column(prop_value)
 
     def clear(self):
-        self.data = []
+        self.data.clear()
 
     def new_row(self):
-        # if len(self._deleted_rows_cache) == 0:
-        return self.row_cls()
-        # else:
-        #     return self._deleted_rows_cache.pop()
+        return {}
 
     @staticmethod
     def parse_header(header_colnames_list: List[str]):
         """
         Parse the header row.
         """
-        cols: List[str] = []
-        for col_index, col_name in enumerate(header_colnames_list):
-            cols.append(col_name)
-            assert col_name.isidentifier, f"Column name '{col_name}' should be an identifier!"
-        return cols
+        return header_colnames_list
 
     @staticmethod
     def from_file(file_name: str, row_types: RowType, encoding='utf-8'):
-        table = Table('', row_type=row_types)
+        table = GeneralTable(row_type=row_types)
         reader = TableReader(file_name,
                              text_encoding=encoding)
         header, rows_iter = reader.read()
-        columns = Table.parse_header(header)
+        columns = GeneralTable.parse_header(header)
 
         for row_data in rows_iter:
-            table_row_obj = table.row_cls(
-                **{col: row_data[i] for i, col in enumerate(columns)})
+            table_row_obj = {col: row_data[i] for i, col in enumerate(columns)}
             table.data.append(table_row_obj)
         return table
 
     def to_file(self, file_name: str, encoding="utf-8"):
         writer = TableWriter(file_name,
                              text_encoding=encoding).write()
-        headers = [row for row in self.row_types.keys()]
+        headers = [col_name for col_name in self.row_types.keys()]
         writer.send(headers)
         for row_data in self.data:
-            writer.send([row_data.__dict__[k] for k in headers])
+            writer.send([row_data[k] for k in headers])
         writer.close()
 
     def to_database(self, engine, table_name: str):
         conn = DatabaseConnector(engine)
-        conn.write_table(table_name, self.row_types, [
-                         d.__dict__ for d in self.data])
+        conn.write_table(table_name, self.row_types, self.data)
 
-    def to_file_with_codegen(self, file_name: str, encoding="utf-8"):
-        writer = TableWriter(file_name,
-                             text_encoding=encoding).write()
-        headers = [row for row in self.row_types.keys()]
-        writer.send(headers)
-        vectorizer = TableRow.vectorizer(headers)
-        for row_data in self.data:
-            writer.send(vectorizer(row_data))
-        writer.close()
+    # def from_pandas(self, df: "pd.DataFrame"):
+    #     """
+    #     Create a general table from pandas dataframe.
+    #     """
+    #     pass
 
     @staticmethod
-    def from_dicts(name: str, row_type: RowType, dicts: List[dict]):
-        table = Table(name, row_type)
-        for dic in dicts:
-            table.data.append(table.row_cls(**dic))
+    def from_dicts(row_type: RowType, dicts: List[dict], copy=True):
+        table = GeneralTable(row_type)
+        if not copy:
+            for dic in dicts:
+                table.data.append(dic)
+        else:
+            for dic in dicts:
+                table.data.append({k: v for k, v in dic.items()})
         return table
 
-    def find_one(self, query: Callable[[object], bool]) -> object:
+    def find_one(self, query: Callable[[dict], bool]) -> Optional[dict]:
         _, obj = self.find_one_with_index(query)
         return obj
 
-    def find_one_with_index(self, query: Callable[[object], bool]) -> Tuple[int, object]:
+    def find_one_with_index(self, query: Callable[[dict], bool]) -> Tuple[int, Optional[dict]]:
         for i, obj in enumerate(self.data):
             if query(obj):
                 return i, obj
         return -1, None
-    # def get_db_class(self):
-    #     if self._db_model_cls is not None:
-    #         self._db_model_cls = type("TableModel_"+self.name, (Base,), {
-    #             '__tablename__': "{}".format(self.name),
-    #             "id": Column(Integer, primary_key=True, autoincrement=True),
-    #             "a": Column(Integer),
-    #             "b": Column(Integer)
-    #         })
-    #     return self._db_model_cls
+
+    @property
+    def iat(self):
+        return TableBase.IatDictsIndicer(self.data)
```

## MelodieTable/table_pyam.py

```diff
@@ -1,10 +1,10 @@
 import csv
 
-from typing import Callable, List, Tuple, Type, Union, Dict
+from typing import Callable, Generic, List, Optional, Tuple, Type, TypeVar, Union, Dict, cast
 from sqlalchemy import Column
 from sqlalchemy.types import TypeEngine
 from sqlalchemy.orm import declarative_base
 from .reader_writer import TableReader
 from .table_base import TableBase, RowBase
 Base = declarative_base()
 
@@ -20,19 +20,22 @@
     def __init__(self, name: str, col_index: int) -> None:
         self.name = name
         self.col_index = col_index
 
 
 RowType = Union[Type, Dict[str, TypeEngine]]
 
+PyAMTableRowType = TypeVar("PyAMTableRowType")
 
-class PyAMTable(TableBase):
-    def __init__(self, name: str, row_type: PyAMTableRow, data_type=float) -> None:
+
+class PyAMTable(TableBase, Generic[PyAMTableRowType]):
+    data: List[PyAMTableRowType]
+
+    def __init__(self, row_type: Union[Type[PyAMTableRow], Dict[str, TypeEngine]], data_type=float) -> None:
         super().__init__()
-        self.name = name
         self.row_cls: Type = None
         self._db_model_cls: Type = None
         self.row_types: Dict[str, Column] = {}
         self.time_points: List[str] = []
         self.data_type: Union[Type[int], Type[float], Type[str]] = data_type
         if callable(row_type):
             self.row_cls = row_type
@@ -41,15 +44,15 @@
             for prop_name, prop_value in row_type.items():
                 self.row_types[prop_name] = Column(prop_value)
         else:
             raise NotImplementedError(
                 f"Cannot recognize table row type {type(row_type)}")
 
     def create_empty(self):
-        return PyAMTable("", {})
+        return PyAMTable(PyAMTableRow)
 
     @staticmethod
     def parse_header(header_colnames_list: List[str]):
         """
         Parse the header row of an PyAM file.
         """
         keys: List[PyAMKey] = []
@@ -59,23 +62,23 @@
             if col_name.isdecimal():
                 time_points.append(col_name)
             else:
                 assert col_name.isidentifier(
                 ), f"{col_name} should be an identifier"
                 keys.append(PyAMKey(col_name, col_index))
         return keys, time_points
+
     def conv_type(self, item):
-        if item=="" or item is None:
+        if item == "" or item is None:
             return None
         return self.data_type(item)
-        
 
     @staticmethod
     def from_file(file_name: str, row_types: RowType, data_type=float, encoding='utf-8'):
-        table = PyAMTable('', row_types, data_type=data_type,)
+        table = PyAMTable(row_types, data_type=data_type,)
         reader = TableReader(file_name,
                              text_encoding=encoding)
         header, rows_iter = reader.read()
         columns, time_points = PyAMTable.parse_header(header)
 
         table.time_points = time_points
         for row_data in rows_iter:
@@ -83,31 +86,25 @@
                 **{col.name: row_data[i] for i, col in enumerate(columns)})
             table_row_obj.data = [table.conv_type(
                 item) for item in row_data[len(columns):]]
             table.data.append(table_row_obj)
         return table
 
     @staticmethod
-    def from_dicts(name: str, row_type: RowType, dicts: List[dict]):
-        table = PyAMTable(name, row_type)
+    def from_dicts(row_type: RowType, dicts: List[dict]):
+        table = PyAMTable(row_type)
         for dic in dicts:
             table.data.append(table.row_cls(**dic))
         return table
 
     def find_one(self, query: Callable[[object], bool]) -> object:
         _, obj = self.find_one_with_index(query)
         return obj
 
-    def find_one_with_index(self, query: Callable[[object], bool]) -> Tuple[int, object]:
+    def find_one_with_index(self, query: Callable[[PyAMTableRowType], bool]) -> Tuple[int, Optional[PyAMTableRowType]]:
         for i, obj in enumerate(self.data):
             if query(obj):
                 return i, obj
         return -1, None
-    # def get_db_class(self):
-    #     if self._db_model_cls is not None:
-    #         self._db_model_cls = type("TableModel_"+self.name, (Base,), {
-    #             '__tablename__': "{}".format(self.name),
-    #             "id": Column(Integer, primary_key=True, autoincrement=True),
-    #             "a": Column(Integer),
-    #             "b": Column(Integer)
-    #         })
-    #     return self._db_model_cls
+
+    def filter(self, query: Callable[[PyAMTableRowType], bool]) -> "PyAMTable[PyAMTableRowType]":
+        return cast(PyAMTable, super().filter(cast(Callable[[object], bool], query)))
```

## Comparing `MelodieTable-0.1.0.dist-info/LICENSE` & `MelodieTable-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

