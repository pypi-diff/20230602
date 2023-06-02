# Comparing `tmp/slixmppbot-2.0.2.tar.gz` & `tmp/slixmppbot-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slixmppbot-2.0.2.tar", max compression
+gzip compressed data, was "slixmppbot-2.0.3.tar", max compression
```

## Comparing `slixmppbot-2.0.2.tar` & `slixmppbot-2.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35141 2017-03-12 18:31:56.511032 slixmppbot-2.0.2/LICENSE
--rw-r--r--   0        0        0      504 2023-04-16 12:03:40.742358 slixmppbot-2.0.2/README.md
--rw-r--r--   0        0        0      787 2023-06-02 15:24:40.749124 slixmppbot-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      159 2023-04-21 18:59:01.852273 slixmppbot-2.0.2/xmppbot/__init__.py
--rw-r--r--   0        0        0     2205 2023-04-16 20:28:02.630945 slixmppbot-2.0.2/xmppbot/basebot.py
--rw-r--r--   0        0        0     4673 2023-04-21 19:00:23.604358 slixmppbot-2.0.2/xmppbot/cmdbot.py
--rw-r--r--   0        0        0      294 2023-04-16 15:21:14.665631 slixmppbot-2.0.2/xmppbot/common.py
--rw-r--r--   0        0        0     3920 2023-04-21 18:10:16.326969 slixmppbot-2.0.2/xmppbot/configbot.py
--rw-r--r--   0        0        0      475 2023-04-16 20:28:02.406945 slixmppbot-2.0.2/xmppbot/timeout.py
--rw-r--r--   0        0        0     7691 2023-04-16 21:15:04.149936 slixmppbot-2.0.2/xmppbot/xmppbot.py
--rw-r--r--   0        0        0     2350 2023-04-14 18:07:41.498686 slixmppbot-2.0.2/xmppbot/xmppmsg.py
--rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 slixmppbot-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35141 2017-03-12 18:31:56.511032 slixmppbot-2.0.3/LICENSE
+-rw-r--r--   0        0        0      504 2023-06-02 15:29:47.872743 slixmppbot-2.0.3/README.md
+-rw-r--r--   0        0        0      787 2023-06-02 16:28:51.941340 slixmppbot-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      159 2023-06-02 15:29:47.884743 slixmppbot-2.0.3/xmppbot/__init__.py
+-rw-r--r--   0        0        0     2205 2023-06-02 15:29:47.884743 slixmppbot-2.0.3/xmppbot/basebot.py
+-rw-r--r--   0        0        0     4673 2023-06-02 15:29:47.884743 slixmppbot-2.0.3/xmppbot/cmdbot.py
+-rw-r--r--   0        0        0      294 2023-06-02 15:29:47.884743 slixmppbot-2.0.3/xmppbot/common.py
+-rw-r--r--   0        0        0     3920 2023-06-02 15:46:26.508820 slixmppbot-2.0.3/xmppbot/configbot.py
+-rw-r--r--   0        0        0      475 2023-06-02 15:29:47.888743 slixmppbot-2.0.3/xmppbot/timeout.py
+-rw-r--r--   0        0        0     7691 2023-06-02 15:46:01.156829 slixmppbot-2.0.3/xmppbot/xmppbot.py
+-rw-r--r--   0        0        0     2730 2023-06-02 16:28:09.277379 slixmppbot-2.0.3/xmppbot/xmppmsg.py
+-rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 slixmppbot-2.0.3/PKG-INFO
```

### Comparing `slixmppbot-2.0.2/LICENSE` & `slixmppbot-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slixmppbot-2.0.2/pyproject.toml` & `slixmppbot-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slixmppbot"
-version = "2.0.2"
+version = "2.0.3"
 description = "A framework for writing Jabber/XMPP bots"
 authors = ["s-nt-s <santos82h@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 include = ["LICENSE"]
 homepage = "https://github.com/s-nt-s/XmppBot"
 keywords = ["xmpp", "bot"]
```

### Comparing `slixmppbot-2.0.2/xmppbot/basebot.py` & `slixmppbot-2.0.3/xmppbot/basebot.py`

 * *Files identical despite different names*

### Comparing `slixmppbot-2.0.2/xmppbot/cmdbot.py` & `slixmppbot-2.0.3/xmppbot/cmdbot.py`

 * *Files identical despite different names*

### Comparing `slixmppbot-2.0.2/xmppbot/configbot.py` & `slixmppbot-2.0.3/xmppbot/configbot.py`

 * *Files identical despite different names*

### Comparing `slixmppbot-2.0.2/xmppbot/xmppbot.py` & `slixmppbot-2.0.3/xmppbot/xmppbot.py`

 * *Files identical despite different names*

### Comparing `slixmppbot-2.0.2/xmppbot/xmppmsg.py` & `slixmppbot-2.0.3/xmppbot/xmppmsg.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,34 @@
 from .basebot import BaseBot
 from .timeout import timeout
 
 
 class SendMsgBot(BaseBot):
     def __init__(self, config_path):
         super().__init__(config_path)
+        if self.config.rooms:
+            self.register_plugin('xep_0045')  # Multi-User Chat
         self.messages = []
         self.add_event_handler("session_start", self.start)
 
     async def start(self, event):
+        await self.get_roster()
         self.send_presence()
-        self.get_roster()
+        rooms = set(self.config.rooms).intersection(tm[0] for tm in self.messages)
+
+        for room in rooms:
+            await self.xep_0045.join_muc(room, self.config.user.split("@")[0])
         while self.messages:
             to, msg = self.messages.pop(0)
+            mtype = 'chat'
+            if to in rooms:
+                mtype = 'groupchat'
             self.send_message(mto=to,
                               mbody=msg,
-                              mtype='chat')
+                              mtype=mtype)
             time.sleep(0.1)
         self.disconnect()
 
     def run(self):
         if not self.messages:
             return
         with timeout(seconds=10):
```

### Comparing `slixmppbot-2.0.2/PKG-INFO` & `slixmppbot-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slixmppbot
-Version: 2.0.2
+Version: 2.0.3
 Summary: A framework for writing Jabber/XMPP bots
 Home-page: https://github.com/s-nt-s/XmppBot
 License: GPLv3
 Keywords: xmpp,bot
 Author: s-nt-s
 Author-email: santos82h@gmail.com
 Requires-Python: >=3.9,<4.0
```

