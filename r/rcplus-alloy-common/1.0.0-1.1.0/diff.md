# Comparing `tmp/rcplus_alloy_common-1.0.0.tar.gz` & `tmp/rcplus_alloy_common-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcplus_alloy_common-1.0.0.tar", max compression
+gzip compressed data, was "rcplus_alloy_common-1.1.0.tar", max compression
```

## Comparing `rcplus_alloy_common-1.0.0.tar` & `rcplus_alloy_common-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       77 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/LICENSE
--rw-r--r--   0        0        0      571 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/README.md
--rw-r--r--   0        0        0     1930 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2881 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/__init__.py
--rw-r--r--   0        0        0      581 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/__init__.py
--rw-r--r--   0        0        0     1182 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/dag.py
--rw-r--r--   0        0        0     1655 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/decorators.py
--rw-r--r--   0        0        0     7448 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/observability.py
--rw-r--r--   0        0        0     9867 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/operators.py
--rw-r--r--   0        0        0     2611 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/sensors.py
--rw-r--r--   0        0        0     2009 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/utils.py
--rw-r--r--   0        0        0     2279 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/constants.py
--rw-r--r--   0        0        0     3866 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/logging.py
--rw-r--r--   0        0        0     6388 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/metrics.py
--rw-r--r--   0        0        0     3925 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/retry.py
--rw-r--r--   0        0        0       19 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/version.py
--rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 rcplus_alloy_common-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       77 2023-05-31 23:19:44.177259 rcplus_alloy_common-1.1.0/LICENSE
+-rw-r--r--   0        0        0      571 2023-05-31 23:19:44.177259 rcplus_alloy_common-1.1.0/README.md
+-rw-r--r--   0        0        0     1930 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2881 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/__init__.py
+-rw-r--r--   0        0        0      567 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/__init__.py
+-rw-r--r--   0        0        0     1179 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/dag.py
+-rw-r--r--   0        0        0     1652 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/decorators.py
+-rw-r--r--   0        0        0     7448 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/observability.py
+-rw-r--r--   0        0        0    10104 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/operators.py
+-rw-r--r--   0        0        0     2611 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/sensors.py
+-rw-r--r--   0        0        0     2799 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/utils.py
+-rw-r--r--   0        0        0     2279 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/constants.py
+-rw-r--r--   0        0        0     3866 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/logging.py
+-rw-r--r--   0        0        0     6388 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/metrics.py
+-rw-r--r--   0        0        0     3925 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/retry.py
+-rw-r--r--   0        0        0       19 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/version.py
+-rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 rcplus_alloy_common-1.1.0/PKG-INFO
```

### Comparing `rcplus_alloy_common-1.0.0/README.md` & `rcplus_alloy_common-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v1.0.0**
+Current version: **v1.1.0**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

### Comparing `rcplus_alloy_common-1.0.0/pyproject.toml` & `rcplus_alloy_common-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 
 [tool.poetry]
 name = "rcplus_alloy_common"
-version = "1.0.0"
+version = "1.1.0"
 description = "RC+/Alloy helpers functions for Python"
 readme = "README.md"
 authors = [
     "Ringier AG <info@rcplus.io>",
 ]
 license = "Proprietary"
 repository = "https://github.com/ringier-data/rcplus-alloy-lib-py-common"
```

### Comparing `rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/__init__.py` & `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/__init__.py` & `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from rcplus_alloy_common.airflow.utils import load_project_config
+from rcplus_alloy_common.airflow.utils import AlloyProject
 from rcplus_alloy_common.airflow.dag import AlloyDag
 from rcplus_alloy_common.airflow.decorators import alloyize
 from rcplus_alloy_common.airflow.operators import (
     AlloyBashOperator, AlloyPythonOperator, AlloyGlueJobOperator, AlloyEcsRunTaskOperator
 )
 from rcplus_alloy_common.airflow.sensors import AlloySqsSensor
 
 
 __all__ = [
-    "load_project_config",
+    "AlloyProject",
     "AlloyDag",
     "alloyize",
     "AlloyBashOperator", "AlloyPythonOperator", "AlloyGlueJobOperator", "AlloyEcsRunTaskOperator",
     "AlloySqsSensor"
 ]
