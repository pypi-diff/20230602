# Comparing `tmp/nodered.py-0.2.1.tar.gz` & `tmp/nodered.py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodered.py-0.2.1.tar", last modified: Wed May 10 10:49:17 2023, max compression
+gzip compressed data, was "nodered.py-0.2.2.tar", last modified: Fri Jun  2 06:36:41 2023, max compression
```

## Comparing `nodered.py-0.2.1.tar` & `nodered.py-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-10 10:49:17.450000 nodered.py-0.2.1/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.1/LICENSE
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-05-10 10:49:17.570000 nodered.py-0.2.1/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2026 2023-05-10 10:48:39.000000 nodered.py-0.2.1/README.md
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-10 10:49:17.460000 nodered.py-0.2.1/nodered.py.egg-info/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-05-10 10:49:17.000000 nodered.py-0.2.1/nodered.py.egg-info/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-05-10 10:49:17.000000 nodered.py-0.2.1/nodered.py.egg-info/SOURCES.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-05-10 10:49:17.000000 nodered.py-0.2.1/nodered.py.egg-info/dependency_links.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       14 2023-05-10 10:49:17.000000 nodered.py-0.2.1/nodered.py.egg-info/requires.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-05-10 10:49:17.000000 nodered.py-0.2.1/nodered.py.egg-info/top_level.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.1/nodered.py.egg-info/zip-safe
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-10 10:49:17.460000 nodered.py-0.2.1/noderedpy/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      403 2023-05-10 09:35:45.000000 nodered.py-0.2.1/noderedpy/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    11475 2023-05-10 10:42:26.000000 nodered.py-0.2.1/noderedpy/_nodered.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4006 2023-05-02 10:42:51.000000 nodered.py-0.2.1/noderedpy/_property.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-10 10:49:17.460000 nodered.py-0.2.1/noderedpy/assets/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.1/noderedpy/assets/python-logo.png
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.1/noderedpy/decorator.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-10 10:49:17.460000 nodered.py-0.2.1/noderedpy/node-red-starter/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.1/noderedpy/node-red-starter/editorTheme.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2512 2023-05-07 01:35:50.000000 nodered.py-0.2.1/noderedpy/node-red-starter/index.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      296 2023-04-27 11:00:04.000000 nodered.py-0.2.1/noderedpy/node-red-starter/package.json
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-10 10:49:17.460000 nodered.py-0.2.1/noderedpy/templates/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7985 2023-05-10 10:44:33.000000 nodered.py-0.2.1/noderedpy/templates/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.1/noderedpy/templates/template.html
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3766 2023-05-07 11:55:40.000000 nodered.py-0.2.1/noderedpy/templates/template.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.1/noderedpy/templates/template.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-05-10 10:49:17.570000 nodered.py-0.2.1/setup.cfg
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-05-07 01:29:24.000000 nodered.py-0.2.1/setup.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-02 06:36:41.180000 nodered.py-0.2.2/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.2/LICENSE
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-06-02 06:36:41.310000 nodered.py-0.2.2/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2026 2023-05-10 10:48:39.000000 nodered.py-0.2.2/README.md
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-02 06:36:41.180000 nodered.py-0.2.2/nodered.py.egg-info/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-06-02 06:36:41.000000 nodered.py-0.2.2/nodered.py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-06-02 06:36:41.000000 nodered.py-0.2.2/nodered.py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-06-02 06:36:41.000000 nodered.py-0.2.2/nodered.py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       14 2023-06-02 06:36:41.000000 nodered.py-0.2.2/nodered.py.egg-info/requires.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-06-02 06:36:41.000000 nodered.py-0.2.2/nodered.py.egg-info/top_level.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.2/nodered.py.egg-info/zip-safe
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-02 06:36:41.180000 nodered.py-0.2.2/noderedpy/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      403 2023-06-02 04:28:48.000000 nodered.py-0.2.2/noderedpy/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    12724 2023-06-02 06:29:12.000000 nodered.py-0.2.2/noderedpy/_nodered.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4006 2023-05-02 10:42:51.000000 nodered.py-0.2.2/noderedpy/_property.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-02 06:36:41.180000 nodered.py-0.2.2/noderedpy/assets/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.2/noderedpy/assets/python-logo.png
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.2/noderedpy/decorator.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-02 06:36:41.190000 nodered.py-0.2.2/noderedpy/node-red-starter/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.2/noderedpy/node-red-starter/editorTheme.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3396 2023-06-02 06:24:22.000000 nodered.py-0.2.2/noderedpy/node-red-starter/index.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-06-02 04:29:58.000000 nodered.py-0.2.2/noderedpy/node-red-starter/package.json
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-02 06:36:41.230000 nodered.py-0.2.2/noderedpy/templates/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7985 2023-05-10 10:44:33.000000 nodered.py-0.2.2/noderedpy/templates/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.2/noderedpy/templates/template.html
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3766 2023-05-07 11:55:40.000000 nodered.py-0.2.2/noderedpy/templates/template.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.2/noderedpy/templates/template.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-06-02 06:36:41.310000 nodered.py-0.2.2/setup.cfg
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.2/setup.py
```

### Comparing `nodered.py-0.2.1/LICENSE` & `nodered.py-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.1/PKG-INFO` & `nodered.py-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.1
+Version: 0.2.2
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
     NodeRED.py
 </h1>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.1 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.2 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
-Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
                              [MIT_License] [pypi]
```

### Comparing `nodered.py-0.2.1/README.md` & `nodered.py-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.1/nodered.py.egg-info/PKG-INFO` & `nodered.py-0.2.2/nodered.py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.1
+Version: 0.2.2
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
     NodeRED.py
 </h1>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.1 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.2 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
-Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
                              [MIT_License] [pypi]
```

### Comparing `nodered.py-0.2.1/nodered.py.egg-info/SOURCES.txt` & `nodered.py-0.2.2/nodered.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.1/noderedpy/_nodered.py` & `nodered.py-0.2.2/noderedpy/_nodered.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class RED:
     """
     Node-RED manager class
     """
     registered_nodes:List["Node"] = []
 
-    def __init__(self, user_dir:str, node_red_dir:str = None, admin_root:str = "/node-red-py", port:int = 1880, show_default_category:bool = True, editor_theme:dict = {}):
+    def __init__(self, user_dir:str, node_red_dir:str = None, admin_root:str = "/node-red-py", port:int = 1880, show_default_category:bool = True, editor_theme:dict = {}, auths:List[dict] = []):
         """
         Set configs of Node-RED and setup
 
         Parameters
         ----------
         user_dir: str, required
             userDir of Node-RED settings
@@ -28,18 +28,22 @@
             httpAdminRoot of Node-RED settings
         port: int, default 1880
             port of Node-RED server
         show_default_category: bool, default True
             show default categories of Node-RED or not
         editor_theme: dict, default {}
             editorTheme of Node-RED server (for detail information, see https://github.com/node-red/node-red/wiki/Design:-Editor-Themes)
+        auths: List[dict], default []
+            auth list for Node-RED
         """
         self.user_dir, self.admin_root, self.port, self.show_default_category, self.editor_theme =\
             user_dir, admin_root, port, show_default_category, self.__default_editor_theme(editor_theme)
         
+        self.node_auths = self.__default_node_auth(auths)
+        
         # set node_red_dir
         if node_red_dir is None:
             self.node_red_dir = os.path.join(__path__[0], "node-red-starter")
         else:
             self.node_red_dir = node_red_dir = os.path.realpath(node_red_dir)
             if os.path.exists(node_red_dir):
                 if not { "index.js", "package.json" }.issubset(set(os.listdir(node_red_dir))):
@@ -77,20 +81,33 @@
             "enabled": project_feature.pop("enabled", False)
         })
 
         editor_theme.update({
             "page": page_theme,
             "header": header_theme,
             "menu": menu_theme,
-            "userMenu": editor_theme.pop("userMenu", False),
+            "userMenu": editor_theme.pop("userMenu", True),
             "projects": project_feature
         })
 
         return editor_theme
     
