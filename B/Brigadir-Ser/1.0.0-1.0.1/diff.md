# Comparing `tmp/Brigadir_Ser-1.0.0.tar.gz` & `tmp/Brigadir_Ser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Brigadir_Ser-1.0.0.tar", last modified: Fri Jun  2 14:29:44 2023, max compression
+gzip compressed data, was "Brigadir_Ser-1.0.1.tar", last modified: Fri Jun  2 14:53:02 2023, max compression
```

## Comparing `Brigadir_Ser-1.0.0.tar` & `Brigadir_Ser-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 14:29:44.574345 Brigadir_Ser-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-06-02 14:29:44.564382 Brigadir_Ser-1.0.0/Brigadir_Ser.egg-info/
--rw-rw-rw-   0        0        0      157 2023-06-02 14:29:44.000000 Brigadir_Ser-1.0.0/Brigadir_Ser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-06-02 14:29:44.000000 Brigadir_Ser-1.0.0/Brigadir_Ser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 14:29:44.000000 Brigadir_Ser-1.0.0/Brigadir_Ser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-02 14:29:44.000000 Brigadir_Ser-1.0.0/Brigadir_Ser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-06-02 14:29:44.000000 Brigadir_Ser-1.0.0/Brigadir_Ser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 14:29:44.571345 Brigadir_Ser-1.0.0/MySerializer/
--rw-rw-rw-   0        0        0      341 2023-05-31 14:10:28.000000 Brigadir_Ser-1.0.0/MySerializer/MySerializer.py
--rw-rw-rw-   0        0        0        0 2023-05-31 14:10:28.000000 Brigadir_Ser-1.0.0/MySerializer/__init__.py
--rw-rw-rw-   0        0        0       88 2023-05-31 14:10:28.000000 Brigadir_Ser-1.0.0/MySerializer/constants.py
--rw-rw-rw-   0        0        0     6775 2023-05-31 14:10:28.000000 Brigadir_Ser-1.0.0/MySerializer/json_utils.py
--rw-rw-rw-   0        0        0     5200 2023-05-31 14:10:28.000000 Brigadir_Ser-1.0.0/MySerializer/pack_utils.py
--rw-rw-rw-   0        0        0     1339 2023-05-31 14:10:28.000000 Brigadir_Ser-1.0.0/MySerializer/serializer.py
--rw-rw-rw-   0        0        0     6823 2023-05-31 14:10:28.000000 Brigadir_Ser-1.0.0/MySerializer/unpack_utils.py
--rw-rw-rw-   0        0        0     6789 2023-05-31 14:10:28.000000 Brigadir_Ser-1.0.0/MySerializer/xml_utils.py
--rw-rw-rw-   0        0        0      157 2023-06-02 14:29:44.574345 Brigadir_Ser-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-21 11:50:46.000000 Brigadir_Ser-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-02 14:29:44.574345 Brigadir_Ser-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      418 2023-06-02 14:27:03.000000 Brigadir_Ser-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 14:29:44.573345 Brigadir_Ser-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-05-21 11:50:46.000000 Brigadir_Ser-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0      905 2023-05-31 14:10:28.000000 Brigadir_Ser-1.0.0/tests/test_attributes.py
--rw-rw-rw-   0        0        0     6558 2023-05-31 14:10:28.000000 Brigadir_Ser-1.0.0/tests/unitest.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:53:02.336517 Brigadir_Ser-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-06-02 14:53:02.295525 Brigadir_Ser-1.0.1/Brigada/
+-rw-rw-rw-   0        0        0      326 2023-06-02 14:51:40.000000 Brigadir_Ser-1.0.1/Brigada/MySerializer.py
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:44:26.000000 Brigadir_Ser-1.0.1/Brigada/__init__.py
+-rw-rw-rw-   0        0        0       88 2023-05-31 14:10:28.000000 Brigadir_Ser-1.0.1/Brigada/constants.py
+-rw-rw-rw-   0        0        0     6760 2023-06-02 14:51:31.000000 Brigadir_Ser-1.0.1/Brigada/json_utils.py
+-rw-rw-rw-   0        0        0     5195 2023-06-02 14:51:40.000000 Brigadir_Ser-1.0.1/Brigada/pack_utils.py
+-rw-rw-rw-   0        0        0     1314 2023-06-02 14:51:40.000000 Brigadir_Ser-1.0.1/Brigada/serializer.py
+-rw-rw-rw-   0        0        0     6818 2023-06-02 14:51:40.000000 Brigadir_Ser-1.0.1/Brigada/unpack_utils.py
+-rw-rw-rw-   0        0        0     6774 2023-06-02 14:51:40.000000 Brigadir_Ser-1.0.1/Brigada/xml_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:53:02.323515 Brigadir_Ser-1.0.1/Brigadir_Ser.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-06-02 14:53:02.000000 Brigadir_Ser-1.0.1/Brigadir_Ser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-06-02 14:53:02.000000 Brigadir_Ser-1.0.1/Brigadir_Ser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 14:53:02.000000 Brigadir_Ser-1.0.1/Brigadir_Ser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-02 14:53:02.000000 Brigadir_Ser-1.0.1/Brigadir_Ser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-06-02 14:53:02.000000 Brigadir_Ser-1.0.1/Brigadir_Ser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      157 2023-06-02 14:53:02.335516 Brigadir_Ser-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-21 11:50:46.000000 Brigadir_Ser-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-02 14:53:02.337519 Brigadir_Ser-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-06-02 14:52:52.000000 Brigadir_Ser-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:53:02.333515 Brigadir_Ser-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-21 11:50:46.000000 Brigadir_Ser-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      905 2023-05-31 14:10:28.000000 Brigadir_Ser-1.0.1/tests/test_attributes.py
+-rw-rw-rw-   0        0        0     6558 2023-05-31 14:10:28.000000 Brigadir_Ser-1.0.1/tests/unitest.py
```

### Comparing `Brigadir_Ser-1.0.0/MySerializer/json_utils.py` & `Brigadir_Ser-1.0.1/Brigada/json_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from MySerializer.constants import PRIMITIVES,COLLECTIONS
-from MySerializer.pack_utils import pack
-from MySerializer.unpack_utils import unpack
+from Brigada.constants import PRIMITIVES,COLLECTIONS
+from Brigada.pack_utils import pack
+from Brigada.unpack_utils import unpack
 
 class Json:
     def __init__(self):
         self.pos = 0
         self.indent = 0
 
     def dump(self, obj, fp):
