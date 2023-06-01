# Comparing `tmp/quantum_serverless-0.1.0.tar.gz` & `tmp/quantum_serverless-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantum_serverless-0.1.0.tar", last modified: Wed May 17 19:21:48 2023, max compression
+gzip compressed data, was "quantum_serverless-0.1.1.tar", last modified: Thu Jun  1 20:52:51 2023, max compression
```

## Comparing `quantum_serverless-0.1.0.tar` & `quantum_serverless-0.1.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:48.714468 quantum_serverless-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-17 19:21:48.714468 quantum_serverless-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:48.710468 quantum_serverless-0.1.0/quantum_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:48.714468 quantum_serverless-0.1.0/quantum_serverless/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/core/program.py
--rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/core/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:48.714468 quantum_serverless-0.1.0/quantum_serverless/library/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/library/transpiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/quantum_serverless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:48.714468 quantum_serverless-0.1.0/quantum_serverless/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/serializers/program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/serializers/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:48.714468 quantum_serverless-0.1.0/quantum_serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/quantum_serverless/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:48.714468 quantum_serverless-0.1.0/quantum_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-17 19:21:48.000000 quantum_serverless-0.1.0/quantum_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-17 19:21:48.000000 quantum_serverless-0.1.0/quantum_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:21:48.000000 quantum_serverless-0.1.0/quantum_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-17 19:21:48.000000 quantum_serverless-0.1.0/quantum_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 19:21:48.000000 quantum_serverless-0.1.0/quantum_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-17 19:21:48.714468 quantum_serverless-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:48.714468 quantum_serverless-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:48.714468 quantum_serverless-0.1.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/tests/core/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/tests/core/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/tests/core/test_program_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/tests/core/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:48.714468 quantum_serverless-0.1.0/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/tests/library/test_transpiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:48.714468 quantum_serverless-0.1.0/tests/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/tests/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/tests/serializers/test_program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/tests/serializers/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/tests/test_quantum_serverless.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-17 19:21:41.000000 quantum_serverless-0.1.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.947531 quantum_serverless-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-01 20:52:51.947531 quantum_serverless-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/quantum_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/quantum_serverless/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/quantum_serverless/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/library/transpiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/quantum_serverless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/quantum_serverless/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/serializers/program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/serializers/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/quantum_serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/utils/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/quantum_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-01 20:52:51.000000 quantum_serverless-0.1.1/quantum_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-01 20:52:51.000000 quantum_serverless-0.1.1/quantum_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:52:51.000000 quantum_serverless-0.1.1/quantum_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-01 20:52:51.000000 quantum_serverless-0.1.1/quantum_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 20:52:51.000000 quantum_serverless-0.1.1/quantum_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 20:52:51.947531 quantum_serverless-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/core/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/core/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/core/test_program_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/core/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/library/test_transpiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.947531 quantum_serverless-0.1.1/tests/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/serializers/test_program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/serializers/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/test_quantum_serverless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/utils.py
```

### Comparing `quantum_serverless-0.1.0/PKG-INFO` & `quantum_serverless-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum_serverless
-Version: 0.1.0
+Version: 0.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -114,15 +114,15 @@
    circuits = []
    for _ in range(3):
        circuit = random_circuit(3, 2)
        circuit.measure_all()
        circuits.append(circuit)
 
    # run program
