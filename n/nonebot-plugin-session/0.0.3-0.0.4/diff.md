# Comparing `tmp/nonebot_plugin_session-0.0.3.tar.gz` & `tmp/nonebot_plugin_session-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_session-0.0.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_session-0.0.4.tar", max compression
```

## Comparing `nonebot_plugin_session-0.0.3.tar` & `nonebot_plugin_session-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1063 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/LICENSE
--rw-r--r--   0        0        0     4217 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/README.md
--rw-r--r--   0        0        0      161 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/nonebot_plugin_session/__init__.py
--rw-r--r--   0        0        0       75 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/nonebot_plugin_session/adapters/__init__.py
--rw-r--r--   0        0        0      585 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/nonebot_plugin_session/adapters/console.py
--rw-r--r--   0        0        0     1190 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/nonebot_plugin_session/adapters/kaiheila.py
--rw-r--r--   0        0        0     2719 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/nonebot_plugin_session/adapters/onebot_v11.py
--rw-r--r--   0        0        0     3537 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/nonebot_plugin_session/adapters/onebot_v12.py
--rw-r--r--   0        0        0     1565 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/nonebot_plugin_session/adapters/qqguild.py
--rw-r--r--   0        0        0     2616 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/nonebot_plugin_session/adapters/telegram.py
--rw-r--r--   0        0        0      398 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/nonebot_plugin_session/const.py
--rw-r--r--   0        0        0     2700 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/nonebot_plugin_session/extractor.py
--rw-r--r--   0        0        0     1525 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/nonebot_plugin_session/migrations/36de70108aeb_init_db.py
--rw-r--r--   0        0        0     2793 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/nonebot_plugin_session/model.py
--rw-r--r--   0        0        0     2207 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/nonebot_plugin_session/saa.py
--rw-r--r--   0        0        0     2053 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/nonebot_plugin_session/session.py
--rw-r--r--   0        0        0     1879 2023-05-17 03:21:36.604661 nonebot_plugin_session-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 nonebot_plugin_session-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4340 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/README.md
+-rw-r--r--   0        0        0      161 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/nonebot_plugin_session/__init__.py
+-rw-r--r--   0        0        0       75 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/__init__.py
+-rw-r--r--   0        0        0      585 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/console.py
+-rw-r--r--   0        0        0     1190 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/kaiheila.py
+-rw-r--r--   0        0        0     2719 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     3537 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     1565 2023-06-02 08:20:23.192325 nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/qqguild.py
+-rw-r--r--   0        0        0     2616 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/telegram.py
+-rw-r--r--   0        0        0      398 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/nonebot_plugin_session/const.py
+-rw-r--r--   0        0        0     2700 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/nonebot_plugin_session/extractor.py
+-rw-r--r--   0        0        0     1525 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/nonebot_plugin_session/migrations/36de70108aeb_init_db.py
+-rw-r--r--   0        0        0     2814 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/nonebot_plugin_session/model.py
+-rw-r--r--   0        0        0     2207 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/nonebot_plugin_session/saa.py
+-rw-r--r--   0        0        0     2053 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/nonebot_plugin_session/session.py
+-rw-r--r--   0        0        0     1879 2023-06-02 08:20:23.196326 nonebot_plugin_session-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5396 1970-01-01 00:00:00.000000 nonebot_plugin_session-0.0.4/PKG-INFO
```

### Comparing `nonebot_plugin_session-0.0.3/LICENSE` & `nonebot_plugin_session-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.3/README.md` & `nonebot_plugin_session-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -76,21 +76,23 @@
     ...
 ```
 
 
 将 `Session` 存至数据库中（需要安装 [nonebot-plugin-datastore](https://github.com/he0119/nonebot-plugin-datastore) 插件）
 
 ```python
+from nonebot_plugin_datastore import create_session
 from nonebot_plugin_session import extract_session
 from nonebot_plugin_session.model import get_or_add_session_model
 
 @matcher.handle()
 async def handle(bot: Bot, event: Event):
     session = extract_session(bot, event)
-    model = await get_or_add_session_model(session)  # 可关联其他表用于筛选等
+    async with create_session() as db_session:
+        session_model = await get_or_add_session_model(session, db_session)  # 可关联其他表用于筛选等
 ```
 
 
 从 `Session` 中获取 `saa` 的 `PlatformTarget` 对象用于发送（需要安装 [nonebot-plugin-send-anything-anywhere](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) 插件）
 
 ```python
 from nonebot_plugin_session import extract_session
