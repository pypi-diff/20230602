# Comparing `tmp/iamlistening-0.1.2.tar.gz` & `tmp/iamlistening-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-0.1.2.tar", max compression
+gzip compressed data, was "iamlistening-0.1.3.tar", max compression
```

## Comparing `iamlistening-0.1.2.tar` & `iamlistening-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-02 15:34:04.072111 iamlistening-0.1.2/LICENSE
--rw-r--r--   0        0        0     1376 2023-06-02 15:34:04.072111 iamlistening-0.1.2/README.md
--rw-r--r--   0        0        0       99 2023-06-02 15:34:04.760120 iamlistening-0.1.2/iamlistening/__init__.py
--rw-r--r--   0        0        0      630 2023-06-02 15:34:04.072111 iamlistening-0.1.2/iamlistening/config.py
--rw-r--r--   0        0        0      229 2023-06-02 15:34:04.072111 iamlistening-0.1.2/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     7291 2023-06-02 15:34:04.072111 iamlistening-0.1.2/iamlistening/main.py
--rw-r--r--   0        0        0     1692 2023-06-02 15:34:04.756120 iamlistening-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 iamlistening-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-02 16:57:43.343311 iamlistening-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1507 2023-06-02 16:57:43.343311 iamlistening-0.1.3/README.md
+-rw-r--r--   0        0        0       99 2023-06-02 16:57:44.079436 iamlistening-0.1.3/iamlistening/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-02 16:57:43.343311 iamlistening-0.1.3/iamlistening/config.py
+-rw-r--r--   0        0        0      229 2023-06-02 16:57:43.343311 iamlistening-0.1.3/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     7319 2023-06-02 16:57:43.343311 iamlistening-0.1.3/iamlistening/main.py
+-rw-r--r--   0        0        0     1692 2023-06-02 16:57:44.079436 iamlistening-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 iamlistening-0.1.3/PKG-INFO
```

### Comparing `iamlistening-0.1.2/LICENSE` & `iamlistening-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.2/README.md` & `iamlistening-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # I Am Listening
 
-| <img width="200" alt="Logo" src="https://github.com/mraniki/iamlistening/assets/8766259/f76331f6-8821-49eb-8f1c-06aedd8557be"> | A python package to interact with messaging platforms. |
+| <img width="200" alt="Logo" src="https://github.com/mraniki/iamlistening/assets/8766259/f76331f6-8821-49eb-8f1c-06aedd8557be"> | A python package to listen to messaging platforms. |
 | ------------- | ------------- |
