# Comparing `tmp/netdata-1.0.3.tar.gz` & `tmp/netdata-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netdata-1.0.3.tar", max compression
+gzip compressed data, was "netdata-1.1.0.tar", max compression
```

## Comparing `netdata-1.0.3.tar` & `netdata-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1110 2021-03-17 09:59:27.484469 netdata-1.0.3/LICENSE
--rw-r--r--   0        0        0     1116 2022-01-04 08:24:16.663550 netdata-1.0.3/README.rst
--rw-r--r--   0        0        0     2890 2021-11-26 13:22:53.767820 netdata-1.0.3/netdata/__init__.py
--rw-r--r--   0        0        0      248 2020-08-15 11:47:01.963105 netdata-1.0.3/netdata/exceptions.py
--rw-r--r--   0        0        0     1123 2022-09-25 09:25:10.579996 netdata-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1865 2022-09-25 09:33:17.031303 netdata-1.0.3/setup.py
--rw-r--r--   0        0        0     2163 2022-09-25 09:33:17.031471 netdata-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1110 2023-05-31 22:55:56.813574 netdata-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1116 2022-01-04 08:24:16.663550 netdata-1.1.0/README.rst
+-rw-r--r--   0        0        0     2958 2023-05-31 22:55:56.814574 netdata-1.1.0/netdata/__init__.py
+-rw-r--r--   0        0        0      248 2020-08-15 11:47:01.963105 netdata-1.1.0/netdata/exceptions.py
+-rw-r--r--   0        0        0     1126 2023-05-31 23:12:49.817386 netdata-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 netdata-1.1.0/PKG-INFO
```

### Comparing `netdata-1.0.3/LICENSE` & `netdata-1.1.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018-2021 Fabian Affolter <fabian@affolter-engineering.ch>
+Copyright (c) 2018-2023 Fabian Affolter <fabian@affolter-engineering.ch>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `netdata-1.0.3/README.rst` & `netdata-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `netdata-1.0.3/netdata/__init__.py` & `netdata-1.1.0/netdata/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 
 API_VERSION = 1
 
 
 class Netdata(object):
     """A class for handling connections with a Netdata instance."""
 
-    def __init__(self, host, port=19999, tls=None, path=None):
+    def __init__(self, host, port=19999, tls=None, path=None, timeout=5.0):
         """Initialize the connection to the Netdata instance."""
         self.host = host
         self.port = port
         self.values = self.alarms = self.metrics = None
+        self.timeout = timeout
 
         self.scheme = "http" if tls is None or not False else "https"
 
         if path is None:
             self.base_url = URL.build(
                 scheme=self.scheme, host=host, port=port, path=f"/api/v{API_VERSION}/"
             )
@@ -38,15 +39,15 @@
                 scheme=self.scheme, host=host, port=port, path=path
             )
 
     async def get_data(self, url) -> Dict:
         """Execute a request to a data endpoint."""
         try:
             async with httpx.AsyncClient() as client:
-                response = await client.get(str(url))
+                response = await client.get(str(url), timeout = self.timeout)
         except httpx.ConnectError:
             raise exceptions.NetdataConnectionError(
                 f"Connection to {self.scheme}://{self.host}:{self.port} failed"
             )
 
         if response.status_code == httpx.codes.OK:
             _LOGGER.debug(response.json())
```

### Comparing `netdata-1.0.3/pyproject.toml` & `netdata-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netdata"
-version = "1.0.3"
+version = "1.1.0"
 description = "Python API for interacting with Netdata"
 authors = ["Fabian Affolter <mail@fabian-affolter.ch>"]
 license = "MIT"
 homepage = "https://github.com/home-assistant-ecosystem/python-netdata"
 repository = "https://github.com/home-assistant-ecosystem/python-netdata"
 readme = "README.rst"
 classifiers = [
@@ -12,27 +12,27 @@
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Topic :: Utilities",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Home Automation"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 httpx = ">=0.23,<1"
-yarl = "^1.7.0"
+yarl = "^1.8.0"
 
 [tool.poetry.dev-dependencies]
-black = "^22.8"
+black = "^23.3.0"
 pytest = "^6.2.5"
 pytest-httpx = ">0.15,<1"
 pytest-asyncio = "^0.15.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `netdata-1.0.3/PKG-INFO` & `netdata-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: netdata
-Version: 1.0.3
+Version: 1.1.0
 Summary: Python API for interacting with Netdata
 Home-page: https://github.com/home-assistant-ecosystem/python-netdata
 License: MIT
 Author: Fabian Affolter
 Author-email: mail@fabian-affolter.ch
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Utilities
 Requires-Dist: httpx (>=0.23,<1)
-Requires-Dist: yarl (>=1.7.0,<2.0.0)
+Requires-Dist: yarl (>=1.8.0,<2.0.0)
 Project-URL: Repository, https://github.com/home-assistant-ecosystem/python-netdata
 Description-Content-Type: text/x-rst
 
 python-netdata
 ==============
 
 Python API for interacting with `Netdata <https://my-netdata.io/>`_. Currently
```

