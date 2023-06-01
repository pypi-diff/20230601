# Comparing `tmp/mafic-2.5.0.tar.gz` & `tmp/mafic-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafic-2.5.0.tar", max compression
+gzip compressed data, was "mafic-2.6.0.tar", max compression
```

## Comparing `mafic-2.5.0.tar` & `mafic-2.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1070 2023-05-31 17:06:46.980485 mafic-2.5.0/LICENSE
--rw-r--r--   0        0        0     3315 2023-05-31 17:06:46.980485 mafic-2.5.0/README.md
--rw-r--r--   0        0        0      886 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/__init__.py
--rw-r--r--   0        0        0     3554 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/__libraries.py
--rw-r--r--   0        0        0     1559 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/__main__.py
--rw-r--r--   0        0        0     4490 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/errors.py
--rw-r--r--   0        0        0     5617 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/events.py
--rw-r--r--   0        0        0    27782 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/filter.py
--rw-r--r--   0        0        0     7397 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/ip.py
--rw-r--r--   0        0        0    40202 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/node.py
--rw-r--r--   0        0        0    25792 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/player.py
--rw-r--r--   0        0        0     1232 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/playlist.py
--rw-r--r--   0        0        0      674 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/plugin.py
--rw-r--r--   0        0        0     8715 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/pool.py
--rw-r--r--   0        0        0        0 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/py.typed
--rw-r--r--   0        0        0     3648 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/region.py
--rw-r--r--   0        0        0     1031 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/search_type.py
--rw-r--r--   0        0        0     3437 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/stats.py
--rw-r--r--   0        0        0     5254 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/strategy.py
--rw-r--r--   0        0        0     4797 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/track.py
--rw-r--r--   0        0        0      747 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/type_variables.py
--rw-r--r--   0        0        0      199 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/typings/__init__.py
--rw-r--r--   0        0        0     2996 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/typings/common.py
--rw-r--r--   0        0        0     4712 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/typings/http.py
--rw-r--r--   0        0        0     2385 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/typings/incoming.py
--rw-r--r--   0        0        0      602 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/typings/misc.py
--rw-r--r--   0        0        0     1189 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/typings/outgoing.py
--rw-r--r--   0        0        0      117 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/utils/__init__.py
--rw-r--r--   0        0        0     1203 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/utils/classproperty.py
--rw-r--r--   0        0        0      745 2023-05-31 17:06:46.980485 mafic-2.5.0/mafic/warnings.py
--rw-r--r--   0        0        0     3766 2023-05-31 17:06:46.980485 mafic-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-01 20:34:38.935827 mafic-2.6.0/LICENSE
+-rw-r--r--   0        0        0     3315 2023-06-01 20:34:38.935827 mafic-2.6.0/README.md
+-rw-r--r--   0        0        0      886 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/__init__.py
+-rw-r--r--   0        0        0     3554 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/__libraries.py
+-rw-r--r--   0        0        0     1559 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/__main__.py
+-rw-r--r--   0        0        0     4490 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/errors.py
+-rw-r--r--   0        0        0     5617 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/events.py
+-rw-r--r--   0        0        0    27782 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/filter.py
+-rw-r--r--   0        0        0     7397 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/ip.py
+-rw-r--r--   0        0        0    42218 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/node.py
+-rw-r--r--   0        0        0    27377 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/player.py
+-rw-r--r--   0        0        0     1232 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/playlist.py
+-rw-r--r--   0        0        0      674 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/plugin.py
+-rw-r--r--   0        0        0    11224 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/pool.py
+-rw-r--r--   0        0        0        0 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/py.typed
+-rw-r--r--   0        0        0     3648 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/region.py
+-rw-r--r--   0        0        0     1031 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/search_type.py
+-rw-r--r--   0        0        0     3437 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/stats.py
+-rw-r--r--   0        0        0     5254 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/strategy.py
+-rw-r--r--   0        0        0     4797 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/track.py
+-rw-r--r--   0        0        0      747 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/type_variables.py
+-rw-r--r--   0        0        0      199 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/typings/__init__.py
+-rw-r--r--   0        0        0     2996 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/typings/common.py
+-rw-r--r--   0        0        0     4712 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/typings/http.py
+-rw-r--r--   0        0        0     2385 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/typings/incoming.py
+-rw-r--r--   0        0        0      602 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/typings/misc.py
+-rw-r--r--   0        0        0     1189 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/typings/outgoing.py
+-rw-r--r--   0        0        0      117 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/utils/__init__.py
+-rw-r--r--   0        0        0     1203 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/utils/classproperty.py
+-rw-r--r--   0        0        0      745 2023-06-01 20:34:38.935827 mafic-2.6.0/mafic/warnings.py
+-rw-r--r--   0        0        0     3766 2023-06-01 20:34:38.935827 mafic-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.6.0/PKG-INFO
```

### Comparing `mafic-2.5.0/LICENSE` & `mafic-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/README.md` & `mafic-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/__init__.py` & `mafic-2.6.0/mafic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .track import *
 from .warnings import *
 
 __title__ = "mafic"
 __author__ = "ooliver1"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present ooliver1"
