# Comparing `tmp/hera-5.3.0.tar.gz` & `tmp/hera-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hera-5.3.0.tar", max compression
+gzip compressed data, was "hera-5.4.0.tar", max compression
```

## Comparing `hera-5.3.0.tar` & `hera-5.4.0.tar`

### file list

```diff
@@ -1,134 +1,134 @@
--rw-r--r--   0        0        0     1066 2023-05-26 16:26:41.880003 hera-5.3.0/LICENSE
--rw-r--r--   0        0        0    11980 2023-05-26 16:26:41.880003 hera-5.3.0/README.md
--rw-r--r--   0        0        0     3530 2023-05-26 16:26:57.651977 hera-5.3.0/pyproject.toml
--rw-r--r--   0        0        0      522 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/__init__.py
--rw-r--r--   0        0        0      300 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/_version.py
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/__init__.py
--rw-r--r--   0        0        0     3267 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.896003 hera-5.3.0/src/hera/events/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/sensor.py
--rw-r--r--   0        0        0      887 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/models/sensor.pyi
--rw-r--r--   0        0        0    27607 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/events/service.py
--rw-r--r--   0        0        0     2186 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/exceptions/__init__.py
--rw-r--r--   0        0        0      282 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/expr/__init__.py
--rw-r--r--   0        0        0    12021 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/expr/_node.py
--rw-r--r--   0        0        0      647 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/expr/_sprig.py
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/py.typed
--rw-r--r--   0        0        0      188 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/shared/__init__.py
--rw-r--r--   0        0        0      269 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/shared/_base_model.py
--rw-r--r--   0        0        0     4927 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/shared/_global_config.py
--rw-r--r--   0        0        0      513 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/shared/serialization.py
--rw-r--r--   0        0        0     4585 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/__init__.py
--rw-r--r--   0        0        0     2912 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/_context.py
--rw-r--r--   0        0        0    34769 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/_mixins.py
--rw-r--r--   0        0        0    32815 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/_unparse.py
--rw-r--r--   0        0        0       25 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/action.py
--rw-r--r--   0        0        0     1115 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/archive.py
--rw-r--r--   0        0        0     7697 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/artifact.py
--rw-r--r--   0        0        0     3464 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/container.py
--rw-r--r--   0        0        0     7280 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/container_set.py
--rw-r--r--   0        0        0     3779 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/cron_workflow.py
--rw-r--r--   0        0        0     2877 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/dag.py
--rw-r--r--   0        0        0     2241 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/data.py
--rw-r--r--   0        0        0     4855 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/env.py
--rw-r--r--   0        0        0     1329 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/env_from.py
--rw-r--r--   0        0        0      208 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/exceptions.py
--rw-r--r--   0        0        0     2346 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/http_template.py
--rw-r--r--   0        0        0       30 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/memoize.py
--rw-r--r--   0        0        0     4418 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/metrics.py
--rw-r--r--   0        0        0     6913 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-05-26 16:26:41.900003 hera-5.3.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/sensor.py
--rw-r--r--   0        0        0      887 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/models/sensor.pyi
--rw-r--r--   0        0        0      722 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/operator.py
--rw-r--r--   0        0        0     4084 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/parameter.py
--rw-r--r--   0        0        0     1018 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/protocol.py
--rw-r--r--   0        0        0     3146 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/resource.py
--rw-r--r--   0        0        0     5262 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/resources.py
--rw-r--r--   0        0        0     1856 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/retry_strategy.py
--rw-r--r--   0        0        0     3707 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/runner.py
--rw-r--r--   0        0        0    16549 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/script.py
--rw-r--r--   0        0        0    55322 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/service.py
--rw-r--r--   0        0        0     6738 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/steps.py
--rw-r--r--   0        0        0     3332 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/suspend.py
--rw-r--r--   0        0        0     8071 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/task.py
--rw-r--r--   0        0        0       27 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/toleration.py
--rw-r--r--   0        0        0     2007 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/user_container.py
--rw-r--r--   0        0        0     2610 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/validators.py
--rw-r--r--   0        0        0    18656 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/volume.py
--rw-r--r--   0        0        0    18117 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/workflow.py
--rw-r--r--   0        0        0      911 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/workflow_status.py
--rw-r--r--   0        0        0     7334 2023-05-26 16:26:41.904003 hera-5.3.0/src/hera/workflows/workflow_template.py
--rw-r--r--   0        0        0    13403 1970-01-01 00:00:00.000000 hera-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-01 09:22:56.981018 hera-5.4.0/LICENSE
+-rw-r--r--   0        0        0    11980 2023-06-01 09:22:56.981018 hera-5.4.0/README.md
+-rw-r--r--   0        0        0     3530 2023-06-01 09:23:13.113041 hera-5.4.0/pyproject.toml
+-rw-r--r--   0        0        0      522 2023-06-01 09:22:56.997018 hera-5.4.0/src/hera/__init__.py
+-rw-r--r--   0        0        0      300 2023-06-01 09:22:56.997018 hera-5.4.0/src/hera/_version.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:56.997018 hera-5.4.0/src/hera/events/__init__.py
+-rw-r--r--   0        0        0     3267 2023-06-01 09:22:56.997018 hera-5.4.0/src/hera/events/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-06-01 09:22:56.997018 hera-5.4.0/src/hera/events/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-06-01 09:22:56.997018 hera-5.4.0/src/hera/events/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:56.997018 hera-5.4.0/src/hera/events/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-06-01 09:22:56.997018 hera-5.4.0/src/hera/events/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-06-01 09:22:56.997018 hera-5.4.0/src/hera/events/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-06-01 09:22:57.001018 hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/events/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/events/models/sensor.pyi
+-rw-r--r--   0        0        0    27607 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/events/service.py
+-rw-r--r--   0        0        0     2186 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/exceptions/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/expr/__init__.py
+-rw-r--r--   0        0        0    12021 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/expr/_node.py
+-rw-r--r--   0        0        0      647 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/expr/_sprig.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/py.typed
+-rw-r--r--   0        0        0      188 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/shared/__init__.py
+-rw-r--r--   0        0        0      269 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/shared/_base_model.py
+-rw-r--r--   0        0        0     4927 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/shared/_global_config.py
+-rw-r--r--   0        0        0      513 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/shared/serialization.py
+-rw-r--r--   0        0        0     4585 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/__init__.py
+-rw-r--r--   0        0        0     2912 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/_context.py
+-rw-r--r--   0        0        0    35054 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/_mixins.py
+-rw-r--r--   0        0        0    32815 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/_unparse.py
+-rw-r--r--   0        0        0       25 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/action.py
+-rw-r--r--   0        0        0     1115 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/archive.py
+-rw-r--r--   0        0        0     7697 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/artifact.py
+-rw-r--r--   0        0        0     3464 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/container.py
+-rw-r--r--   0        0        0     7280 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/container_set.py
+-rw-r--r--   0        0        0     3779 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/cron_workflow.py
+-rw-r--r--   0        0        0     2877 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/dag.py
+-rw-r--r--   0        0        0     2241 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/data.py
+-rw-r--r--   0        0        0     4855 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/env.py
+-rw-r--r--   0        0        0     1329 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/env_from.py
+-rw-r--r--   0        0        0      208 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/exceptions.py
+-rw-r--r--   0        0        0     2346 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/http_template.py
+-rw-r--r--   0        0        0       30 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/memoize.py
+-rw-r--r--   0        0        0     4418 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/metrics.py
+-rw-r--r--   0        0        0     6913 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/models/sensor.pyi
+-rw-r--r--   0        0        0      722 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/operator.py
+-rw-r--r--   0        0        0     4084 2023-06-01 09:22:57.005018 hera-5.4.0/src/hera/workflows/parameter.py
+-rw-r--r--   0        0        0     1018 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/protocol.py
+-rw-r--r--   0        0        0     3146 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/resource.py
+-rw-r--r--   0        0        0     5262 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/resources.py
+-rw-r--r--   0        0        0     1856 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/retry_strategy.py
+-rw-r--r--   0        0        0     3707 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/runner.py
+-rw-r--r--   0        0        0    16549 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/script.py
+-rw-r--r--   0        0        0    55322 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/service.py
+-rw-r--r--   0        0        0     6747 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/steps.py
+-rw-r--r--   0        0        0     3332 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/suspend.py
+-rw-r--r--   0        0        0     7959 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/task.py
+-rw-r--r--   0        0        0       27 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/toleration.py
+-rw-r--r--   0        0        0     2007 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/user_container.py
+-rw-r--r--   0        0        0     2610 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/validators.py
+-rw-r--r--   0        0        0    18709 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/volume.py
+-rw-r--r--   0        0        0    18961 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/workflow.py
+-rw-r--r--   0        0        0      911 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/workflow_status.py
+-rw-r--r--   0        0        0     7343 2023-06-01 09:22:57.009018 hera-5.4.0/src/hera/workflows/workflow_template.py
+-rw-r--r--   0        0        0    13403 1970-01-01 00:00:00.000000 hera-5.4.0/PKG-INFO
```

### Comparing `hera-5.3.0/LICENSE` & `hera-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/README.md` & `hera-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/pyproject.toml` & `hera-5.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "hera"  # project-name
 # The version is automatically substituted by the CI
