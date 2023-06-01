# Comparing `tmp/flux-metrics-api-0.0.1.tar.gz` & `tmp/flux-metrics-api-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-metrics-api-0.0.1.tar", last modified: Wed May 31 04:49:57 2023, max compression
+gzip compressed data, was "flux-metrics-api-0.0.11.tar", last modified: Thu Jun  1 02:32:48 2023, max compression
```

## Comparing `flux-metrics-api-0.0.1.tar` & `flux-metrics-api-0.0.11.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:49:57.987536 flux-metrics-api-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-31 04:49:57.987536 flux-metrics-api-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:49:57.983536 flux-metrics-api-0.0.1/flux_metrics_api/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:49:57.987536 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-31 04:49:57.000000 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-31 04:49:57.000000 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:49:57.000000 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 04:49:57.000000 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:49:57.000000 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 04:49:57.000000 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 04:49:57.000000 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-31 04:49:57.987536 flux-metrics-api-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:32:48.513154 flux-metrics-api-0.0.11/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-06-01 02:32:48.513154 flux-metrics-api-0.0.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:32:48.509154 flux-metrics-api-0.0.11/flux_metrics_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/flux_metrics_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/flux_metrics_api/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/flux_metrics_api/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/flux_metrics_api/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/flux_metrics_api/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/flux_metrics_api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/flux_metrics_api/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/flux_metrics_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/flux_metrics_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/flux_metrics_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:32:48.513154 flux-metrics-api-0.0.11/flux_metrics_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-06-01 02:32:48.000000 flux-metrics-api-0.0.11/flux_metrics_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-01 02:32:48.000000 flux-metrics-api-0.0.11/flux_metrics_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:32:48.000000 flux-metrics-api-0.0.11/flux_metrics_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 02:32:48.000000 flux-metrics-api-0.0.11/flux_metrics_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:32:48.000000 flux-metrics-api-0.0.11/flux_metrics_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 02:32:48.000000 flux-metrics-api-0.0.11/flux_metrics_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 02:32:48.000000 flux-metrics-api-0.0.11/flux_metrics_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-01 02:32:48.513154 flux-metrics-api-0.0.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-01 02:32:07.000000 flux-metrics-api-0.0.11/setup.py
```

### Comparing `flux-metrics-api-0.0.1/LICENSE` & `flux-metrics-api-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-metrics-api-0.0.1/NOTICE` & `flux-metrics-api-0.0.11/NOTICE`

 * *Files identical despite different names*

### Comparing `flux-metrics-api-0.0.1/PKG-INFO` & `flux-metrics-api-0.0.11/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: flux-metrics-api
-Version: 0.0.1
-Summary: Custom metrics exporter for Flux in Kubernetes
-Home-page: https://github.com/converged-computing/flux-metrics-api
-Author: Vanessa Sochat
-Author-email: vsoch@users.noreply.github.com
-Maintainer: Vanessa Sochat
-License: LICENSE
-Keywords: cloud,flux,flux-framework,monitoring
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-Provides-Extra: all
-License-File: LICENSE
-License-File: NOTICE
-
 # Flux Metrics API
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 [![PyPI](https://img.shields.io/pypi/v/flux-metrics-api)](https://pypi.org/project/flux-metrics-api/)
 
@@ -75,26 +52,74 @@
 ```bash
 $ flux-metrics-api start
 
 # customize the port or host
 $ flux-metrics-api start --port 9000 --host 127.0.0.1
 ```
 
+#### SSL
+
 If you want ssl (port 443) you can provide the path to a certificate and keyfile:
 
 ```bash
 $ flux-metrics-api start --ssl-certfile /etc/certs/tls.crt --ssl-keyfile /etc/certs/tls.key
 ```
 
 An example of a full command we might run from within a pod:
 
 ```bash
 $ flux-metrics-api start --port 8443 --ssl-certfile /etc/certs/tls.crt --ssl-keyfile /etc/certs/tls.key --namespace flux-operator --service-name custom-metrics-apiserver
 ```
 
+#### On the fly custom metrics!
+
+If you want to provide custom metrics, you can write a function in an external file that we will read it and add to the server.
+As a general rule:
+
+ - The name of the function will be the name of the custom metric
+ - You can expect the only argument to be the flux handle
+ - You'll need to do imports within your function to get them in scope
+
+This likely can be improved upon, but is a start for now! We provide an [example file](example/custom-metrics.py). As an example:
+
+```bash
+$ flux-metrics-api start --custom-metric ./example/custom-metrics.py
+```
+
+And then test it:
+
+```bash
+$ curl -s http://localhost:8443/apis/custom.metrics.k8s.io/v1beta2/namespaces/flux-operator/metrics/my_custom_metric_name | jq
+```
+```console
+{
+  "items": [
+    {
+      "metric": {
+        "name": "my_custom_metric_name"
+      },
+      "value": 4,
+      "timestamp": "2023-06-01T01:39:08+00:00",
+      "windowSeconds": 0,
+      "describedObject": {
+        "kind": "Service",
+        "namespace": "flux-operator",
+        "name": "custom-metrics-apiserver",
+        "apiVersion": "v1beta2"
+      }
+    }
+  ],
+  "apiVersion": "custom.metrics.k8s.io/v1beta2",
+  "kind": "MetricValueList",
+  "metadata": {
+    "selfLink": "/apis/custom.metrics.k8s.io/v1beta2"
+  }
+}
+```
+
 See `--help` to see other options available.
 
 ### Endpoints
 
 #### Metric
 
 **GET /apis/custom.metrics.k8s.io/v1beta2/namespaces/<namespace>/metrics/<metric_name>**
@@ -132,14 +157,22 @@
 
 The following metrics are supported:
 
  - **node_up_count**: number of nodes up in the MiniCluster
  - **node_free_count**: number of nodes free in the MiniCluster
  - **node_cores_free_count**: number of node cores free in the MiniCluster
  - **node_cores_up_count**: number of node cores up in the MiniCluster
+ - **job_queue_state_new_count**: number of new jobs in the queue
+ - **job_queue_state_depend_count**: number of jobs in the queue in state "depend"
+ - **job_queue_state_priority_count**: number of jobs in the queue in state "priority"
+ - **job_queue_state_sched_count**: number of jobs in the queue in state "sched"
+ - **job_queue_state_run_count**: number of jobs in the queue in state "run"
+ - **job_queue_state_cleanup_count**: number of jobs in the queue in state "cleanup"
+ - **job_queue_state_inactive_count**: number of jobs in the queue in state "inactive"
+
 
 ### Docker
 
 We have a docker container, which you can customize for your use case, but it's more intended to
 be a demo. You can either build it yourself, or use our build.
 
 ```bash
```

### Comparing `flux-metrics-api-0.0.1/README.md` & `flux-metrics-api-0.0.11/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: flux-metrics-api
+Version: 0.0.11
+Summary: Custom metrics exporter for Flux in Kubernetes
+Home-page: https://github.com/converged-computing/flux-metrics-api
+Author: Vanessa Sochat
+Author-email: vsoch@users.noreply.github.com
+Maintainer: Vanessa Sochat
+License: LICENSE
+Keywords: cloud,flux,flux-framework,monitoring
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+Provides-Extra: all
+License-File: LICENSE
+License-File: NOTICE
+
 # Flux Metrics API
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 [![PyPI](https://img.shields.io/pypi/v/flux-metrics-api)](https://pypi.org/project/flux-metrics-api/)
 
@@ -52,26 +75,74 @@
 ```bash
 $ flux-metrics-api start
 
 # customize the port or host
 $ flux-metrics-api start --port 9000 --host 127.0.0.1
 ```
 
+#### SSL
+
 If you want ssl (port 443) you can provide the path to a certificate and keyfile:
 
 ```bash
 $ flux-metrics-api start --ssl-certfile /etc/certs/tls.crt --ssl-keyfile /etc/certs/tls.key
 ```
 
 An example of a full command we might run from within a pod:
 
 ```bash
 $ flux-metrics-api start --port 8443 --ssl-certfile /etc/certs/tls.crt --ssl-keyfile /etc/certs/tls.key --namespace flux-operator --service-name custom-metrics-apiserver
 ```
 
+#### On the fly custom metrics!
+
+If you want to provide custom metrics, you can write a function in an external file that we will read it and add to the server.
+As a general rule:
+
+ - The name of the function will be the name of the custom metric
+ - You can expect the only argument to be the flux handle
+ - You'll need to do imports within your function to get them in scope
+
+This likely can be improved upon, but is a start for now! We provide an [example file](example/custom-metrics.py). As an example:
+
+```bash
+$ flux-metrics-api start --custom-metric ./example/custom-metrics.py
+```
+
+And then test it:
+
+```bash
+$ curl -s http://localhost:8443/apis/custom.metrics.k8s.io/v1beta2/namespaces/flux-operator/metrics/my_custom_metric_name | jq
+```
+```console
+{
+  "items": [
+    {
+      "metric": {
+        "name": "my_custom_metric_name"
+      },
+      "value": 4,
+      "timestamp": "2023-06-01T01:39:08+00:00",
+      "windowSeconds": 0,
+      "describedObject": {
+        "kind": "Service",
+        "namespace": "flux-operator",
+        "name": "custom-metrics-apiserver",
+        "apiVersion": "v1beta2"
+      }
+    }
+  ],
+  "apiVersion": "custom.metrics.k8s.io/v1beta2",
+  "kind": "MetricValueList",
+  "metadata": {
+    "selfLink": "/apis/custom.metrics.k8s.io/v1beta2"
+  }
+}
+```
+
 See `--help` to see other options available.
 
 ### Endpoints
 
 #### Metric
 
 **GET /apis/custom.metrics.k8s.io/v1beta2/namespaces/<namespace>/metrics/<metric_name>**
@@ -109,14 +180,22 @@
 
 The following metrics are supported:
 
  - **node_up_count**: number of nodes up in the MiniCluster
  - **node_free_count**: number of nodes free in the MiniCluster
  - **node_cores_free_count**: number of node cores free in the MiniCluster
  - **node_cores_up_count**: number of node cores up in the MiniCluster
+ - **job_queue_state_new_count**: number of new jobs in the queue
+ - **job_queue_state_depend_count**: number of jobs in the queue in state "depend"
+ - **job_queue_state_priority_count**: number of jobs in the queue in state "priority"
+ - **job_queue_state_sched_count**: number of jobs in the queue in state "sched"
+ - **job_queue_state_run_count**: number of jobs in the queue in state "run"
+ - **job_queue_state_cleanup_count**: number of jobs in the queue in state "cleanup"
+ - **job_queue_state_inactive_count**: number of jobs in the queue in state "inactive"
+
 
 ### Docker
 
 We have a docker container, which you can customize for your use case, but it's more intended to
 be a demo. You can either build it yourself, or use our build.
 
 ```bash
```

### Comparing `flux-metrics-api-0.0.1/flux_metrics_api/apis.py` & `flux-metrics-api-0.0.11/flux_metrics_api/apis.py`

 * *Files identical despite different names*

### Comparing `flux-metrics-api-0.0.1/flux_metrics_api/defaults.py` & `flux-metrics-api-0.0.11/flux_metrics_api/defaults.py`

 * *Files identical despite different names*

### Comparing `flux-metrics-api-0.0.1/flux_metrics_api/logger.py` & `flux-metrics-api-0.0.11/flux_metrics_api/logger.py`

 * *Files identical despite different names*

### Comparing `flux-metrics-api-0.0.1/flux_metrics_api/routes.py` & `flux-metrics-api-0.0.11/flux_metrics_api/routes.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from starlette.responses import JSONResponse
 from starlette.routing import Route
 from starlette_apispec import APISpecSchemaGenerator
 
 import flux_metrics_api.defaults as defaults
 import flux_metrics_api.types as types
 import flux_metrics_api.version as version
-from flux_metrics_api.metrics import metrics
+from flux_metrics_api.metrics import custom_metrics, handle, metrics
 
 schemas = APISpecSchemaGenerator(
     APISpec(
         title="Flux Metrics API",
         version=version.__version__,
         openapi_version="3.0.0",
         info={"description": "Export Flux custom metrics."},
@@ -51,25 +51,28 @@
     metric_name = request.path_params["metric_name"]
     namespace = request.path_params.get("namespace")
     print(f"Requested metric {metric_name} in  namespace {namespace}")
 
     # TODO we don't do anything with namespace currently, we assume we won't
     # be able to hit this if running in the wrong one
     # Unknown metric
-    if metric_name not in metrics:
+    if metric_name not in metrics and metric_name not in custom_metrics:
         print(f"Unknown metric requested {metric_name}")
         return JSONResponse(
             {"detail": "This metric is not known to the server."}, status_code=404
         )
 
     # Prepare the metric
     metric = types.new_identifier(metric_name)
 
     # Get the value from Flux, assemble into listing
-    value = metrics[metric_name]()
+    if metric_name in custom_metrics:
+        value = custom_metrics[metric_name](handle)
+    else:
+        value = metrics[metric_name]()
     metric_value = types.new_metric(metric, value=value)
 
     # Give the endpoint for the service as metadata
     metadata = {"selfLink": defaults.API_ROOT}
     listing = types.new_metric_list([metric_value], metadata=metadata)
     return JSONResponse(listing)
```

### Comparing `flux-metrics-api-0.0.1/flux_metrics_api/server.py` & `flux-metrics-api-0.0.11/flux_metrics_api/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import sys
 
 import uvicorn
 from starlette.applications import Starlette
 
 import flux_metrics_api
 import flux_metrics_api.defaults as defaults
+import flux_metrics_api.metrics as metrics
 from flux_metrics_api.logger import setup_logger
 from flux_metrics_api.routes import routes
 
 
 def get_parser():
     parser = argparse.ArgumentParser(
         description="Flux Metrics API",
@@ -69,14 +70,15 @@
         default=8443,
         type=int,
     )
     start.add_argument("--namespace", help="Namespace the API is running in")
     start.add_argument(
         "--service-name", help="Service name the metrics service is running from"
     )
+    start.add_argument("--custom-metric", help="A Python file with custom metrics")
     start.add_argument(
         "--api-path",
         dest="api_path",
         help="Custom API path (defaults to /apis/custom.metrics.k8s.io/v1beta2)",
         default=None,
     )
     start.add_argument(
@@ -107,14 +109,17 @@
     """
     # Validate certificates if provided
     if args.ssl_keyfile and not args.ssl_certfile:
         sys.exit("A --ssl-keyfile was provided without a --ssl-certfile.")
     if args.ssl_certfile and not args.ssl_keyfile:
         sys.exit("A --ssl-certfile was provided without a --ssl-keyfile.")
 
+    # The user wants to add a file with custom metrics
+    if args.custom_metric:
+        metrics.add_custom_metrics(args.custom_metric)
     app = Starlette(debug=args.debug, routes=routes)
     uvicorn.run(
         app,
         host=args.host,
         port=args.port,
         ssl_keyfile=args.ssl_keyfile,
         ssl_certfile=args.ssl_certfile,
```

### Comparing `flux-metrics-api-0.0.1/flux_metrics_api/types.py` & `flux-metrics-api-0.0.11/flux_metrics_api/types.py`

 * *Files identical despite different names*

### Comparing `flux-metrics-api-0.0.1/flux_metrics_api.egg-info/PKG-INFO` & `flux-metrics-api-0.0.11/flux_metrics_api.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-metrics-api
-Version: 0.0.1
+Version: 0.0.11
 Summary: Custom metrics exporter for Flux in Kubernetes
 Home-page: https://github.com/converged-computing/flux-metrics-api
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cloud,flux,flux-framework,monitoring
@@ -75,26 +75,74 @@
 ```bash
 $ flux-metrics-api start
 
 # customize the port or host
 $ flux-metrics-api start --port 9000 --host 127.0.0.1
 ```
 
+#### SSL
+
 If you want ssl (port 443) you can provide the path to a certificate and keyfile:
 
 ```bash
 $ flux-metrics-api start --ssl-certfile /etc/certs/tls.crt --ssl-keyfile /etc/certs/tls.key
 ```
 
 An example of a full command we might run from within a pod:
 
 ```bash
 $ flux-metrics-api start --port 8443 --ssl-certfile /etc/certs/tls.crt --ssl-keyfile /etc/certs/tls.key --namespace flux-operator --service-name custom-metrics-apiserver
 ```
 
+#### On the fly custom metrics!
+
+If you want to provide custom metrics, you can write a function in an external file that we will read it and add to the server.
+As a general rule:
+
+ - The name of the function will be the name of the custom metric
+ - You can expect the only argument to be the flux handle
+ - You'll need to do imports within your function to get them in scope
+
+This likely can be improved upon, but is a start for now! We provide an [example file](example/custom-metrics.py). As an example:
+
+```bash
+$ flux-metrics-api start --custom-metric ./example/custom-metrics.py
+```
+
+And then test it:
+
+```bash
+$ curl -s http://localhost:8443/apis/custom.metrics.k8s.io/v1beta2/namespaces/flux-operator/metrics/my_custom_metric_name | jq
+```
+```console
+{
+  "items": [
+    {
+      "metric": {
+        "name": "my_custom_metric_name"
+      },
+      "value": 4,
+      "timestamp": "2023-06-01T01:39:08+00:00",
+      "windowSeconds": 0,
+      "describedObject": {
+        "kind": "Service",
+        "namespace": "flux-operator",
+        "name": "custom-metrics-apiserver",
+        "apiVersion": "v1beta2"
+      }
+    }
+  ],
+  "apiVersion": "custom.metrics.k8s.io/v1beta2",
+  "kind": "MetricValueList",
+  "metadata": {
+    "selfLink": "/apis/custom.metrics.k8s.io/v1beta2"
+  }
+}
+```
+
 See `--help` to see other options available.
 
 ### Endpoints
 
 #### Metric
 
 **GET /apis/custom.metrics.k8s.io/v1beta2/namespaces/<namespace>/metrics/<metric_name>**
@@ -132,14 +180,22 @@
 
 The following metrics are supported:
 
  - **node_up_count**: number of nodes up in the MiniCluster
  - **node_free_count**: number of nodes free in the MiniCluster
  - **node_cores_free_count**: number of node cores free in the MiniCluster
  - **node_cores_up_count**: number of node cores up in the MiniCluster
+ - **job_queue_state_new_count**: number of new jobs in the queue
+ - **job_queue_state_depend_count**: number of jobs in the queue in state "depend"
+ - **job_queue_state_priority_count**: number of jobs in the queue in state "priority"
+ - **job_queue_state_sched_count**: number of jobs in the queue in state "sched"
+ - **job_queue_state_run_count**: number of jobs in the queue in state "run"
+ - **job_queue_state_cleanup_count**: number of jobs in the queue in state "cleanup"
+ - **job_queue_state_inactive_count**: number of jobs in the queue in state "inactive"
+
 
 ### Docker
 
 We have a docker container, which you can customize for your use case, but it's more intended to
 be a demo. You can either build it yourself, or use our build.
 
 ```bash
```

### Comparing `flux-metrics-api-0.0.1/flux_metrics_api.egg-info/SOURCES.txt` & `flux-metrics-api-0.0.11/flux_metrics_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-metrics-api-0.0.1/setup.py` & `flux-metrics-api-0.0.11/setup.py`

 * *Files identical despite different names*

