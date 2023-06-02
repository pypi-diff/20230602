# Comparing `tmp/y4d-0.1.3.tar.gz` & `tmp/y4d-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y4d-0.1.3.tar", max compression
+gzip compressed data, was "y4d-0.1.4.tar", max compression
```

## Comparing `y4d-0.1.3.tar` & `y4d-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      580 2023-06-02 19:27:54.053264 y4d-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      217 2023-05-31 19:18:03.375800 y4d-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-27 19:23:01.005617 y4d-0.1.3/y4d/__init__.py
--rw-r--r--   0        0        0     1560 2023-06-02 19:25:50.118169 y4d-0.1.3/y4d/checkAPI.py
--rw-r--r--   0        0        0    15622 2023-06-02 19:26:26.479741 y4d-0.1.3/y4d/codeParser.py
--rw-r--r--   0        0        0     8160 2023-06-02 19:26:45.386030 y4d-0.1.3/y4d/commentController.py
--rw-r--r--   0        0        0     7187 2023-06-02 19:27:05.105316 y4d-0.1.3/y4d/isolator.py
--rw-r--r--   0        0        0    35173 2023-06-02 19:27:27.852256 y4d-0.1.3/y4d/restrictor.py
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 y4d-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      580 2023-06-02 19:50:47.924343 y4d-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      217 2023-05-31 19:18:03.375800 y4d-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 19:23:01.005617 y4d-0.1.4/y4d/__init__.py
+-rw-r--r--   0        0        0     1560 2023-06-02 19:25:50.118169 y4d-0.1.4/y4d/checkAPI.py
+-rw-r--r--   0        0        0    14732 2023-06-02 19:51:03.806133 y4d-0.1.4/y4d/codeParser.py
+-rw-r--r--   0        0        0     8160 2023-06-02 19:26:45.386030 y4d-0.1.4/y4d/commentController.py
+-rw-r--r--   0        0        0     7354 2023-06-02 19:51:25.780979 y4d-0.1.4/y4d/isolator.py
+-rw-r--r--   0        0        0    35173 2023-06-02 19:27:27.852256 y4d-0.1.4/y4d/restrictor.py
+-rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 y4d-0.1.4/PKG-INFO
```

### Comparing `y4d-0.1.3/pyproject.toml` & `y4d-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "y4d"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["BahouA <antonbahou@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 checkAPI = "y4d.checkAPI:app"
 restrict = "y4d.restrictor:app"
```

### Comparing `y4d-0.1.3/y4d/checkAPI.py` & `y4d-0.1.4/y4d/checkAPI.py`

 * *Files identical despite different names*

### Comparing `y4d-0.1.3/y4d/codeParser.py` & `y4d-0.1.4/y4d/codeParser.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,14 @@
 from pathlib import Path
 
 def findLocationFunction(data, prototype: str, source):
     #Check for static, virtual, pure virtual, and constructors
     is_static = False
     is_pure = False
     is_virtual = False
-    has_initializer = "false"
-    
-    #Check constructors with initializer lists
-    if len(prototype.split("(")) > 2:
-        has_initializer = "true" 
 
     #Check static functions
     if len(prototype.split("static")) > 1:
         is_static= True
 
     #Check virtual and pure virtual functions
     if len(prototype.split("virtual")) > 1:
@@ -35,15 +30,14 @@
             type = "template_member_function"
         else:
             type = "template_function"
     elif len(prototype.split("::")) > 1:
         type = "member_function"
     else:
         type="function"
-    
     #Extract information from function prototype
     if type == "member_function" or type == "template_member_function":
         parent_class = prototype.split("::")[0].strip().split(" ")[-1]
         returntype = prototype.split(parent_class)[0]
         prototype=prototype.replace(" ", "")
         name = prototype.split("::")[1].split("(")[0]
         if len(name.split("~")) > 1 and name.split("~")[1] == parent_class:
@@ -55,16 +49,15 @@
             prototype = prototype.split(">")[1].strip()
         name = prototype.split('(')[0].split(" ")[-1].strip()
         returntype = prototype.split(name)[0].strip()
         
     if type == "constructor" or type == "decstructor":
         returntype = "void"
         params = "(" + prototype.split("::")[1].split("(")[1]
-        if has_initializer == "true": 
-            params = params.split(":")[0]
+
     else:
         params = prototype.split(name)[1]
         
     qualtype = returntype + params
     qualtype = qualtype.replace(" ", "")
 
     #Retrieve position of function
@@ -115,15 +108,15 @@
                                     break
                         i = i+1
                         if end != -1:
                             break
                     pos += [start, end, type, item['access_type']] 
     if type == "constructor":
         for item in data['nodes']:
-            if item['kind'] == "CONSTRUCTOR" and item['spelling'].replace(" ", "") == name and item['prototype'].replace(" ", "").split(")")[0]+")"  == qualtype and item['initializer_list'] == has_initializer:
+            if item['kind'] == "CONSTRUCTOR" and item['spelling'].replace(" ", "") == name and item['prototype'].replace(" ", "").split(")")[0]+")" == qualtype:
                 end = item['end']
                 start = item['start']
                 pos += [start, end, type, item['access_type']] 
     if type == "decstructor":
         for item in data['nodes']:
             if item['kind'] == "DESTRUCTOR" and item['spelling'].replace(" ", "") == name:
                 end = item['end']
@@ -159,33 +152,31 @@
                     if item['col'] <= 12:
                         start -= 1
                     end = item['end']
                     class_start = start 
                     class_end = end
                     pos+=[start, end, type, ""]
                     flag =1
-                
             if flag  == 0 : 
                 i = i+1
                 continue
             elif iteration == -1:
                 return pos  
             #check member functions implemented outside the class
             if item['start'] < class_start or item['end'] > class_end:
                 if item['mangled_name'].startswith('?'):
                     mangledName= item['mangled_name'].split("@")
                     if len(mangledName) > 1 and mangledName[1] == name:
                         if item['kind'] == "CXX_METHOD":
-                            returnType = item['prototype'].split(" ")[0].strip()
+                            returnType = item['prototype'].split("(")[0].strip()
                             func_prototype = returnType +" " + name + "::" +item['displayname']
                             pos+= findLocationFunction(data, func_prototype, source)
                     if item['kind'] == "CONSTRUCTOR" or item['kind'] =="DESTRUCTOR":
                         returnType = "void"
                         func_prototype = name+"::" +item['displayname']
-                        print(func_prototype)
                         pos+= findLocationFunction(data, func_prototype, source)
             #check template member functions  
             if item["kind"] == "FUNCTION_TEMPLATE":
                 start_line = item['start']
                 j = i+1
                 template_node = data['nodes'][j]
                 while  j < len(data['nodes']) and template_node['start'] == start_line:
@@ -210,25 +201,14 @@
                     end = item['end']
                     classes +=  [type + " "+  item['spelling']]
             i = i+1
         if iteration == 1:
             return pos
 
     return pos
- 
-
-
-#find if a constructor has expression initializer list
-def hasInitializerList(cursor):
-    for child in cursor.get_children():
-        if child.kind.is_expression():
-            return True
-    return False
-
-
 
 #Compile code and return parse tree
 def prepareData (source: str):
     
     #Get Code from source
     with open(source, 'r') as file:
         source = file.read()
@@ -242,20 +222,14 @@
         
     output = {"nodes": []}
     friendFlag = False
     classPointer = -1
     for node in tu.cursor.walk_preorder():
         access_type =""
         parent_class = ""
-        initializer_list = "false"
-
-        #Check if the constructor has an expression initializer list
-        if node.kind == clang.cindex.CursorKind.CONSTRUCTOR:
-            if hasInitializerList(node):
-                initializer_list = "true"
                 
         #Save access type of member functions, anything else will have value "invalid"              
         access_type = str(node.access_specifier).split(".")[1]
         #Save name of parent class
         if access_type == "INVALID":
             parent_class = ""
         else:
@@ -303,22 +277,21 @@
             "is_virtual_method": node.is_virtual_method(),
             "is_pure": node.is_pure_virtual_method(),
             "is_struct": node.kind == clang.cindex.CursorKind.STRUCT_DECL,
             "is_class": node.kind == clang.cindex.CursorKind.CLASS_DECL,
             "inherits_from": [],
             "friend_with": [],
             "access_type" : access_type.lower(),
-            "parent_class" : parent_class,
-            "initializer_list" : initializer_list,
+            "parent_class" : parent_class
         }
         output["nodes"].append(node_dict)
     
     jsonFormat = json.dumps(output, indent=4)
     data = json.loads(jsonFormat)