-version = "5.3.0"
+version = "5.4.0"
 description = "Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows."
 authors = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 maintainers = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/argoproj-labs/hera"
 repository = "https://github.com/argoproj-labs/hera"
```

### Comparing `hera-5.3.0/src/hera/__init__.py` & `hera-5.4.0/src/hera/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/__init__.py` & `hera-5.4.0/src/hera/events/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/eventsource.py` & `hera-5.4.0/src/hera/events/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/eventsource.pyi` & `hera-5.4.0/src/hera/events/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/grpc/gateway/runtime.py` & `hera-5.4.0/src/hera/events/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/io/argoproj/events/v1alpha1.py` & `hera-5.4.0/src/hera/events/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/io/argoproj/events/v1alpha1.pyi` & `hera-5.4.0/src/hera/events/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.py` & `hera-5.4.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi` & `hera-5.4.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/io/k8s/api/core/v1.py` & `hera-5.4.0/src/hera/events/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/io/k8s/api/core/v1.pyi` & `hera-5.4.0/src/hera/events/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/io/k8s/api/policy/v1beta1.py` & `hera-5.4.0/src/hera/events/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera-5.4.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/sensor.py` & `hera-5.4.0/src/hera/events/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/models/sensor.pyi` & `hera-5.4.0/src/hera/events/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/events/service.py` & `hera-5.4.0/src/hera/events/service.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/exceptions/__init__.py` & `hera-5.4.0/src/hera/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/expr/_node.py` & `hera-5.4.0/src/hera/expr/_node.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/expr/_sprig.py` & `hera-5.4.0/src/hera/expr/_sprig.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/shared/_global_config.py` & `hera-5.4.0/src/hera/shared/_global_config.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/shared/serialization.py` & `hera-5.4.0/src/hera/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/__init__.py` & `hera-5.4.0/src/hera/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/_context.py` & `hera-5.4.0/src/hera/workflows/_context.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/_mixins.py` & `hera-5.4.0/src/hera/workflows/_mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,42 +467,43 @@
 
 
 class CallableTemplateMixin(ArgumentsMixin):
     def __call__(self, *args, **kwargs) -> Union[Step, Task]:
         if "name" not in kwargs:
             kwargs["name"] = self.name  # type: ignore
 
