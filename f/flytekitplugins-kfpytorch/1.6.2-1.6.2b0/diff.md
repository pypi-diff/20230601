# Comparing `tmp/flytekitplugins-kfpytorch-1.6.2.tar.gz` & `tmp/flytekitplugins-kfpytorch-1.6.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfpytorch-1.6.2.tar", last modified: Tue May 30 15:24:18 2023, max compression
+gzip compressed data, was "flytekitplugins-kfpytorch-1.6.2b0.tar", last modified: Thu Jun  1 20:41:56 2023, max compression
```

## Comparing `flytekitplugins-kfpytorch-1.6.2.tar` & `flytekitplugins-kfpytorch-1.6.2b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:18.161497 flytekitplugins-kfpytorch-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-30 15:24:18.161497 flytekitplugins-kfpytorch-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-30 15:23:56.000000 flytekitplugins-kfpytorch-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:18.161497 flytekitplugins-kfpytorch-1.6.2/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:18.161497 flytekitplugins-kfpytorch-1.6.2/flytekitplugins/kfpytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-30 15:23:56.000000 flytekitplugins-kfpytorch-1.6.2/flytekitplugins/kfpytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-05-30 15:23:56.000000 flytekitplugins-kfpytorch-1.6.2/flytekitplugins/kfpytorch/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:18.161497 flytekitplugins-kfpytorch-1.6.2/flytekitplugins_kfpytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-30 15:24:18.000000 flytekitplugins-kfpytorch-1.6.2/flytekitplugins_kfpytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-30 15:24:18.000000 flytekitplugins-kfpytorch-1.6.2/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:24:18.000000 flytekitplugins-kfpytorch-1.6.2/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 15:24:18.000000 flytekitplugins-kfpytorch-1.6.2/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-30 15:24:18.000000 flytekitplugins-kfpytorch-1.6.2/flytekitplugins_kfpytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 15:24:18.000000 flytekitplugins-kfpytorch-1.6.2/flytekitplugins_kfpytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:24:18.161497 flytekitplugins-kfpytorch-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-30 15:24:12.000000 flytekitplugins-kfpytorch-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:56.735852 flytekitplugins-kfpytorch-1.6.2b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-01 20:41:56.735852 flytekitplugins-kfpytorch-1.6.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-01 20:41:31.000000 flytekitplugins-kfpytorch-1.6.2b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:56.731852 flytekitplugins-kfpytorch-1.6.2b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:56.731852 flytekitplugins-kfpytorch-1.6.2b0/flytekitplugins/kfpytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-01 20:41:31.000000 flytekitplugins-kfpytorch-1.6.2b0/flytekitplugins/kfpytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-06-01 20:41:31.000000 flytekitplugins-kfpytorch-1.6.2b0/flytekitplugins/kfpytorch/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:56.735852 flytekitplugins-kfpytorch-1.6.2b0/flytekitplugins_kfpytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-01 20:41:56.000000 flytekitplugins-kfpytorch-1.6.2b0/flytekitplugins_kfpytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-01 20:41:56.000000 flytekitplugins-kfpytorch-1.6.2b0/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:41:56.000000 flytekitplugins-kfpytorch-1.6.2b0/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 20:41:56.000000 flytekitplugins-kfpytorch-1.6.2b0/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 20:41:56.000000 flytekitplugins-kfpytorch-1.6.2b0/flytekitplugins_kfpytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 20:41:56.000000 flytekitplugins-kfpytorch-1.6.2b0/flytekitplugins_kfpytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:41:56.735852 flytekitplugins-kfpytorch-1.6.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-01 20:41:50.000000 flytekitplugins-kfpytorch-1.6.2b0/setup.py
```

### Comparing `flytekitplugins-kfpytorch-1.6.2/PKG-INFO` & `flytekitplugins-kfpytorch-1.6.2b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.6.2
+Version: 1.6.2b0
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.6.2/flytekitplugins/kfpytorch/task.py` & `flytekitplugins-kfpytorch-1.6.2b0/flytekitplugins/kfpytorch/task.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,110 @@
 """
 This Plugin adds the capability of running distributed pytorch training to Flyte using backend plugins, natively on
 Kubernetes. It leverages `Pytorch Job <https://github.com/kubeflow/pytorch-operator>`_ Plugin from kubeflow.
 """
 import os
-from dataclasses import dataclass
+from dataclasses import dataclass, field
+from enum import Enum
 from typing import Any, Callable, Dict, Optional, Union
 
 import cloudpickle
