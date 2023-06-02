# Comparing `tmp/context_menu-1.2.3.tar.gz` & `tmp/context_menu-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\context_menu-1.2.3.tar", last modified: Fri Apr  1 06:05:11 2022, max compression
+gzip compressed data, was "context_menu-1.3.0.tar", last modified: Fri Jun  2 19:52:45 2023, max compression
```

## Comparing `context_menu-1.2.3.tar` & `context_menu-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-04-01 06:05:11.000000 context_menu-1.2.3/
-drwxrwxrwx   0        0        0        0 2022-04-01 06:05:10.000000 context_menu-1.2.3/context_menu/
--rw-rw-rw-   0        0        0    11468 2022-03-31 22:44:34.000000 context_menu-1.2.3/context_menu/linux_menus.py
--rw-rw-rw-   0        0        0     5253 2022-03-31 22:44:34.000000 context_menu-1.2.3/context_menu/menus.py
--rw-rw-rw-   0        0        0    12508 2022-03-31 22:44:34.000000 context_menu-1.2.3/context_menu/windows_menus.py
--rw-rw-rw-   0        0        0       36 2022-03-31 22:44:34.000000 context_menu-1.2.3/context_menu/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-01 06:05:11.000000 context_menu-1.2.3/context_menu.egg-info/
--rw-rw-rw-   0        0        0        1 2022-04-01 06:05:09.000000 context_menu-1.2.3/context_menu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     9562 2022-04-01 06:05:09.000000 context_menu-1.2.3/context_menu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2022-04-01 06:05:09.000000 context_menu-1.2.3/context_menu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       13 2022-04-01 06:05:09.000000 context_menu-1.2.3/context_menu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2022-03-31 22:44:34.000000 context_menu-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     9562 2022-04-01 06:05:11.000000 context_menu-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     9005 2022-03-31 22:44:34.000000 context_menu-1.2.3/README.md
--rw-rw-rw-   0        0        0       42 2022-04-01 06:05:11.000000 context_menu-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      877 2022-04-01 06:04:52.000000 context_menu-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:52:45.047681 context_menu-1.3.0/
+-rw-rw-rw-   0        0        0     1086 2023-06-02 19:45:36.000000 context_menu-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0    14964 2023-06-02 19:52:45.047681 context_menu-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14389 2023-06-02 19:46:16.000000 context_menu-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 19:52:45.015641 context_menu-1.3.0/context_menu/
+-rw-rw-rw-   0        0        0       36 2023-06-02 19:45:36.000000 context_menu-1.3.0/context_menu/__init__.py
+-rw-rw-rw-   0        0        0    11820 2023-06-02 19:45:36.000000 context_menu-1.3.0/context_menu/linux_menus.py
+-rw-rw-rw-   0        0        0     5401 2023-06-02 19:45:36.000000 context_menu-1.3.0/context_menu/menus.py
+-rw-rw-rw-   0        0        0    12508 2023-06-02 19:45:36.000000 context_menu-1.3.0/context_menu/windows_menus.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:52:45.039684 context_menu-1.3.0/context_menu.egg-info/
+-rw-rw-rw-   0        0        0    14964 2023-06-02 19:52:44.000000 context_menu-1.3.0/context_menu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-06-02 19:52:44.000000 context_menu-1.3.0/context_menu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 19:52:44.000000 context_menu-1.3.0/context_menu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 19:52:44.000000 context_menu-1.3.0/context_menu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 19:52:45.047681 context_menu-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      943 2023-06-02 19:48:43.000000 context_menu-1.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `context_menu-1.2.3/context_menu/linux_menus.py` & `context_menu-1.3.0/context_menu/linux_menus.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,31 @@
     '''
 
     CODE_HEAD = '''
 import gi
 import sys
 import os
 
-gi.require_version('Nautilus', '3.0')
+try:
+\tgi.require_version('Nautilus', '3.0')
+except:
+\tgi.require_version('Nautilus', '4.0')
 
 from gi.repository import Nautilus, GObject
 
 # -------------------------------------------- #
 
 try:
 \tfrom urllib import unquote
 except ImportError:
 \tfrom urllib.parse import unquote
     '''
 
     CLASS_TEMPLATE = '''
-class ExampleMenuProvider(GObject.GObject, Nautilus.MenuProvider):
+class {}MenuProvider(GObject.GObject, Nautilus.MenuProvider):
 \tdef __init__(self):
 \t\tpass
 '''
 
     METHOD_HANDLER_TEMPLATE = '''
 \tdef {}(self, menu, files):
 \t\tfilenames = [unquote(subFile.get_uri()[7:]) for subFile in files]
@@ -43,32 +46,35 @@
     COMMAND_HANDLER_TEMPLATE = '''
 \tdef {}(self, menu, files):
 \t\tfilepath = [unquote(subFile.get_uri()[7:]) for subFile in files][0]
 \t\tos.system('{}'{})
 
 '''
 
-    FILE_ITEMS = '\tdef get_file_items(self, window, files):'
-    BACKGROUND_ITEMS = '\tdef get_background_items(self, window, files):'
+    FILE_ITEMS = '''\tdef get_file_items(self, *args):
+\t\tfiles = args[-1]'''
+    BACKGROUND_ITEMS = '''\tdef get_background_items(self, *args):
+\t\tfiles = args[-1]'''
     SUB_MENU = 'submenu{} = Nautilus.Menu()'
     MENU_ITEM = 'menuitem{} = Nautilus.MenuItem(name = "ExampleMenuProvider::{}", label="{}", tip = "{}", icon = "{}")'
 
 # code_builder.py ----------------------------------
 
 
 class CodeBuilder:
     '''
     The CodeBuilder class is used for generating the final python file for the Linux menus.
     '''
 
-    def __init__(self, body_commands: list, script_dirs: list, funcs: list, imports: list, type: str):
+    def __init__(self, name: str, body_commands: list, script_dirs: list, funcs: list, imports: list, type: str):
         '''
         Pass the list of body_commands, the directories of all the scripts, the
         list of the function names, the list of the imports, and the type.
         '''
+        self.name = name
         self.body_commands = body_commands
         self.script_dirs = list(set(script_dirs))
         self.funcs = funcs
         self.imports = list(set(imports))
         self.type = type.upper()
 
     def build_script_dirs(self):
@@ -94,15 +100,15 @@
     def compile(self):
         '''
         Creates the code file.
         '''
         code_head = ExistingCode.CODE_HEAD.value
         script_dirs_code = self.build_script_dirs()
         imports_code = self.build_imports()
-        class_dec = ExistingCode.CLASS_TEMPLATE.value
+        class_dec = ExistingCode.CLASS_TEMPLATE.value.format(self.name)
         class_funcs = '\n\n'.join(self.funcs)
         class_type = ExistingCode.FILE_ITEMS.value
         if self.type in ['DIRECTORY_BACKGROUND', 'DESKTOP_BACKGROUND']:
             class_type = ExistingCode.BACKGROUND_ITEMS.value
         class_body = '\n'.join(map(lambda x: '\t\t' + x, self.body_commands))
 
         code_skeleton = '''
@@ -149,15 +155,17 @@
 class NautilusMenu:
 
     # Constructor, automatically handeled by menus.py
     def __init__(self, name: str, sub_items: list, type: str):
         '''
         Items required are the name of the top menu, the sub items, and the type.
         '''
-        self.name = name
+        # nautilus extensions doesn't work with filenames with spaces
+        # Example menu item -> ExampleMenuItem
+        self.name = "".join([word.title() for word in name.split()]) if len(name.split()) > 0 else name
         self.sub_items = sub_items
         self.type = type
         self.counter = 0
 
 # Create all the necessary lists that will be used later on
         self.commands = []
         self.script_dirs = []
@@ -314,15 +322,15 @@
 
     def build_script(self):
         '''
         Finishes and returns the full code.
         '''
         self.build_script_body(self.name, self.sub_items)
         self.commands.append('return menuitem0,')
-        full_code = CodeBuilder(
+        full_code = CodeBuilder(self.name,
             self.commands, self.script_dirs, self.funcs, self.imports, self.type).compile()
 
         return full_code
 
     def create_path(self, path: str, dir: str):
         '''
         Creates a path to directory. Creates all sub-directories
```

