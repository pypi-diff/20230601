# Comparing `tmp/bitcoinrpc-0.5.0.tar.gz` & `tmp/bitcoinrpc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoinrpc-0.5.0.tar", last modified: Tue Dec 28 10:11:22 2021, max compression
+gzip compressed data, was "bitcoinrpc-0.6.0.tar", last modified: Thu Jun  1 13:45:08 2023, max compression
```

## Comparing `bitcoinrpc-0.5.0.tar` & `bitcoinrpc-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxr-x   0 libor     (1000) libor     (1000)        0 2021-12-28 10:11:22.753707 bitcoinrpc-0.5.0/
--rw-rw-r--   0 libor     (1000) libor     (1000)     1080 2020-09-18 22:13:07.000000 bitcoinrpc-0.5.0/LICENSE
--rw-rw-r--   0 libor     (1000) libor     (1000)     3271 2021-12-28 10:11:22.753707 bitcoinrpc-0.5.0/PKG-INFO
--rw-rw-r--   0 libor     (1000) libor     (1000)     2412 2021-12-28 10:08:22.000000 bitcoinrpc-0.5.0/README.md
--rw-rw-r--   0 libor     (1000) libor     (1000)      510 2021-12-28 10:11:22.753707 bitcoinrpc-0.5.0/setup.cfg
--rw-rw-r--   0 libor     (1000) libor     (1000)     2004 2021-12-28 10:08:22.000000 bitcoinrpc-0.5.0/setup.py
-drwxrwxr-x   0 libor     (1000) libor     (1000)        0 2021-12-28 10:11:22.749707 bitcoinrpc-0.5.0/src/
-drwxrwxr-x   0 libor     (1000) libor     (1000)        0 2021-12-28 10:11:22.753707 bitcoinrpc-0.5.0/src/bitcoinrpc/
--rw-rw-r--   0 libor     (1000) libor     (1000)      225 2021-04-14 00:06:45.000000 bitcoinrpc-0.5.0/src/bitcoinrpc/__init__.py
--rw-rw-r--   0 libor     (1000) libor     (1000)       22 2021-12-28 10:08:22.000000 bitcoinrpc-0.5.0/src/bitcoinrpc/__version__.py
--rw-rw-r--   0 libor     (1000) libor     (1000)      190 2020-10-04 13:05:46.000000 bitcoinrpc-0.5.0/src/bitcoinrpc/_exceptions.py
--rw-rw-r--   0 libor     (1000) libor     (1000)     3953 2021-12-28 10:08:22.000000 bitcoinrpc-0.5.0/src/bitcoinrpc/_types.py
--rw-rw-r--   0 libor     (1000) libor     (1000)     8072 2021-12-28 10:08:22.000000 bitcoinrpc-0.5.0/src/bitcoinrpc/bitcoin_rpc.py
-drwxrwxr-x   0 libor     (1000) libor     (1000)        0 2021-12-28 10:11:22.753707 bitcoinrpc-0.5.0/src/bitcoinrpc.egg-info/
--rw-rw-r--   0 libor     (1000) libor     (1000)     3271 2021-12-28 10:11:22.000000 bitcoinrpc-0.5.0/src/bitcoinrpc.egg-info/PKG-INFO
--rw-rw-r--   0 libor     (1000) libor     (1000)      367 2021-12-28 10:11:22.000000 bitcoinrpc-0.5.0/src/bitcoinrpc.egg-info/SOURCES.txt
--rw-rw-r--   0 libor     (1000) libor     (1000)        1 2021-12-28 10:11:22.000000 bitcoinrpc-0.5.0/src/bitcoinrpc.egg-info/dependency_links.txt
--rw-rw-r--   0 libor     (1000) libor     (1000)       45 2021-12-28 10:11:22.000000 bitcoinrpc-0.5.0/src/bitcoinrpc.egg-info/requires.txt
--rw-rw-r--   0 libor     (1000) libor     (1000)       11 2021-12-28 10:11:22.000000 bitcoinrpc-0.5.0/src/bitcoinrpc.egg-info/top_level.txt
+drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-01 13:45:08.246614 bitcoinrpc-0.6.0/
+-rw-rw-r--   0 boi       (1000) boi       (1000)     1080 2023-05-21 10:38:52.000000 bitcoinrpc-0.6.0/LICENSE
+-rw-rw-r--   0 boi       (1000) boi       (1000)     6810 2023-06-01 13:45:08.246614 bitcoinrpc-0.6.0/PKG-INFO
+-rw-rw-r--   0 boi       (1000) boi       (1000)     5920 2023-06-01 13:44:53.000000 bitcoinrpc-0.6.0/README.md
+-rw-rw-r--   0 boi       (1000) boi       (1000)      576 2023-06-01 13:45:08.246614 bitcoinrpc-0.6.0/setup.cfg
+-rw-rw-r--   0 boi       (1000) boi       (1000)     2054 2023-06-01 13:44:53.000000 bitcoinrpc-0.6.0/setup.py
+drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-01 13:45:08.242614 bitcoinrpc-0.6.0/src/
+drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-01 13:45:08.246614 bitcoinrpc-0.6.0/src/bitcoinrpc/
+-rw-rw-r--   0 boi       (1000) boi       (1000)      205 2023-06-01 13:38:04.000000 bitcoinrpc-0.6.0/src/bitcoinrpc/__init__.py
+-rw-rw-r--   0 boi       (1000) boi       (1000)       22 2023-06-01 13:44:53.000000 bitcoinrpc-0.6.0/src/bitcoinrpc/__version__.py
+-rw-rw-r--   0 boi       (1000) boi       (1000)      140 2023-06-01 13:38:04.000000 bitcoinrpc-0.6.0/src/bitcoinrpc/_exceptions.py
+-rw-rw-r--   0 boi       (1000) boi       (1000)     3953 2023-05-21 10:38:52.000000 bitcoinrpc-0.6.0/src/bitcoinrpc/_types.py
+-rw-rw-r--   0 boi       (1000) boi       (1000)     8280 2023-06-01 13:38:12.000000 bitcoinrpc-0.6.0/src/bitcoinrpc/bitcoin_rpc.py
+drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-01 13:45:08.246614 bitcoinrpc-0.6.0/src/bitcoinrpc.egg-info/
+-rw-rw-r--   0 boi       (1000) boi       (1000)     6810 2023-06-01 13:45:08.000000 bitcoinrpc-0.6.0/src/bitcoinrpc.egg-info/PKG-INFO
+-rw-rw-r--   0 boi       (1000) boi       (1000)      420 2023-06-01 13:45:08.000000 bitcoinrpc-0.6.0/src/bitcoinrpc.egg-info/SOURCES.txt
+-rw-rw-r--   0 boi       (1000) boi       (1000)        1 2023-06-01 13:45:08.000000 bitcoinrpc-0.6.0/src/bitcoinrpc.egg-info/dependency_links.txt
+-rw-rw-r--   0 boi       (1000) boi       (1000)       45 2023-06-01 13:45:08.000000 bitcoinrpc-0.6.0/src/bitcoinrpc.egg-info/requires.txt
+-rw-rw-r--   0 boi       (1000) boi       (1000)       11 2023-06-01 13:45:08.000000 bitcoinrpc-0.6.0/src/bitcoinrpc.egg-info/top_level.txt
+drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-01 13:45:08.246614 bitcoinrpc-0.6.0/tests/
+-rw-rw-r--   0 boi       (1000) boi       (1000)      800 2023-06-01 13:38:04.000000 bitcoinrpc-0.6.0/tests/test_client_config.py
+-rw-rw-r--   0 boi       (1000) boi       (1000)     1603 2023-06-01 13:38:12.000000 bitcoinrpc-0.6.0/tests/test_connection.py
```

### Comparing `bitcoinrpc-0.5.0/LICENSE` & `bitcoinrpc-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoinrpc-0.5.0/setup.py` & `bitcoinrpc-0.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     url="https://github.com/bibajz/bitcoin-python-async-rpc",
     author="Libor Martinek",
     author_email="libasmartinek@protonmail.com",
     package_dir={"": "src"},