-   job = serverless.run_program(
+   job = serverless.run(
        program=program,
        arguments={
            "circuits": circuits
        }
    )
 ```
```

### Comparing `quantum_serverless-0.1.0/README.md` & `quantum_serverless-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
    circuits = []
    for _ in range(3):
        circuit = random_circuit(3, 2)
        circuit.measure_all()
        circuits.append(circuit)
 
    # run program
-   job = serverless.run_program(
+   job = serverless.run(
        program=program,
        arguments={
            "circuits": circuits
        }
    )
 ```
```

### Comparing `quantum_serverless-0.1.0/quantum_serverless/__init__.py` & `quantum_serverless-0.1.1/quantum_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/core/__init__.py` & `quantum_serverless-0.1.1/quantum_serverless/core/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/core/constants.py` & `quantum_serverless-0.1.1/quantum_serverless/core/constants.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/core/decorators.py` & `quantum_serverless-0.1.1/quantum_serverless/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/core/events.py` & `quantum_serverless-0.1.1/quantum_serverless/core/events.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/core/job.py` & `quantum_serverless-0.1.1/quantum_serverless/core/job.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,16 +27,18 @@
     RuntimeEnv
     Job
 """
 import json
 import logging
 import os
 import tarfile
+import time
 from typing import Dict, Any, Optional, List
 from uuid import uuid4
+import warnings
 
 import ray.runtime_env
 import requests
 from ray.dashboard.modules.job.sdk import JobSubmissionClient
 
 from quantum_serverless.core.constants import (
     OT_PROGRAM_NAME,
@@ -59,14 +61,20 @@
 
     def run_program(
         self, program: Program, arguments: Optional[Dict[str, Any]] = None
     ) -> "Job":
         """Runs program."""
         raise NotImplementedError
 
+    def run(
+        self, program: Program, arguments: Optional[Dict[str, Any]] = None
+    ) -> "Job":
+        """Runs program."""
+        raise NotImplementedError
+
     def get(self, job_id) -> Optional["Job"]:
         """Returns job by job id"""
         raise NotImplementedError
 
     def list(self, **kwargs) -> List["Job"]:
         """Returns list of jobs."""
         raise NotImplementedError
@@ -117,14 +125,49 @@
 
     def list(self, **kwargs) -> List["Job"]:
         return [
             Job(job.job_id, job_client=self) for job in self._job_client.list_jobs()
         ]
 
     def run_program(self, program: Program, arguments: Optional[Dict[str, Any]] = None):
+        warnings.warn(
+            "`run_program` is deprecated. Please, consider using `run` instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        arguments = arguments or {}
+        arguments_string = ""
+        if program.arguments is not None:
+            arg_list = []
+            for key, value in arguments.items():
+                if isinstance(value, dict):
+                    arg_list.append(f"--{key}='{json.dumps(value)}'")
+                else:
+                    arg_list.append(f"--{key}={value}")
+            arguments_string = " ".join(arg_list)
+        entrypoint = f"python {program.entrypoint} {arguments_string}"
+
+        # set program name so OT can use it as parent span name
+        env_vars = {
+            **(program.env_vars or {}),
+            **{OT_PROGRAM_NAME: program.title},
+        }
+
+        job_id = self._job_client.submit_job(
+            entrypoint=entrypoint,
+            submission_id=f"qs_{uuid4()}",
+            runtime_env={
+                "working_dir": program.working_dir,
+                "pip": program.dependencies,
+                "env_vars": env_vars,
+            },
+        )
+        return Job(job_id=job_id, job_client=self)
+
+    def run(self, program: Program, arguments: Optional[Dict[str, Any]] = None):
         arguments = arguments or {}
         arguments_string = ""
         if program.arguments is not None:
             arg_list = []
             for key, value in arguments.items():
                 if isinstance(value, dict):
                     arg_list.append(f"--{key}='{json.dumps(value)}'")
@@ -165,14 +208,54 @@
         self.host = host
         self.version = version
         self._token = token
 
     def run_program(  # pylint: disable=too-many-locals
         self, program: Program, arguments: Optional[Dict[str, Any]] = None
     ) -> "Job":
+        warnings.warn(
+            "`run_program` is deprecated. Please, consider using `run` instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        url = f"{self.host}/api/{self.version}/programs/run/"
+        artifact_file_path = os.path.join(program.working_dir, "artifact.tar")
+
+        with tarfile.open(artifact_file_path, "w") as tar:
+            for filename in os.listdir(program.working_dir):
+                fpath = os.path.join(program.working_dir, filename)
+                tar.add(fpath, arcname=filename)
+
+        with open(artifact_file_path, "rb") as file:
+            response_data = safe_json_request(
+                request=lambda: requests.post(
+                    url=url,
+                    data={
+                        "title": program.title,
+                        "entrypoint": program.entrypoint,
+                        "arguments": json.dumps(
+                            arguments or {}, cls=QiskitObjectsEncoder
+                        ),
+                        "dependencies": json.dumps(program.dependencies or []),
+                    },
+                    files={"artifact": file},
+                    headers={"Authorization": f"Bearer {self._token}"},
+                    timeout=REQUESTS_TIMEOUT,
+                )
+            )
+            job_id = response_data.get("id")
+
+        if os.path.exists(artifact_file_path):
+            os.remove(artifact_file_path)
+
+        return Job(job_id, job_client=self)
+
+    def run(  # pylint: disable=too-many-locals
+        self, program: Program, arguments: Optional[Dict[str, Any]] = None
+    ) -> "Job":
         url = f"{self.host}/api/{self.version}/programs/run/"
         artifact_file_path = os.path.join(program.working_dir, "artifact.tar")
 
         with tarfile.open(artifact_file_path, "w") as tar:
             for filename in os.listdir(program.working_dir):
                 fpath = os.path.join(program.working_dir, filename)
                 tar.add(fpath, arcname=filename)
@@ -299,18 +382,38 @@
         """Stops the job from running."""
         return self._job_client.stop(self.job_id)
 
     def logs(self) -> str:
         """Returns logs of the job."""
         return self._job_client.logs(self.job_id)
 
-    def result(self):
-        """Return results of the job."""
+    def result(self, wait=True, cadence=5, verbose=False):
+        """Return results of the job.
+        Args:
+            wait: flag denoting whether to wait for the
+                job result to be populated before returning
+            cadence: time to wait between checking if job has
+                been terminated
+            verbose: flag denoting whether to log a heartbeat
+                while waiting for job result to populate
+        """
+        if wait:
+            if verbose:
+                logging.info("Waiting for job result.")
+            while not self._in_terminal_state():
+                time.sleep(cadence)
+                if verbose:
+                    logging.info(".")
         return self._job_client.result(self.job_id)
 
+    def _in_terminal_state(self) -> bool:
+        """Checks if job is in terminal state"""
+        terminal_states = ["STOPPED", "SUCCEEDED", "FAILED"]
+        return self.status() in terminal_states
+
     def __repr__(self):
         return f"<Job | {self.job_id}>"
 
 
 def save_result(result: Dict[str, Any]):
     """Saves job results."""
```

### Comparing `quantum_serverless-0.1.0/quantum_serverless/core/program.py` & `quantum_serverless-0.1.1/quantum_serverless/core/program.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         return Program(**{k: v for k, v in data.items() if k in field_names})
 
     def __post_init__(self):
         if self.arguments is not None:
             warnings.warn(
                 "Passing `arguments` as constructor argument to `Program` is deprecated "
                 "and will be removed in v0.2. "
-                "Please, consider passing `arguments` to `run_program` "
+                "Please, consider passing `arguments` to `run` "
                 "method of `QuantumServerless` object.",
                 DeprecationWarning,
                 stacklevel=2,
             )
 
 
 class ProgramStorage(ABC):
```

### Comparing `quantum_serverless-0.1.0/quantum_serverless/core/provider.py` & `quantum_serverless-0.1.1/quantum_serverless/core/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     ComputeResource
     Provider
 """
 import logging
 import os.path
 from dataclasses import dataclass
 from typing import Optional, List, Dict, Any
+import warnings
 
 import ray
 import requests
 from ray.dashboard.modules.job.sdk import JobSubmissionClient
 
 from quantum_serverless.core.constants import (
     RAY_IMAGE,
@@ -250,15 +251,15 @@
             )
             return None
         return Job(job_id=job_id, job_client=job_client)
 
     def run_program(
         self, program: Program, arguments: Optional[Dict[str, Any]] = None
     ) -> Job:
-        """Execute a program as a async job.
+        """(Deprecated) Execute a program as a async job.
 
         Example:
             >>> serverless = QuantumServerless()
             >>> program = Program(
             >>>     "job.py",
             >>>     arguments={"arg1": "val1"},
             >>>     dependencies=["requests"]
@@ -269,26 +270,63 @@
         Args:
             arguments: arguments to run program with
             program: Program object
 
         Returns:
             Job
         """
+        warnings.warn(
+            "`run_program` is deprecated. Please, consider using `run` instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         job_client = self.job_client()
 
         if job_client is None:
             logging.warning(  # pylint: disable=logging-fstring-interpolation
                 f"Job has not been submitted as no provider "
                 f"with remote host has been configured. "
                 f"Selected provider: {self}"
             )
             return None
 
         return job_client.run_program(program, arguments)
 
+    def run(self, program: Program, arguments: Optional[Dict[str, Any]] = None) -> Job:
+        """Execute a program as a async job.
+
+        Example:
+            >>> serverless = QuantumServerless()
+            >>> program = Program(
+            >>>     "job.py",
+            >>>     arguments={"arg1": "val1"},
+            >>>     dependencies=["requests"]
+            >>> )
+            >>> job = serverless.run(program)
+            >>> # <Job | ...>
+
+        Args:
+            arguments: arguments to run program with
+            program: Program object
+
+        Returns:
+            Job
+        """
+        job_client = self.job_client()
+
+        if job_client is None:
+            logging.warning(  # pylint: disable=logging-fstring-interpolation
+                f"Job has not been submitted as no provider "
+                f"with remote host has been configured. "
+                f"Selected provider: {self}"
+            )
+            return None
+
+        return job_client.run(program, arguments)
+
 
 class KuberayProvider(Provider):
     """Implements CRUD for Kuberay API server."""
 
     def __init__(
         self,
         name: str,
@@ -533,16 +571,24 @@
 
     def get_job_by_id(self, job_id: str) -> Optional[Job]:
         return self._job_client.get(job_id)
 
     def run_program(
         self, program: Program, arguments: Optional[Dict[str, Any]] = None
     ) -> Job:
+        warnings.warn(
+            "`run_program` is deprecated. Please, consider using `run` instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         return self._job_client.run_program(program, arguments)
 
+    def run(self, program: Program, arguments: Optional[Dict[str, Any]] = None) -> Job:
+        return self._job_client.run(program, arguments)
+
     def get_jobs(self, **kwargs) -> List[Job]:
         return self._job_client.list(**kwargs)
 
     def _fetch_token(self, username: str, password: str):
         response_data = safe_json_request(
             request=lambda: requests.post(
                 url=f"{self.host}/dj-rest-auth/keycloak/login/",
```

### Comparing `quantum_serverless-0.1.0/quantum_serverless/core/state.py` & `quantum_serverless-0.1.1/quantum_serverless/core/state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/core/tracing.py` & `quantum_serverless-0.1.1/quantum_serverless/core/tracing.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/exception.py` & `quantum_serverless-0.1.1/quantum_serverless/exception.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/library/__init__.py` & `quantum_serverless-0.1.1/quantum_serverless/library/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/library/transpiler.py` & `quantum_serverless-0.1.1/quantum_serverless/library/transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/quantum_serverless.py` & `quantum_serverless-0.1.1/quantum_serverless/quantum_serverless.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     def job_client(self):
         """Job client for given provider."""
         return self._selected_provider.job_client()
 
     def run_program(
         self, program: Program, arguments: Optional[Dict[str, Any]] = None
     ) -> Optional[Job]:
-        """Execute a program as a async job
+        """(Deprecated) Execute a program as a async job
 
         Example:
             >>> serverless = QuantumServerless()
             >>> program = Program(
             >>>     "job.py",
             >>>     dependencies=["requests"]
             >>> )
@@ -102,18 +102,48 @@
         Args:
             arguments: arguments to run program with
             program: Program object
 
         Returns:
             Job
         """
+        warnings.warn(
+            "`run_program` is deprecated. Please, consider using `run` instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         if program.arguments is not None:
             arguments = program.arguments
         return self._selected_provider.run_program(program, arguments)
 
+    def run(
+        self, program: Program, arguments: Optional[Dict[str, Any]] = None
+    ) -> Optional[Job]:
+        """Execute a program as a async job
+
+        Example:
+            >>> serverless = QuantumServerless()
+            >>> program = Program(
+            >>>     "job.py",
+            >>>     dependencies=["requests"]
+            >>> )
+            >>> job = serverless.run(program, {"arg1": 1})
+            >>> # <Job | ...>
+
+        Args:
+            arguments: arguments to run program with
+            program: Program object
+
+        Returns:
+            Job
+        """
+        if program.arguments is not None:
+            arguments = program.arguments
+        return self._selected_provider.run(program, arguments)
+
     def get_job_by_id(self, job_id: str) -> Optional[Job]:
         """Returns job by job id.
 
         Args:
             job_id: job id
 
         Returns:
```

### Comparing `quantum_serverless-0.1.0/quantum_serverless/serializers/__init__.py` & `quantum_serverless-0.1.1/quantum_serverless/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/serializers/program_serializers.py` & `quantum_serverless-0.1.1/quantum_serverless/serializers/program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/serializers/serializers.py` & `quantum_serverless-0.1.1/quantum_serverless/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/utils/__init__.py` & `quantum_serverless-0.1.1/quantum_serverless/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/utils/errors.py` & `quantum_serverless-0.1.1/quantum_serverless/utils/errors.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless/utils/json.py` & `quantum_serverless-0.1.1/quantum_serverless/utils/json.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/quantum_serverless.egg-info/PKG-INFO` & `quantum_serverless-0.1.1/quantum_serverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum-serverless
-Version: 0.1.0
+Version: 0.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -114,15 +114,15 @@
    circuits = []
    for _ in range(3):
        circuit = random_circuit(3, 2)
        circuit.measure_all()
        circuits.append(circuit)
 
    # run program
-   job = serverless.run_program(
+   job = serverless.run(
        program=program,
        arguments={
            "circuits": circuits
        }
    )
 ```
```

### Comparing `quantum_serverless-0.1.0/quantum_serverless.egg-info/SOURCES.txt` & `quantum_serverless-0.1.1/quantum_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/setup.py` & `quantum_serverless-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/tests/core/test_decorator.py` & `quantum_serverless-0.1.1/tests/core/test_decorator.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/tests/core/test_program.py` & `quantum_serverless-0.1.1/tests/core/test_program.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             title="simple_job",
             entrypoint="job.py",
             working_dir=resources_path,
             description="description",
             version="0.0.1",
         )
 
-        job = serverless.run_program(program)
+        job = serverless.run(program)
 
         assert isinstance(job, Job)
 
         wait_for_job_completion(job)
 
         assert "42" in job.logs()
         assert job.status().is_terminal()
```

### Comparing `quantum_serverless-0.1.0/tests/core/test_program_repository.py` & `quantum_serverless-0.1.1/tests/core/test_program_repository.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/tests/core/test_state.py` & `quantum_serverless-0.1.1/tests/core/test_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 name="test_docker", host=host, port_job_server=port
             ),
         )
         serverless = QuantumServerless(provider).set_provider("test_docker")
 
         wait_for_job_client(serverless)
 
-        job = serverless.run_program(
+        job = serverless.run(
             Program("test", entrypoint="job_with_state.py", working_dir=resources_path)
         )
 
         wait_for_job_completion(job)
 
         assert "42" in job.logs()
         assert job.status().is_terminal()
```

### Comparing `quantum_serverless-0.1.0/tests/library/test_transpiler.py` & `quantum_serverless-0.1.1/tests/library/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/tests/serializers/test_program_serializers.py` & `quantum_serverless-0.1.1/tests/serializers/test_program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/tests/serializers/test_serializers.py` & `quantum_serverless-0.1.1/tests/serializers/test_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/tests/test_quantum_serverless.py` & `quantum_serverless-0.1.1/tests/test_quantum_serverless.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.0/tests/utils.py` & `quantum_serverless-0.1.1/tests/utils.py`

 * *Files identical despite different names*