### Comparing `context_menu-1.2.3/context_menu/menus.py` & `context_menu-1.3.0/context_menu/menus.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,23 @@
 
 # Need to append all the python subdirectories because Python doesn't recognize them
 sys.path.append(os.path.abspath(os.path.dirname(__file__)))
 
 
 # Import the necessary library depending on the OS
 if platform.system() == 'Linux':
-    import linux_menus
+    try:
+        import linux_menus
+    except:
+        from context_menu import linux_menus
 if platform.system() == 'Windows':
-    import windows_menus
+    try:
+        import windows_menus
+    except:
+        from context_menu import windows_menus
 
 
 class ContextMenu:
     '''
     The general menu class. This class generalizes the menus and eventually passes the correct values to the platform-specifically menus.
     '''
```

### Comparing `context_menu-1.2.3/context_menu/windows_menus.py` & `context_menu-1.3.0/context_menu/windows_menus.py`

 * *Files identical despite different names*

### Comparing `context_menu-1.2.3/LICENSE` & `context_menu-1.3.0/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 willandsallinc
+Copyright (c) 2022 saleguas
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `context_menu-1.2.3/setup.py` & `context_menu-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import pathlib
 import setuptools
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
-README = (HERE / "README.md").read_text()
+README = (HERE / "README.md").read_text(encoding='utf-8')
 
 # This call to setup() does all the work
 setuptools.setup(
     name="context_menu",
-    version="1.2.3",
+    version="1.3.0",
     description="Library to create cross-platform native context menus.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/saleguas/context_menu",
     author="Salvador Aleguas",
     author_email="salvador@aleguas.dev",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
     ],
     packages=setuptools.find_packages(),
 )
```