```

### Comparing `bitcoinrpc-0.5.0/src/bitcoinrpc/_types.py` & `bitcoinrpc-0.6.0/src/bitcoinrpc/_types.py`

 * *Files identical despite different names*

### Comparing `bitcoinrpc-0.5.0/src/bitcoinrpc/bitcoin_rpc.py` & `bitcoinrpc-0.6.0/src/bitcoinrpc/bitcoin_rpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import itertools
 from types import TracebackType
-from typing import Any, List, Optional, Type, Union
+from typing import Any, Callable, List, Optional, Tuple, Type, Union
 
 import httpx
 import orjson
-from typing_extensions import Literal
+from typing_extensions import Literal, Self
 
-from ._exceptions import ImproperlyConfigured, RPCError
-from ._types import (
+from bitcoinrpc._exceptions import RPCError
+from bitcoinrpc._types import (
     BestBlockHash,
     BitcoinRPCResponse,
     Block,
     BlockchainInfo,
     BlockCount,
     BlockHash,
     BlockHeader,
@@ -28,66 +28,66 @@
 
 # Neat trick found in asyncio library for task enumeration
 # https://github.com/python/cpython/blob/3.8/Lib/asyncio/tasks.py#L31
 _next_rpc_id = itertools.count(1).__next__
 
 
 class BitcoinRPC:
-    __slots__ = ("_url", "_client")
+    __slots__ = ("_url", "_client", "_counter")
     """
+    Class representing a JSON-RPC client of a Bitcoin node.
+
+    :param url: URL of the Bitcoin node.
+    :param client: Underlying `httpx.AsyncClient`, which handles the requests issued.
+    :param counter: Optional callable that serves as a generator for the "id" field within JSON-RPC requests.
+
     For list of all available commands, visit:
     https://developer.bitcoin.org/reference/rpc/index.html
     """
 
     def __init__(
         self,
         url: str,
-        rpc_user: str,
-        rpc_password: str,
-        **options: Any,
+        client: httpx.AsyncClient,
+        counter: Callable[[], Union[int, str]] = _next_rpc_id,
     ) -> None:
         self._url = url
-        self._client = self._configure_client(rpc_user, rpc_password, **options)
+        self._client = client
+        self._counter = counter
 
     async def __aenter__(self) -> "BitcoinRPC":
         return self
 
     async def __aexit__(
         self,
         exc_type: Type[BaseException],
         exc_val: BaseException,
         exc_tb: TracebackType,
     ) -> None:
         await self.aclose()
 
-    @staticmethod
-    def _configure_client(
-        rpc_user: str, rpc_password: str, **options: Any
-    ) -> httpx.AsyncClient:
+    @classmethod
+    def from_config(
+        cls,
+        url: str,
+        auth: Optional[Tuple[str, str]],
+        **options: Any,
+    ) -> Self:
         """
-        Configure `httpx.AsyncClient`. If you choose to provide additional options, it
-        is your responsibility to conform to the `httpx.AsyncClient` interface.
+        Instantiate the `BitcoinRPC` client while also configuring the underlying `httpx.AsyncClient`. Additional
+        options are passed directly as kwargs to `httpx.AsyncClient`, so it's your responsibility to conform to its
+        interface.
         """
-        auth = (rpc_user, rpc_password)
-        headers = {"content-type": "application/json"}
 
         options = dict(options)
-        if not options:
-            return httpx.AsyncClient(auth=auth, headers=headers)
-
-        if "auth" in options:
-            raise ImproperlyConfigured("Authentication cannot be set via options!")
-
-        if "headers" in options:
-            _additional_headers = dict(options.pop("headers"))
-            headers.update(_additional_headers)
-            # guard against content-type overwrite
-            headers["content-type"] = "application/json"
-
-        return httpx.AsyncClient(auth=auth, headers=headers, **options)
+        headers = {
+            "content-type": "application/json",
+            **dict(options.pop("headers", {})),
+        }
+        return cls(url, httpx.AsyncClient(auth=auth, headers=headers, **options))
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
     def client(self) -> httpx.AsyncClient:
@@ -102,32 +102,36 @@
         params: List[Union[str, int, List[str], None]],
         **kwargs: Any,
     ) -> BitcoinRPCResponse:
         """
         Pass keyword arguments to directly modify the constructed request -
             see `httpx.Request`.
         """
-        req = self.client.post(
+        response = await self.client.post(
             url=self.url,
             content=orjson.dumps(
                 {
                     "jsonrpc": "2.0",
-                    "id": _next_rpc_id(),
+                    "id": self._counter(),
                     "method": method,
                     "params": params,
                 }
             ),
             **kwargs,
         )
-        resp = orjson.loads((await req).content)
 
-        if resp["error"] is not None:
-            raise RPCError(resp["error"]["code"], resp["error"]["message"])
+        # Raise an exception if return code is not in 2xx range
+        # https://www.python-httpx.org/quickstart/#exceptions
+        response.raise_for_status()
+
+        content = orjson.loads(response.content)
+        if content["error"] is not None:
+            raise RPCError(content["error"]["code"], content["error"]["message"])
         else:
-            return resp["result"]
+            return content["result"]
 
     async def getmempoolinfo(self) -> MempoolInfo:
         """https://developer.bitcoin.org/reference/rpc/getmempoolinfo.html"""
         return await self.acall("getmempoolinfo", [])
 
     async def getmininginfo(self) -> MiningInfo:
         """https://developer.bitcoin.org/reference/rpc/getmininginfo.html"""
```

