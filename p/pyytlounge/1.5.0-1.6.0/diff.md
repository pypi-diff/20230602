# Comparing `tmp/pyytlounge-1.5.0.tar.gz` & `tmp/pyytlounge-1.6.0.tar.gz`

## Comparing `pyytlounge-1.5.0.tar` & `pyytlounge-1.6.0.tar`

### file list

```diff
@@ -1,23 +1,19 @@
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/test.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/variables_example.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.pytest_cache/README.md
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.vscode/launch.json
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/src/pyytlounge/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/src/pyytlounge/api.py
--rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/src/pyytlounge/manual_pairing.py
--rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/src/pyytlounge/wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/tests/__init__.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/tests/conftest.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/tests/devices.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/tests/test_process_event.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/LICENSE
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/README.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/test.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/variables_example.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/.vscode/launch.json
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/src/pyytlounge/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/src/pyytlounge/api.py
+-rwxr-xr-x   0        0        0     1040 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/src/pyytlounge/manual_pairing.py
+-rw-r--r--   0        0        0    18847 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/src/pyytlounge/wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/tests/devices.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/tests/test_process_event.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/LICENSE
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/README.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pyytlounge-1.6.0/PKG-INFO
```

### Comparing `pyytlounge-1.5.0/test.py` & `pyytlounge-1.6.0/test.py`

 * *Files identical despite different names*

### Comparing `pyytlounge-1.5.0/src/pyytlounge/manual_pairing.py` & `pyytlounge-1.6.0/src/pyytlounge/manual_pairing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 #!/usr/bin/env python
 
-import requests
+import asyncio
+import aiohttp
 from api import api_base
-
+async def get_screen(pairing_code):
+    async with aiohttp.ClientSession() as session:
+        async with session.post(f"{api_base}/pairing/get_screen", data={'pairing_code': pairing_code}) as response:
+            return await response.json()
 pairing_code = input("Enter manual pairing code as shown in YouTube app on target: ")
 try:
     pairing_code = int(pairing_code)
 except Exception as ex:
     print(f"Invalid pairing code {pairing_code}", ex)
 
 # initial paring with code
-res = requests.post(f"{api_base}/pairing/get_screen", data={'pairing_code': pairing_code})
-screens = res.json()
+loop = asyncio.get_event_loop()
+
+screens = loop.run_until_complete(get_screen(pairing_code))
 screen = screens["screen"]
 screen_name = screen["name"]
 screen_id = screen["screenId"]
 lounge_token = screen["loungeToken"]
 
 print(f"Found \"{screen_name}\" with id: '{screen_id}' token: '{lounge_token}'")
