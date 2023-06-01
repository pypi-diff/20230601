# Comparing `tmp/prosuite-1.1.0.0.tar.gz` & `tmp/prosuite-1.1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosuite-1.1.0.0.tar", last modified: Fri Apr 28 13:38:51 2023, max compression
+gzip compressed data, was "prosuite-1.1.1.0.tar", last modified: Sat May 27 21:45:22 2023, max compression
```

## Comparing `prosuite-1.1.0.0.tar` & `prosuite-1.1.1.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 13:38:51.542591 prosuite-1.1.0.0/
--rw-rw-rw-   0        0        0     1103 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1701 2023-04-28 13:38:51.542591 prosuite-1.1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1026 2023-02-24 14:29:45.000000 prosuite-1.1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 13:38:51.514593 prosuite-1.1.0.0/prosuite/
--rw-rw-rw-   0        0        0      959 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/__init__.py
--rw-rw-rw-   0        0        0      984 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/advanced_parameters.py
--rw-rw-rw-   0        0        0     4269 2023-04-12 17:32:29.000000 prosuite-1.1.0.0/prosuite/condition.py
--rw-rw-rw-   0        0        0     1109 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/dataset.py
-drwxrwxrwx   0        0        0        0 2023-04-28 13:38:51.526591 prosuite-1.1.0.0/prosuite/datatypes/
--rw-rw-rw-   0        0        0        0 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/datatypes/__init__.py
--rw-rw-rw-   0        0        0      160 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/datatypes/esri_geometry_type.py
--rw-rw-rw-   0        0        0      127 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/datatypes/expected_case.py
--rw-rw-rw-   0        0        0      117 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/datatypes/expected_string_difference.py
--rw-rw-rw-   0        0        0      208 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/datatypes/non_linear_segment_type.py
--rw-rw-rw-   0        0        0       98 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/datatypes/unique_strings_constraint.py
-drwxrwxrwx   0        0        0        0 2023-04-28 13:38:51.531592 prosuite-1.1.0.0/prosuite/factories/
--rw-rw-rw-   0        0        0        0 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/factories/__init__.py
--rw-rw-rw-   0        0        0     3540 2023-04-28 13:38:33.000000 prosuite-1.1.0.0/prosuite/factories/enums.py
--rw-rw-rw-   0        0        0      768 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/factories/issue_filters.py
--rw-rw-rw-   0        0        0   441467 2023-04-28 13:38:33.000000 prosuite-1.1.0.0/prosuite/factories/quality_conditions.py
--rw-rw-rw-   0        0        0      771 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/factories/transformers.py
-drwxrwxrwx   0        0        0        0 2023-04-28 13:38:51.541592 prosuite-1.1.0.0/prosuite/generated/
--rw-rw-rw-   0        0        0      454 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/generated/__init__.py
--rw-rw-rw-   0        0        0    21058 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/generated/quality_test_pb2.py
--rw-rw-rw-   0        0        0     2705 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/generated/quality_test_pb2_grpc.py
--rw-rw-rw-   0        0        0     7878 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/generated/quality_verification_service_pb2.py
--rw-rw-rw-   0        0        0     6983 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/generated/quality_verification_service_pb2_grpc.py
--rw-rw-rw-   0        0        0    21382 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/generated/shared_qa_pb2.py
--rw-rw-rw-   0        0        0    10649 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/generated/shared_types_pb2.py
--rw-rw-rw-   0        0        0      252 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/issue_filter.py
--rw-rw-rw-   0        0        0      496 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/model.py
--rw-rw-rw-   0        0        0     2146 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/parameter.py
--rw-rw-rw-   0        0        0      984 2023-04-12 17:32:29.000000 prosuite-1.1.0.0/prosuite/perimeter.py
--rw-rw-rw-   0        0        0    14618 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/service.py
--rw-rw-rw-   0        0        0      843 2023-04-28 12:31:16.000000 prosuite-1.1.0.0/prosuite/specification.py
--rw-rw-rw-   0        0        0      364 2023-04-28 13:27:29.000000 prosuite-1.1.0.0/prosuite/transformed_dataset.py
--rw-rw-rw-   0        0        0       92 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/transformer.py
--rw-rw-rw-   0        0        0     5321 2023-04-24 10:20:56.000000 prosuite-1.1.0.0/prosuite/utils.py
--rw-rw-rw-   0        0        0      489 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/verification_parameters.py
--rw-rw-rw-   0        0        0     2581 2023-01-20 23:17:38.000000 prosuite-1.1.0.0/prosuite/verification_response.py
--rw-rw-rw-   0        0        0     2543 2023-04-28 13:17:28.000000 prosuite-1.1.0.0/prosuite/xml_specification.py
-drwxrwxrwx   0        0        0        0 2023-04-28 13:38:51.519592 prosuite-1.1.0.0/prosuite.egg-info/
--rw-rw-rw-   0        0        0     1701 2023-04-28 13:38:51.000000 prosuite-1.1.0.0/prosuite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1338 2023-04-28 13:38:51.000000 prosuite-1.1.0.0/prosuite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 13:38:51.000000 prosuite-1.1.0.0/prosuite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-28 13:38:51.000000 prosuite-1.1.0.0/prosuite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-28 13:38:51.000000 prosuite-1.1.0.0/prosuite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2023-02-24 14:29:45.000000 prosuite-1.1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      925 2023-04-28 13:38:51.543592 prosuite-1.1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-02-24 14:29:45.000000 prosuite-1.1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 21:45:22.406787 prosuite-1.1.1.0/
+-rw-rw-rw-   0        0        0     1103 2023-01-20 23:17:38.000000 prosuite-1.1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1701 2023-05-27 21:45:22.406787 prosuite-1.1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1026 2023-02-24 14:29:45.000000 prosuite-1.1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 21:45:22.375788 prosuite-1.1.1.0/prosuite/
+-rw-rw-rw-   0        0        0      959 2023-04-28 13:27:29.000000 prosuite-1.1.1.0/prosuite/__init__.py
+-rw-rw-rw-   0        0        0      984 2023-01-20 23:17:38.000000 prosuite-1.1.1.0/prosuite/advanced_parameters.py
+-rw-rw-rw-   0        0        0     4269 2023-04-12 17:32:29.000000 prosuite-1.1.1.0/prosuite/condition.py
+-rw-rw-rw-   0        0        0     1109 2023-04-28 13:27:29.000000 prosuite-1.1.1.0/prosuite/dataset.py
+drwxrwxrwx   0        0        0        0 2023-05-27 21:45:22.389789 prosuite-1.1.1.0/prosuite/datatypes/
+-rw-rw-rw-   0        0        0        0 2023-01-20 23:17:38.000000 prosuite-1.1.1.0/prosuite/datatypes/__init__.py
+-rw-rw-rw-   0        0        0      160 2023-01-20 23:17:38.000000 prosuite-1.1.1.0/prosuite/datatypes/esri_geometry_type.py
+-rw-rw-rw-   0        0        0      127 2023-01-20 23:17:38.000000 prosuite-1.1.1.0/prosuite/datatypes/expected_case.py
+-rw-rw-rw-   0        0        0      117 2023-01-20 23:17:38.000000 prosuite-1.1.1.0/prosuite/datatypes/expected_string_difference.py
+-rw-rw-rw-   0        0        0      208 2023-01-20 23:17:38.000000 prosuite-1.1.1.0/prosuite/datatypes/non_linear_segment_type.py
+-rw-rw-rw-   0        0        0       98 2023-01-20 23:17:38.000000 prosuite-1.1.1.0/prosuite/datatypes/unique_strings_constraint.py
+drwxrwxrwx   0        0        0        0 2023-05-27 21:45:22.396786 prosuite-1.1.1.0/prosuite/factories/
+-rw-rw-rw-   0        0        0        0 2023-01-20 23:17:38.000000 prosuite-1.1.1.0/prosuite/factories/__init__.py
+-rw-rw-rw-   0        0        0     3790 2023-05-27 21:45:02.000000 prosuite-1.1.1.0/prosuite/factories/enums.py
+-rw-rw-rw-   0        0        0      768 2023-04-28 13:27:29.000000 prosuite-1.1.1.0/prosuite/factories/issue_filters.py
+-rw-rw-rw-   0        0        0   441467 2023-05-27 21:45:02.000000 prosuite-1.1.1.0/prosuite/factories/quality_conditions.py
+-rw-rw-rw-   0        0        0      771 2023-04-28 13:27:29.000000 prosuite-1.1.1.0/prosuite/factories/transformers.py
+drwxrwxrwx   0        0        0        0 2023-05-27 21:45:22.405787 prosuite-1.1.1.0/prosuite/generated/
+-rw-rw-rw-   0        0        0      454 2023-01-20 23:17:38.000000 prosuite-1.1.1.0/prosuite/generated/__init__.py
+-rw-rw-rw-   0        0        0     3578 2023-05-27 12:08:41.000000 prosuite-1.1.1.0/prosuite/generated/quality_test_pb2.py
+-rw-rw-rw-   0        0        0     2705 2023-05-27 12:08:41.000000 prosuite-1.1.1.0/prosuite/generated/quality_test_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5064 2023-05-27 12:08:41.000000 prosuite-1.1.1.0/prosuite/generated/quality_verification_service_pb2.py
+-rw-rw-rw-   0        0        0     6837 2023-05-12 18:55:15.000000 prosuite-1.1.1.0/prosuite/generated/quality_verification_service_pb2_grpc.py
+-rw-rw-rw-   0        0        0    12333 2023-05-27 12:08:41.000000 prosuite-1.1.1.0/prosuite/generated/shared_qa_pb2.py
+-rw-rw-rw-   0        0        0     5811 2023-05-27 12:08:41.000000 prosuite-1.1.1.0/prosuite/generated/shared_types_pb2.py
+-rw-rw-rw-   0        0        0      252 2023-01-20 23:17:38.000000 prosuite-1.1.1.0/prosuite/issue_filter.py
+-rw-rw-rw-   0        0        0      496 2023-04-28 13:27:29.000000 prosuite-1.1.1.0/prosuite/model.py
+-rw-rw-rw-   0        0        0     2146 2023-04-28 13:27:29.000000 prosuite-1.1.1.0/prosuite/parameter.py
+-rw-rw-rw-   0        0        0      984 2023-04-12 17:32:29.000000 prosuite-1.1.1.0/prosuite/perimeter.py
+-rw-rw-rw-   0        0        0    14618 2023-05-22 04:59:18.000000 prosuite-1.1.1.0/prosuite/service.py
+-rw-rw-rw-   0        0        0      843 2023-04-28 12:31:16.000000 prosuite-1.1.1.0/prosuite/specification.py
+-rw-rw-rw-   0        0        0      364 2023-04-28 13:27:29.000000 prosuite-1.1.1.0/prosuite/transformed_dataset.py
+-rw-rw-rw-   0        0        0       92 2023-01-20 23:17:38.000000 prosuite-1.1.1.0/prosuite/transformer.py
+-rw-rw-rw-   0        0        0     5321 2023-04-24 10:20:56.000000 prosuite-1.1.1.0/prosuite/utils.py
+-rw-rw-rw-   0        0        0      489 2023-01-20 23:17:38.000000 prosuite-1.1.1.0/prosuite/verification_parameters.py
+-rw-rw-rw-   0        0        0     2581 2023-01-20 23:17:38.000000 prosuite-1.1.1.0/prosuite/verification_response.py
+-rw-rw-rw-   0        0        0     2543 2023-04-28 13:17:28.000000 prosuite-1.1.1.0/prosuite/xml_specification.py
+drwxrwxrwx   0        0        0        0 2023-05-27 21:45:22.384787 prosuite-1.1.1.0/prosuite.egg-info/
+-rw-rw-rw-   0        0        0     1701 2023-05-27 21:45:22.000000 prosuite-1.1.1.0/prosuite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1338 2023-05-27 21:45:22.000000 prosuite-1.1.1.0/prosuite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 21:45:22.000000 prosuite-1.1.1.0/prosuite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-27 21:45:22.000000 prosuite-1.1.1.0/prosuite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 21:45:22.000000 prosuite-1.1.1.0/prosuite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2023-02-24 14:29:45.000000 prosuite-1.1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      925 2023-05-27 21:45:22.407789 prosuite-1.1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-02-24 14:29:45.000000 prosuite-1.1.1.0/setup.py
```

### Comparing `prosuite-1.1.0.0/LICENSE` & `prosuite-1.1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/PKG-INFO` & `prosuite-1.1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosuite
-Version: 1.1.0.0
+Version: 1.1.1.0
 Summary: An API to configure quality assurance tests for geodata and execute quality verifications on a ProSuite Server
 Home-page: https://dirageosystems.ch/prosuite/doc/api
 Author: Dira GeoSystems
 Author-email: programmers@dirageosystems.ch
 License: MIT
 Keywords: prosuite,gis,arcgis,geodata,spatial-data,quality,quality-assurance,qa,test
 Classifier: Operating System :: OS Independent
