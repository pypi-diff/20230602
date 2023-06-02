# Comparing `tmp/nonebot_plugin_escape_url-0.1.0.tar.gz` & `tmp/nonebot_plugin_escape_url-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_escape_url-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_escape_url-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_escape_url-0.1.0.tar` & `nonebot_plugin_escape_url-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       49 2023-05-31 15:01:24.094557 nonebot_plugin_escape_url-0.1.0/nonebot_plugin_escape_url/__init__.py
--rw-r--r--   0        0        0      887 2023-05-31 14:54:01.294437 nonebot_plugin_escape_url-0.1.0/nonebot_plugin_escape_url/core.py
--rw-r--r--   0        0        0     1054 2023-05-31 15:11:30.346706 nonebot_plugin_escape_url-0.1.0/nonebot_plugin_escape_url/onebot_v11.py
--rw-r--r--   0        0        0      855 2023-05-31 15:02:36.150400 nonebot_plugin_escape_url-0.1.0/nonebot_plugin_escape_url/qqguild.py
--rw-r--r--   0        0        0      549 2023-05-31 14:55:51.004760 nonebot_plugin_escape_url-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      180 2023-05-31 15:15:05.708228 nonebot_plugin_escape_url-0.1.0/README.md
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 nonebot_plugin_escape_url-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-05-31 15:01:24.094557 nonebot_plugin_escape_url-0.1.1/nonebot_plugin_escape_url/__init__.py
+-rw-r--r--   0        0        0      240 2023-06-02 00:25:18.879236 nonebot_plugin_escape_url-0.1.1/nonebot_plugin_escape_url/config.py
+-rw-r--r--   0        0        0     1031 2023-06-02 00:36:31.049274 nonebot_plugin_escape_url-0.1.1/nonebot_plugin_escape_url/core.py
+-rw-r--r--   0        0        0     1148 2023-06-02 00:25:54.493031 nonebot_plugin_escape_url-0.1.1/nonebot_plugin_escape_url/onebot_v11.py
+-rw-r--r--   0        0        0      915 2023-06-02 00:25:54.503107 nonebot_plugin_escape_url-0.1.1/nonebot_plugin_escape_url/qqguild.py
+-rw-r--r--   0        0        0      549 2023-06-02 02:42:05.013519 nonebot_plugin_escape_url-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      223 2023-05-31 15:17:18.124586 nonebot_plugin_escape_url-0.1.1/README.md
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 nonebot_plugin_escape_url-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_escape_url-0.1.0/nonebot_plugin_escape_url/onebot_v11.py` & `nonebot_plugin_escape_url-0.1.1/nonebot_plugin_escape_url/onebot_v11.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from nonebot.typing import overrides
 
+from .config import conf
+
 try:
     from typing import Any, Union
 
     from nonebot import logger, Bot as BaseBot
     from nonebot.adapters.onebot.v11 import Bot, Event, Message, MessageSegment
 
     from .core import escape_text
 
     _origin_call_api = Bot.call_api
 
+
     @overrides(BaseBot)
     async def call_api(self, api: str, **data: Any) -> Any:
         if api == 'send_msg':
             message = data.get("message", None)
 
             if isinstance(message, str):
-                message = escape_text(message)
+                message = escape_text(message, conf.escape_url_replace_dot_by)
             elif isinstance(message, Message):
                 for seg in message:
                     if seg.type == 'text':
-                        seg.data['text'] = escape_text(seg.data['text'])
+                        seg.data['text'] = escape_text(seg.data['text'], conf.escape_url_replace_dot_by)
 
             logger.trace(f"escaped message: {message}")
             data['message'] = message
         return await _origin_call_api(self, api, **data)
 
 
     Bot.call_api = call_api
```

### Comparing `nonebot_plugin_escape_url-0.1.0/pyproject.toml` & `nonebot_plugin_escape_url-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-escape-url"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_escape_url" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_escape_url-0.1.0/PKG-INFO` & `nonebot_plugin_escape_url-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-escape-url
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,14 +13,16 @@
 Description-Content-Type: text/markdown
 
 nonebot-plugin-escape-url
 ========
 
 自动转换发送消息中的URL🤔
 
+支持适配器：OneBot V11、QQ频道
+
 ## 卖家秀
 
 使用前：
 
 ![使用前](img/1.png)
 
 使用后：
```

