# Comparing `tmp/MazgaDB-0.0.2.tar.gz` & `tmp/MazgaDB-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MazgaDB-0.0.2.tar", last modified: Fri Jun  2 10:10:40 2023, max compression
+gzip compressed data, was "MazgaDB-0.0.2.1.tar", last modified: Fri Jun  2 10:24:21 2023, max compression
```

## Comparing `MazgaDB-0.0.2.tar` & `MazgaDB-0.0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 10:10:40.477594 MazgaDB-0.0.2/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 10:10:40.473593 MazgaDB-0.0.2/MazgaDB.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     8777 2023-06-02 10:10:40.000000 MazgaDB-0.0.2/MazgaDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      479 2023-06-02 10:10:40.000000 MazgaDB-0.0.2/MazgaDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 10:10:40.000000 MazgaDB-0.0.2/MazgaDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-06-02 10:10:40.000000 MazgaDB-0.0.2/MazgaDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       22 2023-06-02 10:10:40.000000 MazgaDB-0.0.2/MazgaDB.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 10:10:40.473593 MazgaDB-0.0.2/MazgaDB_func/
--rw-r--r--   0 runner    (1000) runner    (1000)      236 2023-05-22 09:21:29.000000 MazgaDB-0.0.2/MazgaDB_func/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      211 2023-05-22 09:21:29.000000 MazgaDB-0.0.2/MazgaDB_func/append.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3802 2023-05-22 09:21:29.000000 MazgaDB-0.0.2/MazgaDB_func/class_db.py
--rw-r--r--   0 runner    (1000) runner    (1000)      211 2023-05-22 09:21:29.000000 MazgaDB-0.0.2/MazgaDB_func/column.py
--rw-r--r--   0 runner    (1000) runner    (1000)      154 2023-05-22 09:21:29.000000 MazgaDB-0.0.2/MazgaDB_func/delete.py
--rw-r--r--   0 runner    (1000) runner    (1000)      467 2023-05-22 09:21:29.000000 MazgaDB-0.0.2/MazgaDB_func/delete_column.py
--rw-r--r--   0 runner    (1000) runner    (1000)      187 2023-05-22 09:21:29.000000 MazgaDB-0.0.2/MazgaDB_func/is_there.py
--rw-r--r--   0 runner    (1000) runner    (1000)      400 2023-05-22 09:21:29.000000 MazgaDB-0.0.2/MazgaDB_func/new_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)      459 2023-05-22 09:21:29.000000 MazgaDB-0.0.2/MazgaDB_func/read_all.py
--rw-r--r--   0 runner    (1000) runner    (1000)      251 2023-05-22 09:21:29.000000 MazgaDB-0.0.2/MazgaDB_func/select.py
--rw-r--r--   0 runner    (1000) runner    (1000)      235 2023-05-22 09:21:29.000000 MazgaDB-0.0.2/MazgaDB_func/update.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8777 2023-06-02 10:10:40.473593 MazgaDB-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     5940 2023-06-02 10:06:20.000000 MazgaDB-0.0.2/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 10:10:40.473593 MazgaDB-0.0.2/mazga_db/
--rw-r--r--   0 runner    (1000) runner    (1000)     5547 2023-06-02 10:03:38.000000 MazgaDB-0.0.2/mazga_db/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      368 2023-05-22 09:24:18.000000 MazgaDB-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-02 10:10:40.477594 MazgaDB-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      760 2023-06-02 10:07:48.000000 MazgaDB-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 10:24:21.212477 MazgaDB-0.0.2.1/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 10:24:21.208477 MazgaDB-0.0.2.1/MazgaDB.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     8779 2023-06-02 10:24:21.000000 MazgaDB-0.0.2.1/MazgaDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      479 2023-06-02 10:24:21.000000 MazgaDB-0.0.2.1/MazgaDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 10:24:21.000000 MazgaDB-0.0.2.1/MazgaDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-06-02 10:24:21.000000 MazgaDB-0.0.2.1/MazgaDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       22 2023-06-02 10:24:21.000000 MazgaDB-0.0.2.1/MazgaDB.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 10:24:21.212477 MazgaDB-0.0.2.1/MazgaDB_func/
+-rw-r--r--   0 runner    (1000) runner    (1000)      236 2023-05-22 09:21:29.000000 MazgaDB-0.0.2.1/MazgaDB_func/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      211 2023-05-22 09:21:29.000000 MazgaDB-0.0.2.1/MazgaDB_func/append.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3802 2023-05-22 09:21:29.000000 MazgaDB-0.0.2.1/MazgaDB_func/class_db.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      211 2023-05-22 09:21:29.000000 MazgaDB-0.0.2.1/MazgaDB_func/column.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      154 2023-05-22 09:21:29.000000 MazgaDB-0.0.2.1/MazgaDB_func/delete.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      467 2023-05-22 09:21:29.000000 MazgaDB-0.0.2.1/MazgaDB_func/delete_column.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      187 2023-05-22 09:21:29.000000 MazgaDB-0.0.2.1/MazgaDB_func/is_there.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      400 2023-05-22 09:21:29.000000 MazgaDB-0.0.2.1/MazgaDB_func/new_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      459 2023-05-22 09:21:29.000000 MazgaDB-0.0.2.1/MazgaDB_func/read_all.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      251 2023-05-22 09:21:29.000000 MazgaDB-0.0.2.1/MazgaDB_func/select.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      235 2023-05-22 09:21:29.000000 MazgaDB-0.0.2.1/MazgaDB_func/update.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8779 2023-06-02 10:24:21.212477 MazgaDB-0.0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     5940 2023-06-02 10:06:20.000000 MazgaDB-0.0.2.1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 10:24:21.212477 MazgaDB-0.0.2.1/mazga_db/
+-rw-r--r--   0 runner    (1000) runner    (1000)     5547 2023-06-02 10:21:21.000000 MazgaDB-0.0.2.1/mazga_db/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      368 2023-05-22 09:24:18.000000 MazgaDB-0.0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-02 10:24:21.212477 MazgaDB-0.0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      762 2023-06-02 10:22:59.000000 MazgaDB-0.0.2.1/setup.py
```

### Comparing `MazgaDB-0.0.2/MazgaDB.egg-info/PKG-INFO` & `MazgaDB-0.0.2.1/MazgaDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MazgaDB
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: ОРМ для базы данных SQlite
 Home-page: https://github.com/Mazgagzam/MazgaDB
 Author: Mazga
 Author-email: agzamikail@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/Mazgagzam/MazgaDB
 Description: # Documentation MazgaDB
