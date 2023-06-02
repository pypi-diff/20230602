# Comparing `tmp/EdgeGPT-0.7.1.tar.gz` & `tmp/EdgeGPT-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.7.1.tar", last modified: Thu Jun  1 12:50:48 2023, max compression
+gzip compressed data, was "EdgeGPT-0.7.2.tar", last modified: Fri Jun  2 15:13:08 2023, max compression
```

## Comparing `EdgeGPT-0.7.1.tar` & `EdgeGPT-0.7.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:50:48.836774 EdgeGPT-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-01 12:50:19.000000 EdgeGPT-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-01 12:50:48.836774 EdgeGPT-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-06-01 12:50:48.000000 EdgeGPT-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 12:50:48.836774 EdgeGPT-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-01 12:50:19.000000 EdgeGPT-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:50:48.836774 EdgeGPT-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:50:48.836774 EdgeGPT-0.7.1/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-01 12:50:48.000000 EdgeGPT-0.7.1/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-01 12:50:48.000000 EdgeGPT-0.7.1/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:50:48.000000 EdgeGPT-0.7.1/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 12:50:48.000000 EdgeGPT-0.7.1/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 12:50:48.000000 EdgeGPT-0.7.1/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 12:50:48.000000 EdgeGPT-0.7.1/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    43455 2023-06-01 12:50:19.000000 EdgeGPT-0.7.1/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-01 12:50:19.000000 EdgeGPT-0.7.1/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:13:08.705255 EdgeGPT-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-02 15:12:29.000000 EdgeGPT-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-06-02 15:13:08.705255 EdgeGPT-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-06-02 15:13:08.000000 EdgeGPT-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 15:13:08.705255 EdgeGPT-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-02 15:12:29.000000 EdgeGPT-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:13:08.701255 EdgeGPT-0.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:13:08.705255 EdgeGPT-0.7.2/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-06-02 15:13:08.000000 EdgeGPT-0.7.2/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 15:13:08.000000 EdgeGPT-0.7.2/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:13:08.000000 EdgeGPT-0.7.2/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-02 15:13:08.000000 EdgeGPT-0.7.2/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-02 15:13:08.000000 EdgeGPT-0.7.2/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 15:13:08.000000 EdgeGPT-0.7.2/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    43363 2023-06-02 15:12:29.000000 EdgeGPT-0.7.2/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 15:12:29.000000 EdgeGPT-0.7.2/src/ImageGen.py
```

### Comparing `EdgeGPT-0.7.1/LICENSE` & `EdgeGPT-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.7.1/PKG-INFO` & `EdgeGPT-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.7.1
+Version: 0.7.2
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -156,15 +156,15 @@
 ### 2) The `Query` and `Cookie` helper classes
 
   </summary>
 
 Create a simple Bing Chat AI query (using the 'precise' conversation style by default) and see just the main text output rather than the whole API response:
 
 Remeber to store your cookies in a specific format: `bing_cookie_*.json`.
-  
+
 ```python
 from EdgeGPT import Query, Cookie
 
 q = Query("What are you? Give your answer as Python code")
 print(q)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.7.1 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.7.2 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.7.1/README.md` & `EdgeGPT-0.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 ### 2) The `Query` and `Cookie` helper classes
 
   </summary>
 
 Create a simple Bing Chat AI query (using the 'precise' conversation style by default) and see just the main text output rather than the whole API response:
 
 Remeber to store your cookies in a specific format: `bing_cookie_*.json`.
-  
+
 ```python
 from EdgeGPT import Query, Cookie
 
 q = Query("What are you? Give your answer as Python code")
 print(q)
 ```
```

### Comparing `EdgeGPT-0.7.1/setup.py` & `EdgeGPT-0.7.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
 DOCS_PATH = Path(__file__).parents[0] / "docs/README.md"
 PATH = Path("README.md")
 if not PATH.exists():
