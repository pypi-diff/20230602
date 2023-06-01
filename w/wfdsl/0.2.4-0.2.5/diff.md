# Comparing `tmp/wfdsl-0.2.4.tar.gz` & `tmp/wfdsl-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wfdsl-0.2.4.tar", last modified: Thu Mar 30 13:55:51 2023, max compression
+gzip compressed data, was "wfdsl-0.2.5.tar", last modified: Thu Jun  1 23:52:24 2023, max compression
```

## Comparing `wfdsl-0.2.4.tar` & `wfdsl-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 13:55:51.731387 wfdsl-0.2.4/
--rw-r--r--   0 root         (0) root         (0)     1057 2023-01-19 10:37:26.000000 wfdsl-0.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      550 2023-03-30 13:55:51.731387 wfdsl-0.2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       72 2023-01-19 10:37:26.000000 wfdsl-0.2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 13:55:51.731387 wfdsl-0.2.4/dsl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-19 10:37:26.000000 wfdsl-0.2.4/dsl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1223 2023-01-19 10:37:26.000000 wfdsl-0.2.4/dsl/accessrights.py
--rw-r--r--   0 root         (0) root         (0)     5390 2023-02-16 02:21:38.000000 wfdsl-0.2.4/dsl/context.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-01-19 10:37:26.000000 wfdsl-0.2.4/dsl/datatype.py
--rw-r--r--   0 root         (0) root         (0)      193 2023-01-19 10:37:26.000000 wfdsl-0.2.4/dsl/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-01-19 10:37:26.000000 wfdsl-0.2.4/dsl/exechelper.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-01-19 10:37:26.000000 wfdsl-0.2.4/dsl/filemgr.py
--rw-r--r--   0 root         (0) root         (0)    17750 2023-03-30 00:14:46.000000 wfdsl-0.2.4/dsl/fileop.py
--rw-r--r--   0 root         (0) root         (0)    11878 2023-01-19 12:45:03.000000 wfdsl-0.2.4/dsl/grammar.py
--rw-r--r--   0 root         (0) root         (0)    21176 2023-01-19 10:37:26.000000 wfdsl-0.2.4/dsl/graphgen.py
--rw-r--r--   0 root         (0) root         (0)    16644 2023-01-20 06:04:10.000000 wfdsl-0.2.4/dsl/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    10898 2023-01-19 10:37:26.000000 wfdsl-0.2.4/dsl/library.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-01-19 10:37:26.000000 wfdsl-0.2.4/dsl/parser.py
--rw-r--r--   0 root         (0) root         (0)     9466 2023-01-19 10:37:26.000000 wfdsl-0.2.4/dsl/pygen.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-01-19 10:37:26.000000 wfdsl-0.2.4/dsl/symtab.py
--rw-r--r--   0 root         (0) root         (0)     1007 2023-01-19 10:37:26.000000 wfdsl-0.2.4/dsl/taskmgr.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-01-19 10:37:26.000000 wfdsl-0.2.4/dsl/wfobj.py
--rw-r--r--   0 root         (0) root         (0)      459 2023-01-19 10:37:26.000000 wfdsl-0.2.4/dsl/wftimer.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 13:55:51.731387 wfdsl-0.2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      657 2023-03-30 00:17:39.000000 wfdsl-0.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 13:55:51.731387 wfdsl-0.2.4/wfdsl.egg-info/
--rw-r--r--   0 root         (0) root         (0)      550 2023-03-30 13:55:51.000000 wfdsl-0.2.4/wfdsl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      423 2023-03-30 13:55:51.000000 wfdsl-0.2.4/wfdsl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 13:55:51.000000 wfdsl-0.2.4/wfdsl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-30 13:55:51.000000 wfdsl-0.2.4/wfdsl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:52:24.637195 wfdsl-0.2.5/
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-01-19 10:37:26.000000 wfdsl-0.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      550 2023-06-01 23:52:24.637195 wfdsl-0.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       72 2023-01-19 10:37:26.000000 wfdsl-0.2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:52:24.637195 wfdsl-0.2.5/dsl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/accessrights.py
+-rw-r--r--   0 root         (0) root         (0)     5390 2023-02-16 02:21:38.000000 wfdsl-0.2.5/dsl/context.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/datatype.py
+-rw-r--r--   0 root         (0) root         (0)      193 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/exechelper.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/filemgr.py
+-rw-r--r--   0 root         (0) root         (0)    18111 2023-06-01 23:48:34.000000 wfdsl-0.2.5/dsl/fileop.py
+-rw-r--r--   0 root         (0) root         (0)    11878 2023-04-30 12:21:22.000000 wfdsl-0.2.5/dsl/grammar.py
+-rw-r--r--   0 root         (0) root         (0)    21176 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/graphgen.py
+-rw-r--r--   0 root         (0) root         (0)    16635 2023-04-29 16:01:45.000000 wfdsl-0.2.5/dsl/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    10898 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/library.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/parser.py
+-rw-r--r--   0 root         (0) root         (0)     9466 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/pygen.py
+-rw-r--r--   0 root         (0) root         (0)     1231 2023-04-29 16:01:45.000000 wfdsl-0.2.5/dsl/symtab.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/taskmgr.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/wfobj.py
+-rw-r--r--   0 root         (0) root         (0)      459 2023-01-19 10:37:26.000000 wfdsl-0.2.5/dsl/wftimer.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 23:52:24.637195 wfdsl-0.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-01 23:52:15.000000 wfdsl-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:52:24.637195 wfdsl-0.2.5/wfdsl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      550 2023-06-01 23:52:24.000000 wfdsl-0.2.5/wfdsl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      423 2023-06-01 23:52:24.000000 wfdsl-0.2.5/wfdsl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 23:52:24.000000 wfdsl-0.2.5/wfdsl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-01 23:52:24.000000 wfdsl-0.2.5/wfdsl.egg-info/top_level.txt
```

### Comparing `wfdsl-0.2.4/LICENSE` & `wfdsl-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.4/PKG-INFO` & `wfdsl-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfdsl
-Version: 0.2.4
+Version: 0.2.5
 Summary: Workflow Domain Specific Language
 Home-page: https://github.com/srlabUsask/wfdsl
 Author: Muhammad Mainul Hossain
 Author-email: mainul.hossain@usask.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wfdsl-0.2.4/dsl/accessrights.py` & `wfdsl-0.2.5/dsl/accessrights.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.4/dsl/context.py` & `wfdsl-0.2.5/dsl/context.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.4/dsl/fileop.py` & `wfdsl-0.2.5/dsl/fileop.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,15 +310,15 @@
 
     def make_json(self, path):
         raise ValueError("Not implemented error.")
     
     def make_json_r(self, path):
         raise ValueError("Not implemented error.")
 
