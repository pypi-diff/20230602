# Comparing `tmp/y4d-0.1.2.tar.gz` & `tmp/y4d-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y4d-0.1.2.tar", max compression
+gzip compressed data, was "y4d-0.1.3.tar", max compression
```

## Comparing `y4d-0.1.2.tar` & `y4d-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      580 2023-05-31 19:18:15.778486 y4d-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      217 2023-05-31 19:18:03.375800 y4d-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-27 19:23:01.005617 y4d-0.1.2/y4d/__init__.py
--rw-r--r--   0        0        0     1573 2023-05-31 19:18:56.287396 y4d-0.1.2/y4d/checkAPI.py
--rw-r--r--   0        0        0    14966 2023-05-31 19:21:03.766957 y4d-0.1.2/y4d/codeParser.py
--rw-r--r--   0        0        0     7277 2023-05-31 19:20:33.375528 y4d-0.1.2/y4d/commentController.py
--rw-r--r--   0        0        0     6446 2023-05-31 19:20:08.431889 y4d-0.1.2/y4d/isolator.py
--rw-r--r--   0        0        0    34273 2023-05-31 19:19:31.594710 y4d-0.1.2/y4d/restrictor.py
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 y4d-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      580 2023-06-02 19:27:54.053264 y4d-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      217 2023-05-31 19:18:03.375800 y4d-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 19:23:01.005617 y4d-0.1.3/y4d/__init__.py
+-rw-r--r--   0        0        0     1560 2023-06-02 19:25:50.118169 y4d-0.1.3/y4d/checkAPI.py
+-rw-r--r--   0        0        0    15622 2023-06-02 19:26:26.479741 y4d-0.1.3/y4d/codeParser.py
+-rw-r--r--   0        0        0     8160 2023-06-02 19:26:45.386030 y4d-0.1.3/y4d/commentController.py
+-rw-r--r--   0        0        0     7187 2023-06-02 19:27:05.105316 y4d-0.1.3/y4d/isolator.py
+-rw-r--r--   0        0        0    35173 2023-06-02 19:27:27.852256 y4d-0.1.3/y4d/restrictor.py
+-rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 y4d-0.1.3/PKG-INFO
```

### Comparing `y4d-0.1.2/pyproject.toml` & `y4d-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "y4d"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["BahouA <antonbahou@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 checkAPI = "y4d.checkAPI:app"
 restrict = "y4d.restrictor:app"
```

### Comparing `y4d-0.1.2/y4d/checkAPI.py` & `y4d-0.1.3/y4d/checkAPI.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import typer
 from y4d import restrictor as restrictor
 
 app = typer.Typer()
 
 #Function to restrict a single (private/public/protected) function, no need for the YAML file, further explanation available exactly below function definition.
 @app.command("")
-def main(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants restrictor to work on."),
-        compare: str = typer.Argument(..., help="The path of the .cpp or .h file the user wants the source file to be compared to."),
+def main(compare: str = typer.Argument(..., help="The path of the .cpp or .h file the user wants the source file to be compared to."),
+         source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants restrictor to work on."),
         restriction: str = typer.Argument(..., help="The restriction type used for 2 ways of checking:\n\nat_least: Everything being checked must exist (It can be with other functions/classes).\n\nexactly: Everything being checked must only exist (It can not be with other functions/classes)."),
         output: str  = typer.Option("n", "-o", help="If n this will make checkAPI print the number of missing functions/classes then extra functions/classes, Input V if you want a list of violations to be printed and more information (default is n) (Takes only v or V or n or N)."),
         hide:bool = typer.Argument(False, hidden=True, help="A hidden variable for developers use, used to return extra functions and classes found in the code.")):
     """
-    This tool will compare two files together, the source and compare file, it will check if the function prototypes and class names match then return true or false accordingly.
+    Compares two files together, the source and compare file, it will check if the function prototypes and class names match then return true or false accordingly.
     """
     restrictor.checkAPI(source, restriction, compare, output, hide)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `y4d-0.1.2/y4d/codeParser.py` & `y4d-0.1.3/y4d/codeParser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import clang.cindex
+from clang.cindex import CursorKind
 import re
 from pathlib import Path
 
 def findLocationFunction(data, prototype: str, source):
     #Check for static, virtual, pure virtual, and constructors
     is_static = False
     is_pure = False
@@ -38,15 +39,15 @@
         type = "member_function"
     else:
         type="function"
     
     #Extract information from function prototype
     if type == "member_function" or type == "template_member_function":
         parent_class = prototype.split("::")[0].strip().split(" ")[-1]
-        returntype = prototype.split(parent_class)[0].strip().split(" ")[-1]
+        returntype = prototype.split(parent_class)[0]
         prototype=prototype.replace(" ", "")
         name = prototype.split("::")[1].split("(")[0]
         if len(name.split("~")) > 1 and name.split("~")[1] == parent_class:
             type = "decstructor"
         if name == parent_class:
             type = "constructor"   
     else:
@@ -70,15 +71,19 @@
     pos=[]
     if type == "function":
         for item in data['nodes']:
             if item['kind'] == "FUNCTION_DECL" and item['spelling'].replace(" ", "") == name and item['prototype'].replace(" ", "") == qualtype:
                 if is_static == item['is_static_method'] and is_virtual == item['is_virtual_method'] and is_pure == item['is_pure']:
                     end = item['end']
                     start = item['start']
-                    pos += [start, end, type, item['access_type']]
+                    if name == "main":
+                        pos += [start, end, "main", item['access_type']]
+                    else:
+                        pos += [start, end, type, item['access_type']]
+                    
     if type == "member_function":
         for item in data['nodes']:
             if item['kind'] == "CXX_METHOD" and item['spelling'].replace(" ", "") == name and item['prototype'].replace(" ", "") == qualtype and item['parent_class']!="" and parent_class == item['parent_class'].split(" ")[1]:
                 if is_static == item['is_static_method'] and is_virtual == item['is_virtual_method'] and is_pure == item['is_pure']:
                     end = item['end']
                     start = item['start']
                     pos += [start, end, type, item['access_type']]          
@@ -110,15 +115,15 @@
                                     break
                         i = i+1
                         if end != -1:
                             break
                     pos += [start, end, type, item['access_type']] 
     if type == "constructor":
         for item in data['nodes']:
-            if item['kind'] == "CONSTRUCTOR" and item['spelling'].replace(" ", "") == name and item['prototype'].replace(" ", "") == qualtype and item['initializer_list'] == has_initializer:
+            if item['kind'] == "CONSTRUCTOR" and item['spelling'].replace(" ", "") == name and item['prototype'].replace(" ", "").split(")")[0]+")"  == qualtype and item['initializer_list'] == has_initializer:
                 end = item['end']
                 start = item['start']
                 pos += [start, end, type, item['access_type']] 
     if type == "decstructor":
         for item in data['nodes']:
             if item['kind'] == "DESTRUCTOR" and item['spelling'].replace(" ", "") == name:
                 end = item['end']
@@ -158,23 +163,30 @@
                     class_end = end
                     pos+=[start, end, type, ""]
                     flag =1
                 
             if flag  == 0 : 
                 i = i+1
                 continue
+            elif iteration == -1:
+                return pos  
             #check member functions implemented outside the class
             if item['start'] < class_start or item['end'] > class_end:
                 if item['mangled_name'].startswith('?'):
                     mangledName= item['mangled_name'].split("@")
                     if len(mangledName) > 1 and mangledName[1] == name:
                         if item['kind'] == "CXX_METHOD":
-                            returnType = item['prototype'].split(" ")[0]
+                            returnType = item['prototype'].split(" ")[0].strip()
                             func_prototype = returnType +" " + name + "::" +item['displayname']
                             pos+= findLocationFunction(data, func_prototype, source)
+                    if item['kind'] == "CONSTRUCTOR" or item['kind'] =="DESTRUCTOR":
+                        returnType = "void"
+                        func_prototype = name+"::" +item['displayname']
+                        print(func_prototype)
+                        pos+= findLocationFunction(data, func_prototype, source)
             #check template member functions  
             if item["kind"] == "FUNCTION_TEMPLATE":
                 start_line = item['start']
                 j = i+1
                 template_node = data['nodes'][j]
                 while  j < len(data['nodes']) and template_node['start'] == start_line:
                     if template_node['kind'] == "TEMPLATE_TYPE_PARAMETER":
@@ -223,22 +235,23 @@
 
     #String manipulate source for parse to work (removing libraries and using namespace)
     source = re.sub(r'^#include\s*[\s\S][<"]\S+[>"]$', r'// \g<0>', source, flags=re.MULTILINE)
     source = re.sub(r'^\s*using\s+namespace\s+\S+;$', r'// \g<0>', source, flags=re.MULTILINE)
 
     index = clang.cindex.Index.create()
     tu = index.parse('dud.cpp', unsaved_files=[('dud.cpp', source)])
-    
+        
     output = {"nodes": []}
     friendFlag = False
     classPointer = -1
     for node in tu.cursor.walk_preorder():
         access_type =""
         parent_class = ""
         initializer_list = "false"
+
         #Check if the constructor has an expression initializer list
         if node.kind == clang.cindex.CursorKind.CONSTRUCTOR:
             if hasInitializerList(node):
                 initializer_list = "true"
                 
         #Save access type of member functions, anything else will have value "invalid"              
         access_type = str(node.access_specifier).split(".")[1]
@@ -250,28 +263,28 @@
             if parent is None:
                 parent_class=""
             elif parent.kind == clang.cindex.CursorKind.CLASS_DECL:
                 parent_class = "class " + str(parent.spelling)
             elif parent.kind == clang.cindex.CursorKind.STRUCT_DECL:
                 parent_class = "struct " + str(parent.spelling)
             
-        if node.kind == clang.cindex.CursorKind.CLASS_DECL:
+        if node.kind == clang.cindex.CursorKind.CLASS_DECL or node.kind == clang.cindex.CursorKind.STRUCT_DECL:
             classPointer = 0
             friendFlag = False
             
         elif node.kind == clang.cindex.CursorKind.CXX_BASE_SPECIFIER:
             inh = node.spelling
             output["nodes"][classPointer]["inherits_from"].append(inh)
 
         elif node.kind == clang.cindex.CursorKind.FRIEND_DECL:
             friendFlag = True
 
         elif friendFlag:
             friend = node.spelling
-            if len(friend.split("class")) == 1: #check this: or len(friend.split("struct")):
+            if len(friend.split("class")) == 1 or len(friend.split("struct")) ==1:
                 friend = node.type.spelling.split('(')[0] + node.displayname
             output["nodes"][classPointer]["friend_with"].append(friend)
             friendFlag = False
 
         classPointer = classPointer - 1
 
         #Backbone of the project, retuning parse tree information.
@@ -331,8 +344,8 @@
     
     if type == "class" or type == "struct":
         pos = findLocationClass(data, prototype , source, type, option)  
         
     if type == "function":
         pos = findLocationFunction( data, prototype, source)  
         
-    return pos
+    return pos
```

### Comparing `y4d-0.1.2/y4d/commentController.py` & `y4d-0.1.3/y4d/commentController.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
 #This function is responsible for removing all comments from a .cpp or .h file
 @app.command("d")
 def deleteComments(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants delete comments to work on."),
                     output: str  = typer.Option("", "-o", help="The path of the .cpp or .h file the user wants the output to be saved in (Default is printing on the terminal).")):
     """
-    This tool will delete all the comments from a .cpp or .h file and output the source code into the file of your choosing.
+    Deletes all the comments from a .cpp or .h file and output the source code into the file of your choosing.
     """
     with open(source, 'r') as f:
         source = f.read()
     
     # Remove all comments from the input file
     source = re.sub(r'\/\/.*?$|\/\*[\s\S]*?\*\/', '', source, flags=re.MULTILINE)
 
@@ -61,15 +61,15 @@
 
 
 #This function is responsible for extracting all comments from a .cpp or .h file into a file or to print on the terminal
 @app.command("e")
 def extractComments(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants extracts comments to work on."),
                     output: str  = typer.Option("", "-o", help="The path of the .cpp or .h file the user wants the output to be saved in (Default is printing on the terminal).")):
     """
-    This tool will extract all the comments from a C++ file and output the comments into the file of your choosing.
+    Extracts all the comments from a C++ file and output the comments into the file of your choosing.
     """
     with open(source, 'r') as f:
         source = f.read()
     
     # Extract all comments from the input file
     comments = re.findall(r'\/\/.*?$|\/\*[\s\S]*?\*\/', source, flags=re.MULTILINE)
 
@@ -90,15 +90,15 @@
 
 
 #This function is responsible for extracting all header comments from a .cpp or .h file into a file or to print on the terminal
 @app.command("h")
 def extractHeader(input: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants extracts header comments to work on."),
                    output: str  = typer.Option("", "-o", help="The path of the .cpp or .h file the user wants the output to be saved in (Default is printing on the terminal).")):
     """
-    This tool will extract all header comments from a C++ file and output the comments into the file of your choosing.
+    Extracts all header comments from a C++ file and output the comments into the file of your choosing.
     """
     with open(input, 'r') as f:
         source = f.read()
 
     #Find all header comments
     header = re.findall(r'\/\/.*?$|\/\*[\s\S]*?\*\/', source, flags=re.MULTILINE)
     amount = 0
@@ -131,42 +131,65 @@
 
 
 #This function is responsible for commenting out classes specified by the user from a .cpp or .h file
 @app.command("c")
 def CommentOutClass(
     source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants comment out class to work on."),
     prototype: str  = typer.Argument(..., help="The class the user wants to check (Must input like this: \"class name\")."),
-    all: str  = typer.Option("true", "-all", help="If true this will isolate the class with all its children classes"),
+    all: str  = typer.Option("f", "-all", help="If t this will comment out the class with all its children classes, if c this will comment out the class itself without any member function implemented outside the class,if f this will comment out the class with its member functions implemented outside the class. Takes c, t, or f. Default value is f."),
     isolate: int = typer.Argument(0, hidden=True, help="A hidden variable for developers' use, used to show that function was called by isolator."),
     output: str  = typer.Option("", "-o", help="The path of the .cpp or .h file the user wants the output to be saved in (Default is printing on the terminal).")):
     """
-    This tool will comment out a class implementation from a C++ file using a class prototype (equivalent to deleting the class).
+    Comments out a class implementation from a C++ file using a class prototype (equivalent to deleting the class).
     """
-    if all.lower() not in ["true","false"]:
+    if all.lower() not in ["f","t", "c"]:
         print("Invalid input for -all")
         return False
     
     type = prototype.split(" ")[0]
     option = 1
-    if all.lower() == "true":
+    if all == "t":
         option = 0
+    elif all == "c":
+        option = -1
 
     commentMaker(source, type , prototype, isolate, option, output)
 
 
 
 #This function is responsible for commenting out functions specified by the user from a .cpp or .h file
 @app.command("f")
 def CommentOutFunction(
     source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants comment out class to work on."),
     prototype: str  = typer.Argument(..., help="The function the user wants to check (Must input like this: \"int functionName(int, int)\"."),
     isolate: int = typer.Argument(0, hidden=True, help="A hidden variable for developers' use, used to show that function was called by isolator."),
     output: str  = typer.Option("", "-o", help="The path of the .cpp or .h file the user wants the output to be saved in (Default is printing on the terminal).")):
     """
-    This tool will comment out a function implementation from a C++ file using a function prototype (equivalent to deleting the function).
+    Comments out a function implementation from a C++ file using a function prototype (equivalent to deleting the function).
     """
     commentMaker(source, "function" , prototype, isolate, 0, output)
 
 
 
+#This function is responsible for removing all comments from a .cpp or .h file
+def deleteForDeveloper(source: str):
+    """
+    Deletes all the comments from a .cpp or .h file and return the source code.
+    """
+    # Remove all comments from the input file
+    source = re.sub(r'\/\/.*?$|\/\*[\s\S]*?\*\/', '', source, flags=re.MULTILINE)
+
+    return source
+
+
+
+@app.callback()
+def main():
+    """
+    Allows the user to control comments by extracting or removing comments, or by commenting out certain classes or functions.
+    For more information about each tool simply add the command you need followed by --help, for example:\n\n commentCtrl f --help
+    """
+
+
+
 if __name__ == "__main__":
-    app()
+    app()
```

### Comparing `y4d-0.1.2/y4d/isolator.py` & `y4d-0.1.3/y4d/isolator.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 
 
 @app.command("f")
 def isolateFunction(source: str  = typer.Argument(..., help="The source code that the function will be isolated from (.cpp/.h)"),
                     destination: str  = typer.Argument(..., help="The destination code where the function will be embedded or replaced (.cpp/.h)"),
                     prototype: str  = typer.Argument(..., help="The function prototype: return-type function-name parameters-types. In the case of member functions return-type class-name::function-name parameters-types. Example: int test(int, string). Must put them in quotations when using CLI.")):
     """
-    This tool will isolate out a function, the function will be taken from source and replace the one in destination or add one.
+    Isolates out a function, the function will be taken from source and replace the one in destination or add one.
     """
     
-    findFunction = codeParser.positions(source,"function", prototype, True)
+    findFunction = codeParser.positions(source,"function", prototype)
     if findFunction == ["error"]:
         return
     if findFunction == []:
         print("Warning: Function doesn't exist in " + source +" file")
         return 
     
     # Open the source file and read its contents
     with open(source, "r") as source_file:
         lines = source_file.readlines() 
     
     #check if its a member function and parent class exists in destination file 
-    if findFunction[2] != "function" and findFunction[2] != "template_function":
+    if findFunction[2] != "function" and findFunction[2] != "template_function" and findFunction[2] != "main":
         parent_class = prototype.split("::")[0].strip().split(" ")[-1]
-        findClass = codeParser.positions(destination, "class", "class " + parent_class, False)
+        findClass = codeParser.positions(destination, "class", "class " + parent_class)
         if findClass == ["error"]:
             return
         if findClass == []:
-            findClass = codeParser.positions(destination, "struct", "struct " + parent_class, False)
+            findClass = codeParser.positions(destination, "struct", "struct " + parent_class)
             if findClass == ["error"]:
                 return
             if findClass == []:
                 print("Warning: Parent Class doesn't exist in " +destination +" file")
                 return 
         class_end = findClass[1]
         #fixing protoype
@@ -58,14 +58,16 @@
     
     # Open the destination file and insert the copied lines at the appropriate position
     with open(destination, "r") as destination_file:
         lines = destination_file.readlines()
     #functions insertion
     if findFunction[2] == "function" or findFunction[2] == "template_function":
         lines = [prototype +";\n"]+ lines[0:] + ['\n'] + implementation  
+    elif findFunction[2] == "main":
+        lines = lines[0:] + ['\n'] + implementation  
     #member functions insertion 
     else:
         #if function implemented outside the class 
         if  i == 4:
             lines = lines[0: class_end-1] + [findFunction[i+3] + ": "] + [forward_implementation + ";\n"] + lines[class_end-1: ] +['\n']+ implementation 
         #if function implemented inside the class
         else:
@@ -78,23 +80,29 @@
 
 
 @app.command("c")
 def isolateClass(
     source: str  = typer.Argument(..., help="The source code that the function will be isolated from (.cpp/.h)"), 
     destination: str  = typer.Argument(..., help="The destination code where the function will be embedded or replaced (.cpp/.h)"), 
     prototype: str  = typer.Argument(..., help="The class prototype: class class-name. Example: class test. Must put them in quotations when using CLI."),
-    all: str  = typer.Option("false", "-all", help="If true this will isolate the class with all its children classes, only takes true or false, default value is false.")):
+    all: str  = typer.Option("f", "-all", help="If t this will isolate the class with all its children classes, if c this will isolate the class itself without any member function implemented outside the class,if f this will isolate the class with its member functions implemented outside the class. Takes c, t, or f. Default value is f.")):
     """
-    This tool will isolate out a class, the class will be taken from source and replace the one in destination or add one.
+    Isolates out a class, the class will be taken from source and replace the one in destination or add one.
     """
-    option =0
-    if all.lower() == "false":
-        option = 1
+    if all.lower() not in ["f","t", "c"]:
+        print("Invalid input for -all")
+        return False
+    
+    option =1
+    if all == "t":
+        option = 0
+    elif all == "c":
+        option = -1
     type = prototype.split(" ")[0]
-    position = codeParser.positions(source, type, prototype, True, option)
+    position = codeParser.positions(source, type, prototype, option)
     
     if position == ["error"]:
         return
     
     #checking if class exists in source code
     if position == []:
         print("Class not found in " + source)
@@ -112,15 +120,15 @@
         start_line = position[i]
         end_line = position[i+1]
         #functions implemented outside a class
         if start_line <= class_start or end_line >= class_end:
             things += lines[start_line - 1:end_line]
     
     #checking if class already exists in destination code and commenting it out
-    class_position = codeParser.positions(destination, type, prototype, False, 1)
+    class_position = codeParser.positions(destination, type, prototype, 1)
     if class_position == ["error"]:
         return
     commentController.CommentOutClass(destination, prototype, all, 1, destination)
     
     with open(destination, "r") as destination_file:
         lines = destination_file.readlines()
         
@@ -132,13 +140,21 @@
             lines =  lines[0: class_position[0]-1] + things +  ["\n"] + lines[class_position[0]-1: ]
     
     
     
     # Write the modified lines to the destination file
     with open(destination, "w") as destination_file:
         destination_file.writelines(lines)
-    
+
+
+
+@app.callback()
+def main():
+    """
+    Allows the user to copy a given function or class from the source code file into the destination code file and replaces. It consists of two parts, IsolateFunction and IsolateClass.\n\n
+    For more information about each tool simply add the command you need followed by --help, for example:\n\n isolate f --help
+    """
 
 
 
 if __name__ == "__main__":
-    app()
+    app()
```

### Comparing `y4d-0.1.2/y4d/restrictor.py` & `y4d-0.1.3/y4d/restrictor.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 @app.command("r")
 def restrict(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants restrictor to work on."),
              rules: str  = typer.Argument(..., help="The path of the YAML file containing user requirements."),
              output: str  = typer.Option("n", "-o", help="If n this will make restrict print the number of violations, Input V if you want a list of violations to be printed and more information (default is n) (Takes only V or n or N)."),
              hide: bool = typer.Argument(False, hidden=True, help="A hidden variable for developers use, used with checkAPI to show the names of the functions or classes that are violating the YAML file (extra)."),
              hide2: bool = typer.Argument(False, hidden=True, help="A hidden variable for developers use, used to show that checkAPI called restrict")):
     """
-    This tool will recieve a YAML file made by the user and restrict a .cpp or .h file according to that YAML file, it will return a list of findings (for YAML file explanation check GitHub).
+    Recieves a YAML file made by the user and restrict a .cpp or .h file according to that YAML file, it will return a list of findings (for YAML file explanation check GitHub).
     """
     #Used to control the style of output
     if output not in ["n", "N", "V", "v"]:
         print("Invalid -o input")
         return False
     
     outputBool = False
@@ -291,15 +291,15 @@
 #Function to restrict a single library, no need for the YAML file, further explanation available exactly below function definition
 @app.command("l")
 def libRestrict(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants restrictor to work on."),
                  restriction: str = typer.Argument(..., help="The restriction type used for 3 ways of checking:\n\nat_least: The library being checked must exist (It can be with other libraries).\n\nexactly: The library being checked must only exist (It can not be with other libraries).\n\nforbidden: The library being checked must not exist."),
                  lib: str = typer.Argument(..., help="The name of the library the user wants to check (only input the name of the library without #include)."),
                  hide:bool = typer.Argument(False, hidden=True, help="A hidden variable for developers use, used to return boolean")):
     """
-    This tool will check if a certain library inputted by the user follows as certain restriction type of (at_least/exactly/forbidden) in a .cpp or .h file also inputted by the user.
+    Checks if a certain library inputted by the user follows as certain restriction type of (at_least/exactly/forbidden) in a .cpp or .h file also inputted by the user.
     """
 
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
@@ -357,33 +357,40 @@
 @app.command("k")
 def wordRestrict(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants restrictor to work on."),
                  restriction: str = typer.Argument(..., help="The restriction type used for 2 ways of checking:\n\nat_least: The keyword being checked must exist (It can be with other keywords).\n\nforbidden: The keyword being checked must not exist.\n\nexactly not available for keywords, will work as at_least."),
                  keyword: str = typer.Argument(..., help="The keyword the user wants to check (This function matches using regex, function prototypes don't work here, must input exactly what you want to match)."),
                  scope: str = typer.Argument(..., help="The scope the user wants to check inside (Function or Class, use their prototypes)."),
                  hide:bool = typer.Argument(False, hidden=True, help="A hidden variable for developers use, used to return boolean")):
     """
-    This tool will check if a certain keyword inputted by the user follows as certain restriction type of (at_least/exactly/forbidden) in a .cpp or .h file also inputted by the user.
+    Checks if a certain keyword inputted by the user follows as certain restriction type of (at_least/exactly/forbidden) in a .cpp or .h file also inputted by the user.
     """
 
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
-    
+
     #Check if global scope or not, if not then use scopeGetter to get everything in the scope defined by the user
     if scope.lower() == "global" or scope == "":
         with open(source, 'r') as f:
             source = f.read()
     else:
         source = scopeGetter(source, scope)
         if source == ["error"]:
             return False
-    
+
+    source = commentController.deleteForDeveloper(source)
+
+    iter = 0
+    if keyword.lower() == "iteration":
+        iter += len(re.findall(fr"(?i){{[\s\S]*for[\s\S]*}}", source, flags=re.MULTILINE))
+        iter += len(re.findall(fr"(?i){{[\s\S]*while[\s\S]*}}", source, flags=re.MULTILINE))
+        
     #Check if keyword exists and print true or false according to restriction
-    if re.search(fr"(?i).*return\s*[^\n;]+{re.escape(keyword)}.*", source):
+    if len(re.findall(fr"(?i){{[\s\S]*{re.escape(keyword)}[\s\S]*}}", source, flags=re.MULTILINE)) > 0 or iter > 0:
         if restriction.lower() == "at_least" or restriction.lower() == "exactly":
             if not hide:
                 print("True")
             return True
         elif restriction.lower() == "forbidden":
             if not hide:
                 print("False")
@@ -404,15 +411,15 @@
 @app.command("c")
 def classRestrict(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants restrictor to work on."),
                  restriction: str = typer.Argument(..., help="The restriction type used for 3 ways of checking:\n\nat_least: The class being checked must exist (It can be with other classes).\n\nexactly: The class being checked must only exist (It can not be with other classes).\n\nforbidden: The class being checked must not exist."),
                  prototype: str = typer.Argument(..., help="The class the user wants to check (Must input like this: \"class name\")."),
                  scope: str = typer.Argument(..., help="The scope the user wants to check inside (Function or Class, input their prototypes)."),
                  hide:bool = typer.Argument(False, hidden=True, help="A hidden variable for developers use, used to return boolean")):
     """
-    This tool will check if a certain class inputted by the user follows as certain restriction type of (at_least/exactly/forbidden) in a .cpp or .h file also inputted by the user.
+    Checks if a certain class inputted by the user follows as certain restriction type of (at_least/exactly/forbidden) in a .cpp or .h file also inputted by the user.
     """
 
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
@@ -467,15 +474,15 @@
 @app.command("f")
 def funcRestrict(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants restrictor to work on."),
                  restriction: str = typer.Argument(..., help="The restriction type used for 3 ways of checking:\n\nat_least: The function being checked must exist (It can be with other functions).\n\nexactly: The function being checked must only exist (It can not be with other functions).\n\nforbidden: The function being checked must not exist."),
                  prototype: str = typer.Argument(..., help="The function the user wants to check (Must input like this: \"int functionName(int, int)\"."),
                  scope: str = typer.Argument(..., help="The scope the user wants to check inside (Function or Class, input their prototypes)."),
                  hide:bool = typer.Argument(False, hidden=True, help="A hidden variable for developers use, used to return boolean")):
     """
-    This tool will check if a certain function inputted by the user follows as certain restriction type of (at_least/exactly/forbidden) in a .cpp or .h file also inputted by the user.
+    Checks if a certain function inputted by the user follows as certain restriction type of (at_least/exactly/forbidden) in a .cpp or .h file also inputted by the user.
     """
 
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
@@ -530,15 +537,15 @@
 def accessRestrict(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants restrictor to work on."),
                  restriction: str = typer.Argument(..., help="The restriction type used for 3 ways of checking:\n\nat_least: The function being checked must exist (It can be with other functions).\n\nexactly: The function being checked must only exist (It can not be with other functions).\n\nforbidden: The function being checked must not exist."),
                  prototype: str = typer.Argument(..., help="The function the user wants to check (Must input like this: \"int functionName(int, int)\" or \"int functionName(int x,int y)\")."),
                  scope: str = typer.Argument(..., help="The scope the user wants to check inside (Function or Class, input their prototypes)."),
                  type: str = typer.Argument(..., help="The access type the user wants to check for (private/public/protected)."),
                  hide:bool = typer.Argument(False, hidden=True, help="A hidden variable for developers use, used to return boolean")):
     """
-    This tool will check if a certain (private/public/protected) function inputted by the user follows as certain restriction type of (at_least/exactly/forbidden) in a .cpp or .h file also inputted by the user.
+    Checks if a certain (private/public/protected) function inputted by the user follows as certain restriction type of (at_least/exactly/forbidden) in a .cpp or .h file also inputted by the user.
     """
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
     #Check if global scope or not, if not then use scopeGetter to get everything in the scope defined by the user as well as preparing data for access_type search
@@ -572,15 +579,15 @@
 #Function to restrict a single (private/public/protected) function, no need for the YAML file, further explanation available exactly below function definition.
 def checkAPI(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants restrictor to work on."),
             restriction: str = typer.Argument(..., help="The restriction type used for 2 ways of checking:\n\nat_least: Everything being checked must exist (It can be with other functions/classes).\n\nexactly: Everything being checked must only exist (It can not be with other functions/classes)."),
             compare: str = typer.Argument(..., help="The path of the .cpp or .h file the user wants the source file to be compared to."),
             output: str  = typer.Option("n", "-o", help="If n this will make checkAPI print the number of missing functions/classes then extra functions/classes, Input V if you want a list of violations to be printed and more information (default is n) (Takes only v or V or n or N)."),
             hide:bool = typer.Argument(False, hidden=True, help="A hidden variable for developers use, used to return extra functions and classes found in the code.")):
     """
-    This tool will compare two files together, the source and compare file, it will check if the function prototypes and class names match then return true or false accordingly.
+    Compares two files together, the source and compare file, it will check if the function prototypes and class names match then return true or false accordingly.
     """
     #Used to control the style of output
     if output not in ["n", "N", "V", "v"]:
         print("Invalid -o input")
         return False
 
     data = codeParser.prepareData(compare)
@@ -639,9 +646,21 @@
     restrict(source, "checkAPI.YAML", output, hide)
 
     if not hide:
         checkAPI(compare, restriction, source, output, True)
 
 
 
+@app.callback()
+def main():
+    """
+    Allows the user to restrict the use of certain criterion or many criteria in a source file.\n\nThe criteria are libraries, keywords, classes, functions and access type of functions.\n\n
+    The restriction follows one of three types being at_least, exactly and forbidden.\n\n
+    at_least: must exist, can be with others of the same criterion.\n\n
+    exactly: must only exist, can not be with others of the same criterion.\n\n
+    forbidden: must not exist.\n\n
+    For more information about each tool simply add the command you need followed by --help, for example:\n\n restrict r --help
+    """
+
+
 if __name__ == "__main__":
-    app()
+    app()
```

### Comparing `y4d-0.1.2/PKG-INFO` & `y4d-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y4d
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: BahouA
 Author-email: antonbahou@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