+        arguments = self._get_arguments(**kwargs)
+        parameter_names = self._get_parameter_names(arguments)
+        artifact_names = self._get_artifact_names(arguments)
+
         # when the `source` is set via an `@script` decorator, it does not come in with the `kwargs` so we need to
         # set it here in order for the following logic to capture it
         if "source" not in kwargs and hasattr(self, "source"):
             kwargs["source"] = self.source  # type: ignore
 
+        if "source" in kwargs and "with_param" in kwargs:
+            arguments += self._get_deduped_params_from_source(parameter_names, artifact_names, kwargs["source"])
+        elif "source" in kwargs and "with_items" in kwargs:
+            arguments += self._get_deduped_params_from_items(parameter_names, kwargs["with_items"])
+
+        # it is possible for the user to pass `arguments` via `kwargs` along with `with_param`. The `with_param`
+        # additional parameters are inferred and have to be added to the `kwargs['arguments']`, otherwise
+        # the step/task will miss adding them when building the final arguments
+        kwargs["arguments"] = arguments
+
         try:
             from hera.workflows.steps import Step
 
             return Step(*args, template=self, **kwargs)
         except InvalidType:
             pass
 
         try:
             from hera.workflows.task import Task
 
-            arguments = self._get_arguments(**kwargs)
-            parameter_names = self._get_parameter_names(arguments)
-            artifact_names = self._get_artifact_names(arguments)
-            if "source" in kwargs and "with_param" in kwargs:
-                arguments += self._get_deduped_params_from_source(parameter_names, artifact_names, kwargs["source"])
-            elif "source" in kwargs and "with_items" in kwargs:
-                arguments += self._get_deduped_params_from_items(parameter_names, kwargs["with_items"])
-
-            # it is possible for the user to pass `arguments` via `kwargs` along with `with_param`. The `with_param`
-            # additional parameters are inferred and have to be added to the `kwargs['arguments']` for otherwise
-            # the task will miss adding them when building the final arguments
-            kwargs["arguments"] = arguments
-
             return Task(*args, template=self, **kwargs)
         except InvalidType:
             pass
 
         raise InvalidTemplateCall("Container is not under a Steps, Parallel, or DAG context")
 
     def _get_arguments(self, **kwargs) -> List:
@@ -660,21 +661,26 @@
     See https://argoproj.github.io/argo-workflows/workflow-concepts/#template-invocators for
     more on template invocators
     """
 
     name: str
     continue_on: Optional[ContinueOn] = None
     hooks: Optional[Dict[str, LifecycleHook]] = None
-    on_exit: Optional[str] = None
+    on_exit: Optional[Union[str, Templatable]] = None
     template: Optional[Union[str, Template, TemplateMixin]] = None
     template_ref: Optional[TemplateRef] = None
     inline: Optional[Union[Template, TemplateMixin]] = None
     when: Optional[str] = None
     with_sequence: Optional[Sequence] = None
 
+    def _build_on_exit(self) -> Optional[str]:
+        if isinstance(self.on_exit, Templatable):
+            return self.on_exit._build_template().name  # type: ignore
+        return self.on_exit
+
     @property
     def _subtype(self) -> str:
         raise NotImplementedError
 
     @property
     def id(self) -> str:
         """ID of this node."""
@@ -706,14 +712,17 @@
         return f"{{{{{self._subtype}.{self.name}.finishedAt}}}}"
 
     @property
     def result(self) -> str:
         """Result holds the result (stdout) of a script template."""
         return f"{{{{{self._subtype}.{self.name}.outputs.result}}}}"
 
+    def get_result_as(self, name: str) -> Parameter:
+        return Parameter(name=name, value=self.result)
+
     @root_validator(pre=False)
     def _check_values(cls, values):
         def one(xs: List):
             xs = list(map(bool, xs))
             return xs.count(True) == 1
 
         if not one([values.get("template"), values.get("template_ref"), values.get("inline")]):
```

### Comparing `hera-5.3.0/src/hera/workflows/_unparse.py` & `hera-5.4.0/src/hera/workflows/_unparse.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/archive.py` & `hera-5.4.0/src/hera/workflows/archive.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/artifact.py` & `hera-5.4.0/src/hera/workflows/artifact.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/container.py` & `hera-5.4.0/src/hera/workflows/container.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/container_set.py` & `hera-5.4.0/src/hera/workflows/container_set.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/cron_workflow.py` & `hera-5.4.0/src/hera/workflows/cron_workflow.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/dag.py` & `hera-5.4.0/src/hera/workflows/dag.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/data.py` & `hera-5.4.0/src/hera/workflows/data.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/env.py` & `hera-5.4.0/src/hera/workflows/env.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/env_from.py` & `hera-5.4.0/src/hera/workflows/env_from.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/http_template.py` & `hera-5.4.0/src/hera/workflows/http_template.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/metrics.py` & `hera-5.4.0/src/hera/workflows/metrics.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/__init__.py` & `hera-5.4.0/src/hera/workflows/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/eventsource.py` & `hera-5.4.0/src/hera/workflows/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/eventsource.pyi` & `hera-5.4.0/src/hera/workflows/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/grpc/gateway/runtime.py` & `hera-5.4.0/src/hera/workflows/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.py` & `hera-5.4.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi` & `hera-5.4.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py` & `hera-5.4.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi` & `hera-5.4.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/io/k8s/api/core/v1.py` & `hera-5.4.0/src/hera/workflows/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/io/k8s/api/core/v1.pyi` & `hera-5.4.0/src/hera/workflows/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py` & `hera-5.4.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera-5.4.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/sensor.py` & `hera-5.4.0/src/hera/workflows/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/models/sensor.pyi` & `hera-5.4.0/src/hera/workflows/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/operator.py` & `hera-5.4.0/src/hera/workflows/operator.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/parameter.py` & `hera-5.4.0/src/hera/workflows/parameter.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/protocol.py` & `hera-5.4.0/src/hera/workflows/protocol.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/resource.py` & `hera-5.4.0/src/hera/workflows/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/resources.py` & `hera-5.4.0/src/hera/workflows/resources.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/retry_strategy.py` & `hera-5.4.0/src/hera/workflows/retry_strategy.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/runner.py` & `hera-5.4.0/src/hera/workflows/runner.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/script.py` & `hera-5.4.0/src/hera/workflows/script.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/service.py` & `hera-5.4.0/src/hera/workflows/service.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/steps.py` & `hera-5.4.0/src/hera/workflows/steps.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         return _ModelWorkflowStep(
             arguments=self._build_arguments(),
             continue_on=self.continue_on,
             hooks=self.hooks,
             inline=_inline,
             name=self.name,
-            on_exit=self.on_exit,
+            on_exit=self._build_on_exit(),
             template=_template,
             template_ref=self.template_ref,
             when=self.when,
             with_items=self._build_with_items(),
             with_param=self._build_with_param(),
             with_sequence=self.with_sequence,
         )
```

### Comparing `hera-5.3.0/src/hera/workflows/suspend.py` & `hera-5.4.0/src/hera/workflows/suspend.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/task.py` & `hera-5.4.0/src/hera/workflows/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,69 +43,100 @@
 class Task(
     TemplateInvocatorSubNodeMixin,
     ArgumentsMixin,
     SubNodeMixin,
     ParameterMixin,
     ItemMixin,
 ):
-    r"""Task is used to run a given template within a DAG. Must be instantiated under a DAG context.
+    """Task is used to run a given template within a DAG. Must be instantiated under a DAG context.
 
-    ## Dependencies
-    Any Tasks without a dependency defined will start immediately.
+## Dependencies
 
-    Dependencies between Tasks can be described using the convenience syntax `>>`, for example:
-        A = Task(...)
-        B = Task(...)
-        A >> B
-    describes the relationships:
-    * "A has no dependencies (so starts immediately)
-    * "B depends on A".
-    As a diagram:
-    A
-    |
-    B
-
-    `A >> B` is equivalent to `A.next(B)`.
-
-    ## Lists of Tasks
-    A list of Tasks used with the rshift syntax describes an "AND" dependency between the single Task on the left of
-    `>>` and the list Tasks to the right of `>>` (or vice versa). A list of Tasks on both sides of `>>` is not supported.
-    For example:
-        A = Task(...)
-        B = Task(...)
-        C = Task(...)
-        D = Task(...)
-        A >> [B, C] >> D
-    describes the relationships:
-    * "A has no dependencies
-    * "B AND C depend on A"
-    * "D depends on B AND C"
-    As a diagram:
-      A
-     / \
-    B   C
-     \ /
-      D
-
-    Dependencies can be described over multiple statements:
-        A = Task(...)
-        B = Task(...)
-        C = Task(...)
-        D = Task(...)
-        A >> [C, D]
-        B >> [C, D]
-    describes the relationships:
-    * "A and B have no dependencies
-    * "C depends on A AND B"
-    * "D depends on A AND B"
-    As a diagram:
-    A   B
-    | X |
-    C   D
+Any `Tasks` without a dependency defined will start immediately.
+
+Dependencies between Tasks can be described using the convenience syntax `>>`, for example:
+
+```py
+    A = Task(...)
+    B = Task(...)
+    A >> B
+```
+
+describes the relationships:
+
+* "A has no dependencies (so starts immediately)
+* "B depends on A".
+
+As a diagram:
+
+```
+A
+|
+B
+```
+
+`A >> B` is equivalent to `A.next(B)`.
+
+## Lists of Tasks
+
+A list of Tasks used with the rshift syntax describes an "AND" dependency between the single Task on the left of
+`>>` and the list Tasks to the right of `>>` (or vice versa). A list of Tasks on both sides of `>>` is not supported.
+
+For example:
+
+```
+    A = Task(...)
+    B = Task(...)
+    C = Task(...)
+    D = Task(...)
+    A >> [B, C] >> D
+```
+
+describes the relationships:
+
+* "A has no dependencies
+* "B AND C depend on A"
+* "D depends on B AND C"
+
+As a diagram:
+
+```
+  A
+ / \\
+B   C
+ \ /
+  D
+```
+
+Dependencies can be described over multiple statements:
+
+```
+    A = Task(...)
+    B = Task(...)
+    C = Task(...)
+    D = Task(...)
+    A >> [C, D]
+    B >> [C, D]
+```
+
+describes the relationships:
+
+* "A and B have no dependencies
+* "C depends on A AND B"
+* "D depends on A AND B"
+
+As a diagram:
+
+```
+A   B
+| X |
+C   D
+```
     """
