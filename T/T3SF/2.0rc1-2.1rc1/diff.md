# Comparing `tmp/T3SF-2.0rc1.tar.gz` & `tmp/T3SF-2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "T3SF-2.0rc1.tar", last modified: Fri May  5 16:03:16 2023, max compression
+gzip compressed data, was "T3SF-2.1rc1.tar", last modified: Fri Jun  2 16:39:23 2023, max compression
```

## Comparing `T3SF-2.0rc1.tar` & `T3SF-2.1rc1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)    35149 2022-04-20 14:58:09.000000 T3SF-2.0rc1/LICENSE
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       42 2023-04-05 17:28:50.000000 T3SF-2.0rc1/MANIFEST.in
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4748 2023-05-05 16:03:16.035343 T3SF-2.0rc1/PKG-INFO
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4094 2023-04-26 15:27:46.000000 T3SF-2.0rc1/README.md
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      103 2023-05-05 16:03:16.035343 T3SF-2.0rc1/setup.cfg
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1128 2023-05-05 16:03:02.000000 T3SF-2.0rc1/setup.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/T3SF/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    14899 2023-05-05 03:47:07.000000 T3SF-2.0rc1/src/T3SF/T3SF.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-04-10 17:12:06.000000 T3SF-2.0rc1/src/T3SF/__init__.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/T3SF/discord/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       47 2023-04-10 17:12:06.000000 T3SF-2.0rc1/src/T3SF/discord/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6754 2023-05-05 03:50:40.000000 T3SF-2.0rc1/src/T3SF/discord/bot.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    10672 2023-05-05 03:58:00.000000 T3SF-2.0rc1/src/T3SF/discord/discord.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/T3SF/gui/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-04-10 17:12:06.000000 T3SF-2.0rc1/src/T3SF/gui/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4252 2023-05-05 15:15:11.000000 T3SF-2.0rc1/src/T3SF/gui/core.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/T3SF/gui/templates/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4458 2023-04-19 14:36:52.000000 T3SF-2.0rc1/src/T3SF/gui/templates/base.html
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     5575 2023-04-19 15:52:23.000000 T3SF-2.0rc1/src/T3SF/gui/templates/env_creation.html
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7809 2023-05-05 03:49:36.000000 T3SF-2.0rc1/src/T3SF/gui/templates/index.html
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     3603 2023-05-05 15:17:00.000000 T3SF-2.0rc1/src/T3SF/gui/templates/msel_viewer.html
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/T3SF/logger/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       21 2023-04-10 17:12:06.000000 T3SF-2.0rc1/src/T3SF/logger/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1452 2023-04-28 16:51:21.000000 T3SF-2.0rc1/src/T3SF/logger/logger.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/T3SF/slack/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       43 2023-04-10 17:12:06.000000 T3SF-2.0rc1/src/T3SF/slack/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6520 2023-05-05 15:14:14.000000 T3SF-2.0rc1/src/T3SF/slack/bot.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    16784 2023-04-27 16:18:20.000000 T3SF-2.0rc1/src/T3SF/slack/slack.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/T3SF.egg-info/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4748 2023-05-05 16:03:15.000000 T3SF-2.0rc1/src/T3SF.egg-info/PKG-INFO
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      647 2023-05-05 16:03:16.000000 T3SF-2.0rc1/src/T3SF.egg-info/SOURCES.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        1 2023-05-05 16:03:15.000000 T3SF-2.0rc1/src/T3SF.egg-info/dependency_links.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       77 2023-05-05 16:03:15.000000 T3SF-2.0rc1/src/T3SF.egg-info/requires.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        5 2023-05-05 16:03:15.000000 T3SF-2.0rc1/src/T3SF.egg-info/top_level.txt
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)    35149 2022-04-20 14:58:09.000000 T3SF-2.1rc1/LICENSE
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       42 2023-04-05 17:28:50.000000 T3SF-2.1rc1/MANIFEST.in
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4748 2023-06-02 16:39:23.409754 T3SF-2.1rc1/PKG-INFO
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4094 2023-05-30 14:58:35.000000 T3SF-2.1rc1/README.md
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      103 2023-06-02 16:39:23.409754 T3SF-2.1rc1/setup.cfg
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1128 2023-06-02 16:38:11.000000 T3SF-2.1rc1/setup.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.405754 T3SF-2.1rc1/src/
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.405754 T3SF-2.1rc1/src/T3SF/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    14869 2023-06-02 16:18:59.000000 T3SF-2.1rc1/src/T3SF/T3SF.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/__init__.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/discord/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       47 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/discord/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7356 2023-06-02 15:53:09.000000 T3SF-2.1rc1/src/T3SF/discord/bot.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    10375 2023-06-02 16:23:53.000000 T3SF-2.1rc1/src/T3SF/discord/discord.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/gui/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/gui/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4987 2023-06-02 16:22:50.000000 T3SF-2.1rc1/src/T3SF/gui/core.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/gui/templates/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4458 2023-05-30 15:48:00.000000 T3SF-2.1rc1/src/T3SF/gui/templates/base.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     5575 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/gui/templates/env_creation.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     8065 2023-06-02 16:23:01.000000 T3SF-2.1rc1/src/T3SF/gui/templates/index.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     3603 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/gui/templates/msel_viewer.html
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/logger/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       21 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/logger/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1452 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/logger/logger.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/slack/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       43 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/slack/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7129 2023-05-30 16:20:25.000000 T3SF-2.1rc1/src/T3SF/slack/bot.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    11646 2023-06-02 16:23:56.000000 T3SF-2.1rc1/src/T3SF/slack/slack.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      682 2023-06-02 16:25:20.000000 T3SF-2.1rc1/src/T3SF/utils.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF.egg-info/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4748 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/PKG-INFO
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      665 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/SOURCES.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        1 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/dependency_links.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       77 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/requires.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        5 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/top_level.txt
```

### Comparing `T3SF-2.0rc1/LICENSE` & `T3SF-2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `T3SF-2.0rc1/PKG-INFO` & `T3SF-2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: T3SF
-Version: 2.0rc1
+Version: 2.1rc1
 Summary: Technical Tabletop Exercises Simulation Framework
 Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security
 Author-email: jlanfranconi@base4sec.com
 Project-URL: Bug Tracker, https://github.com/Base4Security/T3SF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: T3SF Version: 2.0rc1 Summary: Technical Tabletop
+Metadata-Version: 2.1 Name: T3SF Version: 2.1rc1 Summary: Technical Tabletop
 Exercises Simulation Framework Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security Author-email: jlanfranconi@base4sec.com Project-URL: Bug
 Tracker, https://github.com/Base4Security/T3SF/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown Provides-Extra: Slack
```

