# Comparing `tmp/tkblock-2.2.0.tar.gz` & `tmp/tkblock-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkblock-2.2.0.tar", last modified: Wed May 24 14:14:03 2023, max compression
+gzip compressed data, was "tkblock-2.3.0.tar", last modified: Fri Jun  2 18:27:34 2023, max compression
```

## Comparing `tkblock-2.2.0.tar` & `tkblock-2.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 14:14:03.948090 tkblock-2.2.0/
--rw-rw-rw-   0        0        0     1077 2023-03-07 11:27:05.000000 tkblock-2.2.0/LICENSE
--rw-rw-rw-   0        0        0    15321 2023-05-24 14:14:03.946095 tkblock-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    14597 2023-05-24 14:12:48.000000 tkblock-2.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 14:14:03.949087 tkblock-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1017 2023-05-24 14:00:39.000000 tkblock-2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:14:03.928058 tkblock-2.2.0/tkblock/
--rw-rw-rw-   0        0        0      584 2023-05-19 17:11:52.000000 tkblock-2.2.0/tkblock/__init__.py
--rw-rw-rw-   0        0        0     3408 2023-05-19 17:11:52.000000 tkblock-2.2.0/tkblock/block_framebase.py
--rw-rw-rw-   0        0        0    21644 2023-05-19 17:11:52.000000 tkblock-2.2.0/tkblock/block_framework.py
--rw-rw-rw-   0        0        0    41780 2023-05-24 14:00:11.000000 tkblock-2.2.0/tkblock/block_service.py
--rw-rw-rw-   0        0        0      426 2023-05-19 17:11:52.000000 tkblock-2.2.0/tkblock/block_util.py
--rw-rw-rw-   0        0        0     1418 2023-05-19 17:11:52.000000 tkblock-2.2.0/tkblock/canvas.py
--rw-rw-rw-   0        0        0      494 2023-05-19 17:11:53.000000 tkblock-2.2.0/tkblock/layout.py
--rw-rw-rw-   0        0        0      368 2023-05-19 17:11:53.000000 tkblock-2.2.0/tkblock/scrollbar.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:14:03.944097 tkblock-2.2.0/tkblock.egg-info/
--rw-rw-rw-   0        0        0    15321 2023-05-24 14:14:03.000000 tkblock-2.2.0/tkblock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-05-24 14:14:03.000000 tkblock-2.2.0/tkblock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 14:14:03.000000 tkblock-2.2.0/tkblock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-24 14:14:03.000000 tkblock-2.2.0/tkblock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 18:27:34.557546 tkblock-2.3.0/
+-rw-rw-rw-   0        0        0     1077 2023-06-02 17:09:00.000000 tkblock-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0    15304 2023-06-02 18:27:34.555550 tkblock-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14580 2023-06-02 11:06:20.000000 tkblock-2.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-02 18:27:34.558546 tkblock-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1017 2023-06-02 18:25:46.000000 tkblock-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:27:34.538599 tkblock-2.3.0/tkblock/
+-rw-rw-rw-   0        0        0      584 2023-05-19 17:11:52.000000 tkblock-2.3.0/tkblock/__init__.py
+-rw-rw-rw-   0        0        0     3408 2023-05-19 17:11:52.000000 tkblock-2.3.0/tkblock/block_framebase.py
+-rw-rw-rw-   0        0        0    21644 2023-05-19 17:11:52.000000 tkblock-2.3.0/tkblock/block_framework.py
+-rw-rw-rw-   0        0        0    41266 2023-06-02 18:23:40.000000 tkblock-2.3.0/tkblock/block_service.py
+-rw-rw-rw-   0        0        0      426 2023-05-19 17:11:52.000000 tkblock-2.3.0/tkblock/block_util.py
+-rw-rw-rw-   0        0        0     3750 2023-06-02 18:21:40.000000 tkblock-2.3.0/tkblock/block_waiting_screen.py
+-rw-rw-rw-   0        0        0     1418 2023-05-19 17:11:52.000000 tkblock-2.3.0/tkblock/canvas.py
+-rw-rw-rw-   0        0        0      494 2023-05-19 17:11:53.000000 tkblock-2.3.0/tkblock/layout.py
+-rw-rw-rw-   0        0        0      368 2023-05-19 17:11:53.000000 tkblock-2.3.0/tkblock/scrollbar.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:27:34.551562 tkblock-2.3.0/tkblock.egg-info/
+-rw-rw-rw-   0        0        0    15304 2023-06-02 18:27:34.000000 tkblock-2.3.0/tkblock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-06-02 18:27:34.000000 tkblock-2.3.0/tkblock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 18:27:34.000000 tkblock-2.3.0/tkblock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 18:27:34.000000 tkblock-2.3.0/tkblock.egg-info/top_level.txt
```

### Comparing `tkblock-2.2.0/LICENSE` & `tkblock-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tkblock-2.2.0/PKG-INFO` & `tkblock-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkblock
-Version: 2.2.0
+Version: 2.3.0
 Summary: tkinter block framework
 Home-page: https://github.com/kuri-pome/tkblock
 Author: kuri_pome
 License: MIT
 Keywords: tkinter place widget easy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