-from flyteidl.plugins.pytorch_pb2 import DistributedPyTorchTrainingTask
+from flyteidl.plugins.kubeflow import common_pb2 as kubeflow_common
+from flyteidl.plugins.kubeflow import pytorch_pb2 as pytorch_task
 from google.protobuf.json_format import MessageToDict
 
 import flytekit
-from flytekit import PythonFunctionTask
+from flytekit import PythonFunctionTask, Resources
 from flytekit.configuration import SerializationSettings
+from flytekit.core.resources import convert_resources_to_resource_model
 from flytekit.extend import IgnoreOutputs, TaskPlugins
 
 TORCH_IMPORT_ERROR_MESSAGE = "PyTorch is not installed. Please install `flytekitplugins-kfpytorch['elastic']`."
 
 
 @dataclass
-class PyTorch(object):
+class RestartPolicy(Enum):
+    """
+    RestartPolicy describes how the replicas should be restarted
     """
-    Configuration for an executable `Pytorch Job <https://github.com/kubeflow/pytorch-operator>`_. Use this
-    to run distributed pytorch training on k8s
 
+    ALWAYS = kubeflow_common.RESTART_POLICY_ALWAYS
+    FAILURE = kubeflow_common.RESTART_POLICY_ON_FAILURE
+    NEVER = kubeflow_common.RESTART_POLICY_NEVER
+
+
+@dataclass
+class CleanPodPolicy(Enum):
+    """
+    CleanPodPolicy describes how to deal with pods when the job is finished.
+    """
+
+    NONE = kubeflow_common.CLEANPOD_POLICY_NONE
+    ALL = kubeflow_common.CLEANPOD_POLICY_ALL
+    RUNNING = kubeflow_common.CLEANPOD_POLICY_RUNNING
+
+
+@dataclass
+class RunPolicy:
+    """
+    RunPolicy describes some policy to apply to the execution of a kubeflow job.
     Args:
-        num_workers: integer determining the number of worker replicas spawned in the cluster for this job
-        (in addition to 1 master).
+        clean_pod_policy (int): Defines the policy for cleaning up pods after the PyTorchJob completes. Default to None.
+        ttl_seconds_after_finished (int): Defines the TTL for cleaning up finished PyTorchJobs.
+        active_deadline_seconds (int): Specifies the duration (in seconds) since startTime during which the job.
+        can remain active before it is terminated. Must be a positive integer. This setting applies only to pods.
+        where restartPolicy is OnFailure or Always.
+        backoff_limit (int): Number of retries before marking this job as failed.
+    """
+
+    clean_pod_policy: CleanPodPolicy = None
+    ttl_seconds_after_finished: Optional[int] = None
+    active_deadline_seconds: Optional[int] = None
+    backoff_limit: Optional[int] = None
+
+
+@dataclass
+class Worker:
+    image: Optional[str] = None
+    requests: Optional[Resources] = None
+    limits: Optional[Resources] = None
+    replicas: Optional[int] = None
+    restart_policy: Optional[RestartPolicy] = None
+
 
+@dataclass
+class Master:
+    """
+    Configuration for master replica group. Master should always have 1 replica, so we don't need a `replicas` field
+    """
+
+    image: Optional[str] = None
+    requests: Optional[Resources] = None
+    limits: Optional[Resources] = None
+    restart_policy: Optional[RestartPolicy] = None
+
+
+@dataclass
+class PyTorch(object):
+    """
+    Configuration for an executable `PyTorch Job <https://github.com/kubeflow/pytorch-operator>`_. Use this
+    to run distributed PyTorch training on Kubernetes.
+
+    Args:
+        master: Configuration for the master replica group.
+        worker: Configuration for the worker replica group.
+        run_policy: Configuration for the run policy.
+        num_workers: [DEPRECATED] This argument is deprecated. Use `worker.replicas` instead.
     """
 
-    num_workers: int
+    master: Master = field(default_factory=lambda: Master())
+    worker: Worker = field(default_factory=lambda: Worker())
+    run_policy: Optional[RunPolicy] = field(default_factory=lambda: None)
+    # Support v0 config for backwards compatibility
+    num_workers: Optional[int] = None
 
 
 @dataclass
 class Elastic(object):
     """
     Configuration for `torch elastic training <https://pytorch.org/docs/stable/elastic/run.html>`_.
 
@@ -63,24 +133,65 @@
     Plugin that submits a PyTorchJob (see https://github.com/kubeflow/pytorch-operator)
         defined by the code within the _task_function to k8s cluster.
     """
 
     _PYTORCH_TASK_TYPE = "pytorch"
 
     def __init__(self, task_config: PyTorch, task_function: Callable, **kwargs):
