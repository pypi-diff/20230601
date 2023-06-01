# Comparing `tmp/memphis-py-beta-1.0.4.tar.gz` & `tmp/memphis-py-beta-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/memphis-py-beta-1.0.4.tar", last modified: Wed May 31 07:43:56 2023, max compression
+gzip compressed data, was "dist/memphis-py-beta-1.0.5.tar", last modified: Thu Jun  1 07:02:56 2023, max compression
```

## Comparing `memphis-py-beta-1.0.4.tar` & `memphis-py-beta-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-31 07:43:56.000000 memphis-py-beta-1.0.4/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16488 2023-05-31 07:43:56.000000 memphis-py-beta-1.0.4/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12575 2023-05-31 07:43:55.000000 memphis-py-beta-1.0.4/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-31 07:43:56.000000 memphis-py-beta-1.0.4/memphis/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-05-31 07:43:55.000000 memphis-py-beta-1.0.4/memphis/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8079 2023-05-31 07:43:55.000000 memphis-py-beta-1.0.4/memphis/consumer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-05-31 07:43:55.000000 memphis-py-beta-1.0.4/memphis/exceptions.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-05-31 07:43:55.000000 memphis-py-beta-1.0.4/memphis/headers.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    32276 2023-05-31 07:43:55.000000 memphis-py-beta-1.0.4/memphis/memphis.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2174 2023-05-31 07:43:55.000000 memphis-py-beta-1.0.4/memphis/message.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    14111 2023-05-31 07:43:55.000000 memphis-py-beta-1.0.4/memphis/producer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2192 2023-05-31 07:43:55.000000 memphis-py-beta-1.0.4/memphis/station.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-05-31 07:43:55.000000 memphis-py-beta-1.0.4/memphis/types.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-05-31 07:43:55.000000 memphis-py-beta-1.0.4/memphis/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-31 07:43:56.000000 memphis-py-beta-1.0.4/memphis_py_beta.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16488 2023-05-31 07:43:56.000000 memphis-py-beta-1.0.4/memphis_py_beta.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      429 2023-05-31 07:43:56.000000 memphis-py-beta-1.0.4/memphis_py_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-31 07:43:56.000000 memphis-py-beta-1.0.4/memphis_py_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-05-31 07:43:56.000000 memphis-py-beta-1.0.4/memphis_py_beta.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-05-31 07:43:56.000000 memphis-py-beta-1.0.4/memphis_py_beta.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-05-31 07:43:55.000000 memphis-py-beta-1.0.4/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-05-31 07:43:56.000000 memphis-py-beta-1.0.4/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1331 2023-05-31 07:43:55.000000 memphis-py-beta-1.0.4/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 07:02:56.000000 memphis-py-beta-1.0.5/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16488 2023-06-01 07:02:56.000000 memphis-py-beta-1.0.5/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12575 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 07:02:56.000000 memphis-py-beta-1.0.5/memphis/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8079 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/consumer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/exceptions.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/headers.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    32675 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/memphis.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2174 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/message.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    14111 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/producer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2192 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/station.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/types.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 07:02:56.000000 memphis-py-beta-1.0.5/memphis_py_beta.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16488 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis_py_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      429 2023-06-01 07:02:56.000000 memphis-py-beta-1.0.5/memphis_py_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis_py_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis_py_beta.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis_py_beta.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-06-01 07:02:56.000000 memphis-py-beta-1.0.5/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1331 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/setup.py
```

### Comparing `memphis-py-beta-1.0.4/PKG-INFO` & `memphis-py-beta-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memphis-py-beta
-Version: 1.0.4
+Version: 1.0.5
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.4.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.5.tar.gz
 Description: <div align="center">
           
           ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
```

### Comparing `memphis-py-beta-1.0.4/README.md` & `memphis-py-beta-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.4/memphis/__init__.py` & `memphis-py-beta-1.0.5/memphis/__init__.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.4/memphis/consumer.py` & `memphis-py-beta-1.0.5/memphis/consumer.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.4/memphis/exceptions.py` & `memphis-py-beta-1.0.5/memphis/exceptions.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.4/memphis/headers.py` & `memphis-py-beta-1.0.5/memphis/headers.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.4/memphis/memphis.py` & `memphis-py-beta-1.0.5/memphis/memphis.py`

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

### Comparing `memphis-py-beta-1.0.4/memphis/message.py` & `memphis-py-beta-1.0.5/memphis/message.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.4/memphis/producer.py` & `memphis-py-beta-1.0.5/memphis/producer.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.4/memphis/station.py` & `memphis-py-beta-1.0.5/memphis/station.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.4/memphis/types.py` & `memphis-py-beta-1.0.5/memphis/types.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.4/memphis/utils.py` & `memphis-py-beta-1.0.5/memphis/utils.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.4/memphis_py_beta.egg-info/PKG-INFO` & `memphis-py-beta-1.0.5/memphis_py_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memphis-py-beta
-Version: 1.0.4
+Version: 1.0.5
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.4.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.5.tar.gz
 Description: <div align="center">
           
           ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
```

### Comparing `memphis-py-beta-1.0.4/setup.py` & `memphis-py-beta-1.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="memphis-py-beta",
     packages=["memphis"],
-    version="1.0.4",
+    version="1.0.5",
     license="Apache-2.0",
     description="A powerful messaging platform for modern developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author="Memphis.dev",
     author_email="team@memphis.dev",
     url="https://github.com/memphisdev/memphis.py",
-    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.4.tar.gz",
+    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.5.tar.gz",
     keywords=["message broker", "devtool", "streaming", "data"],
     install_requires=["asyncio", "nats-py", "protobuf", "jsonschema", "graphql-core"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
         "License :: OSI Approved :: GNU General Public License (GPL)",
```