-    def save_upload(self, file, path):
+    def save_upload(self, file, path, offset=None):
         raise ValueError("Not implemented error.")
     
     def download(self, path):
         raise ValueError("Not implemented error.")
     
     def stat(self, path):
         raise ValueError("Not implemented error.")
@@ -507,24 +507,33 @@
     def make_json_r(self, path):
         data_json = self.make_json_item(path)  
         if 'children' in data_json: # folder 
             data_json['children'] = [self.make_json_r(self.join(path, fn)) for fn in self.listdir(path)]
             data_json['loaded'] = True
         return data_json
 
-    def save_upload(self, file, path):
+    def save_upload(self, file, path, offset=None):
         path = self.normalize_path(path)
         if self.isfile(path):
             path = os.path.dirname(path)
         elif not os.path.exists(path):
             os.makedirs(path)
-        path = os.path.join(path, file.filename)
-        file.save(path)
-        return self.strip_root(path)
-    
+        path = os.path.join(path, file.filename)   
+        if offset is None:
+            file.save(path)
+        else:
+            try:
+                with open(path, 'ab') as f:
+                    f.seek(offset)
+                    f.write(file.stream.read())
+            except OSError:
+            # log.exception will include the traceback so we can see what's wrong
+                return
+        return self.strip_root(path), path
+        
     def download(self, path):
         path = self.normalize_path(path)
         return path if os.path.isfile(path) else None
     
     def basename(self, path):
         path = self.normalize_path(path)
         return os.path.basename(path)