-
+    
     return data
 
 
 #Return postions of anything the user is searching for.
 def positions ( source: str, type: str, prototype: str, option = 0):
     source_path = Path(source)
     if source_path.exists() == False:
@@ -344,8 +317,8 @@
     
     if type == "class" or type == "struct":
         pos = findLocationClass(data, prototype , source, type, option)  
         
     if type == "function":
         pos = findLocationFunction( data, prototype, source)  
         
-    return pos
+    return pos
```

### Comparing `y4d-0.1.3/y4d/commentController.py` & `y4d-0.1.4/y4d/commentController.py`

 * *Files identical despite different names*

### Comparing `y4d-0.1.3/y4d/isolator.py` & `y4d-0.1.4/y4d/isolator.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,19 @@
             if findClass == ["error"]:
                 return
             if findClass == []:
                 print("Warning: Parent Class doesn't exist in " +destination +" file")
                 return 
         class_end = findClass[1]
         #fixing protoype
-        forward_implementation = prototype.split(parent_class)[0] + prototype.split(parent_class)[1]
-        forward_implementation = forward_implementation.split("::")[0] + forward_implementation.split("::")[1]
+        if findFunction[2] == "constructor" or findFunction[2] == "destructor":
+            forward_implementation = prototype.split("::")[1]
+        else:
+            forward_implementation = prototype.split(parent_class)[0] + prototype.split(parent_class)[1]
+            forward_implementation = forward_implementation.split("::")[0] + forward_implementation.split("::")[1]
     
     #commenting out the function in destination file
     commentController.CommentOutFunction(destination, prototype, 1, destination)
     
     #case: forward declaration or memebr functions implemented outside a class
     i=0
     if len(findFunction) > 4:
```

### Comparing `y4d-0.1.3/y4d/restrictor.py` & `y4d-0.1.4/y4d/restrictor.py`

 * *Files identical despite different names*

### Comparing `y4d-0.1.3/PKG-INFO` & `y4d-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y4d
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: BahouA
 Author-email: antonbahou@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