```

### Comparing `rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/dag.py` & `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/dag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from airflow.models.dag import DAG
 
 from rcplus_alloy_common.version import head_ref
-from rcplus_alloy_common.airflow.utils import load_project_config
+from rcplus_alloy_common.airflow.utils import AlloyProject
 
 
 class AlloyDag(DAG):
     """Alloy DAG class which enforces tags and dag_id naming convention."""
 
     def __init__(self, dag_id, *args, tags=None, **kwargs):
-        project = load_project_config(2)  # load_project_config, __init__, dag_fun
+        project = AlloyProject(3)  # __init__, _load_project_config, __init__, dag_fun
         dag_id_prefix = f"{project['project_id']}-{project['software_component']}"
         if not dag_id.startswith(dag_id_prefix):
             dag_id = f"{dag_id_prefix}-{dag_id}"
 
         if tags is None:
             tags = []
         if project["git_repo_name"] not in tags:
```

### Comparing `rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/decorators.py` & `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/decorators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from airflow.datasets import Dataset
 
 from rcplus_alloy_common.version import head_ref
-from rcplus_alloy_common.airflow.utils import set_default_callbacks, load_project_config
+from rcplus_alloy_common.airflow.utils import set_default_callbacks, AlloyProject
 
 
 def alloyize(cls):
     """Alloyize a BaseOperator or BaseSensor with default Alloy arguments.
 
     Usage:
         ```
@@ -28,15 +28,15 @@
 
         # add default outlet if not already added
         dag_id = self.get_dag().dag_id
         dataset_uri = f"{dag_id}-{self.task_id}"
         outlets = any(
             True for outlet in self.get_outlet_defs() if isinstance(outlet, Dataset) and Dataset.uri == dataset_uri
         )
-        self.project = load_project_config(3)  # load_project_config, new_init, apply_defaults, dag_fun
+        self.project = AlloyProject(4)  # __init__, _load_project_config, new_init, apply_defaults, dag_fun
         if not outlets:
             self.add_outlets([Dataset(dataset_uri)])
 
     def new_execute(self, *args, **kwargs):
         self.log.info(f"Running task `{self.task_id}` of dag `{self.dag_id}` with `rcplus_alloy_common@{head_ref}`")
         return orig_execute(self, *args, **kwargs)
```

### Comparing `rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/observability.py` & `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/observability.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/operators.py` & `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/operators.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from airflow.models import Variable, BaseOperator
 from airflow.exceptions import AirflowException
 from airflow.operators.bash import BashOperator
 from airflow.operators.python import PythonOperator
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 from airflow.providers.amazon.aws.operators.ecs import EcsRunTaskOperator
 from airflow.providers.amazon.aws.operators.glue import GlueJobOperator
+from airflow.providers.amazon.aws.operators.athena import AthenaOperator
 
 from rcplus_alloy_common.airflow.decorators import alloyize
 
 
 @alloyize
 class AlloyBashOperator(BashOperator):
     """Alloy BashOperator"""
@@ -226,7 +227,13 @@
             f"The lock `{self.lock_key}` not released because its lock id is `{lock_id}` but expected `{self.lock_id}`"
         )
 
 
 @alloyize
 class AlloyS3ReleaseLockOperator(S3ReleaseLockOperator):
     """Alloy S3ReleaseLockOperator"""
+
+
+@alloyize
+class AlloyAthenaOperator(AthenaOperator):
+    """Alloy AthenaOperator"""
+    template_fields = tuple(AthenaOperator.template_fields) + ("workgroup", )
```

### Comparing `rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/sensors.py` & `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/sensors.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/constants.py` & `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/constants.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/logging.py` & `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/logging.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/metrics.py` & `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/metrics.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/retry.py` & `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/retry.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.0.0/PKG-INFO` & `rcplus_alloy_common-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcplus-alloy-common
-Version: 1.0.0
+Version: 1.1.0
 Summary: RC+/Alloy helpers functions for Python
 Home-page: https://github.com/ringier-data/rcplus-alloy-lib-py-common
 License: Proprietary
 Keywords: rcplus,alloy,logging,metrics,utilities
 Author: Ringier AG
 Author-email: info@rcplus.io
 Requires-Python: >=3.10,<4
@@ -29,15 +29,15 @@
 
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v1.0.0**
+Current version: **v1.1.0**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

