# Comparing `tmp/mafic-2.7.0.tar.gz` & `tmp/mafic-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafic-2.7.0.tar", max compression
+gzip compressed data, was "mafic-2.8.0.tar", max compression
```

## Comparing `mafic-2.7.0.tar` & `mafic-2.8.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1070 2023-06-02 11:14:58.780132 mafic-2.7.0/LICENSE
--rw-r--r--   0        0        0     3315 2023-06-02 11:14:58.780132 mafic-2.7.0/README.md
--rw-r--r--   0        0        0      886 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/__init__.py
--rw-r--r--   0        0        0     3554 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/__libraries.py
--rw-r--r--   0        0        0     1559 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/__main__.py
--rw-r--r--   0        0        0     4490 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/errors.py
--rw-r--r--   0        0        0     5617 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/events.py
--rw-r--r--   0        0        0    27782 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/filter.py
--rw-r--r--   0        0        0     7397 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/ip.py
--rw-r--r--   0        0        0    42480 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/node.py
--rw-r--r--   0        0        0    27377 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/player.py
--rw-r--r--   0        0        0     1232 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/playlist.py
--rw-r--r--   0        0        0      674 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/plugin.py
--rw-r--r--   0        0        0    11716 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/pool.py
--rw-r--r--   0        0        0        0 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/py.typed
--rw-r--r--   0        0        0     3648 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/region.py
--rw-r--r--   0        0        0     1031 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/search_type.py
--rw-r--r--   0        0        0     3437 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/stats.py
--rw-r--r--   0        0        0     5254 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/strategy.py
--rw-r--r--   0        0        0     4797 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/track.py
--rw-r--r--   0        0        0      747 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/type_variables.py
--rw-r--r--   0        0        0      199 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/typings/__init__.py
--rw-r--r--   0        0        0     2996 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/typings/common.py
--rw-r--r--   0        0        0     4712 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/typings/http.py
--rw-r--r--   0        0        0     2385 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/typings/incoming.py
--rw-r--r--   0        0        0      602 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/typings/misc.py
--rw-r--r--   0        0        0     1189 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/typings/outgoing.py
--rw-r--r--   0        0        0      117 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/utils/__init__.py
--rw-r--r--   0        0        0     1203 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/utils/classproperty.py
--rw-r--r--   0        0        0      745 2023-06-02 11:14:58.780132 mafic-2.7.0/mafic/warnings.py
--rw-r--r--   0        0        0     3766 2023-06-02 11:14:58.780132 mafic-2.7.0/pyproject.toml
--rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-02 13:31:53.013765 mafic-2.8.0/LICENSE
+-rw-r--r--   0        0        0     3315 2023-06-02 13:31:53.013765 mafic-2.8.0/README.md
+-rw-r--r--   0        0        0      886 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/__init__.py
+-rw-r--r--   0        0        0     3554 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/__libraries.py
+-rw-r--r--   0        0        0     1559 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/__main__.py
+-rw-r--r--   0        0        0     4490 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/errors.py
+-rw-r--r--   0        0        0     5617 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/events.py
+-rw-r--r--   0        0        0    27782 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/filter.py
+-rw-r--r--   0        0        0     7397 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/ip.py
+-rw-r--r--   0        0        0    43682 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/node.py
+-rw-r--r--   0        0        0    27349 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/player.py
+-rw-r--r--   0        0        0     1232 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/playlist.py
+-rw-r--r--   0        0        0      674 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/plugin.py
+-rw-r--r--   0        0        0    12004 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/pool.py
+-rw-r--r--   0        0        0        0 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/py.typed
+-rw-r--r--   0        0        0     3648 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/region.py
+-rw-r--r--   0        0        0     1031 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/search_type.py
+-rw-r--r--   0        0        0     3437 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/stats.py
+-rw-r--r--   0        0        0     5254 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/strategy.py
+-rw-r--r--   0        0        0     4797 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/track.py
+-rw-r--r--   0        0        0      747 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/type_variables.py
+-rw-r--r--   0        0        0      199 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/typings/__init__.py
+-rw-r--r--   0        0        0     2996 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/typings/common.py
+-rw-r--r--   0        0        0     4712 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/typings/http.py
+-rw-r--r--   0        0        0     2385 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/typings/incoming.py
+-rw-r--r--   0        0        0      602 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/typings/misc.py
+-rw-r--r--   0        0        0     1189 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/typings/outgoing.py
+-rw-r--r--   0        0        0      117 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/utils/__init__.py
+-rw-r--r--   0        0        0     1203 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/utils/classproperty.py
+-rw-r--r--   0        0        0      745 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/warnings.py
+-rw-r--r--   0        0        0     3766 2023-06-02 13:31:53.013765 mafic-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.8.0/PKG-INFO
```

### Comparing `mafic-2.7.0/LICENSE` & `mafic-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/README.md` & `mafic-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/__init__.py` & `mafic-2.8.0/mafic/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .track import *
 from .warnings import *
 
 __title__ = "mafic"
 __author__ = "ooliver1"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present ooliver1"