```

#### html2text {}

```diff
@@ -19,26 +19,28 @@
 extract_session @matcher.handle() async def handle(bot: Bot, event: Event):
 session = extract_session(bot, event) ``` è·å `session id`ï¼ ```python from
 nonebot_plugin_session import SessionId, SessionIdType @matcher.handle() async
 def handle(session_id: str = SessionId(SessionIdType.GROUP)): # è·å
 âç¾¤ç»çº§å«â ç session id ... ``` å° `Session`
 å­è³æ°æ®åºä¸­ï¼éè¦å®è£ [nonebot-plugin-datastore](https://
 github.com/he0119/nonebot-plugin-datastore) æä»¶ï¼ ```python from
-nonebot_plugin_session import extract_session from nonebot_plugin_session.model
-import get_or_add_session_model @matcher.handle() async def handle(bot: Bot,
-event: Event): session = extract_session(bot, event) model = await
-get_or_add_session_model(session) # å¯å³èå¶ä»è¡¨ç¨äºç­éç­ ``` ä»
-`Session` ä¸­è·å `saa` ç `PlatformTarget`
-å¯¹è±¡ç¨äºåéï¼éè¦å®è£ [nonebot-plugin-send-anything-anywhere]
-(https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) æä»¶ï¼
-```python from nonebot_plugin_session import extract_session @matcher.handle()
-async def handle(bot: Bot, event: Event): session = extract_session(bot, event)
-target = session.get_saa_target() # ç¨äºåé ``` ä¸åç
-âä¼è¯çº§å«â ä¸ âä¼è¯idç±»åâ ä¸è¿åç id
-å¦ä¸è¡¨æç¤ºï¼ï¼ä¸åå« `bot_id` ç­å±æ§çæåµï¼ | | LEVEL0
+nonebot_plugin_datastore import create_session from nonebot_plugin_session
+import extract_session from nonebot_plugin_session.model import
+get_or_add_session_model @matcher.handle() async def handle(bot: Bot, event:
+Event): session = extract_session(bot, event) async with create_session() as
+db_session: session_model = await get_or_add_session_model(session, db_session)
+# å¯å³èå¶ä»è¡¨ç¨äºç­éç­ ``` ä» `Session` ä¸­è·å `saa` ç
+`PlatformTarget` å¯¹è±¡ç¨äºåéï¼éè¦å®è£ [nonebot-plugin-send-
+anything-anywhere](https://github.com/felinae98/nonebot-plugin-send-anything-
+anywhere) æä»¶ï¼ ```python from nonebot_plugin_session import
+extract_session @matcher.handle() async def handle(bot: Bot, event: Event):
+session = extract_session(bot, event) target = session.get_saa_target() #
+ç¨äºåé ``` ä¸åç âä¼è¯çº§å«â ä¸ âä¼è¯idç±»åâ
+ä¸è¿åç id å¦ä¸è¡¨æç¤ºï¼ï¼ä¸åå« `bot_id` ç­å±æ§çæåµï¼ |
+| LEVEL0
 ï¼æ ç¨æ·ï¼ | LEVEL1
 ï¼åç¨æ·ï¼ | LEVEL2
 ï¼åçº§ç¾¤ç»ï¼ | LEVEL3
 ï¼ä¸¤çº§ç¾¤ç»ï¼ | | --- | --- | --- | --- | --- | | TYPE0 (GLOBAL) | `""` |
 `""` | `""` | `""` | | TYPE1 (USER) | `""` | `"id1"` | `"id1"` | `"id1"` | |
 TYPE2 | `""` | `"id1"` | `"id2"` | `"id2"` | | TYPE3 | `""` | `"id1"` |
 `"id2_id1"` | `"id2_id1"` | | TYPE4 | `""` | `"id1"` | `"id2"` | `"id3"` | |
```

### Comparing `nonebot_plugin_session-0.0.3/nonebot_plugin_session/adapters/console.py` & `nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.3/nonebot_plugin_session/adapters/kaiheila.py` & `nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.3/nonebot_plugin_session/adapters/onebot_v11.py` & `nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.3/nonebot_plugin_session/adapters/onebot_v12.py` & `nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/onebot_v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.3/nonebot_plugin_session/adapters/qqguild.py` & `nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.3/nonebot_plugin_session/adapters/telegram.py` & `nonebot_plugin_session-0.0.4/nonebot_plugin_session/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.3/nonebot_plugin_session/extractor.py` & `nonebot_plugin_session-0.0.4/nonebot_plugin_session/extractor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.3/nonebot_plugin_session/migrations/36de70108aeb_init_db.py` & `nonebot_plugin_session-0.0.4/nonebot_plugin_session/migrations/36de70108aeb_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.3/nonebot_plugin_session/model.py` & `nonebot_plugin_session-0.0.4/nonebot_plugin_session/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from .session import Session, SessionLevel
 
 try:
     from nonebot import require
 
     require("nonebot_plugin_datastore")
 
