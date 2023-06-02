# Comparing `tmp/ramqp-8.4.3.tar.gz` & `tmp/ramqp-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramqp-8.4.3.tar", max compression
+gzip compressed data, was "ramqp-9.0.0.tar", max compression
```

## Comparing `ramqp-8.4.3.tar` & `ramqp-9.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0        0        0        0 2023-06-02 12:57:26.499595 ramqp-8.4.3/LICENSES/
--rw-r--r--   0        0        0    15177 2023-06-02 12:57:26.499595 ramqp-8.4.3/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     7466 2023-06-02 12:57:26.499595 ramqp-8.4.3/README.md
--rw-r--r--   0        0        0     1465 2023-06-02 12:57:38.331385 ramqp-8.4.3/pyproject.toml
--rw-r--r--   0        0        0      321 2023-06-02 12:57:26.501595 ramqp-8.4.3/ramqp/__init__.py
--rw-r--r--   0        0        0    16392 2023-06-02 12:57:26.502595 ramqp-8.4.3/ramqp/abstract.py
--rw-r--r--   0        0        0      668 2023-06-02 12:57:26.502595 ramqp-8.4.3/ramqp/amqp.py
--rw-r--r--   0        0        0     2729 2023-06-02 12:57:26.503595 ramqp-8.4.3/ramqp/config.py
--rw-r--r--   0        0        0    10021 2023-06-02 12:57:26.503595 ramqp-8.4.3/ramqp/depends.py
--rw-r--r--   0        0        0     7010 2023-06-02 12:57:26.503595 ramqp-8.4.3/ramqp/metrics.py
--rw-r--r--   0        0        0     8652 2023-06-02 12:57:26.504595 ramqp-8.4.3/ramqp/mo.py
--rw-r--r--   0        0        0        0 2023-06-02 12:57:26.547598 ramqp-8.4.3/ramqp/py.typed
--rw-r--r--   0        0        0     1367 2023-06-02 12:57:26.504595 ramqp-8.4.3/ramqp/utils.py
--rw-r--r--   0        0        0     8357 1970-01-01 00:00:00.000000 ramqp-8.4.3/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-06-02 13:25:50.890882 ramqp-9.0.0/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-06-02 13:25:50.890882 ramqp-9.0.0/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     7466 2023-06-02 13:25:50.890882 ramqp-9.0.0/README.md
+-rw-r--r--   0        0        0     1465 2023-06-02 13:26:03.776680 ramqp-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-06-02 13:25:50.892882 ramqp-9.0.0/ramqp/__init__.py
+-rw-r--r--   0        0        0    16392 2023-06-02 13:25:50.892882 ramqp-9.0.0/ramqp/abstract.py
+-rw-r--r--   0        0        0      668 2023-06-02 13:25:50.892882 ramqp-9.0.0/ramqp/amqp.py
+-rw-r--r--   0        0        0     2729 2023-06-02 13:25:50.892882 ramqp-9.0.0/ramqp/config.py
+-rw-r--r--   0        0        0    10056 2023-06-02 13:25:50.893882 ramqp-9.0.0/ramqp/depends.py
+-rw-r--r--   0        0        0     7010 2023-06-02 13:25:50.893882 ramqp-9.0.0/ramqp/metrics.py
+-rw-r--r--   0        0        0     8652 2023-06-02 13:25:50.893882 ramqp-9.0.0/ramqp/mo.py
+-rw-r--r--   0        0        0        0 2023-06-02 13:25:50.944886 ramqp-9.0.0/ramqp/py.typed
+-rw-r--r--   0        0        0     1367 2023-06-02 13:25:50.893882 ramqp-9.0.0/ramqp/utils.py
+-rw-r--r--   0        0        0     8357 1970-01-01 00:00:00.000000 ramqp-9.0.0/PKG-INFO
```

### Comparing `ramqp-8.4.3/LICENSES/MPL-2.0.txt` & `ramqp-9.0.0/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.3/README.md` & `ramqp-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.3/pyproject.toml` & `ramqp-9.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ramqp"
-version = "8.4.3"
+version = "9.0.0"
 description = "Rammearkitektur AMQP library (aio_pika wrapper)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ramqp"
 keywords = ["os2mo", "amqp"]
```

### Comparing `ramqp-8.4.3/ramqp/abstract.py` & `ramqp-9.0.0/ramqp/abstract.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.3/ramqp/amqp.py` & `ramqp-9.0.0/ramqp/amqp.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.3/ramqp/config.py` & `ramqp-9.0.0/ramqp/config.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.3/ramqp/depends.py` & `ramqp-9.0.0/ramqp/depends.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
 """This module implement FastAPI dependency injection for RAMQP."""
 import asyncio