```

### Comparing `wfdsl-0.2.4/dsl/grammar.py` & `wfdsl-0.2.5/dsl/grammar.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.4/dsl/graphgen.py` & `wfdsl-0.2.5/dsl/graphgen.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.4/dsl/interpreter.py` & `wfdsl-0.2.5/dsl/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     
     def domember(self, expr):
         objs = expr[0].split('.')
         objs = [i for i in objs if i]
         objs.append(expr[1]) # add the member to the attributes
         
         if not self.context.var_exists(objs[0]):
-            raise ValueError("Object doesn't exist: {0}")
+            raise ValueError(f"Object doesn't exist: {objs[0]}")
         
         obj = self.context.get_var(objs[0])
         for i in range(1, len(objs)):
             obj = getattr(obj, expr[i])
         return obj
 
     def dofuncs(self, expr):
@@ -363,15 +363,15 @@
     # dotaskdefstmt
     # if task has no name, it will be called at once.
     # if task has a name, it will be called like a function call afterwards
     #===========================================================================
     def eval_params(self, expr):
         params = []
         for e in expr:
-            if e[0] is "NAMEDARG":
+            if e[0] == "NAMEDARG":
                 param = self.donamedarg(e[1])
                 self.context.add_var(param[0], param[1])
             else:
                 params.extend([ex for ex in e])
                 
         return params
                         
@@ -380,15 +380,15 @@
             #v = self.get_args(expr[1])
             return self.dotaskstmt(expr[1:], None) # anonymous task; run immediately
         else:
             self.context.library.add_task(expr[0], expr)
     
     def args_to_symtab(self, expr):
         for e in expr:
-            if e[0] is not "NAMEDARG":
+            if e[0] != "NAMEDARG":
                 continue
             param = self.donamedarg(e[1])
             
             #if isinstance(param, tuple):
             self.context.add_var(param[0], param[1])
                 
     def dotaskstmt(self, expr, args):
@@ -511,8 +511,8 @@
         :param prog: Pyparsing ParseResults
         '''
         try:
             #self.context.reload()
             stmt = prog.asList()
             return self.eval(stmt)
         except Exception as err:
-            raise ValueError("Error at line {0}: {1}".format(self.line, err))
+            raise ValueError(f"Error at line {self.line}: {err}")
```

### Comparing `wfdsl-0.2.4/dsl/library.py` & `wfdsl-0.2.5/dsl/library.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.4/dsl/parser.py` & `wfdsl-0.2.5/dsl/parser.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.4/dsl/pygen.py` & `wfdsl-0.2.5/dsl/pygen.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.4/dsl/symtab.py` & `wfdsl-0.2.5/dsl/symtab.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         Checks if a variable exists in the symbol table
         :param name:
         '''
         return name in self.vars
     
     def check_var(self, name):
         if not self.var_exists(name):
-            raise ValueError("var {0} does not exist".format(name))
+            raise ValueError(f"var {name} does not exist")
         return True
             
     def get_var(self, name):
         '''
         Gets value of a variable
         :param name:
         '''
```

### Comparing `wfdsl-0.2.4/dsl/taskmgr.py` & `wfdsl-0.2.5/dsl/taskmgr.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.4/dsl/wfobj.py` & `wfdsl-0.2.5/dsl/wfobj.py`

 * *Files identical despite different names*

### Comparing `wfdsl-0.2.4/setup.py` & `wfdsl-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wfdsl",
-    version="0.2.4",
+    version="0.2.5",
     author="Muhammad Mainul Hossain",
     author_email="mainul.hossain@usask.ca",
     description="Workflow Domain Specific Language",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/srlabUsask/wfdsl",
     packages=setuptools.find_packages(),
```

### Comparing `wfdsl-0.2.4/wfdsl.egg-info/PKG-INFO` & `wfdsl-0.2.5/wfdsl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfdsl
-Version: 0.2.4
+Version: 0.2.5
 Summary: Workflow Domain Specific Language
 Home-page: https://github.com/srlabUsask/wfdsl
 Author: Muhammad Mainul Hossain
 Author-email: mainul.hossain@usask.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