-    with open(DOCS_PATH, encoding="utf-8") as f1:
-        with open(PATH, "w+", encoding="utf-8") as f2:
+    with Path.open(DOCS_PATH, encoding="utf-8") as f1:
+        with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.7.1",
+    version="0.7.2",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
@@ -33,15 +33,15 @@
         "rich",
         "certifi",
         "prompt_toolkit",
         "requests",
         "aiofiles",
         "BingImageCreator>=0.3.0",
     ],
-    long_description=open(PATH, encoding="utf-8").read(),
+    long_description=Path.open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["EdgeGPT", "ImageGen"],
     classifiers=[
         "License :: OSI Approved :: The Unlicense (Unlicense)",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
```

### Comparing `EdgeGPT-0.7.1/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.7.2/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.7.1
+Version: 0.7.2
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -156,15 +156,15 @@
 ### 2) The `Query` and `Cookie` helper classes
 
   </summary>
 
 Create a simple Bing Chat AI query (using the 'precise' conversation style by default) and see just the main text output rather than the whole API response:
 
 Remeber to store your cookies in a specific format: `bing_cookie_*.json`.
-  
+
 ```python
 from EdgeGPT import Query, Cookie
 
 q = Query("What are you? Give your answer as Python code")
 print(q)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.7.1 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.7.2 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.7.1/src/EdgeGPT.py` & `EdgeGPT-0.7.2/src/EdgeGPT.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """
 Main.py
 """
 from __future__ import annotations
 
 import argparse
 import asyncio
-import aiofiles
 import json
 import os
 import random
 import re
 import ssl
 import sys
 import time
 import uuid
 from enum import Enum
 from pathlib import Path
 from typing import Generator
 
+import aiofiles
+
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 from typing import Optional
-from typing import Union
 
 import aiohttp
 import certifi
 import httpx
 from BingImageCreator import ImageGen
 from BingImageCreator import ImageGenAsync
 from prompt_toolkit import PromptSession
@@ -113,15 +113,15 @@
                 "countryConfidence": 8,
                 "Center": {
                     "Latitude": 34.0536909,
                     "Longitude": -118.242766,
                 },
                 "RegionType": 2,
                 "SourceType": 1,
-            }
+            },
         ],
     }
     CHINA = {
         "locale": "zh-CN",
         "LocationHint": [
             {
                 "country": "China",
@@ -131,15 +131,15 @@
                 "countryConfidence": 8,
                 "Center": {
                     "Latitude": 39.9042,
                     "Longitude": 116.4074,
                 },
                 "RegionType": 2,
                 "SourceType": 1,
-            }
+            },
         ],
     }
     EU = {
         "locale": "en-IE",
         "LocationHint": [
             {
                 "country": "Norway",
@@ -149,15 +149,15 @@
                 "countryConfidence": 8,
                 "Center": {
                     "Latitude": 59.9139,
                     "Longitude": 10.7522,
                 },
                 "RegionType": 2,
                 "SourceType": 1,
-            }
+            },
         ],
     }
     UK = {
         "locale": "en-GB",
         "LocationHint": [
             {
                 "country": "United Kingdom",
@@ -172,29 +172,30 @@
                 "RegionType": 2,
                 "SourceType": 1,
             },
         ],
     }
 
 
-LOCATION_HINT_TYPES = Optional[Union[LocationHint, Literal["USA", "CHINA", "EU", "UK"]]]
+LOCATION_HINT_TYPES = Optional[LocationHint | Literal["USA", "CHINA", "EU", "UK"]]
 
 
 def get_location_hint_from_locale(locale: str) -> dict | None:
     locale = locale.lower()
     if locale == "en-us":
-        return LocationHint.USA.value
-    elif locale == "zh-cn":
-        return LocationHint.CHINA.value
-    elif locale == "en-gb":
-        return LocationHint.UK.value
-    elif locale == "en-ie":
-        return LocationHint.EU.value
+        hint = LocationHint.USA.value
+    if locale == "zh-cn":
+        hint = LocationHint.CHINA.value
+    if locale == "en-gb":
+        hint = LocationHint.UK.value
+    if locale == "en-ie":
+        hint = LocationHint.EU.value
     else:
-        return None
+        hint = LocationHint.USA.value
+    return hint.get("LocationHint")
 
 
 class ConversationStyle(Enum):
     creative = [
         "nlu_direct_response_filter",
         "deepleo",
         "disable_emoji_spoken_text",
@@ -245,38 +246,28 @@
         "clgalileo",
         "gencontentv3",
         "nojbfedge",
     ]
 
 
 CONVERSATION_STYLE_TYPE = Optional[
-    Union[ConversationStyle, Literal["creative", "balanced", "precise"]]
+    ConversationStyle | Literal["creative", "balanced", "precise"]
 ]
 
 
 def _append_identifier(msg: dict) -> str:
-    """
-    Appends special character to end of message to identify end of message
-    """
     # Convert dict to json string
     return json.dumps(msg, ensure_ascii=False) + DELIMITER
 
 
 def _get_ran_hex(length: int = 32) -> str:
-    """
-    Returns random hex string
-    """
     return "".join(random.choice("0123456789abcdef") for _ in range(length))
 
 
 class _ChatHubRequest:
-    """
-    Request object for ChatHub
-    """
-
     def __init__(
         self,
         conversation_signature: str,
         client_id: str,
         conversation_id: str,
         invocation_id: int = 0,
     ) -> None:
@@ -292,17 +283,14 @@
         prompt: str,
         conversation_style: CONVERSATION_STYLE_TYPE,
         options: list | None = None,
         webpage_context: str | None = None,
         search_result: bool = False,
         locale: str = "en-US",
     ) -> None:
-        """
-        Updates request object
-        """
         if options is None:
             options = [
                 "deepleo",
                 "enable_debug_commands",
                 "disable_emoji_spoken_text",
                 "enablemm",
             ]
@@ -388,18 +376,14 @@
                     "messageId": "discover-web--page-ping-mriduna-----",
                 },
             ]
         self.invocation_id += 1
 
 
 class _Conversation:
-    """
-    Conversation API
-    """
-
     def __init__(
         self,
         proxy: str | None = None,
         async_mode: bool = False,
         cookies: list[dict] | None = None,
     ) -> None:
         if async_mode:
@@ -511,18 +495,14 @@
             ) from exc
         if self.struct["result"]["value"] == "UnauthorizedRequest":
             raise NotAllowedToAccess(self.struct["result"]["message"])
         return self
 
 
 class _ChatHub:
-    """
-    Chat API
-    """
-
     def __init__(
         self,
         conversation: _Conversation,
         proxy: str = None,
         cookies: list[dict] | None = None,
     ) -> None:
         self.session: aiohttp.ClientSession | None = None
@@ -545,17 +525,14 @@
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         options: dict = None,
         webpage_context: str | None = None,
         search_result: bool = False,
         locale: str = "en-US",
     ) -> Generator[str, None, None]:
-        """
-        Ask a question to the bot
-        """
         timeout = aiohttp.ClientTimeout(total=900)
         self.session = aiohttp.ClientSession(timeout=timeout)
 
         if self.wss and not self.wss.closed:
             await self.wss.close()
         # Check if websocket is closed
         self.wss = await self.session.ws_connect(
@@ -632,15 +609,15 @@
                             == "GenerateContentQuery"
                         ):
                             async with ImageGenAsync("", True) as image_generator:
                                 images = await image_generator.get_images(
                                     response["arguments"][0]["messages"][0]["text"],
                                 )
                             for i, image in enumerate(images):
-                                resp_txt = resp_txt + f"\n![image{i}]({image})"
+                                resp_txt = f"{resp_txt}\n![image{i}]({image})"
                             draw = True
                         if (
                             response["arguments"][0]["messages"][0]["contentOrigin"]
                             != "Apology"
                         ) and not draw:
                             resp_txt = result_text + response["arguments"][0][
                                 "messages"
@@ -697,17 +674,14 @@
                     yield True, response
 
     async def _initial_handshake(self) -> None:
         await self.wss.send_str(_append_identifier({"protocol": "json", "version": 1}))
         await self.wss.receive(timeout=900)
 
     async def close(self) -> None:
-        """
-        Close the connection
-        """
         if self.wss and not self.wss.closed:
             await self.wss.close()
         if self.session and not self.session.closed:
             await self.session.close()
 
 
 class Chatbot:
@@ -727,36 +701,36 @@
             cookies=cookies,
         )
 
     @staticmethod
     async def create(
         proxy: str | None = None,
         cookies: list[dict] | None = None,
-    ):
+    ) -> Chatbot:
         self = Chatbot.__new__(Chatbot)
         self.proxy = proxy
         self.chat_hub = _ChatHub(
             await _Conversation.create(self.proxy, cookies=cookies),
             proxy=self.proxy,
             cookies=cookies,
         )
         return self
 
     async def save_conversation(self, filename: str) -> None:
         """
         Save the conversation to a file
         """
-        async with aiofiles.open(filename, "w") as f:
+        async with aiofiles.Path.open(filename, "w") as f:
             f.write(json.dumps(self.chat_hub.struct))
 
     async def load_conversation(self, filename: str) -> None:
         """
         Load the conversation from a file
         """
-        async with aiofiles.open(filename, "r") as f:
+        async with aiofiles.Path.open(filename, "r") as f:
             self.chat_hub.struct = json.loads(await f.read())
 
     async def ask(
         self,
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
@@ -840,36 +814,36 @@
     )
 
 
 def _create_session() -> PromptSession:
     kb = KeyBindings()
 
     @kb.add("enter")
-    def _(event):
+    def _(event) -> None:
         buffer_text = event.current_buffer.text
         if buffer_text.startswith("!"):
             event.current_buffer.validate_and_handle()
         else:
             event.current_buffer.insert_text("\n")
 
     @kb.add("escape")
-    def _(event):
+    def _(event) -> None:
         if event.current_buffer.complete_state:
             # event.current_buffer.cancel_completion()
             event.current_buffer.text = ""
 
     return PromptSession(key_bindings=kb, history=InMemoryHistory())
 
 
-def _create_completer(commands: list, pattern_str: str = "$"):
+def _create_completer(commands: list, pattern_str: str = "$") -> WordCompleter:
     return WordCompleter(words=commands, pattern=re.compile(pattern_str))
 
 
 def _create_history_logger(f):
-    def logger(*args, **kwargs):
+    def logger(*args, **kwargs) -> None:
         tmp = sys.stdout
         sys.stdout = f
         print(*args, **kwargs, flush=True)
         sys.stdout = tmp
 
     return logger
 
@@ -879,26 +853,26 @@
     Main function
     """
     print("Initializing...")
     print("Enter `alt+enter` or `escape+enter` to send a message")
     # Read and parse cookies
     cookies = None
     if args.cookie_file:
-        cookies = json.loads(open(args.cookie_file, encoding="utf-8").read())
+        cookies = json.loads(Path.open(args.cookie_file, encoding="utf-8").read())
     bot = await Chatbot.create(proxy=args.proxy, cookies=cookies)
     session = _create_session()
     completer = _create_completer(["!help", "!exit", "!reset"])
     initial_prompt = args.prompt
 
     # Log chat history
-    def p_hist(*args, **kwargs):
+    def p_hist(*args, **kwargs) -> None:
         pass
 
     if args.history_file:
-        f = open(args.history_file, "a+", encoding="utf-8")
+        f = Path.open(args.history_file, "a+", encoding="utf-8")
         p_hist = _create_history_logger(f)
 
     while True:
         print("\nYou:")
         p_hist("\nYou:")
         if initial_prompt:
             question = initial_prompt
@@ -1062,15 +1036,15 @@
     current_file_index = 0
     dirpath = Path("./").resolve()
     search_pattern = "bing_cookies_*.json"
     ignore_files = set()
     current_filepath: dict | None = None
 
     @classmethod
-    def fetch_default(cls, path=None):
+    def fetch_default(cls, path: Path | None = None) -> None:
         from selenium import webdriver
         from selenium.webdriver.common.by import By
 
         driver = webdriver.Edge()
         driver.get("https://bing.com/chat")
         time.sleep(5)
         xpath = '//button[@id="bnp_btn_accept"]'
@@ -1084,21 +1058,21 @@
         cookies = driver.get_cookies()
         Path(path).write_text(json.dumps(cookies, indent=4), encoding="utf-8")
         # Path again in case supplied path is: str
         print(f"Cookies saved to: {path}")
         driver.quit()
 
     @classmethod
-    def files(cls):
+    def files(cls) -> list[Path]:
         """Return a sorted list of all cookie files matching .search_pattern"""
         all_files = set(cls.dirpath.glob(cls.search_pattern))
-        return sorted(list(all_files - cls.ignore_files))
+        return sorted(all_files - cls.ignore_files)
 
     @classmethod
-    def import_data(cls):
+    def import_data(cls) -> None:
         """
         Read the active cookie file and populate the following attributes:
 
           .current_filepath
           .current_data
           .image_token
         """
@@ -1106,21 +1080,21 @@
             cls.current_filepath = cls.files()[cls.current_file_index]
         except IndexError as exc:
             print(
                 "> Please set Cookie.current_filepath to a valid cookie file, then run Cookie.import_data()",
             )
             raise "No valid cookie file found." from exc
         print(f"> Importing cookies from: {cls.current_filepath.name}")
-        with open(cls.current_filepath, encoding="utf-8") as file:
+        with Path.open(cls.current_filepath, encoding="utf-8") as file:
             cls.current_data = json.load(file)
         cls.image_token = [x for x in cls.current_data if x.get("name") == "_U"]
         cls.image_token = cls.image_token[0].get("value")
 
     @classmethod
-    def import_next(cls):
+    def import_next(cls) -> None:
         """
         Cycle through to the next cookies file.  Import it.  Mark the previous
         file to be ignored for the remainder of the current session.
         """
         cls.ignore_files.add(cls.current_filepath)
         if Cookie.current_file_index >= len(cls.files()):
             Cookie.current_file_index = 0
@@ -1131,22 +1105,22 @@
     """
     A convenience class that wraps around EdgeGPT.Chatbot to encapsulate input,
     config, and output all together.  Relies on Cookie class for authentication
     """
 
     def __init__(
         self,
-        prompt,
-        style="precise",
-        content_type="text",
-        cookie_file=0,
-        echo=True,
-        echo_prompt=False,
+        prompt: str,
+        style: str = "precise",
+        content_type: str = "text",
+        cookie_file: int = 0,
+        echo: bool = True,
+        echo_prompt: bool = False,
         proxy: str | None = None,
-    ):
+    ) -> None:
         """
         Arguments:
 
         prompt: Text to enter into Bing Chat
         style: creative, balanced, or precise
         content_type: "text" for Bing Chat; "image" for Dall-e
         cookie_file: Path, filepath string, or index (int) to list of cookie paths
@@ -1160,15 +1134,15 @@
         Cookie.import_data()
         self.index += [self]
         self.prompt = prompt
         files = Cookie.files()
         if isinstance(cookie_file, int):
             index = cookie_file if cookie_file < len(files) else 0
         else:
-            if not isinstance(cookie_file, (str, Path)):
+            if not isinstance(cookie_file, str | Path):
                 message = "'cookie_file' must be an int, str, or Path object"
                 raise TypeError(message)
             cookie_file = Path(cookie_file)
             if cookie_file in files:  # Supplied filepath IS in Cookie.dirpath
                 index = files.index(cookie_file)
             else:  # Supplied filepath is NOT in Cookie.dirpath
                 if cookie_file.is_file():
@@ -1179,115 +1153,116 @@
         Cookie.current_file_index = index
         if content_type == "text":
             self.style = style
             self.log_and_send_query(echo, echo_prompt)
         if content_type == "image":
             self.create_image()
 
-    def log_and_send_query(self, echo, echo_prompt):
+    def log_and_send_query(self, echo: bool, echo_prompt: bool) -> None:
         self.response = asyncio.run(self.send_to_bing(echo, echo_prompt))
         name = str(Cookie.current_filepath.name)
         if not self.request_count.get(name):
             self.request_count[name] = 1
         else:
             self.request_count[name] += 1
 
-    def create_image(self):
+    def create_image(self) -> None:
         image_generator = ImageGen(Cookie.image_token)
         image_generator.save_images(
             image_generator.get_images(self.prompt),
             output_dir=self.image_dirpath,
         )
 
-    async def send_to_bing(self, echo=True, echo_prompt=False):
+    async def send_to_bing(self, echo: bool = True, echo_prompt: bool = False) -> str:
         """Creat, submit, then close a Chatbot instance.  Return the response"""
         retries = len(Cookie.files())
         while retries:
             try:
                 # Read the cookies file
                 bot = await Chatbot.create(
-                    proxy=self.proxy, cookies=Cookie.current_data
+                    proxy=self.proxy,
+                    cookies=Cookie.current_data,
                 )
                 if echo_prompt:
                     print(f"> {self.prompt}=")
                 if echo:
                     print("> Waiting for response...")
                 if self.style.lower() not in "creative balanced precise".split():
                     self.style = "precise"
-                response = await bot.ask(
+                return await bot.ask(
                     prompt=self.prompt,
                     conversation_style=getattr(ConversationStyle, self.style),
                     # wss_link="wss://sydney.bing.com/sydney/ChatHub"
                     # What other values can this parameter take? It seems to be optional
                 )
-                return response
             except KeyError:
                 print(
                     f"> KeyError [{Cookie.current_filepath.name} may have exceeded the daily limit]",
                 )
                 Cookie.import_next()
                 retries -= 1
             finally:
                 await bot.close()
+        return None
 
     @property
-    def output(self):
+    def output(self) -> str:
         """The response from a completed Chatbot request"""
         return self.response["item"]["messages"][1]["text"]
 
     @property
-    def sources(self):
+    def sources(self) -> str:
         """The source names and details parsed from a completed Chatbot request"""
         return self.response["item"]["messages"][1]["sourceAttributions"]
 
     @property
-    def sources_dict(self):
+    def sources_dict(self) -> dict[str, str]:
         """The source names and details as a dictionary"""
         sources_dict = {}
         name = "providerDisplayName"
         url = "seeMoreUrl"
         for source in self.sources:
-            if name in source.keys() and url in source.keys():
+            if name in source and url in source:
                 sources_dict[source[name]] = source[url]
             else:
                 continue
         return sources_dict
 
     @property
-    def code(self):
+    def code(self) -> str:
         """Extract and join any snippets of Python code in the response"""
         code_blocks = self.output.split("```")[1:-1:2]
         code_blocks = ["\n".join(x.splitlines()[1:]) for x in code_blocks]
         return "\n\n".join(code_blocks)
 
     @property
-    def languages(self):
+    def languages(self) -> set[str]:
         """Extract all programming languages given in code blocks"""
         code_blocks = self.output.split("```")[1:-1:2]
         return {x.splitlines()[0] for x in code_blocks}
 
     @property
-    def suggestions(self):
+    def suggestions(self) -> list[str]:
         """Follow-on questions suggested by the Chatbot"""
         return [
             x["text"]
             for x in self.response["item"]["messages"][1]["suggestedResponses"]
         ]
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<EdgeGPT.Query: {self.prompt}>"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.output
 
 
 class ImageQuery(Query):
-    def __init__(self, prompt, **kwargs):
-        kwargs.update({"content_type": "image"})
+    def __init__(self, prompt: str, **kwargs) -> None:
+        kwargs["content_type"] = "image"
         super().__init__(prompt, **kwargs)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<EdgeGPT.ImageQuery: {self.prompt}>"
 
 
 if __name__ == "__main__":
     main()
```

