# Comparing `tmp/aio_pika-9.0.7.tar.gz` & `tmp/aio_pika-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_pika-9.0.7.tar", max compression
+gzip compressed data, was "aio_pika-9.1.0.tar", max compression
```

## Comparing `aio_pika-9.0.7.tar` & `aio_pika-9.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     7585 2023-02-18 21:11:58.825819 aio_pika-9.0.7/README.rst
--rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.0.7/aio_pika/__init__.py
--rw-r--r--   0        0        0    24987 2023-05-11 12:01:38.489759 aio_pika-9.0.7/aio_pika/abc.py
--rw-r--r--   0        0        0    13901 2023-05-11 12:01:38.490719 aio_pika-9.0.7/aio_pika/channel.py
--rw-r--r--   0        0        0    10907 2023-05-11 12:01:38.491492 aio_pika-9.0.7/aio_pika/connection.py
--rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.0.7/aio_pika/exceptions.py
--rw-r--r--   0        0        0     6411 2023-05-11 12:01:38.493435 aio_pika-9.0.7/aio_pika/exchange.py
--rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.0.7/aio_pika/log.py
--rw-r--r--   0        0        0    19662 2023-05-11 12:01:38.494544 aio_pika-9.0.7/aio_pika/message.py
--rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.0.7/aio_pika/patterns/__init__.py
--rw-r--r--   0        0        0     1345 2023-05-11 12:01:38.495119 aio_pika-9.0.7/aio_pika/patterns/base.py
--rw-r--r--   0        0        0     6249 2023-05-11 12:01:38.495943 aio_pika-9.0.7/aio_pika/patterns/master.py
--rw-r--r--   0        0        0    14375 2023-05-11 12:01:38.496979 aio_pika-9.0.7/aio_pika/patterns/rpc.py
--rw-r--r--   0        0        0     4352 2023-05-11 12:01:38.497963 aio_pika-9.0.7/aio_pika/pool.py
--rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.0.7/aio_pika/py.typed
--rw-r--r--   0        0        0    16056 2023-05-11 12:01:38.499489 aio_pika-9.0.7/aio_pika/queue.py
--rw-r--r--   0        0        0     6980 2023-05-11 12:01:38.502999 aio_pika-9.0.7/aio_pika/robust_channel.py
--rw-r--r--   0        0        0    10367 2023-05-11 12:01:38.505100 aio_pika-9.0.7/aio_pika/robust_connection.py
--rw-r--r--   0        0        0     2727 2023-05-11 12:01:38.505793 aio_pika-9.0.7/aio_pika/robust_exchange.py
--rw-r--r--   0        0        0     4656 2023-05-11 12:01:38.506997 aio_pika-9.0.7/aio_pika/robust_queue.py
--rw-r--r--   0        0        0     7339 2023-05-11 12:01:38.508241 aio_pika-9.0.7/aio_pika/tools.py
--rw-r--r--   0        0        0     1924 2023-05-11 12:01:38.509992 aio_pika-9.0.7/aio_pika/transaction.py
--rw-r--r--   0        0        0     3264 2023-05-11 15:25:23.113063 aio_pika-9.0.7/pyproject.toml
--rw-r--r--   0        0        0     9488 1970-01-01 00:00:00.000000 aio_pika-9.0.7/PKG-INFO
+-rw-r--r--   0        0        0     7585 2023-02-18 21:11:58.825819 aio_pika-9.1.0/README.rst
+-rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.1.0/aio_pika/__init__.py
+-rw-r--r--   0        0        0    24756 2023-06-01 15:55:44.119921 aio_pika-9.1.0/aio_pika/abc.py
+-rw-r--r--   0        0        0    14701 2023-06-01 15:55:44.121581 aio_pika-9.1.0/aio_pika/channel.py
+-rw-r--r--   0        0        0    10892 2023-06-01 15:55:44.123355 aio_pika-9.1.0/aio_pika/connection.py
+-rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.1.0/aio_pika/exceptions.py
+-rw-r--r--   0        0        0     6730 2023-06-01 15:55:44.124351 aio_pika-9.1.0/aio_pika/exchange.py
+-rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.1.0/aio_pika/log.py
+-rw-r--r--   0        0        0    19763 2023-06-01 15:55:44.125260 aio_pika-9.1.0/aio_pika/message.py
+-rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.1.0/aio_pika/patterns/__init__.py
+-rw-r--r--   0        0        0     1427 2023-06-01 15:55:44.126438 aio_pika-9.1.0/aio_pika/patterns/base.py
+-rw-r--r--   0        0        0     6208 2023-06-01 15:55:44.128054 aio_pika-9.1.0/aio_pika/patterns/master.py
+-rw-r--r--   0        0        0    14343 2023-06-01 15:55:44.129787 aio_pika-9.1.0/aio_pika/patterns/rpc.py
+-rw-r--r--   0        0        0     4177 2023-06-01 15:55:44.130894 aio_pika-9.1.0/aio_pika/pool.py
+-rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.1.0/aio_pika/py.typed
+-rw-r--r--   0        0        0    16598 2023-06-01 15:55:44.131780 aio_pika-9.1.0/aio_pika/queue.py
+-rw-r--r--   0        0        0     8219 2023-06-01 15:55:44.133275 aio_pika-9.1.0/aio_pika/robust_channel.py
+-rw-r--r--   0        0        0    10445 2023-06-01 15:55:44.135097 aio_pika-9.1.0/aio_pika/robust_connection.py
+-rw-r--r--   0        0        0     2889 2023-06-01 15:55:44.136022 aio_pika-9.1.0/aio_pika/robust_exchange.py
+-rw-r--r--   0        0        0     4883 2023-06-01 15:55:44.136895 aio_pika-9.1.0/aio_pika/robust_queue.py
+-rw-r--r--   0        0        0     8639 2023-06-01 15:55:44.138218 aio_pika-9.1.0/aio_pika/tools.py
+-rw-r--r--   0        0        0     2065 2023-06-01 15:55:44.139689 aio_pika-9.1.0/aio_pika/transaction.py
+-rw-r--r--   0        0        0     3269 2023-06-01 15:55:44.144534 aio_pika-9.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9488 1970-01-01 00:00:00.000000 aio_pika-9.1.0/PKG-INFO
```

### Comparing `aio_pika-9.0.7/README.rst` & `aio_pika-9.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.7/aio_pika/__init__.py` & `aio_pika-9.1.0/aio_pika/__init__.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.7/aio_pika/abc.py` & `aio_pika-9.1.0/aio_pika/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from functools import singledispatch
 from types import TracebackType
 from typing import (
     Any, AsyncContextManager, AsyncIterable, Awaitable, Callable, Dict,
     Generator, Iterator, Optional, Type, TypeVar, Union, overload,
 )
 
+
 if sys.version_info >= (3, 8):
     from typing import Literal, TypedDict
 else:
     from typing_extensions import Literal, TypedDict
 
 import aiormq.abc
 from aiormq.abc import ExceptionType
@@ -77,19 +78,14 @@
     message_count: int
     consumer_count: int
 
 
 class AbstractTransaction:
     state: TransactionState
 
-    @property
-    @abstractmethod
-    def channel(self) -> "AbstractChannel":
-        raise NotImplementedError
-
     @abstractmethod
     async def select(
         self, timeout: TimeoutType = None,
     ) -> aiormq.spec.Tx.SelectOk:
         raise NotImplementedError
 
     @abstractmethod
@@ -240,15 +236,15 @@
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
         raise NotImplementedError
 
 
 class AbstractQueue:
-    channel: aiormq.abc.AbstractChannel
+    channel: "AbstractChannel"
     name: str
     durable: bool
     exclusive: bool
     auto_delete: bool
     arguments: Arguments
     passive: bool
     declaration_result: aiormq.spec.Queue.DeclareOk
