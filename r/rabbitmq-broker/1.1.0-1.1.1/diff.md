# Comparing `tmp/rabbitmq_broker-1.1.0-py3-none-any.whl.zip` & `tmp/rabbitmq_broker-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 10568 bytes, number of entries: 15
--rw-r--r--  2.0 unx       22 b- defN 23-May-31 15:11 rmq_broker/__init__.py
+Zip file size: 10580 bytes, number of entries: 15
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-01 12:35 rmq_broker/__init__.py
 -rw-r--r--  2.0 unx     1080 b- defN 23-May-31 15:11 rmq_broker/schemas.py
 -rw-r--r--  2.0 unx      508 b- defN 23-May-26 07:16 rmq_broker/settings.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/async_chains/__init__.py
--rw-r--r--  2.0 unx     8374 b- defN 23-May-31 15:11 rmq_broker/async_chains/base.py
+-rw-r--r--  2.0 unx     8353 b- defN 23-Jun-01 12:35 rmq_broker/async_chains/base.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/chains/__init__.py
--rw-r--r--  2.0 unx     4259 b- defN 23-May-31 15:11 rmq_broker/chains/base.py
+-rw-r--r--  2.0 unx     4283 b- defN 23-Jun-01 12:35 rmq_broker/chains/base.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/queues/__init__.py
 -rw-r--r--  2.0 unx     1107 b- defN 23-May-26 07:16 rmq_broker/queues/base.py
 -rw-r--r--  2.0 unx     1765 b- defN 23-May-26 07:16 rmq_broker/queues/rabbitmq.py
--rw-r--r--  2.0 unx     1074 b- defN 23-May-31 15:12 rabbitmq_broker-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4405 b- defN 23-May-31 15:12 rabbitmq_broker-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-31 15:12 rabbitmq_broker-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-31 15:12 rabbitmq_broker-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1252 b- defN 23-May-31 15:12 rabbitmq_broker-1.1.0.dist-info/RECORD
-15 files, 23949 bytes uncompressed, 8472 bytes compressed:  64.6%
+-rw-r--r--  2.0 unx     1074 b- defN 23-Jun-01 12:36 rabbitmq_broker-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4405 b- defN 23-Jun-01 12:36 rabbitmq_broker-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 12:36 rabbitmq_broker-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-01 12:36 rabbitmq_broker-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1252 b- defN 23-Jun-01 12:36 rabbitmq_broker-1.1.1.dist-info/RECORD
+15 files, 23952 bytes uncompressed, 8484 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: rmq_broker/queues/base.py
 Comment: 
 
 Filename: rmq_broker/queues/rabbitmq.py
 Comment: 
 
-Filename: rabbitmq_broker-1.1.0.dist-info/LICENSE
+Filename: rabbitmq_broker-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: rabbitmq_broker-1.1.0.dist-info/METADATA
+Filename: rabbitmq_broker-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: rabbitmq_broker-1.1.0.dist-info/WHEEL
+Filename: rabbitmq_broker-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: rabbitmq_broker-1.1.0.dist-info/top_level.txt
+Filename: rabbitmq_broker-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rabbitmq_broker-1.1.0.dist-info/RECORD
+Filename: rabbitmq_broker-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rmq_broker/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.0"
+__version__ = "1.1.1"
```

## rmq_broker/async_chains/base.py

```diff
@@ -34,17 +34,17 @@
         Добавляет нового обработчика в цепочку.
         Args:
             chain: Экземпляр обработчика.
 
         Returns:
             None
         """
-        self.chains[chain.request_type] = chain
+        self.chains[chain.request_type.lower()] = chain
         logger.debug(
-            f"{self.__class__.__name__}.add(): {chain.__class__.__name__} added to chains."
+            f"{self.__class__.__name__}.add(): {chain.__name__} added to chains."
         )
 
     @abstractmethod
     async def handle(self, data: IncomingMessage) -> OutgoingMessage:
         """
         Вызывает метод handle() у следующего обработчика в цепочке.
 
@@ -208,22 +208,22 @@
     chains = {}
 
     def __init__(self, parent_chain: BaseChain = BaseChain) -> None:
         """Собирает все обработчики в словарь."""
         if subclasses := parent_chain.__subclasses__():
             for subclass in subclasses:
                 if subclass.request_type:
-                    self.chains[subclass.request_type] = subclass
+                    self.add(subclass)
                 self.__init__(subclass)
 
     async def handle(self, data: IncomingMessage) -> OutgoingMessage:
         """Направляет запрос на нужный обработчик."""
         try:
             self.validate(data, PreMessage)