### Comparing `T3SF-2.0rc1/README.md` & `T3SF-2.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `T3SF-2.0rc1/setup.py` & `T3SF-2.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="T3SF",
-    version="2.0-rc1",
+    version="2.1-rc1",
     author="BASE4 Security",
     author_email="jlanfranconi@base4sec.com",
     description="Technical Tabletop Exercises Simulation Framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Base4Security/T3SF",
     project_urls={
```

### Comparing `T3SF-2.0rc1/src/T3SF/T3SF.py` & `T3SF-2.1rc1/src/T3SF/T3SF.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Internal logging
 from .logger import T3SF_Logger
 # / Internal logging
 
 def keyboard_interrupt_handler(signal_num, frame):
 	T3SF_Logger.emit(message=f"KeyboardInterrupt (ID: {signal_num}) has been caught. Exiting...", message_type="WARN")
-	os.kill(os.getpid(), signal.SIGTERM)
+	os._exit(1)
 
 # Associate the signal handler function with SIGINT (keyboard interrupt)
 signal.signal(signal.SIGINT, keyboard_interrupt_handler)
 
 
 class T3SF(object):
 	def __init__(self, bot = None, app = None, platform = None):
@@ -325,15 +325,15 @@
 				text_input = {"action_id": "regex_custom", "label": "Please type the desired regex. EG: inbox-", "dispatch_action": True}
 				image = {"image_url":"https://i.ibb.co/34rTqMH/image.png", "name": "regex"}
 
 			elif payload['action_id'] == "regex_custom":
 				regex = body['actions'][0]['value']
 				color="GREEN"
 				title="✅ Regex accepted!"
-				description=f"Thanks for confirming the regex for the channels, we are going to use `{user_regex}` to match the inboxes!"
+				description=f"Thanks for confirming the regex for the channels, we are going to use `{regex}` to match the inboxes!"
 
 			self.response_auto = await self.EditMessage(title = title, description = description, color=color, image=image, text_input=text_input, response=self.response_auto)
 
 			if regex != None:
 				await self.slack.InboxesAuto(T3SF_instance=self, regex=regex)
 
 	async def PollAnswerHandler(self, ack=None, body=None, payload=None, query=None):
```

### Comparing `T3SF-2.0rc1/src/T3SF/discord/bot.py` & `T3SF-2.1rc1/src/T3SF/discord/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 bot_discord = commands.Bot(command_prefix='!', intents=intents)
 
 # Defining global variables and events
 T3SF_instance = None
 start_incidents_gui = asyncio.Event()
 create_env = asyncio.Event()
 config_MSEL = None
+
 class create_bot():
 	def __init__(self, MSEL):
 		global config_MSEL
 		config_MSEL = MSEL
 		self.define_commands()
 
 	def define_commands(self):
@@ -63,14 +64,25 @@
 				await T3SF_instance.ProcessIncidents(MSEL = config_MSEL, function_type = "start", ctx=ctx)
 
 			except Exception as e:
 				print("ERROR - Start function")
 				print(e)
 				raise
 
+		@bot_discord.event
+		async def on_command_error(ctx, error):
+		    """
+		    Inform if an error with the commands ocurred.
+		    """
+		    if isinstance(error, commands.errors.CheckFailure):
+		        await ctx.send(embed=discord.Embed(colour=discord.Colour.red(), title="Error 401", description='You do not have the "Game Master" role to use this command.'))
+
+		    elif isinstance(error, discord.HTTPException):
+		        await ctx.send(embed=discord.Embed(colour=discord.Colour.red(), title="Error 5xx", description="We got ratelimited by Discord. Please wait a few seconds and try again."))
+
 async def start_bot():
 	T3SF_instance = T3SF.T3SF(platform="discord", bot=bot_discord)
 	task1 = asyncio.create_task(bot_discord.start(TOKEN))
 	task2 = asyncio.create_task(async_handler_exercise())
 	task3 = asyncio.create_task(create_environment_task())
 
 	# wait for the coroutines to finish
@@ -210,15 +222,15 @@
 	role = discord.utils.get(guild.roles, name="Game Master")
 	
 	if role is None:
 		all_perms = discord.Permissions.all()
 		role = await guild.create_role(name="Game Master", permissions=all_perms, colour=discord.Colour.green())
 
 	category = await create_category_if_not_exists(guild=guild, name="Control Room", private=True, role=role)
-	channels = ['chat','logs']
+	channels = ['gm-chat','logs']
 
 	for channel in channels:
 		await create_channel_if_not_exists(category=category, name=channel)
 	
 	await create_voice_if_not_exists(category=category, name="Game Masters")
 
 	T3SF.T3SF_Logger.emit(message=f'Game Master channels created.', message_type="INFO")
```

### Comparing `T3SF-2.0rc1/src/T3SF/discord/discord.py` & `T3SF-2.1rc1/src/T3SF/discord/discord.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,236 +1,229 @@
-from difflib import SequenceMatcher
 import discord
 import asyncio
 import random
 import json
 import re 
+from T3SF import utils
 
 class Discord(object):
+	def __init__(self, bot):
+		self.bot = bot
 
-		def __init__(self, bot):
-			self.bot = bot
-
-		async def InboxesAuto(self, T3SF_instance):
-			mensaje_inboxes = ""
-			image_example = "https://i.ibb.co/NCrPD3Y/discord-exp.png"
-
-			if T3SF_instance.fetch_inboxes == True:
-				if T3SF_instance._ctx == None:
-					# Exercise started from the GUI
-					guild = self.bot.get_guild(int(T3SF_instance.guild_id))
-					channels = guild.text_channels
-
-					for channel in channels:
-						if "chat" in channel.name:
-							accuracy = similar(str(channel.name).lower(),"gm-chat")
-							if accuracy >= 0.8:
-								inbox = channel.id
-								T3SF_instance._ctx = self.bot.get_channel(channel.id)
-
-				T3SF_instance.response_auto = await self.SendMessage(T3SF_instance=T3SF_instance, title="⚙️ Fetching inboxes...", description=f"Please wait while we fetch all the inboxes in this server!", color="BLUE")
-
-				channels_itinerator = 0
-				player_itinerator = 0
-				regex = ""
-
-				try:
-					channels = T3SF_instance._ctx.message.guild.channels
-					categories = T3SF_instance._ctx.message.guild.categories
-					started_from_gui = False
-
-				except Exception:
-					channels = T3SF_instance._ctx.guild.channels
-					categories = T3SF_instance._ctx.guild.categories
-					started_from_gui = True
-
-				while regex == "" and len(T3SF_instance.players_list) > player_itinerator:
-					for category in categories:
-						if channels_itinerator == 0:
-							past_channel = category.name
-							pass
-						
-						match_channel = similar(str(category).lower(), str(T3SF_instance.players_list[0]).lower())
-						
-						if match_channel >= 0.4:
-							for character in past_channel:
-								if character in category.name:
-									regex += character
-								else:
-									break
-						else:
-							player_itinerator += 1
-							channels_itinerator += 1
-							past_channel = category.name
-							pass
-
-				await T3SF_instance.response_auto.edit(embed=discord.Embed(
-				 title = "ℹ️ Regex detected!",
-				 description = f"Please confirm if the regex detected for the channels, is correct so we can get the inboxes!\n\nExample:\nGroup - Legal\nThe regex should be `Group -`\n\nDetected regex: `{regex}`",
-				 color = 0x77B255).set_image(url=image_example).set_footer(text="Please answer with [Yes(Y)/No(N)]"))
-
-				def check_regex_channels(msg):
-					if started_from_gui:
-						return msg.content.lower() in ["y", "yes", "n", "no"]
-
+	async def InboxesAuto(self, T3SF_instance):
+		mensaje_inboxes = ""
+		image_example = "https://i.ibb.co/NCrPD3Y/discord-exp.png"
+
+		if T3SF_instance.fetch_inboxes == True:
+			if T3SF_instance._ctx == None:
+				# Exercise started from the GUI
+				guild = self.bot.get_guild(int(T3SF_instance.guild_id))
+				channels = guild.text_channels
+
+				for channel in channels:
+					if "chat" in channel.name:
+						accuracy = utils.similar(str(channel.name).lower(),"gm-chat")
+						if accuracy >= 0.8:
+							inbox = channel.id
+							T3SF_instance._ctx = self.bot.get_channel(channel.id)
+
+			T3SF_instance.response_auto = await self.SendMessage(T3SF_instance=T3SF_instance, title="⚙️ Fetching inboxes...", description=f"Please wait while we fetch all the inboxes in this server!", color="BLUE")
+
+			channels_itinerator = 0
+			player_itinerator = 0
+			regex = ""
+
+			try:
+				channels = T3SF_instance._ctx.message.guild.channels
+				categories = T3SF_instance._ctx.message.guild.categories
+				started_from_gui = False
+
+			except Exception:
+				channels = T3SF_instance._ctx.guild.channels
+				categories = T3SF_instance._ctx.guild.categories
+				started_from_gui = True
+
+			while regex == "" and len(T3SF_instance.players_list) > player_itinerator:
+				for category in categories:
+					if channels_itinerator == 0:
+						past_channel = category.name
+						pass
+					
+					match_channel = utils.similar(str(category).lower(), str(T3SF_instance.players_list[0]).lower())
+					
+					if match_channel >= 0.4:
+						for character in past_channel:
+							if character in category.name:
+								regex += character
+							else:
+								break
 					else:
-						return msg.author == T3SF_instance._ctx.author and msg.channel == T3SF_instance._ctx.channel and msg.content.lower() in ["y", "yes", "n", "no"]
+						player_itinerator += 1
+						channels_itinerator += 1
+						past_channel = category.name
+						pass
+
+			await T3SF_instance.response_auto.edit(embed=discord.Embed(
+			 title = "ℹ️ Regex detected!",
+			 description = f"Please confirm if the regex detected for the channels, is correct so we can get the inboxes!\n\nExample:\nGroup - Legal\nThe regex should be `Group -`\n\nDetected regex: `{regex}`",
+			 color = 0x77B255).set_image(url=image_example).set_footer(text="Please answer with [Yes(Y)/No(N)]"))
+
+			def check_regex_channels(msg):
+				if started_from_gui:
+					return msg.content.lower() in ["y", "yes", "n", "no"]
+
+				else:
+					return msg.author == T3SF_instance._ctx.author and msg.channel == T3SF_instance._ctx.channel and msg.content.lower() in ["y", "yes", "n", "no"]
+
+			try:
+				msg = await self.bot.wait_for("message", check=check_regex_channels, timeout=50)
+
+				if msg.content.lower() in ["y", "yes"]:
+					await self.EditMessage(T3SF_instance=T3SF_instance, style="custom", variable="T3SF_instance.response_auto", color="GREEN", title = "✨ Regex detected succesfully! ✨", description = f"Thanks for confirming the regex detected for the channels (I'm going to tell my creator he is so good coding :D ), we are going to use `{regex}` to match the inboxes")
+
+				elif msg.content.lower() in ["n", "no"]:
+					await T3SF_instance.response_auto.edit(embed=discord.Embed(
+					 title = "ℹ️ Regex needed!",
+					 description = "Got it!\n Unluckily, but here we go...\nPlease send me the regex for the channels, so we can get the inboxes!\n\nExample:\nGroup - Legal\nThe regex should be `Group -`",
+					 color = discord.Colour.red()).set_image(url=image_example).set_footer(text="Please answer with the desired regex. EG: `Groups -`"))
 
-				try:
-					msg = await self.bot.wait_for("message", check=check_regex_channels, timeout=50)
+					def get_regex_channels(msg_regex_user):
+						# return msg_regex_user.author == T3SF_instance._ctx.author and msg_regex_user.channel == T3SF_instance._ctx.channel and 
 
-					if msg.content.lower() in ["y", "yes"]:
-						await self.EditMessage(T3SF_instance=T3SF_instance, style="custom", variable="T3SF_instance.response_auto", color="GREEN", title = "✨ Regex detected succesfully! ✨", description = f"Thanks for confirming the regex detected for the channels (I'm going to tell my creator he is so good coding :D ), we are going to use `{regex}` to match the inboxes")
+						if started_from_gui:
+							return msg_regex_user.content != ""
 
-					elif msg.content.lower() in ["n", "no"]:
-						await T3SF_instance.response_auto.edit(embed=discord.Embed(
-						 title = "ℹ️ Regex needed!",
-						 description = "Got it!\n Unluckily, but here we go...\nPlease send me the regex for the channels, so we can get the inboxes!\n\nExample:\nGroup - Legal\nThe regex should be `Group -`",
-						 color = discord.Colour.red()).set_image(url=image_example).set_footer(text="Please answer with the desired regex. EG: `Groups -`"))
+						else:
+							return msg_regex_user.author == T3SF_instance._ctx.author and msg_regex_user.channel == T3SF_instance._ctx.channel and msg_regex_user.content != ""
+					
+					msg_regex_user = await self.bot.wait_for("message", check=get_regex_channels, timeout=50)
+
+					if msg_regex_user.content != "":
+						regex = msg_regex_user
+						await self.EditMessage(T3SF_instance=T3SF_instance, style="custom", variable="T3SF_instance.response_auto", color="GREEN", title="✅ Regex accepted!", description=f"Thanks for confirming the regex for the channels, we are going to use `{msg_regex_user.content}` to match the inboxes!")
+
+			except asyncio.TimeoutError:
+				await self.EditMessage(T3SF_instance=T3SF_instance, style="custom", variable="T3SF_instance.response_auto", color="RED", title = ":x: Sorry, you didn't reply on time", description = "Please start the process again.")
+				raise RuntimeError("We didn't detect any regex, time's up.")
+
+			for player in T3SF_instance.players_list:
+				for channel in channels:
+					category = channel.category
+					if "inbox" in channel.name :
+						accuracy = utils.similar(re.sub(f"({regex})", "",str(category)).lower(),str(player).lower())
+						if accuracy >= 0.4:
+							T3SF_instance.inboxes_all[player] = channel.id
+			
+			json.dump(T3SF_instance.inboxes_all,open(f"inboxes_{T3SF_instance.platform}.json", "w"))
 
-						def get_regex_channels(msg_regex_user):
-							# return msg_regex_user.author == T3SF_instance._ctx.author and msg_regex_user.channel == T3SF_instance._ctx.channel and 
+			for player in T3SF_instance.inboxes_all:
+				mensaje_inboxes += f"**Inbox** {player}[{T3SF_instance.inboxes_all[player]}]\n"
 
-							if started_from_gui:
-								return msg_regex_user.content != ""
+			await self.EditMessage(T3SF_instance=T3SF_instance, style="custom", variable="T3SF_instance.response_auto", color="GREEN", title=f"📩  Inboxes fetched! [{len(T3SF_instance.inboxes_all)}]", description=mensaje_inboxes)
 
-							else:
-								return msg_regex_user.author == T3SF_instance._ctx.author and msg_regex_user.channel == T3SF_instance._ctx.channel and msg_regex_user.content != ""
-						
-						msg_regex_user = await self.bot.wait_for("message", check=get_regex_channels, timeout=50)
-
-						if msg_regex_user.content != "":
-							regex = msg_regex_user
-							await self.EditMessage(T3SF_instance=T3SF_instance, style="custom", variable="T3SF_instance.response_auto", color="GREEN", title="✅ Regex accepted!", description=f"Thanks for confirming the regex for the channels, we are going to use `{msg_regex_user.content}` to match the inboxes!")
-
-				except asyncio.TimeoutError:
-					await self.EditMessage(T3SF_instance=T3SF_instance, style="custom", variable="T3SF_instance.response_auto", color="RED", title = ":x: Sorry, you didn't reply on time", description = "Please start the process again.")
-					raise RuntimeError("We didn't detect any regex, time's up.")
-
-				for player in T3SF_instance.players_list:
-					for channel in channels:
-						category = channel.category
-						if "inbox" in channel.name :
-							accuracy = similar(re.sub(f"({regex})", "",str(category)).lower(),str(player).lower())
-							if accuracy >= 0.4:
-								T3SF_instance.inboxes_all[player] = channel.id
-				
-				json.dump(T3SF_instance.inboxes_all,open(f"inboxes_{T3SF_instance.platform}.json", "w"))
+		return True
 
-				for player in T3SF_instance.inboxes_all:
-					mensaje_inboxes += f"**Inbox** {player}[{T3SF_instance.inboxes_all[player]}]\n"
+	async def InjectHandler(self, T3SF_instance):
+		all_data = f'Date: {T3SF_instance._inject["Date"]}\n\n{T3SF_instance._inject["Script"]}'
 
-				await self.EditMessage(T3SF_instance=T3SF_instance, style="custom", variable="T3SF_instance.response_auto", color="GREEN", title=f"📩  Inboxes fetched! [{len(T3SF_instance.inboxes_all)}]", description=mensaje_inboxes)
+		player = T3SF_instance._inject['Player']
 
-			return True
+		inbox = self.bot.get_channel(T3SF_instance.inboxes_all[player])
 
-		async def InjectHandler(self, T3SF_instance):
-			all_data = f'Date: {T3SF_instance._inject["Date"]}\n\n{T3SF_instance._inject["Script"]}'
+		embed = discord.Embed(title = T3SF_instance._inject['Subject'], description = all_data, color = discord.Colour.blue())
+		
+		if "Photo" in T3SF_instance._inject and T3SF_instance._inject['Photo'] != '':
+			embed.set_image(url=T3SF_instance._inject['Photo'])
+		
+		if "Profile" in T3SF_instance._inject and T3SF_instance._inject['Profile'] != '':
+			profile_pic = T3SF_instance._inject['Profile']
+		else:
+			profile_pic = random.choice([
+				"https://ssl.gstatic.com/ui/v1/icons/mail/profile_mask2.png",
+				"https://lh3.googleusercontent.com/-XdUIqdMkCWA/AAAAAAAAAAI/AAAAAAAAAAA/4252rscbv5M/photo.jpg",
+				"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSTt8Dg9RL4IGOjsJ2Fr-lXThf-DGM5YgPB6j5rD8tHQ9RLrU-03H4dYeskL01FNajqL_0&usqp=CAU"
+			])
 
-			player = T3SF_instance._inject['Player']
+		embed.set_author(name=T3SF_instance._inject["From"], icon_url=profile_pic)
 
-			inbox = self.bot.get_channel(T3SF_instance.inboxes_all[player])
+		T3SF_instance.response_poll = await inbox.send(embed = embed)
 
-			embed = discord.Embed(title = T3SF_instance._inject['Subject'], description = all_data, color = discord.Colour.blue())
-			
-			if "Photo" in T3SF_instance._inject and T3SF_instance._inject['Photo'] != '':
-				embed.set_image(url=T3SF_instance._inject['Photo'])
-			
-			if "Profile" in T3SF_instance._inject and T3SF_instance._inject['Profile'] != '':
-				profile_pic = T3SF_instance._inject['Profile']
-			else:
-				profile_pic = random.choice([
-					"https://ssl.gstatic.com/ui/v1/icons/mail/profile_mask2.png",
-					"https://lh3.googleusercontent.com/-XdUIqdMkCWA/AAAAAAAAAAI/AAAAAAAAAAA/4252rscbv5M/photo.jpg",
-					"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSTt8Dg9RL4IGOjsJ2Fr-lXThf-DGM5YgPB6j5rD8tHQ9RLrU-03H4dYeskL01FNajqL_0&usqp=CAU"
-				])
-
-			embed.set_author(name=T3SF_instance._inject["From"], icon_url=profile_pic)
+		return embed
 
-			T3SF_instance.response_poll = await inbox.send(embed = embed)
+	async def PollHandler(self, T3SF_instance):
+		T3SF_instance.poll_answered = False
 
-			return embed
+		all_data = T3SF_instance._inject["Script"]
 
-		async def PollHandler(self, T3SF_instance):
-			T3SF_instance.poll_answered = False
+		poll_options = T3SF_instance._inject['Poll'].split('|')
+		
+		actual_real_time = re.sub("([^0-9])", "", T3SF_instance._inject['Real Time'])[-2:]
+		
+		next_real_time = re.sub("([^0-9])", "", T3SF_instance.data[int(T3SF_instance._inject['#'])]['Real Time'])[-2:]
 
-			all_data = T3SF_instance._inject["Script"]
-
-			poll_options = T3SF_instance._inject['Poll'].split('|')
-			
-			actual_real_time = re.sub("([^0-9])", "", T3SF_instance._inject['Real Time'])[-2:]
-			
-			next_real_time = re.sub("([^0-9])", "", T3SF_instance.data[int(T3SF_instance._inject['#'])]['Real Time'])[-2:]
+		diff = int(next_real_time) - int(actual_real_time)
+		if diff < 0:
+			diff_no_real = int(actual_real_time) - int(next_real_time)
+			diff = 60 - diff_no_real 
 
-			diff = int(next_real_time) - int(actual_real_time)
-			if diff < 0:
-				diff_no_real = int(actual_real_time) - int(next_real_time)
-				diff = 60 - diff_no_real 
+		diff_secs = diff * 60
 
-			diff_secs = diff * 60
+		view = discord.ui.View()
+		view.add_item(discord.ui.Button(style=discord.ButtonStyle.primary,label=poll_options[0], custom_id="poll|"+poll_options[0]))
+		view.add_item(discord.ui.Button(style=discord.ButtonStyle.primary,label=poll_options[1], custom_id="poll|"+poll_options[1]))
 
-			view = discord.ui.View()
-			view.add_item(discord.ui.Button(style=discord.ButtonStyle.primary,label=poll_options[0], custom_id="poll|"+poll_options[0]))
-			view.add_item(discord.ui.Button(style=discord.ButtonStyle.primary,label=poll_options[1], custom_id="poll|"+poll_options[1]))
+		all_data = all_data+ f"\n\nYou have {diff} minute(s) to answer this poll!"
 
-			all_data = all_data+ f"\n\nYou have {diff} minute(s) to answer this poll!"
+		player = T3SF_instance._inject['Player']
 
-			player = T3SF_instance._inject['Player']
+		inbox = self.bot.get_channel(T3SF_instance.inboxes_all[player])
 
-			inbox = self.bot.get_channel(T3SF_instance.inboxes_all[player])
+		embed = discord.Embed(title = T3SF_instance._inject['Subject'], description = all_data, color = discord.Colour.yellow())
 
-			embed = discord.Embed(title = T3SF_instance._inject['Subject'], description = all_data, color = discord.Colour.yellow())
+		if "Photo" in T3SF_instance._inject and T3SF_instance._inject['Photo'] != '':
+			embed.set_image(url=T3SF_instance._inject['Photo'])
 
-			if "Photo" in T3SF_instance._inject and T3SF_instance._inject['Photo'] != '':
-				embed.set_image(url=T3SF_instance._inject['Photo'])
+		T3SF_instance.response_poll = await inbox.send(embed = embed, view=view)
 
-			T3SF_instance.response_poll = await inbox.send(embed = embed, view=view)
+		return embed
 
-			return embed
+	async def PollAnswerHandler(self, T3SF_instance, interaction=None):
+		if "poll" in interaction.data['custom_id']:
+			poll_msg_og = interaction.message.embeds.copy()[0]
 
-		async def PollAnswerHandler(self, T3SF_instance, interaction=None):
-			if "poll" in interaction.data['custom_id']:
-				poll_msg_og = interaction.message.embeds.copy()[0]
+			title =  poll_msg_og.title
 
-				title =  poll_msg_og.title
+			poll_msg = poll_msg_og.description
+			poll_msg = poll_msg[: poll_msg.rfind('\n')]
 
-				poll_msg = poll_msg_og.description
-				poll_msg = poll_msg[: poll_msg.rfind('\n')]
+			action_user = interaction.user
 
-				action_user = interaction.user
+			selected_option = interaction.data['custom_id'].split('|')[1]
+			description = f'{poll_msg}\n\n@{action_user} selected: {selected_option}'               
 
-				selected_option = interaction.data['custom_id'].split('|')[1]
-				description = f'{poll_msg}\n\n@{action_user} selected: {selected_option}'               
+			T3SF_instance.poll_answered = True
+			T3SF_instance.response_poll = await interaction.response.edit_message(embed=discord.Embed(colour=discord.Colour.green(), title=title, description=description),view=None)
+			await T3SF_instance.NotifyGameMasters(type_info="poll_answered", data={'msg_poll':poll_msg,'answer':selected_option,'user':action_user})
+			return True
+		else:
+			pass
 
-				T3SF_instance.poll_answered = True
-				T3SF_instance.response_poll = await interaction.response.edit_message(embed=discord.Embed(colour=discord.Colour.green(), title=title, description=description),view=None)
-				await T3SF_instance.NotifyGameMasters(type_info="poll_answered", data={'msg_poll':poll_msg,'answer':selected_option,'user':action_user})
-				return True
-			else:
-				pass
+	async def SendMessage(self, T3SF_instance, color="CYAN", title:str=None, description:str=None, view=None, unique=False):
+		colors = {'BLUE' : discord.Colour.dark_blue(), 'RED' : discord.Colour.red(), 'CYAN' : discord.Colour.blue(), 'GREEN' : discord.Colour.green(), 'YELLOW' : discord.Colour.yellow()}
 
-		async def SendMessage(self, T3SF_instance, color="CYAN", title:str=None, description:str=None, view=None, unique=False):
+		if unique == True:
+			T3SF_instance.gm_poll_msg = await T3SF_instance._ctx.send(embed=discord.Embed(color=colors[color], title = title, description = description), view=view)
+			return T3SF_instance.gm_poll_msg
+		
+		else:
+			T3SF_instance.response = await T3SF_instance._ctx.send(embed=discord.Embed(color=colors[color], title = title, description = description), view=view)
+			return T3SF_instance.response
+
+	async def EditMessage(self, T3SF_instance=None, color="CYAN", title:str=None, description:str=None, view=None, style="simple", variable=None):
+
+		if style == "simple":
+			T3SF_instance.response = T3SF_instance.response.edit(embed=discord.Embed(color=colors[color], title = title, description = description), view=view)
+			return T3SF_instance.response
+		else:
 			colors = {'BLUE' : discord.Colour.dark_blue(), 'RED' : discord.Colour.red(), 'CYAN' : discord.Colour.blue(), 'GREEN' : discord.Colour.green(), 'YELLOW' : discord.Colour.yellow()}
-
-			if unique == True:
-				T3SF_instance.gm_poll_msg = await T3SF_instance._ctx.send(embed=discord.Embed(color=colors[color], title = title, description = description), view=view)
-				return T3SF_instance.gm_poll_msg
-			
-			else:
-				T3SF_instance.response = await T3SF_instance._ctx.send(embed=discord.Embed(color=colors[color], title = title, description = description), view=view)
-				return T3SF_instance.response
-
-		async def EditMessage(self, T3SF_instance=None, color="CYAN", title:str=None, description:str=None, view=None, style="simple", variable=None):
-
-			if style == "simple":
-				T3SF_instance.response = T3SF_instance.response.edit(embed=discord.Embed(color=colors[color], title = title, description = description), view=view)
-				return T3SF_instance.response
-			else:
-				colors = {'BLUE' : discord.Colour.dark_blue(), 'RED' : discord.Colour.red(), 'CYAN' : discord.Colour.blue(), 'GREEN' : discord.Colour.green(), 'YELLOW' : discord.Colour.yellow()}
-				variable = eval(variable)
-				await variable.edit(embed=discord.Embed(color=colors[color], title = title, description = description), view=view)
-
-def similar(a, b):
-	"""
-	Based in graphics, find the similarity between 2 strings.
-	"""
-	return SequenceMatcher(None, a, b).ratio()
+			variable = eval(variable)
+			await variable.edit(embed=discord.Embed(color=colors[color], title = title, description = description), view=view)
```

### Comparing `T3SF-2.0rc1/src/T3SF/gui/templates/base.html` & `T3SF-2.1rc1/src/T3SF/gui/templates/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 	</nav>
 	<!-- Toast Placeholder -->
 	<div class="position-fixed top-0 end-0 p-3" id="toast-container"></div>
 	<footer class="footer fixed-bottom bg-light">
 	  <div class="container-fluid">
 	    <div class="row">
 	      <div class="col text-center text-muted">
-	        <p>Version 2.0 | Found a bug? Let us know! <a href="https://github.com/Base4Security/T3SF/issues/new/choose">Submit a bug report</a>.</p>
+	        <p>Version 2.1 | Found a bug? Let us know! <a href="https://github.com/Base4Security/T3SF/issues/new/choose">Submit a bug report</a>.</p>
 	      </div>
 	    </div>
 	  </div>
 	</footer>
 	<script type="text/javascript">
 		const b5toastContainerElement = document.getElementById("toast-container");
```

#### html2text {}

```diff
@@ -5,9 +5,9 @@
     * Github_Project
     * Logs_Viewer
     * [https://user-images.githubusercontent.com/103124157/164258966-7a049d6c-
       4012-49ca-8f7d-2bb814c24009.png]
     * MSEL_Viewer
     * Create_environment
 
-Version 2.0 | Found a bug? Let us know! Submit_a_bug_report.
+Version 2.1 | Found a bug? Let us know! Submit_a_bug_report.
  {% block content %} {% endblock %}
```

### Comparing `T3SF-2.0rc1/src/T3SF/gui/templates/env_creation.html` & `T3SF-2.1rc1/src/T3SF/gui/templates/env_creation.html`

 * *Files identical despite different names*

### Comparing `T3SF-2.0rc1/src/T3SF/gui/templates/index.html` & `T3SF-2.1rc1/src/T3SF/gui/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -276,15 +276,19 @@
 		var message = JSON.parse(event.data);
 		var messageId = message.id;
 
 		// Get the selected log level
 		var logLevel = $('#logs-level-dropdown').val();
 		var logLevel_stored = localStorage.getItem("log_level");
 
-		if (logLevel !== logLevel_stored) {
+		if (logLevel === null || logLevel_stored === null) {
+			$("#logs-level-dropdown").val("INFO").change();
+			logLevel = "INFO";
+		}
+		else if (logLevel !== logLevel_stored) {
 			$("#logs-level-dropdown").val(logLevel_stored).change();
 			logLevel = logLevel_stored;
 		}
 
 		// Check if the message type matches the filtering condition
 		if (!historic_logs.includes(messageId) && logLevels[logLevel].includes(message.type)) {
 			// Store to the historics
@@ -305,14 +309,16 @@
 			logsContent.scrollTop = logsContent.scrollHeight;
 		}
 	};
 
 	function handle_sse_start(event){
 		console.log("Getting server updates");
 		setStatusIndicatorActive(true);
+		document.getElementById('start-button').disabled = false;
+		document.getElementById('stop-button').disabled = false;
 	};
 
 	function handle_sse_errors(event){
 		console.log('EventSource error:', event);
 		setStatusIndicatorActive(false);
 		document.getElementById('start-button').disabled = true;
 		document.getElementById('stop-button').disabled = true;
```

### Comparing `T3SF-2.0rc1/src/T3SF/gui/templates/msel_viewer.html` & `T3SF-2.1rc1/src/T3SF/gui/templates/msel_viewer.html`

 * *Files identical despite different names*

### Comparing `T3SF-2.0rc1/src/T3SF/logger/logger.py` & `T3SF-2.1rc1/src/T3SF/logger/logger.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.0rc1/src/T3SF/slack/bot.py` & `T3SF-2.1rc1/src/T3SF/slack/bot.py`

 * *Files 13% similar despite different names*

```diff
@@ -93,27 +93,27 @@
 		inbox_name = "inbox"
 		extra_chnls = ['chat','decision-log']
 		players_list_local = areas_msel
 
 		channels_ids = []
 
 		for player in players_list_local:
-			inbox =  inbox_name + "-" + player.lower().replace(" ", "-")
+			inbox =  inbox_name + "-" + sanitize_channel_name(player)
 			try:
 				channel_id_inbox = await create_channel_if_not_exists(channel_name=inbox, private=True)
 				
 				if channel_id_inbox:
 					await app_slack.client.conversations_invite(channel=channel_id_inbox, users=admins_users)
 				
 					channels_ids.append(channel_id_inbox)
 
 					T3SF.T3SF_Logger.emit(message=f'Player [{player}] - Channel {inbox_name} created', message_type="DEBUG")
 
 				for extra in extra_chnls:
-					channel = extra + "-" + player.lower().replace(" ", "-")
+					channel = extra + "-" + sanitize_channel_name(player)
 				
 					channel_id_extra = await create_channel_if_not_exists(channel_name=channel, private=True)
 					if channel_id_extra:
 						await app_slack.client.conversations_invite(channel=channel_id_extra, users=admins_users)
 				
 						channels_ids.append(channel_id_extra)
 
@@ -188,8 +188,29 @@
 	for channel in channels:
 		channel_id = await create_channel_if_not_exists(channel)
 		if channel_id:
 			await app_slack.client.conversations_invite(channel=channel_id, users=admins)
 
 	T3SF.T3SF_Logger.emit(message=f'Game Master channels created.', message_type="INFO")
 
-	return True
+	return True
+
+def sanitize_channel_name(name):
+	# Replace whitespace with a hyphen
+	sanitized_name = re.sub(r"\s", "-", name)
+
+	# Remove special characters except for hyphens and periods
+	sanitized_name = re.sub(r"[^\w.-]", "-", sanitized_name)
+
+	# Replace consecutive hyphens and periods with a single hyphen
+	sanitized_name = re.sub(r"[-.]+", "-", sanitized_name)
+
+	# Remove leading and trailing hyphens
+	sanitized_name = sanitized_name.strip("-")
+
+	# Convert to lowercase
+	sanitized_name = sanitized_name.lower()
+
+	# Truncate to a maximum length of 80 characters
+	sanitized_name = sanitized_name[:80]
+
+	return sanitized_name
```

### Comparing `T3SF-2.0rc1/src/T3SF.egg-info/PKG-INFO` & `T3SF-2.1rc1/src/T3SF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: T3SF
-Version: 2.0rc1
+Version: 2.1rc1
 Summary: Technical Tabletop Exercises Simulation Framework
 Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security
 Author-email: jlanfranconi@base4sec.com
 Project-URL: Bug Tracker, https://github.com/Base4Security/T3SF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: T3SF Version: 2.0rc1 Summary: Technical Tabletop
+Metadata-Version: 2.1 Name: T3SF Version: 2.1rc1 Summary: Technical Tabletop
 Exercises Simulation Framework Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security Author-email: jlanfranconi@base4sec.com Project-URL: Bug
 Tracker, https://github.com/Base4Security/T3SF/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown Provides-Extra: Slack
```

### Comparing `T3SF-2.0rc1/src/T3SF.egg-info/SOURCES.txt` & `T3SF-2.1rc1/src/T3SF.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 src/T3SF/T3SF.py
 src/T3SF/__init__.py
+src/T3SF/utils.py
 src/T3SF.egg-info/PKG-INFO
 src/T3SF.egg-info/SOURCES.txt
 src/T3SF.egg-info/dependency_links.txt
 src/T3SF.egg-info/requires.txt
 src/T3SF.egg-info/top_level.txt
 src/T3SF/discord/__init__.py
 src/T3SF/discord/bot.py
```