@@ -320,15 +320,15 @@
 This is a decorator function to decorate the currently executing function.  
 For example, when a function assigned to a button widget is executed, it will output a waiting dialog.   
 
 <img width="218" alt="wait_process1" src="https://github.com/kuri-pome/tkblock/assets/78261582/03c4680c-4de0-4047-89f6-75cc732ec2f9">
 
 To use it, simply set the target frame as an argument and decorate it.  
 ```python
-@wait_processe(BlockService.root)
+@wait_processe()
 def _split_file(
 ```
 
 
 # Summary.  
 If you are going to make a full-fledged app, I would prefer not to use this.  
 I think a small app would be useful.
```

### Comparing `tkblock-2.2.0/README.md` & `tkblock-2.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,15 @@
 This is a decorator function to decorate the currently executing function.  
 For example, when a function assigned to a button widget is executed, it will output a waiting dialog.   
 
 <img width="218" alt="wait_process1" src="https://github.com/kuri-pome/tkblock/assets/78261582/03c4680c-4de0-4047-89f6-75cc732ec2f9">
 
 To use it, simply set the target frame as an argument and decorate it.  
 ```python
-@wait_processe(BlockService.root)
+@wait_processe()
 def _split_file(
 ```
 
 
 # Summary.  
 If you are going to make a full-fledged app, I would prefer not to use this.  
 I think a small app would be useful.
