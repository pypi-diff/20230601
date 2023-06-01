# Comparing `tmp/memphis-py-1.0.2.tar.gz` & `tmp/memphis-py-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/memphis-py-1.0.2.tar", last modified: Wed May 31 09:25:17 2023, max compression
+gzip compressed data, was "dist/memphis-py-1.0.3.tar", last modified: Thu Jun  1 07:27:03 2023, max compression
```

## Comparing `memphis-py-1.0.2.tar` & `memphis-py-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-31 09:25:17.000000 memphis-py-1.0.2/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16483 2023-05-31 09:25:17.000000 memphis-py-1.0.2/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12575 2023-05-31 09:25:16.000000 memphis-py-1.0.2/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-31 09:25:17.000000 memphis-py-1.0.2/memphis/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-05-31 09:25:16.000000 memphis-py-1.0.2/memphis/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8079 2023-05-31 09:25:16.000000 memphis-py-1.0.2/memphis/consumer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-05-31 09:25:16.000000 memphis-py-1.0.2/memphis/exceptions.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-05-31 09:25:16.000000 memphis-py-1.0.2/memphis/headers.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    32276 2023-05-31 09:25:16.000000 memphis-py-1.0.2/memphis/memphis.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2174 2023-05-31 09:25:16.000000 memphis-py-1.0.2/memphis/message.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    14111 2023-05-31 09:25:16.000000 memphis-py-1.0.2/memphis/producer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2192 2023-05-31 09:25:16.000000 memphis-py-1.0.2/memphis/station.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-05-31 09:25:16.000000 memphis-py-1.0.2/memphis/types.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-05-31 09:25:16.000000 memphis-py-1.0.2/memphis/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-31 09:25:17.000000 memphis-py-1.0.2/memphis_py.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16483 2023-05-31 09:25:17.000000 memphis-py-1.0.2/memphis_py.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      404 2023-05-31 09:25:17.000000 memphis-py-1.0.2/memphis_py.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-31 09:25:17.000000 memphis-py-1.0.2/memphis_py.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-05-31 09:25:17.000000 memphis-py-1.0.2/memphis_py.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-05-31 09:25:17.000000 memphis-py-1.0.2/memphis_py.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-05-31 09:25:16.000000 memphis-py-1.0.2/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-05-31 09:25:17.000000 memphis-py-1.0.2/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1326 2023-05-31 09:25:16.000000 memphis-py-1.0.2/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 07:27:03.000000 memphis-py-1.0.3/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16483 2023-06-01 07:27:03.000000 memphis-py-1.0.3/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12575 2023-06-01 07:26:59.000000 memphis-py-1.0.3/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 07:27:03.000000 memphis-py-1.0.3/memphis/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-06-01 07:26:59.000000 memphis-py-1.0.3/memphis/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8079 2023-06-01 07:26:59.000000 memphis-py-1.0.3/memphis/consumer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-06-01 07:26:59.000000 memphis-py-1.0.3/memphis/exceptions.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-06-01 07:26:59.000000 memphis-py-1.0.3/memphis/headers.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    32675 2023-06-01 07:26:59.000000 memphis-py-1.0.3/memphis/memphis.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2174 2023-06-01 07:26:59.000000 memphis-py-1.0.3/memphis/message.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    14111 2023-06-01 07:26:59.000000 memphis-py-1.0.3/memphis/producer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2192 2023-06-01 07:26:59.000000 memphis-py-1.0.3/memphis/station.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-06-01 07:26:59.000000 memphis-py-1.0.3/memphis/types.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-06-01 07:26:59.000000 memphis-py-1.0.3/memphis/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 07:27:03.000000 memphis-py-1.0.3/memphis_py.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16483 2023-06-01 07:27:03.000000 memphis-py-1.0.3/memphis_py.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      404 2023-06-01 07:27:03.000000 memphis-py-1.0.3/memphis_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-06-01 07:27:03.000000 memphis-py-1.0.3/memphis_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-06-01 07:27:03.000000 memphis-py-1.0.3/memphis_py.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-06-01 07:27:03.000000 memphis-py-1.0.3/memphis_py.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-06-01 07:26:59.000000 memphis-py-1.0.3/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-06-01 07:27:03.000000 memphis-py-1.0.3/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1326 2023-06-01 07:27:03.000000 memphis-py-1.0.3/setup.py
```

### Comparing `memphis-py-1.0.2/PKG-INFO` & `memphis-py-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memphis-py
-Version: 1.0.2
+Version: 1.0.3
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.2.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.3.tar.gz
 Description: <div align="center">
           
           ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
