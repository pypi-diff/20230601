# Comparing `tmp/NuOCR-0.2.5.2.tar.gz` & `tmp/NuOCR-0.2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NuOCR-0.2.5.2.tar", last modified: Mon May 22 13:43:08 2023, max compression
+gzip compressed data, was "NuOCR-0.2.5.3.tar", last modified: Thu Jun  1 09:37:31 2023, max compression
```

## Comparing `NuOCR-0.2.5.2.tar` & `NuOCR-0.2.5.3.tar`

### file list

```diff
@@ -1,59 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 13:43:08.025848 NuOCR-0.2.5.2/
-drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.643066 NuOCR-0.2.5.2/NuOCR/
--rw-rw-rw-   0        0        0      300 2023-05-22 07:40:04.000000 NuOCR-0.2.5.2/NuOCR/__init__.py
--rw-rw-rw-   0        0        0     3656 2023-05-22 07:40:04.000000 NuOCR-0.2.5.2/NuOCR/admin.py
--rw-rw-rw-   0        0        0      235 2023-03-27 09:59:57.000000 NuOCR-0.2.5.2/NuOCR/channel.py
--rw-rw-rw-   0        0        0     1815 2023-05-22 07:40:04.000000 NuOCR-0.2.5.2/NuOCR/extractor.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.689137 NuOCR-0.2.5.2/NuOCR/gRPC_proto/
--rw-rw-rw-   0        0        0      346 2023-05-22 07:40:04.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.724430 NuOCR-0.2.5.2/NuOCR/gRPC_proto/extractor/
--rw-rw-rw-   0        0        0       65 2023-03-27 09:59:57.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/extractor/__init__.py
--rw-rw-rw-   0        0        0     3683 2022-12-13 12:07:32.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/extractor/extractor_pb2.py
--rw-rw-rw-   0        0        0     9046 2023-05-17 08:54:24.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.761884 NuOCR-0.2.5.2/NuOCR/gRPC_proto/io_adaptors/
--rw-rw-rw-   0        0        0       69 2023-03-27 09:59:57.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/io_adaptors/__init__.py
--rw-rw-rw-   0        0        0     6450 2023-05-22 07:40:04.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py
--rw-rw-rw-   0        0        0    25493 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.800615 NuOCR-0.2.5.2/NuOCR/gRPC_proto/monitor/
--rw-rw-rw-   0        0        0       61 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/monitor/__init__.py
--rw-rw-rw-   0        0        0     1797 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/monitor/monitor_pb2.py
--rw-rw-rw-   0        0        0     9283 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.833600 NuOCR-0.2.5.2/NuOCR/gRPC_proto/nufarm_poc/
--rw-rw-rw-   0        0        0       67 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/nufarm_poc/__init__.py
--rw-rw-rw-   0        0        0     1648 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py
--rw-rw-rw-   0        0        0     4270 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.867123 NuOCR-0.2.5.2/NuOCR/gRPC_proto/preprocessor/
--rw-rw-rw-   0        0        0       71 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/preprocessor/__init__.py
--rw-rw-rw-   0        0        0     4074 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py
--rw-rw-rw-   0        0        0    13059 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.904038 NuOCR-0.2.5.2/NuOCR/gRPC_proto/templated_flow/
--rw-rw-rw-   0        0        0       75 2023-03-27 09:59:57.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/templated_flow/__init__.py
--rw-rw-rw-   0        0        0     3375 2023-03-27 10:00:02.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py
--rw-rw-rw-   0        0        0     8097 2023-05-17 08:55:07.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.944373 NuOCR-0.2.5.2/NuOCR/gRPC_proto/text_processors/
--rw-rw-rw-   0        0        0       75 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/text_processors/__init__.py
--rw-rw-rw-   0        0        0     2413 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/text_processors/text_processor_pb2.py
--rw-rw-rw-   0        0        0     8128 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/text_processors/text_processor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:43:08.010361 NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/
--rw-rw-rw-   0        0        0      110 2023-03-27 09:59:58.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/__init__.py
--rw-rw-rw-   0        0        0     1414 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/auth_pb2.py
--rw-rw-rw-   0        0        0     2474 2023-05-17 08:55:25.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/auth_pb2_grpc.py
--rw-rw-rw-   0        0        0     4332 2023-03-27 10:00:02.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/user_pb2.py
--rw-rw-rw-   0        0        0    22705 2023-05-17 08:55:31.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/user_pb2_grpc.py
--rw-rw-rw-   0        0        0    15396 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/io_adaptor.py
--rw-rw-rw-   0        0        0     2820 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/monitor.py
--rw-rw-rw-   0        0        0     5896 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/preprocessors.py
--rw-rw-rw-   0        0        0     2779 2023-05-22 13:42:36.000000 NuOCR-0.2.5.2/NuOCR/templated_flow.py
--rw-rw-rw-   0        0        0     2053 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/text.py
--rw-rw-rw-   0        0        0     2788 2023-05-22 08:26:00.000000 NuOCR-0.2.5.2/NuOCR/user.py
--rw-rw-rw-   0        0        0      334 2023-03-27 09:59:59.000000 NuOCR-0.2.5.2/NuOCR/util.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.681228 NuOCR-0.2.5.2/NuOCR.egg-info/
--rw-rw-rw-   0        0        0      540 2023-05-22 13:43:07.000000 NuOCR-0.2.5.2/NuOCR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1563 2023-05-22 13:43:07.000000 NuOCR-0.2.5.2/NuOCR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 13:43:07.000000 NuOCR-0.2.5.2/NuOCR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-22 13:43:07.000000 NuOCR-0.2.5.2/NuOCR.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 13:43:07.000000 NuOCR-0.2.5.2/NuOCR.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      540 2023-05-22 13:43:08.020287 NuOCR-0.2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     4053 2023-03-27 09:59:59.000000 NuOCR-0.2.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 13:43:08.025848 NuOCR-0.2.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1132 2023-05-22 13:43:04.000000 NuOCR-0.2.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:37:31.664336 NuOCR-0.2.5.3/
+drwxrwxrwx   0        0        0        0 2023-06-01 09:37:30.884249 NuOCR-0.2.5.3/NuOCR/
+-rw-rw-rw-   0        0        0      342 2023-06-01 09:33:14.000000 NuOCR-0.2.5.3/NuOCR/__init__.py
+-rw-rw-rw-   0        0        0     3656 2023-05-30 10:56:13.000000 NuOCR-0.2.5.3/NuOCR/admin.py
+-rw-rw-rw-   0        0        0      235 2023-03-27 09:59:57.000000 NuOCR-0.2.5.3/NuOCR/channel.py
+-rw-rw-rw-   0        0        0     1815 2023-05-30 10:56:13.000000 NuOCR-0.2.5.3/NuOCR/extractor.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:37:31.074170 NuOCR-0.2.5.3/NuOCR/gRPC_proto/
+-rw-rw-rw-   0        0        0      393 2023-06-01 09:33:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:37:31.124482 NuOCR-0.2.5.3/NuOCR/gRPC_proto/extractor/
+-rw-rw-rw-   0        0        0       65 2023-03-27 09:59:57.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/extractor/__init__.py
+-rw-rw-rw-   0        0        0     3683 2022-12-13 12:07:32.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/extractor/extractor_pb2.py
+-rw-rw-rw-   0        0        0     9046 2023-05-17 08:54:24.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:37:31.167628 NuOCR-0.2.5.3/NuOCR/gRPC_proto/io_adaptors/
+-rw-rw-rw-   0        0        0       69 2023-03-27 09:59:57.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/io_adaptors/__init__.py
+-rw-rw-rw-   0        0        0     6450 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py
+-rw-rw-rw-   0        0        0    25493 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:37:31.213611 NuOCR-0.2.5.3/NuOCR/gRPC_proto/monitor/
+-rw-rw-rw-   0        0        0       61 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/monitor/__init__.py
+-rw-rw-rw-   0        0        0     1797 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/monitor/monitor_pb2.py
+-rw-rw-rw-   0        0        0     9283 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:37:31.271359 NuOCR-0.2.5.3/NuOCR/gRPC_proto/multiformats/
+-rw-rw-rw-   0        0        0       69 2023-06-01 09:33:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/multiformats/__init__.py
+-rw-rw-rw-   0        0        0     1843 2023-06-01 09:33:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/multiformats/multiformats_pb2.py
+-rw-rw-rw-   0        0        0     9497 2023-06-01 09:33:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/multiformats/multiformats_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:37:31.330436 NuOCR-0.2.5.3/NuOCR/gRPC_proto/nufarm_poc/
+-rw-rw-rw-   0        0        0       67 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/nufarm_poc/__init__.py
+-rw-rw-rw-   0        0        0     1648 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py
+-rw-rw-rw-   0        0        0     4270 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:37:31.390375 NuOCR-0.2.5.3/NuOCR/gRPC_proto/preprocessor/
+-rw-rw-rw-   0        0        0       71 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/preprocessor/__init__.py
+-rw-rw-rw-   0        0        0     4074 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py
+-rw-rw-rw-   0        0        0    13059 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:37:31.464149 NuOCR-0.2.5.3/NuOCR/gRPC_proto/templated_flow/
+-rw-rw-rw-   0        0        0       75 2023-03-27 09:59:57.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/templated_flow/__init__.py
+-rw-rw-rw-   0        0        0     3375 2023-03-27 10:00:02.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py
+-rw-rw-rw-   0        0        0     8097 2023-05-17 08:55:07.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:37:31.533056 NuOCR-0.2.5.3/NuOCR/gRPC_proto/text_processors/
+-rw-rw-rw-   0        0        0       75 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/text_processors/__init__.py
+-rw-rw-rw-   0        0        0     2413 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/text_processors/text_processor_pb2.py
+-rw-rw-rw-   0        0        0     8128 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/text_processors/text_processor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:37:31.626756 NuOCR-0.2.5.3/NuOCR/gRPC_proto/user/
+-rw-rw-rw-   0        0        0      110 2023-03-27 09:59:58.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/user/__init__.py
+-rw-rw-rw-   0        0        0     1414 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/user/auth_pb2.py
+-rw-rw-rw-   0        0        0     2474 2023-05-17 08:55:25.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/user/auth_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4332 2023-03-27 10:00:02.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/user/user_pb2.py
+-rw-rw-rw-   0        0        0    22705 2023-05-17 08:55:31.000000 NuOCR-0.2.5.3/NuOCR/gRPC_proto/user/user_pb2_grpc.py
+-rw-rw-rw-   0        0        0    15396 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/io_adaptor.py
+-rw-rw-rw-   0        0        0     2820 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/monitor.py
+-rw-rw-rw-   0        0        0     2461 2023-06-01 09:33:14.000000 NuOCR-0.2.5.3/NuOCR/multiformats.py
+-rw-rw-rw-   0        0        0     5896 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/preprocessors.py
+-rw-rw-rw-   0        0        0     2779 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/templated_flow.py
+-rw-rw-rw-   0        0        0     2053 2023-05-30 10:56:14.000000 NuOCR-0.2.5.3/NuOCR/text.py
+-rw-rw-rw-   0        0        0     2788 2023-05-29 08:41:20.000000 NuOCR-0.2.5.3/NuOCR/user.py
+-rw-rw-rw-   0        0        0      334 2023-03-27 09:59:59.000000 NuOCR-0.2.5.3/NuOCR/util.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:37:31.045163 NuOCR-0.2.5.3/NuOCR.egg-info/
+-rw-rw-rw-   0        0        0      540 2023-06-01 09:37:29.000000 NuOCR-0.2.5.3/NuOCR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1732 2023-06-01 09:37:30.000000 NuOCR-0.2.5.3/NuOCR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 09:37:29.000000 NuOCR-0.2.5.3/NuOCR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-01 09:37:29.000000 NuOCR-0.2.5.3/NuOCR.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-01 09:37:29.000000 NuOCR-0.2.5.3/NuOCR.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      540 2023-06-01 09:37:31.655363 NuOCR-0.2.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4053 2023-03-27 09:59:59.000000 NuOCR-0.2.5.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-01 09:37:31.665333 NuOCR-0.2.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1132 2023-06-01 09:37:26.000000 NuOCR-0.2.5.3/setup.py
```

### Comparing `NuOCR-0.2.5.2/NuOCR/admin.py` & `NuOCR-0.2.5.3/NuOCR/admin.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/extractor.py` & `NuOCR-0.2.5.3/NuOCR/extractor.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/extractor/extractor_pb2.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/extractor/extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/monitor/monitor_pb2.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/monitor/monitor_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/text_processors/text_processor_pb2.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/text_processors/text_processor_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/text_processors/text_processor_pb2_grpc.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/text_processors/text_processor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/auth_pb2.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/user/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/auth_pb2_grpc.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/user/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/user_pb2.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/user/user_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/user_pb2_grpc.py` & `NuOCR-0.2.5.3/NuOCR/gRPC_proto/user/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/io_adaptor.py` & `NuOCR-0.2.5.3/NuOCR/io_adaptor.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/monitor.py` & `NuOCR-0.2.5.3/NuOCR/monitor.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/preprocessors.py` & `NuOCR-0.2.5.3/NuOCR/preprocessors.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/templated_flow.py` & `NuOCR-0.2.5.3/NuOCR/templated_flow.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/text.py` & `NuOCR-0.2.5.3/NuOCR/text.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR/user.py` & `NuOCR-0.2.5.3/NuOCR/user.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/NuOCR.egg-info/PKG-INFO` & `NuOCR-0.2.5.3/NuOCR.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuOCR
-Version: 0.2.5.2
+Version: 0.2.5.3
 Summary: Using NuOCR service via APIs
 Author: Nuvento Systems Pvt. Ltd. (Jigar Makwana)
 Author-email: <makwana.jigar@nuvento.com>
 Keywords: python,NuOCR,OCR
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NuOCR-0.2.5.2/NuOCR.egg-info/SOURCES.txt` & `NuOCR-0.2.5.3/NuOCR.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 setup.py
 NuOCR/__init__.py
 NuOCR/admin.py
 NuOCR/channel.py
 NuOCR/extractor.py
 NuOCR/io_adaptor.py
 NuOCR/monitor.py
