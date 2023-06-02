# Comparing `tmp/iamlistening-0.1.1.tar.gz` & `tmp/iamlistening-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-0.1.1.tar", max compression
+gzip compressed data, was "iamlistening-0.1.2.tar", max compression
```

## Comparing `iamlistening-0.1.1.tar` & `iamlistening-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-02 11:59:12.555793 iamlistening-0.1.1/LICENSE
--rw-r--r--   0        0        0     1376 2023-06-02 11:59:12.555793 iamlistening-0.1.1/README.md
--rw-r--r--   0        0        0       99 2023-06-02 11:59:13.371803 iamlistening-0.1.1/iamlistening/__init__.py
--rw-r--r--   0        0        0      630 2023-06-02 11:59:12.555793 iamlistening-0.1.1/iamlistening/config.py
--rw-r--r--   0        0        0      229 2023-06-02 11:59:12.555793 iamlistening-0.1.1/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     7286 2023-06-02 11:59:12.555793 iamlistening-0.1.1/iamlistening/main.py
--rw-r--r--   0        0        0     1692 2023-06-02 11:59:13.371803 iamlistening-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 iamlistening-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-02 15:34:04.072111 iamlistening-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1376 2023-06-02 15:34:04.072111 iamlistening-0.1.2/README.md
+-rw-r--r--   0        0        0       99 2023-06-02 15:34:04.760120 iamlistening-0.1.2/iamlistening/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-02 15:34:04.072111 iamlistening-0.1.2/iamlistening/config.py
+-rw-r--r--   0        0        0      229 2023-06-02 15:34:04.072111 iamlistening-0.1.2/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     7291 2023-06-02 15:34:04.072111 iamlistening-0.1.2/iamlistening/main.py
+-rw-r--r--   0        0        0     1692 2023-06-02 15:34:04.756120 iamlistening-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 iamlistening-0.1.2/PKG-INFO
```

### Comparing `iamlistening-0.1.1/LICENSE` & `iamlistening-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.1/README.md` & `iamlistening-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.1/iamlistening/config.py` & `iamlistening-0.1.2/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.1/iamlistening/main.py` & `iamlistening-0.1.2/iamlistening/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
             @bot.on(events.NewMessage())
             async def telethon(event):
                 await self.event(event.message.message)
 
             await bot.run_until_disconnected()
         else:
-            logger.warning("Check settings")
+            self.logger.warning("Check settings")
             await asyncio.sleep(7200)
 
     async def post_init(self):
         return
     async def event(self, event):
         print(event)
         return
```

### Comparing `iamlistening-0.1.1/pyproject.toml` & `iamlistening-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamlistening"
-version = "0.1.1"
+version = "0.1.2"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
```

### Comparing `iamlistening-0.1.1/PKG-INFO` & `iamlistening-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

