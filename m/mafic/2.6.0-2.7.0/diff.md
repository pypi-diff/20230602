# Comparing `tmp/mafic-2.6.0.tar.gz` & `tmp/mafic-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafic-2.6.0.tar", max compression
+gzip compressed data, was "mafic-2.7.0.tar", max compression
```

## Comparing `mafic-2.6.0.tar` & `mafic-2.7.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1070 2023-06-01 20:34:38.935827 mafic-2.6.0/LICENSE
--rw-r--r--   0        0        0     3315 2023-06-01 20:34:38.935827 mafic-2.6.0/README.md
--rw-r--r--   0        0        0      886 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/__init__.py
--rw-r--r--   0        0        0     3554 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/__libraries.py
--rw-r--r--   0        0        0     1559 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/__main__.py
--rw-r--r--   0        0        0     4490 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/errors.py
--rw-r--r--   0        0        0     5617 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/events.py
--rw-r--r--   0        0        0    27782 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/filter.py
--rw-r--r--   0        0        0     7397 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/ip.py
--rw-r--r--   0        0        0    42218 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/node.py
--rw-r--r--   0        0        0    27377 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/player.py
--rw-r--r--   0        0        0     1232 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/playlist.py
--rw-r--r--   0        0        0      674 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/plugin.py
--rw-r--r--   0        0        0    11224 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/pool.py
--rw-r--r--   0        0        0        0 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/py.typed
--rw-r--r--   0        0        0     3648 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/region.py
--rw-r--r--   0        0        0     1031 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/search_type.py
--rw-r--r--   0        0        0     3437 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/stats.py
--rw-r--r--   0        0        0     5254 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/strategy.py
--rw-r--r--   0        0        0     4797 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/track.py
--rw-r--r--   0        0        0      747 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/type_variables.py
--rw-r--r--   0        0        0      199 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/typings/__init__.py
--rw-r--r--   0        0        0     2996 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/typings/common.py
--rw-r--r--   0        0        0     4712 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/typings/http.py
--rw-r--r--   0        0        0     2385 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/typings/incoming.py
--rw-r--r--   0        0        0      602 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/typings/misc.py
--rw-r--r--   0        0        0     1189 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/typings/outgoing.py
--rw-r--r--   0        0        0      117 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/utils/__init__.py
--rw-r--r--   0        0        0     1203 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/utils/classproperty.py
--rw-r--r--   0        0        0      745 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/warnings.py
--rw-r--r--   0        0        0     3766 2023-06-01 20:34:38.935827 mafic-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-02 11:14:58.780132 mafic-2.7.0/LICENSE
+-rw-r--r--   0        0        0     3315 2023-06-02 11:14:58.780132 mafic-2.7.0/README.md
+-rw-r--r--   0        0        0      886 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/__init__.py
+-rw-r--r--   0        0        0     3554 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/__libraries.py
+-rw-r--r--   0        0        0     1559 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/__main__.py
+-rw-r--r--   0        0        0     4490 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/errors.py
+-rw-r--r--   0        0        0     5617 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/events.py
+-rw-r--r--   0        0        0    27782 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/filter.py
+-rw-r--r--   0        0        0     7397 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/ip.py
+-rw-r--r--   0        0        0    42480 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/node.py
+-rw-r--r--   0        0        0    27377 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/player.py
+-rw-r--r--   0        0        0     1232 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/playlist.py
+-rw-r--r--   0        0        0      674 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/plugin.py
+-rw-r--r--   0        0        0    11716 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/pool.py
+-rw-r--r--   0        0        0        0 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/py.typed
+-rw-r--r--   0        0        0     3648 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/region.py
+-rw-r--r--   0        0        0     1031 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/search_type.py
+-rw-r--r--   0        0        0     3437 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/stats.py
+-rw-r--r--   0        0        0     5254 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/strategy.py
+-rw-r--r--   0        0        0     4797 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/track.py
+-rw-r--r--   0        0        0      747 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/type_variables.py
+-rw-r--r--   0        0        0      199 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/typings/__init__.py
+-rw-r--r--   0        0        0     2996 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/typings/common.py
+-rw-r--r--   0        0        0     4712 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/typings/http.py
+-rw-r--r--   0        0        0     2385 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/typings/incoming.py
+-rw-r--r--   0        0        0      602 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/typings/misc.py
+-rw-r--r--   0        0        0     1189 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/typings/outgoing.py
+-rw-r--r--   0        0        0      117 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/utils/__init__.py
+-rw-r--r--   0        0        0     1203 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/utils/classproperty.py
+-rw-r--r--   0        0        0      745 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/warnings.py
+-rw-r--r--   0        0        0     3766 2023-06-02 11:14:58.780132 mafic-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.7.0/PKG-INFO
```

### Comparing `mafic-2.6.0/LICENSE` & `mafic-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/README.md` & `mafic-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/__init__.py` & `mafic-2.7.0/mafic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .track import *
 from .warnings import *
 
 __title__ = "mafic"
 __author__ = "ooliver1"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present ooliver1"
-__version__ = "2.6.0"
+__version__ = "2.7.0"
 """The current version of mafic, using `PEP 440`_ format.
 
 .. _PEP 440: https://peps.python.org/pep-0440/
 """
 
 del __libraries