+from asyncio import Task
 from collections import defaultdict
 from collections.abc import AsyncGenerator
 from collections.abc import Awaitable
 from collections.abc import Callable
 from collections.abc import Hashable
 from contextlib import asynccontextmanager
 from contextlib import AsyncExitStack
+from contextlib import suppress
 from functools import wraps
 from typing import Annotated
 from typing import Any
 from typing import cast
 from typing import DefaultDict
 from typing import TypeVar
 
@@ -76,15 +78,19 @@
         async with AsyncExitStack() as stack:
             request = Request(
                 {
                     "fastapi_astack": stack,
                     "type": "http",
                     "headers": [],
                     "query_string": "",
-                    "state": {"context": context, "message": message},
+                    "state": {
+                        "context": context,
+                        "message": message,
+                        "callback": function,
+                    },
                 }
             )
             dependant = get_dependant(path="", call=function)
 
             values, errors, *_ = await solve_dependencies(
                 request=request, dependant=dependant
             )
@@ -154,14 +160,29 @@
     """
     return state.message
 
 
 Message = Annotated[IncomingMessage, Depends(get_message)]
 
 
+def get_callback(state: State) -> Callable:
+    """Extract the callback function from the request state.
+
+    Args:
+        state: The request state from within the request.
+
+    Returns:
+        The callback function for this request.
+    """
+    return cast(Callable, state.callback)
+
+
+Callback = Annotated[Callable, Depends(get_callback)]
+
+
 def get_routing_key(message: Message) -> str:
     """Extract the AMQP message routing key.
 
     Args:
         message: The AMQP message to extract the payload from.
 
     Returns:
@@ -284,45 +305,43 @@
                 return await coro(*args, **kwargs)
 
         return wrapped
 
     return wrapper
 
 
-def sleep_on_error(delay: int = 30) -> Callable[[], AsyncGenerator[None, None]]:
-    """Construct an pseudo-context manager which delays returning on errors.
-
-    This is used to prevent race-conditions on writes to MO/LoRa, when the upload times
-    out initially but is completed by the backend afterwards. The sleep ensures that
-    the AMQP message is not retried immediately, causing the handler to act on
-    information which could become stale by the queued write. This happens because the
-    backend does not implement fairness of requests, such that read operations can
-    return soon-to-be stale data while a write operation is queued on another thread.
-
-    Specifically, duplicate objects would be created when a write operation failed to
-    complete within the timeout (but would be completed later), and the handler, during
-    retry, read an outdated list of existing objects, and thus dispatched another
-    (duplicate) write operation.
+def rate_limit(
+    delay: int = 30,
+) -> Callable[[Message, Callback], AsyncGenerator[None, None]]:
+    """Rate-limit processing of the same message by `delay` seconds.
 
-    See: https://redmine.magenta-aps.dk/issues/51949#note-23.
+    Rate-limiting is applied per-handler, so different message callback handlers can
+    process the same message simultaneously, without any limits.
 
     Args:
-        delay: The delay in seconds to sleep for.
+        delay: Number of seconds to wait between processing the same message.
 
-    Raises:
-        Whatever exception was thrown by the decorated function.
-
-    Returns:
-        A Coroutine pseudo-context manager which sleeps on any exception.
+    Returns: A dependency-injectable rate-limiter.
     """
+    tasks: dict[tuple[str, int], Task] = {}
 
-    async def inner() -> AsyncGenerator[None, None]:
-        try:
-            yield
-        except Exception:  # pylint: disable=broad-except
+    async def inner(message: Message, callback: Callback) -> AsyncGenerator[None, None]:
+        key = (message.message_id, id(callback))
+
+        with suppress(KeyError):
+            task = tasks[key]
+            await task
+
+        async def rate_limiter() -> None:
             await asyncio.sleep(delay)
-            raise
+            tasks.pop(key)
+
+        if key not in tasks:
+            task = asyncio.create_task(rate_limiter())
+            tasks[key] = task
+
+        yield
 
     return inner
 
 
-SleepOnError = Annotated[None, Depends(sleep_on_error())]
+RateLimit = Annotated[None, Depends(rate_limit())]
```

### Comparing `ramqp-8.4.3/ramqp/metrics.py` & `ramqp-9.0.0/ramqp/metrics.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.3/ramqp/mo.py` & `ramqp-9.0.0/ramqp/mo.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.3/ramqp/utils.py` & `ramqp-9.0.0/ramqp/utils.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.4.3/PKG-INFO` & `ramqp-9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramqp
-Version: 8.4.3
+Version: 9.0.0
 Summary: Rammearkitektur AMQP library (aio_pika wrapper)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
```

