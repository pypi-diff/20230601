# Comparing `tmp/arizon-usb-apiserver-0.4.6.tar.gz` & `tmp/arizon-usb-apiserver-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/arizon-usb-apiserver/arizon-usb-apiserver/dist/.tmp-ju0wfhsz/arizon-usb-apiserver-0.4.6.tar", last modified: Tue Mar  7 03:15:46 2023, max compression
+gzip compressed data, was "/home/runner/work/arizon-usb-apiserver/arizon-usb-apiserver/dist/.tmp-a1sorvv1/arizon-usb-apiserver-0.4.7.tar", last modified: Thu Jun  1 06:42:05 2023, max compression
```

## Comparing `arizon-usb-apiserver-0.4.6.tar` & `arizon-usb-apiserver-0.4.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/Parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/Sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/apiserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/apiserver/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/apiserver/grpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/apiserver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/apiserver/restful_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/apiserver/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/client/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/client/grpc/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/client/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/client/restful/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/client/restful/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/client/restful/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/client/restful/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/cmd/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/cmd/test_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/cmd/test_restful.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/grpc/force_packet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/grpc/force_packet_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/arizon_usb_apiserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:15:46.000000 arizon-usb-apiserver-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/tests/test_client_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/tests/test_client_restful.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/tests/test_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-07 03:15:33.000000 arizon-usb-apiserver-0.4.6/tests/test_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/Parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/Sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/apiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/apiserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/apiserver/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/apiserver/grpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/apiserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/apiserver/restful_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/apiserver/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/client/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/client/grpc/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/client/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/client/restful/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/client/restful/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/client/restful/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/client/restful/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/cmd/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/cmd/test_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/cmd/test_restful.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/grpc/force_packet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/grpc/force_packet_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/arizon_usb_apiserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:42:05.000000 arizon-usb-apiserver-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/tests/test_client_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/tests/test_client_restful.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/tests/test_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-01 06:41:50.000000 arizon-usb-apiserver-0.4.7/tests/test_sensor.py
```

### Comparing `arizon-usb-apiserver-0.4.6/PKG-INFO` & `arizon-usb-apiserver-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arizon-usb-apiserver
-Version: 0.4.6
+Version: 0.4.7
 Summary: Driver for Arizona USB Pressure Sensor
 Author: davidliyutong
 Author-email: davidliyutong@sjtu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # ARIZON USB APIServer
```

### Comparing `arizon-usb-apiserver-0.4.6/README.md` & `arizon-usb-apiserver-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/Config.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/Config.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/Parser.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/Parser.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/Sensor.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/Sensor.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/__main__.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/__main__.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/apiserver/app.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/apiserver/app.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/apiserver/grpc_server.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/apiserver/grpc_server.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/apiserver/main.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/apiserver/main.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/apiserver/restful_server.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/apiserver/restful_server.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/apiserver/server.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/apiserver/server.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/client/grpc/Client.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/client/grpc/Client.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/client/restful/client.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/client/restful/client.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/client/restful/types.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/client/restful/types.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/cmd/configure.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/cmd/configure.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,42 +4,44 @@
 
 
 def main(args):
     while True:
         api_port = must_parse_cli_int("Enter a port number", 1024, 65535, 8080)
         api_interface = must_parse_cli_string("Enter a interface", "0.0.0.0")
         serial_port = must_parse_cli_string("Enter a serial port")
+        addr = must_parse_cli_string("Enter a serial address", default="0")
         serial_baudrate = must_parse_cli_int("Enter a serial baudrate", 0, 921600, 115200)
         debug = must_parse_cli_bool("Debug mode", False)
 
         res = {
             "arizon_usb_apiserver": {
                 "api": {
                     "port": api_port,
                     "interface": api_interface
                 },
-                "serial": [
+                "serials": [
                     {
                         "port": serial_port,
                         "baudrate": serial_baudrate,
-                        "addr": serial_port
+                        "addr": addr
                     },
                 ],
                 "debug": debug
             }
         }
         print("Your configuration is:")
         pprint.pprint(res)
         confirm = must_parse_cli_bool("Confirm?", True)
         if confirm:
             break
         else:
             continue
 
-    dest = must_parse_cli_string("Enter save destination", "./arizon_config.yaml")
+    dest = must_parse_cli_string("Enter save destination", "./"
+                                                           "_config.yaml")
     with open(dest, 'w') as f:
         yaml.dump(res, f)
 
 
 def entry_point(argv):
     main(None)
```

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/cmd/test_grpc.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/cmd/test_grpc.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/cmd/test_restful.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/cmd/test_restful.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/grpc/force_packet_pb2.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/grpc/force_packet_pb2.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver/grpc/force_packet_pb2_grpc.py` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver/grpc/force_packet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver.egg-info/PKG-INFO` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arizon-usb-apiserver
-Version: 0.4.6
+Version: 0.4.7
 Summary: Driver for Arizona USB Pressure Sensor
 Author: davidliyutong
 Author-email: davidliyutong@sjtu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # ARIZON USB APIServer
```

### Comparing `arizon-usb-apiserver-0.4.6/arizon_usb_apiserver.egg-info/SOURCES.txt` & `arizon-usb-apiserver-0.4.7/arizon_usb_apiserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/setup.py` & `arizon-usb-apiserver-0.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 requires = open("requirements.txt", "r").readlines() if os.path.exists("requirements.txt") else open("./arizon_usb_apiserver.egg-info/requires.txt", "r").readlines()
 print("#-------------------    ", str(os.listdir("./")))
 setup(
     name="arizon-usb-apiserver",
-    version="0.4.6",
+    version="0.4.7",
     author="davidliyutong",
     author_email="davidliyutong@sjtu.edu.cn",
     description="Driver for Arizona USB Pressure Sensor",
     packages=[
         "arizon_usb_apiserver",
         "arizon_usb_apiserver.apiserver",
         "arizon_usb_apiserver.client",
```

### Comparing `arizon-usb-apiserver-0.4.6/tests/test_api.py` & `arizon-usb-apiserver-0.4.7/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/tests/test_client_grpc.py` & `arizon-usb-apiserver-0.4.7/tests/test_client_grpc.py`

 * *Files identical despite different names*

### Comparing `arizon-usb-apiserver-0.4.6/tests/test_client_restful.py` & `arizon-usb-apiserver-0.4.7/tests/test_client_restful.py`

 * *Files identical despite different names*

