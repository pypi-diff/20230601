# Comparing `tmp/sonic-client-0.0.5.tar.gz` & `tmp/sonic-client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sonic-client-0.0.5.tar", last modified: Sat Aug  3 09:22:50 2019, max compression
+gzip compressed data, was "sonic-client-1.0.0.tar", last modified: Thu Jun  1 13:39:57 2023, max compression
```

## Comparing `sonic-client-0.0.5.tar` & `sonic-client-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 ahmed     (1000) ahmed     (1000)        0 2019-08-03 09:22:50.000000 sonic-client-0.0.5/
-drwxrwxr-x   0 ahmed     (1000) ahmed     (1000)        0 2019-08-03 09:22:50.000000 sonic-client-0.0.5/sonic_client.egg-info/
--rw-rw-r--   0 ahmed     (1000) ahmed     (1000)      196 2019-08-03 09:22:50.000000 sonic-client-0.0.5/sonic_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ahmed     (1000) ahmed     (1000)        1 2019-08-03 09:22:50.000000 sonic-client-0.0.5/sonic_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ahmed     (1000) ahmed     (1000)     2555 2019-08-03 09:22:50.000000 sonic-client-0.0.5/sonic_client.egg-info/PKG-INFO
--rw-rw-r--   0 ahmed     (1000) ahmed     (1000)        6 2019-08-03 09:22:50.000000 sonic-client-0.0.5/sonic_client.egg-info/top_level.txt
-drwxrwxr-x   0 ahmed     (1000) ahmed     (1000)        0 2019-08-03 09:22:50.000000 sonic-client-0.0.5/sonic/
--rw-rw-r--   0 ahmed     (1000) ahmed     (1000)      108 2019-04-11 10:19:58.000000 sonic-client-0.0.5/sonic/__init__.py
--rw-rw-r--   0 ahmed     (1000) ahmed     (1000)    25963 2019-08-03 09:12:49.000000 sonic-client-0.0.5/sonic/client.py
--rw-rw-r--   0 ahmed     (1000) ahmed     (1000)       38 2019-08-03 09:22:50.000000 sonic-client-0.0.5/setup.cfg
--rw-rw-r--   0 ahmed     (1000) ahmed     (1000)     2555 2019-08-03 09:22:50.000000 sonic-client-0.0.5/PKG-INFO
--rw-rw-r--   0 ahmed     (1000) ahmed     (1000)     1484 2019-04-11 10:10:07.000000 sonic-client-0.0.5/README.md
--rw-rw-r--   0 ahmed     (1000) ahmed     (1000)      927 2019-08-03 09:16:03.000000 sonic-client-0.0.5/setup.py
+drwxrwxr-x   0 xmonader  (1000) xmonader  (1000)        0 2023-06-01 13:39:57.052789 sonic-client-1.0.0/
+-rw-rw-r--   0 xmonader  (1000) xmonader  (1000)     1073 2023-06-01 13:37:21.000000 sonic-client-1.0.0/LICENSE
+-rw-rw-r--   0 xmonader  (1000) xmonader  (1000)     2094 2023-06-01 13:39:57.052789 sonic-client-1.0.0/PKG-INFO
+-rw-rw-r--   0 xmonader  (1000) xmonader  (1000)     1484 2023-06-01 13:37:21.000000 sonic-client-1.0.0/README.md
+-rw-rw-r--   0 xmonader  (1000) xmonader  (1000)       38 2023-06-01 13:39:57.052789 sonic-client-1.0.0/setup.cfg
+-rw-rw-r--   0 xmonader  (1000) xmonader  (1000)      927 2023-06-01 13:38:06.000000 sonic-client-1.0.0/setup.py
+drwxrwxr-x   0 xmonader  (1000) xmonader  (1000)        0 2023-06-01 13:39:57.052789 sonic-client-1.0.0/sonic/
+-rw-rw-r--   0 xmonader  (1000) xmonader  (1000)      108 2023-06-01 13:37:21.000000 sonic-client-1.0.0/sonic/__init__.py
+-rw-rw-r--   0 xmonader  (1000) xmonader  (1000)    26044 2023-06-01 13:37:21.000000 sonic-client-1.0.0/sonic/client.py
+drwxrwxr-x   0 xmonader  (1000) xmonader  (1000)        0 2023-06-01 13:39:57.052789 sonic-client-1.0.0/sonic_client.egg-info/
+-rw-rw-r--   0 xmonader  (1000) xmonader  (1000)     2094 2023-06-01 13:39:57.000000 sonic-client-1.0.0/sonic_client.egg-info/PKG-INFO
+-rw-rw-r--   0 xmonader  (1000) xmonader  (1000)      204 2023-06-01 13:39:57.000000 sonic-client-1.0.0/sonic_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 xmonader  (1000) xmonader  (1000)        1 2023-06-01 13:39:57.000000 sonic-client-1.0.0/sonic_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 xmonader  (1000) xmonader  (1000)        6 2023-06-01 13:39:57.000000 sonic-client-1.0.0/sonic_client.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sonic-client-0.0.5/sonic_client.egg-info/PKG-INFO` & `sonic-client-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,79 @@
 Metadata-Version: 2.1
 Name: sonic-client