+
     dependencies: Optional[List[str]] = None
     depends: Optional[str] = None
 
     def _get_dependency_tasks(self) -> List[str]:
         if self.depends is None:
             return []
 
@@ -230,15 +261,15 @@
             arguments=self._build_arguments(),
             continue_on=self.continue_on,
             dependencies=self.dependencies,
             depends=self.depends,
             hooks=self.hooks,
             inline=_inline,
             name=self.name,
-            on_exit=self.on_exit,
+            on_exit=self._build_on_exit(),
             template=_template,
             template_ref=self.template_ref,
             when=self.when,
             with_items=self._build_with_items(),
             with_param=self._build_with_param(),
             with_sequence=self.with_sequence,
         )
```

### Comparing `hera-5.3.0/src/hera/workflows/user_container.py` & `hera-5.4.0/src/hera/workflows/user_container.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/validators.py` & `hera-5.4.0/src/hera/workflows/validators.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/volume.py` & `hera-5.4.0/src/hera/workflows/volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 
     def __str__(self):
         return str(self.value)
 
 
 class _BaseVolume(_ModelVolumeMount):
     name: Optional[str] = None  # type: ignore
+    mount_path: Optional[str] = None  # type: ignore
 
     @validator("name", pre=True)
     def _check_name(cls, v):
         if v is None:
             return str(uuid.uuid4())
         return v
