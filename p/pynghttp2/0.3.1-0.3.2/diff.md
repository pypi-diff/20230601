# Comparing `tmp/pynghttp2-0.3.1.tar.gz` & `tmp/pynghttp2-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynghttp2-0.3.1.tar", last modified: Sun Jun  3 21:26:50 2018, max compression
+gzip compressed data, was "pynghttp2-0.3.2.tar", last modified: Thu Jun  1 00:53:51 2023, max compression
```

## Comparing `pynghttp2-0.3.1.tar` & `pynghttp2-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-03 21:26:50.000000 pynghttp2-0.3.1/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-03 21:26:50.000000 pynghttp2-0.3.1/pynghttp2/
--rw-r--r--   0 travis    (2000) travis    (2000)      124 2018-06-03 21:26:26.000000 pynghttp2-0.3.1/pynghttp2/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7624 2018-06-03 21:26:26.000000 pynghttp2-0.3.1/pynghttp2/bindings.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1181 2018-06-03 21:26:26.000000 pynghttp2-0.3.1/pynghttp2/http2.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7772 2018-06-03 21:26:26.000000 pynghttp2-0.3.1/pynghttp2/messages.py
--rw-r--r--   0 travis    (2000) travis    (2000)    25053 2018-06-03 21:26:26.000000 pynghttp2-0.3.1/pynghttp2/nghttp2.py
--rw-r--r--   0 travis    (2000) travis    (2000)    20983 2018-06-03 21:26:26.000000 pynghttp2-0.3.1/pynghttp2/sessions.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7096 2018-06-03 21:26:26.000000 pynghttp2-0.3.1/pynghttp2/streams.py
--rw-r--r--   0 travis    (2000) travis    (2000)    23494 2018-06-03 21:26:26.000000 pynghttp2-0.3.1/pynghttp2/typedefs.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-03 21:26:50.000000 pynghttp2-0.3.1/pynghttp2.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     4580 2018-06-03 21:26:50.000000 pynghttp2-0.3.1/pynghttp2.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      354 2018-06-03 21:26:50.000000 pynghttp2-0.3.1/pynghttp2.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-06-03 21:26:50.000000 pynghttp2-0.3.1/pynghttp2.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       48 2018-06-03 21:26:50.000000 pynghttp2-0.3.1/pynghttp2.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       10 2018-06-03 21:26:50.000000 pynghttp2-0.3.1/pynghttp2.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)     2617 2018-06-03 21:26:26.000000 pynghttp2-0.3.1/README.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     1615 2018-06-03 21:26:26.000000 pynghttp2-0.3.1/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4580 2018-06-03 21:26:50.000000 pynghttp2-0.3.1/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)       38 2018-06-03 21:26:50.000000 pynghttp2-0.3.1/setup.cfg
+drwxr-xr-x   0 kahlertl (634488036) domain^users (600260513)        0 2023-06-01 00:53:51.304367 pynghttp2-0.3.2/
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)     1069 2023-06-01 00:01:14.000000 pynghttp2-0.3.2/LICENSE.txt
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)     3621 2023-06-01 00:53:51.304367 pynghttp2-0.3.2/PKG-INFO
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)     2473 2023-06-01 00:37:59.000000 pynghttp2-0.3.2/README.rst
+drwxr-xr-x   0 kahlertl (634488036) domain^users (600260513)        0 2023-06-01 00:53:51.300367 pynghttp2-0.3.2/pynghttp2/
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)      124 2023-06-01 00:01:14.000000 pynghttp2-0.3.2/pynghttp2/__init__.py
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)     7624 2023-06-01 00:01:14.000000 pynghttp2-0.3.2/pynghttp2/bindings.py
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)     1181 2023-06-01 00:01:14.000000 pynghttp2-0.3.2/pynghttp2/http2.py
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)     7772 2023-06-01 00:01:14.000000 pynghttp2-0.3.2/pynghttp2/messages.py
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)    25053 2023-06-01 00:01:14.000000 pynghttp2-0.3.2/pynghttp2/nghttp2.py
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)    20983 2023-06-01 00:01:14.000000 pynghttp2-0.3.2/pynghttp2/sessions.py
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)     7096 2023-06-01 00:01:14.000000 pynghttp2-0.3.2/pynghttp2/streams.py
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)    23494 2023-06-01 00:01:14.000000 pynghttp2-0.3.2/pynghttp2/typedefs.py
+drwxr-xr-x   0 kahlertl (634488036) domain^users (600260513)        0 2023-06-01 00:53:51.304367 pynghttp2-0.3.2/pynghttp2.egg-info/
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)     3621 2023-06-01 00:53:51.000000 pynghttp2-0.3.2/pynghttp2.egg-info/PKG-INFO
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)      366 2023-06-01 00:53:51.000000 pynghttp2-0.3.2/pynghttp2.egg-info/SOURCES.txt
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)        1 2023-06-01 00:53:51.000000 pynghttp2-0.3.2/pynghttp2.egg-info/dependency_links.txt
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)       48 2023-06-01 00:53:51.000000 pynghttp2-0.3.2/pynghttp2.egg-info/requires.txt
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)       10 2023-06-01 00:53:51.000000 pynghttp2-0.3.2/pynghttp2.egg-info/top_level.txt
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)       38 2023-06-01 00:53:51.304367 pynghttp2-0.3.2/setup.cfg
+-rw-r--r--   0 kahlertl (634488036) domain^users (600260513)     1618 2023-06-01 00:45:50.000000 pynghttp2-0.3.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pynghttp2-0.3.1/pynghttp2/bindings.py` & `pynghttp2-0.3.2/pynghttp2/bindings.py`

 * *Files identical despite different names*

### Comparing `pynghttp2-0.3.1/pynghttp2/http2.py` & `pynghttp2-0.3.2/pynghttp2/http2.py`

 * *Files identical despite different names*

### Comparing `pynghttp2-0.3.1/pynghttp2/messages.py` & `pynghttp2-0.3.2/pynghttp2/messages.py`

 * *Files identical despite different names*

### Comparing `pynghttp2-0.3.1/pynghttp2/nghttp2.py` & `pynghttp2-0.3.2/pynghttp2/nghttp2.py`

 * *Files identical despite different names*

### Comparing `pynghttp2-0.3.1/pynghttp2/sessions.py` & `pynghttp2-0.3.2/pynghttp2/sessions.py`

 * *Files identical despite different names*

### Comparing `pynghttp2-0.3.1/pynghttp2/streams.py` & `pynghttp2-0.3.2/pynghttp2/streams.py`

 * *Files identical despite different names*

### Comparing `pynghttp2-0.3.1/pynghttp2/typedefs.py` & `pynghttp2-0.3.2/pynghttp2/typedefs.py`

 * *Files identical despite different names*

### Comparing `pynghttp2-0.3.1/pynghttp2.egg-info/PKG-INFO` & `pynghttp2-0.3.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,123 +1,18 @@
 Metadata-Version: 2.1
 Name: pynghttp2