-Version: 0.0.5
+Version: 1.0.0
 Summary: python client for sonic search backend
 Home-page: https://github.com/xmonader/python-sonic-client
 Author: Ahmed T. Youssef
 Author-email: xmonader@gmail.com
 License: BSD 3-Clause License
-Description: # python-sonic-client
-        
-        Python client for [sonic](https://github.com/valeriansaliou/sonic) search backend.
-        
-        ## Install
-        
-        ```
-        pip install sonic-client
-        ```
-        
-        ## Examples
-        
-        ### Ingest 
-        
-        ```python
-        from sonic import IngestClient
-        
-        with IngestClient("127.0.0.1", 1491, "password") as ingestcl:
-            print(ingestcl.ping())
-            print(ingestcl.protocol)
-            print(ingestcl.bufsize)
-            ingestcl.push("wiki", "articles", "article-1", "for the love of god hell")
-            ingestcl.push("wiki", "articles", "article-2", "for the love of satan heaven")
-            ingestcl.push("wiki", "articles", "article-3", "for the love of lorde hello")
-            ingestcl.push("wiki", "articles", "article-4", "for the god of loaf helmet")
-        ```
-        
-        
-        ### Search
-        
-        ```python
-        from sonic import SearchClient
-        
-        with SearchClient("127.0.0.1", 1491, "password") as querycl:
-            print(querycl.ping())
-            print(querycl.query("wiki", "articles", "for"))
-            print(querycl.query("wiki", "articles", "love"))
-            print(querycl.suggest("wiki", "articles", "hell"))
-        ```
-        
-        
-        ### Control
-        
-        ```python
-        from sonic import ControlClient
-        
-        with ControlClient("127.0.0.1", 1491, "password") as controlcl:
-            print(controlcl.ping())
-            controlcl.trigger("consolidate")
-        ```
-        
-        ## API reference
-        
-        API documentation can be found at [docs/api](./docs/api) and also [Browsable](https://xmonader.github.io/python-sonic-client/api/sonic/)
-        
-        
-        ## Difference from asonic
-        
-        asonic uses asyncio and this client doesn't. It grew out of needing to use sonic within gevent context  
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# python-sonic-client
+
+Python client for [sonic](https://github.com/valeriansaliou/sonic) search backend.
+
+## Install
+
+```
+pip install sonic-client
+```
+
+## Examples
+
+### Ingest 
+
+```python
+from sonic import IngestClient
+
+with IngestClient("127.0.0.1", 1491, "password") as ingestcl:
+    print(ingestcl.ping())
+    print(ingestcl.protocol)
+    print(ingestcl.bufsize)
+    ingestcl.push("wiki", "articles", "article-1", "for the love of god hell")
+    ingestcl.push("wiki", "articles", "article-2", "for the love of satan heaven")
+    ingestcl.push("wiki", "articles", "article-3", "for the love of lorde hello")
+    ingestcl.push("wiki", "articles", "article-4", "for the god of loaf helmet")
+```
+
+
+### Search
+
+```python
+from sonic import SearchClient
+
+with SearchClient("127.0.0.1", 1491, "password") as querycl:
+    print(querycl.ping())
+    print(querycl.query("wiki", "articles", "for"))
+    print(querycl.query("wiki", "articles", "love"))
+    print(querycl.suggest("wiki", "articles", "hell"))
+```
+
+
+### Control
+
+```python
+from sonic import ControlClient
+
+with ControlClient("127.0.0.1", 1491, "password") as controlcl:
+    print(controlcl.ping())
+    controlcl.trigger("consolidate")
+```
+
+## API reference
+
+API documentation can be found at [docs/api](./docs/api) and also [Browsable](https://xmonader.github.io/python-sonic-client/api/sonic/)
+
+
+## Difference from asonic
+
+asonic uses asyncio and this client doesn't. It grew out of needing to use sonic within gevent context  
+
+
```

### Comparing `sonic-client-0.0.5/sonic/client.py` & `sonic-client-1.0.0/sonic/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,16 @@
         resp = self._execute_command("START", self.channel, self._password)
         self.protocol = _parse_protocol_version(resp)
         self.bufsize = _parse_buffer_size(resp)
 
         return self.ping()
 
     def ping(self):
-        return self._execute_command("PING") == "PONG"
+        res = self._execute_command("PING")
+        return res == "PONG" if self.raw else res
 
     def __create_connection(self, address):
         "Create a TCP socket connection"
         # we want to mimic what socket.create_connection does to support
         # ipv4/ipv6, but we want to set options prior to calling
         # socket.connect()
         # snippet taken from redis client code.
@@ -272,21 +273,21 @@
             self.__socket = self.__create_connection(self.address)
 
         return self.__socket
 
     @property
     def _reader(self):
         if not self.__reader:
-            self.__reader = self._socket.makefile('r')
+            self.__reader = self._socket.makefile('r', encoding='utf-8')
         return self.__reader
 
     @property
     def _writer(self):
         if not self.__writer:
-            self.__writer = self._socket.makefile('w')
+            self.__writer = self._socket.makefile('w', encoding='utf-8')
         return self.__writer
 
     def close(self):
         """
         Closes the connection and its resources.
         """
         resources = (self.__reader, self.__writer, self.__socket)
@@ -673,15 +674,15 @@
             limit {int} -- a positive integer number; set within allowed maximum & minimum limits (default: {None})
 
         Returns:
             list -- list of suggested words.
         """
         limit = "LIMIT({})".format(limit) if limit else ''
         word = quote_text(word)
-        return self._execute_command(
+        return self._execute_command_async(
             'SUGGEST', collection, bucket, word, limit)
 
 
 class ControlClient(SonicClient, CommonCommandsMixin):
     def __init__(self, host: str, port: int, password: str):
         """Create Sonic client that operates on the Control Channel
```

### Comparing `sonic-client-0.0.5/PKG-INFO` & `sonic-client-1.0.0/sonic_client.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,79 @@
 Metadata-Version: 2.1
 Name: sonic-client
-Version: 0.0.5
+Version: 1.0.0
 Summary: python client for sonic search backend
 Home-page: https://github.com/xmonader/python-sonic-client
 Author: Ahmed T. Youssef
 Author-email: xmonader@gmail.com
 License: BSD 3-Clause License
-Description: # python-sonic-client
-        
-        Python client for [sonic](https://github.com/valeriansaliou/sonic) search backend.
-        
-        ## Install
-        
-        ```
-        pip install sonic-client
-        ```
-        
-        ## Examples
-        
-        ### Ingest 
-        
-        ```python
-        from sonic import IngestClient
-        
-        with IngestClient("127.0.0.1", 1491, "password") as ingestcl:
-            print(ingestcl.ping())
-            print(ingestcl.protocol)
-            print(ingestcl.bufsize)
-            ingestcl.push("wiki", "articles", "article-1", "for the love of god hell")
-            ingestcl.push("wiki", "articles", "article-2", "for the love of satan heaven")
-            ingestcl.push("wiki", "articles", "article-3", "for the love of lorde hello")
-            ingestcl.push("wiki", "articles", "article-4", "for the god of loaf helmet")
-        ```
-        
-        
-        ### Search
-        
-        ```python
-        from sonic import SearchClient
-        
-        with SearchClient("127.0.0.1", 1491, "password") as querycl:
-            print(querycl.ping())
-            print(querycl.query("wiki", "articles", "for"))
-            print(querycl.query("wiki", "articles", "love"))
-            print(querycl.suggest("wiki", "articles", "hell"))
-        ```
-        
-        
-        ### Control
-        
-        ```python
-        from sonic import ControlClient
-        
-        with ControlClient("127.0.0.1", 1491, "password") as controlcl:
-            print(controlcl.ping())
-            controlcl.trigger("consolidate")
-        ```
-        
-        ## API reference
-        
-        API documentation can be found at [docs/api](./docs/api) and also [Browsable](https://xmonader.github.io/python-sonic-client/api/sonic/)
-        
-        
-        ## Difference from asonic
-        
-        asonic uses asyncio and this client doesn't. It grew out of needing to use sonic within gevent context  
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# python-sonic-client
+
+Python client for [sonic](https://github.com/valeriansaliou/sonic) search backend.
+
+## Install
+
+```
+pip install sonic-client
+```
+
+## Examples
+
+### Ingest 
+
+```python
+from sonic import IngestClient
+
+with IngestClient("127.0.0.1", 1491, "password") as ingestcl:
+    print(ingestcl.ping())
+    print(ingestcl.protocol)
+    print(ingestcl.bufsize)
+    ingestcl.push("wiki", "articles", "article-1", "for the love of god hell")
+    ingestcl.push("wiki", "articles", "article-2", "for the love of satan heaven")
+    ingestcl.push("wiki", "articles", "article-3", "for the love of lorde hello")
+    ingestcl.push("wiki", "articles", "article-4", "for the god of loaf helmet")
+```
+
+
+### Search
+
+```python
+from sonic import SearchClient
+
+with SearchClient("127.0.0.1", 1491, "password") as querycl:
+    print(querycl.ping())
+    print(querycl.query("wiki", "articles", "for"))
+    print(querycl.query("wiki", "articles", "love"))
+    print(querycl.suggest("wiki", "articles", "hell"))
+```
+
+
+### Control
+
+```python
+from sonic import ControlClient
+
+with ControlClient("127.0.0.1", 1491, "password") as controlcl:
+    print(controlcl.ping())
+    controlcl.trigger("consolidate")
+```
+
+## API reference
+
+API documentation can be found at [docs/api](./docs/api) and also [Browsable](https://xmonader.github.io/python-sonic-client/api/sonic/)
+
+
+## Difference from asonic
+
+asonic uses asyncio and this client doesn't. It grew out of needing to use sonic within gevent context  
+
+
```

### Comparing `sonic-client-0.0.5/README.md` & `sonic-client-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sonic-client-0.0.5/setup.py` & `sonic-client-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     # can't have the entry_points option here.
     from distutils.core import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='sonic-client',
-      version='0.0.5',
+      version='1.0.0',
       author="Ahmed T. Youssef",
       author_email="xmonader@gmail.com",
       description='python client for sonic search backend',
       long_description=long_description,
       long_description_content_type="text/markdown",
       packages=['sonic'],
       url="https://github.com/xmonader/python-sonic-client",
```