-__version__ = "2.5.0"
+__version__ = "2.6.0"
 """The current version of mafic, using `PEP 440`_ format.
 
 .. _PEP 440: https://peps.python.org/pep-0440/
 """
 
 del __libraries
```

### Comparing `mafic-2.5.0/mafic/__libraries.py` & `mafic-2.6.0/mafic/__libraries.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/__main__.py` & `mafic-2.6.0/mafic/__main__.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/errors.py` & `mafic-2.6.0/mafic/errors.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/events.py` & `mafic-2.6.0/mafic/events.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/filter.py` & `mafic-2.6.0/mafic/filter.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/ip.py` & `mafic-2.6.0/mafic/ip.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/node.py` & `mafic-2.6.0/mafic/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -418,14 +418,37 @@
         Returns
         -------
         :data:`~typing.Optional`\[:class:`Player`]
             The player for the guild, if found.
         """
         return self._players.get(guild_id)
 
+    async def fetch_player(self, guild_id: int) -> PlayerPayload:
+        """Fetch player data from the node.
+
+        .. note::
+
+            This is an API call. Usually you should use :meth:`get_player` instead.
+
+        .. versionadded:: 2.6
+
+        Parameters
+        ----------
+        guild_id:
+            The guild ID to fetch the player for.
+
+        Returns
+        -------
+        :class:`dict`
+            The player data for the guild.
+        """
+        return await self.__request(
+            "GET", f"sessions/{self._session_id}/players/{guild_id}"
+        )
+
     def add_player(self, guild_id: int, player: Player[ClientT]) -> None:
         """Add a player to the node.
 
         Parameters
         ----------
         guild_id:
             The guild ID to add the player for.
@@ -650,14 +673,52 @@
             _log.info(
                 "Node %s is now available.", self._label, extra={"label": self._label}
             )
             await self.sync_players()
             self._available = True
             self._client.dispatch("node_ready", self)
 
+    async def close(self) -> None:
+        """Close the node.
+
+        This will disconnect the websocket and close the session.
+
+        .. versionadded:: 2.6
+        """
+        if self._ws is not None:
+            _log.debug("Closing websocket.", extra={"label": self._label})
+            await self._ws.close()
+            self._ws = None
+            _log.debug("Websocket closed.", extra={"label": self._label})
+
+        if self.__session is not None:
+            _log.debug("Closing session.", extra={"label": self._label})
+            await self.__session.close()
+            self.__session = None
+            _log.debug("Session closed.", extra={"label": self._label})
+
+        if self._ws_task is not None:
+            _log.debug(
+                "Cancelling websocket listener task.", extra={"label": self._label}
+            )
+            self._ws_task.cancel()
+            self._ws_task = None
+            _log.debug(
+                "Websocket listener task cancelled.", extra={"label": self._label}
+            )
+
+        if self._connect_task is not None:
+            _log.debug("Cancelling connection task.", extra={"label": self._label})
+            self._connect_task.cancel()
+            self._connect_task = None
+            _log.debug("Connection task cancelled.", extra={"label": self._label})
+
+        _log.info("Node %s is now closed.", self._label, extra={"label": self._label})
+        self._available = False
+
     async def _ws_listener(self) -> None:
         """Listen for messages from the websocket."""
         backoff = ExponentialBackoff()
 
         if self._ws is None:
             _log.error(
                 "No websocket was found, aborting listener.",
```

### Comparing `mafic-2.5.0/mafic/player.py` & `mafic-2.6.0/mafic/player.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         self.channel: Connectable = channel
 
         if not isinstance(self.channel, GuildChannel):
             msg = "Voice channel must be a GuildChannel."
             raise TypeError(msg)
 
         self.guild: Guild = self.channel.guild
+        self.endpoint: str | None = None
 
         self._node = node
 
         self._guild_id: int = self.guild.id
         self._session_id: str | None = None
         self._server_state: VoiceServerUpdatePayload | None = None
         self._connected: bool = False
@@ -380,14 +381,15 @@
                 self._node.label,
                 extra={"guild": self._guild_id},
             )
 
         self._node.add_player(self._guild_id, self)
 
         self._guild_id = int(data["guild_id"])
