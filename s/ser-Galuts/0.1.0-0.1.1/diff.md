# Comparing `tmp/ser_Galuts-0.1.0.tar.gz` & `tmp/ser_Galuts-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ser_Galuts-0.1.0.tar", last modified: Fri May 19 16:27:01 2023, max compression
+gzip compressed data, was "ser_Galuts-0.1.1.tar", last modified: Fri Jun  2 19:38:05 2023, max compression
```

## Comparing `ser_Galuts-0.1.0.tar` & `ser_Galuts-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 16:27:01.353801 ser_Galuts-0.1.0/
--rw-rw-rw-   0        0        0      393 2023-05-19 16:27:01.352799 ser_Galuts-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-19 16:05:09.000000 ser_Galuts-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 16:27:01.334118 ser_Galuts-0.1.0/ser_Anton/
--rw-rw-rw-   0        0        0     1430 2023-05-17 15:02:35.000000 ser_Galuts-0.1.0/ser_Anton/constants.py
--rw-rw-rw-   0        0        0      384 2023-05-19 16:20:06.000000 ser_Galuts-0.1.0/ser_Anton/factory.py
--rw-rw-rw-   0        0        0     2975 2023-05-19 16:20:06.000000 ser_Galuts-0.1.0/ser_Anton/json_serializer.py
--rw-rw-rw-   0        0        0     8809 2023-05-19 16:20:06.000000 ser_Galuts-0.1.0/ser_Anton/serializersi.py
--rw-rw-rw-   0        0        0     2981 2023-05-19 16:20:06.000000 ser_Galuts-0.1.0/ser_Anton/xml_serializer.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:27:01.351798 ser_Galuts-0.1.0/ser_Galuts.egg-info/
--rw-rw-rw-   0        0        0      393 2023-05-19 16:27:01.000000 ser_Galuts-0.1.0/ser_Galuts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-05-19 16:27:01.000000 ser_Galuts-0.1.0/ser_Galuts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 16:27:01.000000 ser_Galuts-0.1.0/ser_Galuts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-19 16:27:01.000000 ser_Galuts-0.1.0/ser_Galuts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 16:27:01.000000 ser_Galuts-0.1.0/ser_Galuts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 16:27:01.353801 ser_Galuts-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1031 2023-05-19 16:26:46.000000 ser_Galuts-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:38:05.277915 ser_Galuts-0.1.1/
+-rw-rw-rw-   0        0        0      445 2023-06-02 19:38:05.276914 ser_Galuts-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-19 16:05:09.000000 ser_Galuts-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 19:38:05.256896 ser_Galuts-0.1.1/ser_Anton/
+-rw-rw-rw-   0        0        0     1430 2023-05-17 15:02:35.000000 ser_Galuts-0.1.1/ser_Anton/constants.py
+-rw-rw-rw-   0        0        0      384 2023-05-19 16:20:06.000000 ser_Galuts-0.1.1/ser_Anton/factory.py
+-rw-rw-rw-   0        0        0     2975 2023-05-19 16:20:06.000000 ser_Galuts-0.1.1/ser_Anton/json_serializer.py
+-rw-rw-rw-   0        0        0     9146 2023-06-02 17:24:05.000000 ser_Galuts-0.1.1/ser_Anton/serializersi.py
+-rw-rw-rw-   0        0        0     2981 2023-05-19 16:20:06.000000 ser_Galuts-0.1.1/ser_Anton/xml_serializer.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:38:05.275912 ser_Galuts-0.1.1/ser_Galuts.egg-info/
+-rw-rw-rw-   0        0        0      445 2023-06-02 19:38:05.000000 ser_Galuts-0.1.1/ser_Galuts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-06-02 19:38:05.000000 ser_Galuts-0.1.1/ser_Galuts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 19:38:05.000000 ser_Galuts-0.1.1/ser_Galuts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-02 19:38:05.000000 ser_Galuts-0.1.1/ser_Galuts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-02 19:38:05.000000 ser_Galuts-0.1.1/ser_Galuts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 19:38:05.277915 ser_Galuts-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-06-02 19:36:43.000000 ser_Galuts-0.1.1/setup.py
```

### Comparing `ser_Galuts-0.1.0/ser_Anton/constants.py` & `ser_Galuts-0.1.1/ser_Anton/constants.py`

 * *Files identical despite different names*

### Comparing `ser_Galuts-0.1.0/ser_Anton/json_serializer.py` & `ser_Galuts-0.1.1/ser_Anton/json_serializer.py`

 * *Files identical despite different names*

### Comparing `ser_Galuts-0.1.0/ser_Anton/serializersi.py` & `ser_Galuts-0.1.1/ser_Anton/serializersi.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,28 @@
         return serialize_function(obj)
     elif inspect.iscode(obj):
         return serialize_code(obj)
     elif isinstance(obj, types.CellType):
         return serialize_cell(obj)
     elif inspect.isclass(obj):
         return serialize_class(obj)
+    elif iteration_check(obj):
+        return serialize_iter_objects(obj)
     else:
         return serialize_object(obj)
 
 
+def iteration_check(obj):
+    return hasattr(obj, "__next__") and hasattr(obj, "__iter__") and callable(obj.__iter__)
+
+def serialize_iter_objects(obj):
+    data = list(map(serialize, obj))
+    iter_data = {"type": "iterator", "value": data}
+    return iter_data
+
 def get_obj_type(obj):
     obj_type = str(type(obj))
     return obj_type[8:-2]
 
 
 def serialize_single_var(obj):
     data = {"type": get_obj_type(obj), "value": obj}
@@ -135,16 +145,14 @@
             data[key] = dict()
             data[key]["type"] = "classmethod"
             data[key]["value"] = {"type": "function", "value": get_function_values(value.__func__, obj)}
 
         elif inspect.ismethod(value):
             data[key] = get_function_values(value.__func__, obj)
 
-
-
         elif inspect.isfunction(value):
             data[key] = dict()
             data[key]["type"] = "function"
             data[key]["value"] = get_function_values(value, obj)
 
         else:
             data[key] = serialize(value)
@@ -301,8 +309,7 @@
 
     return des
 
 
 def main():
     pass
 
-main()
```

### Comparing `ser_Galuts-0.1.0/ser_Anton/xml_serializer.py` & `ser_Galuts-0.1.1/ser_Anton/xml_serializer.py`

 * *Files identical despite different names*

### Comparing `ser_Galuts-0.1.0/setup.py` & `ser_Galuts-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="ser_Galuts",
-    version="0.1.0",
+    version="0.1.1",
     description="somme serialization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Galuts Anton",
     author_email="lil_evac@mail.ru",
     license="MIT",
     classifiers=[
```