@@ -303,15 +299,15 @@
         timeout: TimeoutType = None,
     ) -> aiormq.spec.Queue.UnbindOk:
         raise NotImplementedError
 
     @abstractmethod
     async def consume(
         self,
-        callback: Callable[[AbstractIncomingMessage], Any],
+        callback: Callable[[AbstractIncomingMessage], Awaitable[Any]],
         no_ack: bool = False,
         exclusive: bool = False,
         arguments: Arguments = None,
         consumer_tag: Optional[ConsumerTag] = None,
         timeout: TimeoutType = None,
     ) -> ConsumerTag:
         raise NotImplementedError
@@ -405,15 +401,15 @@
 
 class AbstractExchange(ABC):
     name: str
 
     @abstractmethod
     def __init__(
         self,
-        channel: aiormq.abc.AbstractChannel,
+        channel: "AbstractChannel",
         name: str,
         type: Union[ExchangeType, str] = ExchangeType.DIRECT,
         *,
         auto_delete: bool = False,
         durable: bool = False,
         internal: bool = False,
         passive: bool = False,
@@ -524,17 +520,16 @@
     def is_closed(self) -> bool:
         raise NotImplementedError
 
     @abstractmethod
     def close(self, exc: Optional[ExceptionType] = None) -> Awaitable[None]:
         raise NotImplementedError
 
-    @property
     @abstractmethod
-    def channel(self) -> aiormq.abc.AbstractChannel:
+    async def get_underlay_channel(self) -> aiormq.abc.AbstractChannel:
         raise NotImplementedError
 
     @property
     @abstractmethod
     def number(self) -> Optional[int]:
         raise NotImplementedError
 
@@ -756,15 +751,15 @@
         reason: str = "", timeout: TimeoutType = None,
     ) -> aiormq.spec.Connection.UpdateSecretOk:
         raise NotImplementedError
 
 
 class AbstractRobustQueue(AbstractQueue):
     @abstractmethod
-    def restore(self, channel: aiormq.abc.AbstractChannel) -> Awaitable[None]:
+    def restore(self) -> Awaitable[None]:
         raise NotImplementedError
 
     @abstractmethod
     async def bind(
         self,
         exchange: ExchangeParamType,
         routing_key: Optional[str] = None,
@@ -787,15 +782,15 @@
         robust: bool = True,
     ) -> ConsumerTag:
         raise NotImplementedError
 
 
 class AbstractRobustExchange(AbstractExchange):
     @abstractmethod
