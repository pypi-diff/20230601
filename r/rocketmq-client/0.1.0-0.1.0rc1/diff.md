# Comparing `tmp/rocketmq_client-0.1.0.tar.gz` & `tmp/rocketmq_client-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketmq_client-0.1.0.tar", max compression
+gzip compressed data, was "rocketmq_client-0.1.0rc1.tar", max compression
```

## Comparing `rocketmq_client-0.1.0.tar` & `rocketmq_client-0.1.0rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1659 2023-06-01 02:40:43.733043 rocketmq_client-0.1.0/README.md
--rw-r--r--   0        0        0      545 2023-06-01 02:08:18.903581 rocketmq_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-01 01:43:22.576245 rocketmq_client-0.1.0/rocketmq_client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 02:27:10.516611 rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/__init__.py
--rw-r--r--   0        0        0     2003 2023-06-01 02:25:35.240046 rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/admin_pb2.py
--rw-r--r--   0        0        0     1036 2023-06-01 02:25:35.240182 rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/admin_pb2.pyi
--rw-r--r--   0        0        0     2714 2023-06-01 02:25:35.240296 rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/admin_pb2_grpc.py
--rw-r--r--   0        0        0    14313 2023-06-01 02:25:35.240401 rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/definition_pb2.py
--rw-r--r--   0        0        0    16814 2023-06-01 02:25:35.240521 rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/definition_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 02:25:35.240752 rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/definition_pb2_grpc.py
--rw-r--r--   0        0        0    12283 2023-06-01 02:25:35.240890 rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/service_pb2.py
--rw-r--r--   0        0        0    15588 2023-06-01 02:25:35.241087 rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/service_pb2.pyi
--rw-r--r--   0        0        0    26077 2023-06-01 02:25:35.241238 rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/service_pb2_grpc.py
--rw-r--r--   0        0        0       75 2023-06-01 02:35:59.221311 rocketmq_client-0.1.0/rocketmq_client/foo.py
--rw-r--r--   0        0        0     2259 1970-01-01 00:00:00.000000 rocketmq_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1659 2023-06-01 02:40:43.733043 rocketmq_client-0.1.0rc1/README.md
+-rw-r--r--   0        0        0      548 2023-06-01 02:50:09.941571 rocketmq_client-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-01 01:43:22.576245 rocketmq_client-0.1.0rc1/rocketmq_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 02:27:10.516611 rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/__init__.py
+-rw-r--r--   0        0        0     2003 2023-06-01 02:25:35.240046 rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/admin_pb2.py
+-rw-r--r--   0        0        0     1036 2023-06-01 02:25:35.240182 rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/admin_pb2.pyi
+-rw-r--r--   0        0        0     2714 2023-06-01 02:25:35.240296 rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/admin_pb2_grpc.py
+-rw-r--r--   0        0        0    14313 2023-06-01 02:25:35.240401 rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/definition_pb2.py
+-rw-r--r--   0        0        0    16814 2023-06-01 02:25:35.240521 rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/definition_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-01 02:25:35.240752 rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/definition_pb2_grpc.py
+-rw-r--r--   0        0        0    12283 2023-06-01 02:25:35.240890 rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/service_pb2.py
+-rw-r--r--   0        0        0    15588 2023-06-01 02:25:35.241087 rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/service_pb2.pyi
+-rw-r--r--   0        0        0    26077 2023-06-01 02:25:35.241238 rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/service_pb2_grpc.py
+-rw-r--r--   0        0        0       75 2023-06-01 02:35:59.221311 rocketmq_client-0.1.0rc1/rocketmq_client/foo.py
+-rw-r--r--   0        0        0     2262 1970-01-01 00:00:00.000000 rocketmq_client-0.1.0rc1/PKG-INFO
```

### Comparing `rocketmq_client-0.1.0/README.md` & `rocketmq_client-0.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `rocketmq_client-0.1.0/pyproject.toml` & `rocketmq_client-0.1.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rocketmq-client"
-version = "0.1.0"
+version = "0.1.0rc1"
 description = "RocketMQ Python Client"
 authors = ["Aaron Ai <yangkun.ayk@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "rocketmq_client" }]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/admin_pb2.py` & `rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/admin_pb2.pyi` & `rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/admin_pb2_grpc.py` & `rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/admin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/definition_pb2.py` & `rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/definition_pb2.py`

 * *Files identical despite different names*

### Comparing `rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/definition_pb2.pyi` & `rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/definition_pb2.pyi`

 * *Files identical despite different names*

### Comparing `rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/service_pb2.py` & `rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/service_pb2.py`

 * *Files identical despite different names*

### Comparing `rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/service_pb2.pyi` & `rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `rocketmq_client-0.1.0/rocketmq_client/apache/rocketmq/v2/service_pb2_grpc.py` & `rocketmq_client-0.1.0rc1/rocketmq_client/apache/rocketmq/v2/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rocketmq_client-0.1.0/PKG-INFO` & `rocketmq_client-0.1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketmq-client
-Version: 0.1.0
+Version: 0.1.0rc1
 Summary: RocketMQ Python Client
 Author: Aaron Ai
 Author-email: yangkun.ayk@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

