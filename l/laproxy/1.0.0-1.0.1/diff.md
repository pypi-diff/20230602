# Comparing `tmp/laproxy-1.0.0.tar.gz` & `tmp/laproxy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laproxy-1.0.0.tar", max compression
+gzip compressed data, was "laproxy-1.0.1.tar", max compression
```

## Comparing `laproxy-1.0.0.tar` & `laproxy-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      406 2022-07-02 19:58:33.808686 laproxy-1.0.0/laproxy/__init__.py
--rw-r--r--   0        0        0     4868 2022-07-02 19:58:33.808686 laproxy-1.0.0/laproxy/_http.py
--rw-r--r--   0        0        0      501 2022-07-02 19:58:33.808686 laproxy-1.0.0/laproxy/_laproxy.py
--rw-r--r--   0        0        0     2528 2022-07-02 19:58:33.808686 laproxy-1.0.0/laproxy/_tcp.py
--rw-r--r--   0        0        0        0 2022-07-02 19:58:33.808686 laproxy-1.0.0/laproxy/py.typed
--rw-r--r--   0        0        0      735 2022-07-02 19:58:33.808686 laproxy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      519 2022-07-02 19:59:12.477357 laproxy-1.0.0/setup.py
--rw-r--r--   0        0        0      368 2022-07-02 19:59:12.477594 laproxy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      406 2023-06-02 08:55:27.653001 laproxy-1.0.1/laproxy/__init__.py
+-rw-r--r--   0        0        0     5086 2023-06-02 08:55:27.653001 laproxy-1.0.1/laproxy/_http.py
+-rw-r--r--   0        0        0      501 2023-06-02 08:55:27.653001 laproxy-1.0.1/laproxy/_laproxy.py
+-rw-r--r--   0        0        0     2898 2023-06-02 08:55:27.653001 laproxy-1.0.1/laproxy/_tcp.py
+-rw-r--r--   0        0        0        0 2023-06-02 08:55:27.653001 laproxy-1.0.1/laproxy/py.typed
+-rw-r--r--   0        0        0      484 2023-06-02 08:55:27.653001 laproxy-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 laproxy-1.0.1/PKG-INFO
```

### Comparing `laproxy-1.0.0/laproxy/_tcp.py` & `laproxy-1.0.1/laproxy/_tcp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 from __future__ import annotations
-from asyncio import StreamReader, StreamWriter, start_server, open_connection, gather
+from asyncio import (
+    StreamReader,
+    StreamWriter,
+    start_server,
+    open_connection,
+)
 from ._laproxy import Handler, Proxy
 from abc import ABC, abstractmethod
 from collections.abc import Callable
+from aiotools import TaskGroup  # type: ignore
+from typing import TYPE_CHECKING
 from traceback import print_exc
 
+if TYPE_CHECKING:
+    from asyncio import TaskGroup as TG
+
+DEFAULT_TCP_BUFFSIZE = 1024
+
 
 class TCPHandler(Handler, ABC):
+    def buffsize(self) -> int:
+        return DEFAULT_TCP_BUFFSIZE
+
     async def handle(
         self, reader: StreamReader, writer: StreamWriter, inbound: bool, /
     ) -> None:
         while True:
-            packet = await reader.read(1024)
+            packet = await reader.read(self.buffsize())
             if not packet:
                 break
             packet = self.process(packet, inbound)
             if packet is None:
                 break
             writer.write(packet)
 
@@ -44,41 +59,45 @@
         server = await start_server(
             self._thread, self._listen_address, self._listen_port
         )
         async with server:
             await server.serve_forever()
 
     async def _thread(self, reader: StreamReader, writer: StreamWriter, /) -> None:
-        target_reader, target_writer = await open_connection(
-            self._target_address, self._target_port
-        )
-        handler = self._handler()
-        await gather(
-            self._handle(handler, reader, target_writer, True),
-            self._handle(handler, target_reader, writer, False),
-        )
+        try:
+            target_reader, target_writer = await open_connection(
+                self._target_address, self._target_port
+            )
+            handler = self._handler()
+            group: TG
+            async with TaskGroup() as group:  # type: ignore
+                group.create_task(
+                    self._handle(handler, reader, target_writer, True),
+                    name="tcp inbound",
+                )
+                group.create_task(
+                    self._handle(handler, target_reader, writer, False),
+                    name="tcp outbound",
+                )
+        except GeneratorExit:
+            pass
+        except:
+            print_exc()
 
     async def _handle(
         self,
         handler: Handler,
         reader: StreamReader,
         writer: StreamWriter,
         inbound: bool,
         /,
     ) -> None:
         try:
             await handler.handle(reader, writer, inbound)
-        except BaseException as e:
-            if not isinstance(e, GeneratorExit):
-                print_exc()
         finally:
-            try:
-                writer.close()
-                await writer.wait_closed()
-            except BaseException as e:
-                if not isinstance(e, RuntimeError):
-                    print_exc()
+            writer.close()
+            await writer.wait_closed()
 
 
 class NoTCPHandler(TCPHandler):
     def process(self, packet: bytes, _: bool, /) -> bytes | None:
         return packet
```

