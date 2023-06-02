# Comparing `tmp/ser_Galuts-0.1.1.tar.gz` & `tmp/ser_Galuts-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ser_Galuts-0.1.1.tar", last modified: Fri Jun  2 19:38:05 2023, max compression
+gzip compressed data, was "ser_Galuts-0.1.2.tar", last modified: Fri Jun  2 20:06:31 2023, max compression
```

## Comparing `ser_Galuts-0.1.1.tar` & `ser_Galuts-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 19:38:05.277915 ser_Galuts-0.1.1/
--rw-rw-rw-   0        0        0      445 2023-06-02 19:38:05.276914 ser_Galuts-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-19 16:05:09.000000 ser_Galuts-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 19:38:05.256896 ser_Galuts-0.1.1/ser_Anton/
--rw-rw-rw-   0        0        0     1430 2023-05-17 15:02:35.000000 ser_Galuts-0.1.1/ser_Anton/constants.py
--rw-rw-rw-   0        0        0      384 2023-05-19 16:20:06.000000 ser_Galuts-0.1.1/ser_Anton/factory.py
--rw-rw-rw-   0        0        0     2975 2023-05-19 16:20:06.000000 ser_Galuts-0.1.1/ser_Anton/json_serializer.py
--rw-rw-rw-   0        0        0     9146 2023-06-02 17:24:05.000000 ser_Galuts-0.1.1/ser_Anton/serializersi.py
--rw-rw-rw-   0        0        0     2981 2023-05-19 16:20:06.000000 ser_Galuts-0.1.1/ser_Anton/xml_serializer.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:38:05.275912 ser_Galuts-0.1.1/ser_Galuts.egg-info/
--rw-rw-rw-   0        0        0      445 2023-06-02 19:38:05.000000 ser_Galuts-0.1.1/ser_Galuts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-06-02 19:38:05.000000 ser_Galuts-0.1.1/ser_Galuts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 19:38:05.000000 ser_Galuts-0.1.1/ser_Galuts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-02 19:38:05.000000 ser_Galuts-0.1.1/ser_Galuts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-02 19:38:05.000000 ser_Galuts-0.1.1/ser_Galuts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 19:38:05.277915 ser_Galuts-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1031 2023-06-02 19:36:43.000000 ser_Galuts-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:06:31.205839 ser_Galuts-0.1.2/
+-rw-rw-rw-   0        0        0      445 2023-06-02 20:06:31.205839 ser_Galuts-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-19 16:05:09.000000 ser_Galuts-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 20:06:31.197951 ser_Galuts-0.1.2/ser_Anton/
+-rw-rw-rw-   0        0        0     1430 2023-05-17 15:02:35.000000 ser_Galuts-0.1.2/ser_Anton/constants.py
+-rw-rw-rw-   0        0        0      384 2023-05-19 16:20:06.000000 ser_Galuts-0.1.2/ser_Anton/factory.py
+-rw-rw-rw-   0        0        0     2975 2023-05-19 16:20:06.000000 ser_Galuts-0.1.2/ser_Anton/json_serializer.py
+-rw-rw-rw-   0        0        0     9345 2023-06-02 20:00:34.000000 ser_Galuts-0.1.2/ser_Anton/serializersi.py
+-rw-rw-rw-   0        0        0     2981 2023-05-19 16:20:06.000000 ser_Galuts-0.1.2/ser_Anton/xml_serializer.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:06:31.204839 ser_Galuts-0.1.2/ser_Galuts.egg-info/
+-rw-rw-rw-   0        0        0      445 2023-06-02 20:06:31.000000 ser_Galuts-0.1.2/ser_Galuts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-06-02 20:06:31.000000 ser_Galuts-0.1.2/ser_Galuts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 20:06:31.000000 ser_Galuts-0.1.2/ser_Galuts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-02 20:06:31.000000 ser_Galuts-0.1.2/ser_Galuts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-02 20:06:31.000000 ser_Galuts-0.1.2/ser_Galuts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 20:06:31.205839 ser_Galuts-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-06-02 20:02:31.000000 ser_Galuts-0.1.2/setup.py
```

### Comparing `ser_Galuts-0.1.1/ser_Anton/constants.py` & `ser_Galuts-0.1.2/ser_Anton/constants.py`

 * *Files identical despite different names*

### Comparing `ser_Galuts-0.1.1/ser_Anton/json_serializer.py` & `ser_Galuts-0.1.2/ser_Anton/json_serializer.py`

 * *Files identical despite different names*

### Comparing `ser_Galuts-0.1.1/ser_Anton/serializersi.py` & `ser_Galuts-0.1.2/ser_Anton/serializersi.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,17 @@
 
     elif obj["type"] == "class":
         return deserialize_class(obj["value"])
 
     elif obj["type"] in METHODS:
         return METHODS[obj["type"]](deserialize(obj["value"]))
 
+    elif obj["type"] == "iterator":
+        return deserialize_iter_objects(obj)
+
     elif obj["type"] == "object":
         return deserialize_object(obj["value"])
 
 
 def deserialize_base_type(obj):
     return PRIMITIVES[obj["type"]](obj["value"])
 
@@ -239,14 +242,18 @@
     elif obj["type"] == "bytearray":
         return bytearray(map(deserialize, obj["value"]))
     elif obj["type"] == "dict":
         data = {deserialize(item[0]): deserialize(item[1]) for item in obj["value"]}
         return data
 
 
+def deserialize_iter_objects(obj):
+    data = obj["value"]
+    return iter(deserialize(val) for val in data)
+
 def deserialize_code(code):
     return types.CodeType(*(deserialize(code[prop]) for prop in CODE_PROPERTIES))
 
 
 def deserialize_function(func):
     code = func["__code__"]
     globs = func["__globals__"]
```

### Comparing `ser_Galuts-0.1.1/ser_Anton/xml_serializer.py` & `ser_Galuts-0.1.2/ser_Anton/xml_serializer.py`

 * *Files identical despite different names*

### Comparing `ser_Galuts-0.1.1/setup.py` & `ser_Galuts-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="ser_Galuts",
-    version="0.1.1",
+    version="0.1.2",
     description="somme serialization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Galuts Anton",
     author_email="lil_evac@mail.ru",
     license="MIT",
     classifiers=[
```