```

### Comparing `prosuite-1.1.0.0/README.md` & `prosuite-1.1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/prosuite/__init__.py` & `prosuite-1.1.1.0/prosuite/__init__.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/prosuite/advanced_parameters.py` & `prosuite-1.1.1.0/prosuite/advanced_parameters.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/prosuite/condition.py` & `prosuite-1.1.1.0/prosuite/condition.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/prosuite/dataset.py` & `prosuite-1.1.1.0/prosuite/dataset.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/prosuite/factories/enums.py` & `prosuite-1.1.1.0/prosuite/factories/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿__author__ = "The ProSuite Authors"
 __copyright__ = "Copyright 2021-2023, The ProSuite Authors"
 __license__ = "MIT"
-__version__ = "1.1.0.0"
+__version__ = "1.1.1.0"
 __maintainer__ = "Dira GeoSystems"
 __email__ = "programmers@dirageosystems.ch"
-__date__  = "28.04.2023"
+__date__  = "27.05.2023"
 __status__ = "Production"
 
 
 from datetime import datetime
 from typing import List
 
 
@@ -155,8 +155,21 @@
     IntersectionPoints = 1
 
 class JoinType(Enum):
     InnerJoin = 1
     LeftJoin = 2
     RightJoin = 3
 
+class ShapeAllowed(Enum):
+    NoValue = 0
+    Cycles = 1
+    Branches = 2
+    CyclesAndBranches = 3
+    InsideBranches = 4
+    All = 7
+
+class GroupErrorReporting(Enum):
+    ReferToFirstPart = 1
+    ShortestGaps = 2
+    CombineParts = 4
+
```

### Comparing `prosuite-1.1.0.0/prosuite/factories/issue_filters.py` & `prosuite-1.1.1.0/prosuite/factories/issue_filters.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/prosuite/factories/quality_conditions.py` & `prosuite-1.1.1.0/prosuite/factories/quality_conditions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿__author__ = "The ProSuite Authors"
 __copyright__ = "Copyright 2021-2023, The ProSuite Authors"
 __license__ = "MIT"