```

### Comparing `mafic-2.6.0/mafic/__libraries.py` & `mafic-2.7.0/mafic/__libraries.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/__main__.py` & `mafic-2.7.0/mafic/__main__.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/errors.py` & `mafic-2.7.0/mafic/errors.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/events.py` & `mafic-2.7.0/mafic/events.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/filter.py` & `mafic-2.7.0/mafic/filter.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/ip.py` & `mafic-2.7.0/mafic/ip.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/node.py` & `mafic-2.7.0/mafic/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -709,15 +709,24 @@
         if self._connect_task is not None:
             _log.debug("Cancelling connection task.", extra={"label": self._label})
             self._connect_task.cancel()
             self._connect_task = None
             _log.debug("Connection task cancelled.", extra={"label": self._label})
 
         _log.info("Node %s is now closed.", self._label, extra={"label": self._label})
+        self.cleanup()
+
+    def cleanup(self) -> None:
+        """Cleanup the node, as if it was never connected."""
         self._available = False
+        self._ws = None
+        self._ws_task = None
+        self._connect_task = None
+        self.__session = None
+        self._ready.clear()
 
     async def _ws_listener(self) -> None:
         """Listen for messages from the websocket."""
         backoff = ExponentialBackoff()
 
         if self._ws is None:
             _log.error(
```

### Comparing `mafic-2.6.0/mafic/player.py` & `mafic-2.7.0/mafic/player.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/playlist.py` & `mafic-2.7.0/mafic/playlist.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/plugin.py` & `mafic-2.7.0/mafic/plugin.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/pool.py` & `mafic-2.7.0/mafic/pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -183,14 +183,33 @@
             session=session,
             resume_key=resume_key,
             regions=regions,
             shard_ids=shard_ids,
             resuming_session_id=resuming_session_id,
         )
 
+        await self.add_node(node)
+        return node
+
+    async def add_node(self, node: Node[ClientT]) -> None:
+        """Add an existing node to this pool.
+
+        .. note::
+
+            You generally do not want this, use :meth:`create_node` instead.
+            This is used for after running :meth:`remove_node` to re-add the node
+            if it has been restarted.
+
+        .. versionadded:: 2.7
+
+        Parameters
+        ----------
+        node:
+            The node to add.
+        """
         # Add to dictionaries, creating a set or extending it if needed.
         if node.regions:
             for region in node.regions:
                 self._node_regions[region] = {
                     node,
                     *self._node_regions.get(region, set()),
                 }
@@ -198,19 +217,18 @@
         if node.shard_ids:
             for shard_id in node.shard_ids:
                 self._node_shards[shard_id] = {
                     node,
                     *self._node_shards.get(shard_id, set()),
                 }
 
-        _log.info("Created node, connecting it...", extra={"label": label})
+        _log.info("Created node, connecting it...", extra={"label": node.label})
         await node.connect()
 
-        self._nodes[label] = node
-        return node
+        self._nodes[node.label] = node
 
     async def remove_node(
         self, node: Node[ClientT] | str, *, transfer_players: bool = True
     ) -> None:
         """Remove a node from the pool.
 
         .. versionadded:: 2.6
```

### Comparing `mafic-2.6.0/mafic/region.py` & `mafic-2.7.0/mafic/region.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/search_type.py` & `mafic-2.7.0/mafic/search_type.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/stats.py` & `mafic-2.7.0/mafic/stats.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/strategy.py` & `mafic-2.7.0/mafic/strategy.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/track.py` & `mafic-2.7.0/mafic/track.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/type_variables.py` & `mafic-2.7.0/mafic/type_variables.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/typings/common.py` & `mafic-2.7.0/mafic/typings/common.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/typings/http.py` & `mafic-2.7.0/mafic/typings/http.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/typings/incoming.py` & `mafic-2.7.0/mafic/typings/incoming.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/typings/misc.py` & `mafic-2.7.0/mafic/typings/misc.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/typings/outgoing.py` & `mafic-2.7.0/mafic/typings/outgoing.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/utils/classproperty.py` & `mafic-2.7.0/mafic/utils/classproperty.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/mafic/warnings.py` & `mafic-2.7.0/mafic/warnings.py`

 * *Files identical despite different names*

### Comparing `mafic-2.6.0/pyproject.toml` & `mafic-2.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mafic"
-version = "2.6.0"
+version = "2.7.0"
 description = "A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord."
 authors = ["ooliver1 <oliverwilkes2006@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ooliver1/mafic"
 homepage = "https://github.com/ooliver1/mafic"
 keywords = [
```

### Comparing `mafic-2.6.0/PKG-INFO` & `mafic-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafic
-Version: 2.6.0
+Version: 2.7.0
 Summary: A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord.
 Home-page: https://github.com/ooliver1/mafic
 License: MIT
 Keywords: nextcord,disnake,discord,disnake.py,lavalink,lavalink.py,pycord,py-cord
 Author: ooliver1
 Author-email: oliverwilkes2006@icloud.com
 Requires-Python: >=3.8,<4.0
```