```

### Comparing `MazgaDB-0.0.2/MazgaDB_func/class_db.py` & `MazgaDB-0.0.2.1/MazgaDB_func/class_db.py`

 * *Files identical despite different names*

### Comparing `MazgaDB-0.0.2/PKG-INFO` & `MazgaDB-0.0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MazgaDB
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: ОРМ для базы данных SQlite
 Home-page: https://github.com/Mazgagzam/MazgaDB
 Author: Mazga
 Author-email: agzamikail@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/Mazgagzam/MazgaDB
 Description: # Documentation MazgaDB
```

### Comparing `MazgaDB-0.0.2/README.md` & `MazgaDB-0.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `MazgaDB-0.0.2/mazga_db/__init__.py` & `MazgaDB-0.0.2.1/mazga_db/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     def select_class(self, name_table: str, key: str, value, class_data=None) -> object:
         data = self.execute(f'SELECT * FROM {name_table} WHERE {key} = {value}')[0]
         if class_data:
             return class_data(*data)
         elif name_table in self.data_class:
             return self.data_class[name_table](*data)
         else:
-            class_ = make_dataclass(cls_name=name_table.title(), fields=self.accept_type_columns(name_table), namespace={'__save__': lambda self1: __save__(self, self1, name_table)})
+            class_ = make_dataclass(cls_name=name_table.title(), fields=self.accept_type_columns(name_table), namespace={'__call__': lambda self1: __save__(self, self1, name_table)})
             return class_(*data)
 
     def select(self, name_table: str, key: str, value):
         """
         Обычный SELECT из sqlite3
         :param name_table:
         :param key:
```

### Comparing `MazgaDB-0.0.2/setup.py` & `MazgaDB-0.0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 setup(
     name="MazgaDB",
-    version="0.0.2",
+    version="0.0.2.1",
     author="Mazga",
     author_email="agzamikail@gmail.com",
     description="ОРМ для базы данных SQlite",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/Mazgagzam/MazgaDB",
     packages= find_packages(),
```