-__version__ = "1.1.0.0"
+__version__ = "1.1.1.0"
 __maintainer__ = "Dira GeoSystems"
 __email__ = "programmers@dirageosystems.ch"
-__date__  = "28.04.2023"
+__date__  = "27.05.2023"
 __status__ = "Production"
 
 
 from datetime import datetime
 from typing import List
 from prosuite.condition import Condition
 from prosuite.parameter import Parameter
```

### Comparing `prosuite-1.1.0.0/prosuite/factories/transformers.py` & `prosuite-1.1.1.0/prosuite/factories/transformers.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/prosuite/generated/quality_test_pb2_grpc.py` & `prosuite-1.1.1.0/prosuite/generated/quality_test_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 import quality_test_pb2 as quality__test__pb2
 
 
 class QualityTestGrpcStub(object):
@@ -13,15 +13,15 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Execute = channel.unary_stream(
-                '/prosuite.Microservices.Definitions.QA.Test.QualityTestGrpc/Execute',
+                '/ProSuite.Microservices.Definitions.QA.Test.QualityTestGrpc/Execute',
                 request_serializer=quality__test__pb2.ExecuteTestRequest.SerializeToString,
                 response_deserializer=quality__test__pb2.ExecuteTestResponse.FromString,
                 )
 
 
 class QualityTestGrpcServicer(object):
     """*
@@ -45,15 +45,15 @@
             'Execute': grpc.unary_stream_rpc_method_handler(
                     servicer.Execute,
                     request_deserializer=quality__test__pb2.ExecuteTestRequest.FromString,
                     response_serializer=quality__test__pb2.ExecuteTestResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'prosuite.Microservices.Definitions.QA.Test.QualityTestGrpc', rpc_method_handlers)
+            'ProSuite.Microservices.Definitions.QA.Test.QualityTestGrpc', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class QualityTestGrpc(object):
     """*
     The quality test definition.