-__version__ = "2.7.0"
+__version__ = "2.8.0"
 """The current version of mafic, using `PEP 440`_ format.
 
 .. _PEP 440: https://peps.python.org/pep-0440/
 """
 
 del __libraries
```

### Comparing `mafic-2.7.0/mafic/__libraries.py` & `mafic-2.8.0/mafic/__libraries.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/__main__.py` & `mafic-2.8.0/mafic/__main__.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/errors.py` & `mafic-2.8.0/mafic/errors.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/events.py` & `mafic-2.8.0/mafic/events.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/filter.py` & `mafic-2.8.0/mafic/filter.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/ip.py` & `mafic-2.8.0/mafic/ip.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/node.py` & `mafic-2.8.0/mafic/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,15 @@
         "_resuming_session_id",
         "_session_id",
         "_stats",
         "_version",
         "_ws",
         "_ws_uri",
         "_ws_task",
+        "_event_queue",
         "regions",
         "shard_ids",
     )
 
     def __init__(
         self,
         *,
@@ -249,14 +250,16 @@
 
         self._msg_tasks: set[Task[None]] = set()
         self._connect_task: Task[None] | None = None
 
         self._checked_version: bool = False
         self._version: int = 3
 
+        self._event_queue: Event = Event()
+
     @property
     def host(self) -> str:
         """The host of the node."""
         return self._host
 
     @property
     def port(self) -> int:
@@ -567,22 +570,29 @@
                 self._rest_uri,
                 e,
                 extra={"label": self._label},
             )
             raise
 
     async def connect(
-        self, *, backoff: ExponentialBackoff[Literal[False]] | None = None
+        self,
+        *,
+        backoff: ExponentialBackoff[Literal[False]] | None = None,
+        player_cls: type[Player[ClientT]] | None = None,
     ) -> None:
         """Connect to the node.
 
         Parameters
         ----------
         backoff:
             The backoff to use when reconnecting.
+        player_cls:
+            The player class to use for the node when resuming.
+
+            .. versionadded:: 2.8
 
         Raises
         ------
         NodeAlreadyConnected
             If the node is already connected.
         asyncio.TimeoutError
             If the connection times out.
@@ -669,15 +679,16 @@
                 extra={"label": self._label},
             )
             raise
         else:
             _log.info(
                 "Node %s is now available.", self._label, extra={"label": self._label}
             )
-            await self.sync_players()
+            await self.sync_players(player_cls=player_cls)
+            self._event_queue.set()
             self._available = True
             self._client.dispatch("node_ready", self)
 
     async def close(self) -> None:
         """Close the node.
 
         This will disconnect the websocket and close the session.
@@ -719,14 +730,15 @@
         """Cleanup the node, as if it was never connected."""
         self._available = False
         self._ws = None
         self._ws_task = None
         self._connect_task = None
         self.__session = None
         self._ready.clear()
