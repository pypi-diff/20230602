# Comparing `tmp/iamlistening-0.1.0.tar.gz` & `tmp/iamlistening-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-0.1.0.tar", max compression
+gzip compressed data, was "iamlistening-0.1.1.tar", max compression
```

## Comparing `iamlistening-0.1.0.tar` & `iamlistening-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-02 10:15:23.723023 iamlistening-0.1.0/LICENSE
--rw-r--r--   0        0        0     1376 2023-06-02 10:15:23.723023 iamlistening-0.1.0/README.md
--rw-r--r--   0        0        0       99 2023-06-02 10:15:24.655026 iamlistening-0.1.0/iamlistening/__init__.py
--rw-r--r--   0        0        0      630 2023-06-02 10:15:23.723023 iamlistening-0.1.0/iamlistening/config.py
--rw-r--r--   0        0        0      229 2023-06-02 10:15:23.723023 iamlistening-0.1.0/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     4847 2023-06-02 10:15:23.723023 iamlistening-0.1.0/iamlistening/main.py
--rw-r--r--   0        0        0     1692 2023-06-02 10:15:24.655026 iamlistening-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 iamlistening-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-02 11:59:12.555793 iamlistening-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1376 2023-06-02 11:59:12.555793 iamlistening-0.1.1/README.md
+-rw-r--r--   0        0        0       99 2023-06-02 11:59:13.371803 iamlistening-0.1.1/iamlistening/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-02 11:59:12.555793 iamlistening-0.1.1/iamlistening/config.py
+-rw-r--r--   0        0        0      229 2023-06-02 11:59:12.555793 iamlistening-0.1.1/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     7286 2023-06-02 11:59:12.555793 iamlistening-0.1.1/iamlistening/main.py
+-rw-r--r--   0        0        0     1692 2023-06-02 11:59:13.371803 iamlistening-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 iamlistening-0.1.1/PKG-INFO
```

### Comparing `iamlistening-0.1.0/LICENSE` & `iamlistening-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.0/README.md` & `iamlistening-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.0/iamlistening/config.py` & `iamlistening-0.1.1/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.1.0/iamlistening/main.py` & `iamlistening-0.1.1/iamlistening/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,15 @@
  IAmListening Main
 """
 __version__ = "0.0.0"
 
 import os
 import sys
 import asyncio
+import logging 
 
 import apprise
 from apprise import NotifyFormat
 from telethon import TelegramClient, events
 import discord
 import simplematrixbotlib as botlib
 
@@ -22,22 +23,85 @@
     """ i am listening class """
 
     def __init__(
         self,
     ):
         self.logger = logging.getLogger(name="Listener")
     async def start(self):
-        token = settings.bot_token
-        channel = settings.channel
+        # token = settings.bot_token
+        # channel = settings.bot_channel_id
         if settings.discord_webhook_id:
-            print("discord")
+            # DISCORD
+            intents = discord.Intents.default()
+            intents.message_content = True
+            bot = discord.Bot(intents=intents)
+
+            @bot.event
+            async def on_ready():
+                await self.post_init()
+
+            @bot.event
+            async def on_message(message: discord.Message):
+                await self.event(message.content)
+            await bot.start(settings.bot_token)
         elif settings.matrix_hostname:
-            print("matrix")
-        elif settings.telethon_api_id or settings.rocket_chat:
-            print("telethon")
+            # MATRIX
+            config = botlib.Config()
+            config.emoji_verify = True
+            config.ignore_unverified_devices = True
+            config.store_path = './config/matrix/'
+            creds = botlib.Creds(
+                        settings.matrix_hostname,
+                        settings.matrix_user,
+                        settings.matrix_pass
+                        )
+            bot = botlib.Bot(creds, config)
+
+            @bot.listener.on_startup
+            async def room_joined(room):
+                await self.post_init()
+
+            @bot.listener.on_message_event
+            async def on_matrix_message(room, message):
+                await self.event(message.body)
+            await bot.api.login()
+            bot.api.async_client.callbacks = botlib.Callbacks(
+                                                bot.api.async_client, bot
+                                                )
+            await bot.api.async_client.callbacks.setup_callbacks()
+            for action in bot.listener._startup_registry:
+                for room_id in bot.api.async_client.rooms:
+                    await action(room_id)
+            await bot.api.async_client.sync_forever(
+                                                    timeout=3000,
+                                                    full_state=True
+                                                )
+        elif settings.telethon_api_id:
+            # TELEGRAM
+            bot = await TelegramClient(
+                        None,
+                        settings.telethon_api_id,
+                        settings.telethon_api_hash
+                        ).start(bot_token=settings.bot_token)
+            await self.post_init()
+
+            @bot.on(events.NewMessage())
+            async def telethon(event):
+                await self.event(event.message.message)
+
+            await bot.run_until_disconnected()
+        else:
+            logger.warning("Check settings")
+            await asyncio.sleep(7200)
+
+    async def post_init(self):
+        return
+    async def event(self, event):
+        print(event)
+        return
 # async def listener():
 #     """Launch Bot Listener"""
 #     try:
 #         await load_exchange()
 #     except Exception as e:
 #         logger.error("exchange: %s", e)
 #     try:
```

### Comparing `iamlistening-0.1.0/pyproject.toml` & `iamlistening-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamlistening"
-version = "0.1.0"
+version = "0.1.1"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
```

### Comparing `iamlistening-0.1.0/PKG-INFO` & `iamlistening-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

