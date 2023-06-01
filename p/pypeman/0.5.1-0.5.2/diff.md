# Comparing `tmp/pypeman-0.5.1.tar.gz` & `tmp/pypeman-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypeman-0.5.1.tar", last modified: Fri Apr 14 14:08:17 2023, max compression
+gzip compressed data, was "pypeman-0.5.2.tar", last modified: Thu Jun  1 14:28:20 2023, max compression
```

## Comparing `pypeman-0.5.1.tar` & `pypeman-0.5.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-14 14:08:17.465996 pypeman-0.5.1/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11358 2023-04-14 13:27:05.000000 pypeman-0.5.1/LICENSE
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       41 2023-04-14 13:27:05.000000 pypeman-0.5.1/MANIFEST.in
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3077 2023-04-14 14:08:17.465996 pypeman-0.5.1/PKG-INFO
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1928 2023-04-14 13:27:05.000000 pypeman-0.5.1/README.rst
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-14 14:08:17.461996 pypeman-0.5.1/pypeman/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       68 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    34065 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/channels.py
--rwxrwxr-x   0 quentin   (1000) quentin   (1000)    12351 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/commands.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2443 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/conf.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-14 14:08:17.465996 pypeman-0.5.1/pypeman/contrib/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3606 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/csv.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2178 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/ctx.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8624 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/ftp.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6612 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/hl7.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10057 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/http.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      803 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/time.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      971 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/contrib/xml.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2126 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/debug.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1451 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/default_settings.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3437 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/endpoints.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      189 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/errors.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1395 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/events.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2577 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/graph.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-14 14:08:17.465996 pypeman-0.5.1/pypeman/helpers/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      421 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/aio_compat.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3247 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/cli.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      235 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/itertools.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1894 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/lazyload.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      663 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/logging.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3005 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/reloader.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1216 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/sleeper.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      315 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/helpers/tempfile.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1335 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/map_item.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6369 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/message.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    16408 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/msgstore.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    27977 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/nodes.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3713 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/persistence.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3946 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/pjt_templates.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3008 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/plugin_mgr.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    19018 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/remoteadmin.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3790 2023-04-14 13:27:05.000000 pypeman-0.5.1/pypeman/test.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-14 14:08:17.465996 pypeman-0.5.1/pypeman.egg-info/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3077 2023-04-14 14:08:17.000000 pypeman-0.5.1/pypeman.egg-info/PKG-INFO
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1056 2023-04-14 14:08:17.000000 pypeman-0.5.1/pypeman.egg-info/SOURCES.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        1 2023-04-14 14:08:17.000000 pypeman-0.5.1/pypeman.egg-info/dependency_links.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       49 2023-04-14 14:08:17.000000 pypeman-0.5.1/pypeman.egg-info/entry_points.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      175 2023-04-14 14:08:17.000000 pypeman-0.5.1/pypeman.egg-info/requires.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        8 2023-04-14 14:08:17.000000 pypeman-0.5.1/pypeman.egg-info/top_level.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      279 2023-04-14 14:08:17.465996 pypeman-0.5.1/setup.cfg
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2216 2023-04-14 13:27:05.000000 pypeman-0.5.1/setup.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-01 14:28:20.554592 pypeman-0.5.2/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    11358 2023-06-01 14:13:10.000000 pypeman-0.5.2/LICENSE
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       41 2023-06-01 14:13:10.000000 pypeman-0.5.2/MANIFEST.in
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3077 2023-06-01 14:28:20.554592 pypeman-0.5.2/PKG-INFO
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1928 2023-06-01 14:13:10.000000 pypeman-0.5.2/README.rst
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-01 14:28:20.554592 pypeman-0.5.2/pypeman/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       68 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    34065 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/channels.py
+-rwxrwxr-x   0 quentin   (1000) quentin   (1000)    12351 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/commands.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2443 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/conf.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-01 14:28:20.554592 pypeman-0.5.2/pypeman/contrib/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3606 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/csv.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2178 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/ctx.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8624 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/ftp.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6612 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/hl7.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10070 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/http.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      803 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/time.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      971 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/xml.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2126 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/debug.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1451 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/default_settings.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3437 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/endpoints.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      189 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/errors.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1395 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/events.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2577 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/graph.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-01 14:28:20.554592 pypeman-0.5.2/pypeman/helpers/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      421 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/aio_compat.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3247 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/cli.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      235 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/itertools.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1894 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/lazyload.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      663 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/logging.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3005 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/reloader.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1216 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/sleeper.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      315 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/tempfile.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1335 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/map_item.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6369 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/message.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    16408 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/msgstore.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    27977 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/nodes.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3713 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/persistence.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3946 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/pjt_templates.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3008 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/plugin_mgr.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    19018 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/remoteadmin.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3790 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/test.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-01 14:28:20.554592 pypeman-0.5.2/pypeman.egg-info/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3077 2023-06-01 14:28:20.000000 pypeman-0.5.2/pypeman.egg-info/PKG-INFO
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1056 2023-06-01 14:28:20.000000 pypeman-0.5.2/pypeman.egg-info/SOURCES.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        1 2023-06-01 14:28:20.000000 pypeman-0.5.2/pypeman.egg-info/dependency_links.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       49 2023-06-01 14:28:20.000000 pypeman-0.5.2/pypeman.egg-info/entry_points.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      175 2023-06-01 14:28:20.000000 pypeman-0.5.2/pypeman.egg-info/requires.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        8 2023-06-01 14:28:20.000000 pypeman-0.5.2/pypeman.egg-info/top_level.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      279 2023-06-01 14:28:20.558592 pypeman-0.5.2/setup.cfg
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2216 2023-06-01 14:13:10.000000 pypeman-0.5.2/setup.py
```

### Comparing `pypeman-0.5.1/LICENSE` & `pypeman-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/PKG-INFO` & `pypeman-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeman
-Version: 0.5.1
+Version: 0.5.2
 Summary: Minimalistic but pragmatic ESB / ETL / EAI in Python
 Home-page: https://github.com/mhcomm/pypeman
 Author: Jeremie Pardou
 Author-email: jeremie@jeremiez.net
 License: Apache Software License
 Keywords: esb etl eai pipeline data processing asyncio http ftp hl7
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pypeman-0.5.1/README.rst` & `pypeman-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/channels.py` & `pypeman-0.5.2/pypeman/channels.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/commands.py` & `pypeman-0.5.2/pypeman/commands.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/conf.py` & `pypeman-0.5.2/pypeman/conf.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/contrib/csv.py` & `pypeman-0.5.2/pypeman/contrib/csv.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/contrib/ctx.py` & `pypeman-0.5.2/pypeman/contrib/ctx.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/contrib/ftp.py` & `pypeman-0.5.2/pypeman/contrib/ftp.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/contrib/hl7.py` & `pypeman-0.5.2/pypeman/contrib/hl7.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/contrib/http.py` & `pypeman-0.5.2/pypeman/contrib/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         loop = self.channel.loop
         conn = None
         ssl_context = None
         if self.client_cert:
             if self.verify:
                 ssl_context = ssl.create_default_context()
             else:
-                ssl_context = ssl.SSLContext(ssl.PROTOCOL_SSLv23)
+                ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
             try:
                 ssl_context.load_cert_chain(self.client_cert[0], self.client_cert[1])
             except FileNotFoundError:
                 logger.error("loading certs %s failed", self.client_cert)
                 raise
             conn = aiohttp.TCPConnector(ssl=ssl_context, loop=loop)
         else:
@@ -222,15 +222,15 @@
 
         if isinstance(self.auth, tuple):
             basic_auth = aiohttp.BasicAuth(self.auth[0], self.auth[1])
         else:
             basic_auth = self.auth
 
         data = None
-        if method.lower() in ['put', 'post']:
+        if method.lower() in ['put', 'post', 'patch']:
             data = msg.payload
         async with aiohttp.ClientSession(connector=conn, cookies=cookies) as session:
             if self.send_as_json:
                 resp = await session.request(
                         method=method,
                         url=url,
                         auth=basic_auth,
```

### Comparing `pypeman-0.5.1/pypeman/contrib/time.py` & `pypeman-0.5.2/pypeman/contrib/time.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/contrib/xml.py` & `pypeman-0.5.2/pypeman/contrib/xml.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/debug.py` & `pypeman-0.5.2/pypeman/debug.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/default_settings.py` & `pypeman-0.5.2/pypeman/default_settings.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/endpoints.py` & `pypeman-0.5.2/pypeman/endpoints.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/events.py` & `pypeman-0.5.2/pypeman/events.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/graph.py` & `pypeman-0.5.2/pypeman/graph.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/helpers/cli.py` & `pypeman-0.5.2/pypeman/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/helpers/lazyload.py` & `pypeman-0.5.2/pypeman/helpers/lazyload.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/helpers/logging.py` & `pypeman-0.5.2/pypeman/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/helpers/reloader.py` & `pypeman-0.5.2/pypeman/helpers/reloader.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/helpers/sleeper.py` & `pypeman-0.5.2/pypeman/helpers/sleeper.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/map_item.py` & `pypeman-0.5.2/pypeman/map_item.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/message.py` & `pypeman-0.5.2/pypeman/message.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/msgstore.py` & `pypeman-0.5.2/pypeman/msgstore.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/nodes.py` & `pypeman-0.5.2/pypeman/nodes.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/persistence.py` & `pypeman-0.5.2/pypeman/persistence.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/pjt_templates.py` & `pypeman-0.5.2/pypeman/pjt_templates.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/plugin_mgr.py` & `pypeman-0.5.2/pypeman/plugin_mgr.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/remoteadmin.py` & `pypeman-0.5.2/pypeman/remoteadmin.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman/test.py` & `pypeman-0.5.2/pypeman/test.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/pypeman.egg-info/PKG-INFO` & `pypeman-0.5.2/pypeman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeman
-Version: 0.5.1
+Version: 0.5.2
 Summary: Minimalistic but pragmatic ESB / ETL / EAI in Python
 Home-page: https://github.com/mhcomm/pypeman
 Author: Jeremie Pardou
 Author-email: jeremie@jeremiez.net
 License: Apache Software License
 Keywords: esb etl eai pipeline data processing asyncio http ftp hl7
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pypeman-0.5.1/pypeman.egg-info/SOURCES.txt` & `pypeman-0.5.2/pypeman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.1/setup.py` & `pypeman-0.5.2/setup.py`

 * *Files identical despite different names*