+    # fill empty auth in auths
+    def __default_node_auth(self, node_auths:List[dict]) -> List[dict]:
+        new_node_auths = []
+        for node_auth in node_auths:
+            if ("username" in node_auth.keys() and not node_auth["username"] in ( None, "" )) and ("password" in node_auth.keys() and not node_auth["password"] in ( None, "" )):
+                new_node_auths.append({
+                    "username": node_auth["username"],
+                    "password": node_auth["password"],
+                    "permissions": node_auth.pop("permissions", "*")
+                })
+
+        return new_node_auths
+    
     def register(self, node_func:MethodType, name:str, category:str = "nodered_py", version:str = "1.0.0", description:str = "", author:str = "nodered.py", keywords:List[str] = [], icon:str = "function.png", properties:List[Property] = []):
         """
         Function to register Node function
 
         Parameters
         ----------
         node_func: MethodType, required
@@ -166,35 +183,42 @@
         # set cache_dir
         self.__cache_dir = os.path.join(self.user_dir, ".cache")
         if os.path.exists(self.__cache_dir):
             shutil.rmtree(self.__cache_dir)
 
         os.mkdir(self.__cache_dir)
 
-        # save editor_theme
-        with open(os.path.join(self.node_red_dir, "editorTheme.json"), "w", encoding = "utf-8") as tjw:
-            json.dump(self.editor_theme, tjw, indent = 4)
+        # save configs
+        with open(os.path.join(self.node_red_dir, "config.json"), "w", encoding = "utf-8") as cfw:
+            json.dump({
+                "userDir": self.user_dir,
+                "adminRoot": self.admin_root,
+                "port": self.port,
+                "showDefaultCategory": self.show_default_category,
+                "userCategory": list(set([ node.category for node in RED.registered_nodes ])),
+                "editorTheme": self.editor_theme,
+                "adminAuth": self.node_auths
+            }, cfw, indent = 4)
+
+        # # save editor_theme
+        # with open(os.path.join(self.node_red_dir, "editorTheme.json"), "w", encoding = "utf-8") as tjw:
+        #     json.dump(self.editor_theme, tjw, indent = 4)
 
         # remove existing nodes
         for node_dir in glob(os.path.join(self.user_dir, "node_modules", "nodered-py-*")):
             shutil.rmtree(node_dir)
 
         # create custom nodes
         for node in RED.registered_nodes:
             node.create(self.user_dir, self.__cache_dir)
 
         # run Node-RED server
         subprocess.Popen([
             "node",
-            "index.js",
-            f"--user-dir={self.user_dir}",
-            f"--admin-root={self.admin_root}",
-            f"--port={self.port}",
-            f"--show-default-category={'true' if self.show_default_category else 'false'}"
-            f"--user-category={','.join(list(set([ node.category for node in RED.registered_nodes ])))}"
+            "index.js"
         ], shell = False, stdout = sys.stdout if debug else subprocess.DEVNULL, cwd = self.node_red_dir)
 
         while True:
             if os.path.exists(self.__started_file):
                 if callback:
                     callback()
 
@@ -211,22 +235,29 @@
         """
         import time
 
         self.__started_file = os.path.join(self.node_red_dir, "started")
         if os.path.exists(self.__started_file):
             os.remove(self.__started_file)
 
+        # save configs
+        with open(os.path.join(self.node_red_dir, "config.json"), "w", encoding = "utf-8") as cfw:
+            json.dump({
+                "userDir": self.user_dir,
+                "adminRoot": self.admin_root,
+                "port": self.port,
+                "showDefaultCategory": self.show_default_category,
+                "userCategory": list(set([ node.category for node in RED.registered_nodes ])),
+                "editorTheme": self.editor_theme,
+                "adminAuth": []
+            }, cfw, indent = 4)
+
         subprocess.Popen([
             "node",
-            "index.js",
-            f"--user-dir={self.user_dir}",
-            f"--admin-root={self.admin_root}",
-            f"--port={self.port}",
-            f"--show-default-category={'true' if self.show_default_category else 'false'}"
-            f"--user-category={','.join(list(set([ node.category for node in RED.registered_nodes ])))}"
+            "index.js"
         ], shell = False, stdout = subprocess.DEVNULL, cwd = self.node_red_dir)
 
         while True:
             if os.path.exists(self.__started_file):
                 self.stop()
                 break
