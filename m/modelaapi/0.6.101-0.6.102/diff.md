# Comparing `tmp/modelaapi-0.6.101.tar.gz` & `tmp/modelaapi-0.6.102.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelaapi-0.6.101.tar", last modified: Wed May 24 23:38:09 2023, max compression
+gzip compressed data, was "modelaapi-0.6.102.tar", last modified: Thu Jun  1 21:52:40 2023, max compression
```

## Comparing `modelaapi-0.6.101.tar` & `modelaapi-0.6.102.tar`

### file list

```diff
@@ -1,481 +1,481 @@
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.285204 modelaapi-0.6.101/
--rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.101/AUTHORS.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.101/CONTRIBUTING.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.101/DESCRIPTION.md
--rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.101/HISTORY.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.101/LICENSE.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      437 2023-01-26 17:46:09.000000 modelaapi-0.6.101/MANIFEST.in
--rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.101/Makefile
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-05-24 23:38:09.285204 modelaapi-0.6.101/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.101/README.md
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/gogo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/gogo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/gogo/protobuf/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/gogo/protobuf/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/gogo/protobuf/gogoproto/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/gogo/protobuf/gogoproto/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23545 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51143 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/inference/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    25376 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/infra/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    27212 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/team/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/training/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    60842 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/account/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/account/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/account/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/account/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.257206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/alert/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/alert/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/alert/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/attachment/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/attachment/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/attachment/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/batchpredictord/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/batchpredictord/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7549 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/catalog/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/cloudproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6517 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16493 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/commit/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/commit/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/commit/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/common/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/common/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/common/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/common/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/connection/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/connection/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/connection/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8826 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14287 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/conversation/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/conversation/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/conversation/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/data/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/data/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    84527 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   111042 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataapp/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataapp/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataapp/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.261206 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipeline/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipeline/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipelinerun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproduct/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproduct/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproductversion/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproductversion/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataset/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataset/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataset/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19016 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    35095 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datasource/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datasource/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datasource/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dbproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dbproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/entity/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/entity/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/entity/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featuregroup/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featuregroup/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featurehistogram/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featurehistogram/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/fileservices/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/fileservices/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.265205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/fileservices/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/grpcinferenceservice/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18564 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/k8score/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/k8score/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/k8score/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/lab/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/lab/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/lab/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/license/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/license/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/license/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/license/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/model/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/model/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/model/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/model/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelasystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelasystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11304 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19008 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modeldsystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modeldsystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.269205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/notifier/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/notifier/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/notifier/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/objectstored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/objectstored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/objectstored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/offlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/onlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/postmortem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/postmortem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/postmortem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/prediction/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/prediction/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/prediction/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictionstore/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictionstore/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictor/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictor/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictor/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/publisherd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/publisherd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/publisherd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/recipe/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/recipe/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/recipe/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/reciperun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/reciperun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.273205 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/reciperun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/report/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/report/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/report/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/report/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/review/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/review/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/review/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/review/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/runbook/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/runbook/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/runbook/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/servingsite/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/servingsite/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/servingsite/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlquery/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlquery/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlqueryrun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/study/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/study/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/study/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/study/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/system/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/system/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/system/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/system/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/tenant/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/tenant/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/tenant/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/todo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/todo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/todo/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/trainerd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/trainerd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/trainerd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    22775 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    17719 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/userroleclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/userroleclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.277204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/virtualbucket/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/virtualbucket/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-05-24 23:35:11.000000 modelaapi-0.6.101/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/google/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/google/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/google/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/google/api/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-05-24 23:35:11.000000 modelaapi-0.6.101/google/api/annotations_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-05-24 23:35:11.000000 modelaapi-0.6.101/google/api/annotations_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-05-24 23:35:11.000000 modelaapi-0.6.101/google/api/http_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-05-24 23:35:11.000000 modelaapi-0.6.101/google/api/http_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/api/apps/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/api/apps/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/api/apps/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/api/apps/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-05-24 23:35:11.000000 modelaapi-0.6.101/k8s/io/api/apps/v1/generated_pb2.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/api/core/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/api/core/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/api/core/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/api/core/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-05-24 23:35:11.000000 modelaapi-0.6.101/k8s/io/api/core/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/api/core/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/api/rbac/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/api/rbac/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/api/rbac/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/api/rbac/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-05-24 23:35:11.000000 modelaapi-0.6.101/k8s/io/api/rbac/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/api/rbac/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/apimachinery/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/apimachinery/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/apimachinery/pkg/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/apimachinery/pkg/api/resource/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/api/resource/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-05-24 23:35:11.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/apimachinery/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/apimachinery/pkg/apis/meta/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/apis/meta/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/apimachinery/pkg/apis/meta/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-05-24 23:35:11.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/apimachinery/pkg/runtime/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/runtime/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-05-24 23:35:11.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/apimachinery/pkg/runtime/schema/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-05-24 23:35:11.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/apimachinery/pkg/util/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/util/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/k8s/io/apimachinery/pkg/util/intstr/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/util/intstr/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-05-24 23:35:11.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.101/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.281204 modelaapi-0.6.101/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.101/modelaapi/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.101/modelaapi/consts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.101/modelaapi/custom_transformers.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.101/modelaapi/graykite_model.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.101/modelaapi/ts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-05-24 23:38:07.000000 modelaapi-0.6.101/modelaapi/version.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-24 23:38:09.285204 modelaapi-0.6.101/modelaapi.egg-info/
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-05-24 23:38:09.000000 modelaapi-0.6.101/modelaapi.egg-info/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)    19381 2023-05-24 23:38:09.000000 modelaapi-0.6.101/modelaapi.egg-info/SOURCES.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-05-24 23:38:09.000000 modelaapi-0.6.101/modelaapi.egg-info/dependency_links.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-05-24 23:38:09.000000 modelaapi-0.6.101/modelaapi.egg-info/entry_points.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.101/modelaapi.egg-info/not-zip-safe
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-05-24 23:38:09.000000 modelaapi-0.6.101/modelaapi.egg-info/requires.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-05-24 23:38:09.000000 modelaapi-0.6.101/modelaapi.egg-info/top_level.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.101/requirements.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-05-24 23:38:09.285204 modelaapi-0.6.101/setup.cfg
--rw-rw-r--   0 liam      (1000) liam      (1000)     5349 2023-02-27 17:33:55.000000 modelaapi-0.6.101/setup.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.580294 modelaapi-0.6.102/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.102/AUTHORS.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.102/CONTRIBUTING.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.102/DESCRIPTION.md
+-rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.102/HISTORY.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.102/LICENSE.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      437 2023-01-26 17:46:09.000000 modelaapi-0.6.102/MANIFEST.in
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.102/Makefile
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-06-01 21:52:40.580294 modelaapi-0.6.102/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.102/README.md
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.508289 modelaapi-0.6.102/github/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.508289 modelaapi-0.6.102/github/com/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.508289 modelaapi-0.6.102/github/com/gogo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/gogo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/gogo/protobuf/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/gogo/protobuf/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/gogo/protobuf/gogoproto/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/gogo/protobuf/gogoproto/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23584 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51143 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/inference/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    25376 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/infra/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    25800 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/team/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/training/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    60860 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7549 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6517 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16493 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/common/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/common/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/common/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/common/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8826 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14287 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    82473 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   111042 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19016 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    35095 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.536291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.536291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.536291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.536291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.536291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.536291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.536291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18564 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.544291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.544291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.544291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.544291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.544291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.544291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.544291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.560293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.560293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.560293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.560293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.560293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    22775 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17719 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/google/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/google/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/google/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/google/api/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-06-01 21:27:56.000000 modelaapi-0.6.102/google/api/annotations_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/google/api/annotations_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-06-01 21:27:56.000000 modelaapi-0.6.102/google/api/http_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/google/api/http_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/k8s/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/k8s/io/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/k8s/io/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/k8s/io/api/apps/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/apps/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/k8s/io/api/apps/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/apps/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/api/apps/v1/generated_pb2.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/k8s/io/api/core/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/core/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/api/core/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/core/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/api/core/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/core/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/api/rbac/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/rbac/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/api/rbac/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/rbac/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/api/rbac/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/rbac/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/pkg/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/pkg/api/resource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/api/resource/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/meta/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/meta/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/meta/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.576294 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/schema/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.576294 modelaapi-0.6.102/k8s/io/apimachinery/pkg/util/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/util/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.576294 modelaapi-0.6.102/k8s/io/apimachinery/pkg/util/intstr/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/util/intstr/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.576294 modelaapi-0.6.102/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.102/modelaapi/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.102/modelaapi/consts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.102/modelaapi/custom_transformers.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.102/modelaapi/graykite_model.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.102/modelaapi/ts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-06-01 21:52:29.000000 modelaapi-0.6.102/modelaapi/version.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.580294 modelaapi-0.6.102/modelaapi.egg-info/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-06-01 21:52:40.000000 modelaapi-0.6.102/modelaapi.egg-info/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19381 2023-06-01 21:52:40.000000 modelaapi-0.6.102/modelaapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-06-01 21:52:40.000000 modelaapi-0.6.102/modelaapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-06-01 21:52:40.000000 modelaapi-0.6.102/modelaapi.egg-info/entry_points.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.102/modelaapi.egg-info/not-zip-safe
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-06-01 21:52:40.000000 modelaapi-0.6.102/modelaapi.egg-info/requires.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-06-01 21:52:40.000000 modelaapi-0.6.102/modelaapi.egg-info/top_level.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.102/requirements.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-06-01 21:52:40.580294 modelaapi-0.6.102/setup.cfg
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5349 2023-02-27 17:33:55.000000 modelaapi-0.6.102/setup.py
```

### Comparing `modelaapi-0.6.101/CONTRIBUTING.rst` & `modelaapi-0.6.102/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/LICENSE.txt` & `modelaapi-0.6.102/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/Makefile` & `modelaapi-0.6.102/Makefile`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/PKG-INFO` & `modelaapi-0.6.102/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.101
+Version: 0.6.102
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.101
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.102
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.101
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.102
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.101/README.md` & `modelaapi-0.6.102/README.md`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/gogo/protobuf/gogoproto/gogo_pb2.py` & `modelaapi-0.6.102/github/com/gogo/protobuf/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.api.resource import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_api_dot_resource_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x12\x37github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/api/resource/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\xae\x01\n\nAccessSpec\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\x10\n\x08nodePort\x18\x02 \x01(\x05\x12\x0c\n\x04path\x18\x03 \x01(\t\x12\x12\n\naccessType\x18\x04 \x01(\t\x12\x0c\n\x04rest\x18\x05 \x01(\x08\x12\x12\n\nauthMethod\x18\x06 \x01(\t\x12<\n\x0f\x61pikeySecretRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.SecretReference\"b\n\x12\x41\x63\x63ountPermissions\x12\x13\n\x0b\x61\x63\x63ountName\x18\x01 \x01(\t\x12\x37\n\x05roles\x18\x02 \x03(\x0b\x32(.k8s.io.api.core.v1.LocalObjectReference\"\xa5\x01\n\tAlgorithm\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AlgorithmSpec\"\xa4\x01\n\rAlgorithmList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xc0\x01\n\rAlgorithmSpec\x12\x15\n\rframeworkName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\r\n\x05tasks\x18\x04 \x03(\t\x12\x0e\n\x06sparse\x18\x05 \x01(\x08\x12W\n\x06ranges\x18\x06 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\xf3\x01\n\x05\x43loud\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudStatus\"\x9c\x01\n\tCloudList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Cloud\"\xec\x02\n\tCloudSpec\x12\x19\n\x11\x64\x65\x66\x61ultRegionName\x18\x01 \x01(\t\x12\x1f\n\x17\x64\x65\x66\x61ultMachineClassName\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x65\x66\x61ultGpuClassName\x18\x03 \x01(\t\x12]\n\x0emachineClasses\x18\x04 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClass\x12U\n\ngpuClasses\x18\x05 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClass\x12P\n\x07regions\x18\x06 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Region\"\xc7\x01\n\x0b\x43loudStatus\x12_\n\x0cmachineCosts\x18\x01 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClassCost\x12W\n\x08gpuCosts\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClassCost\"A\n\x0c\x43ompilerSpec\x12\x0e\n\x06\x65nable\x18\x01 \x01(\x08\x12\x10\n\x08\x63ompiler\x18\x02 \x01(\t\x12\x0f\n\x07targets\x18\x03 \x03(\t\"l\n\x0f\x43onfusionMatrix\x12Y\n\x04rows\x18\x01 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrixRow\"F\n\x12\x43onfusionMatrixRow\x12\t\n\x01t\x18\x01 \x01(\t\x12\t\n\x01p\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x05\x12\x0b\n\x03pct\x18\x04 \x01(\x01\";\n\x0c\x43ontainerLog\x12\x0b\n\x03job\x18\x01 \x01(\t\x12\x11\n\tcontainer\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\"\"\n\nCurvePoint\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\"(\n\nDataCenter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"\xda\x01\n\x0c\x44\x61taLocation\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x12\n\nbucketName\x18\x03 \x01(\t\x12\x0c\n\x04path\x18\x04 \x01(\t\x12\r\n\x05table\x18\x05 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x06 \x01(\t\x12\x0b\n\x03sql\x18\x07 \x01(\t\x12\r\n\x05topic\x18\x08 \x01(\t\x12\x0b\n\x03url\x18\t \x01(\t\x12\x38\n\x0bresourceRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xc5\x04\n\x0c\x44\x61taTestCase\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nassertThat\x18\x03 \x01(\t\x12\x36\n\tentityRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0c\x63ompareToRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\x12\x0c\n\x04type\x18\x07 \x01(\t\x12\x0e\n\x06metric\x18\x08 \x01(\t\x12\x15\n\rexpectedValue\x18\t \x01(\x01\x12\x18\n\x10\x65xpectedCategory\x18\n \x01(\t\x12\r\n\x05lower\x18\x0b \x01(\x01\x12\r\n\x05upper\x18\x0c \x01(\x01\x12\x13\n\x0b\x65xpectedSet\x18\r \x03(\t\x12\x16\n\x0elowerInclusive\x18\x0e \x01(\x08\x12\x16\n\x0eupperInclusive\x18\x0f \x01(\x08\x12\x11\n\tgenerated\x18\x10 \x01(\x08\x12\x0c\n\x04tags\x18\x11 \x03(\t\x12\x0f\n\x07\x63olumn2\x18\x12 \x01(\t\x12\x37\n\nentityRef2\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07\x63olumns\x18\x14 \x03(\t\x12\x15\n\rfeatureFilter\x18\x15 \x01(\t\x12\x12\n\ndataFilter\x18\x16 \x01(\t\x12\x15\n\rreferenceType\x18\x17 \x01(\t\x12\x0f\n\x07periods\x18\x18 \x01(\x05\"\xac\x01\n\x12\x44\x61taTestCaseResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12T\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x0f\n\x07\x66\x61ilure\x18\x03 \x01(\x08\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\"0\n\x0c\x46ileLocation\x12\x12\n\nbucketName\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"t\n\x0cGithubEvents\x12\x19\n\x11gitConnectionName\x18\x01 \x01(\t\x12\x12\n\nrepository\x18\x02 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x15\n\rblobNameRegex\x18\x04 \x01(\t\x12\x0e\n\x06\x65vents\x18\x05 \x03(\t\"z\n\x08GpuClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12\x0c\n\x04vcpu\x18\x03 \x01(\x05\x12>\n\x06gpumem\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xb5\x01\n\x0cGpuClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"c\n\rHistogramData\x12\x0c\n\x04\x62ins\x18\x01 \x03(\x01\x12\x12\n\ncategories\x18\x02 \x03(\t\x12\x0e\n\x06\x63ounts\x18\x03 \x03(\x01\x12\x0f\n\x07missing\x18\x04 \x01(\x05\x12\x0f\n\x07invalid\x18\x05 \x01(\x05\"I\n\x06Images\x12\x14\n\x0ctrainerImage\x18\x01 \x01(\t\x12\x11\n\tdataImage\x18\x02 \x01(\t\x12\x16\n\x0epublisherImage\x18\x03 \x01(\t\"\xaf\x01\n\rLastRunStatus\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08\x64uration\x18\x04 \x01(\x05\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\"*\n\x03Lib\x12\x12\n\nframeworks\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"q\n\x04Logs\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12Y\n\ncontainers\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ContainerLog\"\xa9\x01\n\x0bMLFramework\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFrameworkSpec\"\xa8\x01\n\x0fMLFrameworkList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFramework\"R\n\x0fMLFrameworkSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x0c\n\x04lang\x18\x04 \x01(\t\"\x8c\x01\n\x0cMachineClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12;\n\x03mem\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12\x0c\n\x04vcpu\x18\x04 \x01(\x05\x12\x0f\n\x07storage\x18\x05 \x01(\t\"\xb9\x01\n\x10MachineClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xab\x01\n\x0cManagedImage\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImageSpec\"\xaa\x01\n\x10ManagedImageList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImage\"\xbb\x03\n\x10ManagedImageSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x10\n\x08registry\x18\x02 \x01(\t\x12\x12\n\nrepository\x18\x03 \x01(\t\x12\x0b\n\x03tag\x18\x04 \x01(\t\x12\'\n\x03\x65nv\x18\x05 \x03(\x0b\x32\x1a.k8s.io.api.core.v1.EnvVar\x12\x0b\n\x03gpu\x18\x06 \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\x07 \x01(\x08\x12\x0f\n\x07preload\x18\x08 \x01(\x08\x12:\n\rconnectionRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04\x62\x61se\x18\n \x01(\t\x12\x0c\n\x04role\x18\x0b \x01(\t\x12\x13\n\x0bmantainedBy\x18\x0c \x01(\t\x12\x0b\n\x03uri\x18\r \x01(\t\x12\x12\n\nframeworks\x18\x0e \x03(\t\x12J\n\x04libs\x18\x0f \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Lib\x12\n\n\x02os\x18\x10 \x01(\t\x12\x11\n\tosVersion\x18\x11 \x01(\t\x12\x0f\n\x07private\x18\x12 \x01(\x08\"\x9a\x02\n\x0bMeasurement\x12\x33\n\x06\x65ntity\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0e\n\x06metric\x18\x03 \x01(\t\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0e\n\x06stddev\x18\x05 \x01(\x01\x12\x0f\n\x07\x62oolQty\x18\x06 \x01(\x08\x12\x10\n\x08\x63\x61tegory\x18\x07 \x01(\t\x12\x10\n\x08valueSet\x18\x08 \x03(\t\x12=\n\ttimePoint\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08taskType\x18\n \x01(\t\x12\x11\n\talgorithm\x18\x0b \x01(\t\"\xb3\x02\n\x13ModelDeploymentSpec\x12\x35\n\x08modelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x14\n\x0cmodelVersion\x18\x03 \x01(\t\x12\x0f\n\x07traffic\x18\x04 \x01(\x05\x12\x0c\n\x04role\x18\x05 \x01(\t\x12\x10\n\x08mountTar\x18\t \x01(\x08\x12\x17\n\x0ftrafficSelector\x18\n \x01(\t\x12\x37\n\napprovedBy\x18\x0c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\r \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xea\x01\n\x10NotificationSpec\x12\x10\n\x08\x65rrorTTL\x18\x02 \x01(\x05\x12\x12\n\nsuccessTTL\x18\x04 \x01(\x05\x12\x14\n\x0cnotifierName\x18\x05 \x01(\t\x12i\n\x08selector\x18\x06 \x03(\x0b\x32W.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec.SelectorEntry\x1a/\n\rSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\rObjectiveSpec\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x0c\n\x04goal\x18\x02 \x01(\t\"^\n\x07PRCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"\x93\x02\n\x0eParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03low\x18\x03 \x01(\x01\x12\x0c\n\x04high\x18\x04 \x01(\x01\x12\x0c\n\x04step\x18\x05 \x01(\x05\x12\x0b\n\x03log\x18\x06 \x01(\x08\x12\x0f\n\x07\x63hoices\x18\x07 \x03(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x08 \x01(\x01\x12\x15\n\rdefaultChoice\x18\t \x01(\t\x12\x13\n\x0b\x63onditional\x18\n \x01(\x08\x12\x0e\n\x06parent\x18\x0b \x01(\t\x12\x16\n\x0eparentValueCat\x18\x0c \x01(\t\x12\x1a\n\x12parentValueInteger\x18\r \x01(\x05\x12\x18\n\x10parentValueFloat\x18\x0e \x01(\x01\"p\n\x0fPermissionsSpec\x12]\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccountPermissions\"\xb1\x01\n\x0fPretrainedModel\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModelSpec\"\xb0\x01\n\x13PretrainedModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModel\"$\n\x13PretrainedModelSpec\x12\r\n\x05image\x18\x01 \x01(\t\"\xad\x01\n\rPublicDataset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDatasetSpec\"\xac\x01\n\x11PublicDatasetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDataset\"\xb6\x02\n\x11PublicDatasetSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12\x10\n\x08openMLID\x18\x04 \x01(\t\x12\x0f\n\x07\x64\x61taUrl\x18\x05 \x01(\t\x12\x10\n\x08\x63itation\x18\x06 \x01(\t\x12\x0c\n\x04rows\x18\x07 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x08 \x01(\x05\x12\x10\n\x08\x66ileSize\x18\t \x01(\x05\x12\x14\n\x0ctargetColumn\x18\n \x01(\t\x12\x10\n\x08industry\x18\x0b \x01(\t\x12\x12\n\nimbalanced\x18\x0c \x01(\x08\x12\x14\n\x0c\x64\x61tasourceCR\x18\r \x01(\t\x12\x11\n\tdatasetCR\x18\x0e \x01(\t\x12\x0f\n\x07studyCR\x18\x0f \x01(\t\x12\x15\n\rdataProductCR\x18\x10 \x01(\t\"\xb6\x01\n\x06Region\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x1d\n\x15\x64\x65\x66\x61ultDatacenterName\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x13\n\x0b\x62illingCode\x18\x04 \x01(\t\x12X\n\x0b\x64\x61tacenters\x18\x05 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataCenter\"?\n\x13ResourceConsumption\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x04\x12\x0e\n\x06memory\x18\x02 \x01(\x04\x12\x0b\n\x03gpu\x18\x03 \x01(\x04\"t\n\x0cResourceSpec\x12\x14\n\x0cworkloadName\x18\x01 \x01(\t\x12\x0e\n\x06\x63ustom\x18\x02 \x01(\x08\x12>\n\x0crequirements\x18\x03 \x01(\x0b\x32(.k8s.io.api.core.v1.ResourceRequirements\"b\n\x0bRocAucCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"\xcd\x01\n\x0bRunSchedule\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x63ron\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x15\n\rmaxRetryCount\x18\x04 \x01(\x05\x12\x15\n\rretryDelaySec\x18\x05 \x01(\x05\x12\x12\n\ntimeoutSec\x18\x06 \x01(\x05\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12=\n\tnextRunAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xfe\x01\n\x11RunScheduleStatus\x12=\n\tlastRunAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x02 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x03 \x01(\t\x12\x13\n\x0blastRunName\x18\x04 \x01(\t\x12R\n\x0blastRunLogs\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x12\n\nretryCount\x18\x06 \x01(\x05\"r\n\tTestSuite\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12T\n\x05tests\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCase\"\xc7\x02\n\x0fTestSuiteResult\x12\x36\n\tentityRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08\x66\x61ilures\x18\x02 \x01(\x05\x12\x0e\n\x06\x65rrors\x18\x03 \x01(\x05\x12=\n\tstartedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12Z\n\x05tests\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCaseResult\"G\n\x0fWorkerRunResult\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"\xad\x01\n\rWorkloadClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClassSpec\"\xac\x01\n\x11WorkloadClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClass\"u\n\x11WorkloadClassSpec\x12`\n\x11resourcesTemplate\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpecB9Z7github.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x12\x37github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/api/resource/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\xae\x01\n\nAccessSpec\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\x10\n\x08nodePort\x18\x02 \x01(\x05\x12\x0c\n\x04path\x18\x03 \x01(\t\x12\x12\n\naccessType\x18\x04 \x01(\t\x12\x0c\n\x04rest\x18\x05 \x01(\x08\x12\x12\n\nauthMethod\x18\x06 \x01(\t\x12<\n\x0f\x61pikeySecretRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.SecretReference\"b\n\x12\x41\x63\x63ountPermissions\x12\x13\n\x0b\x61\x63\x63ountName\x18\x01 \x01(\t\x12\x37\n\x05roles\x18\x02 \x03(\x0b\x32(.k8s.io.api.core.v1.LocalObjectReference\"\xa5\x01\n\tAlgorithm\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AlgorithmSpec\"\xa4\x01\n\rAlgorithmList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xc0\x01\n\rAlgorithmSpec\x12\x15\n\rframeworkName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\r\n\x05tasks\x18\x04 \x03(\t\x12\x0e\n\x06sparse\x18\x05 \x01(\x08\x12W\n\x06ranges\x18\x06 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\xf3\x01\n\x05\x43loud\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudStatus\"\x9c\x01\n\tCloudList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Cloud\"\xec\x02\n\tCloudSpec\x12\x19\n\x11\x64\x65\x66\x61ultRegionName\x18\x01 \x01(\t\x12\x1f\n\x17\x64\x65\x66\x61ultMachineClassName\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x65\x66\x61ultGpuClassName\x18\x03 \x01(\t\x12]\n\x0emachineClasses\x18\x04 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClass\x12U\n\ngpuClasses\x18\x05 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClass\x12P\n\x07regions\x18\x06 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Region\"\xc7\x01\n\x0b\x43loudStatus\x12_\n\x0cmachineCosts\x18\x01 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClassCost\x12W\n\x08gpuCosts\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClassCost\"A\n\x0c\x43ompilerSpec\x12\x0e\n\x06\x65nable\x18\x01 \x01(\x08\x12\x10\n\x08\x63ompiler\x18\x02 \x01(\t\x12\x0f\n\x07targets\x18\x03 \x03(\t\"l\n\x0f\x43onfusionMatrix\x12Y\n\x04rows\x18\x01 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrixRow\"F\n\x12\x43onfusionMatrixRow\x12\t\n\x01t\x18\x01 \x01(\t\x12\t\n\x01p\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x05\x12\x0b\n\x03pct\x18\x04 \x01(\x01\"K\n\x0c\x43ontainerLog\x12\x0b\n\x03job\x18\x01 \x01(\t\x12\x11\n\tcontainer\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x04 \x01(\t\"\"\n\nCurvePoint\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\"(\n\nDataCenter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"\xda\x01\n\x0c\x44\x61taLocation\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x12\n\nbucketName\x18\x03 \x01(\t\x12\x0c\n\x04path\x18\x04 \x01(\t\x12\r\n\x05table\x18\x05 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x06 \x01(\t\x12\x0b\n\x03sql\x18\x07 \x01(\t\x12\r\n\x05topic\x18\x08 \x01(\t\x12\x0b\n\x03url\x18\t \x01(\t\x12\x38\n\x0bresourceRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xc5\x04\n\x0c\x44\x61taTestCase\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nassertThat\x18\x03 \x01(\t\x12\x36\n\tentityRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0c\x63ompareToRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\x12\x0c\n\x04type\x18\x07 \x01(\t\x12\x0e\n\x06metric\x18\x08 \x01(\t\x12\x15\n\rexpectedValue\x18\t \x01(\x01\x12\x18\n\x10\x65xpectedCategory\x18\n \x01(\t\x12\r\n\x05lower\x18\x0b \x01(\x01\x12\r\n\x05upper\x18\x0c \x01(\x01\x12\x13\n\x0b\x65xpectedSet\x18\r \x03(\t\x12\x16\n\x0elowerInclusive\x18\x0e \x01(\x08\x12\x16\n\x0eupperInclusive\x18\x0f \x01(\x08\x12\x11\n\tgenerated\x18\x10 \x01(\x08\x12\x0c\n\x04tags\x18\x11 \x03(\t\x12\x0f\n\x07\x63olumn2\x18\x12 \x01(\t\x12\x37\n\nentityRef2\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07\x63olumns\x18\x14 \x03(\t\x12\x15\n\rfeatureFilter\x18\x15 \x01(\t\x12\x12\n\ndataFilter\x18\x16 \x01(\t\x12\x15\n\rreferenceType\x18\x17 \x01(\t\x12\x0f\n\x07periods\x18\x18 \x01(\x05\"\xac\x01\n\x12\x44\x61taTestCaseResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12T\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x0f\n\x07\x66\x61ilure\x18\x03 \x01(\x08\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\"0\n\x0c\x46ileLocation\x12\x12\n\nbucketName\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"t\n\x0cGithubEvents\x12\x19\n\x11gitConnectionName\x18\x01 \x01(\t\x12\x12\n\nrepository\x18\x02 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x15\n\rblobNameRegex\x18\x04 \x01(\t\x12\x0e\n\x06\x65vents\x18\x05 \x03(\t\"z\n\x08GpuClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12\x0c\n\x04vcpu\x18\x03 \x01(\x05\x12>\n\x06gpumem\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xb5\x01\n\x0cGpuClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"c\n\rHistogramData\x12\x0c\n\x04\x62ins\x18\x01 \x03(\x01\x12\x12\n\ncategories\x18\x02 \x03(\t\x12\x0e\n\x06\x63ounts\x18\x03 \x03(\x01\x12\x0f\n\x07missing\x18\x04 \x01(\x05\x12\x0f\n\x07invalid\x18\x05 \x01(\x05\"I\n\x06Images\x12\x14\n\x0ctrainerImage\x18\x01 \x01(\t\x12\x11\n\tdataImage\x18\x02 \x01(\t\x12\x16\n\x0epublisherImage\x18\x03 \x01(\t\"\xaf\x01\n\rLastRunStatus\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08\x64uration\x18\x04 \x01(\x05\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\"*\n\x03Lib\x12\x12\n\nframeworks\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"q\n\x04Logs\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12Y\n\ncontainers\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ContainerLog\"\xa9\x01\n\x0bMLFramework\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFrameworkSpec\"\xa8\x01\n\x0fMLFrameworkList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFramework\"R\n\x0fMLFrameworkSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x0c\n\x04lang\x18\x04 \x01(\t\"\x8c\x01\n\x0cMachineClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12;\n\x03mem\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12\x0c\n\x04vcpu\x18\x04 \x01(\x05\x12\x0f\n\x07storage\x18\x05 \x01(\t\"\xb9\x01\n\x10MachineClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xab\x01\n\x0cManagedImage\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImageSpec\"\xaa\x01\n\x10ManagedImageList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImage\"\xbb\x03\n\x10ManagedImageSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x10\n\x08registry\x18\x02 \x01(\t\x12\x12\n\nrepository\x18\x03 \x01(\t\x12\x0b\n\x03tag\x18\x04 \x01(\t\x12\'\n\x03\x65nv\x18\x05 \x03(\x0b\x32\x1a.k8s.io.api.core.v1.EnvVar\x12\x0b\n\x03gpu\x18\x06 \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\x07 \x01(\x08\x12\x0f\n\x07preload\x18\x08 \x01(\x08\x12:\n\rconnectionRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04\x62\x61se\x18\n \x01(\t\x12\x0c\n\x04role\x18\x0b \x01(\t\x12\x13\n\x0bmantainedBy\x18\x0c \x01(\t\x12\x0b\n\x03uri\x18\r \x01(\t\x12\x12\n\nframeworks\x18\x0e \x03(\t\x12J\n\x04libs\x18\x0f \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Lib\x12\n\n\x02os\x18\x10 \x01(\t\x12\x11\n\tosVersion\x18\x11 \x01(\t\x12\x0f\n\x07private\x18\x12 \x01(\x08\"\x9a\x02\n\x0bMeasurement\x12\x33\n\x06\x65ntity\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0e\n\x06metric\x18\x03 \x01(\t\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0e\n\x06stddev\x18\x05 \x01(\x01\x12\x0f\n\x07\x62oolQty\x18\x06 \x01(\x08\x12\x10\n\x08\x63\x61tegory\x18\x07 \x01(\t\x12\x10\n\x08valueSet\x18\x08 \x03(\t\x12=\n\ttimePoint\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08taskType\x18\n \x01(\t\x12\x11\n\talgorithm\x18\x0b \x01(\t\"\xb3\x02\n\x13ModelDeploymentSpec\x12\x35\n\x08modelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x14\n\x0cmodelVersion\x18\x03 \x01(\t\x12\x0f\n\x07traffic\x18\x04 \x01(\x05\x12\x0c\n\x04role\x18\x05 \x01(\t\x12\x10\n\x08mountTar\x18\t \x01(\x08\x12\x17\n\x0ftrafficSelector\x18\n \x01(\t\x12\x37\n\napprovedBy\x18\x0c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\r \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xea\x01\n\x10NotificationSpec\x12\x10\n\x08\x65rrorTTL\x18\x02 \x01(\x05\x12\x12\n\nsuccessTTL\x18\x04 \x01(\x05\x12\x14\n\x0cnotifierName\x18\x05 \x01(\t\x12i\n\x08selector\x18\x06 \x03(\x0b\x32W.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec.SelectorEntry\x1a/\n\rSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\rObjectiveSpec\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x0c\n\x04goal\x18\x02 \x01(\t\"^\n\x07PRCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"\x93\x02\n\x0eParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03low\x18\x03 \x01(\x01\x12\x0c\n\x04high\x18\x04 \x01(\x01\x12\x0c\n\x04step\x18\x05 \x01(\x05\x12\x0b\n\x03log\x18\x06 \x01(\x08\x12\x0f\n\x07\x63hoices\x18\x07 \x03(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x08 \x01(\x01\x12\x15\n\rdefaultChoice\x18\t \x01(\t\x12\x13\n\x0b\x63onditional\x18\n \x01(\x08\x12\x0e\n\x06parent\x18\x0b \x01(\t\x12\x16\n\x0eparentValueCat\x18\x0c \x01(\t\x12\x1a\n\x12parentValueInteger\x18\r \x01(\x05\x12\x18\n\x10parentValueFloat\x18\x0e \x01(\x01\"p\n\x0fPermissionsSpec\x12]\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccountPermissions\"\xb1\x01\n\x0fPretrainedModel\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModelSpec\"\xb0\x01\n\x13PretrainedModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModel\"$\n\x13PretrainedModelSpec\x12\r\n\x05image\x18\x01 \x01(\t\"\xad\x01\n\rPublicDataset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDatasetSpec\"\xac\x01\n\x11PublicDatasetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDataset\"\xb6\x02\n\x11PublicDatasetSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12\x10\n\x08openMLID\x18\x04 \x01(\t\x12\x0f\n\x07\x64\x61taUrl\x18\x05 \x01(\t\x12\x10\n\x08\x63itation\x18\x06 \x01(\t\x12\x0c\n\x04rows\x18\x07 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x08 \x01(\x05\x12\x10\n\x08\x66ileSize\x18\t \x01(\x05\x12\x14\n\x0ctargetColumn\x18\n \x01(\t\x12\x10\n\x08industry\x18\x0b \x01(\t\x12\x12\n\nimbalanced\x18\x0c \x01(\x08\x12\x14\n\x0c\x64\x61tasourceCR\x18\r \x01(\t\x12\x11\n\tdatasetCR\x18\x0e \x01(\t\x12\x0f\n\x07studyCR\x18\x0f \x01(\t\x12\x15\n\rdataProductCR\x18\x10 \x01(\t\"\xb6\x01\n\x06Region\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x1d\n\x15\x64\x65\x66\x61ultDatacenterName\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x13\n\x0b\x62illingCode\x18\x04 \x01(\t\x12X\n\x0b\x64\x61tacenters\x18\x05 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataCenter\"?\n\x13ResourceConsumption\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x04\x12\x0e\n\x06memory\x18\x02 \x01(\x04\x12\x0b\n\x03gpu\x18\x03 \x01(\x04\"t\n\x0cResourceSpec\x12\x14\n\x0cworkloadName\x18\x01 \x01(\t\x12\x0e\n\x06\x63ustom\x18\x02 \x01(\x08\x12>\n\x0crequirements\x18\x03 \x01(\x0b\x32(.k8s.io.api.core.v1.ResourceRequirements\"b\n\x0bRocAucCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"\xcd\x01\n\x0bRunSchedule\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x63ron\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x15\n\rmaxRetryCount\x18\x04 \x01(\x05\x12\x15\n\rretryDelaySec\x18\x05 \x01(\x05\x12\x12\n\ntimeoutSec\x18\x06 \x01(\x05\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12=\n\tnextRunAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xfe\x01\n\x11RunScheduleStatus\x12=\n\tlastRunAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x02 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x03 \x01(\t\x12\x13\n\x0blastRunName\x18\x04 \x01(\t\x12R\n\x0blastRunLogs\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x12\n\nretryCount\x18\x06 \x01(\x05\"r\n\tTestSuite\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12T\n\x05tests\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCase\"\xc7\x02\n\x0fTestSuiteResult\x12\x36\n\tentityRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08\x66\x61ilures\x18\x02 \x01(\x05\x12\x0e\n\x06\x65rrors\x18\x03 \x01(\x05\x12=\n\tstartedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12Z\n\x05tests\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCaseResult\"G\n\x0fWorkerRunResult\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"\xad\x01\n\rWorkloadClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClassSpec\"\xac\x01\n\x11WorkloadClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClass\"u\n\x11WorkloadClassSpec\x12`\n\x11resourcesTemplate\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpecB9Z7github.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z7github.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1'
@@ -49,105 +49,105 @@
   _COMPILERSPEC._serialized_start=2162
   _COMPILERSPEC._serialized_end=2227
   _CONFUSIONMATRIX._serialized_start=2229
   _CONFUSIONMATRIX._serialized_end=2337
   _CONFUSIONMATRIXROW._serialized_start=2339
   _CONFUSIONMATRIXROW._serialized_end=2409
   _CONTAINERLOG._serialized_start=2411
-  _CONTAINERLOG._serialized_end=2470
-  _CURVEPOINT._serialized_start=2472
-  _CURVEPOINT._serialized_end=2506
-  _DATACENTER._serialized_start=2508
-  _DATACENTER._serialized_end=2548
-  _DATALOCATION._serialized_start=2551
-  _DATALOCATION._serialized_end=2769
-  _DATATESTCASE._serialized_start=2772
-  _DATATESTCASE._serialized_end=3353
-  _DATATESTCASERESULT._serialized_start=3356
-  _DATATESTCASERESULT._serialized_end=3528
-  _FILELOCATION._serialized_start=3530
-  _FILELOCATION._serialized_end=3578
-  _GITHUBEVENTS._serialized_start=3580
-  _GITHUBEVENTS._serialized_end=3696
-  _GPUCLASS._serialized_start=3698
-  _GPUCLASS._serialized_end=3820
-  _GPUCLASSCOST._serialized_start=3823
-  _GPUCLASSCOST._serialized_end=4004
-  _HISTOGRAMDATA._serialized_start=4006
-  _HISTOGRAMDATA._serialized_end=4105
-  _IMAGES._serialized_start=4107
-  _IMAGES._serialized_end=4180
-  _LASTRUNSTATUS._serialized_start=4183
-  _LASTRUNSTATUS._serialized_end=4358
-  _LIB._serialized_start=4360
-  _LIB._serialized_end=4402
-  _LOGS._serialized_start=4404
-  _LOGS._serialized_end=4517
-  _MLFRAMEWORK._serialized_start=4520
-  _MLFRAMEWORK._serialized_end=4689
-  _MLFRAMEWORKLIST._serialized_start=4692
-  _MLFRAMEWORKLIST._serialized_end=4860
-  _MLFRAMEWORKSPEC._serialized_start=4862
-  _MLFRAMEWORKSPEC._serialized_end=4944
-  _MACHINECLASS._serialized_start=4947
-  _MACHINECLASS._serialized_end=5087
-  _MACHINECLASSCOST._serialized_start=5090
-  _MACHINECLASSCOST._serialized_end=5275
-  _MANAGEDIMAGE._serialized_start=5278
-  _MANAGEDIMAGE._serialized_end=5449
-  _MANAGEDIMAGELIST._serialized_start=5452
-  _MANAGEDIMAGELIST._serialized_end=5622
-  _MANAGEDIMAGESPEC._serialized_start=5625
-  _MANAGEDIMAGESPEC._serialized_end=6068
-  _MEASUREMENT._serialized_start=6071
-  _MEASUREMENT._serialized_end=6353
-  _MODELDEPLOYMENTSPEC._serialized_start=6356
-  _MODELDEPLOYMENTSPEC._serialized_end=6663
-  _NOTIFICATIONSPEC._serialized_start=6666
-  _NOTIFICATIONSPEC._serialized_end=6900
-  _NOTIFICATIONSPEC_SELECTORENTRY._serialized_start=6853
-  _NOTIFICATIONSPEC_SELECTORENTRY._serialized_end=6900
-  _OBJECTIVESPEC._serialized_start=6902
-  _OBJECTIVESPEC._serialized_end=6947
-  _PRCURVE._serialized_start=6949
-  _PRCURVE._serialized_end=7043
-  _PARAMETERRANGE._serialized_start=7046
-  _PARAMETERRANGE._serialized_end=7321
-  _PERMISSIONSSPEC._serialized_start=7323
-  _PERMISSIONSSPEC._serialized_end=7435
-  _PRETRAINEDMODEL._serialized_start=7438
-  _PRETRAINEDMODEL._serialized_end=7615
-  _PRETRAINEDMODELLIST._serialized_start=7618
-  _PRETRAINEDMODELLIST._serialized_end=7794
-  _PRETRAINEDMODELSPEC._serialized_start=7796
-  _PRETRAINEDMODELSPEC._serialized_end=7832
-  _PUBLICDATASET._serialized_start=7835
-  _PUBLICDATASET._serialized_end=8008
-  _PUBLICDATASETLIST._serialized_start=8011
-  _PUBLICDATASETLIST._serialized_end=8183
-  _PUBLICDATASETSPEC._serialized_start=8186
-  _PUBLICDATASETSPEC._serialized_end=8496
-  _REGION._serialized_start=8499
-  _REGION._serialized_end=8681
-  _RESOURCECONSUMPTION._serialized_start=8683
-  _RESOURCECONSUMPTION._serialized_end=8746
-  _RESOURCESPEC._serialized_start=8748
-  _RESOURCESPEC._serialized_end=8864
-  _ROCAUCCURVE._serialized_start=8866
-  _ROCAUCCURVE._serialized_end=8964
-  _RUNSCHEDULE._serialized_start=8967
-  _RUNSCHEDULE._serialized_end=9172
-  _RUNSCHEDULESTATUS._serialized_start=9175
-  _RUNSCHEDULESTATUS._serialized_end=9429
-  _TESTSUITE._serialized_start=9431
-  _TESTSUITE._serialized_end=9545
-  _TESTSUITERESULT._serialized_start=9548
-  _TESTSUITERESULT._serialized_end=9875
-  _WORKERRUNRESULT._serialized_start=9877
-  _WORKERRUNRESULT._serialized_end=9948
-  _WORKLOADCLASS._serialized_start=9951
-  _WORKLOADCLASS._serialized_end=10124
-  _WORKLOADCLASSLIST._serialized_start=10127
-  _WORKLOADCLASSLIST._serialized_end=10299
-  _WORKLOADCLASSSPEC._serialized_start=10301
-  _WORKLOADCLASSSPEC._serialized_end=10418
+  _CONTAINERLOG._serialized_end=2486
+  _CURVEPOINT._serialized_start=2488
+  _CURVEPOINT._serialized_end=2522
+  _DATACENTER._serialized_start=2524
+  _DATACENTER._serialized_end=2564
+  _DATALOCATION._serialized_start=2567
+  _DATALOCATION._serialized_end=2785
+  _DATATESTCASE._serialized_start=2788
+  _DATATESTCASE._serialized_end=3369
+  _DATATESTCASERESULT._serialized_start=3372
+  _DATATESTCASERESULT._serialized_end=3544
+  _FILELOCATION._serialized_start=3546
+  _FILELOCATION._serialized_end=3594
+  _GITHUBEVENTS._serialized_start=3596
+  _GITHUBEVENTS._serialized_end=3712
+  _GPUCLASS._serialized_start=3714
+  _GPUCLASS._serialized_end=3836
+  _GPUCLASSCOST._serialized_start=3839
+  _GPUCLASSCOST._serialized_end=4020
+  _HISTOGRAMDATA._serialized_start=4022
+  _HISTOGRAMDATA._serialized_end=4121
+  _IMAGES._serialized_start=4123
+  _IMAGES._serialized_end=4196
+  _LASTRUNSTATUS._serialized_start=4199
+  _LASTRUNSTATUS._serialized_end=4374
+  _LIB._serialized_start=4376
+  _LIB._serialized_end=4418
+  _LOGS._serialized_start=4420
+  _LOGS._serialized_end=4533
+  _MLFRAMEWORK._serialized_start=4536
+  _MLFRAMEWORK._serialized_end=4705
+  _MLFRAMEWORKLIST._serialized_start=4708
+  _MLFRAMEWORKLIST._serialized_end=4876
+  _MLFRAMEWORKSPEC._serialized_start=4878
+  _MLFRAMEWORKSPEC._serialized_end=4960
+  _MACHINECLASS._serialized_start=4963
+  _MACHINECLASS._serialized_end=5103
+  _MACHINECLASSCOST._serialized_start=5106
+  _MACHINECLASSCOST._serialized_end=5291
+  _MANAGEDIMAGE._serialized_start=5294
+  _MANAGEDIMAGE._serialized_end=5465
+  _MANAGEDIMAGELIST._serialized_start=5468
+  _MANAGEDIMAGELIST._serialized_end=5638
+  _MANAGEDIMAGESPEC._serialized_start=5641
+  _MANAGEDIMAGESPEC._serialized_end=6084
+  _MEASUREMENT._serialized_start=6087
+  _MEASUREMENT._serialized_end=6369
+  _MODELDEPLOYMENTSPEC._serialized_start=6372
+  _MODELDEPLOYMENTSPEC._serialized_end=6679
+  _NOTIFICATIONSPEC._serialized_start=6682
+  _NOTIFICATIONSPEC._serialized_end=6916
+  _NOTIFICATIONSPEC_SELECTORENTRY._serialized_start=6869
+  _NOTIFICATIONSPEC_SELECTORENTRY._serialized_end=6916
+  _OBJECTIVESPEC._serialized_start=6918
+  _OBJECTIVESPEC._serialized_end=6963
+  _PRCURVE._serialized_start=6965
+  _PRCURVE._serialized_end=7059
+  _PARAMETERRANGE._serialized_start=7062
+  _PARAMETERRANGE._serialized_end=7337
+  _PERMISSIONSSPEC._serialized_start=7339
+  _PERMISSIONSSPEC._serialized_end=7451
+  _PRETRAINEDMODEL._serialized_start=7454
+  _PRETRAINEDMODEL._serialized_end=7631
+  _PRETRAINEDMODELLIST._serialized_start=7634
+  _PRETRAINEDMODELLIST._serialized_end=7810
+  _PRETRAINEDMODELSPEC._serialized_start=7812
+  _PRETRAINEDMODELSPEC._serialized_end=7848
+  _PUBLICDATASET._serialized_start=7851
+  _PUBLICDATASET._serialized_end=8024
+  _PUBLICDATASETLIST._serialized_start=8027
+  _PUBLICDATASETLIST._serialized_end=8199
+  _PUBLICDATASETSPEC._serialized_start=8202
+  _PUBLICDATASETSPEC._serialized_end=8512
+  _REGION._serialized_start=8515
+  _REGION._serialized_end=8697
+  _RESOURCECONSUMPTION._serialized_start=8699
+  _RESOURCECONSUMPTION._serialized_end=8762
+  _RESOURCESPEC._serialized_start=8764
+  _RESOURCESPEC._serialized_end=8880
+  _ROCAUCCURVE._serialized_start=8882
+  _ROCAUCCURVE._serialized_end=8980
+  _RUNSCHEDULE._serialized_start=8983
+  _RUNSCHEDULE._serialized_end=9188
+  _RUNSCHEDULESTATUS._serialized_start=9191
+  _RUNSCHEDULESTATUS._serialized_end=9445
+  _TESTSUITE._serialized_start=9447
+  _TESTSUITE._serialized_end=9561
+  _TESTSUITERESULT._serialized_start=9564
+  _TESTSUITERESULT._serialized_end=9891
+  _WORKERRUNRESULT._serialized_start=9893
+  _WORKERRUNRESULT._serialized_end=9964
+  _WORKLOADCLASS._serialized_start=9967
+  _WORKLOADCLASS._serialized_end=10140
+  _WORKLOADCLASSLIST._serialized_start=10143
+  _WORKLOADCLASSLIST._serialized_end=10315
+  _WORKLOADCLASSSPEC._serialized_start=10317
+  _WORKLOADCLASSSPEC._serialized_end=10434
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.api.resource import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_api_dot_resource_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nEgithub.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x12\x35github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/api/resource/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\xf5\x01\n\x07\x41\x63\x63ount\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AccountSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AccountStatus\"\x9e\x01\n\x0b\x41\x63\x63ountList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Account\"\xd1\x02\n\x0b\x41\x63\x63ountSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08username\x18\x04 \x01(\t\x12\x11\n\tfirstName\x18\x05 \x01(\t\x12\x10\n\x08lastName\x18\x06 \x01(\t\x12\r\n\x05\x65mail\x18\x07 \x01(\t\x12\r\n\x05phone\x18\x08 \x01(\t\x12\r\n\x05\x61\x64min\x18\t \x01(\x08\x12\x10\n\x08memberOf\x18\x0b \x01(\t\x12\x15\n\rresetPassword\x18\r \x01(\x08\x12U\n\x06\x61vatar\x18\x12 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x18\n\x10\x66\x61voriteProducts\x18\x13 \x03(\t\"\xf0\x02\n\rAccountStatus\x12=\n\tupdatedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x13\n\x0bmodelsCount\x18\x05 \x01(\x05\x12\x19\n\x11modelClassesCount\x18\x06 \x01(\x05\x12\x17\n\x0fpredictorsCount\x18\x07 \x01(\x05\x12\x1a\n\x12\x66\x65\x61tureGroupsCount\x18\x08 \x01(\x05\x12\x15\n\rdatasetsCount\x18\t \x01(\x05\x12\x14\n\x0cmembersCount\x18\n \x01(\x05\x12\x43\n\nconditions\x18\x0b \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xef\x01\n\x05\x41lert\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AlertSpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AlertStatus\"\x9a\x01\n\tAlertList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Alert\"\x87\x03\n\tAlertSpec\x12\x0f\n\x07subject\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05level\x18\x03 \x01(\t\x12\x36\n\tentityRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x14\n\x0cnotifierName\x18\x05 \x01(\t\x12\r\n\x05owner\x18\x06 \x01(\t\x12\x0b\n\x03ttl\x18\x07 \x01(\x05\x12\\\n\x06\x66ields\x18\x08 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AlertSpec.FieldsEntry\x12\x0b\n\x03url\x18\t \x01(\t\x12\r\n\x05image\x18\n \x01(\t\x12\x36\n\ttenantRef\x18\x0b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x1a-\n\x0b\x46ieldsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x99\x02\n\x0b\x41lertStatus\x12;\n\x07\x66iredAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12=\n\tupdatedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xfe\x01\n\nAttachment\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AttachmentSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AttachmentStatus\"\xa4\x01\n\x0e\x41ttachmentList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Attachment\"\xc6\x01\n\x0e\x41ttachmentSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x36\n\tentityRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x12\n\nbucketName\x18\x04 \x01(\t\x12\x0c\n\x04path\x18\x05 \x01(\t\x12\x36\n\ttenantRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xe1\x01\n\x10\x41ttachmentStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"j\n\x14\x42ucketResourceQuotas\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x41\n\thardLimit\x18\x02 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xfe\x01\n\nConnection\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionStatus\"\xa4\x01\n\x0e\x43onnectionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xe6\x03\n\x0e\x43onnectionSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12\x10\n\x08provider\x18\x03 \x01(\t\x12i\n\nsecretData\x18\x04 \x03(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionSpec.SecretDataEntry\x12\x63\n\x07options\x18\x05 \x03(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionSpec.OptionsEntry\x12\r\n\x05owner\x18\x06 \x01(\t\x12\x36\n\tsecretRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.SecretReference\x1a\x31\n\x0fSecretDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe1\x01\n\x10\x43onnectionStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x97\x01\n\x0bIngressSpec\x12\x0c\n\x04\x66qdn\x18\x01 \x01(\t\x12\x0c\n\x04grpc\x18\x02 \x01(\x08\x12\x0c\n\x04rest\x18\x03 \x01(\x08\x12\x18\n\x10ingressClassName\x18\x04 \x01(\t\x12\x12\n\nissuerName\x18\x05 \x01(\t\x12\x19\n\x11\x63lusterIssuerName\x18\x06 \x01(\t\x12\x15\n\rtlsSecretName\x18\x07 \x01(\t\"\xe9\x01\n\x03Lab\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12L\n\x04spec\x18\x02 \x01(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LabSpec\x12P\n\x06status\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LabStatus\"\x96\x01\n\x07LabList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12I\n\x05items\x18\x02 \x03(\x0b\x32:.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Lab\"\xa3\x02\n\x07LabSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x36\n\ttenantRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06limits\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ResourceLimitSpec\x12\x62\n\x0f\x65xternalCluster\x18\x04 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualClusterSpec\x12\r\n\x05owner\x18\x05 \x01(\t\"\xab\x01\n\tLabStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x03 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf5\x01\n\x07License\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LicenseSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LicenseStatus\"\x9e\x01\n\x0bLicenseList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.License\"\xf9\x03\n\x0bLicenseSpec\x12\x36\n\tsecretRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.SecretReference\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12@\n\x0ctrialStartAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12>\n\ntrialEndAt\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0bmaxProducts\x18\x07 \x01(\x05\x12\x13\n\x0bmaxTrainers\x18\x08 \x01(\x05\x12\x12\n\nmaxServers\x18\t \x01(\x05\x12\x10\n\x08maxUsers\x18\n \x01(\x05\x12\x15\n\rmaxDataPlanes\x18\x0b \x01(\x05\x12\x10\n\x08\x66orecast\x18\x0c \x01(\x08\x12\x0b\n\x03nlp\x18\r \x01(\x08\x12\x0e\n\x06vision\x18\x0e \x01(\x08\x12\x0f\n\x07\x63hatbot\x18\x0f \x01(\x08\x12\x13\n\x0bproductName\x18\x10 \x01(\t\x12\x11\n\tpriceName\x18\x11 \x01(\t\x12<\n\x08\x65xpireAt\x18\x12 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x14\n\x0cnotifierName\x18\x13 \x01(\t\"\xde\x01\n\rLicenseStatus\x12=\n\tupdatedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x84\x02\n\x0cModelaSystem\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12U\n\x04spec\x18\x02 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ModelaSystemSpec\x12Y\n\x06status\x18\x03 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ModelaSystemStatus\"\xa8\x01\n\x10ModelaSystemList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12R\n\x05items\x18\x02 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ModelaSystem\"j\n\x10ModelaSystemSpec\x12\x0f\n\x07release\x18\x01 \x01(\t\x12\x17\n\x0fimagePullPolicy\x18\x02 \x01(\t\x12\x14\n\x0cvaultAddress\x18\x03 \x01(\t\x12\x16\n\x0evaultMountPath\x18\x04 \x01(\t\"\xb9\x01\n\x12ModelaSystemStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12\x15\n\rfailureReason\x18\x02 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x03 \x01(\t\x12\x13\n\x0blastRelease\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xe6\x01\n\x17NotificationChannelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x0c\n\x04info\x18\x03 \x01(\x08\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x38\n\x04\x66rom\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x36\n\x02to\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0b\x64\x65stination\x18\x07 \x01(\t\"\x8d\x01\n\x19NotificationChannelStatus\x12\x41\n\rlastMessageAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x02 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x03 \x01(\t\"\xf8\x01\n\x08Notifier\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotifierSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotifierStatus\"\xa0\x01\n\x0cNotifierList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Notifier\"\xdd\x01\n\x0cNotifierSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x36\n\ttenantRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12`\n\x08\x63hannels\x18\x05 \x03(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotificationChannelSpec\"\x9a\x02\n\x0eNotifierStatus\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12=\n\tupdatedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12h\n\x0e\x63hannelsStatus\x18\x04 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotificationChannelStatus\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xb3\x02\n\x11ResourceLimitSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12>\n\x06maxMem\x18\x02 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12>\n\x06maxCpu\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12\x0f\n\x07maxPods\x18\x04 \x01(\x05\x12\x0e\n\x06maxPvc\x18\x05 \x01(\x05\x12\x34\n\x05quota\x18\x06 \x01(\x0b\x32%.k8s.io.api.core.v1.ResourceQuotaSpec\x12\x36\n\nlimitRange\x18\x07 \x01(\x0b\x32\".k8s.io.api.core.v1.LimitRangeSpec\"+\n\x08RuleSpec\x12\x10\n\x08resource\x18\x01 \x01(\t\x12\r\n\x05verbs\x18\x02 \x03(\t\"\x81\x02\n\x0bServingSite\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ServingSiteSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ServingSiteStatus\"\xa6\x01\n\x0fServingSiteList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ServingSite\"\x8f\x03\n\x0fServingSiteSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x36\n\ttenantRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06limits\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ResourceLimitSpec\x12S\n\x07ingress\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.IngressSpec\x12\x62\n\x0f\x65xternalCluster\x18\x05 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualClusterSpec\x12\r\n\x05owner\x18\x07 \x01(\t\x12\r\n\x05stage\x18\x08 \x01(\t\"\x90\x04\n\x11ServingSiteStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x18\n\x10\x61\x63tivePredictors\x18\x03 \x01(\x05\x12\x1a\n\x12inactivePredictors\x18\x04 \x01(\x05\x12#\n\x1btotalPredictorServiceFailed\x18\x05 \x01(\x05\x12%\n\x1dtotalPredictorDataDriftFailed\x18\x06 \x01(\x05\x12$\n\x1ctotalPredictorAccuracyFailed\x18\x07 \x01(\x05\x12\x1e\n\x16\x64\x61ilyPredictionsCounts\x18\x08 \x03(\x05\x12\x15\n\rfailureReason\x18\t \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12\x17\n\x0fgrpcIngressName\x18\x0b \x01(\t\x12\x17\n\x0frestIngressName\x18\x0c \x01(\t\x12\x18\n\x10grpcIngressReady\x18\r \x01(\x08\x12\x18\n\x10restIngressReady\x18\x0e \x01(\x08\x12\x43\n\nconditions\x18\x0f \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf2\x01\n\x06Tenant\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.TenantSpec\x12S\n\x06status\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.TenantStatus\"\x9c\x01\n\nTenantList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12L\n\x05items\x18\x02 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Tenant\"\xa7\x03\n\nTenantSpec\x12\x16\n\x0e\x64\x65\x66\x61ultLabName\x18\x01 \x01(\t\x12\x1e\n\x16\x64\x65\x66\x61ultServingSiteName\x18\x02 \x01(\t\x12\x19\n\x11\x64\x65\x66\x61ultBucketName\x18\x03 \x01(\t\x12]\n\x0bpermissions\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PermissionsSpec\x12_\n\x0cnotification\x18\x05 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\x42\n\x15onlineStoreConnection\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x42\n\x15metricStoreConnection\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xdd\x01\n\x0cTenantStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xab\x01\n\rUserRoleClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.UserRoleClassSpec\"\xaa\x01\n\x11UserRoleClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.UserRoleClass\"\xbf\x01\n\x11UserRoleClassSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05owner\x18\x03 \x01(\t\x12N\n\x05rules\x18\x04 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.RuleSpec\"\x87\x02\n\rVirtualBucket\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucketSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucketStatus\"\xaa\x01\n\x11VirtualBucketList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"\x88\x02\n\x11VirtualBucketSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12\x0e\n\x06region\x18\x05 \x01(\t\x12\x12\n\nversioning\x18\x06 \x01(\x08\x12[\n\x06quotas\x18\x07 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.BucketResourceQuotas\"\xe4\x01\n\x13VirtualBucketStatus\x12=\n\tupdatedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12\x15\n\rfailureReason\x18\x04 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x05 \x01(\t\x12\x43\n\nconditions\x18\x06 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdb\x03\n\x12VirtualClusterSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05nodes\x18\x03 \x01(\x05\x12\x14\n\x0cinstanceType\x18\x04 \x01(\t\x12\x0c\n\x04gpus\x18\x05 \x01(\x05\x12\x14\n\x0cgpuClassName\x18\x06 \x01(\t\x12\x12\n\nvolumeSize\x18\x07 \x01(\x05\x12\x0c\n\x04spot\x18\x08 \x01(\x08\x12\x16\n\x0e\x63onnectionName\x18\t \x01(\t\x12\r\n\x05owner\x18\n \x01(\t\x12X\n\x06limits\x18\x0b \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ResourceLimitSpec\x12\x0e\n\x06region\x18\x0c \x01(\t\x12\n\n\x02\x61z\x18\r \x01(\t\x12\x19\n\x11kubernetesVersion\x18\x0e \x01(\t\x12\x11\n\tautoscale\x18\x0f \x01(\x08\x12\x10\n\x08minNodes\x18\x10 \x01(\x05\x12\x10\n\x08maxNodes\x18\x11 \x01(\x05\x12\x35\n\x08\x63loudRef\x18\x12 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06sshKey\x18\x13 \x01(\tB7Z5github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nEgithub.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x12\x35github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/api/resource/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\xf5\x01\n\x07\x41\x63\x63ount\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AccountSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AccountStatus\"\x9e\x01\n\x0b\x41\x63\x63ountList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Account\"\xd1\x02\n\x0b\x41\x63\x63ountSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08username\x18\x04 \x01(\t\x12\x11\n\tfirstName\x18\x05 \x01(\t\x12\x10\n\x08lastName\x18\x06 \x01(\t\x12\r\n\x05\x65mail\x18\x07 \x01(\t\x12\r\n\x05phone\x18\x08 \x01(\t\x12\r\n\x05\x61\x64min\x18\t \x01(\x08\x12\x10\n\x08memberOf\x18\x0b \x01(\t\x12\x15\n\rresetPassword\x18\r \x01(\x08\x12U\n\x06\x61vatar\x18\x12 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x18\n\x10\x66\x61voriteProducts\x18\x13 \x03(\t\"\xf0\x02\n\rAccountStatus\x12=\n\tupdatedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x13\n\x0bmodelsCount\x18\x05 \x01(\x05\x12\x19\n\x11modelClassesCount\x18\x06 \x01(\x05\x12\x17\n\x0fpredictorsCount\x18\x07 \x01(\x05\x12\x1a\n\x12\x66\x65\x61tureGroupsCount\x18\x08 \x01(\x05\x12\x15\n\rdatasetsCount\x18\t \x01(\x05\x12\x14\n\x0cmembersCount\x18\n \x01(\x05\x12\x43\n\nconditions\x18\x0b \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xef\x01\n\x05\x41lert\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AlertSpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AlertStatus\"\x9a\x01\n\tAlertList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Alert\"\x87\x03\n\tAlertSpec\x12\x0f\n\x07subject\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05level\x18\x03 \x01(\t\x12\x36\n\tentityRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x14\n\x0cnotifierName\x18\x05 \x01(\t\x12\r\n\x05owner\x18\x06 \x01(\t\x12\x0b\n\x03ttl\x18\x07 \x01(\x05\x12\\\n\x06\x66ields\x18\x08 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AlertSpec.FieldsEntry\x12\x0b\n\x03url\x18\t \x01(\t\x12\r\n\x05image\x18\n \x01(\t\x12\x36\n\ttenantRef\x18\x0b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x1a-\n\x0b\x46ieldsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x99\x02\n\x0b\x41lertStatus\x12;\n\x07\x66iredAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12=\n\tupdatedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xfe\x01\n\nAttachment\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AttachmentSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AttachmentStatus\"\xa4\x01\n\x0e\x41ttachmentList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Attachment\"\xc6\x01\n\x0e\x41ttachmentSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x36\n\tentityRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x12\n\nbucketName\x18\x04 \x01(\t\x12\x0c\n\x04path\x18\x05 \x01(\t\x12\x36\n\ttenantRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xe1\x01\n\x10\x41ttachmentStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"j\n\x14\x42ucketResourceQuotas\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x41\n\thardLimit\x18\x02 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xfe\x01\n\nConnection\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionStatus\"\xa4\x01\n\x0e\x43onnectionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xe6\x03\n\x0e\x43onnectionSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12\x10\n\x08provider\x18\x03 \x01(\t\x12i\n\nsecretData\x18\x04 \x03(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionSpec.SecretDataEntry\x12\x63\n\x07options\x18\x05 \x03(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionSpec.OptionsEntry\x12\r\n\x05owner\x18\x06 \x01(\t\x12\x36\n\tsecretRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.SecretReference\x1a\x31\n\x0fSecretDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe1\x01\n\x10\x43onnectionStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x97\x01\n\x0bIngressSpec\x12\x0c\n\x04\x66qdn\x18\x01 \x01(\t\x12\x0c\n\x04grpc\x18\x02 \x01(\x08\x12\x0c\n\x04rest\x18\x03 \x01(\x08\x12\x18\n\x10ingressClassName\x18\x04 \x01(\t\x12\x12\n\nissuerName\x18\x05 \x01(\t\x12\x19\n\x11\x63lusterIssuerName\x18\x06 \x01(\t\x12\x15\n\rtlsSecretName\x18\x07 \x01(\t\"\xe9\x01\n\x03Lab\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12L\n\x04spec\x18\x02 \x01(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LabSpec\x12P\n\x06status\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LabStatus\"\x96\x01\n\x07LabList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12I\n\x05items\x18\x02 \x03(\x0b\x32:.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Lab\"\xa3\x02\n\x07LabSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x36\n\ttenantRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06limits\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ResourceLimitSpec\x12\x62\n\x0f\x65xternalCluster\x18\x04 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualClusterSpec\x12\r\n\x05owner\x18\x05 \x01(\t\"\xab\x01\n\tLabStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x03 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf5\x01\n\x07License\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LicenseSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LicenseStatus\"\x9e\x01\n\x0bLicenseList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.License\"\xf9\x03\n\x0bLicenseSpec\x12\x36\n\tsecretRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.SecretReference\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12@\n\x0ctrialStartAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12>\n\ntrialEndAt\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0bmaxProducts\x18\x07 \x01(\x05\x12\x13\n\x0bmaxTrainers\x18\x08 \x01(\x05\x12\x12\n\nmaxServers\x18\t \x01(\x05\x12\x10\n\x08maxUsers\x18\n \x01(\x05\x12\x15\n\rmaxDataPlanes\x18\x0b \x01(\x05\x12\x10\n\x08\x66orecast\x18\x0c \x01(\x08\x12\x0b\n\x03nlp\x18\r \x01(\x08\x12\x0e\n\x06vision\x18\x0e \x01(\x08\x12\x0f\n\x07\x63hatbot\x18\x0f \x01(\x08\x12\x13\n\x0bproductName\x18\x10 \x01(\t\x12\x11\n\tpriceName\x18\x11 \x01(\t\x12<\n\x08\x65xpireAt\x18\x12 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x14\n\x0cnotifierName\x18\x13 \x01(\t\"\xde\x01\n\rLicenseStatus\x12=\n\tupdatedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xe6\x01\n\x17NotificationChannelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x0c\n\x04info\x18\x03 \x01(\x08\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x38\n\x04\x66rom\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x36\n\x02to\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0b\x64\x65stination\x18\x07 \x01(\t\"\x8d\x01\n\x19NotificationChannelStatus\x12\x41\n\rlastMessageAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x02 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x03 \x01(\t\"\xf8\x01\n\x08Notifier\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotifierSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotifierStatus\"\xa0\x01\n\x0cNotifierList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Notifier\"\xdd\x01\n\x0cNotifierSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x36\n\ttenantRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12`\n\x08\x63hannels\x18\x05 \x03(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotificationChannelSpec\"\x9a\x02\n\x0eNotifierStatus\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12=\n\tupdatedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12h\n\x0e\x63hannelsStatus\x18\x04 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotificationChannelStatus\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xb3\x02\n\x11ResourceLimitSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12>\n\x06maxMem\x18\x02 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12>\n\x06maxCpu\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12\x0f\n\x07maxPods\x18\x04 \x01(\x05\x12\x0e\n\x06maxPvc\x18\x05 \x01(\x05\x12\x34\n\x05quota\x18\x06 \x01(\x0b\x32%.k8s.io.api.core.v1.ResourceQuotaSpec\x12\x36\n\nlimitRange\x18\x07 \x01(\x0b\x32\".k8s.io.api.core.v1.LimitRangeSpec\"+\n\x08RuleSpec\x12\x10\n\x08resource\x18\x01 \x01(\t\x12\r\n\x05verbs\x18\x02 \x03(\t\"\x81\x02\n\x0bServingSite\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ServingSiteSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ServingSiteStatus\"\xa6\x01\n\x0fServingSiteList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ServingSite\"\x8f\x03\n\x0fServingSiteSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x36\n\ttenantRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06limits\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ResourceLimitSpec\x12S\n\x07ingress\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.IngressSpec\x12\x62\n\x0f\x65xternalCluster\x18\x05 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualClusterSpec\x12\r\n\x05owner\x18\x07 \x01(\t\x12\r\n\x05stage\x18\x08 \x01(\t\"\x90\x04\n\x11ServingSiteStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x18\n\x10\x61\x63tivePredictors\x18\x03 \x01(\x05\x12\x1a\n\x12inactivePredictors\x18\x04 \x01(\x05\x12#\n\x1btotalPredictorServiceFailed\x18\x05 \x01(\x05\x12%\n\x1dtotalPredictorDataDriftFailed\x18\x06 \x01(\x05\x12$\n\x1ctotalPredictorAccuracyFailed\x18\x07 \x01(\x05\x12\x1e\n\x16\x64\x61ilyPredictionsCounts\x18\x08 \x03(\x05\x12\x15\n\rfailureReason\x18\t \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12\x17\n\x0fgrpcIngressName\x18\x0b \x01(\t\x12\x17\n\x0frestIngressName\x18\x0c \x01(\t\x12\x18\n\x10grpcIngressReady\x18\r \x01(\x08\x12\x18\n\x10restIngressReady\x18\x0e \x01(\x08\x12\x43\n\nconditions\x18\x0f \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf2\x01\n\x06Tenant\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.TenantSpec\x12S\n\x06status\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.TenantStatus\"\x9c\x01\n\nTenantList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12L\n\x05items\x18\x02 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Tenant\"\xa7\x03\n\nTenantSpec\x12\x16\n\x0e\x64\x65\x66\x61ultLabName\x18\x01 \x01(\t\x12\x1e\n\x16\x64\x65\x66\x61ultServingSiteName\x18\x02 \x01(\t\x12\x19\n\x11\x64\x65\x66\x61ultBucketName\x18\x03 \x01(\t\x12]\n\x0bpermissions\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PermissionsSpec\x12_\n\x0cnotification\x18\x05 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\x42\n\x15onlineStoreConnection\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x42\n\x15metricStoreConnection\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xdd\x01\n\x0cTenantStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xab\x01\n\rUserRoleClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.UserRoleClassSpec\"\xaa\x01\n\x11UserRoleClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.UserRoleClass\"\xbf\x01\n\x11UserRoleClassSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05owner\x18\x03 \x01(\t\x12N\n\x05rules\x18\x04 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.RuleSpec\"\x87\x02\n\rVirtualBucket\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucketSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucketStatus\"\xaa\x01\n\x11VirtualBucketList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"\x88\x02\n\x11VirtualBucketSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12\x0e\n\x06region\x18\x05 \x01(\t\x12\x12\n\nversioning\x18\x06 \x01(\x08\x12[\n\x06quotas\x18\x07 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.BucketResourceQuotas\"\xe4\x01\n\x13VirtualBucketStatus\x12=\n\tupdatedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12\x15\n\rfailureReason\x18\x04 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x05 \x01(\t\x12\x43\n\nconditions\x18\x06 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdb\x03\n\x12VirtualClusterSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05nodes\x18\x03 \x01(\x05\x12\x14\n\x0cinstanceType\x18\x04 \x01(\t\x12\x0c\n\x04gpus\x18\x05 \x01(\x05\x12\x14\n\x0cgpuClassName\x18\x06 \x01(\t\x12\x12\n\nvolumeSize\x18\x07 \x01(\x05\x12\x0c\n\x04spot\x18\x08 \x01(\x08\x12\x16\n\x0e\x63onnectionName\x18\t \x01(\t\x12\r\n\x05owner\x18\n \x01(\t\x12X\n\x06limits\x18\x0b \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ResourceLimitSpec\x12\x0e\n\x06region\x18\x0c \x01(\t\x12\n\n\x02\x61z\x18\r \x01(\t\x12\x19\n\x11kubernetesVersion\x18\x0e \x01(\t\x12\x11\n\tautoscale\x18\x0f \x01(\x08\x12\x10\n\x08minNodes\x18\x10 \x01(\x05\x12\x10\n\x08maxNodes\x18\x11 \x01(\x05\x12\x35\n\x08\x63loudRef\x18\x12 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06sshKey\x18\x13 \x01(\tB7Z5github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z5github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1'
@@ -87,64 +87,56 @@
   _LICENSE._serialized_end=6006
   _LICENSELIST._serialized_start=6009
   _LICENSELIST._serialized_end=6167
   _LICENSESPEC._serialized_start=6170
   _LICENSESPEC._serialized_end=6675
   _LICENSESTATUS._serialized_start=6678
   _LICENSESTATUS._serialized_end=6900
-  _MODELASYSTEM._serialized_start=6903
-  _MODELASYSTEM._serialized_end=7163
-  _MODELASYSTEMLIST._serialized_start=7166
-  _MODELASYSTEMLIST._serialized_end=7334
-  _MODELASYSTEMSPEC._serialized_start=7336
-  _MODELASYSTEMSPEC._serialized_end=7442
-  _MODELASYSTEMSTATUS._serialized_start=7445
-  _MODELASYSTEMSTATUS._serialized_end=7630
-  _NOTIFICATIONCHANNELSPEC._serialized_start=7633
-  _NOTIFICATIONCHANNELSPEC._serialized_end=7863
-  _NOTIFICATIONCHANNELSTATUS._serialized_start=7866
-  _NOTIFICATIONCHANNELSTATUS._serialized_end=8007
-  _NOTIFIER._serialized_start=8010
-  _NOTIFIER._serialized_end=8258
-  _NOTIFIERLIST._serialized_start=8261
-  _NOTIFIERLIST._serialized_end=8421
-  _NOTIFIERSPEC._serialized_start=8424
-  _NOTIFIERSPEC._serialized_end=8645
-  _NOTIFIERSTATUS._serialized_start=8648
-  _NOTIFIERSTATUS._serialized_end=8930
-  _RESOURCELIMITSPEC._serialized_start=8933
-  _RESOURCELIMITSPEC._serialized_end=9240
-  _RULESPEC._serialized_start=9242
-  _RULESPEC._serialized_end=9285
-  _SERVINGSITE._serialized_start=9288
-  _SERVINGSITE._serialized_end=9545
-  _SERVINGSITELIST._serialized_start=9548
-  _SERVINGSITELIST._serialized_end=9714
-  _SERVINGSITESPEC._serialized_start=9717
-  _SERVINGSITESPEC._serialized_end=10116
-  _SERVINGSITESTATUS._serialized_start=10119
-  _SERVINGSITESTATUS._serialized_end=10647
-  _TENANT._serialized_start=10650
-  _TENANT._serialized_end=10892
-  _TENANTLIST._serialized_start=10895
-  _TENANTLIST._serialized_end=11051
-  _TENANTSPEC._serialized_start=11054
-  _TENANTSPEC._serialized_end=11477
-  _TENANTSTATUS._serialized_start=11480
-  _TENANTSTATUS._serialized_end=11701
-  _USERROLECLASS._serialized_start=11704
-  _USERROLECLASS._serialized_end=11875
-  _USERROLECLASSLIST._serialized_start=11878
-  _USERROLECLASSLIST._serialized_end=12048
-  _USERROLECLASSSPEC._serialized_start=12051
-  _USERROLECLASSSPEC._serialized_end=12242
-  _VIRTUALBUCKET._serialized_start=12245
-  _VIRTUALBUCKET._serialized_end=12508
-  _VIRTUALBUCKETLIST._serialized_start=12511
-  _VIRTUALBUCKETLIST._serialized_end=12681
-  _VIRTUALBUCKETSPEC._serialized_start=12684
-  _VIRTUALBUCKETSPEC._serialized_end=12948
-  _VIRTUALBUCKETSTATUS._serialized_start=12951
-  _VIRTUALBUCKETSTATUS._serialized_end=13179
-  _VIRTUALCLUSTERSPEC._serialized_start=13182
-  _VIRTUALCLUSTERSPEC._serialized_end=13657
+  _NOTIFICATIONCHANNELSPEC._serialized_start=6903
+  _NOTIFICATIONCHANNELSPEC._serialized_end=7133
+  _NOTIFICATIONCHANNELSTATUS._serialized_start=7136
+  _NOTIFICATIONCHANNELSTATUS._serialized_end=7277
+  _NOTIFIER._serialized_start=7280
+  _NOTIFIER._serialized_end=7528
+  _NOTIFIERLIST._serialized_start=7531
+  _NOTIFIERLIST._serialized_end=7691
+  _NOTIFIERSPEC._serialized_start=7694
+  _NOTIFIERSPEC._serialized_end=7915
+  _NOTIFIERSTATUS._serialized_start=7918
+  _NOTIFIERSTATUS._serialized_end=8200
+  _RESOURCELIMITSPEC._serialized_start=8203
+  _RESOURCELIMITSPEC._serialized_end=8510
+  _RULESPEC._serialized_start=8512
+  _RULESPEC._serialized_end=8555
+  _SERVINGSITE._serialized_start=8558
+  _SERVINGSITE._serialized_end=8815
+  _SERVINGSITELIST._serialized_start=8818
+  _SERVINGSITELIST._serialized_end=8984
+  _SERVINGSITESPEC._serialized_start=8987
+  _SERVINGSITESPEC._serialized_end=9386
+  _SERVINGSITESTATUS._serialized_start=9389
+  _SERVINGSITESTATUS._serialized_end=9917
+  _TENANT._serialized_start=9920
+  _TENANT._serialized_end=10162
+  _TENANTLIST._serialized_start=10165
+  _TENANTLIST._serialized_end=10321
+  _TENANTSPEC._serialized_start=10324
+  _TENANTSPEC._serialized_end=10747
+  _TENANTSTATUS._serialized_start=10750
+  _TENANTSTATUS._serialized_end=10971
+  _USERROLECLASS._serialized_start=10974
+  _USERROLECLASS._serialized_end=11145
+  _USERROLECLASSLIST._serialized_start=11148
+  _USERROLECLASSLIST._serialized_end=11318
+  _USERROLECLASSSPEC._serialized_start=11321
+  _USERROLECLASSSPEC._serialized_end=11512
+  _VIRTUALBUCKET._serialized_start=11515
+  _VIRTUALBUCKET._serialized_end=11778
+  _VIRTUALBUCKETLIST._serialized_start=11781
+  _VIRTUALBUCKETLIST._serialized_end=11951
+  _VIRTUALBUCKETSPEC._serialized_start=11954
+  _VIRTUALBUCKETSPEC._serialized_end=12218
+  _VIRTUALBUCKETSTATUS._serialized_start=12221
+  _VIRTUALBUCKETSTATUS._serialized_end=12449
+  _VIRTUALCLUSTERSPEC._serialized_start=12452
+  _VIRTUALCLUSTERSPEC._serialized_end=12927
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_data_dot_v1alpha1_dot_generated__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x12\x38github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x80\x01\n\x17\x41lgorithmParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12W\n\x06ranges\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\x9f\x01\n\x18\x41lgorithmSearchSpaceSpec\x12\x0f\n\x07include\x18\x01 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\x12\x61\n\x06\x63ustom\x18\x03 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmParameterRange\"`\n\x07\x41nomaly\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bvalueColumn\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x64jDeltaColumn\x18\x03 \x01(\t\x12\r\n\x05start\x18\x04 \x01(\t\x12\x0b\n\x03\x65nd\x18\x05 \x01(\t\"\'\n\x11\x41udioPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"M\n\x0c\x42\x61\x63ktestSpec\x12\x0f\n\x07sliding\x18\x01 \x01(\x08\x12\x0e\n\x06splits\x18\x02 \x01(\x05\x12\x0f\n\x07Initial\x18\x03 \x01(\x05\x12\x0b\n\x03gap\x18\x05 \x01(\x05\"?\n\x0c\x42\x61selineSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbaselines\x18\x02 \x03(\t\x12\x0b\n\x03\x61ll\x18\x03 \x01(\x08\"\r\n\x0b\x43hangePoint\"$\n\x14\x43hatbotEstimatorSpec\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\"\x96\x01\n\x0e\x43heckpointSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1a\n\x12\x63heckpointInterval\x18\x02 \x01(\x05\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x92\x01\n\x16\x43lassicalEstimatorSpec\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12\x61\n\nparameters\x18\x02 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperParameterValue\"a\n\x10\x43ustomReportSpec\x12M\n\x05pages\x18\x08 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"L\n\nDataHashes\x12\x11\n\ttrainHash\x18\x01 \x01(\t\x12\x13\n\x0btestingHash\x18\x02 \x01(\t\x12\x16\n\x0evalidationHash\x18\x03 \x01(\t\"\x84\x02\n\rDataSplitSpec\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\r\n\x05train\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x0c\n\x04test\x18\x04 \x01(\x05\x12\x13\n\x0bsplitColumn\x18\x05 \x01(\t\x12W\n\x08segments\x18\x06 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SegmentSpec\x12\x14\n\x0ctrainDataset\x18\x07 \x01(\t\x12\x13\n\x0btestDataset\x18\x08 \x01(\t\x12\x19\n\x11validationDataset\x18\t \x01(\t\"\xa5\x01\n\x12\x44\x65\x65pEstimatorLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12^\n\nparameters\x18\x03 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NNLayerParameter\x12\x13\n\x0binputLayers\x18\x04 \x03(\t\"\xe6\x01\n\x11\x44\x65\x65pEstimatorSpec\x12\\\n\x06layers\x18\x01 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorLayer\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x11\n\tbatchSize\x18\x03 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x04 \x01(\x05\x12\x17\n\x0fvalidationSplit\x18\x05 \x01(\x05\x12\r\n\x05isSeq\x18\x06 \x01(\x08\x12\x0c\n\x04gpus\x18\x07 \x01(\x05\x12\x0c\n\x04loss\x18\x08 \x01(\t\".\n\x13\x44riftDetectorStatus\x12\x17\n\x0foutlierModelURI\x18\x01 \x01(\t\";\n\x0e\x44riftModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10outlierAlgorithm\x18\x02 \x01(\t\"R\n\rEarlyStopSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07initial\x18\x02 \x01(\x05\x12\x1f\n\x17minModelsWithNoProgress\x18\x03 \x01(\x05\"\x0f\n\rEnsembleRules\"\xf3\x01\n\x0c\x45nsembleSpec\x12\x0e\n\x06models\x18\x01 \x03(\t\x12\x64\n\nestimators\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12_\n\x05\x66inal\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x0c\n\x04type\x18\x04 \x01(\t\"_\n\rEnsemblesSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0evotingEnsemble\x18\x02 \x01(\x08\x12\x18\n\x10stackingEnsemble\x18\x03 \x01(\x08\x12\x0b\n\x03top\x18\x04 \x01(\x05\"*\n\tEntityRef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\"\x89\x01\n\x0b\x45valMetrics\x12\x11\n\tselection\x18\x01 \x01(\t\x12\x11\n\treporting\x18\x02 \x03(\t\x12\x0f\n\x07\x61ggFunc\x18\x03 \x01(\t\x12\x11\n\taggPeriod\x18\x04 \x01(\x05\x12\x17\n\x0fnullModelParams\x18\x05 \x01(\t\x12\x17\n\x0frelErrTolerance\x18\x06 \x01(\x01\"\xe0\x01\n\nEvalPeriod\x12\x13\n\x0btestHorizon\x18\x01 \x01(\x05\x12\x1f\n\x17periodsBetweenTrainTest\x18\x02 \x01(\x05\x12\x1e\n\x16\x63vPeriodsBetweenSplits\x18\x03 \x01(\x05\x12\x1a\n\x12\x63vExpandingWindows\x18\x04 \x01(\x08\x12\x11\n\tcvHorizon\x18\x05 \x01(\x05\x12\x19\n\x11\x63vMinTrainPeriods\x18\x06 \x01(\x05\x12\x13\n\x0b\x63vMaxSplits\x18\x07 \x01(\x05\x12\x1d\n\x15\x63vUseMostRecentSplits\x18\x08 \x01(\x08\"\xc7\x06\n\x1a\x46\x65\x61tureEngineeringPipeline\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\x12\x12\n\nimputation\x18\x04 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x05 \x01(\t\x12\x0f\n\x07scaling\x18\x06 \x01(\t\x12\x16\n\x0e\x64iscretisation\x18\x07 \x01(\t\x12\x1e\n\x16variableTransformation\x18\x08 \x01(\t\x12\x17\n\x0foutlierHandling\x18\t \x01(\t\x12\x1e\n\x16\x64\x61tetimeTransformation\x18\n \x01(\t\x12X\n\x04text\x18\x0b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TextPipelineSpec\x12Z\n\x05image\x18\x0c \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImagePipelineSpec\x12Z\n\x05\x61udio\x18\r \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AudioPipelineSpec\x12Z\n\x05video\x18\x0e \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.VideoPipelineSpec\x12`\n\tgenerated\x18\x10 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GeneratedColumnSpec\x12]\n\x06\x63ustom\x18\x11 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GeneratedColumnSpec\x12\x0c\n\x04\x64rop\x18\x12 \x01(\x08\x12\x13\n\x0bpassthrough\x18\x13 \x01(\x08\"\x8d\x03\n\x1c\x46\x65\x61tureEngineeringSearchSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x19\n\x11imbalancedHandler\x18\x02 \x01(\t\x12\x11\n\testimator\x18\x03 \x01(\t\x12\x11\n\tmaxModels\x18\x04 \x01(\x05\x12\x0f\n\x07maxTime\x18\x05 \x01(\x05\x12\x13\n\x0bmaxTrainers\x18\x06 \x01(\x05\x12\x11\n\tsamplePct\x18\x07 \x01(\x05\x12\x12\n\nautoRemove\x18\x08 \x01(\x08\x12\r\n\x05reuse\x18\t \x01(\x08\x12\x63\n\x0b\x66\x65Selection\x18\n \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\"\x80\x01\n\x1e\x46\x65\x61tureEngineeringSearchStatus\x12^\n\x04\x62\x65st\x18\x01 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\"\xf7\x01\n\x16\x46\x65\x61tureEngineeringSpec\x12g\n\tpipelines\x18\x01 \x03(\x0b\x32T.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringPipeline\x12\x11\n\timbalance\x18\x02 \x01(\t\x12\x61\n\tselection\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\"8\n\x11\x46\x65\x61tureImportance\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nimportance\x18\x02 \x01(\x01\":\n\x0b\x46\x65\x61tureInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\"#\n\x0b\x46\x65\x61turePair\x12\t\n\x01x\x18\x01 \x01(\t\x12\t\n\x01y\x18\x02 \x01(\t\"\xd5\x01\n\x14\x46\x65\x61tureSelectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tembedding\x18\x03 \x01(\x08\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\x08\x12\x0f\n\x07wrapper\x18\x05 \x01(\x08\x12\x10\n\x08pipeline\x18\x06 \x03(\t\x12\x14\n\x0cvarThreshold\x18\x07 \x01(\x05\x12\x15\n\rcorrThreshold\x18\x08 \x01(\x05\x12\x13\n\x0bmaxFeatures\x18\t \x01(\x05\x12\x12\n\npercentile\x18\n \x01(\x05\x12\x10\n\x08reserved\x18\x0c \x03(\t\"\xf8\x07\n\x0e\x46orecasterSpec\x12Y\n\x06\x65vents\x18\x02 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TimeSeriesEvent\x12R\n\x04past\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12T\n\x06\x66uture\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12\x10\n\x08\x63overage\x18\x06 \x01(\x01\x12]\n\x0eoutputLocation\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x10\n\x08\x66\x65\x61tures\x18\x08 \x03(\t\x12\x0e\n\x06groups\x18\t \x03(\t\x12\x1a\n\x12predefinedTemplate\x18\n \x01(\t\x12T\n\tanomalies\x18\x0b \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Anomaly\x12\x14\n\x0ctrainEndData\x18\x0c \x01(\t\x12\x13\n\x0bvalueColumn\x18\r \x01(\t\x12\x11\n\thpoBudget\x18\x0e \x01(\x05\x12`\n\x11\x65valuationMetrics\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalMetrics\x12^\n\x10\x65valuationPeriod\x18\x10 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalPeriod\x12^\n\x0bseasonality\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalitySpec\x12\x12\n\nregressors\x18\x12 \x03(\t\x12\x18\n\x10laggedRegressors\x18\x13 \x03(\t\x12\x0e\n\x06growth\x18\x14 \x01(\t\x12\x0b\n\x03key\x18\x15 \x03(\t\x12\x12\n\nestimators\x18\x16 \x03(\t\x12\x0b\n\x03hts\x18\x17 \x01(\t\"x\n\x15GarbageCollectionSpec\x12\x1e\n\x16\x63ollectAtModelClassEnd\x18\x01 \x01(\x08\x12%\n\x1dkeepOnlyBestModelPerAlgorithm\x18\x02 \x01(\x08\x12\x18\n\x10keepPrunedModels\x18\x03 \x01(\x08\"\x8e\x01\n\x17GarbageCollectionStatus\x12\x1c\n\x14\x63ollectedModelsCount\x18\x01 \x01(\x05\x12U\n\x06models\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelResult\"f\n\x13GeneratedColumnSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x66irst\x18\x03 \x01(\t\x12\x0e\n\x06second\x18\x04 \x01(\t\x12\x10\n\x08original\x18\x05 \x01(\t\"V\n\x17GroupSplitLocationsSpec\x12\x1d\n\x15groupTrainingDataFile\x18\x01 \x01(\t\x12\x1c\n\x14groupTestingDataFile\x18\x02 \x01(\t\"2\n\x13HyperParameterValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"o\n\x10HyperbandOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x14\n\x0cmaxResources\x18\x02 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"\'\n\x11ImagePipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\";\n\x15ImbalanceHandlingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\timbalance\x18\x02 \x01(\t\"\x9a\x02\n\x14InterpretabilitySpec\x12\x0b\n\x03ice\x18\x01 \x01(\x08\x12W\n\x08icepairs\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x0c\n\x04lime\x18\x03 \x01(\x08\x12\x0c\n\x04shap\x18\x04 \x01(\t\x12X\n\tshappairs\x18\x05 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x16\n\x0e\x63ounterfactual\x18\x06 \x01(\x08\x12\x0e\n\x06\x61nchor\x18\x07 \x01(\x08\"\xc6\x02\n\x16InterpretabilityStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x14\n\x0c\x65xplainerURI\x18\x03 \x01(\t\x12\x1a\n\x12trainShapValuesURI\x18\x04 \x01(\t\x12\x19\n\x11testShapValuesURI\x18\x05 \x01(\t\x12_\n\nimportance\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\"V\n\x05Level\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05index\x18\x02 \x03(\t\x12\x0f\n\x07horizon\x18\x03 \x01(\x05\x12\x0c\n\x04\x66req\x18\x04 \x01(\t\x12\x11\n\taggregate\x18\x05 \x01(\t\"k\n\x13MedianPrunerOptions\x12\x15\n\rstartupTrials\x18\x01 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x02 \x01(\x05\x12\x15\n\rintervalSteps\x18\x03 \x01(\x05\x12\x11\n\tminTrials\x18\x04 \x01(\x05\"\xf5\x01\n\x05Model\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStatus\"\x84\x02\n\nModelClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassStatus\"\xcd\x04\n\x12ModelClassDataSpec\x12[\n\x0cobservations\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12Z\n\x0bpredictions\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12L\n\x06schema\x18\x03 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latFile\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x12\n\nprimaryKey\x18\x05 \x03(\t\x12\x1c\n\x14predictionTimeColumn\x18\x06 \x01(\t\x12\x0e\n\x06target\x18\x07 \x01(\t\x12Q\n\x05tests\x18\x08 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x1e\n\x16onlineFeatureStoreName\x18\t \x01(\t\x12\x1f\n\x17offlineFeatureStoreName\x18\n \x01(\t\"\xa7\x01\n\x0eModelClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\"\x8d\x02\n\rModelClassRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Y\n\x04spec\x18\x02 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunSpec\x12]\n\x06status\x18\x03 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunStatus\"\xad\x01\n\x11ModelClassRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12V\n\x05items\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\"\xce\x01\n\x11ModelClassRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x03 \x01(\t\x12\x16\n\x0emodelClassName\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x0b\n\x03ttl\x18\t \x01(\x05\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\"\xed\x04\n\x13ModelClassRunStatus\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x11\n\tstudyName\x18\x02 \x01(\t\x12\x11\n\tmodelName\x18\x03 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x07 \x01(\x03\x12\x13\n\x0b\x65valMetrics\x18\x08 \x01(\t\x12\x15\n\rfailureReason\x18\t \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12=\n\tupdatedAt\x18\x0c \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\r \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12>\n\npromotedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04\x61uto\x18\x0f \x01(\x08\x12\x37\n\napprovedBy\x18\x10 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bmodelsCount\x18\x11 \x01(\x05\x12\x43\n\nconditions\x18\x12 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xd5\x02\n\x15ModelClassServingSpec\x12W\n\x08template\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\x12`\n\x12monitoringSchedule\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12`\n\x12predictionSchedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0e\n\x06preSQL\x18\x04 \x03(\t\x12\x0f\n\x07postSQL\x18\x05 \x03(\t\"\xc9\x06\n\x0eModelClassSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04task\x18\x04 \x01(\t\x12\x0f\n\x07subtask\x18\x05 \x01(\t\x12Y\n\tobjective\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12U\n\x08\x65ntities\x18\x07 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EntityRef\x12Z\n\x04\x64\x61ta\x18\x08 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassDataSpec\x12\x62\n\x08training\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassTrainingSpec\x12`\n\x07serving\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassServingSpec\x12_\n\x0cnotification\x18\x0b \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\x0ereportSchedule\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0c\n\x04\x66\x61st\x18\r \x01(\x08\x12\x0e\n\x06paused\x18\x0e \x01(\x08\x12\x12\n\nregistered\x18\x0f \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x10 \x01(\t\"\xfb\x08\n\x10ModelClassStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12j\n\x16trainingScheduleStatus\x18\x04 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12k\n\x17predictionSceduleStatus\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12k\n\x17monitoringSceduleStatus\x18\x06 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12g\n\x13reportSceduleStatus\x18\x07 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x16\n\x0e\x62\x65stModelScore\x18\x08 \x01(\x01\x12\x0f\n\x07retired\x18\t \x03(\t\x12\x15\n\rpredictorName\x18\n \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x0b \x01(\t\x12\x13\n\x0btriggeredBy\x18\x0c \x01(\t\x12\x15\n\rfailureReason\x18\r \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0e \x01(\t\x12=\n\tlastRunAt\x18\x0f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0blastRunName\x18\x10 \x01(\t\x12\x44\n\x10lastPredictionAt\x18\x11 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12lastPredictionName\x18\x12 \x01(\t\x12\x18\n\x10predictionsCount\x18\x13 \x01(\x05\x12\x11\n\trunsCount\x18\x14 \x01(\x05\x12\x13\n\x0bmodelsCount\x18\x15 \x01(\x05\x12\x0c\n\x04live\x18\x16 \x01(\x08\x12\x17\n\x0fpredictorsCount\x18\x17 \x01(\x05\x12\x43\n\nconditions\x18\x18 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xe5\x05\n\x16ModelClassTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x19\n\x11studyTemplateName\x18\x02 \x01(\t\x12Z\n\x0emodelUnitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12^\n\x10trainingSchedule\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\\\n\nmodelImage\x18\x05 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelImageSpec\x12g\n\x0bsearchSpace\x18\x08 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\x12\x0e\n\x06paused\x18\x0b \x01(\x08\x12\x0f\n\x07maxTime\x18\x0c \x01(\x05\x12\x11\n\tmaxModels\x18\r \x01(\x05\x12\x10\n\x08trainers\x18\x0e \x01(\x05\x12\x0f\n\x07\x61\x62orted\x18\x0f \x01(\x08\x12\x11\n\texplained\x18\x10 \x01(\x08\x12\x0e\n\x06preSQL\x18\x11 \x03(\t\x12\x0f\n\x07postSQL\x18\x12 \x03(\t\"\xb3\x01\n\x12ModelGroupByStatus\x12\x11\n\tmodelsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x14\n\x0c\x66orecastsURI\x18\x03 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"R\n\x0eModelImageSpec\x12\r\n\x05\x65xist\x18\x01 \x01(\x08\x12\x11\n\timageName\x18\x02 \x01(\t\x12\x1e\n\x16registryConnectionName\x18\x03 \x01(\t\"\x9d\x01\n\tModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"W\n\x0bModelResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03\x61lg\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x01\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x0f\n\x07trialID\x18\x05 \x01(\x05\"\xd9\x11\n\tModelSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x04 \x01(\t\x12\x11\n\tstudyName\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x06 \x01(\t\x12\x0c\n\x04task\x18\x07 \x01(\t\x12\x0f\n\x07subtask\x18\x08 \x01(\t\x12Y\n\tobjective\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12l\n\x12\x66\x65\x61tureEngineering\x18\n \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12\x63\n\testimator\x18\x0b \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12X\n\x03\x64nn\x18\x0c \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorSpec\x12_\n\x07\x63hatbot\x18\r \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ChatbotEstimatorSpec\x12`\n\x0cnlpEstimator\x18\x0e \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NLPEstimatorSpec\x12X\n\x08\x65nsemble\x18\x0f \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsembleSpec\x12X\n\x08training\x18\x10 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x0e\n\x06tested\x18\x12 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x13 \x01(\x08\x12\x10\n\x08packaged\x18\x14 \x01(\x08\x12\x11\n\tpublished\x18\x15 \x01(\x08\x12\x0e\n\x06pushed\x18\x16 \x01(\x08\x12\x10\n\x08reported\x18\x17 \x01(\x08\x12\x0e\n\x06paused\x18\x18 \x01(\x08\x12\x10\n\x08profiled\x18\x19 \x01(\x08\x12\x10\n\x08\x61rchived\x18\x1a \x01(\x08\x12\x12\n\nforecasted\x18\x1b \x01(\x08\x12\x0f\n\x07predict\x18\x1e \x01(\x08\x12\r\n\x05tuned\x18\x1f \x01(\x08\x12\x11\n\texplained\x18  \x01(\x08\x12\x15\n\rcodeGenerated\x18! \x01(\x08\x12\x10\n\x08\x62\x61seline\x18\" \x01(\x08\x12\x18\n\x10genDriftDetector\x18# \x01(\x08\x12\x0c\n\x04\x66\x61st\x18$ \x01(\x08\x12\x12\n\nunitTested\x18% \x01(\x08\x12?\n\x12\x66\x65\x65\x64\x62\x61\x63kDatasetRef\x18& \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07\x66lagged\x18\' \x01(\x08\x12W\n\x08location\x18( \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12]\n\x0b\x66orecasting\x18) \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12Z\n\x0b\x63ompilation\x18* \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CompilerSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18+ \x01(\x03\x12\x15\n\restimatorType\x18, \x01(\t\x12\x0b\n\x03ttl\x18- \x01(\x05\x12\x12\n\nmodelClass\x18. \x01(\t\x12\x0f\n\x07trialID\x18/ \x01(\x05\x12T\n\x08\x61pproval\x18\x30 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalSpec\x12h\n\x10interpretability\x18\x31 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12U\n\tunitTests\x18\x32 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12Y\n\rfeedbackTests\x18\x33 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12q\n\x12partitionLocations\x18\x34 \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PartitionModelLocationsSpec\x12\x16\n\x0emodelClassName\x18\x35 \x01(\t\x12\x19\n\x11modelClassRunName\x18\x36 \x01(\t\x12\x0c\n\x04role\x18\x37 \x01(\t\x12\x10\n\x08released\x18\x38 \x01(\x08\"\x93\x02\n\x10ModelStageStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12=\n\tstartedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05\x65rror\x18\n \x01(\t\"\xd7\"\n\x0bModelStatus\x12\x45\n\x11trainingStartedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12G\n\x13trainingCompletedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x44\n\x10testingStartedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x46\n\x12testingCompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x0ftuningStartedAt\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x45\n\x11tuningCompletedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0f\n\x07\x63vScore\x18\t \x01(\x01\x12\x15\n\rtrainingScore\x18\n \x01(\x01\x12\x11\n\ttestScore\x18\x0b \x01(\x01\x12\x0c\n\x04\x63ost\x18\x0c \x01(\x01\x12\x0c\n\x04\x62\x65st\x18\r \x01(\x08\x12P\n\x02\x63v\x18\x0e \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12S\n\x05train\x18\x0f \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04test\x18\x10 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04tune\x18\x11 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12V\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x12 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x43\n\x16lastFeedbackDatasetRef\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\r\n\x05phase\x18\x14 \x01(\t\x12\x12\n\nreportName\x18\x15 \x01(\t\x12\x11\n\treportURI\x18\x16 \x01(\t\x12\x13\n\x0bmanifestURI\x18\x17 \x01(\t\x12\x17\n\x0ftrainWeightsURI\x18\x18 \x01(\t\x12\x16\n\x0etestWeightsURI\x18\x19 \x01(\t\x12\x16\n\x0e\x66ullWeightsURI\x18\x1a \x01(\t\x12\x18\n\x10\x64riftDetectorURI\x18\x1b \x01(\t\x12\x1c\n\x14trainLabelEncoderURI\x18\x1c \x01(\t\x12\x1b\n\x13testLabelEncoderURI\x18\x1d \x01(\t\x12\x1b\n\x13\x66ullLabelEncoderURI\x18\x1e \x01(\t\x12\x0f\n\x07logsURI\x18\x1f \x01(\t\x12\x12\n\nprofileURI\x18  \x01(\t\x12\x1c\n\x14misclassificationURI\x18! \x01(\t\x12\x0e\n\x06tarURI\x18\" \x01(\t\x12\x0e\n\x06\x61ppURI\x18# \x01(\t\x12\x11\n\timageName\x18$ \x01(\t\x12g\n\x12impurityImportance\x18% \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12j\n\x15permutationImportance\x18& \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12\x13\n\x0b\x66orecastURI\x18\' \x01(\t\x12X\n\x07runtime\x18( \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus\x12\x63\n\x14trainDatasetLocation\x18) \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18* \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18+ \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18, \x01(\x03\x12\x14\n\x0ctrainingRows\x18- \x01(\x05\x12\x13\n\x0btestingRows\x18. \x01(\x05\x12\x16\n\x0evalidationRows\x18/ \x01(\x05\x12\x15\n\rfailureReason\x18\x30 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x31 \x01(\t\x12\x10\n\x08progress\x18\x32 \x01(\x05\x12\x13\n\x0bsizeInBytes\x18\x33 \x01(\x05\x12\x0f\n\x07latency\x18\x34 \x01(\x01\x12\x0b\n\x03url\x18\x35 \x01(\t\x12X\n\x07serving\x18\x36 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingStatus\x12>\n\nreleasedAt\x18\x37 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0bpredictedAt\x18\x38 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0btarFileHash\x18\x39 \x01(\t\x12\x11\n\timageHash\x18: \x01(\t\x12^\n\x10trainingDataHash\x18; \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12g\n\x11trainingResources\x18< \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x66\n\x10testingResources\x18= \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x11\n\ttrainedBy\x18> \x01(\t\x12\x0c\n\x04team\x18? \x01(\t\x12K\n\x04logs\x18\x41 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12V\n\x08rocCurve\x18\x42 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RocAucCurve\x12Q\n\x07prCurve\x18\x43 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PRCurve\x12\x66\n\x14trainConfusionMatrix\x18\x44 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x65\n\x13testConfusionMatrix\x18\x45 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x61\n\x16\x63orrelationsWithTarget\x18\x46 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18G \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12=\n\tupdatedAt\x18H \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12V\n\x08\x61pproval\x18I \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalStatus\x12j\n\x10interpretability\x18J \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilityStatus\x12O\n\x06images\x18K \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12\x61\n\x0funitTestsResult\x18L \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x65\n\x13\x66\x65\x65\x64\x62\x61\x63kTestsResult\x18M \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12]\n\x07groupby\x18N \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelGroupByStatus\x12Z\n\x06stages\x18O \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStageStatus\x12[\n\x05usage\x18P \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18Q \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdf\x01\n\x0eModelTestSuite\x12=\n\x10\x62\x61selineModelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\ndatasetRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\" \n\x10NLPEstimatorSpec\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\"/\n\x10NNLayerParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xcc\x01\n\x1bPartitionModelLocationsSpec\x12\x17\n\x0fpartitionFolder\x18\x01 \x01(\t\x12\x1e\n\x16partitionProfileFolder\x18\x02 \x01(\t\x12\x1b\n\x13partitionReportFile\x18\x03 \x01(\t\x12\x1c\n\x14partitionModelFolder\x18\x04 \x01(\t\x12\x1a\n\x12partitionModelFile\x18\x05 \x01(\t\x12\x1d\n\x15partitionForecastFile\x18\x06 \x01(\t\"\x84\x01\n\x17PercentilePrunerOptions\x12\x12\n\npercentile\x18\x01 \x01(\x05\x12\x15\n\rstartupTrials\x18\x02 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x16\n\x0eintervalTrials\x18\x04 \x01(\x05\x12\x11\n\tminTrials\x18\x05 \x01(\x05\"\x93\x04\n\nPrunerSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12]\n\x06median\x18\x02 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.MedianPrunerOptions\x12\x65\n\npercentile\x18\x03 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PercentilePrunerOptions\x12m\n\x11successiveHalving\x18\x04 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingOptions\x12]\n\thyperband\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperbandOptions\x12\x63\n\tthreshold\x18\x06 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ThresholdPrunerOptions\"\xd0\x01\n\x18RegressionForecasterSpec\x12\x10\n\x08\x65nsemble\x18\x01 \x01(\x08\x12\x12\n\nimputation\x18\x02 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x0f\n\x07scaling\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\x08\x12\x0f\n\x07windows\x18\x06 \x03(\x05\x12\x0c\n\x04lags\x18\x07 \x03(\x05\x12\x11\n\tfunctions\x18\x08 \x03(\t\x12\x0b\n\x03\x65ma\x18\t \x01(\x08\x12\x0b\n\x03log\x18\n \x01(\x08\x12\x11\n\treduction\x18\x0b \x01(\t\"\xf8\x01\n\x06Report\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportStatus\"\x8a\x01\n\x13ReportGroupByStatus\x12\x12\n\nreportsURI\x18\x01 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9f\x01\n\nReportList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xdb\x03\n\nReportSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x36\n\tentityRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12W\n\x08location\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x12\n\nreportType\x18\x06 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x07 \x01(\t\x12\x14\n\x0cnotifierName\x18\x08 \x01(\t\x12\r\n\x05owner\x18\t \x01(\t\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\x0b \x01(\x03\x12\x33\n\x06labRef\x18\x0c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0b\n\x03key\x18\r \x03(\t\x12\x16\n\x0emodelClassName\x18\x0e \x01(\t\x12\x19\n\x11modelClassRunName\x18\x0f \x01(\t\"\xe7\x03\n\x0cReportStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12^\n\x07groupby\x18\t \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportGroupByStatus\x12\x43\n\nconditions\x18\n \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf1\x01\n\rRuntimeStatus\x12\x15\n\rpythonVersion\x18\x01 \x01(\t\x12\x11\n\tpythonCmd\x18\x02 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12s\n\x0epythonPackages\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus.PythonPackagesEntry\x1a\x35\n\x13PythonPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x9e\x05\n\nSearchSpec\x12\x0f\n\x07sampler\x18\x01 \x01(\t\x12T\n\x06pruner\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PrunerSpec\x12\x0f\n\x07maxCost\x18\x03 \x01(\x05\x12\x0f\n\x07maxTime\x18\x04 \x01(\x05\x12\x11\n\tmaxModels\x18\x05 \x01(\x05\x12\x14\n\x0cminBestScore\x18\x06 \x01(\x01\x12\x10\n\x08trainers\x18\x07 \x01(\x05\x12\x0c\n\x04test\x18\x08 \x01(\x05\x12\x11\n\tretainTop\x18\t \x01(\x05\x12\x13\n\x0bretainedFor\x18\n \x01(\x05\x12g\n\x0bsearchSpace\x18\x0b \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\x12Y\n\tobjective\x18\x0e \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12Z\n\nobjective2\x18\x0f \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x0c\n\x04tune\x18\x10 \x01(\x08\x12\x0c\n\x04goal\x18\x11 \x01(\t\"L\n\x15SeasonalityPeriodSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x61uto\x18\x02 \x01(\x08\x12\x14\n\x0c\x66ourierOrder\x18\x03 \x01(\x05\"\x87\x04\n\x0fSeasonalitySpec\x12\x0c\n\x04\x61uto\x18\x01 \x01(\x08\x12_\n\x06yearly\x18\x02 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12\x62\n\tquarterly\x18\x03 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12`\n\x07monthly\x18\x04 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12_\n\x06weekly\x18\x05 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12^\n\x05\x64\x61ily\x18\x06 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\"<\n\x0bSegmentSpec\x12\x12\n\ncolumnName\x18\x01 \x01(\t\x12\n\n\x02op\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xb7\x03\n\x12ServingEnvironment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12;\n\x0eservingSiteRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12S\n\x06\x61\x63\x63\x65ss\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x05 \x01(\x05\x12\x0e\n\x06online\x18\x06 \x01(\x08\x12\x11\n\tdashboard\x18\x07 \x01(\x08\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0e\n\x06preSQL\x18\t \x03(\t\x12\x0f\n\x07postSQL\x18\n \x03(\t\"\xe2\x03\n\x0bServingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12X\n\tresources\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingSiteRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06online\x18\x07 \x01(\x08\x12\x11\n\tdashboard\x18\x08 \x01(\x08\x12S\n\x06\x61\x63\x63\x65ss\x18\t \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\n \x01(\x05\x12\x11\n\tpromotion\x18\x0c \x01(\t\x12\x37\n\napprovedBy\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"g\n\rServingStatus\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x03 \x01(\t\x12\x14\n\x0cpredictorURI\x18\x04 \x01(\t\x12\x14\n\x0c\x64\x61shboardURI\x18\x05 \x01(\t\"\xf5\x01\n\x05Study\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudySpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyStatus\"\x89\x01\n\x12StudyGroupByStatus\x12\x12\n\nstudiesURI\x18\x01 \x01(\t\x12_\n\rworkerResults\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\tStudyList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\xb4\x02\n\x10StudyPhaseStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12waitingModelsCount\x18\x03 \x01(\x05\x12\x1a\n\x12runningModelsCount\x18\x04 \x01(\x05\x12\x19\n\x11\x66\x61iledModelsCount\x18\x05 \x01(\x05\x12\x1c\n\x14\x63ompletedModelsCount\x18\x06 \x01(\x05\x12\x11\n\tbestScore\x18\x07 \x01(\x01\x12\x1c\n\x14modelsWithNoProgress\x18\x08 \x01(\x05\"a\n\x11StudyScheduleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12;\n\x07startAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xee\x10\n\tStudySpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x33\n\x06labRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x61tasetName\x18\x06 \x01(\t\x12\x0c\n\x04task\x18\x07 \x01(\t\x12\x0f\n\x07subtask\x18\x08 \x01(\t\x12h\n\x08\x66\x65Search\x18\t \x01(\x0b\x32V.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSearchSpec\x12i\n\x10imbalanceHandler\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImbalanceHandlingSpec\x12X\n\x08\x62\x61seline\x18\x0b \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.BaselineSpec\x12T\n\x06search\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SearchSpec\x12Z\n\tensembles\x18\r \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsemblesSpec\x12`\n\x10trainingTemplate\x18\x0e \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12]\n\x0b\x66\x63tTemplate\x18\x10 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12]\n\x08schedule\x18\x11 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyScheduleSpec\x12h\n\x10interpretability\x18\x12 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12`\n\x0e\x64riftDetection\x18\x13 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftModelSpec\x12\x0f\n\x07\x61\x62orted\x18\x14 \x01(\x08\x12\x10\n\x08reported\x18\x15 \x01(\x08\x12\x0e\n\x06paused\x18\x16 \x01(\x08\x12\x10\n\x08profiled\x18\x17 \x01(\x08\x12\x16\n\x0emodelPublished\x18\x18 \x01(\x08\x12\x18\n\x10modelImagePushed\x18\x19 \x01(\x08\x12\x16\n\x0emodelExplained\x18\x1a \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x1b \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x1c \x01(\t\x12\r\n\x05owner\x18\x1d \x01(\t\x12Z\n\x0b\x63ompilation\x18\x1e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CompilerSpec\x12\x10\n\x08template\x18\x1f \x01(\x08\x12\x0f\n\x07\x66lagged\x18  \x01(\x08\x12_\n\x0cnotification\x18! \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\nmodelImage\x18\" \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelImageSpec\x12[\n\x02gc\x18# \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionSpec\x12\x0b\n\x03ttl\x18$ \x01(\x05\x12\x14\n\x0cmodelVersion\x18% \x01(\t\x12\x0f\n\x07timeout\x18& \x01(\x05\x12\x15\n\rcodeGenerated\x18\' \x01(\x08\x12]\n\x11unitTestsTemplate\x18( \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12i\n\x0egroupLocations\x18) \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GroupSplitLocationsSpec\x12\x16\n\x0emodelClassName\x18* \x01(\t\x12\x19\n\x11modelClassRunName\x18+ \x01(\t\x12V\n\x07serving\x18, \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\"\xb0\x10\n\x0bStudyStatus\x12\x13\n\x0bmodelsCount\x18\x01 \x01(\x05\x12?\n\x0b\x63ompletedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x11\n\tbestModel\x18\x04 \x01(\t\x12\x16\n\x0e\x62\x65stModelScore\x18\x05 \x01(\x01\x12\x12\n\nprofileURI\x18\x06 \x01(\t\x12\x11\n\treportURI\x18\x07 \x01(\t\x12\x12\n\nreportName\x18\x08 \x01(\t\x12\r\n\x05phase\x18\t \x01(\t\x12\x1a\n\x12observedGeneration\x18\n \x01(\x03\x12\x63\n\x14trainDatasetLocation\x18\x0b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x13\n\x0blastModelID\x18\x0e \x01(\x03\x12\x15\n\rfailureReason\x18\x0f \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x10 \x01(\t\x12\x19\n\x11trainingRowsCount\x18\x11 \x01(\x05\x12\x18\n\x10testingRowsCount\x18\x12 \x01(\x05\x12\x1b\n\x13validationRowsCount\x18\x13 \x01(\x05\x12\x10\n\x08progress\x18\x14 \x01(\x05\x12^\n\x10trainingDataHash\x18\x16 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12\x13\n\x0btriggeredBy\x18\x17 \x01(\t\x12K\n\x04logs\x18\x18 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x66\n\x12\x66\x65\x61tureEngineering\x18\x19 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x62\x61seline\x18\x1a \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12Z\n\x06search\x18\x1b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x65nsemble\x18\x1c \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12X\n\x04test\x18\x1d \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12[\n\x07\x65xplain\x18\x1e \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\x65\n\x0e\x64riftDetection\x18\x1f \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftDetectorStatus\x12=\n\tupdatedAt\x18  \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18! \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12]\n\x02gc\x18\" \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionStatus\x12]\n\x07groupby\x18# \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyGroupByStatus\x12[\n\x05usage\x18$ \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18% \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x7f\n\x18SuccessiveHalvingOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x02 \x01(\x05\x12\x1c\n\x14minEarlyStoppingRate\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"h\n\x15SuccessiveHalvingSpec\x12\x0e\n\x06\x62udget\x18\x01 \x01(\x05\x12\x0f\n\x07\x62racket\x18\x02 \x01(\x05\x12\x0c\n\x04rung\x18\x03 \x01(\x05\x12\x0e\n\x06\x63onfID\x18\x04 \x01(\x05\x12\x10\n\x08modality\x18\x1a \x01(\t\"\xad\x01\n\x10TextPipelineSpec\x12\x0f\n\x07\x65ncoder\x18\x01 \x01(\t\x12\x11\n\ttokenizer\x18\x02 \x01(\t\x12\x11\n\tstopwords\x18\x03 \x01(\x08\x12\x0b\n\x03pos\x18\x04 \x01(\x08\x12\r\n\x05lemma\x18\x05 \x01(\x08\x12\x0c\n\x04stem\x18\x06 \x01(\x08\x12\x11\n\tembedding\x18\x07 \x01(\t\x12\x0b\n\x03svd\x18\x08 \x01(\x08\x12\x18\n\x10maxSvdComponents\x18\t \x01(\x05\"b\n\x16ThresholdPrunerOptions\x12\r\n\x05lower\x18\x01 \x01(\x01\x12\r\n\x05upper\x18\x02 \x01(\x01\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x15\n\rintervalSteps\x18\x04 \x01(\x05\"\x8a\x01\n\x0fTimeSeriesEvent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0f\n\x07holiday\x18\x03 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x10\n\x08preEvent\x18\x05 \x01(\x05\x12\x11\n\tpostEvent\x18\x06 \x01(\x05\x12\x12\n\ntimePoints\x18\x07 \x03(\t\"\x9c\x05\n\x0cTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08priority\x18\x02 \x01(\t\x12\x0e\n\x06\x63vtype\x18\x03 \x01(\t\x12\n\n\x02\x63V\x18\x04 \x01(\x08\x12\r\n\x05\x66olds\x18\x05 \x01(\x05\x12V\n\x05split\x18\x06 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataSplitSpec\x12\x13\n\x0b\x65valMetrics\x18\x07 \x03(\t\x12[\n\x02sh\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingSpec\x12\x0c\n\x04seed\x18\x0b \x01(\x01\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03gpu\x18\r \x01(\x08\x12\x13\n\x0b\x64istributed\x18\x0e \x01(\x08\x12\x19\n\x11\x66\x65\x61tureImportance\x18\x0f \x01(\x08\x12\x11\n\tnodeCount\x18\x10 \x01(\x05\x12\x11\n\tsamplePct\x18\x11 \x01(\x05\x12\\\n\ncheckpoint\x18\x12 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CheckpointSpec\x12\x10\n\x08logLevel\x18\x13 \x01(\t\x12\x15\n\rtimeoutInSecs\x18\x14 \x01(\x05\"\xdc\x01\n\x18UnivariateForecastStatus\x12\x1b\n\x13gridSearchResultURI\x18\x01 \x01(\t\x12g\n\rbaseEstimator\x18\x02 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x10\n\x08modelURI\x18\x03 \x01(\t\x12\x13\n\x0b\x63vResultURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x05 \x01(\t\"\'\n\x11VideoPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"=\n\nWindowSpec\x12\x10\n\x08interval\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x0e\n\x06length\x18\x03 \x01(\x05\x42:Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x12\x38github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x80\x01\n\x17\x41lgorithmParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12W\n\x06ranges\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\x9f\x01\n\x18\x41lgorithmSearchSpaceSpec\x12\x0f\n\x07include\x18\x01 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\x12\x61\n\x06\x63ustom\x18\x03 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmParameterRange\"`\n\x07\x41nomaly\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bvalueColumn\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x64jDeltaColumn\x18\x03 \x01(\t\x12\r\n\x05start\x18\x04 \x01(\t\x12\x0b\n\x03\x65nd\x18\x05 \x01(\t\"\'\n\x11\x41udioPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"M\n\x0c\x42\x61\x63ktestSpec\x12\x0f\n\x07sliding\x18\x01 \x01(\x08\x12\x0e\n\x06splits\x18\x02 \x01(\x05\x12\x0f\n\x07Initial\x18\x03 \x01(\x05\x12\x0b\n\x03gap\x18\x05 \x01(\x05\"?\n\x0c\x42\x61selineSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbaselines\x18\x02 \x03(\t\x12\x0b\n\x03\x61ll\x18\x03 \x01(\x08\"\r\n\x0b\x43hangePoint\"$\n\x14\x43hatbotEstimatorSpec\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\"\x96\x01\n\x0e\x43heckpointSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1a\n\x12\x63heckpointInterval\x18\x02 \x01(\x05\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x92\x01\n\x16\x43lassicalEstimatorSpec\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12\x61\n\nparameters\x18\x02 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperParameterValue\"a\n\x10\x43ustomReportSpec\x12M\n\x05pages\x18\x08 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"L\n\nDataHashes\x12\x11\n\ttrainHash\x18\x01 \x01(\t\x12\x13\n\x0btestingHash\x18\x02 \x01(\t\x12\x16\n\x0evalidationHash\x18\x03 \x01(\t\"\x84\x02\n\rDataSplitSpec\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\r\n\x05train\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x0c\n\x04test\x18\x04 \x01(\x05\x12\x13\n\x0bsplitColumn\x18\x05 \x01(\t\x12W\n\x08segments\x18\x06 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SegmentSpec\x12\x14\n\x0ctrainDataset\x18\x07 \x01(\t\x12\x13\n\x0btestDataset\x18\x08 \x01(\t\x12\x19\n\x11validationDataset\x18\t \x01(\t\"\xa5\x01\n\x12\x44\x65\x65pEstimatorLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12^\n\nparameters\x18\x03 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NNLayerParameter\x12\x13\n\x0binputLayers\x18\x04 \x03(\t\"\xe6\x01\n\x11\x44\x65\x65pEstimatorSpec\x12\\\n\x06layers\x18\x01 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorLayer\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x11\n\tbatchSize\x18\x03 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x04 \x01(\x05\x12\x17\n\x0fvalidationSplit\x18\x05 \x01(\x05\x12\r\n\x05isSeq\x18\x06 \x01(\x08\x12\x0c\n\x04gpus\x18\x07 \x01(\x05\x12\x0c\n\x04loss\x18\x08 \x01(\t\".\n\x13\x44riftDetectorStatus\x12\x17\n\x0foutlierModelURI\x18\x01 \x01(\t\";\n\x0e\x44riftModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10outlierAlgorithm\x18\x02 \x01(\t\"R\n\rEarlyStopSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07initial\x18\x02 \x01(\x05\x12\x1f\n\x17minModelsWithNoProgress\x18\x03 \x01(\x05\"\x0f\n\rEnsembleRules\"\xf3\x01\n\x0c\x45nsembleSpec\x12\x0e\n\x06models\x18\x01 \x03(\t\x12\x64\n\nestimators\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12_\n\x05\x66inal\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x0c\n\x04type\x18\x04 \x01(\t\"_\n\rEnsemblesSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0evotingEnsemble\x18\x02 \x01(\x08\x12\x18\n\x10stackingEnsemble\x18\x03 \x01(\x08\x12\x0b\n\x03top\x18\x04 \x01(\x05\"*\n\tEntityRef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\"\x89\x01\n\x0b\x45valMetrics\x12\x11\n\tselection\x18\x01 \x01(\t\x12\x11\n\treporting\x18\x02 \x03(\t\x12\x0f\n\x07\x61ggFunc\x18\x03 \x01(\t\x12\x11\n\taggPeriod\x18\x04 \x01(\x05\x12\x17\n\x0fnullModelParams\x18\x05 \x01(\t\x12\x17\n\x0frelErrTolerance\x18\x06 \x01(\x01\"\xe0\x01\n\nEvalPeriod\x12\x13\n\x0btestHorizon\x18\x01 \x01(\x05\x12\x1f\n\x17periodsBetweenTrainTest\x18\x02 \x01(\x05\x12\x1e\n\x16\x63vPeriodsBetweenSplits\x18\x03 \x01(\x05\x12\x1a\n\x12\x63vExpandingWindows\x18\x04 \x01(\x08\x12\x11\n\tcvHorizon\x18\x05 \x01(\x05\x12\x19\n\x11\x63vMinTrainPeriods\x18\x06 \x01(\x05\x12\x13\n\x0b\x63vMaxSplits\x18\x07 \x01(\x05\x12\x1d\n\x15\x63vUseMostRecentSplits\x18\x08 \x01(\x08\"\xc7\x06\n\x1a\x46\x65\x61tureEngineeringPipeline\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\x12\x12\n\nimputation\x18\x04 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x05 \x01(\t\x12\x0f\n\x07scaling\x18\x06 \x01(\t\x12\x16\n\x0e\x64iscretisation\x18\x07 \x01(\t\x12\x1e\n\x16variableTransformation\x18\x08 \x01(\t\x12\x17\n\x0foutlierHandling\x18\t \x01(\t\x12\x1e\n\x16\x64\x61tetimeTransformation\x18\n \x01(\t\x12X\n\x04text\x18\x0b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TextPipelineSpec\x12Z\n\x05image\x18\x0c \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImagePipelineSpec\x12Z\n\x05\x61udio\x18\r \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AudioPipelineSpec\x12Z\n\x05video\x18\x0e \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.VideoPipelineSpec\x12`\n\tgenerated\x18\x10 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GeneratedColumnSpec\x12]\n\x06\x63ustom\x18\x11 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GeneratedColumnSpec\x12\x0c\n\x04\x64rop\x18\x12 \x01(\x08\x12\x13\n\x0bpassthrough\x18\x13 \x01(\x08\"\x8d\x03\n\x1c\x46\x65\x61tureEngineeringSearchSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x19\n\x11imbalancedHandler\x18\x02 \x01(\t\x12\x11\n\testimator\x18\x03 \x01(\t\x12\x11\n\tmaxModels\x18\x04 \x01(\x05\x12\x0f\n\x07maxTime\x18\x05 \x01(\x05\x12\x13\n\x0bmaxTrainers\x18\x06 \x01(\x05\x12\x11\n\tsamplePct\x18\x07 \x01(\x05\x12\x12\n\nautoRemove\x18\x08 \x01(\x08\x12\r\n\x05reuse\x18\t \x01(\x08\x12\x63\n\x0b\x66\x65Selection\x18\n \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\"\x80\x01\n\x1e\x46\x65\x61tureEngineeringSearchStatus\x12^\n\x04\x62\x65st\x18\x01 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\"\xf7\x01\n\x16\x46\x65\x61tureEngineeringSpec\x12g\n\tpipelines\x18\x01 \x03(\x0b\x32T.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringPipeline\x12\x11\n\timbalance\x18\x02 \x01(\t\x12\x61\n\tselection\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\"8\n\x11\x46\x65\x61tureImportance\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nimportance\x18\x02 \x01(\x01\":\n\x0b\x46\x65\x61tureInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\"#\n\x0b\x46\x65\x61turePair\x12\t\n\x01x\x18\x01 \x01(\t\x12\t\n\x01y\x18\x02 \x01(\t\"\xd5\x01\n\x14\x46\x65\x61tureSelectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tembedding\x18\x03 \x01(\x08\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\x08\x12\x0f\n\x07wrapper\x18\x05 \x01(\x08\x12\x10\n\x08pipeline\x18\x06 \x03(\t\x12\x14\n\x0cvarThreshold\x18\x07 \x01(\x05\x12\x15\n\rcorrThreshold\x18\x08 \x01(\x05\x12\x13\n\x0bmaxFeatures\x18\t \x01(\x05\x12\x12\n\npercentile\x18\n \x01(\x05\x12\x10\n\x08reserved\x18\x0c \x03(\t\"\xf8\x07\n\x0e\x46orecasterSpec\x12Y\n\x06\x65vents\x18\x02 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TimeSeriesEvent\x12R\n\x04past\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12T\n\x06\x66uture\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12\x10\n\x08\x63overage\x18\x06 \x01(\x01\x12]\n\x0eoutputLocation\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x10\n\x08\x66\x65\x61tures\x18\x08 \x03(\t\x12\x0e\n\x06groups\x18\t \x03(\t\x12\x1a\n\x12predefinedTemplate\x18\n \x01(\t\x12T\n\tanomalies\x18\x0b \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Anomaly\x12\x14\n\x0ctrainEndData\x18\x0c \x01(\t\x12\x13\n\x0bvalueColumn\x18\r \x01(\t\x12\x11\n\thpoBudget\x18\x0e \x01(\x05\x12`\n\x11\x65valuationMetrics\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalMetrics\x12^\n\x10\x65valuationPeriod\x18\x10 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalPeriod\x12^\n\x0bseasonality\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalitySpec\x12\x12\n\nregressors\x18\x12 \x03(\t\x12\x18\n\x10laggedRegressors\x18\x13 \x03(\t\x12\x0e\n\x06growth\x18\x14 \x01(\t\x12\x0b\n\x03key\x18\x15 \x03(\t\x12\x12\n\nestimators\x18\x16 \x03(\t\x12\x0b\n\x03hts\x18\x17 \x01(\t\"x\n\x15GarbageCollectionSpec\x12\x1e\n\x16\x63ollectAtModelClassEnd\x18\x01 \x01(\x08\x12%\n\x1dkeepOnlyBestModelPerAlgorithm\x18\x02 \x01(\x08\x12\x18\n\x10keepPrunedModels\x18\x03 \x01(\x08\"\x8e\x01\n\x17GarbageCollectionStatus\x12\x1c\n\x14\x63ollectedModelsCount\x18\x01 \x01(\x05\x12U\n\x06models\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelResult\"f\n\x13GeneratedColumnSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x66irst\x18\x03 \x01(\t\x12\x0e\n\x06second\x18\x04 \x01(\t\x12\x10\n\x08original\x18\x05 \x01(\t\"V\n\x17GroupSplitLocationsSpec\x12\x1d\n\x15groupTrainingDataFile\x18\x01 \x01(\t\x12\x1c\n\x14groupTestingDataFile\x18\x02 \x01(\t\"2\n\x13HyperParameterValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"o\n\x10HyperbandOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x14\n\x0cmaxResources\x18\x02 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"\'\n\x11ImagePipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\";\n\x15ImbalanceHandlingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\timbalance\x18\x02 \x01(\t\"\x9a\x02\n\x14InterpretabilitySpec\x12\x0b\n\x03ice\x18\x01 \x01(\x08\x12W\n\x08icepairs\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x0c\n\x04lime\x18\x03 \x01(\x08\x12\x0c\n\x04shap\x18\x04 \x01(\t\x12X\n\tshappairs\x18\x05 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x16\n\x0e\x63ounterfactual\x18\x06 \x01(\x08\x12\x0e\n\x06\x61nchor\x18\x07 \x01(\x08\"\xc6\x02\n\x16InterpretabilityStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x14\n\x0c\x65xplainerURI\x18\x03 \x01(\t\x12\x1a\n\x12trainShapValuesURI\x18\x04 \x01(\t\x12\x19\n\x11testShapValuesURI\x18\x05 \x01(\t\x12_\n\nimportance\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\"V\n\x05Level\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05index\x18\x02 \x03(\t\x12\x0f\n\x07horizon\x18\x03 \x01(\x05\x12\x0c\n\x04\x66req\x18\x04 \x01(\t\x12\x11\n\taggregate\x18\x05 \x01(\t\"k\n\x13MedianPrunerOptions\x12\x15\n\rstartupTrials\x18\x01 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x02 \x01(\x05\x12\x15\n\rintervalSteps\x18\x03 \x01(\x05\x12\x11\n\tminTrials\x18\x04 \x01(\x05\"\xf5\x01\n\x05Model\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStatus\"\x84\x02\n\nModelClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassStatus\"\xcd\x04\n\x12ModelClassDataSpec\x12[\n\x0cobservations\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12Z\n\x0bpredictions\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12L\n\x06schema\x18\x03 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latFile\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x12\n\nprimaryKey\x18\x05 \x03(\t\x12\x1c\n\x14predictionTimeColumn\x18\x06 \x01(\t\x12\x0e\n\x06target\x18\x07 \x01(\t\x12Q\n\x05tests\x18\x08 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x1e\n\x16onlineFeatureStoreName\x18\t \x01(\t\x12\x1f\n\x17offlineFeatureStoreName\x18\n \x01(\t\"\xa7\x01\n\x0eModelClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\"\x8d\x02\n\rModelClassRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Y\n\x04spec\x18\x02 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunSpec\x12]\n\x06status\x18\x03 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunStatus\"\xad\x01\n\x11ModelClassRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12V\n\x05items\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\"\xce\x01\n\x11ModelClassRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x03 \x01(\t\x12\x16\n\x0emodelClassName\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x0b\n\x03ttl\x18\t \x01(\x05\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\"\xed\x04\n\x13ModelClassRunStatus\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x11\n\tstudyName\x18\x02 \x01(\t\x12\x11\n\tmodelName\x18\x03 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x07 \x01(\x03\x12\x13\n\x0b\x65valMetrics\x18\x08 \x01(\t\x12\x15\n\rfailureReason\x18\t \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12=\n\tupdatedAt\x18\x0c \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\r \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12>\n\npromotedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04\x61uto\x18\x0f \x01(\x08\x12\x37\n\napprovedBy\x18\x10 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bmodelsCount\x18\x11 \x01(\x05\x12\x43\n\nconditions\x18\x12 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xd5\x02\n\x15ModelClassServingSpec\x12W\n\x08template\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\x12`\n\x12monitoringSchedule\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12`\n\x12predictionSchedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0e\n\x06preSQL\x18\x04 \x03(\t\x12\x0f\n\x07postSQL\x18\x05 \x03(\t\"\xc9\x06\n\x0eModelClassSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04task\x18\x04 \x01(\t\x12\x0f\n\x07subtask\x18\x05 \x01(\t\x12Y\n\tobjective\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12U\n\x08\x65ntities\x18\x07 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EntityRef\x12Z\n\x04\x64\x61ta\x18\x08 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassDataSpec\x12\x62\n\x08training\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassTrainingSpec\x12`\n\x07serving\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassServingSpec\x12_\n\x0cnotification\x18\x0b \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\x0ereportSchedule\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0c\n\x04\x66\x61st\x18\r \x01(\x08\x12\x0e\n\x06paused\x18\x0e \x01(\x08\x12\x12\n\nregistered\x18\x0f \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x10 \x01(\t\"\xfb\x08\n\x10ModelClassStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12j\n\x16trainingScheduleStatus\x18\x04 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12k\n\x17predictionSceduleStatus\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12k\n\x17monitoringSceduleStatus\x18\x06 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12g\n\x13reportSceduleStatus\x18\x07 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x16\n\x0e\x62\x65stModelScore\x18\x08 \x01(\x01\x12\x0f\n\x07retired\x18\t \x03(\t\x12\x15\n\rpredictorName\x18\n \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x0b \x01(\t\x12\x13\n\x0btriggeredBy\x18\x0c \x01(\t\x12\x15\n\rfailureReason\x18\r \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0e \x01(\t\x12=\n\tlastRunAt\x18\x0f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0blastRunName\x18\x10 \x01(\t\x12\x44\n\x10lastPredictionAt\x18\x11 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12lastPredictionName\x18\x12 \x01(\t\x12\x18\n\x10predictionsCount\x18\x13 \x01(\x05\x12\x11\n\trunsCount\x18\x14 \x01(\x05\x12\x13\n\x0bmodelsCount\x18\x15 \x01(\x05\x12\x0c\n\x04live\x18\x16 \x01(\x08\x12\x17\n\x0fpredictorsCount\x18\x17 \x01(\x05\x12\x43\n\nconditions\x18\x18 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xe5\x05\n\x16ModelClassTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x19\n\x11studyTemplateName\x18\x02 \x01(\t\x12Z\n\x0emodelUnitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12^\n\x10trainingSchedule\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\\\n\nmodelImage\x18\x05 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelImageSpec\x12g\n\x0bsearchSpace\x18\x08 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\x12\x0e\n\x06paused\x18\x0b \x01(\x08\x12\x0f\n\x07maxTime\x18\x0c \x01(\x05\x12\x11\n\tmaxModels\x18\r \x01(\x05\x12\x10\n\x08trainers\x18\x0e \x01(\x05\x12\x0f\n\x07\x61\x62orted\x18\x0f \x01(\x08\x12\x11\n\texplained\x18\x10 \x01(\x08\x12\x0e\n\x06preSQL\x18\x11 \x03(\t\x12\x0f\n\x07postSQL\x18\x12 \x03(\t\"\xb3\x01\n\x12ModelGroupByStatus\x12\x11\n\tmodelsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x14\n\x0c\x66orecastsURI\x18\x03 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"R\n\x0eModelImageSpec\x12\r\n\x05\x65xist\x18\x01 \x01(\x08\x12\x11\n\timageName\x18\x02 \x01(\t\x12\x1e\n\x16registryConnectionName\x18\x03 \x01(\t\"\x9d\x01\n\tModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"W\n\x0bModelResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03\x61lg\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x01\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x0f\n\x07trialID\x18\x05 \x01(\x05\"\xd9\x11\n\tModelSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x04 \x01(\t\x12\x11\n\tstudyName\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x06 \x01(\t\x12\x0c\n\x04task\x18\x07 \x01(\t\x12\x0f\n\x07subtask\x18\x08 \x01(\t\x12Y\n\tobjective\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12l\n\x12\x66\x65\x61tureEngineering\x18\n \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12\x63\n\testimator\x18\x0b \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12X\n\x03\x64nn\x18\x0c \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorSpec\x12_\n\x07\x63hatbot\x18\r \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ChatbotEstimatorSpec\x12`\n\x0cnlpEstimator\x18\x0e \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NLPEstimatorSpec\x12X\n\x08\x65nsemble\x18\x0f \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsembleSpec\x12X\n\x08training\x18\x10 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x0e\n\x06tested\x18\x12 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x13 \x01(\x08\x12\x10\n\x08packaged\x18\x14 \x01(\x08\x12\x11\n\tpublished\x18\x15 \x01(\x08\x12\x0e\n\x06pushed\x18\x16 \x01(\x08\x12\x10\n\x08reported\x18\x17 \x01(\x08\x12\x0e\n\x06paused\x18\x18 \x01(\x08\x12\x10\n\x08profiled\x18\x19 \x01(\x08\x12\x10\n\x08\x61rchived\x18\x1a \x01(\x08\x12\x12\n\nforecasted\x18\x1b \x01(\x08\x12\x0f\n\x07predict\x18\x1e \x01(\x08\x12\r\n\x05tuned\x18\x1f \x01(\x08\x12\x11\n\texplained\x18  \x01(\x08\x12\x15\n\rcodeGenerated\x18! \x01(\x08\x12\x10\n\x08\x62\x61seline\x18\" \x01(\x08\x12\x18\n\x10genDriftDetector\x18# \x01(\x08\x12\x0c\n\x04\x66\x61st\x18$ \x01(\x08\x12\x12\n\nunitTested\x18% \x01(\x08\x12?\n\x12\x66\x65\x65\x64\x62\x61\x63kDatasetRef\x18& \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07\x66lagged\x18\' \x01(\x08\x12W\n\x08location\x18( \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12]\n\x0b\x66orecasting\x18) \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12Z\n\x0b\x63ompilation\x18* \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CompilerSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18+ \x01(\x03\x12\x15\n\restimatorType\x18, \x01(\t\x12\x0b\n\x03ttl\x18- \x01(\x05\x12\x12\n\nmodelClass\x18. \x01(\t\x12\x0f\n\x07trialID\x18/ \x01(\x05\x12T\n\x08\x61pproval\x18\x30 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalSpec\x12h\n\x10interpretability\x18\x31 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12U\n\tunitTests\x18\x32 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12Y\n\rfeedbackTests\x18\x33 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12q\n\x12partitionLocations\x18\x34 \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PartitionModelLocationsSpec\x12\x16\n\x0emodelClassName\x18\x35 \x01(\t\x12\x19\n\x11modelClassRunName\x18\x36 \x01(\t\x12\x0c\n\x04role\x18\x37 \x01(\t\x12\x10\n\x08released\x18\x38 \x01(\x08\"\x93\x02\n\x10ModelStageStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12=\n\tstartedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05\x65rror\x18\n \x01(\t\"\xd7\"\n\x0bModelStatus\x12\x45\n\x11trainingStartedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12G\n\x13trainingCompletedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x44\n\x10testingStartedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x46\n\x12testingCompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x0ftuningStartedAt\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x45\n\x11tuningCompletedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0f\n\x07\x63vScore\x18\t \x01(\x01\x12\x15\n\rtrainingScore\x18\n \x01(\x01\x12\x11\n\ttestScore\x18\x0b \x01(\x01\x12\x0c\n\x04\x63ost\x18\x0c \x01(\x01\x12\x0c\n\x04\x62\x65st\x18\r \x01(\x08\x12P\n\x02\x63v\x18\x0e \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12S\n\x05train\x18\x0f \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04test\x18\x10 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04tune\x18\x11 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12V\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x12 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x43\n\x16lastFeedbackDatasetRef\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\r\n\x05phase\x18\x14 \x01(\t\x12\x12\n\nreportName\x18\x15 \x01(\t\x12\x11\n\treportURI\x18\x16 \x01(\t\x12\x13\n\x0bmanifestURI\x18\x17 \x01(\t\x12\x17\n\x0ftrainWeightsURI\x18\x18 \x01(\t\x12\x16\n\x0etestWeightsURI\x18\x19 \x01(\t\x12\x16\n\x0e\x66ullWeightsURI\x18\x1a \x01(\t\x12\x18\n\x10\x64riftDetectorURI\x18\x1b \x01(\t\x12\x1c\n\x14trainLabelEncoderURI\x18\x1c \x01(\t\x12\x1b\n\x13testLabelEncoderURI\x18\x1d \x01(\t\x12\x1b\n\x13\x66ullLabelEncoderURI\x18\x1e \x01(\t\x12\x0f\n\x07logsURI\x18\x1f \x01(\t\x12\x12\n\nprofileURI\x18  \x01(\t\x12\x1c\n\x14misclassificationURI\x18! \x01(\t\x12\x0e\n\x06tarURI\x18\" \x01(\t\x12\x0e\n\x06\x61ppURI\x18# \x01(\t\x12\x11\n\timageName\x18$ \x01(\t\x12g\n\x12impurityImportance\x18% \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12j\n\x15permutationImportance\x18& \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12\x13\n\x0b\x66orecastURI\x18\' \x01(\t\x12X\n\x07runtime\x18( \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus\x12\x63\n\x14trainDatasetLocation\x18) \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18* \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18+ \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18, \x01(\x03\x12\x14\n\x0ctrainingRows\x18- \x01(\x05\x12\x13\n\x0btestingRows\x18. \x01(\x05\x12\x16\n\x0evalidationRows\x18/ \x01(\x05\x12\x15\n\rfailureReason\x18\x30 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x31 \x01(\t\x12\x10\n\x08progress\x18\x32 \x01(\x05\x12\x13\n\x0bsizeInBytes\x18\x33 \x01(\x05\x12\x0f\n\x07latency\x18\x34 \x01(\x01\x12\x0b\n\x03url\x18\x35 \x01(\t\x12X\n\x07serving\x18\x36 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingStatus\x12>\n\nreleasedAt\x18\x37 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0bpredictedAt\x18\x38 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0btarFileHash\x18\x39 \x01(\t\x12\x11\n\timageHash\x18: \x01(\t\x12^\n\x10trainingDataHash\x18; \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12g\n\x11trainingResources\x18< \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x66\n\x10testingResources\x18= \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x11\n\ttrainedBy\x18> \x01(\t\x12\x0c\n\x04team\x18? \x01(\t\x12K\n\x04logs\x18\x41 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12V\n\x08rocCurve\x18\x42 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RocAucCurve\x12Q\n\x07prCurve\x18\x43 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PRCurve\x12\x66\n\x14trainConfusionMatrix\x18\x44 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x65\n\x13testConfusionMatrix\x18\x45 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x61\n\x16\x63orrelationsWithTarget\x18\x46 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18G \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12=\n\tupdatedAt\x18H \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12V\n\x08\x61pproval\x18I \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalStatus\x12j\n\x10interpretability\x18J \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilityStatus\x12O\n\x06images\x18K \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12\x61\n\x0funitTestsResult\x18L \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x65\n\x13\x66\x65\x65\x64\x62\x61\x63kTestsResult\x18M \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12]\n\x07groupby\x18N \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelGroupByStatus\x12Z\n\x06stages\x18O \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStageStatus\x12[\n\x05usage\x18P \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18Q \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdf\x01\n\x0eModelTestSuite\x12=\n\x10\x62\x61selineModelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\ndatasetRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\" \n\x10NLPEstimatorSpec\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\"/\n\x10NNLayerParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xcc\x01\n\x1bPartitionModelLocationsSpec\x12\x17\n\x0fpartitionFolder\x18\x01 \x01(\t\x12\x1e\n\x16partitionProfileFolder\x18\x02 \x01(\t\x12\x1b\n\x13partitionReportFile\x18\x03 \x01(\t\x12\x1c\n\x14partitionModelFolder\x18\x04 \x01(\t\x12\x1a\n\x12partitionModelFile\x18\x05 \x01(\t\x12\x1d\n\x15partitionForecastFile\x18\x06 \x01(\t\"\x84\x01\n\x17PercentilePrunerOptions\x12\x12\n\npercentile\x18\x01 \x01(\x05\x12\x15\n\rstartupTrials\x18\x02 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x16\n\x0eintervalTrials\x18\x04 \x01(\x05\x12\x11\n\tminTrials\x18\x05 \x01(\x05\"\x93\x04\n\nPrunerSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12]\n\x06median\x18\x02 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.MedianPrunerOptions\x12\x65\n\npercentile\x18\x03 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PercentilePrunerOptions\x12m\n\x11successiveHalving\x18\x04 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingOptions\x12]\n\thyperband\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperbandOptions\x12\x63\n\tthreshold\x18\x06 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ThresholdPrunerOptions\"\xd0\x01\n\x18RegressionForecasterSpec\x12\x10\n\x08\x65nsemble\x18\x01 \x01(\x08\x12\x12\n\nimputation\x18\x02 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x0f\n\x07scaling\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\x08\x12\x0f\n\x07windows\x18\x06 \x03(\x05\x12\x0c\n\x04lags\x18\x07 \x03(\x05\x12\x11\n\tfunctions\x18\x08 \x03(\t\x12\x0b\n\x03\x65ma\x18\t \x01(\x08\x12\x0b\n\x03log\x18\n \x01(\x08\x12\x11\n\treduction\x18\x0b \x01(\t\"\xf8\x01\n\x06Report\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportStatus\"\x8a\x01\n\x13ReportGroupByStatus\x12\x12\n\nreportsURI\x18\x01 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9f\x01\n\nReportList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\x9e\x03\n\nReportSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x36\n\tentityRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x12\n\nreportType\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12\x14\n\x0cnotifierName\x18\x05 \x01(\t\x12\r\n\x05owner\x18\x06 \x01(\t\x12X\n\tresources\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\x08 \x01(\x03\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0b\n\x03key\x18\n \x03(\t\x12\x1a\n\x12\x61rtifactBucketName\x18\x0b \x01(\t\x12\x16\n\x0emodelClassName\x18\x0c \x01(\t\x12\x19\n\x11modelClassRunName\x18\r \x01(\t\"\xb3\x04\n\x0cReportStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12^\n\x07groupby\x18\t \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportGroupByStatus\x12\x43\n\nconditions\x18\n \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf1\x01\n\rRuntimeStatus\x12\x15\n\rpythonVersion\x18\x01 \x01(\t\x12\x11\n\tpythonCmd\x18\x02 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12s\n\x0epythonPackages\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus.PythonPackagesEntry\x1a\x35\n\x13PythonPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x9e\x05\n\nSearchSpec\x12\x0f\n\x07sampler\x18\x01 \x01(\t\x12T\n\x06pruner\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PrunerSpec\x12\x0f\n\x07maxCost\x18\x03 \x01(\x05\x12\x0f\n\x07maxTime\x18\x04 \x01(\x05\x12\x11\n\tmaxModels\x18\x05 \x01(\x05\x12\x14\n\x0cminBestScore\x18\x06 \x01(\x01\x12\x10\n\x08trainers\x18\x07 \x01(\x05\x12\x0c\n\x04test\x18\x08 \x01(\x05\x12\x11\n\tretainTop\x18\t \x01(\x05\x12\x13\n\x0bretainedFor\x18\n \x01(\x05\x12g\n\x0bsearchSpace\x18\x0b \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\x12Y\n\tobjective\x18\x0e \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12Z\n\nobjective2\x18\x0f \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x0c\n\x04tune\x18\x10 \x01(\x08\x12\x0c\n\x04goal\x18\x11 \x01(\t\"L\n\x15SeasonalityPeriodSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x61uto\x18\x02 \x01(\x08\x12\x14\n\x0c\x66ourierOrder\x18\x03 \x01(\x05\"\x87\x04\n\x0fSeasonalitySpec\x12\x0c\n\x04\x61uto\x18\x01 \x01(\x08\x12_\n\x06yearly\x18\x02 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12\x62\n\tquarterly\x18\x03 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12`\n\x07monthly\x18\x04 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12_\n\x06weekly\x18\x05 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12^\n\x05\x64\x61ily\x18\x06 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\"<\n\x0bSegmentSpec\x12\x12\n\ncolumnName\x18\x01 \x01(\t\x12\n\n\x02op\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xb7\x03\n\x12ServingEnvironment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12;\n\x0eservingSiteRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12S\n\x06\x61\x63\x63\x65ss\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x05 \x01(\x05\x12\x0e\n\x06online\x18\x06 \x01(\x08\x12\x11\n\tdashboard\x18\x07 \x01(\x08\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0e\n\x06preSQL\x18\t \x03(\t\x12\x0f\n\x07postSQL\x18\n \x03(\t\"\xe2\x03\n\x0bServingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12X\n\tresources\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingSiteRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06online\x18\x07 \x01(\x08\x12\x11\n\tdashboard\x18\x08 \x01(\x08\x12S\n\x06\x61\x63\x63\x65ss\x18\t \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\n \x01(\x05\x12\x11\n\tpromotion\x18\x0c \x01(\t\x12\x37\n\napprovedBy\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"g\n\rServingStatus\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x03 \x01(\t\x12\x14\n\x0cpredictorURI\x18\x04 \x01(\t\x12\x14\n\x0c\x64\x61shboardURI\x18\x05 \x01(\t\"\xf5\x01\n\x05Study\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudySpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyStatus\"\x89\x01\n\x12StudyGroupByStatus\x12\x12\n\nstudiesURI\x18\x01 \x01(\t\x12_\n\rworkerResults\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\tStudyList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\xb4\x02\n\x10StudyPhaseStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12waitingModelsCount\x18\x03 \x01(\x05\x12\x1a\n\x12runningModelsCount\x18\x04 \x01(\x05\x12\x19\n\x11\x66\x61iledModelsCount\x18\x05 \x01(\x05\x12\x1c\n\x14\x63ompletedModelsCount\x18\x06 \x01(\x05\x12\x11\n\tbestScore\x18\x07 \x01(\x01\x12\x1c\n\x14modelsWithNoProgress\x18\x08 \x01(\x05\"a\n\x11StudyScheduleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12;\n\x07startAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xee\x10\n\tStudySpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x33\n\x06labRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x61tasetName\x18\x06 \x01(\t\x12\x0c\n\x04task\x18\x07 \x01(\t\x12\x0f\n\x07subtask\x18\x08 \x01(\t\x12h\n\x08\x66\x65Search\x18\t \x01(\x0b\x32V.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSearchSpec\x12i\n\x10imbalanceHandler\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImbalanceHandlingSpec\x12X\n\x08\x62\x61seline\x18\x0b \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.BaselineSpec\x12T\n\x06search\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SearchSpec\x12Z\n\tensembles\x18\r \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsemblesSpec\x12`\n\x10trainingTemplate\x18\x0e \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12]\n\x0b\x66\x63tTemplate\x18\x10 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12]\n\x08schedule\x18\x11 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyScheduleSpec\x12h\n\x10interpretability\x18\x12 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12`\n\x0e\x64riftDetection\x18\x13 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftModelSpec\x12\x0f\n\x07\x61\x62orted\x18\x14 \x01(\x08\x12\x10\n\x08reported\x18\x15 \x01(\x08\x12\x0e\n\x06paused\x18\x16 \x01(\x08\x12\x10\n\x08profiled\x18\x17 \x01(\x08\x12\x16\n\x0emodelPublished\x18\x18 \x01(\x08\x12\x18\n\x10modelImagePushed\x18\x19 \x01(\x08\x12\x16\n\x0emodelExplained\x18\x1a \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x1b \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x1c \x01(\t\x12\r\n\x05owner\x18\x1d \x01(\t\x12Z\n\x0b\x63ompilation\x18\x1e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CompilerSpec\x12\x10\n\x08template\x18\x1f \x01(\x08\x12\x0f\n\x07\x66lagged\x18  \x01(\x08\x12_\n\x0cnotification\x18! \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\nmodelImage\x18\" \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelImageSpec\x12[\n\x02gc\x18# \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionSpec\x12\x0b\n\x03ttl\x18$ \x01(\x05\x12\x14\n\x0cmodelVersion\x18% \x01(\t\x12\x0f\n\x07timeout\x18& \x01(\x05\x12\x15\n\rcodeGenerated\x18\' \x01(\x08\x12]\n\x11unitTestsTemplate\x18( \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12i\n\x0egroupLocations\x18) \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GroupSplitLocationsSpec\x12\x16\n\x0emodelClassName\x18* \x01(\t\x12\x19\n\x11modelClassRunName\x18+ \x01(\t\x12V\n\x07serving\x18, \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\"\xb0\x10\n\x0bStudyStatus\x12\x13\n\x0bmodelsCount\x18\x01 \x01(\x05\x12?\n\x0b\x63ompletedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x11\n\tbestModel\x18\x04 \x01(\t\x12\x16\n\x0e\x62\x65stModelScore\x18\x05 \x01(\x01\x12\x12\n\nprofileURI\x18\x06 \x01(\t\x12\x11\n\treportURI\x18\x07 \x01(\t\x12\x12\n\nreportName\x18\x08 \x01(\t\x12\r\n\x05phase\x18\t \x01(\t\x12\x1a\n\x12observedGeneration\x18\n \x01(\x03\x12\x63\n\x14trainDatasetLocation\x18\x0b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x13\n\x0blastModelID\x18\x0e \x01(\x03\x12\x15\n\rfailureReason\x18\x0f \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x10 \x01(\t\x12\x19\n\x11trainingRowsCount\x18\x11 \x01(\x05\x12\x18\n\x10testingRowsCount\x18\x12 \x01(\x05\x12\x1b\n\x13validationRowsCount\x18\x13 \x01(\x05\x12\x10\n\x08progress\x18\x14 \x01(\x05\x12^\n\x10trainingDataHash\x18\x16 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12\x13\n\x0btriggeredBy\x18\x17 \x01(\t\x12K\n\x04logs\x18\x18 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x66\n\x12\x66\x65\x61tureEngineering\x18\x19 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x62\x61seline\x18\x1a \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12Z\n\x06search\x18\x1b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x65nsemble\x18\x1c \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12X\n\x04test\x18\x1d \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12[\n\x07\x65xplain\x18\x1e \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\x65\n\x0e\x64riftDetection\x18\x1f \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftDetectorStatus\x12=\n\tupdatedAt\x18  \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18! \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12]\n\x02gc\x18\" \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionStatus\x12]\n\x07groupby\x18# \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyGroupByStatus\x12[\n\x05usage\x18$ \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18% \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x7f\n\x18SuccessiveHalvingOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x02 \x01(\x05\x12\x1c\n\x14minEarlyStoppingRate\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"h\n\x15SuccessiveHalvingSpec\x12\x0e\n\x06\x62udget\x18\x01 \x01(\x05\x12\x0f\n\x07\x62racket\x18\x02 \x01(\x05\x12\x0c\n\x04rung\x18\x03 \x01(\x05\x12\x0e\n\x06\x63onfID\x18\x04 \x01(\x05\x12\x10\n\x08modality\x18\x1a \x01(\t\"\xad\x01\n\x10TextPipelineSpec\x12\x0f\n\x07\x65ncoder\x18\x01 \x01(\t\x12\x11\n\ttokenizer\x18\x02 \x01(\t\x12\x11\n\tstopwords\x18\x03 \x01(\x08\x12\x0b\n\x03pos\x18\x04 \x01(\x08\x12\r\n\x05lemma\x18\x05 \x01(\x08\x12\x0c\n\x04stem\x18\x06 \x01(\x08\x12\x11\n\tembedding\x18\x07 \x01(\t\x12\x0b\n\x03svd\x18\x08 \x01(\x08\x12\x18\n\x10maxSvdComponents\x18\t \x01(\x05\"b\n\x16ThresholdPrunerOptions\x12\r\n\x05lower\x18\x01 \x01(\x01\x12\r\n\x05upper\x18\x02 \x01(\x01\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x15\n\rintervalSteps\x18\x04 \x01(\x05\"\x8a\x01\n\x0fTimeSeriesEvent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0f\n\x07holiday\x18\x03 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x10\n\x08preEvent\x18\x05 \x01(\x05\x12\x11\n\tpostEvent\x18\x06 \x01(\x05\x12\x12\n\ntimePoints\x18\x07 \x03(\t\"\x9c\x05\n\x0cTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08priority\x18\x02 \x01(\t\x12\x0e\n\x06\x63vtype\x18\x03 \x01(\t\x12\n\n\x02\x63V\x18\x04 \x01(\x08\x12\r\n\x05\x66olds\x18\x05 \x01(\x05\x12V\n\x05split\x18\x06 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataSplitSpec\x12\x13\n\x0b\x65valMetrics\x18\x07 \x03(\t\x12[\n\x02sh\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingSpec\x12\x0c\n\x04seed\x18\x0b \x01(\x01\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03gpu\x18\r \x01(\x08\x12\x13\n\x0b\x64istributed\x18\x0e \x01(\x08\x12\x19\n\x11\x66\x65\x61tureImportance\x18\x0f \x01(\x08\x12\x11\n\tnodeCount\x18\x10 \x01(\x05\x12\x11\n\tsamplePct\x18\x11 \x01(\x05\x12\\\n\ncheckpoint\x18\x12 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CheckpointSpec\x12\x10\n\x08logLevel\x18\x13 \x01(\t\x12\x15\n\rtimeoutInSecs\x18\x14 \x01(\x05\"\xdc\x01\n\x18UnivariateForecastStatus\x12\x1b\n\x13gridSearchResultURI\x18\x01 \x01(\t\x12g\n\rbaseEstimator\x18\x02 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x10\n\x08modelURI\x18\x03 \x01(\t\x12\x13\n\x0b\x63vResultURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x05 \x01(\t\"\'\n\x11VideoPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"=\n\nWindowSpec\x12\x10\n\x08interval\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x0e\n\x06length\x18\x03 \x01(\x05\x42:Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1'
@@ -174,61 +174,61 @@
   _REPORT._serialized_start=22294
   _REPORT._serialized_end=22542
   _REPORTGROUPBYSTATUS._serialized_start=22545
   _REPORTGROUPBYSTATUS._serialized_end=22683
   _REPORTLIST._serialized_start=22686
   _REPORTLIST._serialized_end=22845
   _REPORTSPEC._serialized_start=22848
-  _REPORTSPEC._serialized_end=23323
-  _REPORTSTATUS._serialized_start=23326
-  _REPORTSTATUS._serialized_end=23813
-  _RUNTIMESTATUS._serialized_start=23816
-  _RUNTIMESTATUS._serialized_end=24057
-  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_start=24004
-  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_end=24057
-  _SEARCHSPEC._serialized_start=24060
-  _SEARCHSPEC._serialized_end=24730
-  _SEASONALITYPERIODSPEC._serialized_start=24732
-  _SEASONALITYPERIODSPEC._serialized_end=24808
-  _SEASONALITYSPEC._serialized_start=24811
-  _SEASONALITYSPEC._serialized_end=25330
-  _SEGMENTSPEC._serialized_start=25332
-  _SEGMENTSPEC._serialized_end=25392
-  _SERVINGENVIRONMENT._serialized_start=25395
-  _SERVINGENVIRONMENT._serialized_end=25834
-  _SERVINGSPEC._serialized_start=25837
-  _SERVINGSPEC._serialized_end=26319
-  _SERVINGSTATUS._serialized_start=26321
-  _SERVINGSTATUS._serialized_end=26424
-  _STUDY._serialized_start=26427
-  _STUDY._serialized_end=26672
-  _STUDYGROUPBYSTATUS._serialized_start=26675
-  _STUDYGROUPBYSTATUS._serialized_end=26812
-  _STUDYLIST._serialized_start=26815
-  _STUDYLIST._serialized_end=26972
-  _STUDYPHASESTATUS._serialized_start=26975
-  _STUDYPHASESTATUS._serialized_end=27283
-  _STUDYSCHEDULESPEC._serialized_start=27285
-  _STUDYSCHEDULESPEC._serialized_end=27382
-  _STUDYSPEC._serialized_start=27385
-  _STUDYSPEC._serialized_end=29543
-  _STUDYSTATUS._serialized_start=29546
-  _STUDYSTATUS._serialized_end=31642
-  _SUCCESSIVEHALVINGOPTIONS._serialized_start=31644
-  _SUCCESSIVEHALVINGOPTIONS._serialized_end=31771
-  _SUCCESSIVEHALVINGSPEC._serialized_start=31773
-  _SUCCESSIVEHALVINGSPEC._serialized_end=31877
-  _TEXTPIPELINESPEC._serialized_start=31880
-  _TEXTPIPELINESPEC._serialized_end=32053
-  _THRESHOLDPRUNEROPTIONS._serialized_start=32055
-  _THRESHOLDPRUNEROPTIONS._serialized_end=32153
-  _TIMESERIESEVENT._serialized_start=32156
-  _TIMESERIESEVENT._serialized_end=32294
-  _TRAININGSPEC._serialized_start=32297
-  _TRAININGSPEC._serialized_end=32965
-  _UNIVARIATEFORECASTSTATUS._serialized_start=32968
-  _UNIVARIATEFORECASTSTATUS._serialized_end=33188
-  _VIDEOPIPELINESPEC._serialized_start=33190
-  _VIDEOPIPELINESPEC._serialized_end=33229
-  _WINDOWSPEC._serialized_start=33231
-  _WINDOWSPEC._serialized_end=33292
+  _REPORTSPEC._serialized_end=23262
+  _REPORTSTATUS._serialized_start=23265
+  _REPORTSTATUS._serialized_end=23828
+  _RUNTIMESTATUS._serialized_start=23831
+  _RUNTIMESTATUS._serialized_end=24072
+  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_start=24019
+  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_end=24072
+  _SEARCHSPEC._serialized_start=24075
+  _SEARCHSPEC._serialized_end=24745
+  _SEASONALITYPERIODSPEC._serialized_start=24747
+  _SEASONALITYPERIODSPEC._serialized_end=24823
+  _SEASONALITYSPEC._serialized_start=24826
+  _SEASONALITYSPEC._serialized_end=25345
+  _SEGMENTSPEC._serialized_start=25347
+  _SEGMENTSPEC._serialized_end=25407
+  _SERVINGENVIRONMENT._serialized_start=25410
+  _SERVINGENVIRONMENT._serialized_end=25849
+  _SERVINGSPEC._serialized_start=25852
+  _SERVINGSPEC._serialized_end=26334
+  _SERVINGSTATUS._serialized_start=26336
+  _SERVINGSTATUS._serialized_end=26439
+  _STUDY._serialized_start=26442
+  _STUDY._serialized_end=26687
+  _STUDYGROUPBYSTATUS._serialized_start=26690
+  _STUDYGROUPBYSTATUS._serialized_end=26827
+  _STUDYLIST._serialized_start=26830
+  _STUDYLIST._serialized_end=26987
+  _STUDYPHASESTATUS._serialized_start=26990
+  _STUDYPHASESTATUS._serialized_end=27298
+  _STUDYSCHEDULESPEC._serialized_start=27300
+  _STUDYSCHEDULESPEC._serialized_end=27397
+  _STUDYSPEC._serialized_start=27400
+  _STUDYSPEC._serialized_end=29558
+  _STUDYSTATUS._serialized_start=29561
+  _STUDYSTATUS._serialized_end=31657
+  _SUCCESSIVEHALVINGOPTIONS._serialized_start=31659
+  _SUCCESSIVEHALVINGOPTIONS._serialized_end=31786
+  _SUCCESSIVEHALVINGSPEC._serialized_start=31788
+  _SUCCESSIVEHALVINGSPEC._serialized_end=31892
+  _TEXTPIPELINESPEC._serialized_start=31895
+  _TEXTPIPELINESPEC._serialized_end=32068
+  _THRESHOLDPRUNEROPTIONS._serialized_start=32070
+  _THRESHOLDPRUNEROPTIONS._serialized_end=32168
+  _TIMESERIESEVENT._serialized_start=32171
+  _TIMESERIESEVENT._serialized_end=32309
+  _TRAININGSPEC._serialized_start=32312
+  _TRAININGSPEC._serialized_end=32980
+  _UNIVARIATEFORECASTSTATUS._serialized_start=32983
+  _UNIVARIATEFORECASTSTATUS._serialized_end=33203
+  _VIDEOPIPELINESPEC._serialized_start=33205
+  _VIDEOPIPELINESPEC._serialized_end=33244
+  _WINDOWSPEC._serialized_start=33246
+  _WINDOWSPEC._serialized_end=33307
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_inference_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_infra_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_catalog_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.services.common.v1 import common_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_common_dot_v1_dot_common__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9github.com/metaprov/modelaapi/services/data/v1/data.proto\x12.github.com.metaprov.modelaapi.services.data.v1\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1aIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\x1a\"k8s.io/api/core/v1/generated.proto\"\xfd\x03\n\x11\x44sReadFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12]\n\x06secret\x18\x06 \x03(\x0b\x32M.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x83\x04\n\x14\x44sReadFeatureRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12`\n\x06secret\x18\x06 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xcf\x04\n\x12\x44sWriteFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x07\x63ontent\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x07 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd0\x02\n\x12\x44sReadAudioRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x03 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x89\x04\n\x17\x44sReadTextCorpusRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x05 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadTextCorpusRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd8\x04\n\x17\x44sReadFromStoreResponse\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12M\n\x06result\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x06 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"p\n\x18\x44sRunDataPipelineRequest\x12T\n\x08pipeline\x18\x01 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"j\n\x19\x44sRunDataPipelineResponse\x12M\n\x06result\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xd1\x08\n\x12\x44sRunRecipeRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\\\n\x11storageConnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\rstorageSecret\x18\x07 \x03(\x0b\x32U.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x62\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.DbSecretEntry\x12L\n\x06recipe\x18\n \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\x12R\n\treciperun\x18\x0b \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"c\n\x13\x44sRunRecipeResponse\x12L\n\x06result\x18\x01 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x9b\x08\n\x1c\x44sCreateRecipeProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\\\n\x11storageConnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12v\n\rstorageSecret\x18\x07 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileRequest.DbSecretEntry\x12L\n\x06recipe\x18\n \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"l\n\x1d\x44sCreateRecipeProfileResponse\x12K\n\x06result\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\x14\n\x12\x44\x61taSourceResponse\"\x11\n\x0f\x44\x61tasetResponse\"\xf4\x02\n\x1d\x44sCreateDatasetProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xb3\x02\n\x1e\x44sCreateDatasetProfileResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0f\x61nomalyLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xce\x08\n\x1b\x44sCreateModelProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12g\n\x06secret\x18\n \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest.SecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x0b \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\x0c \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"+\n\x1c\x44sCreateModelProfileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xde\x08\n\x1a\x44sMergeForecastFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x66\n\x06secret\x18\n \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.SecretEntry\x12\x11\n\tforecasts\x18\x0b \x03(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12j\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"*\n\x1b\x44sMergeForecastFileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xcf\x08\n\x1b\x44sCreateStudyProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x05study\x18\x04 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12O\n\x06models\x18\x08 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12g\n\x06secret\x18\t \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest.SecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\n \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\x0b \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"+\n\x1c\x44sCreateStudyProfileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xc3\x07\n\x13RunTestSuiteRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12Y\n\thistogram\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12\\\n\x0crefHistogram\x18\n \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12Q\n\x05suite\x18\x0b \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"p\n\x14RunTestSuiteResponse\x12X\n\x06result\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\"\xba\x07\n\x18\x44sGenerateDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x64\n\x06secret\x18\x06 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest.SecretEntry\x12\x0c\n\x04rows\x18\x07 \x01(\x05\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12h\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest.DbSecretEntry\x12U\n\x06target\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"r\n\x19\x44sGenerateDatasetResponse\x12U\n\x06target\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xaa\t\n\x15\x44sSplitDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x61\n\x06secret\x18\x08 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest.SecretEntry\x12V\n\x0ftrainingDataset\x18\t \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\x0etestingDataset\x18\n \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\r\n\x05group\x18\x0b \x01(\x08\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x65\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xa8\x01\n\x16\x44sSplitDatasetResponse\x12\x10\n\x08training\x18\x01 \x01(\x05\x12\x0f\n\x07testing\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x15\n\rtraining_hash\x18\x04 \x01(\t\x12\x14\n\x0ctesting_hash\x18\x05 \x01(\t\x12\x17\n\x0fvalidation_hash\x18\x06 \x01(\t\x12\x11\n\tindexFile\x18\x07 \x01(\t\"\xc8\x05\n\x1c\x44sSplitDatasetToRungsRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12h\n\x06secret\x18\x07 \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsRequest.SecretEntry\x12\r\n\x05rungs\x18\x08 \x01(\x05\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x1f\n\x1d\x44sSplitDatasetToRungsResponse\"\xa4\x07\n\x12\x44sTransformRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x08 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsTransformRequest.SecretEntry\x12V\n\x0ftrainingDataset\x18\t \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\x0etestingDataset\x18\n \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"[\n\x13\x44sTransformResponse\x12\x15\n\rtraining_hash\x18\x04 \x01(\t\x12\x14\n\x0ctesting_hash\x18\x05 \x01(\t\x12\x17\n\x0fvalidation_hash\x18\x06 \x01(\t\"\xd9\x07\n\x1c\x44sCreateColumnProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12h\n\x06secret\x18\x07 \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileRequest.SecretEntry\x12\x12\n\ncolumnType\x18\x08 \x01(\t\x12\x12\n\ncolumnName\x18\t \x01(\t\x12W\n\x0c\x64\x62\x43onnection\x18\n \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\x0b \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"s\n\x1d\x44sCreateColumnProfileResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x44\n\x04plot\x18\x02 \x01(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.Plot\"\x9c\x07\n\x15GroupByDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x61\n\x06secret\x18\x07 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest.SecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x65\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"%\n\x16GroupByDatasetResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xd5\x01\n\x14\x44sInferSchemaRequest\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"j\n\x15\x44sInferSchemaResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\"\xdc\x01\n\x15\x44sGetTableViewRequest\x12Z\n\x08\x66latfile\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"h\n\x16\x44sGetTableViewResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\xb2\x07\n\x18\x43reateModelReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x64\n\x06secret\x18\x08 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.CreateModelReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\n \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12\r\n\x05group\x18\x0b \x01(\x08\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xb2\t\n\x1b\x43reateForecastReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12Q\n\x08\x66orecast\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12g\n\x06secret\x18\x08 \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\n \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12\r\n\x05group\x18\x0b \x01(\x08\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd7\x06\n\x1a\x43reateSummaryReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12U\n\nconnection\x18\x03 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x06secret\x18\x04 \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\x06 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12j\n\x08\x64\x62Secret\x18\x08 \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"#\n\x14\x43reateReportResponse\x12\x0b\n\x03pdf\x18\x01 \x01(\x0c\"\xc3\x03\n\x1a\x43reateDatasetReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12P\n\x06report\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\x9c\t\n\x18\x43reateStudyReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12S\n\x06models\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelList\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x64\n\x06secret\x18\t \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.CreateStudyReportRequest.SecretEntry\x12P\n\x06report\x18\n \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12W\n\x0c\x64\x62\x43onnection\x18\x0b \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12h\n\x08\x64\x62Secret\x18\x0c \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.CreateStudyReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xc4\x04\n\x0f\x41skModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x11\n\tdefaultHP\x18\x07 \x01(\x08\x12\x11\n\talgorithm\x18\x08 \x01(\t\x12V\n\nalgorithms\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xc6\x03\n\x1fGetTimeSeriesDatasetKeysRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"0\n GetTimeSeriesDatasetKeysResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\"\xa4\x04\n\x17\x41skForecastModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0c\n\x04keys\x18\x06 \x03(\t\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"j\n\x18\x41skForecastModelResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xe2\x04\n\x12\x41skEnsembleRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12O\n\x06models\x18\x06 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skEnsembleResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xb0\x04\n\x12\x41skBaselineRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x10\n\x08\x61lgnames\x18\x06 \x03(\t\x12\x0b\n\x03\x61ll\x18\x07 \x01(\x08\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skBaselineResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xb7\x04\n\x1a\x41skAllModelsForTaskRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x0c\n\x04task\x18\x07 \x01(\t\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"m\n\x1b\x41skAllModelsForTaskResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x97\x04\n\x10TellModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12\x0e\n\x06\x66\x61iled\x18\x07 \x01(\x08\"#\n\x11TellModelResponse\x12\x0e\n\x06pruned\x18\x01 \x01(\x08\"\x13\n\x11\x44sShutdownRequest\"\x14\n\x12\x44sShutdownResponse\"\xda\x02\n\x17\x44sTestConnectionRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x63\n\x06secret\x18\x03 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"7\n\x18\x44sTestConnectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x08\x12\x0b\n\x03msg\x18\x02 \x01(\t\"\xf7\x05\n\x13\x44sStudyEndedRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12_\n\x06secret\x18\x08 \x03(\x0b\x32O.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x16\n\x14\x44sStudyEndedResponse\"\xfd\x05\n\x16SaveOptimizerDBRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x62\n\x06secret\x18\x08 \x03(\x0b\x32R.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x19\n\x17SaveOptimizerDBResponse\"n\n\x15\x44sGetDatabasesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"+\n\x16\x44sGetDatabasesResponse\x12\x11\n\tdatabases\x18\x01 \x03(\t\"k\n\x12\x44sGetTablesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"%\n\x13\x44sGetTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"y\n\x13\x44sExecuteSqlRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x0b\n\x03sql\x18\x04 \x01(\t\"f\n\x14\x44sExecuteSqlResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\xe8\x02\n\x11\x44sSnapshotRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\x14\n\x12\x44sSnapshotResponse\"b\n\x10\x41skModelResponse\x12N\n\x05model\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x95\x08\n\x16GenTrainingDataRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12\\\n\x11storageConnection\x18\x03 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12p\n\rstorageSecret\x18\x05 \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x08\x64\x62Secret\x18\x07 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest.DbSecretEntry\x12S\n\x05model\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x08\x65ntities\x18\t \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\n \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\'\n\x17GenTrainingDataResponse\x12\x0c\n\x04path\x18\x01 \x01(\t\"\xeb\x06\n\x16SyncOnlineStoreRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12p\n\rstorageSecret\x18\x03 \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x19\n\x17SyncOnlineStoreResponse\"\xfd\x06\n\x1cGenOnlineStoreDatasetRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12v\n\rstorageSecret\x18\x03 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"x\n\x1dGenOnlineStoreDatasetResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x8d\x08\n\x13\x42\x61tchPredictRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12m\n\rstorageSecret\x18\x03 \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.DbSecretEntry\x12X\n\nmodelclass\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x05model\x18\x07 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x08\x65ntities\x18\x08 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12Y\n\nprediction\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"$\n\x14\x42\x61tchPredictResponse\x12\x0c\n\x04rows\x18\x01 \x01(\x05\"\xba\x05\n\x12SaveDatasetRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12X\n\nmodelclass\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x05 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x62\n\x08\x64\x62Secret\x18\x07 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.SaveDatasetRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x84\x06\n\x10SaveModelRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12X\n\nmodelclass\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x04 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12R\n\x06groups\x18\x06 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12`\n\x08\x64\x62Secret\x18\x08 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.SaveModelRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xce\x05\n\x15SavePredictionRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\tpredictor\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\x12Y\n\nprediction\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x65\n\x08\x64\x62Secret\x18\x07 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.SavePredictionRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x92\x04\n\x14SavePredictorRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12X\n\tpredictor\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x64\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32R.github.com.metaprov.modelaapi.services.data.v1.SavePredictorRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x84\x01\n\x19\x43reateMetricsStoreRequest\x12\x0e\n\x06tenant\x18\x01 \x01(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x1c\n\x1a\x43reateMetricsStoreResponse\"\x1c\n\x0cSaveResponse\x12\x0c\n\x04\x64\x62id\x18\x01 \x01(\x05\x32\xf7\x43\n\x0b\x44\x61taService\x12\x98\x01\n\x08ReadFile\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9e\x01\n\x0bReadFeature\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9a\x01\n\tReadAudio\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fRunDataPipeline\x12H.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineResponse\"\x00\x12\x96\x01\n\tRunRecipe\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeResponse\"\x00\x12\x9a\x01\n\tWriteFile\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fGenerateDataset\x12H.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetResponse\"\x00\x12\x9f\x01\n\x0cSplitDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetResponse\"\x00\x12\x96\x01\n\tTransform\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsTransformRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsTransformResponse\"\x00\x12\xb4\x01\n\x13\x43reateColumnProfile\x12L.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileResponse\"\x00\x12\x9c\x01\n\x0bInferSchema\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaRequest\x1a\x45.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaResponse\"\x00\x12\x9f\x01\n\x0cGetTableView\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewResponse\"\x00\x12\xb4\x01\n\x13SplitDatasetToRungs\x12L.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsResponse\"\x00\x12\xb7\x01\n\x14\x43reateDatasetProfile\x12M.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileRequest\x1aN.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateModelProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateStudyProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileResponse\"\x00\x12\xb4\x01\n\x13\x43reateRecipeProfile\x12L.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileResponse\"\x00\x12\xa5\x01\n\x11\x43reateModelReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateModelReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa5\x01\n\x11\x43reateStudyReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateStudyReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateDatasetReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateDatasetReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xab\x01\n\x14\x43reateForecastReport\x12K.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateSummaryReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\x8c\x01\n\x05\x41skFE\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\x98\x01\n\x0b\x41skBaseline\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskBaselineRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskBaselineResponse\"\x00\x12\x98\x01\n\x0b\x41skEnsemble\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleResponse\"\x00\x12\xa7\x01\n\x10\x41skForecastModel\x12G.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelResponse\"\x00\x12\x8f\x01\n\x08\x41skModel\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\xb0\x01\n\x13\x41skAllModelsForTask\x12J.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskResponse\"\x00\x12\x99\x01\n\x10TellPartialModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\x92\x01\n\tTellModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\xae\x01\n\x11MergeForecastFile\x12J.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileResponse\"\x00\x12\xa7\x01\n\x10\x44sTestConnection\x12G.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionResponse\"\x00\x12\x93\x01\n\x08ShutDown\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsShutdownRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsShutdownResponse\"\x00\x12\x99\x01\n\nStudyEnded\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedResponse\"\x00\x12\xa4\x01\n\x0fSaveOptimizerDB\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBResponse\"\x00\x12\x9f\x01\n\x0cGetDatabases\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesResponse\"\x00\x12\x96\x01\n\tGetTables\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesResponse\"\x00\x12\x99\x01\n\nExecuteSql\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlResponse\"\x00\x12\x93\x01\n\x08Snapshot\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotResponse\"\x00\x12\x9e\x01\n\x0fUnitTestDataset\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9c\x01\n\rUnitTestModel\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9f\x01\n\x10UnitTestFeedback\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa7\x01\n\x18UnitTestFeatureHistogram\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa0\x01\n\x11UnitTestPredictor\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa1\x01\n\x0eGroupByDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetResponse\"\x00\x12\xa4\x01\n\x0fSyncOnlineStore\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreResponse\"\x00\x12\xa4\x01\n\x0fGenTrainingData\x12\x46.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataResponse\"\x00\x12\xb6\x01\n\x15GenOnlineStoreDataset\x12L.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetResponse\"\x00\x12\x9b\x01\n\x0c\x42\x61tchPredict\x12\x43.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.BatchPredictResponse\"\x00\x12\x91\x01\n\x0bSaveDataSet\x12\x42.github.com.metaprov.modelaapi.services.data.v1.SaveDatasetRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x8d\x01\n\tSaveModel\x12@.github.com.metaprov.modelaapi.services.data.v1.SaveModelRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x97\x01\n\x0eSavePrediction\x12\x45.github.com.metaprov.modelaapi.services.data.v1.SavePredictionRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\xad\x01\n\x12\x43reateMetricsStore\x12I.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreRequest\x1aJ.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreResponse\"\x00\x42\x30Z.github.com/metaprov/modelaapi/services/data/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9github.com/metaprov/modelaapi/services/data/v1/data.proto\x12.github.com.metaprov.modelaapi.services.data.v1\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1aIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\x1a\"k8s.io/api/core/v1/generated.proto\"\xfd\x03\n\x11\x44sReadFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12]\n\x06secret\x18\x06 \x03(\x0b\x32M.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x83\x04\n\x14\x44sReadFeatureRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12`\n\x06secret\x18\x06 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xcf\x04\n\x12\x44sWriteFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x07\x63ontent\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x07 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd0\x02\n\x12\x44sReadAudioRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x03 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x89\x04\n\x17\x44sReadTextCorpusRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x05 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadTextCorpusRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd8\x04\n\x17\x44sReadFromStoreResponse\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12M\n\x06result\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x06 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"p\n\x18\x44sRunDataPipelineRequest\x12T\n\x08pipeline\x18\x01 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"j\n\x19\x44sRunDataPipelineResponse\x12M\n\x06result\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xd1\x08\n\x12\x44sRunRecipeRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\\\n\x11storageConnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\rstorageSecret\x18\x07 \x03(\x0b\x32U.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x62\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.DbSecretEntry\x12L\n\x06recipe\x18\n \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\x12R\n\treciperun\x18\x0b \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"c\n\x13\x44sRunRecipeResponse\x12L\n\x06result\x18\x01 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x9b\x08\n\x1c\x44sCreateRecipeProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\\\n\x11storageConnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12v\n\rstorageSecret\x18\x07 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileRequest.DbSecretEntry\x12L\n\x06recipe\x18\n \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"l\n\x1d\x44sCreateRecipeProfileResponse\x12K\n\x06result\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\x14\n\x12\x44\x61taSourceResponse\"\x11\n\x0f\x44\x61tasetResponse\"\xf4\x02\n\x1d\x44sCreateDatasetProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xb3\x02\n\x1e\x44sCreateDatasetProfileResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0f\x61nomalyLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xce\x08\n\x1b\x44sCreateModelProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12g\n\x06secret\x18\n \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest.SecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x0b \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\x0c \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"+\n\x1c\x44sCreateModelProfileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xde\x08\n\x1a\x44sMergeForecastFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x66\n\x06secret\x18\n \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.SecretEntry\x12\x11\n\tforecasts\x18\x0b \x03(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12j\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"*\n\x1b\x44sMergeForecastFileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xcf\x08\n\x1b\x44sCreateStudyProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x05study\x18\x04 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12O\n\x06models\x18\x08 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12g\n\x06secret\x18\t \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest.SecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\n \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\x0b \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"+\n\x1c\x44sCreateStudyProfileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xc3\x07\n\x13RunTestSuiteRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12Y\n\thistogram\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12\\\n\x0crefHistogram\x18\n \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12Q\n\x05suite\x18\x0b \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"p\n\x14RunTestSuiteResponse\x12X\n\x06result\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\"\xba\x07\n\x18\x44sGenerateDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x64\n\x06secret\x18\x06 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest.SecretEntry\x12\x0c\n\x04rows\x18\x07 \x01(\x05\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12h\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest.DbSecretEntry\x12U\n\x06target\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"r\n\x19\x44sGenerateDatasetResponse\x12U\n\x06target\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xaa\t\n\x15\x44sSplitDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x61\n\x06secret\x18\x08 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest.SecretEntry\x12V\n\x0ftrainingDataset\x18\t \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\x0etestingDataset\x18\n \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\r\n\x05group\x18\x0b \x01(\x08\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x65\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xa8\x01\n\x16\x44sSplitDatasetResponse\x12\x10\n\x08training\x18\x01 \x01(\x05\x12\x0f\n\x07testing\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x15\n\rtraining_hash\x18\x04 \x01(\t\x12\x14\n\x0ctesting_hash\x18\x05 \x01(\t\x12\x17\n\x0fvalidation_hash\x18\x06 \x01(\t\x12\x11\n\tindexFile\x18\x07 \x01(\t\"\xc8\x05\n\x1c\x44sSplitDatasetToRungsRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12h\n\x06secret\x18\x07 \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsRequest.SecretEntry\x12\r\n\x05rungs\x18\x08 \x01(\x05\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x1f\n\x1d\x44sSplitDatasetToRungsResponse\"\xa4\x07\n\x12\x44sTransformRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x08 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsTransformRequest.SecretEntry\x12V\n\x0ftrainingDataset\x18\t \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\x0etestingDataset\x18\n \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"[\n\x13\x44sTransformResponse\x12\x15\n\rtraining_hash\x18\x04 \x01(\t\x12\x14\n\x0ctesting_hash\x18\x05 \x01(\t\x12\x17\n\x0fvalidation_hash\x18\x06 \x01(\t\"\xd9\x07\n\x1c\x44sCreateColumnProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12h\n\x06secret\x18\x07 \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileRequest.SecretEntry\x12\x12\n\ncolumnType\x18\x08 \x01(\t\x12\x12\n\ncolumnName\x18\t \x01(\t\x12W\n\x0c\x64\x62\x43onnection\x18\n \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\x0b \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"s\n\x1d\x44sCreateColumnProfileResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x44\n\x04plot\x18\x02 \x01(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.Plot\"\x9c\x07\n\x15GroupByDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x61\n\x06secret\x18\x07 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest.SecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x65\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"%\n\x16GroupByDatasetResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xd5\x01\n\x14\x44sInferSchemaRequest\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"j\n\x15\x44sInferSchemaResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\"\xdc\x01\n\x15\x44sGetTableViewRequest\x12Z\n\x08\x66latfile\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"h\n\x16\x44sGetTableViewResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\xe1\x04\n\x18\x43reateModelReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xb2\t\n\x1b\x43reateForecastReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12Q\n\x08\x66orecast\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12g\n\x06secret\x18\x08 \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\n \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12\r\n\x05group\x18\x0b \x01(\x08\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd7\x06\n\x1a\x43reateSummaryReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12U\n\nconnection\x18\x03 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x06secret\x18\x04 \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\x06 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12j\n\x08\x64\x62Secret\x18\x08 \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"#\n\x14\x43reateReportResponse\x12\x0b\n\x03pdf\x18\x01 \x01(\x0c\"\xc3\x03\n\x1a\x43reateDatasetReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12P\n\x06report\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe6\x04\n\x18\x43reateStudyReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12S\n\x06models\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelList\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xc4\x04\n\x0f\x41skModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x11\n\tdefaultHP\x18\x07 \x01(\x08\x12\x11\n\talgorithm\x18\x08 \x01(\t\x12V\n\nalgorithms\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xc6\x03\n\x1fGetTimeSeriesDatasetKeysRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"0\n GetTimeSeriesDatasetKeysResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\"\xa4\x04\n\x17\x41skForecastModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0c\n\x04keys\x18\x06 \x03(\t\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"j\n\x18\x41skForecastModelResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xe2\x04\n\x12\x41skEnsembleRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12O\n\x06models\x18\x06 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skEnsembleResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xb0\x04\n\x12\x41skBaselineRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x10\n\x08\x61lgnames\x18\x06 \x03(\t\x12\x0b\n\x03\x61ll\x18\x07 \x01(\x08\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skBaselineResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xb7\x04\n\x1a\x41skAllModelsForTaskRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x0c\n\x04task\x18\x07 \x01(\t\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"m\n\x1b\x41skAllModelsForTaskResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x97\x04\n\x10TellModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12\x0e\n\x06\x66\x61iled\x18\x07 \x01(\x08\"#\n\x11TellModelResponse\x12\x0e\n\x06pruned\x18\x01 \x01(\x08\"\x13\n\x11\x44sShutdownRequest\"\x14\n\x12\x44sShutdownResponse\"\xda\x02\n\x17\x44sTestConnectionRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x63\n\x06secret\x18\x03 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"7\n\x18\x44sTestConnectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x08\x12\x0b\n\x03msg\x18\x02 \x01(\t\"\xf7\x05\n\x13\x44sStudyEndedRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12_\n\x06secret\x18\x08 \x03(\x0b\x32O.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x16\n\x14\x44sStudyEndedResponse\"\xfd\x05\n\x16SaveOptimizerDBRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x62\n\x06secret\x18\x08 \x03(\x0b\x32R.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x19\n\x17SaveOptimizerDBResponse\"n\n\x15\x44sGetDatabasesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"+\n\x16\x44sGetDatabasesResponse\x12\x11\n\tdatabases\x18\x01 \x03(\t\"k\n\x12\x44sGetTablesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"%\n\x13\x44sGetTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"y\n\x13\x44sExecuteSqlRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x0b\n\x03sql\x18\x04 \x01(\t\"f\n\x14\x44sExecuteSqlResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\xe8\x02\n\x11\x44sSnapshotRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\x14\n\x12\x44sSnapshotResponse\"b\n\x10\x41skModelResponse\x12N\n\x05model\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x95\x08\n\x16GenTrainingDataRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12\\\n\x11storageConnection\x18\x03 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12p\n\rstorageSecret\x18\x05 \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x08\x64\x62Secret\x18\x07 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest.DbSecretEntry\x12S\n\x05model\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x08\x65ntities\x18\t \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\n \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\'\n\x17GenTrainingDataResponse\x12\x0c\n\x04path\x18\x01 \x01(\t\"\xeb\x06\n\x16SyncOnlineStoreRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12p\n\rstorageSecret\x18\x03 \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x19\n\x17SyncOnlineStoreResponse\"\xfd\x06\n\x1cGenOnlineStoreDatasetRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12v\n\rstorageSecret\x18\x03 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"x\n\x1dGenOnlineStoreDatasetResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x8d\x08\n\x13\x42\x61tchPredictRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12m\n\rstorageSecret\x18\x03 \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.DbSecretEntry\x12X\n\nmodelclass\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x05model\x18\x07 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x08\x65ntities\x18\x08 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12Y\n\nprediction\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"$\n\x14\x42\x61tchPredictResponse\x12\x0c\n\x04rows\x18\x01 \x01(\x05\"\xba\x05\n\x12SaveDatasetRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12X\n\nmodelclass\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x05 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x62\n\x08\x64\x62Secret\x18\x07 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.SaveDatasetRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x84\x06\n\x10SaveModelRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12X\n\nmodelclass\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x04 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12R\n\x06groups\x18\x06 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12`\n\x08\x64\x62Secret\x18\x08 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.SaveModelRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xce\x05\n\x15SavePredictionRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\tpredictor\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\x12Y\n\nprediction\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x65\n\x08\x64\x62Secret\x18\x07 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.SavePredictionRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x92\x04\n\x14SavePredictorRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12X\n\tpredictor\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x64\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32R.github.com.metaprov.modelaapi.services.data.v1.SavePredictorRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x84\x01\n\x19\x43reateMetricsStoreRequest\x12\x0e\n\x06tenant\x18\x01 \x01(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x1c\n\x1a\x43reateMetricsStoreResponse\"\x1c\n\x0cSaveResponse\x12\x0c\n\x04\x64\x62id\x18\x01 \x01(\x05\x32\xf7\x43\n\x0b\x44\x61taService\x12\x98\x01\n\x08ReadFile\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9e\x01\n\x0bReadFeature\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9a\x01\n\tReadAudio\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fRunDataPipeline\x12H.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineResponse\"\x00\x12\x96\x01\n\tRunRecipe\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeResponse\"\x00\x12\x9a\x01\n\tWriteFile\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fGenerateDataset\x12H.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetResponse\"\x00\x12\x9f\x01\n\x0cSplitDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetResponse\"\x00\x12\x96\x01\n\tTransform\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsTransformRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsTransformResponse\"\x00\x12\xb4\x01\n\x13\x43reateColumnProfile\x12L.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileResponse\"\x00\x12\x9c\x01\n\x0bInferSchema\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaRequest\x1a\x45.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaResponse\"\x00\x12\x9f\x01\n\x0cGetTableView\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewResponse\"\x00\x12\xb4\x01\n\x13SplitDatasetToRungs\x12L.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsResponse\"\x00\x12\xb7\x01\n\x14\x43reateDatasetProfile\x12M.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileRequest\x1aN.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateModelProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateStudyProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileResponse\"\x00\x12\xb4\x01\n\x13\x43reateRecipeProfile\x12L.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileResponse\"\x00\x12\xa5\x01\n\x11\x43reateModelReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateModelReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa5\x01\n\x11\x43reateStudyReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateStudyReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateDatasetReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateDatasetReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xab\x01\n\x14\x43reateForecastReport\x12K.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateSummaryReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\x8c\x01\n\x05\x41skFE\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\x98\x01\n\x0b\x41skBaseline\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskBaselineRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskBaselineResponse\"\x00\x12\x98\x01\n\x0b\x41skEnsemble\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleResponse\"\x00\x12\xa7\x01\n\x10\x41skForecastModel\x12G.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelResponse\"\x00\x12\x8f\x01\n\x08\x41skModel\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\xb0\x01\n\x13\x41skAllModelsForTask\x12J.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskResponse\"\x00\x12\x99\x01\n\x10TellPartialModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\x92\x01\n\tTellModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\xae\x01\n\x11MergeForecastFile\x12J.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileResponse\"\x00\x12\xa7\x01\n\x10\x44sTestConnection\x12G.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionResponse\"\x00\x12\x93\x01\n\x08ShutDown\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsShutdownRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsShutdownResponse\"\x00\x12\x99\x01\n\nStudyEnded\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedResponse\"\x00\x12\xa4\x01\n\x0fSaveOptimizerDB\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBResponse\"\x00\x12\x9f\x01\n\x0cGetDatabases\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesResponse\"\x00\x12\x96\x01\n\tGetTables\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesResponse\"\x00\x12\x99\x01\n\nExecuteSql\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlResponse\"\x00\x12\x93\x01\n\x08Snapshot\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotResponse\"\x00\x12\x9e\x01\n\x0fUnitTestDataset\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9c\x01\n\rUnitTestModel\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9f\x01\n\x10UnitTestFeedback\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa7\x01\n\x18UnitTestFeatureHistogram\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa0\x01\n\x11UnitTestPredictor\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa1\x01\n\x0eGroupByDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetResponse\"\x00\x12\xa4\x01\n\x0fSyncOnlineStore\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreResponse\"\x00\x12\xa4\x01\n\x0fGenTrainingData\x12\x46.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataResponse\"\x00\x12\xb6\x01\n\x15GenOnlineStoreDataset\x12L.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetResponse\"\x00\x12\x9b\x01\n\x0c\x42\x61tchPredict\x12\x43.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.BatchPredictResponse\"\x00\x12\x91\x01\n\x0bSaveDataSet\x12\x42.github.com.metaprov.modelaapi.services.data.v1.SaveDatasetRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x8d\x01\n\tSaveModel\x12@.github.com.metaprov.modelaapi.services.data.v1.SaveModelRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x97\x01\n\x0eSavePrediction\x12\x45.github.com.metaprov.modelaapi.services.data.v1.SavePredictionRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\xad\x01\n\x12\x43reateMetricsStore\x12I.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreRequest\x1aJ.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreResponse\"\x00\x42\x30Z.github.com/metaprov/modelaapi/services/data/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.data.v1.data_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z.github.com/metaprov/modelaapi/services/data/v1'
@@ -76,28 +76,22 @@
   _DSCREATECOLUMNPROFILEREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _DSCREATECOLUMNPROFILEREQUEST_DBSECRETENTRY._options = None
   _DSCREATECOLUMNPROFILEREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
   _GROUPBYDATASETREQUEST_SECRETENTRY._options = None
   _GROUPBYDATASETREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _GROUPBYDATASETREQUEST_DBSECRETENTRY._options = None
   _GROUPBYDATASETREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
-  _CREATEMODELREPORTREQUEST_SECRETENTRY._options = None
-  _CREATEMODELREPORTREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _CREATEFORECASTREPORTREQUEST_SECRETENTRY._options = None
   _CREATEFORECASTREPORTREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _CREATEFORECASTREPORTREQUEST_DBSECRETENTRY._options = None
   _CREATEFORECASTREPORTREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
   _CREATESUMMARYREPORTREQUEST_SECRETENTRY._options = None
   _CREATESUMMARYREPORTREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _CREATESUMMARYREPORTREQUEST_DBSECRETENTRY._options = None
   _CREATESUMMARYREPORTREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
-  _CREATESTUDYREPORTREQUEST_SECRETENTRY._options = None
-  _CREATESTUDYREPORTREQUEST_SECRETENTRY._serialized_options = b'8\001'
-  _CREATESTUDYREPORTREQUEST_DBSECRETENTRY._options = None
-  _CREATESTUDYREPORTREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
   _DSTESTCONNECTIONREQUEST_SECRETENTRY._options = None
   _DSTESTCONNECTIONREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _DSSTUDYENDEDREQUEST_SECRETENTRY._options = None
   _DSSTUDYENDEDREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _SAVEOPTIMIZERDBREQUEST_SECRETENTRY._options = None
   _SAVEOPTIMIZERDBREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _GENTRAININGDATAREQUEST_STORAGESECRETENTRY._options = None
@@ -253,155 +247,149 @@
   _DSINFERSCHEMARESPONSE._serialized_start=18032
   _DSINFERSCHEMARESPONSE._serialized_end=18138
   _DSGETTABLEVIEWREQUEST._serialized_start=18141
   _DSGETTABLEVIEWREQUEST._serialized_end=18361
   _DSGETTABLEVIEWRESPONSE._serialized_start=18363
   _DSGETTABLEVIEWRESPONSE._serialized_end=18467
   _CREATEMODELREPORTREQUEST._serialized_start=18470
-  _CREATEMODELREPORTREQUEST._serialized_end=19416
-  _CREATEMODELREPORTREQUEST_SECRETENTRY._serialized_start=1036
-  _CREATEMODELREPORTREQUEST_SECRETENTRY._serialized_end=1081
-  _CREATEFORECASTREPORTREQUEST._serialized_start=19419
-  _CREATEFORECASTREPORTREQUEST._serialized_end=20621
+  _CREATEMODELREPORTREQUEST._serialized_end=19079
+  _CREATEFORECASTREPORTREQUEST._serialized_start=19082
+  _CREATEFORECASTREPORTREQUEST._serialized_end=20284
   _CREATEFORECASTREPORTREQUEST_SECRETENTRY._serialized_start=1036
   _CREATEFORECASTREPORTREQUEST_SECRETENTRY._serialized_end=1081
   _CREATEFORECASTREPORTREQUEST_DBSECRETENTRY._serialized_start=4942
   _CREATEFORECASTREPORTREQUEST_DBSECRETENTRY._serialized_end=4989
-  _CREATESUMMARYREPORTREQUEST._serialized_start=20624
-  _CREATESUMMARYREPORTREQUEST._serialized_end=21479
+  _CREATESUMMARYREPORTREQUEST._serialized_start=20287
+  _CREATESUMMARYREPORTREQUEST._serialized_end=21142
   _CREATESUMMARYREPORTREQUEST_SECRETENTRY._serialized_start=1036
   _CREATESUMMARYREPORTREQUEST_SECRETENTRY._serialized_end=1081
   _CREATESUMMARYREPORTREQUEST_DBSECRETENTRY._serialized_start=4942
   _CREATESUMMARYREPORTREQUEST_DBSECRETENTRY._serialized_end=4989
-  _CREATEREPORTRESPONSE._serialized_start=21481
-  _CREATEREPORTRESPONSE._serialized_end=21516
-  _CREATEDATASETREPORTREQUEST._serialized_start=21519
-  _CREATEDATASETREPORTREQUEST._serialized_end=21970
-  _CREATESTUDYREPORTREQUEST._serialized_start=21973
-  _CREATESTUDYREPORTREQUEST._serialized_end=23153
-  _CREATESTUDYREPORTREQUEST_SECRETENTRY._serialized_start=1036
-  _CREATESTUDYREPORTREQUEST_SECRETENTRY._serialized_end=1081
-  _CREATESTUDYREPORTREQUEST_DBSECRETENTRY._serialized_start=4942
-  _CREATESTUDYREPORTREQUEST_DBSECRETENTRY._serialized_end=4989
-  _ASKMODELREQUEST._serialized_start=23156
-  _ASKMODELREQUEST._serialized_end=23736
-  _GETTIMESERIESDATASETKEYSREQUEST._serialized_start=23739
-  _GETTIMESERIESDATASETKEYSREQUEST._serialized_end=24193
-  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_start=24195
-  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_end=24243
-  _ASKFORECASTMODELREQUEST._serialized_start=24246
-  _ASKFORECASTMODELREQUEST._serialized_end=24794
-  _ASKFORECASTMODELRESPONSE._serialized_start=24796
-  _ASKFORECASTMODELRESPONSE._serialized_end=24902
-  _ASKENSEMBLEREQUEST._serialized_start=24905
-  _ASKENSEMBLEREQUEST._serialized_end=25515
-  _ASKENSEMBLERESPONSE._serialized_start=25517
-  _ASKENSEMBLERESPONSE._serialized_end=25618
-  _ASKBASELINEREQUEST._serialized_start=25621
-  _ASKBASELINEREQUEST._serialized_end=26181
-  _ASKBASELINERESPONSE._serialized_start=26183
-  _ASKBASELINERESPONSE._serialized_end=26284
-  _ASKALLMODELSFORTASKREQUEST._serialized_start=26287
-  _ASKALLMODELSFORTASKREQUEST._serialized_end=26854
-  _ASKALLMODELSFORTASKRESPONSE._serialized_start=26856
-  _ASKALLMODELSFORTASKRESPONSE._serialized_end=26965
-  _TELLMODELREQUEST._serialized_start=26968
-  _TELLMODELREQUEST._serialized_end=27503
-  _TELLMODELRESPONSE._serialized_start=27505
-  _TELLMODELRESPONSE._serialized_end=27540
-  _DSSHUTDOWNREQUEST._serialized_start=27542
-  _DSSHUTDOWNREQUEST._serialized_end=27561
-  _DSSHUTDOWNRESPONSE._serialized_start=27563
-  _DSSHUTDOWNRESPONSE._serialized_end=27583
-  _DSTESTCONNECTIONREQUEST._serialized_start=27586
-  _DSTESTCONNECTIONREQUEST._serialized_end=27932
+  _CREATEREPORTRESPONSE._serialized_start=21144
+  _CREATEREPORTRESPONSE._serialized_end=21179
+  _CREATEDATASETREPORTREQUEST._serialized_start=21182
+  _CREATEDATASETREPORTREQUEST._serialized_end=21633
+  _CREATESTUDYREPORTREQUEST._serialized_start=21636
+  _CREATESTUDYREPORTREQUEST._serialized_end=22250
+  _ASKMODELREQUEST._serialized_start=22253
+  _ASKMODELREQUEST._serialized_end=22833
+  _GETTIMESERIESDATASETKEYSREQUEST._serialized_start=22836
+  _GETTIMESERIESDATASETKEYSREQUEST._serialized_end=23290
+  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_start=23292
+  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_end=23340
+  _ASKFORECASTMODELREQUEST._serialized_start=23343
+  _ASKFORECASTMODELREQUEST._serialized_end=23891
+  _ASKFORECASTMODELRESPONSE._serialized_start=23893
+  _ASKFORECASTMODELRESPONSE._serialized_end=23999
+  _ASKENSEMBLEREQUEST._serialized_start=24002
+  _ASKENSEMBLEREQUEST._serialized_end=24612
+  _ASKENSEMBLERESPONSE._serialized_start=24614
+  _ASKENSEMBLERESPONSE._serialized_end=24715
+  _ASKBASELINEREQUEST._serialized_start=24718
+  _ASKBASELINEREQUEST._serialized_end=25278
+  _ASKBASELINERESPONSE._serialized_start=25280
+  _ASKBASELINERESPONSE._serialized_end=25381
+  _ASKALLMODELSFORTASKREQUEST._serialized_start=25384
+  _ASKALLMODELSFORTASKREQUEST._serialized_end=25951
+  _ASKALLMODELSFORTASKRESPONSE._serialized_start=25953
+  _ASKALLMODELSFORTASKRESPONSE._serialized_end=26062
+  _TELLMODELREQUEST._serialized_start=26065
+  _TELLMODELREQUEST._serialized_end=26600
+  _TELLMODELRESPONSE._serialized_start=26602
+  _TELLMODELRESPONSE._serialized_end=26637
+  _DSSHUTDOWNREQUEST._serialized_start=26639
+  _DSSHUTDOWNREQUEST._serialized_end=26658
+  _DSSHUTDOWNRESPONSE._serialized_start=26660
+  _DSSHUTDOWNRESPONSE._serialized_end=26680
+  _DSTESTCONNECTIONREQUEST._serialized_start=26683
+  _DSTESTCONNECTIONREQUEST._serialized_end=27029
   _DSTESTCONNECTIONREQUEST_SECRETENTRY._serialized_start=1036
   _DSTESTCONNECTIONREQUEST_SECRETENTRY._serialized_end=1081
-  _DSTESTCONNECTIONRESPONSE._serialized_start=27934
-  _DSTESTCONNECTIONRESPONSE._serialized_end=27989
-  _DSSTUDYENDEDREQUEST._serialized_start=27992
-  _DSSTUDYENDEDREQUEST._serialized_end=28751
+  _DSTESTCONNECTIONRESPONSE._serialized_start=27031
+  _DSTESTCONNECTIONRESPONSE._serialized_end=27086
+  _DSSTUDYENDEDREQUEST._serialized_start=27089
+  _DSSTUDYENDEDREQUEST._serialized_end=27848
   _DSSTUDYENDEDREQUEST_SECRETENTRY._serialized_start=1036
   _DSSTUDYENDEDREQUEST_SECRETENTRY._serialized_end=1081
-  _DSSTUDYENDEDRESPONSE._serialized_start=28753
-  _DSSTUDYENDEDRESPONSE._serialized_end=28775
-  _SAVEOPTIMIZERDBREQUEST._serialized_start=28778
-  _SAVEOPTIMIZERDBREQUEST._serialized_end=29543
+  _DSSTUDYENDEDRESPONSE._serialized_start=27850
+  _DSSTUDYENDEDRESPONSE._serialized_end=27872
+  _SAVEOPTIMIZERDBREQUEST._serialized_start=27875
+  _SAVEOPTIMIZERDBREQUEST._serialized_end=28640
   _SAVEOPTIMIZERDBREQUEST_SECRETENTRY._serialized_start=1036
   _SAVEOPTIMIZERDBREQUEST_SECRETENTRY._serialized_end=1081
-  _SAVEOPTIMIZERDBRESPONSE._serialized_start=29545
-  _SAVEOPTIMIZERDBRESPONSE._serialized_end=29570
-  _DSGETDATABASESREQUEST._serialized_start=29572
-  _DSGETDATABASESREQUEST._serialized_end=29682
-  _DSGETDATABASESRESPONSE._serialized_start=29684
-  _DSGETDATABASESRESPONSE._serialized_end=29727
-  _DSGETTABLESREQUEST._serialized_start=29729
-  _DSGETTABLESREQUEST._serialized_end=29836
-  _DSGETTABLESRESPONSE._serialized_start=29838
-  _DSGETTABLESRESPONSE._serialized_end=29875
-  _DSEXECUTESQLREQUEST._serialized_start=29877
-  _DSEXECUTESQLREQUEST._serialized_end=29998
-  _DSEXECUTESQLRESPONSE._serialized_start=30000
-  _DSEXECUTESQLRESPONSE._serialized_end=30102
-  _DSSNAPSHOTREQUEST._serialized_start=30105
-  _DSSNAPSHOTREQUEST._serialized_end=30465
-  _DSSNAPSHOTRESPONSE._serialized_start=30467
-  _DSSNAPSHOTRESPONSE._serialized_end=30487
-  _ASKMODELRESPONSE._serialized_start=30489
-  _ASKMODELRESPONSE._serialized_end=30587
-  _GENTRAININGDATAREQUEST._serialized_start=30590
-  _GENTRAININGDATAREQUEST._serialized_end=31635
+  _SAVEOPTIMIZERDBRESPONSE._serialized_start=28642
+  _SAVEOPTIMIZERDBRESPONSE._serialized_end=28667
+  _DSGETDATABASESREQUEST._serialized_start=28669
+  _DSGETDATABASESREQUEST._serialized_end=28779
+  _DSGETDATABASESRESPONSE._serialized_start=28781
+  _DSGETDATABASESRESPONSE._serialized_end=28824
+  _DSGETTABLESREQUEST._serialized_start=28826
+  _DSGETTABLESREQUEST._serialized_end=28933
+  _DSGETTABLESRESPONSE._serialized_start=28935
+  _DSGETTABLESRESPONSE._serialized_end=28972
+  _DSEXECUTESQLREQUEST._serialized_start=28974
+  _DSEXECUTESQLREQUEST._serialized_end=29095
+  _DSEXECUTESQLRESPONSE._serialized_start=29097
+  _DSEXECUTESQLRESPONSE._serialized_end=29199
+  _DSSNAPSHOTREQUEST._serialized_start=29202
+  _DSSNAPSHOTREQUEST._serialized_end=29562
+  _DSSNAPSHOTRESPONSE._serialized_start=29564
+  _DSSNAPSHOTRESPONSE._serialized_end=29584
+  _ASKMODELRESPONSE._serialized_start=29586
+  _ASKMODELRESPONSE._serialized_end=29684
+  _GENTRAININGDATAREQUEST._serialized_start=29687
+  _GENTRAININGDATAREQUEST._serialized_end=30732
   _GENTRAININGDATAREQUEST_STORAGESECRETENTRY._serialized_start=4888
   _GENTRAININGDATAREQUEST_STORAGESECRETENTRY._serialized_end=4940
   _GENTRAININGDATAREQUEST_DBSECRETENTRY._serialized_start=4942
   _GENTRAININGDATAREQUEST_DBSECRETENTRY._serialized_end=4989
-  _GENTRAININGDATARESPONSE._serialized_start=31637
-  _GENTRAININGDATARESPONSE._serialized_end=31676
-  _SYNCONLINESTOREREQUEST._serialized_start=31679
-  _SYNCONLINESTOREREQUEST._serialized_end=32554
+  _GENTRAININGDATARESPONSE._serialized_start=30734
+  _GENTRAININGDATARESPONSE._serialized_end=30773
+  _SYNCONLINESTOREREQUEST._serialized_start=30776
+  _SYNCONLINESTOREREQUEST._serialized_end=31651
   _SYNCONLINESTOREREQUEST_STORAGESECRETENTRY._serialized_start=4888
   _SYNCONLINESTOREREQUEST_STORAGESECRETENTRY._serialized_end=4940
   _SYNCONLINESTOREREQUEST_DBSECRETENTRY._serialized_start=4942
   _SYNCONLINESTOREREQUEST_DBSECRETENTRY._serialized_end=4989
-  _SYNCONLINESTORERESPONSE._serialized_start=32556
-  _SYNCONLINESTORERESPONSE._serialized_end=32581
-  _GENONLINESTOREDATASETREQUEST._serialized_start=32584
-  _GENONLINESTOREDATASETREQUEST._serialized_end=33477
+  _SYNCONLINESTORERESPONSE._serialized_start=31653
+  _SYNCONLINESTORERESPONSE._serialized_end=31678
+  _GENONLINESTOREDATASETREQUEST._serialized_start=31681
+  _GENONLINESTOREDATASETREQUEST._serialized_end=32574
   _GENONLINESTOREDATASETREQUEST_STORAGESECRETENTRY._serialized_start=4888
   _GENONLINESTOREDATASETREQUEST_STORAGESECRETENTRY._serialized_end=4940
   _GENONLINESTOREDATASETREQUEST_DBSECRETENTRY._serialized_start=4942
   _GENONLINESTOREDATASETREQUEST_DBSECRETENTRY._serialized_end=4989
-  _GENONLINESTOREDATASETRESPONSE._serialized_start=33479
-  _GENONLINESTOREDATASETRESPONSE._serialized_end=33599
-  _BATCHPREDICTREQUEST._serialized_start=33602
-  _BATCHPREDICTREQUEST._serialized_end=34639
+  _GENONLINESTOREDATASETRESPONSE._serialized_start=32576
+  _GENONLINESTOREDATASETRESPONSE._serialized_end=32696
+  _BATCHPREDICTREQUEST._serialized_start=32699
+  _BATCHPREDICTREQUEST._serialized_end=33736
   _BATCHPREDICTREQUEST_STORAGESECRETENTRY._serialized_start=4888
   _BATCHPREDICTREQUEST_STORAGESECRETENTRY._serialized_end=4940
   _BATCHPREDICTREQUEST_DBSECRETENTRY._serialized_start=4942
   _BATCHPREDICTREQUEST_DBSECRETENTRY._serialized_end=4989
-  _BATCHPREDICTRESPONSE._serialized_start=34641
-  _BATCHPREDICTRESPONSE._serialized_end=34677
-  _SAVEDATASETREQUEST._serialized_start=34680
-  _SAVEDATASETREQUEST._serialized_end=35378
+  _BATCHPREDICTRESPONSE._serialized_start=33738
+  _BATCHPREDICTRESPONSE._serialized_end=33774
+  _SAVEDATASETREQUEST._serialized_start=33777
+  _SAVEDATASETREQUEST._serialized_end=34475
   _SAVEDATASETREQUEST_DBSECRETENTRY._serialized_start=4942
   _SAVEDATASETREQUEST_DBSECRETENTRY._serialized_end=4989
-  _SAVEMODELREQUEST._serialized_start=35381
-  _SAVEMODELREQUEST._serialized_end=36153
+  _SAVEMODELREQUEST._serialized_start=34478
+  _SAVEMODELREQUEST._serialized_end=35250
   _SAVEMODELREQUEST_DBSECRETENTRY._serialized_start=4942
   _SAVEMODELREQUEST_DBSECRETENTRY._serialized_end=4989
-  _SAVEPREDICTIONREQUEST._serialized_start=36156
-  _SAVEPREDICTIONREQUEST._serialized_end=36874
+  _SAVEPREDICTIONREQUEST._serialized_start=35253
+  _SAVEPREDICTIONREQUEST._serialized_end=35971
   _SAVEPREDICTIONREQUEST_DBSECRETENTRY._serialized_start=4942
   _SAVEPREDICTIONREQUEST_DBSECRETENTRY._serialized_end=4989
-  _SAVEPREDICTORREQUEST._serialized_start=36877
-  _SAVEPREDICTORREQUEST._serialized_end=37407
+  _SAVEPREDICTORREQUEST._serialized_start=35974
+  _SAVEPREDICTORREQUEST._serialized_end=36504
   _SAVEPREDICTORREQUEST_DBSECRETENTRY._serialized_start=4942
   _SAVEPREDICTORREQUEST_DBSECRETENTRY._serialized_end=4989
-  _CREATEMETRICSSTOREREQUEST._serialized_start=37410
-  _CREATEMETRICSSTOREREQUEST._serialized_end=37542
-  _CREATEMETRICSSTORERESPONSE._serialized_start=37544
-  _CREATEMETRICSSTORERESPONSE._serialized_end=37572
-  _SAVERESPONSE._serialized_start=37574
-  _SAVERESPONSE._serialized_end=37602
-  _DATASERVICE._serialized_start=37605
-  _DATASERVICE._serialized_end=46300
+  _CREATEMETRICSSTOREREQUEST._serialized_start=36507
+  _CREATEMETRICSSTOREREQUEST._serialized_end=36639
+  _CREATEMETRICSSTORERESPONSE._serialized_start=36641
+  _CREATEMETRICSSTORERESPONSE._serialized_end=36669
+  _SAVERESPONSE._serialized_start=36671
+  _SAVERESPONSE._serialized_end=36699
+  _DATASERVICE._serialized_start=36702
+  _DATASERVICE._serialized_end=45397
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,29 +35,14 @@
                 response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.UpdateModelaSystemResponse.FromString,
                 )
         self.DeleteModelaSystem = channel.unary_unary(
                 '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/DeleteModelaSystem',
                 request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DeleteModelaSystemRequest.SerializeToString,
                 response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DeleteModelaSystemResponse.FromString,
                 )
-        self.DownloadLogfile = channel.unary_unary(
-                '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/DownloadLogfile',
-                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DownloadLogFileRequest.SerializeToString,
-                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DownloadLogFileResponse.FromString,
-                )
-        self.BackupDatabase = channel.unary_unary(
-                '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/BackupDatabase',
-                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.BackupDatabaseRequest.SerializeToString,
-                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.BackupDatabaseResponse.FromString,
-                )
-        self.BackupEtcd = channel.unary_unary(
-                '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/BackupEtcd',
-                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.BackupEtcdRequest.SerializeToString,
-                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.BackupEtcdResponse.FromString,
-                )
 
 
 class ModelaSystemServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def ListModelaSystems(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -85,32 +70,14 @@
 
     def DeleteModelaSystem(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DownloadLogfile(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def BackupDatabase(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def BackupEtcd(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
 
 def add_ModelaSystemServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ListModelaSystems': grpc.unary_unary_rpc_method_handler(
                     servicer.ListModelaSystems,
                     request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.ListModelaSystemsRequest.FromString,
                     response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.ListModelaSystemsResponse.SerializeToString,
@@ -131,29 +98,14 @@
                     response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.UpdateModelaSystemResponse.SerializeToString,
             ),
             'DeleteModelaSystem': grpc.unary_unary_rpc_method_handler(
                     servicer.DeleteModelaSystem,
                     request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DeleteModelaSystemRequest.FromString,
                     response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DeleteModelaSystemResponse.SerializeToString,
             ),
-            'DownloadLogfile': grpc.unary_unary_rpc_method_handler(
-                    servicer.DownloadLogfile,
-                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DownloadLogFileRequest.FromString,
-                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DownloadLogFileResponse.SerializeToString,
-            ),
-            'BackupDatabase': grpc.unary_unary_rpc_method_handler(
-                    servicer.BackupDatabase,
-                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.BackupDatabaseRequest.FromString,
-                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.BackupDatabaseResponse.SerializeToString,
-            ),
-            'BackupEtcd': grpc.unary_unary_rpc_method_handler(
-                    servicer.BackupEtcd,
-                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.BackupEtcdRequest.FromString,
-                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.BackupEtcdResponse.SerializeToString,
-            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -240,58 +192,7 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/DeleteModelaSystem',
             github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DeleteModelaSystemRequest.SerializeToString,
             github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DeleteModelaSystemResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def DownloadLogfile(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/DownloadLogfile',
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DownloadLogFileRequest.SerializeToString,
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DownloadLogFileResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def BackupDatabase(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/BackupDatabase',
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.BackupDatabaseRequest.SerializeToString,
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.BackupDatabaseResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def BackupEtcd(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/BackupEtcd',
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.BackupEtcdRequest.SerializeToString,
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.BackupEtcdResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,198 +1,198 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from github.com.metaprov.modelaapi.services.modelasystem.v1 import modelasystem_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2
+from github.com.metaprov.modelaapi.services.virtualbucket.v1 import virtualbucket_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2
 
 
-class ModelaSystemServiceStub(object):
+class VirtualBucketServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.ListModelaSystems = channel.unary_unary(
-                '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/ListModelaSystems',
-                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.ListModelaSystemsRequest.SerializeToString,
-                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.ListModelaSystemsResponse.FromString,
+        self.ListVirtualBuckets = channel.unary_unary(
+                '/github.com.metaprov.modelaapi.services.virtualbucket.v1.VirtualBucketService/ListVirtualBuckets',
+                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.ListVirtualBucketsRequest.SerializeToString,
+                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.ListVirtualBucketsResponse.FromString,
                 )
-        self.CreateModelaSystem = channel.unary_unary(
-                '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/CreateModelaSystem',
-                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.CreateModelaSystemRequest.SerializeToString,
-                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.CreateModelaSystemResponse.FromString,
+        self.CreateVirtualBucket = channel.unary_unary(
+                '/github.com.metaprov.modelaapi.services.virtualbucket.v1.VirtualBucketService/CreateVirtualBucket',
+                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.CreateVirtualBucketRequest.SerializeToString,
+                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.CreateVirtualBucketResponse.FromString,
                 )
-        self.GetModelaSystem = channel.unary_unary(
-                '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/GetModelaSystem',
-                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.GetModelaSystemRequest.SerializeToString,
-                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.GetModelaSystemResponse.FromString,
+        self.GetVirtualBucket = channel.unary_unary(
+                '/github.com.metaprov.modelaapi.services.virtualbucket.v1.VirtualBucketService/GetVirtualBucket',
+                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.GetVirtualBucketRequest.SerializeToString,
+                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.GetVirtualBucketResponse.FromString,
                 )
-        self.UpdateModelaSystem = channel.unary_unary(
-                '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/UpdateModelaSystem',
-                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.UpdateModelaSystemRequest.SerializeToString,
-                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.UpdateModelaSystemResponse.FromString,
+        self.UpdateVirtualBucket = channel.unary_unary(
+                '/github.com.metaprov.modelaapi.services.virtualbucket.v1.VirtualBucketService/UpdateVirtualBucket',
+                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.UpdateVirtualBucketRequest.SerializeToString,
+                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.UpdateVirtualBucketResponse.FromString,
                 )
-        self.DeleteModelaSystem = channel.unary_unary(
-                '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/DeleteModelaSystem',
-                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DeleteModelaSystemRequest.SerializeToString,
-                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DeleteModelaSystemResponse.FromString,
+        self.DeleteVirtualBucket = channel.unary_unary(
+                '/github.com.metaprov.modelaapi.services.virtualbucket.v1.VirtualBucketService/DeleteVirtualBucket',
+                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.DeleteVirtualBucketRequest.SerializeToString,
+                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.DeleteVirtualBucketResponse.FromString,
                 )
 
 
-class ModelaSystemServiceServicer(object):
+class VirtualBucketServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def ListModelaSystems(self, request, context):
+    def ListVirtualBuckets(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CreateModelaSystem(self, request, context):
+    def CreateVirtualBucket(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetModelaSystem(self, request, context):
+    def GetVirtualBucket(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def UpdateModelaSystem(self, request, context):
+    def UpdateVirtualBucket(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DeleteModelaSystem(self, request, context):
+    def DeleteVirtualBucket(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_ModelaSystemServiceServicer_to_server(servicer, server):
+def add_VirtualBucketServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'ListModelaSystems': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListModelaSystems,
-                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.ListModelaSystemsRequest.FromString,
-                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.ListModelaSystemsResponse.SerializeToString,
+            'ListVirtualBuckets': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListVirtualBuckets,
+                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.ListVirtualBucketsRequest.FromString,
+                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.ListVirtualBucketsResponse.SerializeToString,
             ),
-            'CreateModelaSystem': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateModelaSystem,
-                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.CreateModelaSystemRequest.FromString,
-                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.CreateModelaSystemResponse.SerializeToString,
+            'CreateVirtualBucket': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateVirtualBucket,
+                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.CreateVirtualBucketRequest.FromString,
+                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.CreateVirtualBucketResponse.SerializeToString,
             ),
-            'GetModelaSystem': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetModelaSystem,
-                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.GetModelaSystemRequest.FromString,
-                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.GetModelaSystemResponse.SerializeToString,
+            'GetVirtualBucket': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetVirtualBucket,
+                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.GetVirtualBucketRequest.FromString,
+                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.GetVirtualBucketResponse.SerializeToString,
             ),
-            'UpdateModelaSystem': grpc.unary_unary_rpc_method_handler(
-                    servicer.UpdateModelaSystem,
-                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.UpdateModelaSystemRequest.FromString,
-                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.UpdateModelaSystemResponse.SerializeToString,
+            'UpdateVirtualBucket': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdateVirtualBucket,
+                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.UpdateVirtualBucketRequest.FromString,
+                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.UpdateVirtualBucketResponse.SerializeToString,
             ),
-            'DeleteModelaSystem': grpc.unary_unary_rpc_method_handler(
-                    servicer.DeleteModelaSystem,
-                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DeleteModelaSystemRequest.FromString,
-                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DeleteModelaSystemResponse.SerializeToString,
+            'DeleteVirtualBucket': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteVirtualBucket,
+                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.DeleteVirtualBucketRequest.FromString,
+                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.DeleteVirtualBucketResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService', rpc_method_handlers)
+            'github.com.metaprov.modelaapi.services.virtualbucket.v1.VirtualBucketService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class ModelaSystemService(object):
+class VirtualBucketService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def ListModelaSystems(request,
+    def ListVirtualBuckets(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/ListModelaSystems',
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.ListModelaSystemsRequest.SerializeToString,
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.ListModelaSystemsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.virtualbucket.v1.VirtualBucketService/ListVirtualBuckets',
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.ListVirtualBucketsRequest.SerializeToString,
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.ListVirtualBucketsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CreateModelaSystem(request,
+    def CreateVirtualBucket(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/CreateModelaSystem',
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.CreateModelaSystemRequest.SerializeToString,
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.CreateModelaSystemResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.virtualbucket.v1.VirtualBucketService/CreateVirtualBucket',
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.CreateVirtualBucketRequest.SerializeToString,
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.CreateVirtualBucketResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetModelaSystem(request,
+    def GetVirtualBucket(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/GetModelaSystem',
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.GetModelaSystemRequest.SerializeToString,
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.GetModelaSystemResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.virtualbucket.v1.VirtualBucketService/GetVirtualBucket',
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.GetVirtualBucketRequest.SerializeToString,
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.GetVirtualBucketResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def UpdateModelaSystem(request,
+    def UpdateVirtualBucket(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/UpdateModelaSystem',
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.UpdateModelaSystemRequest.SerializeToString,
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.UpdateModelaSystemResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.virtualbucket.v1.VirtualBucketService/UpdateVirtualBucket',
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.UpdateVirtualBucketRequest.SerializeToString,
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.UpdateVirtualBucketResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def DeleteModelaSystem(request,
+    def DeleteVirtualBucket(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.modelasystem.v1.ModelaSystemService/DeleteModelaSystem',
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DeleteModelaSystemRequest.SerializeToString,
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_modelasystem_dot_v1_dot_modelasystem__pb2.DeleteModelaSystemResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.virtualbucket.v1.VirtualBucketService/DeleteVirtualBucket',
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.DeleteVirtualBucketRequest.SerializeToString,
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_virtualbucket_dot_v1_dot_virtualbucket__pb2.DeleteVirtualBucketResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py` & `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/google/api/annotations_pb2.py` & `modelaapi-0.6.102/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/google/api/http_pb2.py` & `modelaapi-0.6.102/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/k8s/io/api/apps/v1/generated_pb2.py` & `modelaapi-0.6.102/k8s/io/api/apps/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/k8s/io/api/core/v1/generated_pb2.py` & `modelaapi-0.6.102/k8s/io/api/core/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/k8s/io/api/rbac/v1/generated_pb2.py` & `modelaapi-0.6.102/k8s/io/api/rbac/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py` & `modelaapi-0.6.102/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py` & `modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/k8s/io/apimachinery/pkg/runtime/generated_pb2.py` & `modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py` & `modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py` & `modelaapi-0.6.102/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/modelaapi/consts.py` & `modelaapi-0.6.102/modelaapi/consts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/modelaapi/custom_transformers.py` & `modelaapi-0.6.102/modelaapi/custom_transformers.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/modelaapi/graykite_model.py` & `modelaapi-0.6.102/modelaapi/graykite_model.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/modelaapi/ts.py` & `modelaapi-0.6.102/modelaapi/ts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/modelaapi/version.py` & `modelaapi-0.6.102/modelaapi/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
     "minor": 6,
-    "micro": 101,
+    "micro": 102,
     "releaselevel": "alpha",
     "post": 0,
     "serial": 1,
 }
 
 ##########################################################################
 ## Helper Functions
```

### Comparing `modelaapi-0.6.101/modelaapi.egg-info/PKG-INFO` & `modelaapi-0.6.102/modelaapi.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.101
+Version: 0.6.102
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.101
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.102
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.101
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.102
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.101/modelaapi.egg-info/SOURCES.txt` & `modelaapi-0.6.102/modelaapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/setup.cfg` & `modelaapi-0.6.102/setup.cfg`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.101/setup.py` & `modelaapi-0.6.102/setup.py`

 * *Files identical despite different names*