-    from nonebot_plugin_datastore import create_session, get_plugin_data
+    from nonebot_plugin_datastore import get_plugin_data
     from sqlalchemy import Enum, String, UniqueConstraint, select
+    from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm import Mapped, mapped_column
 
     Model = get_plugin_data().Model
 
     class SessionModel(Model):
         __table_args__ = (
             UniqueConstraint(
@@ -44,38 +45,41 @@
                 platform=self.platform,
                 level=self.level,
                 id1=self.id1,
                 id2=self.id2,
                 id3=self.id3,
             )
 
-    async def get_or_add_session_model(session: Session) -> SessionModel:
-        async with create_session() as db_session:
-            statement = (
-                select(SessionModel)
-                .where(SessionModel.bot_id == session.bot_id)
-                .where(SessionModel.bot_type == session.bot_type)
-                .where(SessionModel.platform == session.platform)
-                .where(SessionModel.level == session.level)
-                .where(SessionModel.id1 == session.id1)
-                .where(SessionModel.id2 == session.id2)
-                .where(SessionModel.id3 == session.id3)
-            )
-            results = await db_session.scalars(statement)
-            if session_model := results.one_or_none():
-                return session_model
-
-            session_model = SessionModel(
-                bot_id=session.bot_id,
-                bot_type=session.bot_type,
-                platform=session.platform,
-                level=session.level,
-                id1=session.id1,
-                id2=session.id2,
-                id3=session.id3,
-            )
-            db_session.add(session_model)
-            await db_session.commit()
+    async def get_or_add_session_model(
+        session: Session, db_session: AsyncSession, commit: bool = True
+    ) -> SessionModel:
+        statement = (
+            select(SessionModel)
+            .where(SessionModel.bot_id == session.bot_id)
+            .where(SessionModel.bot_type == session.bot_type)
+            .where(SessionModel.platform == session.platform)
+            .where(SessionModel.level == session.level)
+            .where(SessionModel.id1 == session.id1)
+            .where(SessionModel.id2 == session.id2)
+            .where(SessionModel.id3 == session.id3)
+        )
+        results = await db_session.scalars(statement)
+        if session_model := results.one_or_none():
             return session_model
 
+        session_model = SessionModel(
+            bot_id=session.bot_id,
+            bot_type=session.bot_type,
+            platform=session.platform,
+            level=session.level,
+            id1=session.id1,
+            id2=session.id2,
+            id3=session.id3,
+        )
+        db_session.add(session_model)
+        if commit:
+            await db_session.commit()
+            await db_session.refresh(session_model)
+        return session_model
+
 except (ImportError, RuntimeError):
     pass
```

### Comparing `nonebot_plugin_session-0.0.3/nonebot_plugin_session/saa.py` & `nonebot_plugin_session-0.0.4/nonebot_plugin_session/saa.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.3/nonebot_plugin_session/session.py` & `nonebot_plugin_session-0.0.4/nonebot_plugin_session/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.3/pyproject.toml` & `nonebot_plugin_session-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_session"
-version = "0.0.3"
+version = "0.0.4"
 description = "Nonebot2 会话信息提取与会话id定义"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-session"
 repository = "https://github.com/noneplugin/nonebot-plugin-session"
```

### Comparing `nonebot_plugin_session-0.0.3/PKG-INFO` & `nonebot_plugin_session-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-session
-Version: 0.0.3
+Version: 0.0.4
 Summary: Nonebot2 会话信息提取与会话id定义
 Home-page: https://github.com/noneplugin/nonebot-plugin-session
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -101,21 +101,23 @@
     ...
 ```
 
 
 将 `Session` 存至数据库中（需要安装 [nonebot-plugin-datastore](https://github.com/he0119/nonebot-plugin-datastore) 插件）
 
 ```python
+from nonebot_plugin_datastore import create_session
 from nonebot_plugin_session import extract_session
 from nonebot_plugin_session.model import get_or_add_session_model
 
 @matcher.handle()
 async def handle(bot: Bot, event: Event):
     session = extract_session(bot, event)
-    model = await get_or_add_session_model(session)  # 可关联其他表用于筛选等
+    async with create_session() as db_session:
+        session_model = await get_or_add_session_model(session, db_session)  # 可关联其他表用于筛选等
 ```
 
 
 从 `Session` 中获取 `saa` 的 `PlatformTarget` 对象用于发送（需要安装 [nonebot-plugin-send-anything-anywhere](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) 插件）
 
 ```python
 from nonebot_plugin_session import extract_session
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-session Version: 0.0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-session Version: 0.0.4 Summary:
 Nonebot2 ä¼è¯ä¿¡æ¯æåä¸ä¼è¯idå®ä¹ Home-page: https://github.com/
 noneplugin/nonebot-plugin-session License: MIT Author: meetwq Author-email:
 meetwq@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: all
@@ -34,26 +34,28 @@
 extract_session @matcher.handle() async def handle(bot: Bot, event: Event):
 session = extract_session(bot, event) ``` è·å `session id`ï¼ ```python from
 nonebot_plugin_session import SessionId, SessionIdType @matcher.handle() async
 def handle(session_id: str = SessionId(SessionIdType.GROUP)): # è·å
 âç¾¤ç»çº§å«â ç session id ... ``` å° `Session`
 å­è³æ°æ®åºä¸­ï¼éè¦å®è£ [nonebot-plugin-datastore](https://
 github.com/he0119/nonebot-plugin-datastore) æä»¶ï¼ ```python from
-nonebot_plugin_session import extract_session from nonebot_plugin_session.model
-import get_or_add_session_model @matcher.handle() async def handle(bot: Bot,
-event: Event): session = extract_session(bot, event) model = await
-get_or_add_session_model(session) # å¯å³èå¶ä»è¡¨ç¨äºç­éç­ ``` ä»
-`Session` ä¸­è·å `saa` ç `PlatformTarget`
-å¯¹è±¡ç¨äºåéï¼éè¦å®è£ [nonebot-plugin-send-anything-anywhere]
-(https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) æä»¶ï¼
-```python from nonebot_plugin_session import extract_session @matcher.handle()
-async def handle(bot: Bot, event: Event): session = extract_session(bot, event)
-target = session.get_saa_target() # ç¨äºåé ``` ä¸åç
-âä¼è¯çº§å«â ä¸ âä¼è¯idç±»åâ ä¸è¿åç id
-å¦ä¸è¡¨æç¤ºï¼ï¼ä¸åå« `bot_id` ç­å±æ§çæåµï¼ | | LEVEL0
+nonebot_plugin_datastore import create_session from nonebot_plugin_session
+import extract_session from nonebot_plugin_session.model import
+get_or_add_session_model @matcher.handle() async def handle(bot: Bot, event:
+Event): session = extract_session(bot, event) async with create_session() as
+db_session: session_model = await get_or_add_session_model(session, db_session)
+# å¯å³èå¶ä»è¡¨ç¨äºç­éç­ ``` ä» `Session` ä¸­è·å `saa` ç
+`PlatformTarget` å¯¹è±¡ç¨äºåéï¼éè¦å®è£ [nonebot-plugin-send-
+anything-anywhere](https://github.com/felinae98/nonebot-plugin-send-anything-
+anywhere) æä»¶ï¼ ```python from nonebot_plugin_session import
+extract_session @matcher.handle() async def handle(bot: Bot, event: Event):
+session = extract_session(bot, event) target = session.get_saa_target() #
+ç¨äºåé ``` ä¸åç âä¼è¯çº§å«â ä¸ âä¼è¯idç±»åâ
+ä¸è¿åç id å¦ä¸è¡¨æç¤ºï¼ï¼ä¸åå« `bot_id` ç­å±æ§çæåµï¼ |
+| LEVEL0
 ï¼æ ç¨æ·ï¼ | LEVEL1
 ï¼åç¨æ·ï¼ | LEVEL2
 ï¼åçº§ç¾¤ç»ï¼ | LEVEL3
 ï¼ä¸¤çº§ç¾¤ç»ï¼ | | --- | --- | --- | --- | --- | | TYPE0 (GLOBAL) | `""` |
 `""` | `""` | `""` | | TYPE1 (USER) | `""` | `"id1"` | `"id1"` | `"id1"` | |
 TYPE2 | `""` | `"id1"` | `"id2"` | `"id2"` | | TYPE3 | `""` | `"id1"` |
 `"id2_id1"` | `"id2_id1"` | | TYPE4 | `""` | `"id1"` | `"id2"` | `"id3"` | |
```

