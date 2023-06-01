# Comparing `tmp/lanarky-0.7.5.tar.gz` & `tmp/lanarky-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanarky-0.7.5.tar", max compression
+gzip compressed data, was "lanarky-0.7.6.tar", max compression
```

## Comparing `lanarky-0.7.5.tar` & `lanarky-0.7.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1073 2023-05-31 22:20:50.117144 lanarky-0.7.5/LICENSE
--rw-r--r--   0        0        0     4575 2023-05-31 22:20:50.117144 lanarky-0.7.5/README.md
--rw-r--r--   0        0        0       68 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/__init__.py
--rw-r--r--   0        0        0     2874 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/callbacks/__init__.py
--rw-r--r--   0        0        0     3023 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/callbacks/agents.py
--rw-r--r--   0        0        0     2200 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/callbacks/base.py
--rw-r--r--   0        0        0     1685 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/callbacks/llm.py
--rw-r--r--   0        0        0     3461 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0      422 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/register/__init__.py
--rw-r--r--   0        0        0     1171 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/register/base.py
--rw-r--r--   0        0        0     1074 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/register/callbacks.py
--rw-r--r--   0        0        0       74 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/responses/__init__.py
--rw-r--r--   0        0        0     3996 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/responses/streaming.py
--rw-r--r--   0        0        0      150 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/routing/__init__.py
--rw-r--r--   0        0        0     5266 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/routing/langchain.py
--rw-r--r--   0        0        0     4185 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/routing/utils.py
--rw-r--r--   0        0        0      715 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/schemas.py
--rw-r--r--   0        0        0       69 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/testing/__init__.py
--rw-r--r--   0        0        0     3212 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/testing/settings.py
--rw-r--r--   0        0        0       73 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/websockets/__init__.py
--rw-r--r--   0        0        0     3844 2023-05-31 22:20:50.325146 lanarky-0.7.5/lanarky/websockets/base.py
--rw-r--r--   0        0        0     1399 2023-05-31 22:20:50.325146 lanarky-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     5709 1970-01-01 00:00:00.000000 lanarky-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-01 22:26:50.860827 lanarky-0.7.6/LICENSE
+-rw-r--r--   0        0        0     4575 2023-06-01 22:26:50.860827 lanarky-0.7.6/README.md
+-rw-r--r--   0        0        0       68 2023-06-01 22:26:51.036829 lanarky-0.7.6/lanarky/__init__.py
+-rw-r--r--   0        0        0     2874 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/callbacks/__init__.py
+-rw-r--r--   0        0        0     3023 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/callbacks/agents.py
+-rw-r--r--   0        0        0     2200 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/callbacks/base.py
+-rw-r--r--   0        0        0     1685 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/callbacks/llm.py
+-rw-r--r--   0        0        0     3461 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0      422 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/register/__init__.py
+-rw-r--r--   0        0        0     1171 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/register/base.py
+-rw-r--r--   0        0        0     1074 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/register/callbacks.py
+-rw-r--r--   0        0        0       74 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/responses/__init__.py
+-rw-r--r--   0        0        0     4956 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/responses/streaming.py
+-rw-r--r--   0        0        0      150 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/routing/__init__.py
+-rw-r--r--   0        0        0     5266 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/routing/langchain.py
+-rw-r--r--   0        0        0     4185 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/routing/utils.py
+-rw-r--r--   0        0        0      715 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/schemas.py
+-rw-r--r--   0        0        0       69 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/testing/__init__.py
+-rw-r--r--   0        0        0     3212 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/websockets/__init__.py
+-rw-r--r--   0        0        0     3844 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/websockets/base.py
+-rw-r--r--   0        0        0     1399 2023-06-01 22:26:51.040829 lanarky-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     5709 1970-01-01 00:00:00.000000 lanarky-0.7.6/PKG-INFO
```

### Comparing `lanarky-0.7.5/LICENSE` & `lanarky-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.5/README.md` & `lanarky-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.5/lanarky/callbacks/__init__.py` & `lanarky-0.7.6/lanarky/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.5/lanarky/callbacks/agents.py` & `lanarky-0.7.6/lanarky/callbacks/agents.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.5/lanarky/callbacks/base.py` & `lanarky-0.7.6/lanarky/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.5/lanarky/callbacks/llm.py` & `lanarky-0.7.6/lanarky/callbacks/llm.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.5/lanarky/callbacks/retrieval_qa.py` & `lanarky-0.7.6/lanarky/callbacks/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.5/lanarky/register/base.py` & `lanarky-0.7.6/lanarky/register/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.5/lanarky/register/callbacks.py` & `lanarky-0.7.6/lanarky/register/callbacks.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.5/lanarky/responses/streaming.py` & `lanarky-0.7.6/lanarky/responses/streaming.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Credits:
 
 * `gist@ninely <https://gist.github.com/ninely/88485b2e265d852d3feb8bd115065b1a>`_
 * `langchain@#1705 <https://github.com/hwchase17/langchain/discussions/1706>`_
 """
+import asyncio
 import logging
-from functools import wraps
+from functools import partial, wraps
 from typing import Any, Awaitable, Callable, Optional, Union
 
 import aiohttp
 from fastapi.responses import StreamingResponse as _StreamingResponse
 from langchain.chains.base import Chain
 from starlette.background import BackgroundTask
 from starlette.types import Receive, Scope, Send
@@ -28,21 +29,21 @@
             import openai  # type: ignore
         except ImportError:
             raise ImportError(
                 "openai is not installed. Install it with `pip install 'lanarky[openai]'`."
             )
 
         openai.aiosession.set(aiohttp.ClientSession())
-        logger.info(f"opeanai.aiosession set: {openai.aiosession.get()}")
+        logger.debug(f"opeanai.aiosession set: {openai.aiosession.get()}")
 
         try:
             await func(*args, **kwargs)
         finally:
             await openai.aiosession.get().close()
-            logger.info(f"opeanai.aiosession closed: {openai.aiosession.get()}")
+            logger.debug(f"opeanai.aiosession closed: {openai.aiosession.get()}")
 
     return wrapper
 
 
 # TODO: create OpenAIStreamingResponse for streaming with OpenAI only
 class StreamingResponse(_StreamingResponse):
     """StreamingResponse class wrapper for langchain chains."""
@@ -53,14 +54,21 @@
         background: Optional[BackgroundTask] = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(content=iter(()), background=background, **kwargs)
 
         self.chain_executor = chain_executor
 
+    async def listen_for_disconnect(self, receive: Receive) -> None:
+        while True:
+            message = await receive()
+            if message["type"] == "http.disconnect":
+                logger.debug("Client disconnected")
+                break
+
     async def stream_response(self, send: Send) -> None:
         await send(
             {
                 "type": "http.response.start",
                 "status": self.status_code,
                 "headers": self.raw_headers,
             }
@@ -82,15 +90,35 @@
             )
             return
 
         await send({"type": "http.response.body", "body": b"", "more_body": False})
 
     @openai_aiosession
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
-        await super().__call__(scope, receive, send)
+        async def wrap(func: Callable[[], Awaitable[None]]) -> None:
+            await func()
+            raise asyncio.CancelledError
+
+        async def run_tasks():
+            stream_response_task = asyncio.create_task(
+                wrap(partial(self.stream_response, send))
+            )
+            listen_for_disconnect_task = asyncio.create_task(
+                wrap(partial(self.listen_for_disconnect, receive))
+            )
+
+            try:
+                await asyncio.gather(stream_response_task, listen_for_disconnect_task)
+            except asyncio.CancelledError:
+                pass
+
+        await asyncio.create_task(run_tasks())
+
+        if self.background is not None:
+            await self.background()
 
     @staticmethod
     def _create_chain_executor(
         chain: Chain,
         inputs: Union[dict[str, Any], Any],
         as_json: bool = False,
         **callback_kwargs,
```

### Comparing `lanarky-0.7.5/lanarky/routing/langchain.py` & `lanarky-0.7.6/lanarky/routing/langchain.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.5/lanarky/routing/utils.py` & `lanarky-0.7.6/lanarky/routing/utils.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.5/lanarky/schemas.py` & `lanarky-0.7.6/lanarky/schemas.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.5/lanarky/testing/gradio.py` & `lanarky-0.7.6/lanarky/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.5/lanarky/websockets/base.py` & `lanarky-0.7.6/lanarky/websockets/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.5/pyproject.toml` & `lanarky-0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lanarky"
-version = "0.7.5"
+version = "0.7.6"
 description = "Ship production-ready LLM projects with FastAPI"
 authors = ["Ajinkya Indulkar <26824103+ajndkr@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/ajndkr/lanarky"
 repository = "https://github.com/ajndkr/lanarky"
 license = "MIT"
 packages = [{include = "lanarky"}]
```

### Comparing `lanarky-0.7.5/PKG-INFO` & `lanarky-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanarky
-Version: 0.7.5
+Version: 0.7.6
 Summary: Ship production-ready LLM projects with FastAPI
 Home-page: https://github.com/ajndkr/lanarky
 License: MIT
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

