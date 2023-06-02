# Comparing `tmp/slixmppbot-1.0.8.tar.gz` & `tmp/slixmppbot-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slixmppbot-1.0.8.tar", last modified: Wed Jan 18 21:07:35 2023, max compression
+gzip compressed data, was "slixmppbot-2.0.2.tar", max compression
```

## Comparing `slixmppbot-1.0.8.tar` & `slixmppbot-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,12 @@
-drwxrwxr-x   0 santos    (1000) santos    (1000)        0 2023-01-18 21:07:35.000000 slixmppbot-1.0.8/
--rw-r--r--   0 santos    (1000) santos    (1000)    35141 2017-03-12 18:31:56.000000 slixmppbot-1.0.8/LICENSE
--rw-rw-r--   0 santos    (1000) santos    (1000)     1291 2023-01-18 21:07:35.000000 slixmppbot-1.0.8/PKG-INFO
--rw-rw-r--   0 santos    (1000) santos    (1000)      609 2021-01-25 20:47:38.000000 slixmppbot-1.0.8/README.md
--rw-rw-r--   0 santos    (1000) santos    (1000)      103 2023-01-18 21:07:35.000000 slixmppbot-1.0.8/setup.cfg
--rw-rw-r--   0 santos    (1000) santos    (1000)     1104 2023-01-18 21:07:28.000000 slixmppbot-1.0.8/setup.py
-drwxrwxr-x   0 santos    (1000) santos    (1000)        0 2023-01-18 21:07:35.000000 slixmppbot-1.0.8/slixmppbot.egg-info/
--rw-rw-r--   0 santos    (1000) santos    (1000)       70 2023-01-18 21:07:35.000000 slixmppbot-1.0.8/slixmppbot.egg-info/requires.txt
--rw-rw-r--   0 santos    (1000) santos    (1000)        8 2023-01-18 21:07:35.000000 slixmppbot-1.0.8/slixmppbot.egg-info/top_level.txt
--rw-rw-r--   0 santos    (1000) santos    (1000)      319 2023-01-18 21:07:35.000000 slixmppbot-1.0.8/slixmppbot.egg-info/SOURCES.txt
--rw-rw-r--   0 santos    (1000) santos    (1000)     1291 2023-01-18 21:07:35.000000 slixmppbot-1.0.8/slixmppbot.egg-info/PKG-INFO
--rw-rw-r--   0 santos    (1000) santos    (1000)        1 2023-01-18 21:07:35.000000 slixmppbot-1.0.8/slixmppbot.egg-info/dependency_links.txt
-drwxrwxr-x   0 santos    (1000) santos    (1000)        0 2023-01-18 21:07:35.000000 slixmppbot-1.0.8/xmppbot/
--rw-rw-r--   0 santos    (1000) santos    (1000)     9060 2023-01-18 18:34:39.000000 slixmppbot-1.0.8/xmppbot/xmppbot.py
--rw-rw-r--   0 santos    (1000) santos    (1000)     2580 2023-01-18 18:56:33.000000 slixmppbot-1.0.8/xmppbot/common.py
--rw-rw-r--   0 santos    (1000) santos    (1000)       66 2021-01-25 18:32:22.000000 slixmppbot-1.0.8/xmppbot/__init__.py
--rw-rw-r--   0 santos    (1000) santos    (1000)      762 2023-01-18 18:56:33.000000 slixmppbot-1.0.8/xmppbot/basebot.py
--rw-rw-r--   0 santos    (1000) santos    (1000)     3093 2023-01-18 19:00:57.000000 slixmppbot-1.0.8/xmppbot/xmppmsg.py
--rw-rw-r--   0 santos    (1000) santos    (1000)      461 2023-01-18 19:00:03.000000 slixmppbot-1.0.8/xmppbot/timeout.py
+-rw-r--r--   0        0        0    35141 2017-03-12 18:31:56.511032 slixmppbot-2.0.2/LICENSE
+-rw-r--r--   0        0        0      504 2023-04-16 12:03:40.742358 slixmppbot-2.0.2/README.md
+-rw-r--r--   0        0        0      787 2023-06-02 15:24:40.749124 slixmppbot-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      159 2023-04-21 18:59:01.852273 slixmppbot-2.0.2/xmppbot/__init__.py
+-rw-r--r--   0        0        0     2205 2023-04-16 20:28:02.630945 slixmppbot-2.0.2/xmppbot/basebot.py
+-rw-r--r--   0        0        0     4673 2023-04-21 19:00:23.604358 slixmppbot-2.0.2/xmppbot/cmdbot.py
+-rw-r--r--   0        0        0      294 2023-04-16 15:21:14.665631 slixmppbot-2.0.2/xmppbot/common.py
+-rw-r--r--   0        0        0     3920 2023-04-21 18:10:16.326969 slixmppbot-2.0.2/xmppbot/configbot.py
+-rw-r--r--   0        0        0      475 2023-04-16 20:28:02.406945 slixmppbot-2.0.2/xmppbot/timeout.py
+-rw-r--r--   0        0        0     7691 2023-04-16 21:15:04.149936 slixmppbot-2.0.2/xmppbot/xmppbot.py
+-rw-r--r--   0        0        0     2350 2023-04-14 18:07:41.498686 slixmppbot-2.0.2/xmppbot/xmppmsg.py
+-rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 slixmppbot-2.0.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `slixmppbot-1.0.8/LICENSE` & `slixmppbot-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slixmppbot-1.0.8/xmppbot/xmppbot.py` & `slixmppbot-2.0.2/xmppbot/xmppbot.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,235 +18,219 @@
 A framework for writing Jabber/XMPP bots.
 The XmppBot framework allows you to easily write bots
 that use the XMPP protocol. You can create commands by
 decorating functions in your subclass or customize the
 bot's operation completely.
 """
 
-import inspect
-import os
+import logging
 import re
+from functools import cached_property
+from slixmpp.exceptions import XMPPError
+import traceback
 
-from .basebot import BaseBot
-
-sp = re.compile(r"\s+", re.MULTILINE | re.UNICODE)
-url_img = re.compile(r"(https?://\S+\.(gif|png|jpe?g)\S*)", re.IGNORECASE)
-creator_order = 0
+from .cmdbot import CmdBot
+from .basebot import BaseBot, Message
 
+logger = logging.getLogger(__name__)
 
-def botcmd(*args, **kwargs):
-    """Decorator for bot command functions"""
-    global creator_order
-
-    def decorate(func, creator_order, name=None, names=None, delay=False, fromuser=None, regex=None, rg_mode="match"):
-        setattr(func, '_command', True)
-        setattr(func, '_command_names', names or [name or func.__name__])
-        setattr(func, '_command_delay', delay)
-        setattr(func, '_command_fromuser', fromuser)
-        setattr(func, '_command_regex', regex)
-        setattr(func, '_command_rg_mode', rg_mode)
-        setattr(func, '_command_order', creator_order)
-        return func
-
-    creator_order += 1
-
-    if len(args):
-        return decorate(args[0], creator_order, **kwargs)
-    else:
-        return lambda func: decorate(func, creator_order, **kwargs)
+re_sp = re.compile(r"\s+", re.MULTILINE | re.UNICODE)
+url_img = re.compile(r"(https?://\S+\.(gif|png|jpe?g)\S*)", re.IGNORECASE)
 
 
 class XmppBot(BaseBot):
     MSG_ERROR_OCCURRED = "ERROR!!"
 
     def __init__(self, config_path):
         super().__init__(config_path)
-        self.use_ipv6 = self.config.get("use_ipv6", True)
-        self.delay = False
-        self.commands = []
-        plugins = set(self.config.get("plugins", "").split())
-
-        commands = inspect.getmembers(self, inspect.ismethod)
-        commands = filter(lambda x: getattr(x[1], '_command', False), commands)
-        commands = sorted(
-            commands, key=lambda x: getattr(x[1], '_command_order'))
-
-        for name, value in commands:
-            names = getattr(value, '_command_names')
-            order = getattr(value, '_command_order', 0)
-            self.log.info('Registered %dº command: %s' %
-                          (order, " ".join(names)))
-            self.commands.append(value)
-            self.delay = self.delay or getattr(value, '_command_delay', False)
+        self.commands = self.__get_commands()
+        self.__validate()
 
-        self.nick = self.config['user'].split("@")[0]
+        self.nick = self.config.user.split("@")[0]
 
         self.auto_reconnect = True
-        if self.config.get("auto", False):
+        if self.config.friendly:
             self.auto_authorize = True
             self.auto_subscribe = True
 
-        plugins.add('xep_0030')  # Service Discovery
-        plugins.add('xep_0004')  # Data Forms
-        plugins.add('xep_0060')  # PubSub
-        plugins.add('xep_0199')  # XMPP Ping
-        if self.delay:
-            plugins.add('xep_0203')  # XMPP Delayed messages
-        if self.config.get('vcard', None):
-            plugins.add('xep_0054')
-        if self.config.get('avatar', None):
-            if os.path.isfile(self.config['avatar']):
-                plugins.add('xep_0084')
-                plugins.add('xep_0153')
-            else:
-                del self.config['avatar']
-
-        if self.config.get('rooms', None):
-            plugins.add('xep_0045')  # Multi-User Chat
+        if 'xep_0203' not in self.config.plugins and self.allow_delay:
+            # XMPP Delayed messages
+            self.config.plugins = self.config.plugins + ('xep_0203', )
 
-        if self.config.get('img_to_oob', False):
-            plugins.add('xep_0066')  # OOB
-
-        for plugin in plugins:
+        for plugin in self.config.plugins:
             self.register_plugin(plugin)
 
         self.add_event_handler("session_start", self.start)
         self.add_event_handler("message", self.read_message)
         self.add_event_handler("groupchat_subject", self.groupchat_subject)
 
-        self.custom_roster = self.config.get('roster')
+    def __get_commands(self):
+        commands: list[CmdBot] = []
+        for k, v in self.__class__.__dict__.items():
+            cmd = getattr(v, 'cmd', None)
+            if isinstance(cmd, CmdBot):
+                func = getattr(self, k, None)
+                if func is not None:
+                    cmd = getattr(func, 'cmd', None)
+                    cmd.func = func
+                    commands.append(cmd)
+        commands = sorted(commands, key=lambda x: x.index)
+        for c in commands:
+            logger.info(f'Registered {c.index}º command: ' + " ".join(c.names))
+        return tuple(commands)
+
+    def __validate(self):
+        if not self.config.lisent:
+            raise Exception("This bot need lisent != None")
+        if not self.commands:
+            raise Exception("This bot need commands")
 
-        if not self.config.get('lisent'):
-            self.config['lisent'] = ['chat', 'normal']
-            if self.config.get('rooms', None):
-                self.config['lisent'].append('groupchat')
+    @cached_property
+    def allow_delay(self) -> bool:
+        for c in self.commands:
+            if c.delay is True:
+                return True
+        return False
 
-    def start(self, event):
+    async def start(self, event):
         self.send_presence()
-        self.get_roster()
-        if self.config.get('vcard', None):
-            vcard = self['xep_0054'].stanza.VCardTemp()
-            vcard['JABBERID'] = self.boundjid.bare
-            for f in self.config['vcard']:
-                vcard[f] = self.config['vcard'][f]
-                if f.upper() == 'NICKNAME':
-                    self.nick = self.config['vcard'][f]
-            self['xep_0054'].publish_vcard(vcard)
-        if self.config.get('avatar', None):
-            avatar_data = None
-            try:
-                with open(self.config['avatar'], 'rb') as avatar_file:
-                    avatar_data = avatar_file.read()
-            except IOError:
-                self.log.debug('Could not load avatar')
-            if avatar_data:
-                ext = os.path.splitext(self.config['avatar'])[1][1:]
-                mtype = 'image/' + ext
-                avatar_id = self['xep_0084'].generate_id(avatar_data)
-                info = {
-                    'id': avatar_id,
-                    'type': mtype,
-                    'bytes': len(avatar_data)
-                }
-                self['xep_0084'].publish_avatar(avatar_data)
-                self['xep_0084'].publish_avatar_metadata(items=[info])
-                self['xep_0153'].set_avatar(avatar=avatar_data, mtype=mtype)
-
-        for room in self.config.get('rooms', []):
-            self.plugin['xep_0045'].joinMUC(room,
-                                            self.nick,
-                                            wait=True)
+        await self.get_roster()
+        await self.__set_vcard()
+        await self.__set_avatar()
+        self.__join_rooms()
+
+    async def __set_vcard(self):
+        if self.config.vcard is None:
+            return
+        vcard = self.xep_0054.stanza.VCardTemp()
+        vcard['JABBERID'] = self.boundjid.bare
+        for k, v in self.config.vcard.items():
+            vcard[k] = v
+            if k.upper() == 'NICKNAME':
+                self.nick = v
+        await self.xep_0054.publish_vcard(vcard)
+
+    async def __set_avatar(self):
+        if self.config.avatar is None:
+            return
+        avatar = self.config.avatar
+        avatar_metadata = {
+            'id': self.xep_0084.generate_id(avatar.content),
+            'type': avatar.mtype,
+            'bytes': len(avatar.content)
+        }
+
+        used_xep84 = False
+        result = await self.xep_0084.publish_avatar(avatar.content)
+        if isinstance(result, XMPPError):
+            logger.debug('Could not publish XEP-0084 avatar')
+        else:
+            used_xep84 = True
+
+        result = await self.xep_0153.set_avatar(
+            avatar=avatar.content,
+            mtype=avatar.mtype
+        )
+        if isinstance(result, XMPPError):
+            logger.debug('Could not set vCard avatar')
+
+        if used_xep84:
+            result = await self.xep_0084.publish_avatar_metadata(
+                items=[avatar_metadata]
+            )
+            if isinstance(result, XMPPError):
+                logger.debug('Could not publish XEP-0084 metadata')
+
+        # Wait for presence updates to propagate...
+        # self.schedule('end', 5, self.disconnect, kwargs={'wait': True})
+
+    def __join_rooms(self):
+        for room in self.config.rooms:
+            self.xep_0045.join_muc(room, self.nick)
             msg = self.joined_room(room)
             if msg:
                 self.send_message(mto=room, mbody=msg, mtype='groupchat')
 
-        return None
-
     def joined_room(self, room):
         pass
 
     def groupchat_subject(self, data):
         pass
 
-    def get_match(self, regex, mode, text):
-        if mode == "findall":
-            return regex.findall(text)
-        m = None
-        if mode == "match":
-            m = regex.match(text)
-        elif mode == "search":
-            m = regex.search(text)
-        if m:
-            return m.groups()
-        return None
-
-    def get_cmd(self, msg, user, text):
-        delay = self.is_delay(msg)
-        cmd = text.split(' ', 1)[0].lower()
-        for c in self.commands:
-            if delay and not c._command_delay:
-                continue
-            if c._command_fromuser and user not in c._command_fromuser:
-                continue
-            if c._command_regex:
-                arg = self.get_match(
-                    c._command_regex, c._command_rg_mode, text)
-                if arg is not None and len(arg) > 0:
-                    return c, arg
-            elif cmd in c._command_names:
-                return c, text.split(' ')[1:]
-        return None, None
-
     def read_message(self, msg):
-        if msg['type'] not in self.config['lisent'] or not msg['body'] or not msg['from']:
-            return
-        if msg['type'] == 'groupchat' and msg['from'].resource.lower() == self.nick.lower():
-            return
-
-        user = msg['from'].bare
-        if user == self.boundjid.bare or (self.custom_roster and user not in self.custom_roster):
-            return
-
-        text = sp.sub(" ", msg['body']).strip()
-        if len(text) == 0:
+        msg: Message = Message.init(msg)
+        if self.__discard_message(msg):
             return
-
-        cmd, args = self.get_cmd(msg, user, text)
-        if not cmd:
-            self.log.debug("Unknown command from %s: %s" % (user, text))
+        cmd = self.__get_command(msg)
+        if cmd is None:
+            logger.debug(f"Unknown command from {msg.sender}: {msg.text}")
             return
-
-        self.log.debug("*** Command from %s: %s" % (user, text))
-
-        if msg['type'] == 'groupchat':
-            user = msg['from'].resource
+        logger.debug(f"Command from {msg.sender}: {msg.text}")
 
         try:
-            reply = cmd(*args, user=user, text=text, msg=msg)
+            reply = cmd.run(msg)
         except Exception as error:
-            self.log.exception('An error happened while processing '
-                               'the message: %s' % text)
-            reply = self.command_error(
-                error, *args, user=user, text=text, msg=msg)
+            logger.exception(
+                'An error happened while processing the message: ' +
+                msg.text)
+            reply = self.command_error(msg, error)
         if reply:
-            self.reply_message(msg, reply, *args, **msg)
+            self.reply_message(msg, reply)
 
-    def command_error(self, *args, **kwargs):
+    def __discard_message(self, msg):
+        if self.__is_weird_message(msg):
+            return True
+        if self.__is_from_me(msg):
+            return True
+        if not self.__is_in_my_inbox(msg):
+            return True
+        return False
+
+    def __is_weird_message(self, msg):
+        if not msg['body'] or (msg['from'] is None or not str(msg['from'])):
+            return True
+        txt = re_sp.sub(" ", msg['body']).strip()
+        if len(txt) == 0:
+            return True
+        return False
+
+    def __is_from_me(self, msg):
+        if msg['type'] == 'groupchat' and msg['from'].resource.lower(
+        ) == self.nick.lower():
+            return True
+        user = msg['from'].bare
+        if user == self.boundjid.bare:
+            return True
+        return False
+
+    def __is_in_my_inbox(self, msg):
+        if msg['type'] not in self.config.lisent:
+            return False
+        user = msg['from'].bare
+        if self.config.roster and user not in self.config.roster:
+            return False
+        return True
+
+    def __get_command(self, msg) -> CmdBot:
+        for cmd in self.commands:
+            if cmd.is_for_me(msg):
+                return cmd
+        return None
+
+    def command_error(self, msg, error):
+        if msg.sender in self.config.admin:
+            return str(error) + "\n\n" + traceback.format_exc()
         return self.MSG_ERROR_OCCURRED
 
     def tune_reply(self, txt):
         return txt
 
-    def reply_message(self, msg, txt, *args, **kwargs):
-        msgreply = msg.reply(self.tune_reply(txt))
-        _to = msgreply['to']
+    def reply_message(self, msg, txt):
+        reply = self.tune_reply(txt)
+        msgreply = msg.reply(reply)
         msgreply.send()
-        if self.config.get('img_to_oob', False):
+        if self.config.img_to_oob:
             imgs = set([i[0] for i in url_img.findall(txt)])
             for i in imgs:
                 imgreply = msg.reply()
-                imgreply['to'] = _to
                 imgreply['oob']['url'] = i
                 imgreply.send()
-
-    def is_delay(self, msg):
-        return self.delay and bool(msg['delay']._get_attr('stamp'))
```