-Version: 0.3.1
+Version: 0.3.2
 Summary: Asyncio bindings for libnghttp2 based on ctypes
-Home-page: https://github.com/f3anaro/pynghttp2
+Home-page: https://github.com/kahlertl/pynghttp2
 Author: Lucas Kahlert
 Author-email: lucas.kahlert@square-src.de
 License: MIT
-Project-URL: Source Code, https://github.com/f3anaro/pynghttp2/
+Project-URL: Source Code, https://github.com/kahlertl/pynghttp2/
 Project-URL: Documentation, https://pynghttp2.readthedocs.io/
-Project-URL: Bug Tracker, https://github.com/f3anaro/pynghttp2/issues
-Description: =========
-        pynghttp2
-        =========
-        
-        .. image:: https://badge.fury.io/py/pynghttp2.svg
-            :target: https://badge.fury.io/py/pynghttp2
-            :alt: PyPi Version
-        
-        .. image:: https://travis-ci.org/f3anaro/pynghttp2.svg?branch=master
-            :target: https://travis-ci.org/f3anaro/pynghttp2
-            :alt: Build Status
-        
-        .. image:: https://codecov.io/gh/f3anaro/pynghttp2/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/f3anaro/pynghttp2
-            :alt: Code Coverage
-        
-        .. image:: https://readthedocs.org/projects/pynghttp2/badge/?version=latest
-            :target: http://pynghttp2.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        pynghttp2 are simple asyncio Python bindings based on ctypes for the nghttp2_
-        library. The only thing you need is a ``libnghttp2`` version on your system.
-        
-        On Debian-based systems you can install nghttp2 simply via apt:
-        
-        .. code:: bash
-        
-            apt-get install libnghttp2-14
-        
-        The project was created in the context of a student work for an HTTP/2 protocol
-        gateway in the µPCN_ project - an implementation of Delay-tolerant Networking
-        (DTN) protocols.
-        
-        
-        Installation
-        ============
-        
-        .. code:: bash
-        
-            pip install pynghttp2
-        
-        
-        Examples
-        ========
-        
-        High-Level API
-        --------------
-        
-        .. code:: python
-        
-            from pynghttp2 import http2
-        
-            # GET request
-            resp = await http2.get('http://localhost:64602/ping')
-        
-            content = await resp.text()
-            assert content == 'pong'
-        
-            # POST request
-            message = b"Lorem ipsum dolorem"
-            resp = await http2.post('http://localhost:64602/echo', data=message)
-            echo = await resp.read()
-            assert echo == message
-        
-        
-        Client Session
-        --------------
-        
-        .. code:: python
-        
-            from pynghttp2 import ClientSession
-        
-            # Multiplex two requests
-            async with ClientSession(host='localhost', port=64602) as session:
-                stream1 = session.get('http://localhost:64602/stream')
-                stream2 = session.get('http://localhost:64602/stream')
-        
-                await asyncio.gather(stream1.read(), stream2.read())
-        
-        
-        Server Session
-        --------------
-        
-        .. code:: python
-        
-            import asyncio
-            from pynghttp2 import ServerSession
-        
-            async def handle_request(req):
-                """Echo the request body"""
-                msg = await req.read()
-                await req.response(200, data=msg)
-        
-            with ServerSession(host='localhost', port=8080) as session:
-                while True:
-                    # Wait for next incoming request
-                    req = await session
-        
-                    # Handle each request in its own task to be able to multiplex
-                    # multiple requests and responses
-                    asyncio.ensure_future(handle_request(req))
-        
-        
-        .. _nghttp2: https://nghttp2.org/
-        .. _µPCN: https://upcn.eu/
+Project-URL: Bug Tracker, https://github.com/kahlertl/pynghttp2/issues
 Keywords: HTTP/2 nghttp2 bindings asyncio ctypes
 Platform: POSIX/Unix
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
@@ -126,7 +21,110 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: dev
+License-File: LICENSE.txt
+
+=========
+pynghttp2
+=========
+
+.. image:: https://badge.fury.io/py/pynghttp2.svg
+    :target: https://badge.fury.io/py/pynghttp2
+    :alt: PyPi Version
+
+.. image:: https://codecov.io/gh/kahlertl/pynghttp2/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/kahlertl/pynghttp2
+    :alt: Code Coverage
+
+.. image:: https://readthedocs.org/projects/pynghttp2/badge/?version=latest
+    :target: http://pynghttp2.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+pynghttp2 are simple asyncio Python bindings based on ctypes for the nghttp2_
+library. The only thing you need is a ``libnghttp2`` version on your system.
+
+On Debian-based systems you can install nghttp2 simply via apt:
+
+.. code:: bash
+
+    apt-get install libnghttp2-14
+
+The project was created in the context of a student work for an HTTP/2 protocol
+gateway in the µPCN_ project - an implementation of Delay-tolerant Networking
+(DTN) protocols.
+
+
+Installation
+============
+
+.. code:: bash
+
+    pip install pynghttp2
+
+
+Examples
+========
+
+High-Level API
+--------------
+
+.. code:: python
+
+    from pynghttp2 import http2
+
+    # GET request
+    resp = await http2.get('http://localhost:64602/ping')
+
+    content = await resp.text()
+    assert content == 'pong'
+
+    # POST request
+    message = b"Lorem ipsum dolorem"
+    resp = await http2.post('http://localhost:64602/echo', data=message)
+    echo = await resp.read()
+    assert echo == message
+
+
+Client Session
+--------------
+
+.. code:: python
+
+    from pynghttp2 import ClientSession
+
+    # Multiplex two requests
+    async with ClientSession(host='localhost', port=64602) as session:
+        stream1 = session.get('http://localhost:64602/stream')
+        stream2 = session.get('http://localhost:64602/stream')
+
+        await asyncio.gather(stream1.read(), stream2.read())
+
+
+Server Session
+--------------
+
+.. code:: python
+
+    import asyncio
+    from pynghttp2 import ServerSession
+
+    async def handle_request(req):
+        """Echo the request body"""
+        msg = await req.read()
+        await req.response(200, data=msg)
+
+    with ServerSession(host='localhost', port=8080) as session:
+        while True:
+            # Wait for next incoming request
+            req = await session
+
+            # Handle each request in its own task to be able to multiplex
+            # multiple requests and responses
+            asyncio.ensure_future(handle_request(req))
+
+
+.. _nghttp2: https://nghttp2.org/
+.. _µPCN: https://upcn.eu/
```

### Comparing `pynghttp2-0.3.1/README.rst` & `pynghttp2-0.3.2/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,16 @@
 pynghttp2
 =========
 
 .. image:: https://badge.fury.io/py/pynghttp2.svg
     :target: https://badge.fury.io/py/pynghttp2
     :alt: PyPi Version
 