```

### Comparing `memphis-py-1.0.2/README.md` & `memphis-py-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.2/memphis/__init__.py` & `memphis-py-1.0.3/memphis/__init__.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.2/memphis/consumer.py` & `memphis-py-1.0.3/memphis/consumer.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.2/memphis/exceptions.py` & `memphis-py-1.0.3/memphis/exceptions.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.2/memphis/headers.py` & `memphis-py-1.0.3/memphis/headers.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.2/memphis/memphis.py` & `memphis-py-1.0.3/memphis/memphis.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import asyncio
+import copy
 import json
 import ssl
 from typing import Iterable, Union
 import uuid
 import base64
 
 import nats as broker
@@ -84,25 +85,35 @@
             )
             self.configuration_tasks = task
         except Exception as err:
             raise MemphisError(err)
 
     async def get_broker_manager_connection(self, connection_opts):
         if "user" in connection_opts:
-            ping_connection_opts = connection_opts
+            async def ping_error_cb(e):
+                if "authorization violation" not in (str(e)).lower():
+                    print(MemphisError(str(e)))
+            
+            async def error_cb(e):
+                return
+            
+            ping_connection_opts = copy.deepcopy(connection_opts)
             ping_connection_opts["allow_reconnect"] = False
+            ping_connection_opts["error_cb"] = ping_error_cb
+
             try:
                 conn = await broker.connect(**ping_connection_opts)
                 await conn.close()
             except Exception as e:
                 if "authorization violation" in str(e).lower():
                     try:
                         if "localhost" in connection_opts['servers']: # for handling bad quality networks like port fwd
                             await asyncio.sleep(1)
                         ping_connection_opts["user"] = self.username
+                        ping_connection_opts["error_cb"] = error_cb
                         conn = await broker.connect(**ping_connection_opts)
                         await conn.close()
                         connection_opts["user"] = self.username
                     except Exception as e_1:
                         raise e_1
                 else:
                     raise e
```

### Comparing `memphis-py-1.0.2/memphis/message.py` & `memphis-py-1.0.3/memphis/message.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.2/memphis/producer.py` & `memphis-py-1.0.3/memphis/producer.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.2/memphis/station.py` & `memphis-py-1.0.3/memphis/station.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.2/memphis/types.py` & `memphis-py-1.0.3/memphis/types.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.2/memphis/utils.py` & `memphis-py-1.0.3/memphis/utils.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.2/memphis_py.egg-info/PKG-INFO` & `memphis-py-1.0.3/memphis_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memphis-py
-Version: 1.0.2
+Version: 1.0.3
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.2.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.3.tar.gz
 Description: <div align="center">
           
           ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
```

### Comparing `memphis-py-1.0.2/setup.py` & `memphis-py-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="memphis-py",
     packages=["memphis"],
-    version="1.0.2",
+    version="1.0.3",
     license="Apache-2.0",
     description="A powerful messaging platform for modern developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author="Memphis.dev",
     author_email="team@memphis.dev",
     url="https://github.com/memphisdev/memphis.py",
-    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.2.tar.gz",
+    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.3.tar.gz",
     keywords=["message broker", "devtool", "streaming", "data"],
     install_requires=["asyncio", "nats-py", "protobuf", "jsonschema", "graphql-core"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
         "License :: OSI Approved :: GNU General Public License (GPL)",
```