+        self._endpoint = data["endpoint"]
         self._server_state = data
 
         await self._dispatch_player_update()
 
         self._voice_server_update_event.set()
 
     async def connect(
@@ -474,14 +476,62 @@
         self._paused = False
         self._ping = 0
         self._channel = None
         self._connected = False
 
         return super().cleanup()
 
+    async def transfer_to(self, node: Node[ClientT]) -> None:
+        """Transfer the player to a new node.
+
+        Parameters
+        ----------
+        node:
+            The node to transfer to.
+        """
+        if self._node is None:
+            raise PlayerNotConnected
+
+        if self._node == node:
+            return
+
+        state = await self._node.fetch_player(self.guild.id)
+
+        # Remove from the current node, but no need to destroy.
+        self._node.remove_player(self.guild.id)
+
+        old_node = self._node
+        self._node = node
+        self._node.add_player(self.guild.id, self)
+
+        if self._session_id is None or self._server_state is None:
+            msg = "Cannot transfer player with session data."
+            raise RuntimeError(msg)
+
+        # We need to update the voice server as the endpoint may have changed.
+        await self._node.voice_update(
+            guild_id=self._guild_id,
+            session_id=self._session_id,
+            data=self._server_state,
+        )
+
+        # Needed so .update does not fail.
+        self._connected = True
+        # Update player with all other state.
+        # Position, filters, track, etc.
+        await self.update(
+            track=self._current,
+            position=self.position,
+            volume=state["volume"],
+            pause=self._paused,
+            filter=reduce(or_, self._filters.values()) if self._filters else Filter(),
+        )
+
+        await old_node.destroy(guild_id=self.guild.id)
+
     async def destroy(self) -> None:
         """Destroy the player.
 
         This will disconnect the player and remove it from the node.
         """
         _log.debug(
             "Disconnecting player and destroying client.",
```

### Comparing `mafic-2.5.0/mafic/playlist.py` & `mafic-2.6.0/mafic/playlist.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/plugin.py` & `mafic-2.6.0/mafic/plugin.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/pool.py` & `mafic-2.6.0/mafic/pool.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 r"""A module containing a :class:`NodePool`, used to manage :class:`Node`\s."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
+import asyncio
 from collections.abc import Sequence
 from functools import partial
 from logging import getLogger
 from random import choice
 from typing import TYPE_CHECKING, Any, Generic, List, TypeVar, Union, cast
 
-from .errors import NoNodesAvailable
+from .errors import NoNodesAvailable, PlayerNotConnected
 from .node import Node
 from .strategy import Strategy, StrategyCallable, call_strategy
 from .type_variables import ClientT
 from .utils import classproperty
 
 if TYPE_CHECKING:
     from typing import ClassVar
@@ -203,14 +204,89 @@
 
         _log.info("Created node, connecting it...", extra={"label": label})
         await node.connect()
 
         self._nodes[label] = node
         return node
 
+    async def remove_node(
+        self, node: Node[ClientT] | str, *, transfer_players: bool = True
+    ) -> None:
+        """Remove a node from the pool.
+
+        .. versionadded:: 2.6
+
+        Parameters
+        ----------
+        node:
+            The node to remove.
+        transfer_players:
+            Whether to transfer players to other nodes or destroy them.
+        """
+        if isinstance(node, str):
+            node = self._nodes[node]
+
+        if node.regions:
+            for region in node.regions:
+                self._node_regions[region].remove(node)
+
+        if node.shard_ids:
+            for shard_id in node.shard_ids:
+                self._node_shards[shard_id].remove(node)
+
+        # Remove prematurely so it is not chosen.
+        del self._nodes[node.label]
+
+        if transfer_players:
+            if TYPE_CHECKING:
+                from .player import Player
+
+            async def transfer_player(player: Player[ClientT]) -> None:
+                try:
+                    target = self.get_node(
+                        guild_id=player.guild.id,
+                        endpoint=player.endpoint,  # pyright: ignore[reportPrivateUsage]
+                    )
+                    await player.transfer_to(target)
+                except (RuntimeError, NoNodesAvailable, PlayerNotConnected):
+                    _log.error(
+                        "Failed to transfer player %d, destroying it...",
+                        player.guild.id,
+                        exc_info=True,
+                        extra={"label": node.label},
+                    )
+                    await player.destroy()
+
+            tasks = [transfer_player(player) for player in node.players]
+            await asyncio.gather(*tasks)
+        else:
+            if TYPE_CHECKING:
+                from .player import Player
+
+            async def destroy_player(player: Player[ClientT]) -> None:
+                _log.debug(
+                    "Destroying player %d due to node removal...",
+                    player.guild.id,
+                    extra={"label": node.label},
+                )
+                await player.destroy()
+
+            tasks = [destroy_player(player) for player in node.players]
+            await asyncio.gather(*tasks)
+
+        await node.close()
+
+    async def close(self) -> None:
+        """Close all nodes in the pool.
+
+        .. versionadded:: 2.6
+        """
+        for node in self._nodes.values():
+            await node.close()
+
     @classmethod
     def get_node(
         cls,
         *,
         guild_id: str | int,
         endpoint: str | None,
         strategies: StrategyList[ClientT] | None = None,
```

### Comparing `mafic-2.5.0/mafic/region.py` & `mafic-2.6.0/mafic/region.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/search_type.py` & `mafic-2.6.0/mafic/search_type.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/stats.py` & `mafic-2.6.0/mafic/stats.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/strategy.py` & `mafic-2.6.0/mafic/strategy.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/track.py` & `mafic-2.6.0/mafic/track.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/type_variables.py` & `mafic-2.6.0/mafic/type_variables.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/typings/common.py` & `mafic-2.6.0/mafic/typings/common.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/typings/http.py` & `mafic-2.6.0/mafic/typings/http.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/typings/incoming.py` & `mafic-2.6.0/mafic/typings/incoming.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/typings/misc.py` & `mafic-2.6.0/mafic/typings/misc.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/typings/outgoing.py` & `mafic-2.6.0/mafic/typings/outgoing.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/utils/classproperty.py` & `mafic-2.6.0/mafic/utils/classproperty.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/mafic/warnings.py` & `mafic-2.6.0/mafic/warnings.py`

 * *Files identical despite different names*

### Comparing `mafic-2.5.0/pyproject.toml` & `mafic-2.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mafic"
-version = "2.5.0"
+version = "2.6.0"
 description = "A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord."
 authors = ["ooliver1 <oliverwilkes2006@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ooliver1/mafic"
 homepage = "https://github.com/ooliver1/mafic"
 keywords = [
```

### Comparing `mafic-2.5.0/PKG-INFO` & `mafic-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafic
-Version: 2.5.0
+Version: 2.6.0
 Summary: A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord.
 Home-page: https://github.com/ooliver1/mafic
 License: MIT
 Keywords: nextcord,disnake,discord,disnake.py,lavalink,lavalink.py,pycord,py-cord
 Author: ooliver1
 Author-email: oliverwilkes2006@icloud.com
 Requires-Python: >=3.8,<4.0
```

