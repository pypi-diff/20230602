# Comparing `tmp/wombo-0.1.51.tar.gz` & `tmp/wombo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wombo-0.1.51.tar", max compression
+gzip compressed data, was "wombo-0.1.6.tar", max compression
```

## Comparing `wombo-0.1.51.tar` & `wombo-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-06-02 14:02:35.382424 wombo-0.1.51/LICENSE
--rw-r--r--   0        0        0     1407 2023-06-02 16:56:22.134424 wombo-0.1.51/README.md
--rw-r--r--   0        0        0      341 2023-06-02 16:56:27.506424 wombo-0.1.51/pyproject.toml
--rw-r--r--   0        0        0       70 2023-06-02 14:20:19.386424 wombo-0.1.51/wombo/__init__.py
--rw-r--r--   0        0        0     4013 2023-06-02 15:51:51.722424 wombo-0.1.51/wombo/async_dream.py
--rw-r--r--   0        0        0     3421 2023-06-02 15:37:20.226424 wombo-0.1.51/wombo/dream.py
--rw-r--r--   0        0        0       93 2023-06-02 14:55:39.890424 wombo-0.1.51/wombo/models/__init__.py
--rw-r--r--   0        0        0      524 2023-06-02 15:01:24.554424 wombo-0.1.51/wombo/models/check_task.py
--rw-r--r--   0        0        0      513 2023-06-02 14:46:35.578424 wombo-0.1.51/wombo/models/create_task.py
--rw-r--r--   0        0        0     3274 2023-06-02 14:21:55.846424 wombo-0.1.51/wombo/urls.py
--rw-r--r--   0        0        0     1931 1970-01-01 00:00:00.000000 wombo-0.1.51/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-02 14:02:35.382424 wombo-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2081 2023-06-02 20:51:04.421083 wombo-0.1.6/README.md
+-rw-r--r--   0        0        0      347 2023-06-02 21:12:26.313083 wombo-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-06-02 14:20:19.386424 wombo-0.1.6/wombo/__init__.py
+-rw-r--r--   0        0        0     4439 2023-06-02 21:07:06.797083 wombo-0.1.6/wombo/async_dream.py
+-rw-r--r--   0        0        0     3981 2023-06-02 21:10:40.925083 wombo-0.1.6/wombo/dream.py
+-rw-r--r--   0        0        0       93 2023-06-02 14:55:39.890424 wombo-0.1.6/wombo/models/__init__.py
+-rw-r--r--   0        0        0      524 2023-06-02 15:01:24.554424 wombo-0.1.6/wombo/models/check_task.py
+-rw-r--r--   0        0        0      513 2023-06-02 14:46:35.578424 wombo-0.1.6/wombo/models/create_task.py
+-rw-r--r--   0        0        0     3274 2023-06-02 14:21:55.846424 wombo-0.1.6/wombo/urls.py
+-rw-r--r--   0        0        0     2611 1970-01-01 00:00:00.000000 wombo-0.1.6/PKG-INFO
```

### Comparing `wombo-0.1.51/LICENSE` & `wombo-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wombo-0.1.51/wombo/async_dream.py` & `wombo-0.1.6/wombo/async_dream.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,16 +72,31 @@
         result = CheckTask.parse_obj(result)
         if only_bool:
             if result.photo_url_list:
                 return True
             else:
                 return False
         return result
+    
+    async def generate(self, text: str, style: int = 84, gif: bool = False):
+        """Generate image"""
+        task = await self.create_task(text=text, style=style)
+        await asyncio.sleep(2)
+        for _ in range(10):
+            task = await self.check_task(task_id=task.id, only_bool=False)
+            if task.photo_url_list and task.state != "generating":
+                if gif:
+                    res = await self.gif(task.photo_url_list)
+                else:
+                    res = task
+                break
+            await asyncio.sleep(2)
+        return res
 
-
+    # ============================================================================================= # 
     def gif_creating(self, frames: list, duration: int = 400) -> io.BytesIO:
         result = io.BytesIO()
         frames[0].save(
             result,
             save_all=True,
             append_images=frames[1:],  # Срез который игнорирует первый кадр.
             format='GIF',
@@ -102,23 +117,16 @@
         return result
 
 
 
     
 async def main():
     dream = AsyncDream()
-    task = await dream.create_task(input("Промт: "))
-    while True:
-        if await dream.check_task(task.id):
-            break
-        await asyncio.sleep(3)
-    task = await dream.check_task(task.id, False)
-    with open("file.gif", "wb") as f:
-        res = await dream.gif(task.photo_url_list)
-        f.write(res.getvalue())
+    task = await dream.generate("Anime waifu in bikini")
+    print(task)
     # frames = await dream.get_stage_task(task)
 
 
 if __name__ == "__main__":  
     asyncio.run(main())
```

### Comparing `wombo-0.1.51/wombo/dream.py` & `wombo-0.1.6/wombo/dream.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import httpx
 import re
 import io
+import time
 
 from PIL import Image
 from wombo.urls import urls, auth_key_headers, headers_gen, check_headers
 from wombo.models import CreateTask, CheckTask
 
 class Dream:
     def __init__(self) -> None:
@@ -70,14 +71,29 @@
         if only_bool:
             if result.photo_url_list:
                 return True
             else:
                 return False
         return result
     
+    def generate(self, text: str, style: int = 84, gif: bool = False):
+        """Generate image"""
+        task = self.create_task(text=text, style=style)
+        time.sleep(2)
+        for _ in range(100):
+            task = self.check_task(task_id=task.id, only_bool=False)
+            if task.photo_url_list and task.state != "generating":
+                if gif:
+                    res = self.gif(task.photo_url_list)
+                else:
+                    res = task
+                break
+            time.sleep(2)
+        return res
+    
     def gif_creating(self, frames: list, duration: int = 400) -> io.BytesIO:
 
         result = io.BytesIO()
         frames[0].save(
             result,
             save_all=True,
             append_images=frames[1:],  # Срез который игнорирует первый кадр.
```

### Comparing `wombo-0.1.51/wombo/models/check_task.py` & `wombo-0.1.6/wombo/models/check_task.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.51/wombo/models/create_task.py` & `wombo-0.1.6/wombo/models/create_task.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.51/wombo/urls.py` & `wombo-0.1.6/wombo/urls.py`

 * *Files identical despite different names*