+NuOCR/multiformats.py
 NuOCR/preprocessors.py
 NuOCR/templated_flow.py
 NuOCR/text.py
 NuOCR/user.py
 NuOCR/util.py
 NuOCR.egg-info/PKG-INFO
 NuOCR.egg-info/SOURCES.txt
@@ -22,14 +23,17 @@
 NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py
 NuOCR/gRPC_proto/io_adaptors/__init__.py
 NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py
 NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py
 NuOCR/gRPC_proto/monitor/__init__.py
 NuOCR/gRPC_proto/monitor/monitor_pb2.py
 NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py
+NuOCR/gRPC_proto/multiformats/__init__.py
+NuOCR/gRPC_proto/multiformats/multiformats_pb2.py
+NuOCR/gRPC_proto/multiformats/multiformats_pb2_grpc.py
 NuOCR/gRPC_proto/nufarm_poc/__init__.py
 NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py
 NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py
 NuOCR/gRPC_proto/preprocessor/__init__.py
 NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py
 NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py
 NuOCR/gRPC_proto/templated_flow/__init__.py
```

### Comparing `NuOCR-0.2.5.2/PKG-INFO` & `NuOCR-0.2.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuOCR
-Version: 0.2.5.2
+Version: 0.2.5.3
 Summary: Using NuOCR service via APIs
 Author: Nuvento Systems Pvt. Ltd. (Jigar Makwana)
 Author-email: <makwana.jigar@nuvento.com>
 Keywords: python,NuOCR,OCR
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NuOCR-0.2.5.2/README.md` & `NuOCR-0.2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.2/setup.py` & `NuOCR-0.2.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '0.2.5.2'
+VERSION = '0.2.5.3'
 DESCRIPTION = 'Using NuOCR service via APIs'
 LONG_DESCRIPTION = 'A package that allows to utilize NuOCR sevices through API implementation.'
 
 # Setting up
 setup(
     name="NuOCR",
     version=VERSION,
```