```

### Comparing `hera-5.3.0/src/hera/workflows/workflow.py` & `hera-5.4.0/src/hera/workflows/workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     WorkflowCreateRequest,
     WorkflowLintRequest,
     WorkflowMetadata,
     WorkflowSpec as _ModelWorkflowSpec,
     WorkflowStatus as _ModelWorkflowStatus,
     WorkflowTemplateRef,
 )
+from hera.workflows.parameter import Parameter
 from hera.workflows.protocol import Templatable, TTemplate, TWorkflow, VolumeClaimable
 from hera.workflows.service import WorkflowsService
 from hera.workflows.workflow_status import WorkflowStatus
 
 _yaml: Optional[ModuleType] = None
 try:
     import yaml
@@ -116,15 +117,15 @@
     entrypoint: Optional[str] = None
     executor: Optional[ExecutorConfig] = None
     hooks: Optional[Dict[str, LifecycleHook]] = None
     host_aliases: Optional[List[HostAlias]] = None
     host_network: Optional[bool] = None
     image_pull_secrets: ImagePullSecrets = None
     node_selector: Optional[Dict[str, str]] = None
-    on_exit: Optional[str] = None
+    on_exit: Optional[Union[str, Templatable]] = None
     parallelism: Optional[int] = None
     pod_disruption_budget: Optional[PodDisruptionBudgetSpec] = None
     pod_gc: Optional[PodGC] = None
     pod_metadata: Optional[Metadata] = None
     pod_priority: Optional[int] = None
     pod_priority_class_name: Optional[str] = None
     pod_spec_patch: Optional[str] = None