+        self._event_queue.clear()
 
     async def _ws_listener(self) -> None:
         """Listen for messages from the websocket."""
         backoff = ExponentialBackoff()
 
         if self._ws is None:
             _log.error(
@@ -785,14 +797,17 @@
         Parameters
         ----------
         data:
             The data to handle.
         """
         _log.debug("Event data: %s", data)
         _log.debug("Received event with op %s", data["op"])
+        # Queue up events like "playerUpdate" until we receive "ready" and resumed.
+        if data["op"] != "ready":
+            await self._event_queue.wait()
 
         if data["op"] == "playerUpdate":
             guild_id = int(data["guildId"])
             player = self.get_player(guild_id)
 
             if player is None:
                 if data["state"]["connected"] is True:
@@ -873,15 +888,17 @@
                     guild.id,
                     extra={"label": self._label},
                 )
                 await player.disconnect(force=True)
                 return
 
             _log.error(
-                "Could not find player for guild %s, discarding event.", data["guildId"]
+                "Could not find player for guild %s, discarding event.",
+                data["guildId"],
+                extra={"label": self._label},
             )
             return
 
         player.dispatch_event(data)
 
     def voice_update(
         self,
@@ -1279,23 +1296,30 @@
             "POST", "routeplanner/free/address", json={"address": address}
         )
 
     async def unmark_all_addresses(self) -> None:
         """Unmark all failed addresses so they can be used again."""
         await self.__request("POST", "routeplanner/free/all")
 
-    async def _add_unknown_player(self, player_id: int, state: PlayerPayload) -> None:
+    async def _add_unknown_player(
+        self,
+        player_id: int,
+        state: PlayerPayload,
+        cls: type[Player[ClientT]] | None = None,
+    ) -> None:
         """Add an unknown player to the node.
 
         Parameters
         ----------
         player_id:
             The guild ID of the player.
         state:
             The state of the player.
+        cls:
+            The class of the player to use.
         """
         guild = self.client.get_guild(player_id)
         if guild is None:
             guild = await self.client.fetch_guild(player_id)
 
         voice_state = guild.me.voice
 
@@ -1306,49 +1330,63 @@
 
         if channel is None:
             return
 
         # Circular, pool -> node -> player -> pool
         from .player import Player
 
-        player = Player(self.client, channel)
+        player = (cls or Player)(self.client, channel)
 
         player.set_state(state)
+        player._node = self  # pyright: ignore[reportPrivateUsage]
 
         self._players[player_id] = player
+        key, _ = player.channel._get_voice_client_key()  # pyright: ignore
+        self.client._connection._add_voice_client(key, player)  # pyright: ignore
 
     async def _remove_unknown_player(self, player_id: int) -> None:
         """Remove an unknown player from the node.
 
         Parameters
         ----------
         player_id:
             The guild ID of the player.
         """
         await self._players[player_id].disconnect(force=True)
         self.remove_player(player_id)
 
-    async def sync_players(self) -> None:
+    async def sync_players(
+        self, player_cls: type[Player[ClientT]] | None = None
+    ) -> None:
         """Sync the players with the node.
 
         .. note::
 
             This method is called automatically when the client is ready.
             You should not need to call this method yourself.
+
+        Parameters
+        ----------
+        player_cls:
+            The class of the player to use.
+
+            .. versionadded:: 2.8
         """
         players: list[PlayerPayload] = await self.__request(
             "GET", f"sessions/{self._session_id}/players"
         )
         actual_players = {int(player["guildId"]): player for player in players}
         actual_player_ids = set(actual_players.keys())
         expected_player_ids = set(self._players.keys())
 
         await gather(
             *(
-                self._add_unknown_player(player_id, actual_players[player_id])
+                self._add_unknown_player(
+                    player_id, actual_players[player_id], cls=player_cls
+                )
                 for player_id in actual_player_ids - expected_player_ids
             ),
             *(
                 self._remove_unknown_player(player_id)
                 for player_id in expected_player_ids - actual_player_ids
             ),
         )
```

### Comparing `mafic-2.7.0/mafic/player.py` & `mafic-2.8.0/mafic/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
         .. note::
 
             This is used internally to set the state of the player.
             You should not need to use this.
         """
         self._session_id = state["voice"]["sessionId"]
-        self._ping = state["voice"]["ping"]
+        self._ping = state["voice"].get("ping", -1)
         self._current = (
             Track.from_data_with_info(state["track"]) if state["track"] else None
         )
         self._filters = OrderedDict({"RESUME": Filter.from_payload(state["filters"])})
         self._paused = state["paused"]
         self._server_state = {
             "token": state["voice"]["token"],
@@ -416,14 +416,15 @@
             Whether to deafen the bot on connect.
         """
         if not isinstance(self.channel, (VoiceChannel, StageChannel)):
             msg = "Voice channel must be a VoiceChannel or StageChannel."
             raise TypeError(msg)
 
         if not NodePool.nodes:  # pyright: ignore
+            self.cleanup()
             raise NoNodesAvailable
 
         _log.debug("Connecting to voice channel %s", self.channel.id)
 
         await self.channel.guild.change_voice_state(
             channel=self.channel, self_mute=self_mute, self_deaf=self_deaf
         )
@@ -642,19 +643,16 @@
             filter=filter,
             no_replace=not replace,
         )
 
         if data["track"]:
             self._current = Track.from_data_with_info(data["track"])
 
-        if data["volume"]:
-            self._volume = data["volume"]
-
-        if data["paused"]:
-            self._paused = data["paused"]
+        self._volume = data["volume"]
+        self._paused = data["paused"]
 
     async def play(
         self,
         track: Track | str,
         /,
         *,
         start_time: int | None = None,
```

### Comparing `mafic-2.7.0/mafic/playlist.py` & `mafic-2.8.0/mafic/playlist.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/plugin.py` & `mafic-2.8.0/mafic/plugin.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/pool.py` & `mafic-2.8.0/mafic/pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .utils import classproperty
 
 if TYPE_CHECKING:
     from typing import ClassVar
 
     import aiohttp
 
+    from .player import Player
     from .region import Group, Region, VoiceRegion
 
 
 T = TypeVar("T")
 __all__ = ("NodePool",)
 
 _log = getLogger(__name__)
@@ -106,14 +107,15 @@
         heartbeat: int = 30,
         timeout: float = 10,
         session: aiohttp.ClientSession | None = None,
         resume_key: str | None = None,
         regions: Sequence[Group | Region | VoiceRegion] | None = None,
         shard_ids: Sequence[int] | None = None,
         resuming_session_id: str | None = None,
+        player_cls: type[Player[ClientT]] | None = None,
     ) -> Node[ClientT]:
         r"""Create a node and connect it.
 
         The parameters here relate to :class:`Node`.
 
         Parameters
         ----------
@@ -152,14 +154,18 @@
 
             This should be stored from :func:`~mafic.on_node_ready` with
             :attr:`session_id` to resume the session and gain control of the players.
             If the node is not resuming, players will be destroyed if Lavalink loses
             connection to us.
 
             .. versionadded:: 2.2
+        player_cls:
+            The player class to use for this node when resuming.
+
+            .. versionadded:: 2.8
 
         Returns
         -------
         :class:`Node`
             The created node.
 
         Raises
@@ -183,32 +189,38 @@
             session=session,
             resume_key=resume_key,
             regions=regions,
             shard_ids=shard_ids,
             resuming_session_id=resuming_session_id,
         )
 
-        await self.add_node(node)
+        await self.add_node(node, player_cls=player_cls)
         return node
 
-    async def add_node(self, node: Node[ClientT]) -> None:
+    async def add_node(
+        self, node: Node[ClientT], *, player_cls: type[Player[ClientT]] | None = None
+    ) -> None:
         """Add an existing node to this pool.
 
         .. note::
 
             You generally do not want this, use :meth:`create_node` instead.
             This is used for after running :meth:`remove_node` to re-add the node
             if it has been restarted.
 
         .. versionadded:: 2.7
 
         Parameters
         ----------
         node:
             The node to add.
+        player:
+            The player class to use for this node when resuming.
+
+            .. versionadded:: 2.8
         """
         # Add to dictionaries, creating a set or extending it if needed.
         if node.regions:
             for region in node.regions:
                 self._node_regions[region] = {
                     node,
                     *self._node_regions.get(region, set()),
@@ -218,15 +230,15 @@
             for shard_id in node.shard_ids:
                 self._node_shards[shard_id] = {
                     node,
                     *self._node_shards.get(shard_id, set()),
                 }
 
         _log.info("Created node, connecting it...", extra={"label": node.label})
-        await node.connect()
+        await node.connect(player_cls=player_cls)
 
         self._nodes[node.label] = node
 
     async def remove_node(
         self, node: Node[ClientT] | str, *, transfer_players: bool = True
     ) -> None:
         """Remove a node from the pool.
@@ -251,16 +263,14 @@
             for shard_id in node.shard_ids:
                 self._node_shards[shard_id].remove(node)
 
         # Remove prematurely so it is not chosen.
         del self._nodes[node.label]
 
         if transfer_players:
-            if TYPE_CHECKING:
-                from .player import Player
 
             async def transfer_player(player: Player[ClientT]) -> None:
                 try:
                     target = self.get_node(
                         guild_id=player.guild.id,
                         endpoint=player.endpoint,  # pyright: ignore[reportPrivateUsage]
                     )
@@ -273,16 +283,14 @@
                         extra={"label": node.label},
                     )
                     await player.destroy()
 
             tasks = [transfer_player(player) for player in node.players]
             await asyncio.gather(*tasks)
         else:
-            if TYPE_CHECKING:
-                from .player import Player
 
             async def destroy_player(player: Player[ClientT]) -> None:
                 _log.debug(
                     "Destroying player %d due to node removal...",
                     player.guild.id,
                     extra={"label": node.label},
                 )
```

### Comparing `mafic-2.7.0/mafic/region.py` & `mafic-2.8.0/mafic/region.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/search_type.py` & `mafic-2.8.0/mafic/search_type.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/stats.py` & `mafic-2.8.0/mafic/stats.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/strategy.py` & `mafic-2.8.0/mafic/strategy.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/track.py` & `mafic-2.8.0/mafic/track.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/type_variables.py` & `mafic-2.8.0/mafic/type_variables.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/typings/common.py` & `mafic-2.8.0/mafic/typings/common.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/typings/http.py` & `mafic-2.8.0/mafic/typings/http.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/typings/incoming.py` & `mafic-2.8.0/mafic/typings/incoming.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/typings/misc.py` & `mafic-2.8.0/mafic/typings/misc.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/typings/outgoing.py` & `mafic-2.8.0/mafic/typings/outgoing.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/utils/classproperty.py` & `mafic-2.8.0/mafic/utils/classproperty.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/mafic/warnings.py` & `mafic-2.8.0/mafic/warnings.py`

 * *Files identical despite different names*

### Comparing `mafic-2.7.0/pyproject.toml` & `mafic-2.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mafic"
-version = "2.7.0"
+version = "2.8.0"
 description = "A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord."
 authors = ["ooliver1 <oliverwilkes2006@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ooliver1/mafic"
 homepage = "https://github.com/ooliver1/mafic"
 keywords = [
```

### Comparing `mafic-2.7.0/PKG-INFO` & `mafic-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafic
-Version: 2.7.0
+Version: 2.8.0
 Summary: A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord.
 Home-page: https://github.com/ooliver1/mafic
 License: MIT
 Keywords: nextcord,disnake,discord,disnake.py,lavalink,lavalink.py,pycord,py-cord
 Author: ooliver1
 Author-email: oliverwilkes2006@icloud.com
 Requires-Python: >=3.8,<4.0
```