-    def restore(self, channel: aiormq.abc.AbstractChannel) -> Awaitable[None]:
+    def restore(self) -> Awaitable[None]:
         raise NotImplementedError
 
     @abstractmethod
     async def bind(
         self,
         exchange: ExchangeParamType,
         routing_key: str = "",
@@ -811,15 +806,15 @@
     reopen_callbacks: CallbackCollection
 
     @abstractmethod
     def reopen(self) -> Awaitable[None]:
         raise NotImplementedError
 
     @abstractmethod
-    async def restore(self, connection: aiormq.abc.AbstractConnection) -> None:
+    async def restore(self) -> None:
         raise NotImplementedError
 
     @abstractmethod
     async def declare_exchange(
         self,
         name: str,
         type: Union[ExchangeType, str] = ExchangeType.DIRECT,
```

### Comparing `aio_pika-9.0.7/aio_pika/channel.py` & `aio_pika-9.1.0/aio_pika/channel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import asyncio
+import warnings
 from abc import ABC
 from types import TracebackType
 from typing import Any, AsyncContextManager, Generator, Optional, Type, Union
 from warnings import warn
 
 import aiormq
 import aiormq.abc
 from pamqp.common import Arguments
 
 from .abc import (
-    AbstractChannel, AbstractExchange, AbstractQueue, TimeoutType,
-    UnderlayChannel,
+    AbstractChannel, AbstractConnection, AbstractExchange, AbstractQueue,
+    TimeoutType, UnderlayChannel,
 )
+from .exceptions import ChannelInvalidStateError
 from .exchange import Exchange, ExchangeType
 from .log import get_logger
 from .message import IncomingMessage
 from .queue import Queue
 from .tools import CallbackCollection
 from .transaction import Transaction
 
@@ -48,15 +50,15 @@
     QUEUE_CLASS = Queue
     EXCHANGE_CLASS = Exchange
 
     _channel: Optional[UnderlayChannel]
 
     def __init__(
         self,
-        connection: aiormq.abc.AbstractConnection,
+        connection: AbstractConnection,
         channel_number: Optional[int] = None,
         publisher_confirms: bool = True,
         on_return_raises: bool = False,
     ):
         """
 
         :param connection: :class:`aio_pika.adapter.AsyncioConnection` instance
@@ -69,20 +71,20 @@
 
         if not publisher_confirms and on_return_raises:
             raise RuntimeError(
                 '"on_return_raises" not applicable '
                 'without "publisher_confirms"',
             )
 
-        self._connection: aiormq.abc.AbstractConnection = connection
+        self._connection: AbstractConnection = connection
 
         # That's means user closed channel instance explicitly
         self._closed: bool = False
 
-        self._channel = None
+        self._channel: Optional[UnderlayChannel] = None
         self._channel_number = channel_number
 
         self.close_callbacks = CallbackCollection(self)
         self.return_callbacks = CallbackCollection(self)
 
         self.publisher_confirms = publisher_confirms
         self.on_return_raises = on_return_raises
@@ -95,17 +97,18 @@
 
     @property
     def is_closed(self) -> bool:
         """Returns True when the channel has been closed from the broker
         side or after the close() method has been called."""
         if not self.is_initialized or self._closed:
             return True
-        if not self._channel:
+        channel = self._channel
+        if channel is None:
             return True
-        return self._channel.channel.is_closed
+        return channel.channel.is_closed
 
     async def close(
         self,
         exc: Optional[aiormq.abc.ExceptionType] = None,
     ) -> None:
         if not self.is_initialized:
             log.warning("Channel not opened")
@@ -115,67 +118,80 @@
             log.warning("Transport is not ready")
             return
 
         log.debug("Closing channel %r", self)
         self._closed = True
         await self._channel.close()
 
-    @property
-    def channel(self) -> aiormq.abc.AbstractChannel:
+    async def get_underlay_channel(self) -> aiormq.abc.AbstractChannel:
 
         if not self.is_initialized or not self._channel:
             raise aiormq.exceptions.ChannelInvalidStateError(
                 "Channel was not opened",
             )
 
-        if self.is_closed:
-            raise aiormq.exceptions.ChannelInvalidStateError(
-                "Channel has been closed",
-            )
+        return self._channel.channel
 
+    @property
+    def channel(self) -> aiormq.abc.AbstractChannel:
+        warnings.warn(
+            "This property is deprecated, do not use this anymore.",
+            DeprecationWarning,
+        )
+        if self._channel is None:
+            raise aiormq.exceptions.ChannelInvalidStateError
         return self._channel.channel
 
     @property
     def number(self) -> Optional[int]:
-        return (
-            self.channel.number
-            if self.is_initialized
-            else self._channel_number
-        )
+        if self._channel is None:
+            return self._channel_number
+
+        underlay_channel: UnderlayChannel = self._channel
+        return underlay_channel.channel.number
 
     def __str__(self) -> str:
         return "{}".format(self.number or "Not initialized channel")
 
     async def _open(self) -> None:
         await self._connection.ready()
 
+        transport = self._connection.transport
+        if transport is None:
+            raise ChannelInvalidStateError("No active transport in channel")
+
         channel = await UnderlayChannel.create(
-            self._connection,
+            transport.connection,
             self._on_close,
             publisher_confirms=self.publisher_confirms,
             on_return_raises=self.on_return_raises,
             channel_number=self._channel_number,
         )
 
-        await self._on_open(channel.channel)
         self._channel = channel
+        try:
+            await self._on_open()
+        except BaseException as e:
+            await channel.close(e)
+            self._channel = None
+            raise
         self._closed = False
 
     async def initialize(self, timeout: TimeoutType = None) -> None:
         if self.is_initialized:
             raise RuntimeError("Already initialized")
         elif self._closed:
             raise RuntimeError("Can't initialize closed channel")
 
         await self._open()
         await self._on_initialized()
 
-    async def _on_open(self, channel: aiormq.abc.AbstractChannel) -> None:
+    async def _on_open(self) -> None:
         self.default_exchange: Exchange = self.EXCHANGE_CLASS(
-            channel=channel,
+            channel=self,
             arguments=None,
             auto_delete=False,
             durable=False,
             internal=False,
             name="",
             passive=False,
             type=ExchangeType.DIRECT,
@@ -188,15 +204,16 @@
             exc = e
         await self.close_callbacks(exc)
 
         if self._channel and self._channel.channel:
             self._channel.channel.on_return_callbacks.discard(self._on_return)
 
     async def _on_initialized(self) -> None:
-        self.channel.on_return_callbacks.add(self._on_return)
+        channel = await self.get_underlay_channel()
+        channel.on_return_callbacks.add(self._on_return)
 
     def _on_return(self, message: aiormq.abc.DeliveredMessage) -> None:
         self.return_callbacks(IncomingMessage(message, no_ack=True))
 
     async def reopen(self) -> None:
         log.debug("Start reopening channel %r", self)
         await self._open()
@@ -237,15 +254,15 @@
         :return: :class:`aio_pika.exchange.Exchange` instance
         """
 
         if auto_delete and durable is None:
             durable = False
 
         exchange = self.EXCHANGE_CLASS(
-            channel=self.channel,
+            channel=self,
             name=name,
             type=type,
             durable=durable,
             auto_delete=auto_delete,
             internal=internal,
             passive=passive,
             arguments=arguments,
@@ -277,15 +294,15 @@
         :raises: :class:`aio_pika.exceptions.ChannelClosed` instance
         """
 
         if ensure:
             return await self.declare_exchange(name=name, passive=True)
         else:
             return self.EXCHANGE_CLASS(
-                channel=self.channel,
+                channel=self,
                 name=name,
                 durable=False,
                 auto_delete=False,
                 internal=False,
                 passive=True,
                 arguments=None,
             )
@@ -317,15 +334,15 @@
         :param arguments: additional arguments
         :param timeout: execution timeout
         :return: :class:`aio_pika.queue.Queue` instance
         :raises: :class:`aio_pika.exceptions.ChannelClosed` instance
         """
 
         queue: AbstractQueue = self.QUEUE_CLASS(
-            channel=self.channel,
+            channel=self,
             name=name,
             durable=durable,
             exclusive=exclusive,
             auto_delete=auto_delete,
             arguments=arguments,
             passive=passive,
         )
@@ -354,15 +371,15 @@
         :raises: :class:`aio_pika.exceptions.ChannelClosed` instance
         """
 
         if ensure:
             return await self.declare_queue(name=name, passive=True)
         else:
             return self.QUEUE_CLASS(
-                channel=self.channel,
+                channel=self,
                 name=name,
                 durable=False,
                 exclusive=False,
                 auto_delete=False,
                 arguments=None,
                 passive=True,
             )
@@ -375,45 +392,49 @@
         timeout: TimeoutType = None,
         all_channels: Optional[bool] = None,
     ) -> aiormq.spec.Basic.QosOk:
         if all_channels is not None:
             warn('Use "global_" instead of "all_channels"', DeprecationWarning)
             global_ = all_channels
 
-        return await self.channel.basic_qos(
+        channel = await self.get_underlay_channel()
+
+        return await channel.basic_qos(
             prefetch_count=prefetch_count,
             prefetch_size=prefetch_size,
             global_=global_,
             timeout=timeout,
         )
 
     async def queue_delete(
         self,
         queue_name: str,
         timeout: TimeoutType = None,
         if_unused: bool = False,
         if_empty: bool = False,
         nowait: bool = False,
     ) -> aiormq.spec.Queue.DeleteOk:
-        return await self.channel.queue_delete(
+        channel = await self.get_underlay_channel()
+        return await channel.queue_delete(
             queue=queue_name,
             if_unused=if_unused,
             if_empty=if_empty,
             nowait=nowait,
             timeout=timeout,
         )
 
     async def exchange_delete(
         self,
         exchange_name: str,
         timeout: TimeoutType = None,
         if_unused: bool = False,
         nowait: bool = False,
     ) -> aiormq.spec.Exchange.DeleteOk:
-        return await self.channel.exchange_delete(
+        channel = await self.get_underlay_channel()
+        return await channel.exchange_delete(
             exchange=exchange_name,
             if_unused=if_unused,
             nowait=nowait,
             timeout=timeout,
         )
 
     def transaction(self) -> Transaction:
@@ -422,11 +443,12 @@
                 "Cannot create transaction when publisher "
                 "confirms are enabled",
             )
 
         return Transaction(self)
 
     async def flow(self, active: bool = True) -> aiormq.spec.Channel.FlowOk:
-        return await self.channel.flow(active=active)
+        channel = await self.get_underlay_channel()
+        return await channel.flow(active=active)
 
 
 __all__ = ("Channel",)
```

### Comparing `aio_pika-9.0.7/aio_pika/connection.py` & `aio_pika-9.1.0/aio_pika/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import asyncio
 from ssl import SSLContext
 from types import TracebackType
 from typing import Any, Callable, Dict, Optional, Tuple, Type, TypeVar, Union
 
 import aiormq.abc
-from aiormq.tools import censor_url
 from pamqp.common import FieldTable
 from yarl import URL
 
 from .abc import (
     AbstractChannel, AbstractConnection, SSLOptions, TimeoutType,
     UnderlayConnection,
 )
 from .channel import Channel
+from .exceptions import ConnectionClosed
 from .log import get_logger
 from .tools import CallbackCollection
 
 
 log = get_logger(__name__)
 T = TypeVar("T")
 
@@ -30,15 +30,15 @@
     _closed: bool
 
     @property
     def is_closed(self) -> bool:
         return self._closed
 
     async def close(
-        self, exc: Optional[aiormq.abc.ExceptionType] = asyncio.CancelledError,
+        self, exc: Optional[aiormq.abc.ExceptionType] = ConnectionClosed,
     ) -> None:
         transport, self.transport = self.transport, None
         self._close_called = True
         if not transport:
             return
         await transport.close(exc)
         self._closed = True
@@ -65,45 +65,47 @@
             kwargs or dict(self.url.query),
         )
         self.kwargs["context"] = ssl_context
         self.close_callbacks = CallbackCollection(self)
         self.connected: asyncio.Event = asyncio.Event()
 
     def __str__(self) -> str:
-        return str(censor_url(self.url))
+        url = self.url
+        if url.password:
+            url = url.with_password("******")
+        return str(url)
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__}: "{self}">'
 
     async def _on_connection_close(self, closing: asyncio.Future) -> None:
         try:
             exc = closing.exception()
         except asyncio.CancelledError as e:
             exc = e
         self.connected.clear()
         await self.close_callbacks(exc)
 
-    async def _on_connected(self, transport: UnderlayConnection) -> None:
+    async def _on_connected(self) -> None:
         self.connected.set()
 
     async def connect(self, timeout: TimeoutType = None) -> None:
         """ Connect to AMQP server. This method should be called after
         :func:`aio_pika.connection.Connection.__init__`
 
         .. note::
             This method is called by :func:`connect`.
             You shouldn't call it explicitly.
 
         """
-        transport = await UnderlayConnection.connect(
+        self.transport = await UnderlayConnection.connect(
             self.url, self._on_connection_close,
             timeout=timeout, **self.kwargs,
         )
-        await self._on_connected(transport)
-        self.transport = transport
+        await self._on_connected()
 
     def channel(
         self,
         channel_number: Optional[int] = None,
         publisher_confirms: bool = True,
         on_return_raises: bool = False,
     ) -> AbstractChannel:
@@ -162,15 +164,15 @@
 
         if not self.transport:
             raise RuntimeError("Connection was not opened")
 
         log.debug("Creating AMQP channel for connection: %r", self)
 
         channel = self.CHANNEL_CLASS(
-            connection=self.transport.connection,
+            connection=self,
             channel_number=channel_number,
             publisher_confirms=publisher_confirms,
             on_return_raises=on_return_raises,
         )
 
         log.debug("Channel created: %r", channel)
         return channel
```

### Comparing `aio_pika-9.0.7/aio_pika/exceptions.py` & `aio_pika-9.1.0/aio_pika/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.7/aio_pika/exchange.py` & `aio_pika-9.1.0/aio_pika/exchange.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Optional, Union
 
 import aiormq
 from pamqp.common import Arguments
 
 from .abc import (
-    AbstractExchange, AbstractMessage, ExchangeParamType, ExchangeType,
-    TimeoutType, get_exchange_name,
+    AbstractChannel, AbstractExchange, AbstractMessage, ExchangeParamType,
+    ExchangeType, TimeoutType, get_exchange_name,
 )
 from .log import get_logger
 
 
 log = get_logger(__name__)
 
 
 class Exchange(AbstractExchange):
     """ Exchange abstraction """
-    channel: aiormq.abc.AbstractChannel
+    channel: AbstractChannel
 
     def __init__(
         self,
-        channel: aiormq.abc.AbstractChannel,
+        channel: AbstractChannel,
         name: str,
         type: Union[ExchangeType, str] = ExchangeType.DIRECT,
         *,
         auto_delete: bool = False,
         durable: bool = False,
         internal: bool = False,
         passive: bool = False,
@@ -48,15 +48,16 @@
             f" durable={self.durable},"
             f" arguments={self.arguments!r})>"
         )
 
     async def declare(
         self, timeout: TimeoutType = None,
     ) -> aiormq.spec.Exchange.DeclareOk:
-        return await self.channel.exchange_declare(
+        channel = await self.channel.get_underlay_channel()
+        return await channel.exchange_declare(
             self.name,
             exchange_type=self._type,
             durable=self.durable,
             auto_delete=self.auto_delete,
             internal=self.internal,
             passive=self.passive,
             arguments=self.arguments,
@@ -110,15 +111,16 @@
             "Binding exchange %r to exchange %r, routing_key=%r, arguments=%r",
             self,
             exchange,
             routing_key,
             arguments,
         )
 
-        return await self.channel.exchange_bind(
+        channel = await self.channel.get_underlay_channel()
+        return await channel.exchange_bind(
             arguments=arguments,
             destination=self.name,
             routing_key=routing_key,
             source=get_exchange_name(exchange),
             timeout=timeout,
         )
 
@@ -145,15 +147,16 @@
             "routing_key=%r, arguments=%r",
             self,
             exchange,
             routing_key,
             arguments,
         )
 
-        return await self.channel.exchange_unbind(
+        channel = await self.channel.get_underlay_channel()
+        return await channel.exchange_unbind(
             arguments=arguments,
             destination=self.name,
             routing_key=routing_key,
             source=get_exchange_name(exchange),
             timeout=timeout,
         )
 
@@ -183,15 +186,16 @@
 
         if self.internal:
             # Caught on the client side to prevent channel closure
             raise ValueError(
                 f"Can not publish to internal exchange: '{self.name}'!",
             )
 
-        return await self.channel.basic_publish(
+        channel = await self.channel.get_underlay_channel()
+        return await channel.basic_publish(
             exchange=self.name,
             routing_key=routing_key,
             body=message.body,
             properties=message.properties,
             mandatory=mandatory,
             immediate=immediate,
             timeout=timeout,
@@ -204,13 +208,16 @@
         """ Delete the queue
 
         :param timeout: operation timeout
         :param if_unused: perform deletion when queue has no bindings.
         """
 
         log.info("Deleting %r", self)
-        return await self.channel.exchange_delete(
+        channel = await self.channel.get_underlay_channel()
+        result = await channel.exchange_delete(
             self.name, if_unused=if_unused, timeout=timeout,
         )
+        del self.channel
+        return result
 
 
 __all__ = ("Exchange", "ExchangeType", "ExchangeParamType")
```

### Comparing `aio_pika-9.0.7/aio_pika/message.py` & `aio_pika-9.1.0/aio_pika/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pamqp.common import FieldValue
 
 from .abc import (
     MILLISECONDS, ZERO_TIME, AbstractChannel, AbstractIncomingMessage,
     AbstractMessage, AbstractProcessContext, DateType, DeliveryMode,
     HeadersType, MessageInfo, NoneType,
 )
-from .exceptions import MessageProcessError
+from .exceptions import ChannelInvalidStateError, MessageProcessError
 from .log import get_logger
 
 
 log = get_logger(__name__)
 
 
 def to_milliseconds(seconds: Union[float, int]) -> int:
@@ -406,14 +406,16 @@
 
         if no_ack or not self.delivery_tag:
             self.lock()
             self.__processed = True
 
     @property
     def channel(self) -> aiormq.abc.AbstractChannel:
+        if self.__channel.is_closed:
+            raise ChannelInvalidStateError
         return self.__channel
 
     def process(
         self,
         requeue: bool = False,
         reject_on_redelivered: bool = False,
         ignore_processed: bool = False,
@@ -467,26 +469,26 @@
         if self.__no_ack:
             raise TypeError('Can\'t ack message with "no_ack" flag')
 
         if self.__processed:
             raise MessageProcessError("Message already processed", self)
 
         if self.delivery_tag is not None:
-            await self.__channel.basic_ack(
+            await self.channel.basic_ack(
                 delivery_tag=self.delivery_tag, multiple=multiple,
             )
 
         self.__processed = True
 
         if not self.locked:
             self.lock()
 
     async def reject(self, requeue: bool = False) -> None:
         """ When `requeue=True` the message will be returned to queue.
-        Otherwise message will be dropped.
+        Otherwise, message will be dropped.
 
         .. note::
             This method looks like a blocking-method, but actually it just
             sends bytes to the socket and doesn't require any responses from
             the broker.
 
         :param requeue: bool
@@ -494,15 +496,15 @@
         if self.__no_ack:
             raise TypeError('This message has "no_ack" flag.')
 
         if self.__processed:
             raise MessageProcessError("Message already processed", self)
 
         if self.delivery_tag is not None:
-            await self.__channel.basic_reject(
+            await self.channel.basic_reject(
                 delivery_tag=self.delivery_tag,
                 requeue=requeue,
             )
 
         self.__processed = True
         if not self.locked:
             self.lock()
@@ -517,15 +519,15 @@
         if self.__no_ack:
             raise TypeError('Can\'t nack message with "no_ack" flag')
 
         if self.__processed:
             raise MessageProcessError("Message already processed", self)
 
         if self.delivery_tag is not None:
-            await self.__channel.basic_nack(
+            await self.channel.basic_nack(
                 delivery_tag=self.delivery_tag,
                 multiple=multiple,
                 requeue=requeue,
             )
 
         self.__processed = True
```

### Comparing `aio_pika-9.0.7/aio_pika/patterns/base.py` & `aio_pika-9.1.0/aio_pika/patterns/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import pickle
-from typing import Any, Callable
+from typing import Any, Awaitable, Callable, TypeVar
+
+
+T = TypeVar("T")
+CallbackType = Callable[..., Awaitable[T]]
 
 
 class Method:
     __slots__ = (
         "name",
         "func",
     )
```

### Comparing `aio_pika-9.0.7/aio_pika/patterns/master.py` & `aio_pika-9.1.0/aio_pika/patterns/master.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import asyncio
 import gzip
 import json
 import logging
 from functools import partial
 from types import MappingProxyType
-from typing import Any, Awaitable, Callable, Mapping, Optional, TypeVar
+from typing import Any, Awaitable, Mapping, Optional
 
 import aiormq
-from aiormq.tools import awaitable
 
 from aio_pika.abc import (
     AbstractChannel, AbstractExchange, AbstractIncomingMessage, AbstractQueue,
     ConsumerTag, DeliveryMode,
 )
 from aio_pika.message import Message, ReturnedMessage
 
-from ..tools import create_task
-from .base import Base, Proxy
+from ..tools import create_task, ensure_awaitable
+from .base import Base, CallbackType, Proxy, T
 
 
 log = logging.getLogger(__name__)
-T = TypeVar("T")
 
 
 class MessageProcessingError(Exception):
     pass
 
 
 class NackMessage(MessageProcessingError):
@@ -139,25 +137,26 @@
         :param data: Data which will be deserialized
         :returns: :class:`Any`
         """
         return super().deserialize(data)
 
     @classmethod
     async def execute(
-        cls, func: Callable[..., Awaitable[T]], kwargs: Any,
+        cls, func: CallbackType, kwargs: Any,
     ) -> T:
         kwargs = kwargs or {}
 
         if not isinstance(kwargs, dict):
+            logging.error("Bad kwargs %r received for the %r", kwargs, func)
             raise RejectMessage(requeue=False)
 
         return await func(**kwargs)
 
     async def on_message(
-        self, func: Callable[..., Any],
+        self, func: CallbackType,
         message: AbstractIncomingMessage,
     ) -> None:
         async with message.process(
             requeue=self._requeue,
             reject_on_redelivered=self._reject_on_redelivered,
             ignore_processed=True,
         ):
@@ -170,25 +169,23 @@
 
     async def create_queue(
         self, queue_name: str, **kwargs: Any,
     ) -> AbstractQueue:
         return await self.channel.declare_queue(queue_name, **kwargs)
 
     async def create_worker(
-        self, queue_name: str, func: Callable[..., Any], **kwargs: Any,
+        self, queue_name: str,
+        func: CallbackType,
+        **kwargs: Any,
     ) -> Worker:
         """ Creates a new :class:`Worker` instance. """
-
         queue = await self.create_queue(queue_name, **kwargs)
-
-        if hasattr(func, "_is_coroutine"):
-            fn = func
-        else:
-            fn = awaitable(func)
-        consumer_tag = await queue.consume(partial(self.on_message, fn))
+        consumer_tag = await queue.consume(
+            partial(self.on_message, ensure_awaitable(func)),
+        )
 
         return Worker(queue, consumer_tag, self.loop)
 
     async def create_task(
         self, channel_name: str,
         kwargs: Mapping[str, Any] = MappingProxyType({}),
         **message_kwargs: Any,
```

### Comparing `aio_pika-9.0.7/aio_pika/patterns/rpc.py` & `aio_pika-9.1.0/aio_pika/patterns/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 import asyncio
 import json
 import logging
 import time
 import uuid
 from enum import Enum
 from functools import partial
-from typing import Any, Callable, Dict, Optional, Tuple, TypeVar
+from typing import Any, Callable, Dict, Optional, Tuple
 
 from aiormq.abc import ExceptionType
-from aiormq.tools import awaitable
 
 from aio_pika.abc import (
     AbstractChannel, AbstractExchange, AbstractIncomingMessage, AbstractQueue,
     ConsumerTag, DeliveryMode,
 )
 from aio_pika.exceptions import MessageProcessError
 from aio_pika.exchange import ExchangeType
 from aio_pika.message import IncomingMessage, Message, ReturnedMessage
 
-from .base import Base, Proxy
+from ..tools import ensure_awaitable
+from .base import Base, CallbackType, Proxy, T
 
 
 log = logging.getLogger(__name__)
 
-T = TypeVar("T")
-CallbackType = Callable[..., T]
-
 
 class RPCException(RuntimeError):
     pass
 
 
 class RPCMessageType(str, Enum):
     ERROR = "error"
@@ -386,14 +383,16 @@
         :raises RuntimeError:
             Function already registered in this :class:`RPC` instance
             or method_name already used.
         """
         arguments = kwargs.pop("arguments", {})
         arguments.update({"x-dead-letter-exchange": self.DLX_NAME})
 
+        func = ensure_awaitable(func)
+
         kwargs["arguments"] = arguments
 
         queue = await self.channel.declare_queue(method_name, **kwargs)
 
         if func in self.consumer_tags:
             raise RuntimeError("Function already registered")
 
@@ -402,15 +401,15 @@
                 "Method name already used for %r" % self.routes[method_name],
             )
 
         self.consumer_tags[func] = await queue.consume(
             partial(self.on_call_message, method_name),
         )
 
-        self.routes[method_name] = awaitable(func)
+        self.routes[method_name] = func
         self.queues[func] = queue
 
     async def unregister(self, func: CallbackType) -> None:
         """ Cancels subscription to the method-queue.
 
         :param func: Function
         """
@@ -453,13 +452,12 @@
         payload = await super().deserialize_message(message)
         if message.type == RPCMessageType.ERROR:
             payload = JsonRPCError("RPC exception", payload)
         return payload
 
 
 __all__ = (
-    "CallbackType",
     "JsonRPC",
     "RPC",
     "RPCException",
     "RPCMessageType",
 )
```

### Comparing `aio_pika-9.0.7/aio_pika/pool.py` & `aio_pika-9.1.0/aio_pika/pool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import abc
 import asyncio
 from types import TracebackType
 from typing import (
-    Any, AsyncContextManager, Awaitable, Callable, Coroutine, Generic, Optional,
-    Set, Tuple, Type, TypeVar, Union,
+    Any, AsyncContextManager, Awaitable, Callable, Generic, Optional, Set,
+    Tuple, Type, TypeVar,
 )
 
-from aiormq.tools import awaitable
-
 from aio_pika.log import get_logger
 from aio_pika.tools import create_task
 
 
 log = get_logger(__name__)
 
 
@@ -20,19 +18,15 @@
     def close(self) -> Awaitable[None]:
         raise NotImplementedError
 
 
 T = TypeVar("T")
 ConstructorType = Callable[
     ...,
-    Union[
-        Awaitable[PoolInstance],
-        PoolInstance,
-        Coroutine[Any, Any, PoolInstance],
-    ],
+    Awaitable[PoolInstance],
 ]
 
 
 class PoolInvalidStateError(RuntimeError):
     pass
 
 
@@ -54,17 +48,15 @@
         constructor: ConstructorType,
         *args: Any,
         max_size: Optional[int] = None,
         loop: Optional[asyncio.AbstractEventLoop] = None,
     ):
         self.loop = loop or asyncio.get_event_loop()
         self.__closed = False
-        self.__constructor: Callable[..., Awaitable[Any]] = awaitable(
-            constructor,
-        )
+        self.__constructor: Callable[..., Awaitable[Any]] = constructor
         self.__constructor_args: Tuple[Any, ...] = args or ()
         self.__created: int = 0
         self.__item_set: Set[PoolInstance] = set()
         self.__items: asyncio.Queue = asyncio.Queue()
         self.__lock: asyncio.Lock = asyncio.Lock()
         self.__max_size: Optional[int] = max_size
```

### Comparing `aio_pika-9.0.7/aio_pika/queue.py` & `aio_pika-9.1.0/aio_pika/queue.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import asyncio
 import sys
 from functools import partial
 from types import TracebackType
-from typing import Any, Callable, Optional, Type, overload
+from typing import Any, Awaitable, Callable, Optional, Type, overload
 
 import aiormq
 from aiormq.abc import DeliveredMessage
 from pamqp.common import Arguments
 
 from .abc import (
-    AbstractIncomingMessage, AbstractQueue, AbstractQueueIterator, ConsumerTag,
-    TimeoutType, get_exchange_name,
+    AbstractChannel, AbstractIncomingMessage, AbstractQueue,
+    AbstractQueueIterator, ConsumerTag, TimeoutType, get_exchange_name,
 )
 from .exceptions import QueueEmpty
 from .exchange import ExchangeParamType
 from .log import get_logger
 from .message import IncomingMessage
-from .tools import CallbackCollection, create_task
+from .tools import CallbackCollection, create_task, ensure_awaitable
 
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -38,15 +38,15 @@
 
 
 class Queue(AbstractQueue):
     """ AMQP queue abstraction """
 
     def __init__(
         self,
-        channel: aiormq.abc.AbstractChannel,
+        channel: AbstractChannel,
         name: Optional[str],
         durable: bool,
         exclusive: bool,
         auto_delete: bool,
         arguments: Arguments,
         passive: bool = False,
     ):
@@ -78,15 +78,16 @@
         """ Declare queue.
 
         :param timeout: execution timeout
         :param passive: Only check to see if the queue exists.
         :return: :class:`None`
         """
         log.debug("Declaring queue: %r", self)
-        self.declaration_result = await self.channel.queue_declare(
+        channel = await self.channel.get_underlay_channel()
+        self.declaration_result = await channel.queue_declare(
             queue=self.name,
             durable=self.durable,
             exclusive=self.exclusive,
             auto_delete=self.auto_delete,
             arguments=self.arguments,
             passive=self.passive,
             timeout=timeout,
@@ -131,15 +132,16 @@
             "Binding queue %r: exchange=%r, routing_key=%r, arguments=%r",
             self,
             exchange,
             routing_key,
             arguments,
         )
 
-        return await self.channel.queue_bind(
+        channel = await self.channel.get_underlay_channel()
+        return await channel.queue_bind(
             self.name,
             exchange=get_exchange_name(exchange),
             routing_key=routing_key,
             arguments=arguments,
             timeout=timeout,
         )
 
@@ -169,37 +171,38 @@
             "Unbinding queue %r: exchange=%r, routing_key=%r, arguments=%r",
             self,
             exchange,
             routing_key,
             arguments,
         )
 
-        return await self.channel.queue_unbind(
+        channel = await self.channel.get_underlay_channel()
+        return await channel.queue_unbind(
             queue=self.name,
             exchange=get_exchange_name(exchange),
             routing_key=routing_key,
             arguments=arguments,
             timeout=timeout,
         )
 
     async def consume(
         self,
-        callback: Callable[[AbstractIncomingMessage], Any],
+        callback: Callable[[AbstractIncomingMessage], Awaitable[Any]],
         no_ack: bool = False,
         exclusive: bool = False,
         arguments: Arguments = None,
         consumer_tag: Optional[ConsumerTag] = None,
         timeout: TimeoutType = None,
     ) -> ConsumerTag:
 
         """ Start to consuming the :class:`Queue`.
 
         :param timeout: :class:`asyncio.TimeoutError` will be raises when the
                         Future was not finished after this time.
-        :param callback: Consuming callback. Could be a coroutine.
+        :param callback: Consuming callback. Should be a coroutine function.
         :param no_ack:
             if :class:`True` you don't need to call
             :func:`aio_pika.message.IncomingMessage.ack`
         :param exclusive:
             Makes this queue exclusive. Exclusive queues may only
             be accessed by the current connection, and are deleted
             when that connection closes. Passive declaration of an
@@ -210,16 +213,18 @@
         :raises asyncio.TimeoutError:
             when the consuming timeout period has elapsed.
         :return str: consumer tag :class:`str`
 
         """
 
         log.debug("Start to consuming queue: %r", self)
+        callback = ensure_awaitable(callback)
 
-        consume_result = await self.channel.basic_consume(
+        channel = await self.channel.get_underlay_channel()
+        consume_result = await channel.basic_consume(
             queue=self.name,
             consumer_callback=partial(
                 consumer,
                 callback,
                 no_ack=no_ack,
             ),
             exclusive=exclusive,
@@ -255,15 +260,16 @@
         :param consumer_tag:
             consumer tag returned by :func:`~aio_pika.Queue.consume`
         :param timeout: execution timeout
         :param bool nowait: Do not expect a Basic.CancelOk response
         :return: Basic.CancelOk when operation completed successfully
         """
 
-        return await self.channel.basic_cancel(
+        channel = await self.channel.get_underlay_channel()
+        return await channel.basic_cancel(
             consumer_tag=consumer_tag, nowait=nowait, timeout=timeout,
         )
 
     @overload
     async def get(
         self, *, no_ack: bool = False,
         fail: Literal[True] = ..., timeout: TimeoutType = ...,
@@ -288,15 +294,16 @@
                        :func:`aio_pika.message.IncomingMessage.ack`
         :param timeout: execution timeout
         :param fail: Should return :class:`None` instead of raise an
                      exception :class:`aio_pika.exceptions.QueueEmpty`.
         :return: :class:`aio_pika.message.IncomingMessage`
         """
 
-        msg: DeliveredMessage = await self.channel.basic_get(
+        channel = await self.channel.get_underlay_channel()
+        msg: DeliveredMessage = await channel.basic_get(
             self.name, no_ack=no_ack, timeout=timeout,
         )
 
         if isinstance(msg.delivery, aiormq.spec.Basic.GetEmpty):
             if fail:
                 raise QueueEmpty
             return None
@@ -311,15 +318,16 @@
         :param no_wait: no wait response
         :param timeout: execution timeout
         :return: :class:`None`
         """
 
         log.info("Purging queue: %r", self)
 
-        return await self.channel.queue_purge(
+        channel = await self.channel.get_underlay_channel()
+        return await channel.queue_purge(
             self.name, nowait=no_wait, timeout=timeout,
         )
 
     async def delete(
         self, *, if_unused: bool = True,
         if_empty: bool = True, timeout: TimeoutType = None,
     ) -> aiormq.spec.Queue.DeleteOk:
@@ -330,15 +338,16 @@
         :param if_empty: Perform delete only when empty
         :param timeout: execution timeout
         :return: :class:`None`
         """
 
         log.info("Deleting %r", self)
 
-        return await self.channel.queue_delete(
+        channel = await self.channel.get_underlay_channel()
+        return await channel.queue_delete(
             self.name,
             if_unused=if_unused,
             if_empty=if_empty,
             timeout=timeout,
         )
 
     def __aiter__(self) -> "AbstractQueueIterator":
```

### Comparing `aio_pika-9.0.7/aio_pika/robust_channel.py` & `aio_pika-9.1.0/aio_pika/robust_channel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import asyncio
+import warnings
 from collections import defaultdict
 from itertools import chain
-from typing import Any, DefaultDict, Dict, Optional, Set, Type, Union
+from typing import Any, DefaultDict, Dict, MutableSet, Optional, Type, Union
 from warnings import warn
+from weakref import WeakSet
 
 import aiormq
 
 from .abc import (
-    AbstractRobustChannel, AbstractRobustExchange, AbstractRobustQueue,
-    TimeoutType,
+    AbstractConnection, AbstractRobustChannel, AbstractRobustExchange,
+    AbstractRobustQueue, TimeoutType,
 )
 from .channel import Channel
 from .exchange import Exchange, ExchangeType
 from .log import get_logger
 from .queue import Queue
 from .robust_exchange import RobustExchange
 from .robust_queue import RobustQueue
@@ -24,21 +26,23 @@
 
 class RobustChannel(Channel, AbstractRobustChannel):    # type: ignore
     """ Channel abstraction """
 
     QUEUE_CLASS: Type[Queue] = RobustQueue
     EXCHANGE_CLASS: Type[Exchange] = RobustExchange
 
-    _exchanges: DefaultDict[str, Set[AbstractRobustExchange]]
-    _queues: DefaultDict[str, Set[RobustQueue]]
+    RESTORE_RETRY_DELAY: int = 2
+
+    _exchanges: DefaultDict[str, MutableSet[AbstractRobustExchange]]
+    _queues: DefaultDict[str, MutableSet[RobustQueue]]
     default_exchange: RobustExchange
 
     def __init__(
         self,
-        connection: aiormq.abc.AbstractConnection,
+        connection: AbstractConnection,
         channel_number: Optional[int] = None,
         publisher_confirms: bool = True,
         on_return_raises: bool = False,
     ):
         """
 
         :param connection: :class:`aio_pika.adapter.AsyncioConnection` instance
@@ -53,59 +57,92 @@
         super().__init__(
             connection=connection,
             channel_number=channel_number,
             publisher_confirms=publisher_confirms,
             on_return_raises=on_return_raises,
         )
 
-        self._exchanges = defaultdict(set)
-        self._queues = defaultdict(set)
+        self._exchanges = defaultdict(WeakSet)
+        self._queues = defaultdict(WeakSet)
         self._prefetch_count: int = 0
         self._prefetch_size: int = 0
         self._global_qos: bool = False
         self.reopen_callbacks: CallbackCollection = CallbackCollection(self)
-        self.close_callbacks.add(self.__close_callback)
         self.__restore_lock = asyncio.Lock()
+        self.__ready = asyncio.Event()
+        self.__restored = True
+        self.close_callbacks.add(self.__close_callback)
 
-    async def __close_callback(self, *_: Any) -> None:
-        if self._closed or self._connection.is_closed:
-            self.close_callbacks.discard(self.__close_callback)
-            return
+    async def ready(self) -> None:
+        while not self.__restored:
+            await self.__ready.wait()
 
-        await self.reopen()
+    async def get_underlay_channel(self) -> aiormq.abc.AbstractChannel:
+        await self._connection.ready()
+        return await super().get_underlay_channel()
+
+    async def restore(self, channel: Any = None) -> None:
+        if channel is not None:
+            warnings.warn(
+                "Channel argument will be ignored because you "
+                "don't need to pass this anymore.",
+                DeprecationWarning,
+            )
 
-    async def restore(self, connection: aiormq.abc.AbstractConnection) -> None:
         async with self.__restore_lock:
-            self._connection = connection
+            if self.__restored:
+                return
+
             await self.reopen()
+            self.__restored = True
+
+    async def __close_callback(self, _: Any, exc: BaseException) -> None:
+        if isinstance(exc, asyncio.CancelledError):
+            # This happens only if the channel is forced to close from the
+            # outside, for example, if the connection is closed.
+            # Of course, here you need to exit from this function
+            # as soon as possible and to avoid a recovery attempt.
+            return
+
+        in_restore_state = not self.__restored
+        self.__restored = False
+        self.__ready.clear()
+
+        if self._closed or in_restore_state:
+            return
+
+        await self.restore()
 
     async def _open(self) -> None:
         await super()._open()
         await self.reopen_callbacks()
 
-    async def _on_open(self, channel: aiormq.abc.AbstractChannel) -> None:
+    async def _on_open(self) -> None:
         if not hasattr(self, "default_exchange"):
-            await super()._on_open(channel)
+            await super()._on_open()
 
         exchanges = tuple(chain(*self._exchanges.values()))
         queues = tuple(chain(*self._queues.values()))
+        channel = await self.get_underlay_channel()
 
         await channel.basic_qos(
             prefetch_count=self._prefetch_count,
             prefetch_size=self._prefetch_size,
         )
 
         for exchange in exchanges:
-            await exchange.restore(channel)
+            await exchange.restore()
 
         for queue in queues:
-            await queue.restore(channel)
+            await queue.restore()
 
         if hasattr(self, "default_exchange"):
-            self.default_exchange.channel = channel
+            self.default_exchange.channel = self
+
+        self.__ready.set()
 
     async def set_qos(
         self,
         prefetch_count: int = 0,
         prefetch_size: int = 0,
         global_: bool = False,
         timeout: TimeoutType = None,
@@ -137,14 +174,15 @@
         internal: bool = False,
         passive: bool = False,
         arguments: Optional[Dict[str, Any]] = None,
         timeout: TimeoutType = None,
         robust: bool = True,
     ) -> AbstractRobustExchange:
         await self._connection.ready()
+        await self.ready()
         exchange = (
             await super().declare_exchange(
                 name=name,
                 type=type,
                 durable=durable,
                 auto_delete=auto_delete,
                 internal=internal,
@@ -164,14 +202,15 @@
         self,
         exchange_name: str,
         timeout: TimeoutType = None,
         if_unused: bool = False,
         nowait: bool = False,
     ) -> aiormq.spec.Exchange.DeleteOk:
         await self._connection.ready()
+        await self.ready()
         result = await super().exchange_delete(
             exchange_name=exchange_name,
             timeout=timeout,
             if_unused=if_unused,
             nowait=nowait,
         )
         self._exchanges.pop(exchange_name, None)
@@ -186,14 +225,15 @@
         passive: bool = False,
         auto_delete: bool = False,
         arguments: Optional[Dict[str, Any]] = None,
         timeout: TimeoutType = None,
         robust: bool = True,
     ) -> AbstractRobustQueue:
         await self._connection.ready()
+        await self.ready()
         queue: RobustQueue = await super().declare_queue(   # type: ignore
             name=name,
             durable=durable,
             exclusive=exclusive,
             passive=passive,
             auto_delete=auto_delete,
             arguments=arguments,
@@ -208,14 +248,15 @@
         queue_name: str,
         timeout: TimeoutType = None,
         if_unused: bool = False,
         if_empty: bool = False,
         nowait: bool = False,
     ) -> aiormq.spec.Queue.DeleteOk:
         await self._connection.ready()
+        await self.ready()
         result = await super().queue_delete(
             queue_name=queue_name,
             timeout=timeout,
             if_unused=if_unused,
             if_empty=if_empty,
             nowait=nowait,
         )
```

### Comparing `aio_pika-9.0.7/aio_pika/robust_connection.py` & `aio_pika-9.1.0/aio_pika/robust_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import aiormq.abc
 from aiormq.connection import parse_bool, parse_timeout
 from pamqp.common import FieldTable
 from yarl import URL
 
 from .abc import (
     AbstractRobustChannel, AbstractRobustConnection, SSLOptions, TimeoutType,
-    UnderlayConnection,
 )
 from .connection import Connection, make_url
 from .exceptions import CONNECTION_EXCEPTIONS
 from .log import get_logger
 from .robust_channel import RobustChannel
 from .tools import CallbackCollection
 
@@ -77,37 +76,42 @@
         log.info(
             "Connection to %s closed. Reconnecting after %r seconds.",
             self, self.reconnect_interval,
         )
 
         self.__connection_close_event.set()
 
-    async def _on_connected(self, transport: UnderlayConnection) -> None:
+    async def _on_connected(self) -> None:
+        await super()._on_connected()
+
+        transport = self.transport
+        if transport is None:
+            raise RuntimeError("No active transport for connection %r", self)
+
         try:
             for channel in self.__channels:
                 try:
-                    await channel.restore(transport.connection)
+                    await channel.restore()
                 except Exception:
                     log.exception("Failed to reopen channel")
                     raise
         except asyncio.CancelledError:
             # In python 3.7 asyncio.CancelledError inherited
             # from Exception and this needed for catch it first
             raise
         except Exception as e:
             closing = self.loop.create_future()
             closing.set_exception(e)
             await self.close_callbacks(closing)
             await asyncio.gather(
-                transport.connection.close(e), return_exceptions=True,
+                transport.connection.close(e),
+                return_exceptions=True,
             )
             raise
 
-        await super()._on_connected(transport)
-
         if self.connection_attempt:
             await self.reconnect_callbacks()
 
         self.connection_attempt += 1
         self.__connection_close_event.clear()
 
     async def __connection_factory(self) -> None:
@@ -201,14 +205,15 @@
     ) -> None:
         if self.__reconnection_task is not None:
             self.__reconnection_task.cancel()
             await asyncio.gather(
                 self.__reconnection_task, return_exceptions=True,
             )
             self.__reconnection_task = None
+
         return await super().close(exc)
 
 
 async def connect_robust(
     url: Union[str, URL, None] = None,
     *,
     host: str = "localhost",
@@ -316,15 +321,15 @@
             password=password,
             virtualhost=virtualhost,
             ssl=ssl,
             ssl_options=ssl_options,
             client_properties=client_properties,
             **kwargs,
         ),
-        loop=loop, ssl_context=ssl_context, **kwargs
+        loop=loop, ssl_context=ssl_context, **kwargs,
     )
 
     await connection.connect(timeout=timeout)
     return connection
 
 
 __all__ = (
```

### Comparing `aio_pika-9.0.7/aio_pika/robust_exchange.py` & `aio_pika-9.1.0/aio_pika/robust_exchange.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import asyncio
+import warnings
 from typing import Any, Dict, Union
 
 import aiormq
 from pamqp.common import Arguments
 
 from .abc import (
-    AbstractExchange, AbstractRobustExchange, ExchangeParamType, TimeoutType,
+    AbstractChannel, AbstractExchange, AbstractRobustExchange,
+    ExchangeParamType, TimeoutType,
 )
 from .exchange import Exchange, ExchangeType
 from .log import get_logger
 
 
 log = get_logger(__name__)
 
@@ -17,15 +19,15 @@
 class RobustExchange(Exchange, AbstractRobustExchange):
     """ Exchange abstraction """
 
     _bindings: Dict[Union[AbstractExchange, str], Dict[str, Any]]
 
     def __init__(
         self,
-        channel: aiormq.abc.AbstractChannel,
+        channel: AbstractChannel,
         name: str,
         type: Union[ExchangeType, str] = ExchangeType.DIRECT,
         *,
         auto_delete: bool = False,
         durable: bool = False,
         internal: bool = False,
         passive: bool = False,
@@ -41,29 +43,32 @@
             passive=passive,
             arguments=arguments,
         )
 
         self._bindings = {}
         self.__restore_lock = asyncio.Lock()
 
-    async def restore(self, channel: aiormq.abc.AbstractChannel) -> None:
+    async def restore(self, channel: Any = None) -> None:
+        if channel is not None:
+            warnings.warn(
+                "Channel argument will be ignored because you "
+                "don't need to pass this anymore.",
+                DeprecationWarning,
+            )
         async with self.__restore_lock:
             try:
-                self.channel = channel
-
                 # special case for default exchange
                 if self.name == "":
                     return
 
                 await self.declare()
 
                 for exchange, kwargs in tuple(self._bindings.items()):
                     await self.bind(exchange, **kwargs)
             except Exception:
-                del self.channel
                 raise
 
     async def bind(
         self,
         exchange: ExchangeParamType,
         routing_key: str = "",
         *,
```

### Comparing `aio_pika-9.0.7/aio_pika/robust_queue.py` & `aio_pika-9.1.0/aio_pika/robust_queue.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import warnings
 from random import Random
-from typing import Any, Callable, Dict, Optional, Tuple, Union
+from typing import Any, Awaitable, Callable, Dict, Optional, Tuple, Union
 
 import aiormq
 from aiormq import ChannelInvalidStateError
 from pamqp.common import Arguments
 
 from .abc import (
-    AbstractExchange, AbstractIncomingMessage, AbstractQueueIterator,
-    AbstractRobustQueue, ConsumerTag, TimeoutType,
+    AbstractChannel, AbstractExchange, AbstractIncomingMessage,
+    AbstractQueueIterator, AbstractRobustQueue, ConsumerTag, TimeoutType,
 )
 from .exchange import ExchangeParamType
 from .log import get_logger
 from .queue import Queue, QueueIterator
 
 
 log = get_logger(__name__)
@@ -28,15 +29,15 @@
     @classmethod
     def _get_random_queue_name(cls) -> str:
         rnd = cls._rnd_gen.getrandbits(128)
         return "amq_%s" % hex(rnd).lower()
 
     def __init__(
         self,
-        channel: aiormq.abc.AbstractChannel,
+        channel: AbstractChannel,
         name: Optional[str],
         durable: bool = False,
         exclusive: bool = False,
         auto_delete: bool = False,
         arguments: Arguments = None,
         passive: bool = False,
     ):
@@ -50,16 +51,22 @@
             arguments=arguments,
             passive=passive,
         )
 
         self._consumers = {}
         self._bindings = {}
 
-    async def restore(self, channel: aiormq.abc.AbstractChannel) -> None:
-        self.channel = channel
+    async def restore(self, channel: Any = None) -> None:
+        if channel is not None:
+            warnings.warn(
+                "Channel argument will be ignored because you "
+                "don't need to pass this anymore.",
+                DeprecationWarning,
+            )
+
         await self.declare()
         bindings = tuple(self._bindings.items())
         consumers = tuple(self._consumers.items())
 
         for (exchange, routing_key), kwargs in bindings:
             await self.bind(exchange, routing_key, **kwargs)
 
@@ -105,15 +112,15 @@
         )
         self._bindings.pop((exchange, routing_key), None)
 
         return result
 
     async def consume(
         self,
-        callback: Callable[[AbstractIncomingMessage], Any],
+        callback: Callable[[AbstractIncomingMessage], Awaitable[Any]],
         no_ack: bool = False,
         exclusive: bool = False,
         arguments: Arguments = None,
         consumer_tag: Optional[ConsumerTag] = None,
         timeout: TimeoutType = None,
         robust: bool = True,
     ) -> ConsumerTag:
@@ -152,11 +159,11 @@
 
 class RobustQueueIterator(QueueIterator):
     async def consume(self) -> None:
         while True:
             try:
                 return await super().consume()
             except ChannelInvalidStateError:
-                await self._amqp_queue.channel.connection.ready()
+                await self._amqp_queue.channel.get_underlay_channel()
 
 
 __all__ = ("RobustQueue",)
```

### Comparing `aio_pika-9.0.7/aio_pika/transaction.py` & `aio_pika-9.1.0/aio_pika/transaction.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,30 +29,33 @@
             raise RuntimeError("Closed channel")
 
         return self.__channel
 
     async def select(
         self, timeout: TimeoutType = None,
     ) -> aiormq.spec.Tx.SelectOk:
-        result = await self.channel.channel.tx_select(timeout=timeout)
+        channel = await self.channel.get_underlay_channel()
+        result = await channel.tx_select(timeout=timeout)
 
         self.state = TransactionState.STARTED
         return result
 
     async def rollback(
         self, timeout: TimeoutType = None,
     ) -> commands.Tx.RollbackOk:
-        result = await self.channel.channel.tx_rollback(timeout=timeout)
+        channel = await self.channel.get_underlay_channel()
+        result = await channel.tx_rollback(timeout=timeout)
         self.state = TransactionState.ROLLED_BACK
         return result
 
     async def commit(
         self, timeout: TimeoutType = None,
     ) -> commands.Tx.CommitOk:
-        result = await self.channel.channel.tx_commit(timeout=timeout)
+        channel = await self.channel.get_underlay_channel()
+        result = await channel.tx_commit(timeout=timeout)
         self.state = TransactionState.COMMITED
         return result
 
     async def __aenter__(self) -> "Transaction":
         await self.select()
         return self
```

### Comparing `aio_pika-9.0.7/pyproject.toml` & `aio_pika-9.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-pika"
-version = "9.0.7"
+version = "9.1.0"
 description = "Wrapper around the aiormq for asyncio and humans"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.rst"
 license = "Apache-2.0"
 keywords=["rabbitmq", "asyncio", "amqp", "amqp 0.9.1", "aiormq"]
 homepage = "https://github.com/mosquito/aio-pika"
 classifiers = [
@@ -41,15 +41,15 @@
 yarl = [{ version = '*'}]
 typing_extensions = [{ version = '*', python = "< 3.8" }]
 # for pkg_resources
 setuptools = [{ version = '*', python = "< 3.8" }]
 
 [tool.poetry.group.dev.dependencies]
 aiomisc = "^17.2"
-aiomisc-pytest = "*"
+aiomisc-pytest = "^1.1.1"
 collective-checkdocs = "^0.2"
 coverage = "^6.5.0"
 coveralls = "^3.3.1"
 mypy = "^0.991"
 nox = "^2022.11.21"
 pylama = "^8.4.1"
 pytest = "^7.2.0"
```

### Comparing `aio_pika-9.0.7/PKG-INFO` & `aio_pika-9.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-pika
-Version: 9.0.7
+Version: 9.1.0
 Summary: Wrapper around the aiormq for asyncio and humans
 Home-page: https://github.com/mosquito/aio-pika
 License: Apache-2.0
 Keywords: rabbitmq,asyncio,amqp,amqp 0.9.1,aiormq
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.7,<4.0
```