```

### Comparing `nodered.py-0.2.1/noderedpy/_property.py` & `nodered.py-0.2.2/noderedpy/_property.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.1/noderedpy/assets/python-logo.png` & `nodered.py-0.2.2/noderedpy/assets/python-logo.png`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.1/noderedpy/decorator.py` & `nodered.py-0.2.2/noderedpy/decorator.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.1/noderedpy/node-red-starter/index.js` & `nodered.py-0.2.2/noderedpy/node-red-starter/index.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,66 +1,72 @@
 // import modules
-const {
-    ArgumentParser
-} = require("argparse"),
-    express = require("express"),
+// const { ArgumentParser } = require("argparse"),
+const express = require("express"),
     http = require("http"),
     RED = require("node-red"),
-    fs = require("fs"), path = require("path");
+    fs = require("fs"),
+    path = require("path");
 
-// parser
-const parser = new ArgumentParser();
-parser.add_argument("--user-dir", {
-    type: "str"
-});
-parser.add_argument("--admin-root", {
-    type: "str"
-});
-parser.add_argument("--port", {
-    type: "int"
-});
-parser.add_argument("--user-category", {
-    type: "str",
-    default: ""
-});
-parser.add_argument("--show-default-category", {
-    type: "str"
-});
-const args = parser.parse_args();
-
-// parse user-category
-if (args["user_category"] == "") {
-    args["user_category"] = [];
-} else {
-    const raw_categories = args["user_category"].split(",");
-    args["user_category"] = [];
-    for (var raw_category of raw_categories) {
-        args["user_category"].push(raw_category.trim());
-    }
-}
+// read config file
+const configs = JSON.parse(fs.readFileSync(path.join(__dirname, "config.json")));
+
+// // parser
+// const parser = new ArgumentParser();
+// parser.add_argument("--user-dir", { type: "str" });
+// parser.add_argument("--admin-root", { type: "str" });
+// parser.add_argument("--port", { type: "int" });
+// parser.add_argument("--user-category", { type: "str", default: "" });
+// parser.add_argument("--show-default-category", { type: "str" });
+// const args = parser.parse_args();
+
+// // parse user-category
+// if (args["user_category"] == "") {
+//     args["user_category"] = [];
+// }
+// else {
+//     const raw_categories = args["user_category"].split(",");
+//     args["user_category"] = [];
+//     for (var raw_category of raw_categories) {
+//         args["user_category"].push(raw_category.trim());
+//     }
+// }
 
 
 // create express and node-red server
 const exapp = express();
 const RED_server = http.createServer(exapp);
 
-// set configs
-var editorTheme = JSON.parse(fs.readFileSync(path.join(__dirname, "editorTheme.json")))
-editorTheme["projects"] = {
-    enabled: false
-};
+// // set configs
+// var editorTheme = JSON.parse(fs.readFileSync(path.join(__dirname, "editorTheme.json")))
+// editorTheme["projects"] = { enabled: false };
 
 let opts = {
-    editorTheme: editorTheme,
-    httpAdminRoot: args["admin_root"].startsWith("/") ? args["admin_root"] : `/${args["admin_root"]}`,
+    // editorTheme: editorTheme,
+    editorTheme: configs.editorTheme,
+    // httpAdminRoot: args["admin_root"].startsWith("/") ? args["admin_root"] : `/${args["admin_root"]}`,
+    httpAdminRoot: configs.adminRoot.startsWith("/") ? configs.adminRoot : `/${config.adminRoot}`,
     httpNodeRoot: "/",
     flowFile: "noderedpy.json",
-    userDir: args["user_dir"],
-    paletteCategories: args["show_default_category"] == "true" ? args["user_category"].concat(["subflows", "common", "function", "network", "sequence", "parser", "storage"]) : args["user_category"]
+    // userDir: args["user_dir"],
+    userDir: configs.userDir,
+    // paletteCategories: args["show_default_category"] == "true" ? args["user_category"].concat([ "subflows", "common", "function", "network", "sequence", "parser", "storage" ]) : args["user_category"]
+    paletteCategories: configs.showDefaultCategory ? configs.userCategory.concat(["subflows", "common", "function", "network", "sequence", "parser", "storage"]) : configs.userCategory
 };
+if (configs.adminAuth != []) {
+    var realAuth = [];
+    for (var auth of configs.adminAuth) {
+        auth.password = require("bcryptjs").hashSync(auth.password, 8)
+        realAuth.push(auth);
+    }
+
+    opts.adminAuth = {
+        type: "credentials",
+        users: realAuth
+    }
+}
 // if (![ "None", "null", "" ].includes(args["admin_auth"])) {
 //     opts.adminAuth = {
 //         type: "credentials",
 //         users: [
 //             {
 //                 username: "nodered-py",
 //                 password: args["admin_auth"],
@@ -82,11 +88,12 @@
 // node-red default routes
 exapp.use("/", express.static("web"));
 exapp.use(RED.settings.httpAdminRoot, RED.httpAdmin);
 exapp.use(RED.settings.httpNodeRoot, RED.httpNode);
 
 // start node-red
 RED.start().then(() => {
-    RED_server.listen(args.port, "0.0.0.0", () => {
+    // RED_server.listen(args.port, "0.0.0.0", () => {
+    RED_server.listen(configs.port, "0.0.0.0", () => {
         fs.writeFileSync(path.join(__dirname, "started"), "");
     });
 });
```

### Comparing `nodered.py-0.2.1/noderedpy/templates/__init__.py` & `nodered.py-0.2.2/noderedpy/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.1/noderedpy/templates/template.html` & `nodered.py-0.2.2/noderedpy/templates/template.html`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.1/noderedpy/templates/template.js` & `nodered.py-0.2.2/noderedpy/templates/template.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.1/setup.py` & `nodered.py-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 setup(
     # publish informations
     name = "nodered.py",
     author = __author__,
     author_email = __email__,
     url = "https://github.com/oyajiDev/NodeRED.py",
     version = __version__,
-    python_requires = ">=3.9",
+    python_requires = ">=3.7",
     install_requires = requires,
     setup_requires = requires,
     license = "MIT license",
     description = "make python function to Node-RED node",
     long_description = readme,
     long_description_content_type = "text/markdown",
     # package informations
```