```

### Comparing `Brigadir_Ser-1.0.0/MySerializer/pack_utils.py` & `Brigadir_Ser-1.0.1/Brigada/pack_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 import types
-from MySerializer.constants import PRIMITIVES, COLLECTIONS
+from Brigada.constants import PRIMITIVES, COLLECTIONS
 from types import FunctionType, BuiltinFunctionType, LambdaType, GetSetDescriptorType, MappingProxyType, \
     MethodDescriptorType, WrapperDescriptorType
 
 
 def is_function(obj):
     return inspect.isfunction(obj) or inspect.ismethod(obj) or isinstance(obj, LambdaType)
```

### Comparing `Brigadir_Ser-1.0.0/MySerializer/serializer.py` & `Brigadir_Ser-1.0.1/Brigada/serializer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from argparse import ArgumentParser
-from MySerializer.MySerializer import MySerializer
+from Brigada.Brigada import Brigada
 
 def main():
     try:
         parse = ArgumentParser()
         parse.add_argument('file_from',type=str, help='file from which you load data')    
         parse.add_argument('file_to',type=str, help='file to which you save serialized data')
         parse.add_argument('format_from',type=str, help='format from which you deserialize data, can be any of json/xml')
@@ -15,16 +15,16 @@
             print("File from and file to are the same. Please check your data and try again")
             exit()
 
         if args.format_from == args.format_to:
             print("Format from and format to are the same. Please check your data and try again")
             exit()
 
-        from_serializer = MySerializer.createSerializer(args.format_from)
-        to_serializer = MySerializer.createSerializer(args.format_to)
+        from_serializer = Brigada.createSerializer(args.format_from)
+        to_serializer = Brigada.createSerializer(args.format_to)
 
         with open(args.file_from) as file:
             obj = from_serializer.load(file)
             with open(args.file_to, "w") as output_file:
                 to_serializer.dump(obj, output_file)
     except Exception as e:
         print(e)
```

### Comparing `Brigadir_Ser-1.0.0/MySerializer/unpack_utils.py` & `Brigadir_Ser-1.0.1/Brigada/unpack_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 import builtins
 import types
-from MySerializer.constants import PRIMITIVES
+from Brigada.constants import PRIMITIVES
 from types import FunctionType, LambdaType, CodeType, CellType, GeneratorType, ModuleType
 
 def is_function(obj):
     return inspect.isfunction(obj) or inspect.ismethod(obj) or isinstance(obj, LambdaType)
 
 
 def is_iterable(obj):
```

### Comparing `Brigadir_Ser-1.0.0/MySerializer/xml_utils.py` & `Brigadir_Ser-1.0.1/Brigada/xml_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from MySerializer.constants import PRIMITIVES,COLLECTIONS
-from MySerializer.pack_utils import pack
-from MySerializer.unpack_utils import unpack
+from Brigada.constants import PRIMITIVES,COLLECTIONS
+from Brigada.pack_utils import pack
+from Brigada.unpack_utils import unpack
 
 
 class Xml:
     def __init__(self):
         self.pos = 0
         self.indent = 0
```

### Comparing `Brigadir_Ser-1.0.0/tests/test_attributes.py` & `Brigadir_Ser-1.0.1/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `Brigadir_Ser-1.0.0/tests/unitest.py` & `Brigadir_Ser-1.0.1/tests/unitest.py`

 * *Files identical despite different names*