```

### Comparing `tkblock-2.2.0/setup.py` & `tkblock-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 # README.mdをlong_discriptionにするために読み込む
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 setup(
     name=package_name,
-    version="2.2.0",
+    version="2.3.0",
     description="tkinter block framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kuri-pome/tkblock",
     author="kuri_pome",
     license="MIT",
     keywords="tkinter place widget easy",
```

### Comparing `tkblock-2.2.0/tkblock/__init__.py` & `tkblock-2.3.0/tkblock/__init__.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.2.0/tkblock/block_framebase.py` & `tkblock-2.3.0/tkblock/block_framebase.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.2.0/tkblock/block_framework.py` & `tkblock-2.3.0/tkblock/block_framework.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.2.0/tkblock/block_service.py` & `tkblock-2.3.0/tkblock/block_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,79 +1,54 @@
 #!/usr/local/bin/python
 # -*- coding: utf-8 -*-
 # kuri_pome
 """BlockService
 
 このクラスを使用することでblock指定でwidgetを配置することができる。
 """
-import time
 import threading
 from typing import Any
 from functools import wraps, partial
 
 from .canvas import ResizingCanvas
 from .block_framebase import *
 from .layout import Layout
 from .scrollbar import Scrollbar
 from .block_framework import BlockFramework
+from .block_waiting_screen import BlockWaitingScreen
 
 
-def wait_processe(frame):
+def wait_processe(frame=None):
     """処理の完了を待つ。その間、待機描画処理を行う。
 
     Arguments:
         args (tuple): 位置引数
         kwargs (dict): キーワード引数 (名前で指定する引数)
     """
 
-    def _create_wait_toplevel(frame, is_exit):
-        toplevel = BlockService.create_toplevel(
-            frame, "wait", 300, 300, is_focus=True, is_grab=True
-        )
-        frame: BlockFrame = BlockService.create_frame(
-            "wait_toplevel",
-            col=10,
-            row=10,
-            root=toplevel,
-        )
-        label = BlockService.create_label(frame, 1, 9, 1, 9, text="")
-        BlockService.place_frame_widget(frame=toplevel)
-        toplevel.update_idletasks()
-        # toplevel.wait_window(toplevel)
-
-        while True:
-            if is_exit[0]:
-                break
-            label.config(text="実行中です。(ぐるぐる描画にしたい。)")
-            time.sleep(0.5)
-            label.config(text="少々お待ちを。(ぐるぐる描画にしたい。)")
-            time.sleep(0.5)
-            toplevel.update_idletasks()
-
-        toplevel.destroy()
-
     def wrapper(func):
         @wraps(func)
         def wait_processe(*args, **kwargs):
-            is_exit = [False]
+            root = BlockService.root if frame is None else frame
             result = [None]
-
-            def _execute(result, func, *args, **kwargs):
+            is_force_finish = [False]
+            wait_screen = BlockWaitingScreen(root, is_force_finish)
+            
+            def _execute(result, wait_screen, func, *args, **kwargs):
                 result[0] = func(*args, **kwargs)
-                is_exit[0] = True
+                wait_screen.end_thread()
 
-            wait_thread = threading.Thread(
-                target=partial(_create_wait_toplevel, frame, is_exit)
-            )
-            main_thread = threading.Thread(
-                target=partial(_execute, result, func, *args, **kwargs)
-            )
+            # # スレッドを実行して、関数を実行
+            wait_thread = threading.Thread(target=wait_screen.start_thread)
+            # wait_thread.daemon = False
             wait_thread.start()
-            time.sleep(0.5)
-            main_thread.start()
+            # run_thread = threading.Thread(target=partial(_execute, result, wait_screen, func, args=args, kwargs=kwargs), args=args, kwargs=kwargs)
+            run_thread = threading.Thread(target=partial(_execute, result, wait_screen, func), args=args, kwargs=kwargs)
+            # run_thread.daemon = True
+            run_thread.start()
             return result[0]
 
         return wait_processe
 
     return wrapper
 
 
@@ -266,15 +241,14 @@
         toplevel.width = width
         toplevel.hegith = height
         if is_focus:
             toplevel.focus_set()
         if is_grab:
             toplevel.grab_set()  # モーダルにする
         # dialog.transient(self.root)  # タスクバーに表示しない
-
         return toplevel
 
     @classmethod
     def create_canvas(
         cls,
         frame,
         col_start,
```

### Comparing `tkblock-2.2.0/tkblock/canvas.py` & `tkblock-2.3.0/tkblock/canvas.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.2.0/tkblock.egg-info/PKG-INFO` & `tkblock-2.3.0/tkblock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkblock
-Version: 2.2.0
+Version: 2.3.0
 Summary: tkinter block framework
 Home-page: https://github.com/kuri-pome/tkblock
 Author: kuri_pome
 License: MIT
 Keywords: tkinter place widget easy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
@@ -320,15 +320,15 @@
 This is a decorator function to decorate the currently executing function.  
 For example, when a function assigned to a button widget is executed, it will output a waiting dialog.   
 
 <img width="218" alt="wait_process1" src="https://github.com/kuri-pome/tkblock/assets/78261582/03c4680c-4de0-4047-89f6-75cc732ec2f9">
 
 To use it, simply set the target frame as an argument and decorate it.  
 ```python
-@wait_processe(BlockService.root)
+@wait_processe()
 def _split_file(
 ```
 
 
 # Summary.  
 If you are going to make a full-fledged app, I would prefer not to use this.  
 I think a small app would be useful.
```