-.. image:: https://travis-ci.org/f3anaro/pynghttp2.svg?branch=master
-    :target: https://travis-ci.org/f3anaro/pynghttp2
-    :alt: Build Status
-
-.. image:: https://codecov.io/gh/f3anaro/pynghttp2/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/f3anaro/pynghttp2
+.. image:: https://codecov.io/gh/kahlertl/pynghttp2/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/kahlertl/pynghttp2
     :alt: Code Coverage
 
 .. image:: https://readthedocs.org/projects/pynghttp2/badge/?version=latest
     :target: http://pynghttp2.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 pynghttp2 are simple asyncio Python bindings based on ctypes for the nghttp2_
```

### Comparing `pynghttp2-0.3.1/setup.py` & `pynghttp2-0.3.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as fd:
         return fd.read()
 
 setup(
     name='pynghttp2',
-    version='0.3.1',
+    version='0.3.2',
     platforms=['POSIX/Unix'],
     description='Asyncio bindings for libnghttp2 based on ctypes',
     long_description=read('README.rst'),
     long_description_content_type='text/x-rst; charset=UTF-8',
     license='MIT',
     author='Lucas Kahlert',
     author_email='lucas.kahlert@square-src.de',
-    url='https://github.com/f3anaro/pynghttp2',
+    url='https://github.com/kahlertl/pynghttp2',
     keywords=' '.join(['HTTP/2', 'nghttp2', 'bindings', 'asyncio', 'ctypes']),
     packages=['pynghttp2'],
     install_requires=[],
     extras_require={
         'dev': [
             'pytest',
             'pytest-asyncio',
@@ -38,12 +38,12 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Software Development',
     ],
     project_urls={
-        'Source Code': 'https://github.com/f3anaro/pynghttp2/',
+        'Source Code': 'https://github.com/kahlertl/pynghttp2/',
         'Documentation': 'https://pynghttp2.readthedocs.io/',
-        'Bug Tracker': 'https://github.com/f3anaro/pynghttp2/issues',
+        'Bug Tracker': 'https://github.com/kahlertl/pynghttp2/issues',
     },
 )
```

### Comparing `pynghttp2-0.3.1/PKG-INFO` & `pynghttp2-0.3.2/pynghttp2.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,123 +1,18 @@
 Metadata-Version: 2.1
 Name: pynghttp2
-Version: 0.3.1
+Version: 0.3.2
 Summary: Asyncio bindings for libnghttp2 based on ctypes
-Home-page: https://github.com/f3anaro/pynghttp2
+Home-page: https://github.com/kahlertl/pynghttp2
 Author: Lucas Kahlert
 Author-email: lucas.kahlert@square-src.de
 License: MIT
-Project-URL: Source Code, https://github.com/f3anaro/pynghttp2/
+Project-URL: Source Code, https://github.com/kahlertl/pynghttp2/
 Project-URL: Documentation, https://pynghttp2.readthedocs.io/
-Project-URL: Bug Tracker, https://github.com/f3anaro/pynghttp2/issues
-Description: =========
-        pynghttp2
-        =========
-        
-        .. image:: https://badge.fury.io/py/pynghttp2.svg
-            :target: https://badge.fury.io/py/pynghttp2
-            :alt: PyPi Version
-        
-        .. image:: https://travis-ci.org/f3anaro/pynghttp2.svg?branch=master
-            :target: https://travis-ci.org/f3anaro/pynghttp2
-            :alt: Build Status
-        
-        .. image:: https://codecov.io/gh/f3anaro/pynghttp2/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/f3anaro/pynghttp2
-            :alt: Code Coverage
-        
-        .. image:: https://readthedocs.org/projects/pynghttp2/badge/?version=latest
-            :target: http://pynghttp2.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        pynghttp2 are simple asyncio Python bindings based on ctypes for the nghttp2_
-        library. The only thing you need is a ``libnghttp2`` version on your system.
-        
-        On Debian-based systems you can install nghttp2 simply via apt:
-        
-        .. code:: bash
-        
-            apt-get install libnghttp2-14
-        
-        The project was created in the context of a student work for an HTTP/2 protocol
-        gateway in the µPCN_ project - an implementation of Delay-tolerant Networking
-        (DTN) protocols.
-        
-        
-        Installation
-        ============
-        
-        .. code:: bash
-        
-            pip install pynghttp2
-        
-        
-        Examples
-        ========
-        
-        High-Level API
-        --------------
-        
-        .. code:: python
-        
-            from pynghttp2 import http2
-        
-            # GET request
-            resp = await http2.get('http://localhost:64602/ping')
-        
-            content = await resp.text()
-            assert content == 'pong'
-        
-            # POST request
-            message = b"Lorem ipsum dolorem"
-            resp = await http2.post('http://localhost:64602/echo', data=message)
-            echo = await resp.read()
-            assert echo == message
-        
-        
-        Client Session
-        --------------
-        
-        .. code:: python
-        
-            from pynghttp2 import ClientSession
-        
-            # Multiplex two requests
-            async with ClientSession(host='localhost', port=64602) as session:
-                stream1 = session.get('http://localhost:64602/stream')
-                stream2 = session.get('http://localhost:64602/stream')
-        
-                await asyncio.gather(stream1.read(), stream2.read())
-        
-        
-        Server Session
-        --------------
-        
-        .. code:: python
-        
-            import asyncio
-            from pynghttp2 import ServerSession
-        
-            async def handle_request(req):
-                """Echo the request body"""
-                msg = await req.read()
-                await req.response(200, data=msg)
-        
-            with ServerSession(host='localhost', port=8080) as session:
-                while True:
-                    # Wait for next incoming request
-                    req = await session
-        
-                    # Handle each request in its own task to be able to multiplex
-                    # multiple requests and responses
-                    asyncio.ensure_future(handle_request(req))
-        
-        
-        .. _nghttp2: https://nghttp2.org/
-        .. _µPCN: https://upcn.eu/
+Project-URL: Bug Tracker, https://github.com/kahlertl/pynghttp2/issues
 Keywords: HTTP/2 nghttp2 bindings asyncio ctypes
 Platform: POSIX/Unix
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
@@ -126,7 +21,110 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: dev
+License-File: LICENSE.txt
+
+=========
+pynghttp2
+=========
+
+.. image:: https://badge.fury.io/py/pynghttp2.svg
+    :target: https://badge.fury.io/py/pynghttp2
+    :alt: PyPi Version
+
+.. image:: https://codecov.io/gh/kahlertl/pynghttp2/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/kahlertl/pynghttp2
+    :alt: Code Coverage
+
+.. image:: https://readthedocs.org/projects/pynghttp2/badge/?version=latest
+    :target: http://pynghttp2.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+pynghttp2 are simple asyncio Python bindings based on ctypes for the nghttp2_
+library. The only thing you need is a ``libnghttp2`` version on your system.
+
+On Debian-based systems you can install nghttp2 simply via apt:
+
+.. code:: bash
+
+    apt-get install libnghttp2-14
+
+The project was created in the context of a student work for an HTTP/2 protocol
+gateway in the µPCN_ project - an implementation of Delay-tolerant Networking
+(DTN) protocols.
+
+
+Installation
+============
+
+.. code:: bash
+
+    pip install pynghttp2
+
+
+Examples
+========
+
+High-Level API
+--------------
+
+.. code:: python
+
+    from pynghttp2 import http2
+
+    # GET request
+    resp = await http2.get('http://localhost:64602/ping')
+
+    content = await resp.text()
+    assert content == 'pong'
+
+    # POST request
+    message = b"Lorem ipsum dolorem"
+    resp = await http2.post('http://localhost:64602/echo', data=message)
+    echo = await resp.read()
+    assert echo == message
+
+
+Client Session
+--------------
+
+.. code:: python
+
+    from pynghttp2 import ClientSession
+
+    # Multiplex two requests
+    async with ClientSession(host='localhost', port=64602) as session:
+        stream1 = session.get('http://localhost:64602/stream')
+        stream2 = session.get('http://localhost:64602/stream')
+
+        await asyncio.gather(stream1.read(), stream2.read())
+
+
+Server Session
+--------------
+
+.. code:: python
+
+    import asyncio
+    from pynghttp2 import ServerSession
+
+    async def handle_request(req):
+        """Echo the request body"""
+        msg = await req.read()
+        await req.response(200, data=msg)
+
+    with ServerSession(host='localhost', port=8080) as session:
+        while True:
+            # Wait for next incoming request
+            req = await session
+
+            # Handle each request in its own task to be able to multiplex
+            # multiple requests and responses
+            asyncio.ensure_future(handle_request(req))
+
+
+.. _nghttp2: https://nghttp2.org/
+.. _µPCN: https://upcn.eu/
```