-|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/iamlistening?icon=pypi&label)](https://pypi.org/project/iamlistening/) ![Version](https://img.shields.io/pypi/v/iamlistening)<br>  ![Pypi](https://img.shields.io/pypi/dm/iamlistening)<br> [![Build](https://github.com/mraniki/iamlistening/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/listening/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/listening/branch/dev/graph/badge.svg)](https://codecov.io/gh/mraniki/listening) | build a client to interact with messaging platform|
+|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/iamlistening?icon=pypi&label)](https://pypi.org/project/iamlistening/) ![Version](https://img.shields.io/pypi/v/iamlistening)<br>  ![Pypi](https://img.shields.io/pypi/dm/iamlistening)<br> [![Build](https://github.com/mraniki/iamlistening/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/listening/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/iamlistening/branch/main/graph/badge.svg?token=QZ55U6KQFN)](https://codecov.io/gh/mraniki/iamlistening) | build a client to interact with messaging platform|
 
 Key features:
 
-
+ - support discord, telegram and matrix platform
 
 ## Install
 
 `pip install iamlistening`
 
 ## How to use it
 
 ```
-
+ from iamlisterning import Listerner
+ 
+ bot = listerner.start()
 ```
 
 ### Example
 
 [example](https://github.com/mraniki/iamlistening/blob/main/examples/example.py)
 
 ### Real use case
```

### Comparing `iamlistening-0.1.2/iamlistening/config.py` & `iamlistening-0.1.3/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.2/iamlistening/main.py` & `iamlistening-0.1.3/iamlistening/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
             @bot.event
             async def on_ready():
                 await self.post_init()
 
             @bot.event
             async def on_message(message: discord.Message):
-                await self.event(message.content)
+                await self.event_action(message.content)
             await bot.start(settings.bot_token)
         elif settings.matrix_hostname:
             # MATRIX
             config = botlib.Config()
             config.emoji_verify = True
             config.ignore_unverified_devices = True
             config.store_path = './config/matrix/'
@@ -58,15 +58,15 @@
 
             @bot.listener.on_startup
             async def room_joined(room):
                 await self.post_init()
 
             @bot.listener.on_message_event
             async def on_matrix_message(room, message):
-                await self.event(message.body)
+                await self.event_action(message.body)
             await bot.api.login()
             bot.api.async_client.callbacks = botlib.Callbacks(
                                                 bot.api.async_client, bot
                                                 )
             await bot.api.async_client.callbacks.setup_callbacks()
             for action in bot.listener._startup_registry:
                 for room_id in bot.api.async_client.rooms:
@@ -82,24 +82,24 @@
                         settings.telethon_api_id,
                         settings.telethon_api_hash
                         ).start(bot_token=settings.bot_token)
             await self.post_init()
 
             @bot.on(events.NewMessage())
             async def telethon(event):
-                await self.event(event.message.message)
+                await self.event_action(event.message.message)
 
             await bot.run_until_disconnected()
         else:
             self.logger.warning("Check settings")
             await asyncio.sleep(7200)
 
     async def post_init(self):
         return
-    async def event(self, event):
+    async def event_action(self, event):
         print(event)
         return
 # async def listener():
 #     """Launch Bot Listener"""
 #     try:
 #         await load_exchange()
 #     except Exception as e:
```

### Comparing `iamlistening-0.1.2/pyproject.toml` & `iamlistening-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamlistening"
-version = "0.1.2"
+version = "0.1.3"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
```

### Comparing `iamlistening-0.1.2/PKG-INFO` & `iamlistening-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,30 +20,32 @@
 Project-URL: Changelog, https://github.com/mraniki/iamlistening/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/iamlistening/issues
 Project-URL: Support, https://github.com/mraniki/iamlistening/discussions
 Description-Content-Type: text/markdown
 
 # I Am Listening
 
-| <img width="200" alt="Logo" src="https://github.com/mraniki/iamlistening/assets/8766259/f76331f6-8821-49eb-8f1c-06aedd8557be"> | A python package to interact with messaging platforms. |
+| <img width="200" alt="Logo" src="https://github.com/mraniki/iamlistening/assets/8766259/f76331f6-8821-49eb-8f1c-06aedd8557be"> | A python package to listen to messaging platforms. |
 | ------------- | ------------- |
-|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/iamlistening?icon=pypi&label)](https://pypi.org/project/iamlistening/) ![Version](https://img.shields.io/pypi/v/iamlistening)<br>  ![Pypi](https://img.shields.io/pypi/dm/iamlistening)<br> [![Build](https://github.com/mraniki/iamlistening/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/listening/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/listening/branch/dev/graph/badge.svg)](https://codecov.io/gh/mraniki/listening) | build a client to interact with messaging platform|
+|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/iamlistening?icon=pypi&label)](https://pypi.org/project/iamlistening/) ![Version](https://img.shields.io/pypi/v/iamlistening)<br>  ![Pypi](https://img.shields.io/pypi/dm/iamlistening)<br> [![Build](https://github.com/mraniki/iamlistening/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/listening/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/iamlistening/branch/main/graph/badge.svg?token=QZ55U6KQFN)](https://codecov.io/gh/mraniki/iamlistening) | build a client to interact with messaging platform|
 
 Key features:
 
-
+ - support discord, telegram and matrix platform
 
 ## Install
 
 `pip install iamlistening`
 
 ## How to use it
 
 ```
-
+ from iamlisterning import Listerner
+ 
+ bot = listerner.start()
 ```
 
 ### Example
 
 [example](https://github.com/mraniki/iamlistening/blob/main/examples/example.py)
 
 ### Real use case
```