-            chain = self.chains[data["request_type"]]
+            chain = self.chains[data["request_type"].lower()]
             return await chain().handle(data)
         except SchemaError as e:
             msg = f"Incoming message validation error: {e}"
         except KeyError as e:
             msg = f"Can't handle this request type: {e}"
         logger.error(f"{self.__class__.__name__}.handle(): {msg}")
         return self.form_response(
```

## rmq_broker/chains/base.py

```diff
@@ -40,15 +40,15 @@
             self.validate(data, PreMessage)
         except SchemaError as e:
             logger.error(f"{self.__class__.__name__}.handle(): SchemaError: {e}")
             return self.form_response(
                 MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
             )
         response = {}
-        if self.request_type == data["request_type"]:
+        if self.request_type.lower() == data["request_type"].lower():
             response["request_id"] = data["request_id"]
             response["request_type"] = data["request_type"]
             try:
                 response.update(self.get_response_body(data))
                 logger.debug(
                     f"{self.__class__.__name__}.handle(): After body update {response=}"
                 )
@@ -87,15 +87,15 @@
 class ChainManager(AsyncChainManager):
     """Синхронная версия менеджера распределения запросов."""
 
     def handle(self, data: IncomingMessage) -> OutgoingMessage:
         """Направляет запрос на нужный обработчик."""
         try:
             self.validate(data, PreMessage)
-            chain = self.chains[data["request_type"]]
+            chain = self.chains[data["request_type"].lower()]
             return chain().handle(data)
         except SchemaError as e:
             msg = f"Incoming message validation error: {e}"
         except KeyError as e:
             msg = f"Can't handle this request type: {e}"
         logger.error(f"{self.__class__.__name__}: handle(data): {msg}")
         return self.form_response(
```

## Comparing `rabbitmq_broker-1.1.0.dist-info/LICENSE` & `rabbitmq_broker-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rabbitmq_broker-1.1.0.dist-info/METADATA` & `rabbitmq_broker-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitmq-broker
-Version: 1.1.0
+Version: 1.1.1
 Summary: RPC брокер сообщений
 Author-email: Nikita Sysoev <njt55cs@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

## Comparing `rabbitmq_broker-1.1.0.dist-info/RECORD` & `rabbitmq_broker-1.1.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-rmq_broker/__init__.py,sha256=LGVQyDsWifdACo7qztwb8RWWHds1E7uQ-ZqD8SAjyw4,22
+rmq_broker/__init__.py,sha256=q8_5C0f-8mHWNb6mMw02zlYPnEGXBqvOmP3z0CEwZKM,22
 rmq_broker/schemas.py,sha256=1XNpJKdyX34IU1RGnpVpYdH5LgzQfejDT7pAi27_mWg,1080
 rmq_broker/settings.py,sha256=kqSzECBSLWz6n7jjpuDzIM_Fvn_BQqtlR19axAia2Cc,508
 rmq_broker/async_chains/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rmq_broker/async_chains/base.py,sha256=aCHS5tnUb1m5WXO6jQ6b1rlRdwSAq_Gg-7g0321VZVk,8374
+rmq_broker/async_chains/base.py,sha256=cKzrVMoh2kiGrmOIpQ4Sr31QUx_d5fKsi00oO8IeDKs,8353
 rmq_broker/chains/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rmq_broker/chains/base.py,sha256=AU2_JNx2w2Qz9hS44g83EBCPiL1Uv3CNLg3JtGJMsHE,4259
+rmq_broker/chains/base.py,sha256=EOYBWp5BkSVM8lZNafldfR7F-V9ve7bUHaxWCLNyHF0,4283
 rmq_broker/queues/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rmq_broker/queues/base.py,sha256=XgUIn04MxoulYjN-v8LVcPKprmiSHy9UmKTzoBfyBug,1107
 rmq_broker/queues/rabbitmq.py,sha256=cujY9KKwld146SEyCHhcXe08cgHxRn3ARIxOfXuIViQ,1765
-rabbitmq_broker-1.1.0.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-rabbitmq_broker-1.1.0.dist-info/METADATA,sha256=HZ3Wfk0nfdlK8CgRmEPgocyOTWt1lszlYvfiCHk3o-s,4405
-rabbitmq_broker-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rabbitmq_broker-1.1.0.dist-info/top_level.txt,sha256=gyiGN4_aIuuxH76M_A_yn64Bxy2nj4fFJ1C84g3BPQQ,11
-rabbitmq_broker-1.1.0.dist-info/RECORD,,
+rabbitmq_broker-1.1.1.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+rabbitmq_broker-1.1.1.dist-info/METADATA,sha256=PJIfh7luzrzUOwHVtOkh3auveHSvmRSC-v6aZ4ESWjU,4405
+rabbitmq_broker-1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rabbitmq_broker-1.1.1.dist-info/top_level.txt,sha256=gyiGN4_aIuuxH76M_A_yn64Bxy2nj4fFJ1C84g3BPQQ,11
+rabbitmq_broker-1.1.1.dist-info/RECORD,,
```