@@ -66,12 +66,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/prosuite.Microservices.Definitions.QA.Test.QualityTestGrpc/Execute',
+        return grpc.experimental.unary_stream(request, target, '/ProSuite.Microservices.Definitions.QA.Test.QualityTestGrpc/Execute',
             quality__test__pb2.ExecuteTestRequest.SerializeToString,
             quality__test__pb2.ExecuteTestResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `prosuite-1.1.0.0/prosuite/generated/quality_verification_service_pb2_grpc.py` & `prosuite-1.1.1.0/prosuite/generated/quality_verification_service_pb2_grpc.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
-import quality_verification_service_pb2 as quality__verification__service__pb2
-
-
-class QualityVerificationGrpcStub(object):
-    """*
-    The quality verification service definition.
-    """
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.VerifyQuality = channel.unary_stream(
-                '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyQuality',
-                request_serializer=quality__verification__service__pb2.VerificationRequest.SerializeToString,
-                response_deserializer=quality__verification__service__pb2.VerificationResponse.FromString,
-                )
-        self.VerifyDataQuality = channel.stream_stream(
-                '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyDataQuality',
-                request_serializer=quality__verification__service__pb2.DataVerificationRequest.SerializeToString,
-                response_deserializer=quality__verification__service__pb2.DataVerificationResponse.FromString,
-                )
-        self.VerifyStandaloneXml = channel.unary_stream(
-                '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyStandaloneXml',
-                request_serializer=quality__verification__service__pb2.StandaloneVerificationRequest.SerializeToString,
-                response_deserializer=quality__verification__service__pb2.StandaloneVerificationResponse.FromString,
-                )
-
-
-class QualityVerificationGrpcServicer(object):
-    """*
-    The quality verification service definition.
-    """
-
-    def VerifyQuality(self, request, context):
-        """*
-        Verifies the quality definied in the data dictionary.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def VerifyDataQuality(self, request_iterator, context):
-        """*
-        Experimental - Verifies the data quality definied in the data dictionary. The data is provided by the client.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def VerifyStandaloneXml(self, request, context):
-        """*
-        Verifies the quality using an XML definition instead of accessing the data dictionary.
-        This is a simplified interface with a basic response and no parallelism. Consider using
-        VerifyQuality instead.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_QualityVerificationGrpcServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'VerifyQuality': grpc.unary_stream_rpc_method_handler(
-                    servicer.VerifyQuality,
-                    request_deserializer=quality__verification__service__pb2.VerificationRequest.FromString,
-                    response_serializer=quality__verification__service__pb2.VerificationResponse.SerializeToString,
-            ),
-            'VerifyDataQuality': grpc.stream_stream_rpc_method_handler(
-                    servicer.VerifyDataQuality,
-                    request_deserializer=quality__verification__service__pb2.DataVerificationRequest.FromString,
-                    response_serializer=quality__verification__service__pb2.DataVerificationResponse.SerializeToString,
-            ),
-            'VerifyStandaloneXml': grpc.unary_stream_rpc_method_handler(
-                    servicer.VerifyStandaloneXml,
-                    request_deserializer=quality__verification__service__pb2.StandaloneVerificationRequest.FromString,
-                    response_serializer=quality__verification__service__pb2.StandaloneVerificationResponse.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class QualityVerificationGrpc(object):
-    """*
-    The quality verification service definition.
-    """
-
-    @staticmethod
-    def VerifyQuality(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyQuality',
-            quality__verification__service__pb2.VerificationRequest.SerializeToString,
-            quality__verification__service__pb2.VerificationResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def VerifyDataQuality(request_iterator,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.stream_stream(request_iterator, target, '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyDataQuality',
-            quality__verification__service__pb2.DataVerificationRequest.SerializeToString,
-            quality__verification__service__pb2.DataVerificationResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def VerifyStandaloneXml(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyStandaloneXml',
-            quality__verification__service__pb2.StandaloneVerificationRequest.SerializeToString,
-            quality__verification__service__pb2.StandaloneVerificationResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
+import quality_verification_service_pb2 as quality__verification__service__pb2
+
+
+class QualityVerificationGrpcStub(object):
+    """*
+    The quality verification service definition.
+    """
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.VerifyQuality = channel.unary_stream(
+                '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyQuality',
+                request_serializer=quality__verification__service__pb2.VerificationRequest.SerializeToString,
+                response_deserializer=quality__verification__service__pb2.VerificationResponse.FromString,
+                )
+        self.VerifyDataQuality = channel.stream_stream(
+                '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyDataQuality',
+                request_serializer=quality__verification__service__pb2.DataVerificationRequest.SerializeToString,
+                response_deserializer=quality__verification__service__pb2.DataVerificationResponse.FromString,
+                )
+        self.VerifyStandaloneXml = channel.unary_stream(
+                '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyStandaloneXml',
+                request_serializer=quality__verification__service__pb2.StandaloneVerificationRequest.SerializeToString,
+                response_deserializer=quality__verification__service__pb2.StandaloneVerificationResponse.FromString,
+                )
+
+
+class QualityVerificationGrpcServicer(object):
+    """*
+    The quality verification service definition.
+    """
+
+    def VerifyQuality(self, request, context):
+        """*
+        Verifies the quality definied in the data dictionary.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def VerifyDataQuality(self, request_iterator, context):
+        """*
+        Experimental - Verifies the data quality definied in the data dictionary. The data is provided by the client.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def VerifyStandaloneXml(self, request, context):
+        """*
+        Verifies the quality using an XML definition instead of accessing the data dictionary.
+        This is a simplified interface with a basic response and no parallelism. Consider using
+        VerifyQuality instead.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_QualityVerificationGrpcServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'VerifyQuality': grpc.unary_stream_rpc_method_handler(
+                    servicer.VerifyQuality,
+                    request_deserializer=quality__verification__service__pb2.VerificationRequest.FromString,
+                    response_serializer=quality__verification__service__pb2.VerificationResponse.SerializeToString,
+            ),
+            'VerifyDataQuality': grpc.stream_stream_rpc_method_handler(
+                    servicer.VerifyDataQuality,
+                    request_deserializer=quality__verification__service__pb2.DataVerificationRequest.FromString,
+                    response_serializer=quality__verification__service__pb2.DataVerificationResponse.SerializeToString,
+            ),
+            'VerifyStandaloneXml': grpc.unary_stream_rpc_method_handler(
+                    servicer.VerifyStandaloneXml,
+                    request_deserializer=quality__verification__service__pb2.StandaloneVerificationRequest.FromString,
+                    response_serializer=quality__verification__service__pb2.StandaloneVerificationResponse.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class QualityVerificationGrpc(object):
+    """*
+    The quality verification service definition.
+    """
+
+    @staticmethod
+    def VerifyQuality(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyQuality',
+            quality__verification__service__pb2.VerificationRequest.SerializeToString,
+            quality__verification__service__pb2.VerificationResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def VerifyDataQuality(request_iterator,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.stream_stream(request_iterator, target, '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyDataQuality',
+            quality__verification__service__pb2.DataVerificationRequest.SerializeToString,
+            quality__verification__service__pb2.DataVerificationResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def VerifyStandaloneXml(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyStandaloneXml',
+            quality__verification__service__pb2.StandaloneVerificationRequest.SerializeToString,
+            quality__verification__service__pb2.StandaloneVerificationResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `prosuite-1.1.0.0/prosuite/parameter.py` & `prosuite-1.1.1.0/prosuite/parameter.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/prosuite/perimeter.py` & `prosuite-1.1.1.0/prosuite/perimeter.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/prosuite/service.py` & `prosuite-1.1.1.0/prosuite/service.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/prosuite/specification.py` & `prosuite-1.1.1.0/prosuite/specification.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/prosuite/utils.py` & `prosuite-1.1.1.0/prosuite/utils.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/prosuite/verification_response.py` & `prosuite-1.1.1.0/prosuite/verification_response.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/prosuite/xml_specification.py` & `prosuite-1.1.1.0/prosuite/xml_specification.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/prosuite.egg-info/PKG-INFO` & `prosuite-1.1.1.0/prosuite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosuite
-Version: 1.1.0.0
+Version: 1.1.1.0
 Summary: An API to configure quality assurance tests for geodata and execute quality verifications on a ProSuite Server
 Home-page: https://dirageosystems.ch/prosuite/doc/api
 Author: Dira GeoSystems
 Author-email: programmers@dirageosystems.ch
 License: MIT
 Keywords: prosuite,gis,arcgis,geodata,spatial-data,quality,quality-assurance,qa,test
 Classifier: Operating System :: OS Independent
```

### Comparing `prosuite-1.1.0.0/prosuite.egg-info/SOURCES.txt` & `prosuite-1.1.1.0/prosuite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosuite-1.1.0.0/setup.cfg` & `prosuite-1.1.1.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 00000160: 726b 646f 776e 0d0a 6b65 7977 6f72 6473  rkdown..keywords
 00000170: 203d 2070 726f 7375 6974 652c 2067 6973   = prosuite, gis
 00000180: 2c20 6172 6367 6973 2c20 6765 6f64 6174  , arcgis, geodat
 00000190: 612c 2073 7061 7469 616c 2d64 6174 612c  a, spatial-data,
 000001a0: 2071 7561 6c69 7479 2c20 7175 616c 6974   quality, qualit
 000001b0: 792d 6173 7375 7261 6e63 652c 2071 612c  y-assurance, qa,
 000001c0: 2074 6573 740d 0a76 6572 7369 6f6e 203d   test..version =
-000001d0: 2031 2e31 2e30 2e30 0d0a 6c69 6365 6e73   1.1.0.0..licens
+000001d0: 2031 2e31 2e31 2e30 0d0a 6c69 6365 6e73   1.1.1.0..licens
 000001e0: 6520 3d20 4d49 540d 0a6c 6963 656e 7365  e = MIT..license
 000001f0: 5f66 696c 6573 203d 204c 4943 454e 5345  _files = LICENSE
 00000200: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
 00000210: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
 00000220: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
 00000230: 6e64 656e 740d 0a09 5072 6f67 7261 6d6d  ndent...Programm
 00000240: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language ::
```