@@ -240,14 +241,31 @@
                         new_volume_claims_map[claim.metadata.name] = claim
 
                     for claim_name, claim in new_volume_claims_map.items():
                         if claim_name not in current_volume_claims_map:
                             self.volume_claim_templates.append(claim)
         return templates
 
+    def _build_on_exit(self) -> Optional[str]:
+        if isinstance(self.on_exit, Templatable):
+            return self.on_exit._build_template().name  # type: ignore
+        return self.on_exit
+
+    def get_parameter(self, name: str) -> Parameter:
+        arguments = self._build_arguments()
+        if arguments is None:
+            raise KeyError("Workflow has no arguments set")
+        if arguments.parameters is None:
+            raise KeyError("Workflow has no argument parameters set")
+
+        parameters = arguments.parameters
+        if next((p for p in parameters if p.name == name), None) is None:
+            raise KeyError(f"`{name}` is not a valid workflow parameter")
+        return Parameter(name=name, value=f"{{{{workflow.parameters.{name}}}}}")
+
     def build(self) -> TWorkflow:
         """Builds the Workflow and its components into an Argo schema Workflow object."""
         self = self._dispatch_hooks()
 
         templates = self._build_templates()
         workflow_claims = self._build_persistent_volume_claims()
         volume_claim_templates = (self.volume_claim_templates or []) + (workflow_claims or [])
@@ -286,15 +304,15 @@
                 executor=self.executor,
                 hooks=self.hooks,
                 host_aliases=self.host_aliases,
                 host_network=self.host_network,
                 image_pull_secrets=self.image_pull_secrets,
                 metrics=self._build_metrics(),
                 node_selector=self.node_selector,
-                on_exit=self.on_exit,
+                on_exit=self._build_on_exit(),
                 parallelism=self.parallelism,
                 pod_disruption_budget=self.pod_disruption_budget,
                 pod_gc=self.pod_gc,
                 pod_metadata=self.pod_metadata,
                 pod_priority=self.pod_priority,
                 pod_priority_class_name=self.pod_priority_class_name,
                 pod_spec_patch=self.pod_spec_patch,
```

### Comparing `hera-5.3.0/src/hera/workflows/workflow_status.py` & `hera-5.4.0/src/hera/workflows/workflow_status.py`

 * *Files identical despite different names*

### Comparing `hera-5.3.0/src/hera/workflows/workflow_template.py` & `hera-5.4.0/src/hera/workflows/workflow_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                 executor=self.executor,
                 hooks=self.hooks,
                 host_aliases=self.host_aliases,
                 host_network=self.host_network,
                 image_pull_secrets=self.image_pull_secrets,
                 metrics=self._build_metrics(),
                 node_selector=self.node_selector,
-                on_exit=self.on_exit,
+                on_exit=self._build_on_exit(),
                 parallelism=self.parallelism,
                 pod_disruption_budget=self.pod_disruption_budget,
                 pod_gc=self.pod_gc,
                 pod_metadata=self.pod_metadata,
                 pod_priority=self.pod_priority,
                 pod_priority_class_name=self.pod_priority_class_name,
                 pod_spec_patch=self.pod_spec_patch,
```

### Comparing `hera-5.3.0/PKG-INFO` & `hera-5.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera
-Version: 5.3.0
+Version: 5.4.0
 Summary: Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows.
 Home-page: https://github.com/argoproj-labs/hera
 License: MIT
 Author: Flaviu Vadan
 Author-email: flaviu.vadan@dynotx.com
 Maintainer: Flaviu Vadan
 Maintainer-email: flaviu.vadan@dynotx.com
```

