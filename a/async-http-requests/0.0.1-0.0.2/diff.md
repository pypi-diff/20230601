# Comparing `tmp/async-http-requests-0.0.1.tar.gz` & `tmp/async-http-requests-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-http-requests-0.0.1.tar", last modified: Sun Apr 16 17:04:52 2023, max compression
+gzip compressed data, was "async-http-requests-0.0.2.tar", last modified: Thu Jun  1 14:24:08 2023, max compression
```

## Comparing `async-http-requests-0.0.1.tar` & `async-http-requests-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-04-16 17:04:52.731696 async-http-requests-0.0.1/
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     1078 2023-04-13 10:12:28.000000 async-http-requests-0.0.1/LICENSE
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       17 2023-04-14 15:28:46.000000 async-http-requests-0.0.1/MANIFEST.in
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5168 2023-04-16 17:04:52.731696 async-http-requests-0.0.1/PKG-INFO
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     3413 2023-04-16 16:58:44.000000 async-http-requests-0.0.1/README.md
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      854 2023-04-16 17:01:18.000000 async-http-requests-0.0.1/pyproject.toml
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       38 2023-04-16 17:04:52.731696 async-http-requests-0.0.1/setup.cfg
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       38 2023-04-13 22:04:33.000000 async-http-requests-0.0.1/setup.py
-drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-04-16 17:04:52.731696 async-http-requests-0.0.1/src/
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5226 2023-04-16 16:18:11.000000 async-http-requests-0.0.1/src/AsyncRequests.py
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      608 2023-04-14 09:22:32.000000 async-http-requests-0.0.1/src/RequestObject.py
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      476 2023-04-14 10:05:37.000000 async-http-requests-0.0.1/src/RequestsType.py
-drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-04-16 17:04:52.731696 async-http-requests-0.0.1/src/async_http_requests.egg-info/
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5168 2023-04-16 17:04:52.000000 async-http-requests-0.0.1/src/async_http_requests.egg-info/PKG-INFO
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      376 2023-04-16 17:04:52.000000 async-http-requests-0.0.1/src/async_http_requests.egg-info/SOURCES.txt
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)        1 2023-04-16 17:04:52.000000 async-http-requests-0.0.1/src/async_http_requests.egg-info/dependency_links.txt
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      144 2023-04-16 17:04:52.000000 async-http-requests-0.0.1/src/async_http_requests.egg-info/requires.txt
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       48 2023-04-16 17:04:52.000000 async-http-requests-0.0.1/src/async_http_requests.egg-info/top_level.txt
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      459 2023-04-13 16:22:15.000000 async-http-requests-0.0.1/src/helper.py
-drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-04-16 17:04:52.731696 async-http-requests-0.0.1/test/
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     1213 2023-04-14 16:02:07.000000 async-http-requests-0.0.1/test/test.py
+drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-06-01 14:24:08.582024 async-http-requests-0.0.2/
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     1078 2023-04-13 10:12:28.000000 async-http-requests-0.0.2/LICENSE
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       17 2023-04-14 15:28:46.000000 async-http-requests-0.0.2/MANIFEST.in
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5148 2023-06-01 14:24:08.582024 async-http-requests-0.0.2/PKG-INFO
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     3413 2023-04-16 16:58:44.000000 async-http-requests-0.0.2/README.md
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      858 2023-05-31 11:31:14.000000 async-http-requests-0.0.2/pyproject.toml
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       38 2023-06-01 14:24:08.582024 async-http-requests-0.0.2/setup.cfg
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       38 2023-04-13 22:04:33.000000 async-http-requests-0.0.2/setup.py
+drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-06-01 14:24:08.578024 async-http-requests-0.0.2/src/
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5741 2023-06-01 13:29:55.000000 async-http-requests-0.0.2/src/AsyncRequests.py
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      608 2023-04-14 09:22:32.000000 async-http-requests-0.0.2/src/RequestObject.py
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      476 2023-04-14 10:05:37.000000 async-http-requests-0.0.2/src/RequestsType.py
+drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-06-01 14:24:08.582024 async-http-requests-0.0.2/src/async_http_requests.egg-info/
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5148 2023-06-01 14:24:08.000000 async-http-requests-0.0.2/src/async_http_requests.egg-info/PKG-INFO
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      376 2023-06-01 14:24:08.000000 async-http-requests-0.0.2/src/async_http_requests.egg-info/SOURCES.txt
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)        1 2023-06-01 14:24:08.000000 async-http-requests-0.0.2/src/async_http_requests.egg-info/dependency_links.txt
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      100 2023-06-01 14:24:08.000000 async-http-requests-0.0.2/src/async_http_requests.egg-info/requires.txt
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       48 2023-06-01 14:24:08.000000 async-http-requests-0.0.2/src/async_http_requests.egg-info/top_level.txt
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      459 2023-04-13 16:22:15.000000 async-http-requests-0.0.2/src/helper.py
+drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-06-01 14:24:08.582024 async-http-requests-0.0.2/test/
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     1625 2023-06-01 13:32:21.000000 async-http-requests-0.0.2/test/test.py
```

### Comparing `async-http-requests-0.0.1/LICENSE` & `async-http-requests-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async-http-requests-0.0.1/PKG-INFO` & `async-http-requests-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-http-requests
-Version: 0.0.1
+Version: 0.0.2
 Summary: Asynchronous HTTP requests
 Author-email: Andrea Sergi <andrea.serg1@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 sclash - Andrea Sergi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,15 +28,14 @@
 Project-URL: Homepage, https://github.com/sclash/AsyncRequests
 Keywords: http,requests,api,asyncio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
 
 # Async Requests
 
 Python library to handle asynchronous http requests, built on top of the [requests](https://requests.readthedocs.io/en/latest/) library
```

### Comparing `async-http-requests-0.0.1/README.md` & `async-http-requests-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `async-http-requests-0.0.1/pyproject.toml` & `async-http-requests-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "async-http-requests"
-version = "0.0.1"
+version = "0.0.2"
 description = "Asynchronous HTTP requests"
 readme = "README.md"
 authors = [{ name = "Andrea Sergi", email = "andrea.serg1@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -20,12 +20,12 @@
     'requests>=2.28.0',
     'requests-oauthlib>=1.3.0',
     'dataclasses>=0.6',
     'tomli>=2.0.1; python_version < "3.11"',
 ]
 requires-python = ">=3.9"
 
-[project.optional-dependencies]
-dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
+# [project.optional-dependencies]
+# dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/sclash/AsyncRequests"
```

### Comparing `async-http-requests-0.0.1/src/AsyncRequests.py` & `async-http-requests-0.0.2/src/AsyncRequests.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from helper import split_chunk
 
 from typing import List, Callable, Optional
 
 from RequestsType import RequestType
 from RequestObject import RequestObject
 from dataclasses import asdict
+import pandas as pd
 
 import logging
 
 c_handler = logging.StreamHandler()
 c_format = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(funcName)s - %(lineno)s - %(message)s', datefmt= '%d-%m-%Y %H:%M:%S')
 c_handler.setFormatter(c_format)
 logger = logging.getLogger(__name__)
@@ -33,43 +34,48 @@
         self.request_type = request_type
         self.queue = asyncio.Queue()
         self.N_PRODUCERS = N_PRODUCERS
         self.N_CONSUMERS = N_CONSUMERS
         self.url_chunk = split_chunk(self.url, self.N_PRODUCERS)
         self.response = []
         self.error_response = []
+        self.error_data: pd.DataFrame = None
 
     def sync_http(self, r_obj: RequestObject, **fixed_kwargs):
         try:
             url = r_obj.url
             var_kwargs = {k: asdict(r_obj)[k] for k in asdict(r_obj).keys() if k != 'url' and asdict(r_obj)[k]!=None} 
             # kwargs = {k: asdict(r_obj)[k] for k in asdict(r_obj).keys() if k != 'url'} | fixed_kwargs
             kwargs = var_kwargs | fixed_kwargs
             r = self.request_type(url, **kwargs)
             r.raise_for_status()
             logger.info(f"SUCCESSFULL Request for {r_obj.url} - {var_kwargs}")
             return r
         except Exception as e:
-            self.error_response.append((r_obj, r.status_code))
+            # self.error_response.append((r_obj, r.status_code))
+            self.error_response.append((r_obj) )
+
             logger.error(f"Request ERROR for {r_obj.url}: {e}")
-            return r.status_code
+            # return r.status_code
     
     async def __async_http_thread(self, r_obj: RequestObject, **fixed_kwargs):
         return await asyncio.to_thread(self.sync_http, r_obj , **fixed_kwargs)
     
     async def __produce(self, chunk: List[RequestObject], **fixed_kwargs):
         try:
             for r_obj in chunk:
                 r = await self.__async_http_thread(r_obj, **fixed_kwargs)
                 if r:
                     await self.queue.put(r)
                 else:
                     await self.queue.put(None)
         except Exception as e:
-            self.error_response.append((r_obj, r.status_code))
+            # self.error_response.append((r_obj, r.status_code))
+            # self.error_response.append(asdict(r_obj)| {'status_code': r.status_code, 'response': r.text})
+            self.error_response.append((r_obj))
             logger.error(f"PRODUCER ERROR: {r_obj}")
             print(e)
 
     async def __consume(self, callback: Optional[Callable] = None):
         while True:
             try:
                 data = await self.queue.get()
@@ -91,14 +97,19 @@
         consumers = [asyncio.create_task(self.__consume(callback)) for i in range(self.N_CONSUMERS)]
         await asyncio.gather(*producers)
         
         await self.queue.join()
         for c in consumers:
             c.cancel()
 
+        if len(self.error_response) > 0:
+            self.error_data = pd.DataFrame()
+            for err in self.error_response:
+                self.error_data = pd.concat([self.error_data, pd.DataFrame(asdict(err)) ])
+                
 
 class AsyncHTTP(AsyncRequests):
 
     def __init__(self, url: List[RequestObject], N_PRODUCERS, N_CONSUMERS):
         super().__init__(url, N_PRODUCERS, N_CONSUMERS)
```

### Comparing `async-http-requests-0.0.1/src/RequestObject.py` & `async-http-requests-0.0.2/src/RequestObject.py`

 * *Files identical despite different names*

### Comparing `async-http-requests-0.0.1/src/async_http_requests.egg-info/PKG-INFO` & `async-http-requests-0.0.2/src/async_http_requests.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-http-requests
-Version: 0.0.1
+Version: 0.0.2
 Summary: Asynchronous HTTP requests
 Author-email: Andrea Sergi <andrea.serg1@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 sclash - Andrea Sergi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,15 +28,14 @@
 Project-URL: Homepage, https://github.com/sclash/AsyncRequests
 Keywords: http,requests,api,asyncio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
 
 # Async Requests
 
 Python library to handle asynchronous http requests, built on top of the [requests](https://requests.readthedocs.io/en/latest/) library
```

### Comparing `async-http-requests-0.0.1/test/test.py` & `async-http-requests-0.0.2/test/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,45 +4,61 @@
 
 api = 'https://api.publicapis.org/entries'
 headers = {'user-agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36'}
 
 
 endpoints = [RequestObject(url = api, params = {"title":"cat"}),
              RequestObject(url = api, params = {"title":"dog"}),
+             RequestObject(url = 'https://fuckweb.com/', params = {"title":"fica"}),
              RequestObject(url = api, params = {"title":"house"}),
              RequestObject(url = api, params = {"title":"weath"}),
+             RequestObject(url = 'https://fuckweb.com/', params = {"title":"cazzo"}),
              RequestObject(url = api, params = {"title":"py"})]
+             
 
 a = AsyncHTTP(
     url = endpoints,
     N_PRODUCERS=5,
     N_CONSUMERS=5
 )
 len(a.url_chunk)
 def get_json(r):
     return r.json()
 
 start = perf_counter()
 a.async_request(
     request_type= RequestType.GET,
     callback=get_json,
-    headers = headers
+    headers = headers, 
+    timeout = 5
 )
 # print(a.response)
 end = perf_counter()
 print(f"Async EXECUTION TIME: {end-start}")
 
-
+len(a.response)
+len(a.error_data)
 
 import requests
 
 start = perf_counter()
 
 res = []
 for e in endpoints:
     res.append(requests.get(e.url,params = e.params, headers = headers).json()) 
 
 end = perf_counter()
 print(f"Sync EXECUTION TIME: {end-start}")
 
 len(a.response)
 
+
+
+requests.get(url = api , params = {"tile":"cazzo"})
+
+
+
+# import pandas as pd
+# from dataclasses import asdict
+err = a.error_response
+# df = pd.DataFrame()
+# asdict(err[0][0])
```