```

### Comparing `pyytlounge-1.5.0/src/pyytlounge/wrapper.py` & `pyytlounge-1.6.0/src/pyytlounge/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Wrapper class for YouTube Lounge API"""
 
 import json
 import logging
 from enum import Enum
 from typing import Any, AsyncIterator, List, TypedDict, Union, Callable
+from dataclasses import dataclass
 
 import aiohttp
-from aiohttp import ClientTimeout
-from requests.models import PreparedRequest
+from aiohttp import ClientTimeout, StreamReader
 
 from .api import api_base
 
 
 class State(Enum):
+    """Playback state"""
+
     Stopped = -1
     Buffering = 0  # unsure, happens between videos
     Playing = 1
     Paused = 2
     Starting = 3  # unsure, only seen once
     Advertisement = 1081
 
@@ -77,28 +79,39 @@
     version: int
     screenId: str
     loungeIdToken: str
     refreshToken: str
     expiry: int
 
 
+@dataclass
 class AuthState:
+    """Stores information used to authenticate with YouTube.
+    Can be serialized and deserialized for reuse."""
+
     version: int
     screen_id: str
     lounge_id_token: str
     refresh_token: str
     expiry: int
 
     def __init__(self):
+        super().__init__()
         self.version = CURRENT_AUTH_VERSION
+        self.screen_id = None
+        self.lounge_id_token = None
+        self.refresh_token = None
+        self.expiry = None
 
     def serialize(self) -> AuthStateData:
+        """Serializes the current state into a dictionary."""
         return vars(self)
 
     def deserialize(self, data: AuthStateData):
+        """Deserializes state from a dictionary into this object."""
         if data["version"] == CURRENT_AUTH_VERSION:
             for key in data:
                 setattr(self, key, data[key])
 
 
 class __DeviceInfo(TypedDict):
     brand: str
@@ -113,20 +126,22 @@
     deviceInfo: str  # json string
 
 
 class __LoungeStatus(TypedDict):
     devices: str  # json string containing list of __Device
 
 
-async def desync(it):
-    for x in it:
-        yield x
+async def desync(iterator):
+    """Turns a synchronous iterator into an asynchronous iterator"""
+    for item in iterator:
+        yield item
 
 
-async def iter_response_lines(resp):
+async def iter_response_lines(resp: StreamReader):
+    """Enumerate lines in response one at a time."""
     while True:
         line = await resp.readline()
         if line:
             yield line.decode()
         else:
             break
 
@@ -263,15 +278,15 @@
             self._update_state()
         elif event_type == "loungeStatus":
             data: __LoungeStatus = args[0]
             devices: List[__Device] = json.loads(data["devices"])
             for device in devices:
                 if device["type"] == "LOUNGE_SCREEN":
                     self._screen_name = device["name"]
-                    self._device_info = json.loads(device["deviceInfo"])
+                    self._device_info = json.loads(device.get("deviceInfo", "null"))
                     break
         elif event_type == "loungeScreenDisconnected":
             self.state = PlaybackState(self._logger)
             self._update_state()
             self._connection_lost()
         elif event_type == "noop":
             pass  # no-op
@@ -401,20 +416,19 @@
             "RID": "rpc",
             "SID": self._sid,
             "CI": "0",
             "AID": self._last_event_id,
             "gsessionid": self._gsession,
             "TYPE": "xmlhttp",
         }
-        req = PreparedRequest()
-        req.prepare_url(f"{api_base}/bc/bind", params)
+        url = f"{api_base}/bc/bind"
         self._logger.info("Subscribing to lounge id %s", self.auth.lounge_id_token)
         try:
             async with aiohttp.ClientSession(timeout=ClientTimeout()) as session:
-                async with session.get(req.url) as resp:
+                async with session.get(url=url, params=params) as resp:
                     if not self._handle_session_result(resp.status, resp.reason):
                         return
 
                     async for events in self._parse_event_chunks(
                         iter_response_lines(resp.content)
                     ):
                         pre_state_update = self.state_update
@@ -426,14 +440,51 @@
                     self._logger.info(
                         "Subscribe completed, status %i %s", resp.status, resp.reason
                     )
 
         except Exception as ex:
             self._logger.exception(ex)
 
+    async def disconnect(self) -> bool:
+        """Disconnect from the current session"""
+        if not self.connected():
+            raise Exception("Not connected")
+
+        command_body = {
+            "ui": "",
+            "TYPE": "terminate",
+            "clientDisconnectReason": "MDX_SESSION_DISCONNECT_REASON_DISCONNECTED_BY_USER",
+        }
+        params = {
+            "device": "REMOTE_CONTROL",
+            "name": self.device_name,
+            "app": "youtube-desktop",
+            "loungeIdToken": self.auth.lounge_id_token,
+            "VER": "8",
+            "v": "2",
+            "CVER": "1",
+            "RID": self._command_offset,
+            "SID": self._sid,
+            "AID": self._last_event_id,
+            "gsessionid": self._gsession,
+            "auth_failure_option": "send_error",
+        }
+        url = f"{api_base}/bc/bind"
+        async with aiohttp.ClientSession() as session:
+            async with session.post(url=url, data=command_body, params=params) as resp:
+                try:
+                    response_text = await resp.text()
+                    if not self._handle_session_result(resp.status, response_text):
+                        return False
+                    resp.raise_for_status()
+                    return True
+                except Exception as ex:
+                    self._logger.exception(ex)
+                    return False
+
     async def _command(self, command: str, command_parameters: dict = None) -> bool:
         if not self.connected():
             raise Exception("Not connected")
 
         command_body = {"count": 1, "ofs": self._command_offset, "req0__sc": command}
         if command_parameters:
             for cmd_param in command_parameters:
@@ -449,18 +500,17 @@
             "VER": "8",
             "v": "2",
             "RID": self._command_offset,
             "SID": self._sid,
             "AID": self._last_event_id,
             "gsessionid": self._gsession,
         }
-        req = PreparedRequest()
-        req.prepare_url(f"{api_base}/bc/bind", params)
+        url = f"{api_base}/bc/bind"
         async with aiohttp.ClientSession() as session:
-            async with session.post(url=req.url, data=command_body) as resp:
+            async with session.post(url=url, data=command_body, params=params) as resp:
                 try:
                     response_text = await resp.text()
                     if not self._handle_session_result(resp.status, response_text):
                         return False
                     resp.raise_for_status()
                     return True
                 except Exception as ex:
@@ -482,7 +532,15 @@
     async def next(self) -> bool:
         """Sends next command to screen"""
         return await self._command("next")
 
     async def seek_to(self, time: float) -> bool:
         """Seek to given time (seconds)"""
         return await self._command("seekTo", {"newTime": time})
+
+    async def skip_ad(self) -> bool:
+        """Skips ad if possible"""
+        return await self._command("skipAd")
+
+    async def set_volume(self, volume: int) -> bool:
+        """Sets volume to given value (0-100)"""
+        return await self._command("setVolume", {"volume": volume})
```

### Comparing `pyytlounge-1.5.0/tests/devices.py` & `pyytlounge-1.6.0/tests/devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypedDict
+from typing import TypedDict, Dict
 from dataclasses import dataclass
 
 
 class DeviceData(TypedDict):
     loungeStatus: str
 
 
@@ -14,15 +14,15 @@
 
 @dataclass
 class Device:
     data: DeviceData
     expectations: DeviceExpectations
 
 
-devices: dict[str, Device] = {
+devices: Dict[str, Device] = {
     "LG OLED55C7V": Device(
         {
             "loungeStatus": {
                 "devices": """[
                 {
                     "app": "lb-v4",
                     "capabilities": "dsp,mic,dpa,ntb,que,mus",
```

### Comparing `pyytlounge-1.5.0/LICENSE` & `pyytlounge-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyytlounge-1.5.0/pyproject.toml` & `pyytlounge-1.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [project]
 name = "pyytlounge"
-version = "1.5.0"
+version = "1.6.0"
 authors = [
   { name="Fabio", email="example@example.com" },
 ]
 description = "YouTube Lounge API wrapper"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  'requests==2.28.1',
-  'aiohttp==3.8.1',
+  'aiohttp==3.8.4',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/FabioGNR/pyytlounge"
 "Bug Tracker" = "https://github.com/FabioGNR/pyytlounge/issues"
 
 [project.optional-dependencies]
```

