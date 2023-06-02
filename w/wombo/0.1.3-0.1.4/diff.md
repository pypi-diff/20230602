# Comparing `tmp/wombo-0.1.3.tar.gz` & `tmp/wombo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wombo-0.1.3.tar", max compression
+gzip compressed data, was "wombo-0.1.4.tar", max compression
```

## Comparing `wombo-0.1.3.tar` & `wombo-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-06-02 14:02:35.382424 wombo-0.1.3/LICENSE
--rw-r--r--   0        0        0       35 2023-06-02 15:32:46.562424 wombo-0.1.3/README.md
--rw-r--r--   0        0        0      340 2023-06-02 15:48:32.238424 wombo-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       70 2023-06-02 14:20:19.386424 wombo-0.1.3/wombo/__init__.py
--rw-r--r--   0        0        0     3944 2023-06-02 15:33:20.162424 wombo-0.1.3/wombo/async_dream.py
--rw-r--r--   0        0        0     3421 2023-06-02 15:37:20.226424 wombo-0.1.3/wombo/dream.py
--rw-r--r--   0        0        0       93 2023-06-02 14:55:39.890424 wombo-0.1.3/wombo/models/__init__.py
--rw-r--r--   0        0        0      524 2023-06-02 15:01:24.554424 wombo-0.1.3/wombo/models/check_task.py
--rw-r--r--   0        0        0      513 2023-06-02 14:46:35.578424 wombo-0.1.3/wombo/models/create_task.py
--rw-r--r--   0        0        0     3274 2023-06-02 14:21:55.846424 wombo-0.1.3/wombo/urls.py
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 wombo-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-02 14:02:35.382424 wombo-0.1.4/LICENSE
+-rw-r--r--   0        0        0       35 2023-06-02 15:32:46.562424 wombo-0.1.4/README.md
+-rw-r--r--   0        0        0      340 2023-06-02 16:01:10.574424 wombo-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-06-02 14:20:19.386424 wombo-0.1.4/wombo/__init__.py
+-rw-r--r--   0        0        0     4013 2023-06-02 15:51:51.722424 wombo-0.1.4/wombo/async_dream.py
+-rw-r--r--   0        0        0     3421 2023-06-02 15:37:20.226424 wombo-0.1.4/wombo/dream.py
+-rw-r--r--   0        0        0       93 2023-06-02 14:55:39.890424 wombo-0.1.4/wombo/models/__init__.py
+-rw-r--r--   0        0        0      524 2023-06-02 15:01:24.554424 wombo-0.1.4/wombo/models/check_task.py
+-rw-r--r--   0        0        0      513 2023-06-02 14:46:35.578424 wombo-0.1.4/wombo/models/create_task.py
+-rw-r--r--   0        0        0     3274 2023-06-02 14:21:55.846424 wombo-0.1.4/wombo/urls.py
+-rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 wombo-0.1.4/PKG-INFO
```

### Comparing `wombo-0.1.3/LICENSE` & `wombo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wombo-0.1.3/wombo/async_dream.py` & `wombo-0.1.4/wombo/async_dream.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         url = f"https://dream.ai/_next/static/chunks/pages/_app-{js_filename}.js"
         response = await self.client.get(url)
 
         key = re.findall(r'"(AI\w+)"', response.text)
         return key[0]
     
     async def _get_auth_key(self) -> str:
+        ''' Get Auth Key from JS file '''
         params = {'key': await self._get_google_key()}
         json_data = {'returnSecureToken': True}
 
         response = await self.client.post(urls["auth_key"],
 				headers=auth_key_headers,
 				params=params,
 				json=json_data,
@@ -74,15 +75,14 @@
                 return True
             else:
                 return False
         return result
 
 
     def gif_creating(self, frames: list, duration: int = 400) -> io.BytesIO:
-
         result = io.BytesIO()
         frames[0].save(
             result,
             save_all=True,
             append_images=frames[1:],  # Срез который игнорирует первый кадр.
             format='GIF',
             duration=duration, 
@@ -114,11 +114,11 @@
     task = await dream.check_task(task.id, False)
     with open("file.gif", "wb") as f:
         res = await dream.gif(task.photo_url_list)
         f.write(res.getvalue())
     # frames = await dream.get_stage_task(task)
 
 
-    
-asyncio.run(main())
+if __name__ == "__main__":  
+    asyncio.run(main())
```

### Comparing `wombo-0.1.3/wombo/dream.py` & `wombo-0.1.4/wombo/dream.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.3/wombo/models/check_task.py` & `wombo-0.1.4/wombo/models/check_task.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.3/wombo/models/create_task.py` & `wombo-0.1.4/wombo/models/create_task.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.3/wombo/urls.py` & `wombo-0.1.4/wombo/urls.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.3/PKG-INFO` & `wombo-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wombo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dream api
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