+        if task_config.num_workers and task_config.worker.replicas:
+            raise ValueError(
+                "Cannot specify both `num_workers` and `worker.replicas`. Please use `worker.replicas` as `num_workers` is depreacated."
+            )
+        if task_config.num_workers is None and task_config.worker.replicas is None:
+            raise ValueError(
+                "Must specify either `num_workers` or `worker.replicas`. Please use `worker.replicas` as `num_workers` is depreacated."
+            )
         super().__init__(
             task_config,
             task_function,
             task_type=self._PYTORCH_TASK_TYPE,
             **kwargs,
         )
 
+    def _convert_replica_spec(
+        self, replica_config: Union[Master, Worker]
+    ) -> pytorch_task.DistributedPyTorchTrainingReplicaSpec:
+        resources = convert_resources_to_resource_model(requests=replica_config.requests, limits=replica_config.limits)
+        replicas = 1
+        # Master should always have 1 replica
+        if not isinstance(replica_config, Master):
+            replicas = replica_config.replicas
+        return pytorch_task.DistributedPyTorchTrainingReplicaSpec(
+            replicas=replicas,
+            image=replica_config.image,
+            resources=resources.to_flyte_idl() if resources else None,
+            restart_policy=replica_config.restart_policy.value if replica_config.restart_policy else None,
+        )
+
+    def _convert_run_policy(self, run_policy: RunPolicy) -> kubeflow_common.RunPolicy:
+        return kubeflow_common.RunPolicy(
+            clean_pod_policy=run_policy.clean_pod_policy.value if run_policy.clean_pod_policy else None,
+            ttl_seconds_after_finished=run_policy.ttl_seconds_after_finished,
+            active_deadline_seconds=run_policy.active_deadline_seconds,
+            backoff_limit=run_policy.active_deadline_seconds,
+        )
+
     def get_custom(self, settings: SerializationSettings) -> Dict[str, Any]:
-        job = DistributedPyTorchTrainingTask(workers=self.task_config.num_workers)
-        return MessageToDict(job)
+        worker = self._convert_replica_spec(self.task_config.worker)
+        # support v0 config for backwards compatibility
+        if self.task_config.num_workers:
+            worker.replicas = self.task_config.num_workers
+
+        run_policy = self._convert_run_policy(self.task_config.run_policy) if self.task_config.run_policy else None
+        pytorch_job = pytorch_task.DistributedPyTorchTrainingTask(
+            worker_replicas=worker,
+            master_replicas=self._convert_replica_spec(self.task_config.master),
+            run_policy=run_policy,
+        )
+        return MessageToDict(pytorch_job)
 
 
 # Register the Pytorch Plugin into the flytekit core plugin system
 TaskPlugins.register_pythontask_plugin(PyTorch, PyTorchFunctionTask)
 
 
 def spawn_helper(fn: bytes, kwargs) -> Any:
@@ -232,16 +343,18 @@
             elastic_config = ElasticConfig(
                 rdzv_backend=self.rdzv_backend,
                 min_replicas=self.min_nodes,
                 max_replicas=self.max_nodes,
                 nproc_per_node=self.task_config.nproc_per_node,
                 max_restarts=self.task_config.max_restarts,
             )
-            job = DistributedPyTorchTrainingTask(
-                workers=self.max_nodes,
+            job = pytorch_task.DistributedPyTorchTrainingTask(
+                worker_replicas=pytorch_task.DistributedPyTorchTrainingReplicaSpec(
+                    replicas=self.max_nodes,
+                ),
                 elastic_config=elastic_config,
             )
             return MessageToDict(job)
 
 
 # Register the PytorchElastic Plugin into the flytekit core plugin system
 TaskPlugins.register_pythontask_plugin(Elastic, PytorchElasticFunctionTask)
```

### Comparing `flytekitplugins-kfpytorch-1.6.2/flytekitplugins_kfpytorch.egg-info/PKG-INFO` & `flytekitplugins-kfpytorch-1.6.2b0/flytekitplugins_kfpytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.6.2
+Version: 1.6.2b0
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.6.2/setup.py` & `flytekitplugins-kfpytorch-1.6.2b0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 PLUGIN_NAME = "kfpytorch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
-plugin_requires = ["cloudpickle", "flytekit>=1.3.0,<2.0.0", "flyteidl>=1.3.19"]
+plugin_requires = ["cloudpickle", "flytekit>=1.6.1"]
 
-__version__ = "1.6.2"
+__version__ = "1.6.2b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Pytorch plugin for Flytekit",
```

