# Comparing `tmp/broadcast_service-1.3.0.tar.gz` & `tmp/broadcast_service-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\broadcast_service-1.3.0.tar", last modified: Tue Mar 21 05:28:07 2023, max compression
+gzip compressed data, was "broadcast_service-1.3.1.tar", last modified: Thu Jun  1 08:09:15 2023, max compression
```

## Comparing `broadcast_service-1.3.0.tar` & `broadcast_service-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 05:28:07.000000 broadcast_service-1.3.0/
--rw-rw-rw-   0        0        0    11558 2022-11-21 04:35:58.000000 broadcast_service-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     4579 2023-03-21 05:28:07.000000 broadcast_service-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3712 2023-01-13 14:24:57.000000 broadcast_service-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-21 05:28:07.000000 broadcast_service-1.3.0/broadcast_service/
--rw-rw-rw-   0        0        0      666 2022-11-21 05:32:10.000000 broadcast_service-1.3.0/broadcast_service/__init__.py
--rw-rw-rw-   0        0        0     7604 2023-03-21 05:23:04.000000 broadcast_service-1.3.0/broadcast_service/_core.py
-drwxrwxrwx   0        0        0        0 2023-03-21 05:28:07.000000 broadcast_service-1.3.0/broadcast_service.egg-info/
--rw-rw-rw-   0        0        0     4579 2023-03-21 05:28:07.000000 broadcast_service-1.3.0/broadcast_service.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-03-21 05:28:07.000000 broadcast_service-1.3.0/broadcast_service.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 05:28:07.000000 broadcast_service-1.3.0/broadcast_service.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-03-21 05:28:07.000000 broadcast_service-1.3.0/broadcast_service.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-21 05:28:07.000000 broadcast_service-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1800 2023-03-21 05:18:14.000000 broadcast_service-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-21 05:28:07.000000 broadcast_service-1.3.0/tests/
--rw-rw-rw-   0        0        0      642 2022-11-21 05:32:10.000000 broadcast_service-1.3.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1468 2023-01-11 16:52:30.000000 broadcast_service-1.3.0/tests/test_async.py
--rw-rw-rw-   0        0        0     8106 2023-03-21 05:13:46.000000 broadcast_service-1.3.0/tests/test_base.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:09:15.362672 broadcast_service-1.3.1/
+-rw-rw-rw-   0        0        0    11558 2022-11-21 04:35:58.000000 broadcast_service-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     4579 2023-06-01 08:09:15.361670 broadcast_service-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3712 2023-06-01 08:01:29.000000 broadcast_service-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 08:09:15.343673 broadcast_service-1.3.1/broadcast_service/
+-rw-rw-rw-   0        0        0      666 2022-11-21 05:32:10.000000 broadcast_service-1.3.1/broadcast_service/__init__.py
+-rw-rw-rw-   0        0        0     7676 2023-06-01 08:03:10.000000 broadcast_service-1.3.1/broadcast_service/_core.py
+-rw-rw-rw-   0        0        0      656 2023-05-13 17:09:36.000000 broadcast_service-1.3.1/broadcast_service/singleton.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:09:15.352664 broadcast_service-1.3.1/broadcast_service.egg-info/
+-rw-rw-rw-   0        0        0     4579 2023-06-01 08:09:14.000000 broadcast_service-1.3.1/broadcast_service.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-06-01 08:09:15.000000 broadcast_service-1.3.1/broadcast_service.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 08:09:14.000000 broadcast_service-1.3.1/broadcast_service.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-01 08:09:14.000000 broadcast_service-1.3.1/broadcast_service.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 08:09:15.362672 broadcast_service-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1800 2023-06-01 08:08:00.000000 broadcast_service-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:09:15.358663 broadcast_service-1.3.1/tests/
+-rw-rw-rw-   0        0        0      642 2022-11-21 05:32:10.000000 broadcast_service-1.3.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     1468 2023-01-11 16:52:30.000000 broadcast_service-1.3.1/tests/test_async.py
+-rw-rw-rw-   0        0        0     8106 2023-06-01 08:01:29.000000 broadcast_service-1.3.1/tests/test_base.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `broadcast_service-1.3.0/LICENSE` & `broadcast_service-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `broadcast_service-1.3.0/PKG-INFO` & `broadcast_service-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broadcast_service
-Version: 1.3.0
+Version: 1.3.1
 Summary: A lightweight third-party broadcast/pubsub library
 Home-page: https://github.com/Undertone0809/broadcast-service
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: broadcast,broadcast-service
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `broadcast_service-1.3.0/README.md` & `broadcast_service-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `broadcast_service-1.3.0/broadcast_service/__init__.py` & `broadcast_service-1.3.1/broadcast_service/__init__.py`

 * *Files identical despite different names*

### Comparing `broadcast_service-1.3.0/broadcast_service/_core.py` & `broadcast_service-1.3.1/broadcast_service/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from typing import Optional, List, Callable
 from concurrent.futures import ThreadPoolExecutor
+from broadcast_service.singleton import Singleton
 
 __all__ = ['broadcast_service', 'BroadcastService', 'enable_log']
 
 
 def enable_log():
     logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 
 
-class BroadcastService:
+class BroadcastService(metaclass=Singleton):
     """
     This class implements broadcast mode, you can import the instance by single class.
     By BroadcastService, you can send topic message,it will automatically execute the
     callback function if some classes subscribe the topic.
 
     example:
     ---------------------------------------------------------------------------------
```

### Comparing `broadcast_service-1.3.0/broadcast_service.egg-info/PKG-INFO` & `broadcast_service-1.3.1/broadcast_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broadcast-service
-Version: 1.3.0
+Version: 1.3.1
 Summary: A lightweight third-party broadcast/pubsub library
 Home-page: https://github.com/Undertone0809/broadcast-service
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: broadcast,broadcast-service
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `broadcast_service-1.3.0/setup.py` & `broadcast_service-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="broadcast_service",
-    version="1.3.0",
+    version="1.3.1",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
     description="A lightweight third-party broadcast/pubsub library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Undertone0809/broadcast-service",
     packages=setuptools.find_packages(),
```

### Comparing `broadcast_service-1.3.0/tests/__init__.py` & `broadcast_service-1.3.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `broadcast_service-1.3.0/tests/test_async.py` & `broadcast_service-1.3.1/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `broadcast_service-1.3.0/tests/test_base.py` & `broadcast_service-1.3.1/tests/test_base.py`

 * *Files identical despite different names*

