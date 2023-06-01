# Comparing `tmp/google-cloud-talent-2.9.0.tar.gz` & `tmp/google-cloud-talent-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-talent-2.9.0.tar", last modified: Tue Jan 10 17:29:17 2023, max compression
+gzip compressed data, was "google-cloud-talent-2.9.1.tar", last modified: Mon Jan 23 15:38:00 2023, max compression
```

## Comparing `google-cloud-talent-2.9.0.tar` & `google-cloud-talent-2.9.1.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.952717 google-cloud-talent-2.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4684 2023-01-10 17:29:17.952717 google-cloud-talent-2.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3771 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.920701 google-cloud-talent-2.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.920701 google-cloud-talent-2.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.924703 google-cloud-talent-2.9.0/google/cloud/talent/
--rw-rw-r--   0 root         (0)     1003     5286 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.924703 google-cloud-talent-2.9.0/google/cloud/talent_v4/
--rw-rw-r--   0 root         (0)     1003     4450 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/__init__.py
--rw-rw-r--   0 root         (0)     1003     6954 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.928705 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.928705 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/
--rw-rw-r--   0 root         (0)     1003      769 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    33899 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    42871 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/client.py
--rw-rw-r--   0 root         (0)     1003     5788 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.928705 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9163 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16308 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16638 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.928705 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/
--rw-rw-r--   0 root         (0)     1003      753 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/__init__.py
--rw-rw-r--   0 root         (0)     1003    12811 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/async_client.py
--rw-rw-r--   0 root         (0)     1003    21921 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.928705 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/transports/
--rw-rw-r--   0 root         (0)     1003     1157 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6528 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11835 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12036 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.928705 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/
--rw-rw-r--   0 root         (0)     1003      761 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    15037 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    23926 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.932707 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/transports/
--rw-rw-r--   0 root         (0)     1003     1175 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6069 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12055 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12272 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.932707 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/
--rw-rw-r--   0 root         (0)     1003      753 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    58824 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    69034 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/client.py
--rw-rw-r--   0 root         (0)     1003     5574 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.932707 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/transports/
--rw-rw-r--   0 root         (0)     1003     1157 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11384 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    23366 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23939 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.932707 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    33332 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    41746 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/client.py
--rw-rw-r--   0 root         (0)     1003     5712 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.936709 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/transports/
--rw-rw-r--   0 root         (0)     1003     1184 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9109 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16111 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16427 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.936709 google-cloud-talent-2.9.0/google/cloud/talent_v4/types/
--rw-rw-r--   0 root         (0)     1003     3589 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    29765 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/types/common.py
--rw-rw-r--   0 root         (0)     1003     6276 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/types/company.py
--rw-rw-r--   0 root         (0)     1003     6218 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/types/company_service.py
--rw-rw-r--   0 root         (0)     1003     5355 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/types/completion_service.py
--rw-rw-r--   0 root         (0)     1003     4841 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/types/event.py
--rw-rw-r--   0 root         (0)     1003     1678 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/types/event_service.py
--rw-rw-r--   0 root         (0)     1003    20058 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/types/filters.py
--rw-rw-r--   0 root         (0)     1003     2515 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/types/histogram.py
--rw-rw-r--   0 root         (0)     1003    23587 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/types/job.py
--rw-rw-r--   0 root         (0)     1003    45564 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/types/job_service.py
--rw-rw-r--   0 root         (0)     1003     1814 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/types/tenant.py
--rw-rw-r--   0 root         (0)     1003     5531 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4/types/tenant_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.936709 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/
--rw-rw-r--   0 root         (0)     1003     4288 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6964 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.936709 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.940711 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/
--rw-rw-r--   0 root         (0)     1003      769 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    35484 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    44036 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/client.py
--rw-rw-r--   0 root         (0)     1003     5833 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.940711 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9467 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17223 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17553 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.940711 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/
--rw-rw-r--   0 root         (0)     1003      753 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/__init__.py
--rw-rw-r--   0 root         (0)     1003    14791 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/async_client.py
--rw-rw-r--   0 root         (0)     1003    23472 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.940711 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/transports/
--rw-rw-r--   0 root         (0)     1003     1157 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6822 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12720 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12921 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.940711 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/
--rw-rw-r--   0 root         (0)     1003      761 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17282 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    26284 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.940711 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/transports/
--rw-rw-r--   0 root         (0)     1003     1175 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6363 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12940 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13157 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.944713 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/
--rw-rw-r--   0 root         (0)     1003      753 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    60935 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    70717 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/client.py
--rw-rw-r--   0 root         (0)     1003    15659 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.944713 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/transports/
--rw-rw-r--   0 root         (0)     1003     1157 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11624 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24268 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24827 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.944713 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    34553 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    42948 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/client.py
--rw-rw-r--   0 root         (0)     1003     5757 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.944713 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/transports/
--rw-rw-r--   0 root         (0)     1003     1184 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9413 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17026 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17342 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.948715 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/
--rw-rw-r--   0 root         (0)     1003     3427 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003      742 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/batch.py
--rw-rw-r--   0 root         (0)     1003    29923 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/common.py
--rw-rw-r--   0 root         (0)     1003     6446 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/company.py
--rw-rw-r--   0 root         (0)     1003     6773 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/company_service.py
--rw-rw-r--   0 root         (0)     1003     5626 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/completion_service.py
--rw-rw-r--   0 root         (0)     1003     5290 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/event.py
--rw-rw-r--   0 root         (0)     1003     1803 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/event_service.py
--rw-rw-r--   0 root         (0)     1003    20583 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/filters.py
--rw-rw-r--   0 root         (0)     1003     2704 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/histogram.py
--rw-rw-r--   0 root         (0)     1003    23556 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/job.py
--rw-rw-r--   0 root         (0)     1003    45659 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/job_service.py
--rw-rw-r--   0 root         (0)     1003     3290 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/tenant.py
--rw-rw-r--   0 root         (0)     1003     5581 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/tenant_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.948715 google-cloud-talent-2.9.0/google_cloud_talent.egg-info/
--rw-r--r--   0 root         (0)     1003     4684 2023-01-10 17:29:17.000000 google-cloud-talent-2.9.0/google_cloud_talent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     7722 2023-01-10 17:29:17.000000 google-cloud-talent-2.9.0/google_cloud_talent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-10 17:29:17.000000 google-cloud-talent-2.9.0/google_cloud_talent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-10 17:29:17.000000 google-cloud-talent-2.9.0/google_cloud_talent.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-10 17:29:17.000000 google-cloud-talent-2.9.0/google_cloud_talent.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-10 17:29:17.000000 google-cloud-talent-2.9.0/google_cloud_talent.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-10 17:29:17.000000 google-cloud-talent-2.9.0/google_cloud_talent.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-10 17:29:17.952717 google-cloud-talent-2.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2970 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.948715 google-cloud-talent-2.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.948715 google-cloud-talent-2.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.948715 google-cloud-talent-2.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.952717 google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4/__init__.py
--rw-rw-r--   0 root         (0)     1003   107018 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4/test_company_service.py
--rw-rw-r--   0 root         (0)     1003    55782 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4/test_completion.py
--rw-rw-r--   0 root         (0)     1003    59718 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4/test_event_service.py
--rw-rw-r--   0 root         (0)     1003   148931 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4/test_job_service.py
--rw-rw-r--   0 root         (0)     1003    98437 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4/test_tenant_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 17:29:17.952717 google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   111373 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4beta1/test_company_service.py
--rw-rw-r--   0 root         (0)     1003    60680 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4beta1/test_completion.py
--rw-rw-r--   0 root         (0)     1003    65327 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4beta1/test_event_service.py
--rw-rw-r--   0 root         (0)     1003   167135 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4beta1/test_job_service.py
--rw-rw-r--   0 root         (0)     1003   105953 2023-01-10 17:26:33.000000 google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4beta1/test_tenant_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.326657 google-cloud-talent-2.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4684 2023-01-23 15:38:00.326657 google-cloud-talent-2.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3771 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.294654 google-cloud-talent-2.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.298654 google-cloud-talent-2.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.298654 google-cloud-talent-2.9.1/google/cloud/talent/
+-rw-rw-r--   0 root         (0)     1003     5286 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.302655 google-cloud-talent-2.9.1/google/cloud/talent_v4/
+-rw-rw-r--   0 root         (0)     1003     4450 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6954 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.302655 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.302655 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/
+-rw-rw-r--   0 root         (0)     1003      769 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    33899 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    42897 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5788 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.302655 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9163 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16308 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16638 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.302655 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/
+-rw-rw-r--   0 root         (0)     1003      753 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12811 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/async_client.py
+-rw-rw-r--   0 root         (0)     1003    21943 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.302655 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/transports/
+-rw-rw-r--   0 root         (0)     1003     1157 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6528 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    11835 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12036 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.306655 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/
+-rw-rw-r--   0 root         (0)     1003      761 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15037 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    23950 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.306655 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1175 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6069 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12055 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12272 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.306655 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/
+-rw-rw-r--   0 root         (0)     1003      753 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    58881 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    69113 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5574 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.306655 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1157 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11384 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    23366 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23939 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.306655 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    33332 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    41771 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5712 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.306655 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1184 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9109 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16111 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16427 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.310655 google-cloud-talent-2.9.1/google/cloud/talent_v4/types/
+-rw-rw-r--   0 root         (0)     1003     3589 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    48409 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/types/common.py
+-rw-rw-r--   0 root         (0)     1003     6276 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/types/company.py
+-rw-rw-r--   0 root         (0)     1003     6218 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/types/company_service.py
+-rw-rw-r--   0 root         (0)     1003     7214 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/types/completion_service.py
+-rw-rw-r--   0 root         (0)     1003    10653 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/types/event.py
+-rw-rw-r--   0 root         (0)     1003     1678 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/types/event_service.py
+-rw-rw-r--   0 root         (0)     1003    23405 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/types/filters.py
+-rw-rw-r--   0 root         (0)     1003     2515 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/types/histogram.py
+-rw-rw-r--   0 root         (0)     1003    23587 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/types/job.py
+-rw-rw-r--   0 root         (0)     1003    52602 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/types/job_service.py
+-rw-rw-r--   0 root         (0)     1003     1815 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/types/tenant.py
+-rw-rw-r--   0 root         (0)     1003     5531 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4/types/tenant_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.310655 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/
+-rw-rw-r--   0 root         (0)     1003     4288 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6964 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.310655 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.314656 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/
+-rw-rw-r--   0 root         (0)     1003      769 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    35484 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    44062 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5833 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.314656 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9467 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17223 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17553 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.314656 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/
+-rw-rw-r--   0 root         (0)     1003      753 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14791 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/async_client.py
+-rw-rw-r--   0 root         (0)     1003    23494 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.314656 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/transports/
+-rw-rw-r--   0 root         (0)     1003     1157 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6822 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12720 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12921 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.314656 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/
+-rw-rw-r--   0 root         (0)     1003      761 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17282 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26308 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.314656 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1175 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6363 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12940 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13157 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.318656 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/
+-rw-rw-r--   0 root         (0)     1003      753 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    61011 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    70815 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/client.py
+-rw-rw-r--   0 root         (0)     1003    15659 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.318656 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1157 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11624 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24268 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24827 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.318656 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    34553 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    42973 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5757 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.318656 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1184 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9413 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17026 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17342 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.322656 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/
+-rw-rw-r--   0 root         (0)     1003     3427 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003      742 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/batch.py
+-rw-rw-r--   0 root         (0)     1003    48464 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/common.py
+-rw-rw-r--   0 root         (0)     1003     6446 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/company.py
+-rw-rw-r--   0 root         (0)     1003     6773 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/company_service.py
+-rw-rw-r--   0 root         (0)     1003     7520 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/completion_service.py
+-rw-rw-r--   0 root         (0)     1003    11132 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/event.py
+-rw-rw-r--   0 root         (0)     1003     1803 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/event_service.py
+-rw-rw-r--   0 root         (0)     1003    23990 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/filters.py
+-rw-rw-r--   0 root         (0)     1003     2704 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/histogram.py
+-rw-rw-r--   0 root         (0)     1003    23556 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/job.py
+-rw-rw-r--   0 root         (0)     1003    52244 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/job_service.py
+-rw-rw-r--   0 root         (0)     1003     3706 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/tenant.py
+-rw-rw-r--   0 root         (0)     1003     5581 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/tenant_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.322656 google-cloud-talent-2.9.1/google_cloud_talent.egg-info/
+-rw-r--r--   0 root         (0)     1003     4684 2023-01-23 15:38:00.000000 google-cloud-talent-2.9.1/google_cloud_talent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     7722 2023-01-23 15:38:00.000000 google-cloud-talent-2.9.1/google_cloud_talent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:38:00.000000 google-cloud-talent-2.9.1/google_cloud_talent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-01-23 15:38:00.000000 google-cloud-talent-2.9.1/google_cloud_talent.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:38:00.000000 google-cloud-talent-2.9.1/google_cloud_talent.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-01-23 15:38:00.000000 google-cloud-talent-2.9.1/google_cloud_talent.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-01-23 15:38:00.000000 google-cloud-talent-2.9.1/google_cloud_talent.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-01-23 15:38:00.326657 google-cloud-talent-2.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2970 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.322656 google-cloud-talent-2.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.322656 google-cloud-talent-2.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.322656 google-cloud-talent-2.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.326657 google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4/__init__.py
+-rw-rw-r--   0 root         (0)     1003   107018 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4/test_company_service.py
+-rw-rw-r--   0 root         (0)     1003    55782 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4/test_completion.py
+-rw-rw-r--   0 root         (0)     1003    59718 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4/test_event_service.py
+-rw-rw-r--   0 root         (0)     1003   148931 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4/test_job_service.py
+-rw-rw-r--   0 root         (0)     1003    98437 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4/test_tenant_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:38:00.326657 google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   111373 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4beta1/test_company_service.py
+-rw-rw-r--   0 root         (0)     1003    60680 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4beta1/test_completion.py
+-rw-rw-r--   0 root         (0)     1003    65327 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4beta1/test_event_service.py
+-rw-rw-r--   0 root         (0)     1003   167135 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4beta1/test_job_service.py
+-rw-rw-r--   0 root         (0)     1003   105953 2023-01-23 15:35:14.000000 google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4beta1/test_tenant_service.py
```

### Comparing `google-cloud-talent-2.9.0/LICENSE` & `google-cloud-talent-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/MANIFEST.in` & `google-cloud-talent-2.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/PKG-INFO` & `google-cloud-talent-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-talent
-Version: 2.9.0
+Version: 2.9.1
 Summary: Google Cloud Talent API client library
 Home-page: https://github.com/googleapis/python-talent
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-talent-2.9.0/README.rst` & `google-cloud-talent-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent/gapic_version.py` & `google-cloud-talent-2.9.1/google/cloud/talent/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/gapic_metadata.json` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/gapic_version.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/async_client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1040,15 +1040,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "CompanyServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/pagers.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/transports/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/transports/base.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/transports/grpc.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/company_service/transports/grpc_asyncio.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/company_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/async_client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -533,15 +533,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "CompletionClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/transports/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/transports/base.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/transports/grpc.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/completion/transports/grpc_asyncio.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/completion/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/async_client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -567,15 +567,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "EventServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/transports/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/transports/base.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/transports/grpc.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/event_service/transports/grpc_asyncio.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/event_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/async_client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,16 +423,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.talent_v4.types.BatchCreateJobsResponse` The result of [JobService.BatchCreateJobs][google.cloud.talent.v4.JobService.BatchCreateJobs]. It's used to
-                   replace
+                The result type for the operation will be :class:`google.cloud.talent_v4.types.BatchCreateJobsResponse` The result of
+                   [JobService.BatchCreateJobs][google.cloud.talent.v4.JobService.BatchCreateJobs].
+                   It's used to replace
                    [google.longrunning.Operation.response][google.longrunning.Operation.response]
                    in case of success.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -808,16 +809,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.talent_v4.types.BatchUpdateJobsResponse` The result of [JobService.BatchUpdateJobs][google.cloud.talent.v4.JobService.BatchUpdateJobs]. It's used to
-                   replace
+                The result type for the operation will be :class:`google.cloud.talent_v4.types.BatchUpdateJobsResponse` The result of
+                   [JobService.BatchUpdateJobs][google.cloud.talent.v4.JobService.BatchUpdateJobs].
+                   It's used to replace
                    [google.longrunning.Operation.response][google.longrunning.Operation.response]
                    in case of success.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -1051,16 +1053,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.talent_v4.types.BatchDeleteJobsResponse` The result of [JobService.BatchDeleteJobs][google.cloud.talent.v4.JobService.BatchDeleteJobs]. It's used to
-                   replace
+                The result type for the operation will be :class:`google.cloud.talent_v4.types.BatchDeleteJobsResponse` The result of
+                   [JobService.BatchDeleteJobs][google.cloud.talent.v4.JobService.BatchDeleteJobs].
+                   It's used to replace
                    [google.longrunning.Operation.response][google.longrunning.Operation.response]
                    in case of success.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -689,16 +689,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.talent_v4.types.BatchCreateJobsResponse` The result of [JobService.BatchCreateJobs][google.cloud.talent.v4.JobService.BatchCreateJobs]. It's used to
-                   replace
+                The result type for the operation will be :class:`google.cloud.talent_v4.types.BatchCreateJobsResponse` The result of
+                   [JobService.BatchCreateJobs][google.cloud.talent.v4.JobService.BatchCreateJobs].
+                   It's used to replace
                    [google.longrunning.Operation.response][google.longrunning.Operation.response]
                    in case of success.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -1064,16 +1065,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.talent_v4.types.BatchUpdateJobsResponse` The result of [JobService.BatchUpdateJobs][google.cloud.talent.v4.JobService.BatchUpdateJobs]. It's used to
-                   replace
+                The result type for the operation will be :class:`google.cloud.talent_v4.types.BatchUpdateJobsResponse` The result of
+                   [JobService.BatchUpdateJobs][google.cloud.talent.v4.JobService.BatchUpdateJobs].
+                   It's used to replace
                    [google.longrunning.Operation.response][google.longrunning.Operation.response]
                    in case of success.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -1297,16 +1299,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.talent_v4.types.BatchDeleteJobsResponse` The result of [JobService.BatchDeleteJobs][google.cloud.talent.v4.JobService.BatchDeleteJobs]. It's used to
-                   replace
+                The result type for the operation will be :class:`google.cloud.talent_v4.types.BatchDeleteJobsResponse` The result of
+                   [JobService.BatchDeleteJobs][google.cloud.talent.v4.JobService.BatchDeleteJobs].
+                   It's used to replace
                    [google.longrunning.Operation.response][google.longrunning.Operation.response]
                    in case of success.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -1684,15 +1687,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "JobServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/pagers.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/transports/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/transports/base.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/transports/grpc.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/job_service/transports/grpc_asyncio.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/job_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/async_client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1010,15 +1010,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "TenantServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/pagers.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/transports/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/transports/base.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/transports/grpc.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/services/tenant_service/transports/grpc_asyncio.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/services/tenant_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/types/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/types/common.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/types/job.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,842 +12,559 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
-from google.protobuf import wrappers_pb2  # type: ignore
-from google.type import latlng_pb2  # type: ignore
-from google.type import money_pb2  # type: ignore
-from google.type import postal_address_pb2  # type: ignore
 import proto  # type: ignore
 
+from google.cloud.talent_v4.types import common
+
 __protobuf__ = proto.module(
     package="google.cloud.talent.v4",
     manifest={
-        "CompanySize",
-        "JobBenefit",
-        "DegreeType",
-        "EmploymentType",
-        "JobLevel",
-        "JobCategory",
-        "PostingRegion",
-        "Visibility",
-        "HtmlSanitization",
-        "CommuteMethod",
-        "TimestampRange",
-        "Location",
-        "RequestMetadata",
-        "ResponseMetadata",
-        "DeviceInfo",
-        "CustomAttribute",
-        "SpellingCorrection",
-        "CompensationInfo",
-        "BatchOperationMetadata",
+        "Job",
     },
 )
 
 
-class CompanySize(proto.Enum):
-    r"""An enum that represents the size of the company."""
-    COMPANY_SIZE_UNSPECIFIED = 0
-    MINI = 1
-    SMALL = 2
-    SMEDIUM = 3
-    MEDIUM = 4
-    BIG = 5
-    BIGGER = 6
-    GIANT = 7
+class Job(proto.Message):
+    r"""A Job resource represents a job posting (also referred to as a "job
+    listing" or "job requisition"). A job belongs to a
+    [Company][google.cloud.talent.v4.Company], which is the hiring
+    entity responsible for the job.
 
+    Attributes:
+        name (str):
+            Required during job update.
 
-class JobBenefit(proto.Enum):
-    r"""An enum that represents employee benefits included with the
-    job.
-    """
-    JOB_BENEFIT_UNSPECIFIED = 0
-    CHILD_CARE = 1
-    DENTAL = 2
-    DOMESTIC_PARTNER = 3
-    FLEXIBLE_HOURS = 4
-    MEDICAL = 5
-    LIFE_INSURANCE = 6
-    PARENTAL_LEAVE = 7
-    RETIREMENT_PLAN = 8
-    SICK_DAYS = 9
-    VACATION = 10
-    VISION = 11
-
-
-class DegreeType(proto.Enum):
-    r"""Educational degree level defined in International Standard
-    Classification of Education (ISCED).
-    """
-    DEGREE_TYPE_UNSPECIFIED = 0
-    PRIMARY_EDUCATION = 1
-    LOWER_SECONDARY_EDUCATION = 2
-    UPPER_SECONDARY_EDUCATION = 3
-    ADULT_REMEDIAL_EDUCATION = 4
-    ASSOCIATES_OR_EQUIVALENT = 5
-    BACHELORS_OR_EQUIVALENT = 6
-    MASTERS_OR_EQUIVALENT = 7
-    DOCTORAL_OR_EQUIVALENT = 8
-
-
-class EmploymentType(proto.Enum):
-    r"""An enum that represents the employment type of a job."""
-    EMPLOYMENT_TYPE_UNSPECIFIED = 0
-    FULL_TIME = 1
-    PART_TIME = 2
-    CONTRACTOR = 3
-    CONTRACT_TO_HIRE = 4
-    TEMPORARY = 5
-    INTERN = 6
-    VOLUNTEER = 7
-    PER_DIEM = 8
-    FLY_IN_FLY_OUT = 9
-    OTHER_EMPLOYMENT_TYPE = 10
-
-
-class JobLevel(proto.Enum):
-    r"""An enum that represents the required experience level
-    required for the job.
-    """
-    JOB_LEVEL_UNSPECIFIED = 0
-    ENTRY_LEVEL = 1
-    EXPERIENCED = 2
-    MANAGER = 3
-    DIRECTOR = 4
-    EXECUTIVE = 5
+            The resource name for the job. This is generated by the
+            service when a job is created.
 
+            The format is
+            "projects/{project_id}/tenants/{tenant_id}/jobs/{job_id}".
+            For example, "projects/foo/tenants/bar/jobs/baz".
+
+            Use of this field in job queries and API calls is preferred
+            over the use of
+            [requisition_id][google.cloud.talent.v4.Job.requisition_id]
+            since this value is unique.
+        company (str):
+            Required. The resource name of the company listing the job.
+
+            The format is
+            "projects/{project_id}/tenants/{tenant_id}/companies/{company_id}".
+            For example, "projects/foo/tenants/bar/companies/baz".
+        requisition_id (str):
+            Required. The requisition ID, also referred to as the
+            posting ID, is assigned by the client to identify a job.
+            This field is intended to be used by clients for client
+            identification and tracking of postings. A job isn't allowed
+            to be created if there is another job with the same
+            [company][google.cloud.talent.v4.Job.name],
+            [language_code][google.cloud.talent.v4.Job.language_code]
+            and
+            [requisition_id][google.cloud.talent.v4.Job.requisition_id].
 
-class JobCategory(proto.Enum):
-    r"""An enum that represents the categorization or primary focus
-    of specific role. This value is different than the "industry"
-    associated with a role, which is related to the categorization
-    of the company listing the job.
-    """
-    JOB_CATEGORY_UNSPECIFIED = 0
-    ACCOUNTING_AND_FINANCE = 1
-    ADMINISTRATIVE_AND_OFFICE = 2
-    ADVERTISING_AND_MARKETING = 3
-    ANIMAL_CARE = 4
-    ART_FASHION_AND_DESIGN = 5
-    BUSINESS_OPERATIONS = 6
-    CLEANING_AND_FACILITIES = 7
-    COMPUTER_AND_IT = 8
-    CONSTRUCTION = 9
-    CUSTOMER_SERVICE = 10
-    EDUCATION = 11
-    ENTERTAINMENT_AND_TRAVEL = 12
-    FARMING_AND_OUTDOORS = 13
-    HEALTHCARE = 14
-    HUMAN_RESOURCES = 15
-    INSTALLATION_MAINTENANCE_AND_REPAIR = 16
-    LEGAL = 17
-    MANAGEMENT = 18
-    MANUFACTURING_AND_WAREHOUSE = 19
-    MEDIA_COMMUNICATIONS_AND_WRITING = 20
-    OIL_GAS_AND_MINING = 21
-    PERSONAL_CARE_AND_SERVICES = 22
-    PROTECTIVE_SERVICES = 23
-    REAL_ESTATE = 24
-    RESTAURANT_AND_HOSPITALITY = 25
-    SALES_AND_RETAIL = 26
-    SCIENCE_AND_ENGINEERING = 27
-    SOCIAL_SERVICES_AND_NON_PROFIT = 28
-    SPORTS_FITNESS_AND_RECREATION = 29
-    TRANSPORTATION_AND_LOGISTICS = 30
-
-
-class PostingRegion(proto.Enum):
-    r"""An enum that represents the job posting region. In most
-    cases, job postings don't need to specify a region. If a region
-    is given, jobs are eligible for searches in the specified
-    region.
-    """
-    POSTING_REGION_UNSPECIFIED = 0
-    ADMINISTRATIVE_AREA = 1
-    NATION = 2
-    TELECOMMUTE = 3
+            The maximum number of allowed characters is 255.
+        title (str):
+            Required. The title of the job, such as
+            "Software Engineer"
+            The maximum number of allowed characters is 500.
+        description (str):
+            Required. The description of the job, which typically
+            includes a multi-paragraph description of the company and
+            related information. Separate fields are provided on the job
+            object for
+            [responsibilities][google.cloud.talent.v4.Job.responsibilities],
+            [qualifications][google.cloud.talent.v4.Job.qualifications],
+            and other job characteristics. Use of these separate job
+            fields is recommended.
+
+            This field accepts and sanitizes HTML input, and also
+            accepts bold, italic, ordered list, and unordered list
+            markup tags.
+
+            The maximum number of allowed characters is 100,000.
+        addresses (MutableSequence[str]):
+            Strongly recommended for the best service experience.
+
+            Location(s) where the employer is looking to hire for this
+            job posting.
+
+            Specifying the full street address(es) of the hiring
+            location enables better API results, especially job searches
+            by commute time.
+
+            At most 50 locations are allowed for best search
+            performance. If a job has more locations, it is suggested to
+            split it into multiple jobs with unique
+            [requisition_id][google.cloud.talent.v4.Job.requisition_id]s
+            (e.g. 'ReqA' becomes 'ReqA-1', 'ReqA-2', and so on.) as
+            multiple jobs with the same
+            [company][google.cloud.talent.v4.Job.company],
+            [language_code][google.cloud.talent.v4.Job.language_code]
+            and
+            [requisition_id][google.cloud.talent.v4.Job.requisition_id]
+            are not allowed. If the original
+            [requisition_id][google.cloud.talent.v4.Job.requisition_id]
+            must be preserved, a custom field should be used for
+            storage. It is also suggested to group the locations that
+            close to each other in the same job for better search
+            experience.
+
+            Jobs with multiple addresses must have their addresses with
+            the same [LocationType][] to allow location filtering to
+            work properly. (For example, a Job with addresses "1600
+            Amphitheatre Parkway, Mountain View, CA, USA" and "London,
+            UK" may not have location filters applied correctly at
+            search time since the first is a
+            [LocationType.STREET_ADDRESS][] and the second is a
+            [LocationType.LOCALITY][].) If a job needs to have multiple
+            addresses, it is suggested to split it into multiple jobs
+            with same LocationTypes.
+
+            The maximum number of allowed characters is 500.
+        application_info (google.cloud.talent_v4.types.Job.ApplicationInfo):
+            Job application information.
+        job_benefits (MutableSequence[google.cloud.talent_v4.types.JobBenefit]):
+            The benefits included with the job.
+        compensation_info (google.cloud.talent_v4.types.CompensationInfo):
+            Job compensation information (a.k.a. "pay
+            rate") i.e., the compensation that will paid to
+            the employee.
+        custom_attributes (MutableMapping[str, google.cloud.talent_v4.types.CustomAttribute]):
+            A map of fields to hold both filterable and non-filterable
+            custom job attributes that are not covered by the provided
+            structured fields.
+
+            The keys of the map are strings up to 64 bytes and must
+            match the pattern: ``[a-zA-Z][a-zA-Z0-9_]*``. For example,
+            key0LikeThis or KEY_1_LIKE_THIS.
+
+            At most 100 filterable and at most 100 unfilterable keys are
+            supported. For filterable ``string_values``, across all keys
+            at most 200 values are allowed, with each string no more
+            than 255 characters. For unfilterable ``string_values``, the
+            maximum total size of ``string_values`` across all keys is
+            50KB.
+        degree_types (MutableSequence[google.cloud.talent_v4.types.DegreeType]):
+            The desired education degrees for the job,
+            such as Bachelors, Masters.
+        department (str):
+            The department or functional area within the
+            company with the open position.
 
+            The maximum number of allowed characters is 255.
+        employment_types (MutableSequence[google.cloud.talent_v4.types.EmploymentType]):
+            The employment type(s) of a job, for example, [full
+            time][google.cloud.talent.v4.EmploymentType.FULL_TIME] or
+            [part
+            time][google.cloud.talent.v4.EmploymentType.PART_TIME].
+        incentives (str):
+            A description of bonus, commission, and other
+            compensation incentives associated with the job
+            not including salary or pay.
+            The maximum number of allowed characters is
+            10,000.
+        language_code (str):
+            The language of the posting. This field is distinct from any
+            requirements for fluency that are associated with the job.
+
+            Language codes must be in BCP-47 format, such as "en-US" or
+            "sr-Latn". For more information, see `Tags for Identifying
+            Languages <https://tools.ietf.org/html/bcp47>`__\ {:
+            class="external" target="_blank" }.
+
+            If this field is unspecified and
+            [Job.description][google.cloud.talent.v4.Job.description] is
+            present, detected language code based on
+            [Job.description][google.cloud.talent.v4.Job.description] is
+            assigned, otherwise defaults to 'en_US'.
+        job_level (google.cloud.talent_v4.types.JobLevel):
+            The experience level associated with the job,
+            such as "Entry Level".
+        promotion_value (int):
+            A promotion value of the job, as determined by the client.
+            The value determines the sort order of the jobs returned
+            when searching for jobs using the featured jobs search call,
+            with higher promotional values being returned first and ties
+            being resolved by relevance sort. Only the jobs with a
+            promotionValue >0 are returned in a FEATURED_JOB_SEARCH.
+
+            Default value is 0, and negative values are treated as 0.
+        qualifications (str):
+            A description of the qualifications required to perform the
+            job. The use of this field is recommended as an alternative
+            to using the more general
+            [description][google.cloud.talent.v4.Job.description] field.
+
+            This field accepts and sanitizes HTML input, and also
+            accepts bold, italic, ordered list, and unordered list
+            markup tags.
+
+            The maximum number of allowed characters is 10,000.
+        responsibilities (str):
+            A description of job responsibilities. The use of this field
+            is recommended as an alternative to using the more general
+            [description][google.cloud.talent.v4.Job.description] field.
+
+            This field accepts and sanitizes HTML input, and also
+            accepts bold, italic, ordered list, and unordered list
+            markup tags.
+
+            The maximum number of allowed characters is 10,000.
+        posting_region (google.cloud.talent_v4.types.PostingRegion):
+            The job
+            [PostingRegion][google.cloud.talent.v4.PostingRegion] (for
+            example, state, country) throughout which the job is
+            available. If this field is set, a
+            [LocationFilter][google.cloud.talent.v4.LocationFilter] in a
+            search query within the job region finds this job posting if
+            an exact location match isn't specified. If this field is
+            set to
+            [PostingRegion.NATION][google.cloud.talent.v4.PostingRegion.NATION]
+            or
+            [PostingRegion.ADMINISTRATIVE_AREA][google.cloud.talent.v4.PostingRegion.ADMINISTRATIVE_AREA],
+            setting job
+            [Job.addresses][google.cloud.talent.v4.Job.addresses] to the
+            same location level as this field is strongly recommended.
+        visibility (google.cloud.talent_v4.types.Visibility):
+            Deprecated. The job is only visible to the owner.
+
+            The visibility of the job.
+
+            Defaults to
+            [Visibility.ACCOUNT_ONLY][google.cloud.talent.v4.Visibility.ACCOUNT_ONLY]
+            if not specified.
+        job_start_time (google.protobuf.timestamp_pb2.Timestamp):
+            The start timestamp of the job in UTC time
+            zone. Typically this field is used for
+            contracting engagements. Invalid timestamps are
+            ignored.
+        job_end_time (google.protobuf.timestamp_pb2.Timestamp):
+            The end timestamp of the job. Typically this
+            field is used for contracting engagements.
+            Invalid timestamps are ignored.
+        posting_publish_time (google.protobuf.timestamp_pb2.Timestamp):
+            The timestamp this job posting was most
+            recently published. The default value is the
+            time the request arrives at the server. Invalid
+            timestamps are ignored.
+        posting_expire_time (google.protobuf.timestamp_pb2.Timestamp):
+            Strongly recommended for the best service experience.
+
+            The expiration timestamp of the job. After this timestamp,
+            the job is marked as expired, and it no longer appears in
+            search results. The expired job can't be listed by the
+            [ListJobs][google.cloud.talent.v4.JobService.ListJobs] API,
+            but it can be retrieved with the
+            [GetJob][google.cloud.talent.v4.JobService.GetJob] API or
+            updated with the
+            [UpdateJob][google.cloud.talent.v4.JobService.UpdateJob] API
+            or deleted with the
+            [DeleteJob][google.cloud.talent.v4.JobService.DeleteJob]
+            API. An expired job can be updated and opened again by using
+            a future expiration timestamp. Updating an expired job fails
+            if there is another existing open job with same
+            [company][google.cloud.talent.v4.Job.company],
+            [language_code][google.cloud.talent.v4.Job.language_code]
+            and
+            [requisition_id][google.cloud.talent.v4.Job.requisition_id].
 
-class Visibility(proto.Enum):
-    r"""Deprecated. All resources are only visible to the owner.
-    An enum that represents who has view access to the resource.
+            The expired jobs are retained in our system for 90 days.
+            However, the overall expired job count cannot exceed 3 times
+            the maximum number of open jobs over previous 7 days. If
+            this threshold is exceeded, expired jobs are cleaned out in
+            order of earliest expire time. Expired jobs are no longer
+            accessible after they are cleaned out.
+
+            Invalid timestamps are ignored, and treated as expire time
+            not provided.
+
+            If the timestamp is before the instant request is made, the
+            job is treated as expired immediately on creation. This kind
+            of job can not be updated. And when creating a job with past
+            timestamp, the
+            [posting_publish_time][google.cloud.talent.v4.Job.posting_publish_time]
+            must be set before
+            [posting_expire_time][google.cloud.talent.v4.Job.posting_expire_time].
+            The purpose of this feature is to allow other objects, such
+            as [Application][], to refer a job that didn't exist in the
+            system prior to becoming expired. If you want to modify a
+            job that was expired on creation, delete it and create a new
+            one.
+
+            If this value isn't provided at the time of job creation or
+            is invalid, the job posting expires after 30 days from the
+            job's creation time. For example, if the job was created on
+            2017/01/01 13:00AM UTC with an unspecified expiration date,
+            the job expires after 2017/01/31 13:00AM UTC.
+
+            If this value isn't provided on job update, it depends on
+            the field masks set by
+            [UpdateJobRequest.update_mask][google.cloud.talent.v4.UpdateJobRequest.update_mask].
+            If the field masks include
+            [job_end_time][google.cloud.talent.v4.Job.job_end_time], or
+            the masks are empty meaning that every field is updated, the
+            job posting expires after 30 days from the job's last update
+            time. Otherwise the expiration date isn't updated.
+        posting_create_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. The timestamp when this job
+            posting was created.
+        posting_update_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. The timestamp when this job
+            posting was last updated.
+        company_display_name (str):
+            Output only. Display name of the company
+            listing the job.
+        derived_info (google.cloud.talent_v4.types.Job.DerivedInfo):
+            Output only. Derived details about the job
+            posting.
+        processing_options (google.cloud.talent_v4.types.Job.ProcessingOptions):
+            Options for job processing.
     """
-    _pb_options = {"deprecated": True}
-    VISIBILITY_UNSPECIFIED = 0
-    ACCOUNT_ONLY = 1
-    SHARED_WITH_GOOGLE = 2
-    SHARED_WITH_PUBLIC = 3
-
 
-class HtmlSanitization(proto.Enum):
-    r"""Option for HTML content sanitization on user input fields,
-    for example, job description. By setting this option, user can
-    determine whether and how sanitization is performed on these
-    fields.
-    """
-    HTML_SANITIZATION_UNSPECIFIED = 0
-    HTML_SANITIZATION_DISABLED = 1
-    SIMPLE_FORMATTING_ONLY = 2
+    class ApplicationInfo(proto.Message):
+        r"""Application related details of a job posting.
 
+        Attributes:
+            emails (MutableSequence[str]):
+                Use this field to specify email address(es)
+                to which resumes or applications can be sent.
+                The maximum number of allowed characters for
+                each entry is 255.
+            instruction (str):
+                Use this field to provide instructions, such
+                as "Mail your application to ...", that a
+                candidate can follow to apply for the job.
+                This field accepts and sanitizes HTML input, and
+                also accepts bold, italic, ordered list, and
+                unordered list markup tags.
+                The maximum number of allowed characters is
+                3,000.
+            uris (MutableSequence[str]):
+                Use this URI field to direct an applicant to
+                a website, for example to link to an online
+                application form.
+                The maximum number of allowed characters for
+                each entry is 2,000.
+        """
 
-class CommuteMethod(proto.Enum):
-    r"""Method for commute. Walking, biking and wheelchair accessible
-    transit is still in the Preview stage.
-    """
-    COMMUTE_METHOD_UNSPECIFIED = 0
-    DRIVING = 1
-    TRANSIT = 2
-    WALKING = 3
-    CYCLING = 4
-    TRANSIT_ACCESSIBLE = 5
+        emails: MutableSequence[str] = proto.RepeatedField(
+            proto.STRING,
+            number=1,
+        )
+        instruction: str = proto.Field(
+            proto.STRING,
+            number=2,
+        )
+        uris: MutableSequence[str] = proto.RepeatedField(
+            proto.STRING,
+            number=3,
+        )
 
+    class DerivedInfo(proto.Message):
+        r"""Derived details about the job posting.
 
-class TimestampRange(proto.Message):
-    r"""Message representing a period of time between two timestamps.
+        Attributes:
+            locations (MutableSequence[google.cloud.talent_v4.types.Location]):
+                Structured locations of the job, resolved from
+                [Job.addresses][google.cloud.talent.v4.Job.addresses].
+
+                [locations][google.cloud.talent.v4.Job.DerivedInfo.locations]
+                are exactly matched to
+                [Job.addresses][google.cloud.talent.v4.Job.addresses] in the
+                same order.
+            job_categories (MutableSequence[google.cloud.talent_v4.types.JobCategory]):
+                Job categories derived from
+                [Job.title][google.cloud.talent.v4.Job.title] and
+                [Job.description][google.cloud.talent.v4.Job.description].
+        """
 
-    Attributes:
-        start_time (google.protobuf.timestamp_pb2.Timestamp):
-            Begin of the period (inclusive).
-        end_time (google.protobuf.timestamp_pb2.Timestamp):
-            End of the period (exclusive).
-    """
+        locations: MutableSequence[common.Location] = proto.RepeatedField(
+            proto.MESSAGE,
+            number=1,
+            message=common.Location,
+        )
+        job_categories: MutableSequence[common.JobCategory] = proto.RepeatedField(
+            proto.ENUM,
+            number=3,
+            enum=common.JobCategory,
+        )
 
-    start_time: timestamp_pb2.Timestamp = proto.Field(
-        proto.MESSAGE,
-        number=1,
-        message=timestamp_pb2.Timestamp,
-    )
-    end_time: timestamp_pb2.Timestamp = proto.Field(
-        proto.MESSAGE,
-        number=2,
-        message=timestamp_pb2.Timestamp,
-    )
+    class ProcessingOptions(proto.Message):
+        r"""Options for job processing.
 
+        Attributes:
+            disable_street_address_resolution (bool):
+                If set to ``true``, the service does not attempt to resolve
+                a more precise address for the job.
+            html_sanitization (google.cloud.talent_v4.types.HtmlSanitization):
+                Option for job HTML content sanitization. Applied fields
+                are:
+
+                -  description
+                -  applicationInfo.instruction
+                -  incentives
+                -  qualifications
+                -  responsibilities
 
-class Location(proto.Message):
-    r"""A resource that represents a location with full geographic
-    information.
+                HTML tags in these fields may be stripped if sanitiazation
+                isn't disabled.
 
-    Attributes:
-        location_type (google.cloud.talent_v4.types.Location.LocationType):
-            The type of a location, which corresponds to the address
-            lines field of
-            [google.type.PostalAddress][google.type.PostalAddress]. For
-            example, "Downtown, Atlanta, GA, USA" has a type of
-            [LocationType.NEIGHBORHOOD][google.cloud.talent.v4.Location.LocationType.NEIGHBORHOOD],
-            and "Kansas City, KS, USA" has a type of
-            [LocationType.LOCALITY][google.cloud.talent.v4.Location.LocationType.LOCALITY].
-        postal_address (google.type.postal_address_pb2.PostalAddress):
-            Postal address of the location that includes
-            human readable information, such as postal
-            delivery and payments addresses. Given a postal
-            address, a postal service can deliver items to a
-            premises, P.O. Box, or other delivery location.
-        lat_lng (google.type.latlng_pb2.LatLng):
-            An object representing a latitude/longitude
-            pair.
-        radius_miles (float):
-            Radius in miles of the job location. This value is derived
-            from the location bounding box in which a circle with the
-            specified radius centered from
-            [google.type.LatLng][google.type.LatLng] covers the area
-            associated with the job location. For example, currently,
-            "Mountain View, CA, USA" has a radius of 6.17 miles.
-    """
+                Defaults to
+                [HtmlSanitization.SIMPLE_FORMATTING_ONLY][google.cloud.talent.v4.HtmlSanitization.SIMPLE_FORMATTING_ONLY].
+        """
 
-    class LocationType(proto.Enum):
-        r"""An enum which represents the type of a location."""
-        LOCATION_TYPE_UNSPECIFIED = 0
-        COUNTRY = 1
-        ADMINISTRATIVE_AREA = 2
-        SUB_ADMINISTRATIVE_AREA = 3
-        LOCALITY = 4
-        POSTAL_CODE = 5
-        SUB_LOCALITY = 6
-        SUB_LOCALITY_1 = 7
-        SUB_LOCALITY_2 = 8
-        NEIGHBORHOOD = 9
-        STREET_ADDRESS = 10
+        disable_street_address_resolution: bool = proto.Field(
+            proto.BOOL,
+            number=1,
+        )
+        html_sanitization: common.HtmlSanitization = proto.Field(
+            proto.ENUM,
+            number=2,
+            enum=common.HtmlSanitization,
+        )
 
-    location_type: LocationType = proto.Field(
-        proto.ENUM,
+    name: str = proto.Field(
+        proto.STRING,
         number=1,
-        enum=LocationType,
     )
-    postal_address: postal_address_pb2.PostalAddress = proto.Field(
-        proto.MESSAGE,
+    company: str = proto.Field(
+        proto.STRING,
         number=2,
-        message=postal_address_pb2.PostalAddress,
     )
-    lat_lng: latlng_pb2.LatLng = proto.Field(
-        proto.MESSAGE,
+    requisition_id: str = proto.Field(
+        proto.STRING,
         number=3,
-        message=latlng_pb2.LatLng,
     )
-    radius_miles: float = proto.Field(
-        proto.DOUBLE,
+    title: str = proto.Field(
+        proto.STRING,
         number=4,
     )
-
-
-class RequestMetadata(proto.Message):
-    r"""Meta information related to the job searcher or entity
-    conducting the job search. This information is used to improve
-    the performance of the service.
-
-    Attributes:
-        domain (str):
-            Required if
-            [allow_missing_ids][google.cloud.talent.v4.RequestMetadata.allow_missing_ids]
-            is unset or ``false``.
-
-            The client-defined scope or source of the service call,
-            which typically is the domain on which the service has been
-            implemented and is currently being run.
-
-            For example, if the service is being run by client Foo,
-            Inc., on job board www.foo.com and career site www.bar.com,
-            then this field is set to "foo.com" for use on the job
-            board, and "bar.com" for use on the career site.
-
-            Note that any improvements to the model for a particular
-            tenant site rely on this field being set correctly to a
-            unique domain.
-
-            The maximum number of allowed characters is 255.
-        session_id (str):
-            Required if
-            [allow_missing_ids][google.cloud.talent.v4.RequestMetadata.allow_missing_ids]
-            is unset or ``false``.
-
-            A unique session identification string. A session is defined
-            as the duration of an end user's interaction with the
-            service over a certain period. Obfuscate this field for
-            privacy concerns before providing it to the service.
-
-            Note that any improvements to the model for a particular
-            tenant site rely on this field being set correctly to a
-            unique session ID.
-
-            The maximum number of allowed characters is 255.
-        user_id (str):
-            Required if
-            [allow_missing_ids][google.cloud.talent.v4.RequestMetadata.allow_missing_ids]
-            is unset or ``false``.
-
-            A unique user identification string, as determined by the
-            client. To have the strongest positive impact on search
-            quality make sure the client-level is unique. Obfuscate this
-            field for privacy concerns before providing it to the
-            service.
-
-            Note that any improvements to the model for a particular
-            tenant site rely on this field being set correctly to a
-            unique user ID.
-
-            The maximum number of allowed characters is 255.
-        allow_missing_ids (bool):
-            Only set when any of
-            [domain][google.cloud.talent.v4.RequestMetadata.domain],
-            [session_id][google.cloud.talent.v4.RequestMetadata.session_id]
-            and
-            [user_id][google.cloud.talent.v4.RequestMetadata.user_id]
-            isn't available for some reason. It is highly recommended
-            not to set this field and provide accurate
-            [domain][google.cloud.talent.v4.RequestMetadata.domain],
-            [session_id][google.cloud.talent.v4.RequestMetadata.session_id]
-            and
-            [user_id][google.cloud.talent.v4.RequestMetadata.user_id]
-            for the best service experience.
-        device_info (google.cloud.talent_v4.types.DeviceInfo):
-            The type of device used by the job seeker at
-            the time of the call to the service.
-    """
-
-    domain: str = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
-        number=1,
+        number=5,
     )
-    session_id: str = proto.Field(
+    addresses: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
-        number=2,
+        number=6,
     )
-    user_id: str = proto.Field(
-        proto.STRING,
-        number=3,
+    application_info: ApplicationInfo = proto.Field(
+        proto.MESSAGE,
+        number=7,
+        message=ApplicationInfo,
     )
-    allow_missing_ids: bool = proto.Field(
-        proto.BOOL,
-        number=4,
+    job_benefits: MutableSequence[common.JobBenefit] = proto.RepeatedField(
+        proto.ENUM,
+        number=8,
+        enum=common.JobBenefit,
     )
-    device_info: "DeviceInfo" = proto.Field(
+    compensation_info: common.CompensationInfo = proto.Field(
         proto.MESSAGE,
-        number=5,
-        message="DeviceInfo",
+        number=9,
+        message=common.CompensationInfo,
     )
-
-
-class ResponseMetadata(proto.Message):
-    r"""Additional information returned to client, such as debugging
-    information.
-
-    Attributes:
-        request_id (str):
-            A unique id associated with this call.
-            This id is logged for tracking purposes.
-    """
-
-    request_id: str = proto.Field(
+    custom_attributes: MutableMapping[str, common.CustomAttribute] = proto.MapField(
         proto.STRING,
-        number=1,
+        proto.MESSAGE,
+        number=10,
+        message=common.CustomAttribute,
     )
-
-
-class DeviceInfo(proto.Message):
-    r"""Device information collected from the job seeker, candidate,
-    or other entity conducting the job search. Providing this
-    information improves the quality of the search results across
-    devices.
-
-    Attributes:
-        device_type (google.cloud.talent_v4.types.DeviceInfo.DeviceType):
-            Type of the device.
-        id (str):
-            A device-specific ID. The ID must be a unique
-            identifier that distinguishes the device from
-            other devices.
-    """
-
-    class DeviceType(proto.Enum):
-        r"""An enumeration describing an API access portal and exposure
-        mechanism.
-        """
-        DEVICE_TYPE_UNSPECIFIED = 0
-        WEB = 1
-        MOBILE_WEB = 2
-        ANDROID = 3
-        IOS = 4
-        BOT = 5
-        OTHER = 6
-
-    device_type: DeviceType = proto.Field(
+    degree_types: MutableSequence[common.DegreeType] = proto.RepeatedField(
         proto.ENUM,
-        number=1,
-        enum=DeviceType,
+        number=11,
+        enum=common.DegreeType,
     )
-    id: str = proto.Field(
+    department: str = proto.Field(
         proto.STRING,
-        number=2,
+        number=12,
     )
-
-
-class CustomAttribute(proto.Message):
-    r"""Custom attribute values that are either filterable or
-    non-filterable.
-
-    Attributes:
-        string_values (MutableSequence[str]):
-            Exactly one of
-            [string_values][google.cloud.talent.v4.CustomAttribute.string_values]
-            or
-            [long_values][google.cloud.talent.v4.CustomAttribute.long_values]
-            must be specified.
-
-            This field is used to perform a string match
-            (``CASE_SENSITIVE_MATCH`` or ``CASE_INSENSITIVE_MATCH``)
-            search. For filterable ``string_value``\ s, a maximum total
-            number of 200 values is allowed, with each ``string_value``
-            has a byte size of no more than 500B. For unfilterable
-            ``string_values``, the maximum total byte size of
-            unfilterable ``string_values`` is 50KB.
-
-            Empty string isn't allowed.
-        long_values (MutableSequence[int]):
-            Exactly one of
-            [string_values][google.cloud.talent.v4.CustomAttribute.string_values]
-            or
-            [long_values][google.cloud.talent.v4.CustomAttribute.long_values]
-            must be specified.
-
-            This field is used to perform number range search. (``EQ``,
-            ``GT``, ``GE``, ``LE``, ``LT``) over filterable
-            ``long_value``.
-
-            Currently at most 1
-            [long_values][google.cloud.talent.v4.CustomAttribute.long_values]
-            is supported.
-        filterable (bool):
-            If the ``filterable`` flag is true, the custom field values
-            may be used for custom attribute filters
-            [JobQuery.custom_attribute_filter][google.cloud.talent.v4.JobQuery.custom_attribute_filter].
-            If false, these values may not be used for custom attribute
-            filters.
-
-            Default is false.
-        keyword_searchable (bool):
-            If the ``keyword_searchable`` flag is true, the keywords in
-            custom fields are searchable by keyword match. If false, the
-            values are not searchable by keyword match.
-
-            Default is false.
-    """
-
-    string_values: MutableSequence[str] = proto.RepeatedField(
-        proto.STRING,
-        number=1,
+    employment_types: MutableSequence[common.EmploymentType] = proto.RepeatedField(
+        proto.ENUM,
+        number=13,
+        enum=common.EmploymentType,
     )
-    long_values: MutableSequence[int] = proto.RepeatedField(
-        proto.INT64,
-        number=2,
+    incentives: str = proto.Field(
+        proto.STRING,
+        number=14,
     )
-    filterable: bool = proto.Field(
-        proto.BOOL,
-        number=3,
+    language_code: str = proto.Field(
+        proto.STRING,
+        number=15,
     )
-    keyword_searchable: bool = proto.Field(
-        proto.BOOL,
-        number=4,
+    job_level: common.JobLevel = proto.Field(
+        proto.ENUM,
+        number=16,
+        enum=common.JobLevel,
     )
-
-
-class SpellingCorrection(proto.Message):
-    r"""Spell check result.
-
-    Attributes:
-        corrected (bool):
-            Indicates if the query was corrected by the
-            spell checker.
-        corrected_text (str):
-            Correction output consisting of the corrected
-            keyword string.
-        corrected_html (str):
-            Corrected output with html tags to highlight
-            the corrected words. Corrected words are called
-            out with the "<b><i>...</i></b>" html tags.
-            For example, the user input query is "software
-            enginear", where the second word, "enginear," is
-            incorrect. It should be "engineer". When
-            spelling correction is enabled, this value is
-            "software <b><i>engineer</i></b>".
-    """
-
-    corrected: bool = proto.Field(
-        proto.BOOL,
-        number=1,
+    promotion_value: int = proto.Field(
+        proto.INT32,
+        number=17,
     )
-    corrected_text: str = proto.Field(
+    qualifications: str = proto.Field(
         proto.STRING,
-        number=2,
+        number=18,
     )
-    corrected_html: str = proto.Field(
+    responsibilities: str = proto.Field(
         proto.STRING,
-        number=3,
+        number=19,
     )
-
-
-class CompensationInfo(proto.Message):
-    r"""Job compensation details.
-
-    Attributes:
-        entries (MutableSequence[google.cloud.talent_v4.types.CompensationInfo.CompensationEntry]):
-            Job compensation information.
-
-            At most one entry can be of type
-            [CompensationInfo.CompensationType.BASE][google.cloud.talent.v4.CompensationInfo.CompensationType.BASE],
-            which is referred as **base compensation entry** for the
-            job.
-        annualized_base_compensation_range (google.cloud.talent_v4.types.CompensationInfo.CompensationRange):
-            Output only. Annualized base compensation range. Computed as
-            base compensation entry's
-            [CompensationEntry.amount][google.cloud.talent.v4.CompensationInfo.CompensationEntry.amount]
-            times
-            [CompensationEntry.expected_units_per_year][google.cloud.talent.v4.CompensationInfo.CompensationEntry.expected_units_per_year].
-
-            See
-            [CompensationEntry][google.cloud.talent.v4.CompensationInfo.CompensationEntry]
-            for explanation on compensation annualization.
-        annualized_total_compensation_range (google.cloud.talent_v4.types.CompensationInfo.CompensationRange):
-            Output only. Annualized total compensation range. Computed
-            as all compensation entries'
-            [CompensationEntry.amount][google.cloud.talent.v4.CompensationInfo.CompensationEntry.amount]
-            times
-            [CompensationEntry.expected_units_per_year][google.cloud.talent.v4.CompensationInfo.CompensationEntry.expected_units_per_year].
-
-            See
-            [CompensationEntry][google.cloud.talent.v4.CompensationInfo.CompensationEntry]
-            for explanation on compensation annualization.
-    """
-
-    class CompensationType(proto.Enum):
-        r"""The type of compensation.
-
-        For compensation amounts specified in non-monetary amounts, describe
-        the compensation scheme in the
-        [CompensationEntry.description][google.cloud.talent.v4.CompensationInfo.CompensationEntry.description].
-
-        For example, tipping format is described in
-        [CompensationEntry.description][google.cloud.talent.v4.CompensationInfo.CompensationEntry.description]
-        (for example, "expect 15-20% tips based on customer bill.") and an
-        estimate of the tips provided in
-        [CompensationEntry.amount][google.cloud.talent.v4.CompensationInfo.CompensationEntry.amount]
-        or
-        [CompensationEntry.range][google.cloud.talent.v4.CompensationInfo.CompensationEntry.range]
-        ($10 per hour).
-
-        For example, equity is described in
-        [CompensationEntry.description][google.cloud.talent.v4.CompensationInfo.CompensationEntry.description]
-        (for example, "1% - 2% equity vesting over 4 years, 1 year cliff")
-        and value estimated in
-        [CompensationEntry.amount][google.cloud.talent.v4.CompensationInfo.CompensationEntry.amount]
-        or
-        [CompensationEntry.range][google.cloud.talent.v4.CompensationInfo.CompensationEntry.range].
-        If no value estimate is possible, units are
-        [CompensationUnit.COMPENSATION_UNIT_UNSPECIFIED][google.cloud.talent.v4.CompensationInfo.CompensationUnit.COMPENSATION_UNIT_UNSPECIFIED]
-        and then further clarified in
-        [CompensationEntry.description][google.cloud.talent.v4.CompensationInfo.CompensationEntry.description]
-        field.
-        """
-        COMPENSATION_TYPE_UNSPECIFIED = 0
-        BASE = 1
-        BONUS = 2
-        SIGNING_BONUS = 3
-        EQUITY = 4
-        PROFIT_SHARING = 5
-        COMMISSIONS = 6
-        TIPS = 7
-        OTHER_COMPENSATION_TYPE = 8
-
-    class CompensationUnit(proto.Enum):
-        r"""Pay frequency."""
-        COMPENSATION_UNIT_UNSPECIFIED = 0
-        HOURLY = 1
-        DAILY = 2
-        WEEKLY = 3
-        MONTHLY = 4
-        YEARLY = 5
-        ONE_TIME = 6
-        OTHER_COMPENSATION_UNIT = 7
-
-    class CompensationEntry(proto.Message):
-        r"""A compensation entry that represents one component of compensation,
-        such as base pay, bonus, or other compensation type.
-
-        Annualization: One compensation entry can be annualized if
-
-        -  it contains valid
-           [amount][google.cloud.talent.v4.CompensationInfo.CompensationEntry.amount]
-           or
-           [range][google.cloud.talent.v4.CompensationInfo.CompensationEntry.range].
-        -  and its
-           [expected_units_per_year][google.cloud.talent.v4.CompensationInfo.CompensationEntry.expected_units_per_year]
-           is set or can be derived. Its annualized range is determined as
-           ([amount][google.cloud.talent.v4.CompensationInfo.CompensationEntry.amount]
-           or
-           [range][google.cloud.talent.v4.CompensationInfo.CompensationEntry.range])
-           times
-           [expected_units_per_year][google.cloud.talent.v4.CompensationInfo.CompensationEntry.expected_units_per_year].
-
-        This message has `oneof`_ fields (mutually exclusive fields).
-        For each oneof, at most one member field can be set at the same time.
-        Setting any member of the oneof automatically clears all other
-        members.
-
-        .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
-
-        Attributes:
-            type_ (google.cloud.talent_v4.types.CompensationInfo.CompensationType):
-                Compensation type.
-
-                Default is
-                [CompensationType.COMPENSATION_TYPE_UNSPECIFIED][google.cloud.talent.v4.CompensationInfo.CompensationType.COMPENSATION_TYPE_UNSPECIFIED].
-            unit (google.cloud.talent_v4.types.CompensationInfo.CompensationUnit):
-                Frequency of the specified amount.
-
-                Default is
-                [CompensationUnit.COMPENSATION_UNIT_UNSPECIFIED][google.cloud.talent.v4.CompensationInfo.CompensationUnit.COMPENSATION_UNIT_UNSPECIFIED].
-            amount (google.type.money_pb2.Money):
-                Compensation amount.
-
-                This field is a member of `oneof`_ ``compensation_amount``.
-            range_ (google.cloud.talent_v4.types.CompensationInfo.CompensationRange):
-                Compensation range.
-
-                This field is a member of `oneof`_ ``compensation_amount``.
-            description (str):
-                Compensation description.  For example, could
-                indicate equity terms or provide additional
-                context to an estimated bonus.
-            expected_units_per_year (google.protobuf.wrappers_pb2.DoubleValue):
-                Expected number of units paid each year. If not specified,
-                when
-                [Job.employment_types][google.cloud.talent.v4.Job.employment_types]
-                is FULLTIME, a default value is inferred based on
-                [unit][google.cloud.talent.v4.CompensationInfo.CompensationEntry.unit].
-                Default values:
-
-                -  HOURLY: 2080
-                -  DAILY: 260
-                -  WEEKLY: 52
-                -  MONTHLY: 12
-                -  ANNUAL: 1
-        """
-
-        type_: "CompensationInfo.CompensationType" = proto.Field(
-            proto.ENUM,
-            number=1,
-            enum="CompensationInfo.CompensationType",
-        )
-        unit: "CompensationInfo.CompensationUnit" = proto.Field(
-            proto.ENUM,
-            number=2,
-            enum="CompensationInfo.CompensationUnit",
-        )
-        amount: money_pb2.Money = proto.Field(
-            proto.MESSAGE,
-            number=3,
-            oneof="compensation_amount",
-            message=money_pb2.Money,
-        )
-        range_: "CompensationInfo.CompensationRange" = proto.Field(
-            proto.MESSAGE,
-            number=4,
-            oneof="compensation_amount",
-            message="CompensationInfo.CompensationRange",
-        )
-        description: str = proto.Field(
-            proto.STRING,
-            number=5,
-        )
-        expected_units_per_year: wrappers_pb2.DoubleValue = proto.Field(
-            proto.MESSAGE,
-            number=6,
-            message=wrappers_pb2.DoubleValue,
-        )
-
-    class CompensationRange(proto.Message):
-        r"""Compensation range.
-
-        Attributes:
-            max_compensation (google.type.money_pb2.Money):
-                The maximum amount of compensation. If left empty, the value
-                is set to a maximal compensation value and the currency code
-                is set to match the [currency
-                code][google.type.Money.currency_code] of min_compensation.
-            min_compensation (google.type.money_pb2.Money):
-                The minimum amount of compensation. If left empty, the value
-                is set to zero and the currency code is set to match the
-                [currency code][google.type.Money.currency_code] of
-                max_compensation.
-        """
-
-        max_compensation: money_pb2.Money = proto.Field(
-            proto.MESSAGE,
-            number=2,
-            message=money_pb2.Money,
-        )
-        min_compensation: money_pb2.Money = proto.Field(
-            proto.MESSAGE,
-            number=1,
-            message=money_pb2.Money,
-        )
-
-    entries: MutableSequence[CompensationEntry] = proto.RepeatedField(
-        proto.MESSAGE,
-        number=1,
-        message=CompensationEntry,
-    )
-    annualized_base_compensation_range: CompensationRange = proto.Field(
-        proto.MESSAGE,
-        number=2,
-        message=CompensationRange,
-    )
-    annualized_total_compensation_range: CompensationRange = proto.Field(
-        proto.MESSAGE,
-        number=3,
-        message=CompensationRange,
-    )
-
-
-class BatchOperationMetadata(proto.Message):
-    r"""Metadata used for long running operations returned by CTS batch
-    APIs. It's used to replace
-    [google.longrunning.Operation.metadata][google.longrunning.Operation.metadata].
-
-    Attributes:
-        state (google.cloud.talent_v4.types.BatchOperationMetadata.State):
-            The state of a long running operation.
-        state_description (str):
-            More detailed information about operation
-            state.
-        success_count (int):
-            Count of successful item(s) inside an
-            operation.
-        failure_count (int):
-            Count of failed item(s) inside an operation.
-        total_count (int):
-            Count of total item(s) inside an operation.
-        create_time (google.protobuf.timestamp_pb2.Timestamp):
-            The time when the batch operation is created.
-        update_time (google.protobuf.timestamp_pb2.Timestamp):
-            The time when the batch operation status is updated. The
-            metadata and the
-            [update_time][google.cloud.talent.v4.BatchOperationMetadata.update_time]
-            is refreshed every minute otherwise cached data is returned.
-        end_time (google.protobuf.timestamp_pb2.Timestamp):
-            The time when the batch operation is finished and
-            [google.longrunning.Operation.done][google.longrunning.Operation.done]
-            is set to ``true``.
-    """
-
-    class State(proto.Enum):
-        r""""""
-        STATE_UNSPECIFIED = 0
-        INITIALIZING = 1
-        PROCESSING = 2
-        SUCCEEDED = 3
-        FAILED = 4
-        CANCELLING = 5
-        CANCELLED = 6
-
-    state: State = proto.Field(
+    posting_region: common.PostingRegion = proto.Field(
         proto.ENUM,
-        number=1,
-        enum=State,
+        number=20,
+        enum=common.PostingRegion,
     )
-    state_description: str = proto.Field(
-        proto.STRING,
-        number=2,
+    visibility: common.Visibility = proto.Field(
+        proto.ENUM,
+        number=21,
+        enum=common.Visibility,
     )
-    success_count: int = proto.Field(
-        proto.INT32,
-        number=3,
+    job_start_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=22,
+        message=timestamp_pb2.Timestamp,
     )
-    failure_count: int = proto.Field(
-        proto.INT32,
-        number=4,
+    job_end_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=23,
+        message=timestamp_pb2.Timestamp,
     )
-    total_count: int = proto.Field(
-        proto.INT32,
-        number=5,
+    posting_publish_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=24,
+        message=timestamp_pb2.Timestamp,
     )
-    create_time: timestamp_pb2.Timestamp = proto.Field(
+    posting_expire_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
-        number=6,
+        number=25,
         message=timestamp_pb2.Timestamp,
     )
-    update_time: timestamp_pb2.Timestamp = proto.Field(
+    posting_create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
-        number=7,
+        number=26,
         message=timestamp_pb2.Timestamp,
     )
-    end_time: timestamp_pb2.Timestamp = proto.Field(
+    posting_update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
-        number=8,
+        number=27,
         message=timestamp_pb2.Timestamp,
     )
+    company_display_name: str = proto.Field(
+        proto.STRING,
+        number=28,
+    )
+    derived_info: DerivedInfo = proto.Field(
+        proto.MESSAGE,
+        number=29,
+        message=DerivedInfo,
+    )
+    processing_options: ProcessingOptions = proto.Field(
+        proto.MESSAGE,
+        number=30,
+        message=ProcessingOptions,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/types/company.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/types/company.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/types/company_service.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/types/company_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/types/completion_service.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/types/completion_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -63,21 +63,64 @@
             [CompletionScope.PUBLIC][google.cloud.talent.v4.CompleteQueryRequest.CompletionScope.PUBLIC].
         type_ (google.cloud.talent_v4.types.CompleteQueryRequest.CompletionType):
             The completion topic. The default is
             [CompletionType.COMBINED][google.cloud.talent.v4.CompleteQueryRequest.CompletionType.COMBINED].
     """
 
     class CompletionScope(proto.Enum):
-        r"""Enum to specify the scope of completion."""
+        r"""Enum to specify the scope of completion.
+
+        Values:
+            COMPLETION_SCOPE_UNSPECIFIED (0):
+                Default value.
+            TENANT (1):
+                Suggestions are based only on the data
+                provided by the client.
+            PUBLIC (2):
+                Suggestions are based on all jobs data in the
+                system that's visible to the client
+        """
         COMPLETION_SCOPE_UNSPECIFIED = 0
         TENANT = 1
         PUBLIC = 2
 
     class CompletionType(proto.Enum):
-        r"""Enum to specify auto-completion topics."""
+        r"""Enum to specify auto-completion topics.
+
+        Values:
+            COMPLETION_TYPE_UNSPECIFIED (0):
+                Default value.
+            JOB_TITLE (1):
+                Suggest job titles for jobs autocomplete.
+
+                For
+                [CompletionType.JOB_TITLE][google.cloud.talent.v4.CompleteQueryRequest.CompletionType.JOB_TITLE]
+                type, only open jobs with the same
+                [language_codes][google.cloud.talent.v4.CompleteQueryRequest.language_codes]
+                are returned.
+            COMPANY_NAME (2):
+                Suggest company names for jobs autocomplete.
+
+                For
+                [CompletionType.COMPANY_NAME][google.cloud.talent.v4.CompleteQueryRequest.CompletionType.COMPANY_NAME]
+                type, only companies having open jobs with the same
+                [language_codes][google.cloud.talent.v4.CompleteQueryRequest.language_codes]
+                are returned.
+            COMBINED (3):
+                Suggest both job titles and company names for jobs
+                autocomplete.
+
+                For
+                [CompletionType.COMBINED][google.cloud.talent.v4.CompleteQueryRequest.CompletionType.COMBINED]
+                type, only open jobs with the same
+                [language_codes][google.cloud.talent.v4.CompleteQueryRequest.language_codes]
+                or companies having open jobs with the same
+                [language_codes][google.cloud.talent.v4.CompleteQueryRequest.language_codes]
+                are returned.
+        """
         COMPLETION_TYPE_UNSPECIFIED = 0
         JOB_TITLE = 1
         COMPANY_NAME = 2
         COMBINED = 3
 
     tenant: str = proto.Field(
         proto.STRING,
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/types/event_service.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/types/event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/types/filters.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/types/filters.py`

 * *Files 11% similar despite different names*

```diff
@@ -338,15 +338,29 @@
             filters, telecommuting jobs can be treated as less relevant
             than other jobs in the search response.
 
             This field is only used for job search requests.
     """
 
     class TelecommutePreference(proto.Enum):
-        r"""Specify whether to include telecommute jobs."""
+        r"""Specify whether to include telecommute jobs.
+
+        Values:
+            TELECOMMUTE_PREFERENCE_UNSPECIFIED (0):
+                Default value if the telecommute preference
+                isn't specified.
+            TELECOMMUTE_EXCLUDED (1):
+                Deprecated: Ignore telecommute status of jobs. Use
+                TELECOMMUTE_JOBS_EXCLUDED if want to exclude telecommute
+                jobs.
+            TELECOMMUTE_ALLOWED (2):
+                Allow telecommute jobs.
+            TELECOMMUTE_JOBS_EXCLUDED (3):
+                Exclude telecommute jobs.
+        """
         TELECOMMUTE_PREFERENCE_UNSPECIFIED = 0
         TELECOMMUTE_EXCLUDED = 1
         TELECOMMUTE_ALLOWED = 2
         TELECOMMUTE_JOBS_EXCLUDED = 3
 
     address: str = proto.Field(
         proto.STRING,
@@ -385,15 +399,62 @@
             Compensation range.
         include_jobs_with_unspecified_compensation_range (bool):
             If set to true, jobs with unspecified
             compensation range fields are included.
     """
 
     class FilterType(proto.Enum):
-        r"""Specify the type of filtering."""
+        r"""Specify the type of filtering.
+
+        Values:
+            FILTER_TYPE_UNSPECIFIED (0):
+                Filter type unspecified. Position holder,
+                INVALID, should never be used.
+            UNIT_ONLY (1):
+                Filter by ``base compensation entry's`` unit. A job is a
+                match if and only if the job contains a base
+                CompensationEntry and the base CompensationEntry's unit
+                matches provided
+                [units][google.cloud.talent.v4.CompensationFilter.units].
+                Populate one or more
+                [units][google.cloud.talent.v4.CompensationFilter.units].
+
+                See
+                [CompensationInfo.CompensationEntry][google.cloud.talent.v4.CompensationInfo.CompensationEntry]
+                for definition of base compensation entry.
+            UNIT_AND_AMOUNT (2):
+                Filter by ``base compensation entry's`` unit and amount /
+                range. A job is a match if and only if the job contains a
+                base CompensationEntry, and the base entry's unit matches
+                provided
+                [CompensationUnit][google.cloud.talent.v4.CompensationInfo.CompensationUnit]
+                and amount or range overlaps with provided
+                [CompensationRange][google.cloud.talent.v4.CompensationInfo.CompensationRange].
+
+                See
+                [CompensationInfo.CompensationEntry][google.cloud.talent.v4.CompensationInfo.CompensationEntry]
+                for definition of base compensation entry.
+
+                Set exactly one
+                [units][google.cloud.talent.v4.CompensationFilter.units] and
+                populate
+                [range][google.cloud.talent.v4.CompensationFilter.range].
+            ANNUALIZED_BASE_AMOUNT (3):
+                Filter by annualized base compensation amount and
+                ``base compensation entry's`` unit. Populate
+                [range][google.cloud.talent.v4.CompensationFilter.range] and
+                zero or more
+                [units][google.cloud.talent.v4.CompensationFilter.units].
+            ANNUALIZED_TOTAL_AMOUNT (4):
+                Filter by annualized total compensation amount and
+                ``base compensation entry's`` unit . Populate
+                [range][google.cloud.talent.v4.CompensationFilter.range] and
+                zero or more
+                [units][google.cloud.talent.v4.CompensationFilter.units].
+        """
         FILTER_TYPE_UNSPECIFIED = 0
         UNIT_ONLY = 1
         UNIT_AND_AMOUNT = 2
         ANNUALIZED_BASE_AMOUNT = 3
         ANNUALIZED_TOTAL_AMOUNT = 4
 
     type_: FilterType = proto.Field(
@@ -460,15 +521,26 @@
             Currently traffic model is restricted to hour level
             resolution.
 
             This field is a member of `oneof`_ ``traffic_option``.
     """
 
     class RoadTraffic(proto.Enum):
-        r"""The traffic density to use when calculating commute time."""
+        r"""The traffic density to use when calculating commute time.
+
+        Values:
+            ROAD_TRAFFIC_UNSPECIFIED (0):
+                Road traffic situation isn't specified.
+            TRAFFIC_FREE (1):
+                Optimal commute time without considering any
+                traffic impact.
+            BUSY_HOUR (2):
+                Commute time calculation takes in account the
+                peak traffic impact.
+        """
         ROAD_TRAFFIC_UNSPECIFIED = 0
         TRAFFIC_FREE = 1
         BUSY_HOUR = 2
 
     commute_method: common.CommuteMethod = proto.Field(
         proto.ENUM,
         number=1,
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/types/histogram.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/types/histogram.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/types/job.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/job.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,74 +14,80 @@
 # limitations under the License.
 #
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
-from google.cloud.talent_v4.types import common
+from google.cloud.talent_v4beta1.types import common
 
 __protobuf__ = proto.module(
-    package="google.cloud.talent.v4",
+    package="google.cloud.talent.v4beta1",
     manifest={
         "Job",
     },
 )
 
 
 class Job(proto.Message):
     r"""A Job resource represents a job posting (also referred to as a "job
     listing" or "job requisition"). A job belongs to a
-    [Company][google.cloud.talent.v4.Company], which is the hiring
+    [Company][google.cloud.talent.v4beta1.Company], which is the hiring
     entity responsible for the job.
 
     Attributes:
         name (str):
             Required during job update.
 
             The resource name for the job. This is generated by the
             service when a job is created.
 
             The format is
             "projects/{project_id}/tenants/{tenant_id}/jobs/{job_id}".
             For example, "projects/foo/tenants/bar/jobs/baz".
 
+            If tenant id is unspecified, the default tenant is used. For
+            example, "projects/foo/jobs/bar".
+
             Use of this field in job queries and API calls is preferred
             over the use of
-            [requisition_id][google.cloud.talent.v4.Job.requisition_id]
+            [requisition_id][google.cloud.talent.v4beta1.Job.requisition_id]
             since this value is unique.
         company (str):
             Required. The resource name of the company listing the job.
 
             The format is
             "projects/{project_id}/tenants/{tenant_id}/companies/{company_id}".
             For example, "projects/foo/tenants/bar/companies/baz".
+
+            If tenant id is unspecified, the default tenant is used. For
+            example, "projects/foo/companies/bar".
         requisition_id (str):
             Required. The requisition ID, also referred to as the
             posting ID, is assigned by the client to identify a job.
             This field is intended to be used by clients for client
             identification and tracking of postings. A job isn't allowed
             to be created if there is another job with the same
-            [company][google.cloud.talent.v4.Job.name],
-            [language_code][google.cloud.talent.v4.Job.language_code]
+            [company][google.cloud.talent.v4beta1.Job.name],
+            [language_code][google.cloud.talent.v4beta1.Job.language_code]
             and
-            [requisition_id][google.cloud.talent.v4.Job.requisition_id].
+            [requisition_id][google.cloud.talent.v4beta1.Job.requisition_id].
 
             The maximum number of allowed characters is 255.
         title (str):
             Required. The title of the job, such as
             "Software Engineer"
             The maximum number of allowed characters is 500.
         description (str):
             Required. The description of the job, which typically
             includes a multi-paragraph description of the company and
             related information. Separate fields are provided on the job
             object for
-            [responsibilities][google.cloud.talent.v4.Job.responsibilities],
-            [qualifications][google.cloud.talent.v4.Job.qualifications],
+            [responsibilities][google.cloud.talent.v4beta1.Job.responsibilities],
+            [qualifications][google.cloud.talent.v4beta1.Job.qualifications],
             and other job characteristics. Use of these separate job
             fields is recommended.
 
             This field accepts and sanitizes HTML input, and also
             accepts bold, italic, ordered list, and unordered list
             markup tags.
 
@@ -95,76 +101,65 @@
             Specifying the full street address(es) of the hiring
             location enables better API results, especially job searches
             by commute time.
 
             At most 50 locations are allowed for best search
             performance. If a job has more locations, it is suggested to
             split it into multiple jobs with unique
-            [requisition_id][google.cloud.talent.v4.Job.requisition_id]s
+            [requisition_id][google.cloud.talent.v4beta1.Job.requisition_id]s
             (e.g. 'ReqA' becomes 'ReqA-1', 'ReqA-2', and so on.) as
             multiple jobs with the same
-            [company][google.cloud.talent.v4.Job.company],
-            [language_code][google.cloud.talent.v4.Job.language_code]
+            [company][google.cloud.talent.v4beta1.Job.company],
+            [language_code][google.cloud.talent.v4beta1.Job.language_code]
             and
-            [requisition_id][google.cloud.talent.v4.Job.requisition_id]
+            [requisition_id][google.cloud.talent.v4beta1.Job.requisition_id]
             are not allowed. If the original
-            [requisition_id][google.cloud.talent.v4.Job.requisition_id]
+            [requisition_id][google.cloud.talent.v4beta1.Job.requisition_id]
             must be preserved, a custom field should be used for
             storage. It is also suggested to group the locations that
             close to each other in the same job for better search
             experience.
 
-            Jobs with multiple addresses must have their addresses with
-            the same [LocationType][] to allow location filtering to
-            work properly. (For example, a Job with addresses "1600
-            Amphitheatre Parkway, Mountain View, CA, USA" and "London,
-            UK" may not have location filters applied correctly at
-            search time since the first is a
-            [LocationType.STREET_ADDRESS][] and the second is a
-            [LocationType.LOCALITY][].) If a job needs to have multiple
-            addresses, it is suggested to split it into multiple jobs
-            with same LocationTypes.
-
             The maximum number of allowed characters is 500.
-        application_info (google.cloud.talent_v4.types.Job.ApplicationInfo):
+        application_info (google.cloud.talent_v4beta1.types.Job.ApplicationInfo):
             Job application information.
-        job_benefits (MutableSequence[google.cloud.talent_v4.types.JobBenefit]):
+        job_benefits (MutableSequence[google.cloud.talent_v4beta1.types.JobBenefit]):
             The benefits included with the job.
-        compensation_info (google.cloud.talent_v4.types.CompensationInfo):
+        compensation_info (google.cloud.talent_v4beta1.types.CompensationInfo):
             Job compensation information (a.k.a. "pay
             rate") i.e., the compensation that will paid to
             the employee.
-        custom_attributes (MutableMapping[str, google.cloud.talent_v4.types.CustomAttribute]):
+        custom_attributes (MutableMapping[str, google.cloud.talent_v4beta1.types.CustomAttribute]):
             A map of fields to hold both filterable and non-filterable
             custom job attributes that are not covered by the provided
             structured fields.
 
             The keys of the map are strings up to 64 bytes and must
             match the pattern: ``[a-zA-Z][a-zA-Z0-9_]*``. For example,
             key0LikeThis or KEY_1_LIKE_THIS.
 
             At most 100 filterable and at most 100 unfilterable keys are
             supported. For filterable ``string_values``, across all keys
             at most 200 values are allowed, with each string no more
             than 255 characters. For unfilterable ``string_values``, the
             maximum total size of ``string_values`` across all keys is
             50KB.
-        degree_types (MutableSequence[google.cloud.talent_v4.types.DegreeType]):
+        degree_types (MutableSequence[google.cloud.talent_v4beta1.types.DegreeType]):
             The desired education degrees for the job,
             such as Bachelors, Masters.
         department (str):
             The department or functional area within the
             company with the open position.
 
             The maximum number of allowed characters is 255.
-        employment_types (MutableSequence[google.cloud.talent_v4.types.EmploymentType]):
+        employment_types (MutableSequence[google.cloud.talent_v4beta1.types.EmploymentType]):
             The employment type(s) of a job, for example, [full
-            time][google.cloud.talent.v4.EmploymentType.FULL_TIME] or
-            [part
-            time][google.cloud.talent.v4.EmploymentType.PART_TIME].
+            time][google.cloud.talent.v4beta1.EmploymentType.FULL_TIME]
+            or [part
+            time][google.cloud.talent.v4beta1.EmploymentType.PART_TIME].
         incentives (str):
             A description of bonus, commission, and other
             compensation incentives associated with the job
             not including salary or pay.
             The maximum number of allowed characters is
             10,000.
         language_code (str):
@@ -173,19 +168,19 @@
 
             Language codes must be in BCP-47 format, such as "en-US" or
             "sr-Latn". For more information, see `Tags for Identifying
             Languages <https://tools.ietf.org/html/bcp47>`__\ {:
             class="external" target="_blank" }.
 
             If this field is unspecified and
-            [Job.description][google.cloud.talent.v4.Job.description] is
-            present, detected language code based on
-            [Job.description][google.cloud.talent.v4.Job.description] is
-            assigned, otherwise defaults to 'en_US'.
-        job_level (google.cloud.talent_v4.types.JobLevel):
+            [Job.description][google.cloud.talent.v4beta1.Job.description]
+            is present, detected language code based on
+            [Job.description][google.cloud.talent.v4beta1.Job.description]
+            is assigned, otherwise defaults to 'en_US'.
+        job_level (google.cloud.talent_v4beta1.types.JobLevel):
             The experience level associated with the job,
             such as "Entry Level".
         promotion_value (int):
             A promotion value of the job, as determined by the client.
             The value determines the sort order of the jobs returned
             when searching for jobs using the featured jobs search call,
             with higher promotional values being returned first and ties
@@ -193,53 +188,56 @@
             promotionValue >0 are returned in a FEATURED_JOB_SEARCH.
 
             Default value is 0, and negative values are treated as 0.
         qualifications (str):
             A description of the qualifications required to perform the
             job. The use of this field is recommended as an alternative
             to using the more general
-            [description][google.cloud.talent.v4.Job.description] field.
+            [description][google.cloud.talent.v4beta1.Job.description]
+            field.
 
             This field accepts and sanitizes HTML input, and also
             accepts bold, italic, ordered list, and unordered list
             markup tags.
 
             The maximum number of allowed characters is 10,000.
         responsibilities (str):
             A description of job responsibilities. The use of this field
             is recommended as an alternative to using the more general
-            [description][google.cloud.talent.v4.Job.description] field.
+            [description][google.cloud.talent.v4beta1.Job.description]
+            field.
 
             This field accepts and sanitizes HTML input, and also
             accepts bold, italic, ordered list, and unordered list
             markup tags.
 
             The maximum number of allowed characters is 10,000.
-        posting_region (google.cloud.talent_v4.types.PostingRegion):
+        posting_region (google.cloud.talent_v4beta1.types.PostingRegion):
             The job
-            [PostingRegion][google.cloud.talent.v4.PostingRegion] (for
-            example, state, country) throughout which the job is
+            [PostingRegion][google.cloud.talent.v4beta1.PostingRegion]
+            (for example, state, country) throughout which the job is
             available. If this field is set, a
-            [LocationFilter][google.cloud.talent.v4.LocationFilter] in a
-            search query within the job region finds this job posting if
-            an exact location match isn't specified. If this field is
-            set to
-            [PostingRegion.NATION][google.cloud.talent.v4.PostingRegion.NATION]
+            [LocationFilter][google.cloud.talent.v4beta1.LocationFilter]
+            in a search query within the job region finds this job
+            posting if an exact location match isn't specified. If this
+            field is set to
+            [PostingRegion.NATION][google.cloud.talent.v4beta1.PostingRegion.NATION]
             or
-            [PostingRegion.ADMINISTRATIVE_AREA][google.cloud.talent.v4.PostingRegion.ADMINISTRATIVE_AREA],
+            [PostingRegion.ADMINISTRATIVE_AREA][google.cloud.talent.v4beta1.PostingRegion.ADMINISTRATIVE_AREA],
             setting job
-            [Job.addresses][google.cloud.talent.v4.Job.addresses] to the
-            same location level as this field is strongly recommended.
-        visibility (google.cloud.talent_v4.types.Visibility):
+            [Job.addresses][google.cloud.talent.v4beta1.Job.addresses]
+            to the same location level as this field is strongly
+            recommended.
+        visibility (google.cloud.talent_v4beta1.types.Visibility):
             Deprecated. The job is only visible to the owner.
 
             The visibility of the job.
 
             Defaults to
-            [Visibility.ACCOUNT_ONLY][google.cloud.talent.v4.Visibility.ACCOUNT_ONLY]
+            [Visibility.ACCOUNT_ONLY][google.cloud.talent.v4beta1.Visibility.ACCOUNT_ONLY]
             if not specified.
         job_start_time (google.protobuf.timestamp_pb2.Timestamp):
             The start timestamp of the job in UTC time
             zone. Typically this field is used for
             contracting engagements. Invalid timestamps are
             ignored.
         job_end_time (google.protobuf.timestamp_pb2.Timestamp):
@@ -253,28 +251,28 @@
             timestamps are ignored.
         posting_expire_time (google.protobuf.timestamp_pb2.Timestamp):
             Strongly recommended for the best service experience.
 
             The expiration timestamp of the job. After this timestamp,
             the job is marked as expired, and it no longer appears in
             search results. The expired job can't be listed by the
-            [ListJobs][google.cloud.talent.v4.JobService.ListJobs] API,
-            but it can be retrieved with the
-            [GetJob][google.cloud.talent.v4.JobService.GetJob] API or
-            updated with the
-            [UpdateJob][google.cloud.talent.v4.JobService.UpdateJob] API
-            or deleted with the
-            [DeleteJob][google.cloud.talent.v4.JobService.DeleteJob]
+            [ListJobs][google.cloud.talent.v4beta1.JobService.ListJobs]
+            API, but it can be retrieved with the
+            [GetJob][google.cloud.talent.v4beta1.JobService.GetJob] API
+            or updated with the
+            [UpdateJob][google.cloud.talent.v4beta1.JobService.UpdateJob]
+            API or deleted with the
+            [DeleteJob][google.cloud.talent.v4beta1.JobService.DeleteJob]
             API. An expired job can be updated and opened again by using
             a future expiration timestamp. Updating an expired job fails
             if there is another existing open job with same
-            [company][google.cloud.talent.v4.Job.company],
-            [language_code][google.cloud.talent.v4.Job.language_code]
+            [company][google.cloud.talent.v4beta1.Job.company],
+            [language_code][google.cloud.talent.v4beta1.Job.language_code]
             and
-            [requisition_id][google.cloud.talent.v4.Job.requisition_id].
+            [requisition_id][google.cloud.talent.v4beta1.Job.requisition_id].
 
             The expired jobs are retained in our system for 90 days.
             However, the overall expired job count cannot exceed 3 times
             the maximum number of open jobs over previous 7 days. If
             this threshold is exceeded, expired jobs are cleaned out in
             order of earliest expire time. Expired jobs are no longer
             accessible after they are cleaned out.
@@ -282,50 +280,50 @@
             Invalid timestamps are ignored, and treated as expire time
             not provided.
 
             If the timestamp is before the instant request is made, the
             job is treated as expired immediately on creation. This kind
             of job can not be updated. And when creating a job with past
             timestamp, the
-            [posting_publish_time][google.cloud.talent.v4.Job.posting_publish_time]
+            [posting_publish_time][google.cloud.talent.v4beta1.Job.posting_publish_time]
             must be set before
-            [posting_expire_time][google.cloud.talent.v4.Job.posting_expire_time].
+            [posting_expire_time][google.cloud.talent.v4beta1.Job.posting_expire_time].
             The purpose of this feature is to allow other objects, such
-            as [Application][], to refer a job that didn't exist in the
-            system prior to becoming expired. If you want to modify a
-            job that was expired on creation, delete it and create a new
-            one.
+            as [Application][google.cloud.talent.v4beta1.Application],
+            to refer a job that didn't exist in the system prior to
+            becoming expired. If you want to modify a job that was
+            expired on creation, delete it and create a new one.
 
             If this value isn't provided at the time of job creation or
             is invalid, the job posting expires after 30 days from the
             job's creation time. For example, if the job was created on
             2017/01/01 13:00AM UTC with an unspecified expiration date,
             the job expires after 2017/01/31 13:00AM UTC.
 
             If this value isn't provided on job update, it depends on
             the field masks set by
-            [UpdateJobRequest.update_mask][google.cloud.talent.v4.UpdateJobRequest.update_mask].
+            [UpdateJobRequest.update_mask][google.cloud.talent.v4beta1.UpdateJobRequest.update_mask].
             If the field masks include
-            [job_end_time][google.cloud.talent.v4.Job.job_end_time], or
-            the masks are empty meaning that every field is updated, the
-            job posting expires after 30 days from the job's last update
-            time. Otherwise the expiration date isn't updated.
+            [job_end_time][google.cloud.talent.v4beta1.Job.job_end_time],
+            or the masks are empty meaning that every field is updated,
+            the job posting expires after 30 days from the job's last
+            update time. Otherwise the expiration date isn't updated.
         posting_create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when this job
             posting was created.
         posting_update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when this job
             posting was last updated.
         company_display_name (str):
             Output only. Display name of the company
             listing the job.
-        derived_info (google.cloud.talent_v4.types.Job.DerivedInfo):
+        derived_info (google.cloud.talent_v4beta1.types.Job.DerivedInfo):
             Output only. Derived details about the job
             posting.
-        processing_options (google.cloud.talent_v4.types.Job.ProcessingOptions):
+        processing_options (google.cloud.talent_v4beta1.types.Job.ProcessingOptions):
             Options for job processing.
     """
 
     class ApplicationInfo(proto.Message):
         r"""Application related details of a job posting.
 
         Attributes:
@@ -364,26 +362,26 @@
             number=3,
         )
 
     class DerivedInfo(proto.Message):
         r"""Derived details about the job posting.
 
         Attributes:
-            locations (MutableSequence[google.cloud.talent_v4.types.Location]):
+            locations (MutableSequence[google.cloud.talent_v4beta1.types.Location]):
                 Structured locations of the job, resolved from
-                [Job.addresses][google.cloud.talent.v4.Job.addresses].
+                [Job.addresses][google.cloud.talent.v4beta1.Job.addresses].
 
-                [locations][google.cloud.talent.v4.Job.DerivedInfo.locations]
+                [locations][google.cloud.talent.v4beta1.Job.DerivedInfo.locations]
                 are exactly matched to
-                [Job.addresses][google.cloud.talent.v4.Job.addresses] in the
-                same order.
-            job_categories (MutableSequence[google.cloud.talent_v4.types.JobCategory]):
+                [Job.addresses][google.cloud.talent.v4beta1.Job.addresses]
+                in the same order.
+            job_categories (MutableSequence[google.cloud.talent_v4beta1.types.JobCategory]):
                 Job categories derived from
-                [Job.title][google.cloud.talent.v4.Job.title] and
-                [Job.description][google.cloud.talent.v4.Job.description].
+                [Job.title][google.cloud.talent.v4beta1.Job.title] and
+                [Job.description][google.cloud.talent.v4beta1.Job.description].
         """
 
         locations: MutableSequence[common.Location] = proto.RepeatedField(
             proto.MESSAGE,
             number=1,
             message=common.Location,
         )
@@ -396,29 +394,29 @@
     class ProcessingOptions(proto.Message):
         r"""Options for job processing.
 
         Attributes:
             disable_street_address_resolution (bool):
                 If set to ``true``, the service does not attempt to resolve
                 a more precise address for the job.
-            html_sanitization (google.cloud.talent_v4.types.HtmlSanitization):
+            html_sanitization (google.cloud.talent_v4beta1.types.HtmlSanitization):
                 Option for job HTML content sanitization. Applied fields
                 are:
 
                 -  description
                 -  applicationInfo.instruction
                 -  incentives
                 -  qualifications
                 -  responsibilities
 
                 HTML tags in these fields may be stripped if sanitiazation
                 isn't disabled.
 
                 Defaults to
-                [HtmlSanitization.SIMPLE_FORMATTING_ONLY][google.cloud.talent.v4.HtmlSanitization.SIMPLE_FORMATTING_ONLY].
+                [HtmlSanitization.SIMPLE_FORMATTING_ONLY][google.cloud.talent.v4beta1.HtmlSanitization.SIMPLE_FORMATTING_ONLY].
         """
 
         disable_street_address_resolution: bool = proto.Field(
             proto.BOOL,
             number=1,
         )
         html_sanitization: common.HtmlSanitization = proto.Field(
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/types/job_service.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/types/job_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,45 @@
 
 class JobView(proto.Enum):
     r"""An enum that specifies the job attributes that are returned in the
     [MatchingJob.job][google.cloud.talent.v4.SearchJobsResponse.MatchingJob.job]
     or
     [ListJobsResponse.jobs][google.cloud.talent.v4.ListJobsResponse.jobs]
     fields.
+
+    Values:
+        JOB_VIEW_UNSPECIFIED (0):
+            Default value.
+        JOB_VIEW_ID_ONLY (1):
+            A ID only view of job, with following attributes:
+            [Job.name][google.cloud.talent.v4.Job.name],
+            [Job.requisition_id][google.cloud.talent.v4.Job.requisition_id],
+            [Job.language_code][google.cloud.talent.v4.Job.language_code].
+        JOB_VIEW_MINIMAL (2):
+            A minimal view of the job, with the following attributes:
+            [Job.name][google.cloud.talent.v4.Job.name],
+            [Job.requisition_id][google.cloud.talent.v4.Job.requisition_id],
+            [Job.title][google.cloud.talent.v4.Job.title],
+            [Job.company][google.cloud.talent.v4.Job.company],
+            [Job.DerivedInfo.locations][google.cloud.talent.v4.Job.DerivedInfo.locations],
+            [Job.language_code][google.cloud.talent.v4.Job.language_code].
+        JOB_VIEW_SMALL (3):
+            A small view of the job, with the following attributes in
+            the search results:
+            [Job.name][google.cloud.talent.v4.Job.name],
+            [Job.requisition_id][google.cloud.talent.v4.Job.requisition_id],
+            [Job.title][google.cloud.talent.v4.Job.title],
+            [Job.company][google.cloud.talent.v4.Job.company],
+            [Job.DerivedInfo.locations][google.cloud.talent.v4.Job.DerivedInfo.locations],
+            [Job.visibility][google.cloud.talent.v4.Job.visibility],
+            [Job.language_code][google.cloud.talent.v4.Job.language_code],
+            [Job.description][google.cloud.talent.v4.Job.description].
+        JOB_VIEW_FULL (4):
+            All available attributes are included in the
+            search results.
     """
     JOB_VIEW_UNSPECIFIED = 0
     JOB_VIEW_ID_ONLY = 1
     JOB_VIEW_MINIMAL = 2
     JOB_VIEW_SMALL = 3
     JOB_VIEW_FULL = 4
 
@@ -567,14 +598,32 @@
             [KeywordMatchMode.KEYWORD_MATCH_ALL][google.cloud.talent.v4.SearchJobsRequest.KeywordMatchMode.KEYWORD_MATCH_ALL]
             if no value is specified.
     """
 
     class SearchMode(proto.Enum):
         r"""A string-represented enumeration of the job search mode. The
         service operate differently for different modes of service.
+
+        Values:
+            SEARCH_MODE_UNSPECIFIED (0):
+                The mode of the search method isn't specified. The default
+                search behavior is identical to JOB_SEARCH search behavior.
+            JOB_SEARCH (1):
+                The job search matches against all jobs, and
+                featured jobs (jobs with promotionValue > 0) are
+                not specially handled.
+            FEATURED_JOB_SEARCH (2):
+                The job search matches only against featured
+                jobs (jobs with a promotionValue > 0). This
+                method doesn't return any jobs having a
+                promotionValue <= 0. The search results order is
+                determined by the promotionValue (jobs with a
+                higher promotionValue are returned higher up in
+                the search results), with relevance being used
+                as a tiebreaker.
         """
         SEARCH_MODE_UNSPECIFIED = 0
         JOB_SEARCH = 1
         FEATURED_JOB_SEARCH = 2
 
     class DiversificationLevel(proto.Enum):
         r"""Controls whether highly similar jobs are returned next to
@@ -585,14 +634,45 @@
         higher up in the results, with the other jobs being displayed
         lower down in the results.
 
         If you are using pageToken to page through the result set,
         latency might be lower but we can't guarantee that all results
         are returned. If you are using page offset, latency might be
         higher but all results are returned.
+
+        Values:
+            DIVERSIFICATION_LEVEL_UNSPECIFIED (0):
+                The diversification level isn't specified.
+            DISABLED (1):
+                Disables diversification. Jobs that would
+                normally be pushed to the last page would not
+                have their positions altered. This may result in
+                highly similar jobs appearing in sequence in the
+                search results.
+            SIMPLE (2):
+                Default diversifying behavior. The result
+                list is ordered so that highly similar results
+                are pushed to the end of the last page of search
+                results.
+            ONE_PER_COMPANY (3):
+                Only one job from the same company will be
+                shown at once, other jobs under same company are
+                pushed to the end of the last page of search
+                result.
+            TWO_PER_COMPANY (4):
+                Similar to ONE_PER_COMPANY, but it allows at most two jobs
+                in the same company to be shown at once, the other jobs
+                under same company are pushed to the end of the last page of
+                search result.
+            DIVERSIFY_BY_LOOSER_SIMILARITY (5):
+                The result list is ordered such that somewhat
+                similar results are pushed to the end of the
+                last page of the search results. This option is
+                recommended if SIMPLE diversification does not
+                diversify enough.
         """
         DIVERSIFICATION_LEVEL_UNSPECIFIED = 0
         DISABLED = 1
         SIMPLE = 2
         ONE_PER_COMPANY = 3
         TWO_PER_COMPANY = 4
         DIVERSIFY_BY_LOOSER_SIMILARITY = 5
@@ -611,14 +691,35 @@
         regardless of this enum's value.
 
         Use
         [Company.keyword_searchable_job_custom_attributes][google.cloud.talent.v4.Company.keyword_searchable_job_custom_attributes]
         if company-specific globally matched custom field/attribute string
         values are needed. Enabling keyword match improves recall of
         subsequent search requests.
+
+        Values:
+            KEYWORD_MATCH_MODE_UNSPECIFIED (0):
+                The keyword match option isn't specified. Defaults to
+                [KeywordMatchMode.KEYWORD_MATCH_ALL][google.cloud.talent.v4.SearchJobsRequest.KeywordMatchMode.KEYWORD_MATCH_ALL]
+                behavior.
+            KEYWORD_MATCH_DISABLED (1):
+                Disables keyword matching.
+            KEYWORD_MATCH_ALL (2):
+                Enable keyword matching over
+                [Job.title][google.cloud.talent.v4.Job.title],
+                [Job.description][google.cloud.talent.v4.Job.description],
+                [Job.company_display_name][google.cloud.talent.v4.Job.company_display_name],
+                [Job.addresses][google.cloud.talent.v4.Job.addresses],
+                [Job.qualifications][google.cloud.talent.v4.Job.qualifications],
+                and keyword searchable
+                [Job.custom_attributes][google.cloud.talent.v4.Job.custom_attributes]
+                fields.
+            KEYWORD_MATCH_TITLE_ONLY (3):
+                Only enable keyword matching over
+                [Job.title][google.cloud.talent.v4.Job.title].
         """
         KEYWORD_MATCH_MODE_UNSPECIFIED = 0
         KEYWORD_MATCH_DISABLED = 1
         KEYWORD_MATCH_ALL = 2
         KEYWORD_MATCH_TITLE_ONLY = 3
 
     class CustomRankingInfo(proto.Message):
@@ -659,14 +760,49 @@
                 Sample ranking expression (year + 25) \* 0.25 - (freshness /
                 0.5)
         """
 
         class ImportanceLevel(proto.Enum):
             r"""The importance level for
             [CustomRankingInfo.ranking_expression][google.cloud.talent.v4.SearchJobsRequest.CustomRankingInfo.ranking_expression].
+
+            Values:
+                IMPORTANCE_LEVEL_UNSPECIFIED (0):
+                    Default value if the importance level isn't
+                    specified.
+                NONE (1):
+                    The given ranking expression is of None
+                    importance, existing relevance score (determined
+                    by API algorithm) dominates job's final ranking
+                    position.
+                LOW (2):
+                    The given ranking expression is of Low
+                    importance in terms of job's final ranking
+                    position compared to existing relevance score
+                    (determined by API algorithm).
+                MILD (3):
+                    The given ranking expression is of Mild
+                    importance in terms of job's final ranking
+                    position compared to existing relevance score
+                    (determined by API algorithm).
+                MEDIUM (4):
+                    The given ranking expression is of Medium
+                    importance in terms of job's final ranking
+                    position compared to existing relevance score
+                    (determined by API algorithm).
+                HIGH (5):
+                    The given ranking expression is of High
+                    importance in terms of job's final ranking
+                    position compared to existing relevance score
+                    (determined by API algorithm).
+                EXTREME (6):
+                    The given ranking expression is of Extreme
+                    importance, and dominates job's final ranking
+                    position with existing relevance score
+                    (determined by API algorithm) ignored.
             """
             IMPORTANCE_LEVEL_UNSPECIFIED = 0
             NONE = 1
             LOW = 2
             MILD = 3
             MEDIUM = 4
             HIGH = 5
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/types/tenant.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/types/tenant.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             service when a tenant is created.
 
             The format is "projects/{project_id}/tenants/{tenant_id}",
             for example, "projects/foo/tenants/bar".
         external_id (str):
             Required. Client side tenant identifier, used
             to uniquely identify the tenant.
+
             The maximum number of allowed characters is 255.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4/types/tenant_service.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4/types/tenant_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/gapic_metadata.json` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/gapic_version.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/async_client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1015,15 +1015,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "CompanyServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/pagers.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/transports/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/transports/base.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/transports/grpc.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/company_service/transports/grpc_asyncio.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/company_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/async_client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,15 +518,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "CompletionClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/transports/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/transports/base.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/transports/grpc.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/completion/transports/grpc_asyncio.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/completion/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/async_client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,15 +575,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "EventServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/transports/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/transports/base.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/transports/grpc.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/event_service/transports/grpc_asyncio.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/event_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/async_client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.talent_v4beta1.types.JobOperationResult` The result of [JobService.BatchCreateJobs][google.cloud.talent.v4beta1.JobService.BatchCreateJobs] or
+                The result type for the operation will be :class:`google.cloud.talent_v4beta1.types.JobOperationResult` The result of
+                   [JobService.BatchCreateJobs][google.cloud.talent.v4beta1.JobService.BatchCreateJobs]
+                   or
                    [JobService.BatchUpdateJobs][google.cloud.talent.v4beta1.JobService.BatchUpdateJobs]
                    APIs. It's used to replace
                    [google.longrunning.Operation.response][google.longrunning.Operation.response]
                    in case of success.
 
         """
         # Create or coerce a protobuf request object.
@@ -791,15 +793,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.talent_v4beta1.types.JobOperationResult` The result of [JobService.BatchCreateJobs][google.cloud.talent.v4beta1.JobService.BatchCreateJobs] or
+                The result type for the operation will be :class:`google.cloud.talent_v4beta1.types.JobOperationResult` The result of
+                   [JobService.BatchCreateJobs][google.cloud.talent.v4beta1.JobService.BatchCreateJobs]
+                   or
                    [JobService.BatchUpdateJobs][google.cloud.talent.v4beta1.JobService.BatchUpdateJobs]
                    APIs. It's used to replace
                    [google.longrunning.Operation.response][google.longrunning.Operation.response]
                    in case of success.
 
         """
         # Create or coerce a protobuf request object.
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -673,15 +673,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.talent_v4beta1.types.JobOperationResult` The result of [JobService.BatchCreateJobs][google.cloud.talent.v4beta1.JobService.BatchCreateJobs] or
+                The result type for the operation will be :class:`google.cloud.talent_v4beta1.types.JobOperationResult` The result of
+                   [JobService.BatchCreateJobs][google.cloud.talent.v4beta1.JobService.BatchCreateJobs]
+                   or
                    [JobService.BatchUpdateJobs][google.cloud.talent.v4beta1.JobService.BatchUpdateJobs]
                    APIs. It's used to replace
                    [google.longrunning.Operation.response][google.longrunning.Operation.response]
                    in case of success.
 
         """
         # Create or coerce a protobuf request object.
@@ -1032,15 +1034,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.talent_v4beta1.types.JobOperationResult` The result of [JobService.BatchCreateJobs][google.cloud.talent.v4beta1.JobService.BatchCreateJobs] or
+                The result type for the operation will be :class:`google.cloud.talent_v4beta1.types.JobOperationResult` The result of
+                   [JobService.BatchCreateJobs][google.cloud.talent.v4beta1.JobService.BatchCreateJobs]
+                   or
                    [JobService.BatchUpdateJobs][google.cloud.talent.v4beta1.JobService.BatchUpdateJobs]
                    APIs. It's used to replace
                    [google.longrunning.Operation.response][google.longrunning.Operation.response]
                    in case of success.
 
         """
         # Create or coerce a protobuf request object.
@@ -1664,15 +1668,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "JobServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/pagers.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/transports/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/transports/base.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/transports/grpc.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/job_service/transports/grpc_asyncio.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/job_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/async_client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/client.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -991,15 +991,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "TenantServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/pagers.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/transports/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/transports/base.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/transports/grpc.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/services/tenant_service/transports/grpc_asyncio.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/services/tenant_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/__init__.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/batch.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/common.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/filters.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,840 +11,579 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from typing import MutableMapping, MutableSequence
 
-from google.protobuf import timestamp_pb2  # type: ignore
-from google.protobuf import wrappers_pb2  # type: ignore
+from google.protobuf import duration_pb2  # type: ignore
 from google.type import latlng_pb2  # type: ignore
-from google.type import money_pb2  # type: ignore
-from google.type import postal_address_pb2  # type: ignore
+from google.type import timeofday_pb2  # type: ignore
 import proto  # type: ignore
 
+from google.cloud.talent_v4beta1.types import common
+
 __protobuf__ = proto.module(
     package="google.cloud.talent.v4beta1",
     manifest={
-        "CompanySize",
-        "JobBenefit",
-        "DegreeType",
-        "EmploymentType",
-        "JobLevel",
-        "JobCategory",
-        "PostingRegion",
-        "Visibility",
-        "HtmlSanitization",
-        "CommuteMethod",
-        "TimestampRange",
-        "Location",
-        "RequestMetadata",
-        "ResponseMetadata",
-        "DeviceInfo",
-        "CustomAttribute",
-        "SpellingCorrection",
-        "CompensationInfo",
-        "BatchOperationMetadata",
+        "JobQuery",
+        "LocationFilter",
+        "CompensationFilter",
+        "CommuteFilter",
     },
 )
 
 
-class CompanySize(proto.Enum):
-    r"""An enum that represents the size of the company."""
-    COMPANY_SIZE_UNSPECIFIED = 0
-    MINI = 1
-    SMALL = 2
-    SMEDIUM = 3
-    MEDIUM = 4
-    BIG = 5
-    BIGGER = 6
-    GIANT = 7
-
-
-class JobBenefit(proto.Enum):
-    r"""An enum that represents employee benefits included with the
-    job.
-    """
-    JOB_BENEFIT_UNSPECIFIED = 0
-    CHILD_CARE = 1
-    DENTAL = 2
-    DOMESTIC_PARTNER = 3
-    FLEXIBLE_HOURS = 4
-    MEDICAL = 5
-    LIFE_INSURANCE = 6
-    PARENTAL_LEAVE = 7
-    RETIREMENT_PLAN = 8
-    SICK_DAYS = 9
-    VACATION = 10
-    VISION = 11
-
-
-class DegreeType(proto.Enum):
-    r"""Educational degree level defined in International Standard
-    Classification of Education (ISCED).
-    """
-    DEGREE_TYPE_UNSPECIFIED = 0
-    PRIMARY_EDUCATION = 1
-    LOWER_SECONDARY_EDUCATION = 2
-    UPPER_SECONDARY_EDUCATION = 3
-    ADULT_REMEDIAL_EDUCATION = 4
-    ASSOCIATES_OR_EQUIVALENT = 5
-    BACHELORS_OR_EQUIVALENT = 6
-    MASTERS_OR_EQUIVALENT = 7
-    DOCTORAL_OR_EQUIVALENT = 8
-
-
-class EmploymentType(proto.Enum):
-    r"""An enum that represents the employment type of a job."""
-    EMPLOYMENT_TYPE_UNSPECIFIED = 0
-    FULL_TIME = 1
-    PART_TIME = 2
-    CONTRACTOR = 3
-    CONTRACT_TO_HIRE = 4
-    TEMPORARY = 5
-    INTERN = 6
-    VOLUNTEER = 7
-    PER_DIEM = 8
-    FLY_IN_FLY_OUT = 9
-    OTHER_EMPLOYMENT_TYPE = 10
-
-
-class JobLevel(proto.Enum):
-    r"""An enum that represents the required experience level
-    required for the job.
-    """
-    JOB_LEVEL_UNSPECIFIED = 0
-    ENTRY_LEVEL = 1
-    EXPERIENCED = 2
-    MANAGER = 3
-    DIRECTOR = 4
-    EXECUTIVE = 5
-
-
-class JobCategory(proto.Enum):
-    r"""An enum that represents the categorization or primary focus
-    of specific role. This value is different than the "industry"
-    associated with a role, which is related to the categorization
-    of the company listing the job.
-    """
-    JOB_CATEGORY_UNSPECIFIED = 0
-    ACCOUNTING_AND_FINANCE = 1
-    ADMINISTRATIVE_AND_OFFICE = 2
-    ADVERTISING_AND_MARKETING = 3
-    ANIMAL_CARE = 4
-    ART_FASHION_AND_DESIGN = 5
-    BUSINESS_OPERATIONS = 6
-    CLEANING_AND_FACILITIES = 7
-    COMPUTER_AND_IT = 8
-    CONSTRUCTION = 9
-    CUSTOMER_SERVICE = 10
-    EDUCATION = 11
-    ENTERTAINMENT_AND_TRAVEL = 12
-    FARMING_AND_OUTDOORS = 13
-    HEALTHCARE = 14
-    HUMAN_RESOURCES = 15
-    INSTALLATION_MAINTENANCE_AND_REPAIR = 16
-    LEGAL = 17
-    MANAGEMENT = 18
-    MANUFACTURING_AND_WAREHOUSE = 19
-    MEDIA_COMMUNICATIONS_AND_WRITING = 20
-    OIL_GAS_AND_MINING = 21
-    PERSONAL_CARE_AND_SERVICES = 22
-    PROTECTIVE_SERVICES = 23
-    REAL_ESTATE = 24
-    RESTAURANT_AND_HOSPITALITY = 25
-    SALES_AND_RETAIL = 26
-    SCIENCE_AND_ENGINEERING = 27
-    SOCIAL_SERVICES_AND_NON_PROFIT = 28
-    SPORTS_FITNESS_AND_RECREATION = 29
-    TRANSPORTATION_AND_LOGISTICS = 30
-
-
-class PostingRegion(proto.Enum):
-    r"""An enum that represents the job posting region. In most
-    cases, job postings don't need to specify a region. If a region
-    is given, jobs are eligible for searches in the specified
-    region.
-    """
-    POSTING_REGION_UNSPECIFIED = 0
-    ADMINISTRATIVE_AREA = 1
-    NATION = 2
-    TELECOMMUTE = 3
-
-
-class Visibility(proto.Enum):
-    r"""Deprecated. All resources are only visible to the owner.
-    An enum that represents who has view access to the resource.
-    """
-    _pb_options = {"deprecated": True}
-    VISIBILITY_UNSPECIFIED = 0
-    ACCOUNT_ONLY = 1
-    SHARED_WITH_GOOGLE = 2
-    SHARED_WITH_PUBLIC = 3
-
-
-class HtmlSanitization(proto.Enum):
-    r"""Option for HTML content sanitization on user input fields,
-    for example, job description. By setting this option, user can
-    determine whether and how sanitization is performed on these
-    fields.
-    """
-    HTML_SANITIZATION_UNSPECIFIED = 0
-    HTML_SANITIZATION_DISABLED = 1
-    SIMPLE_FORMATTING_ONLY = 2
-
-
-class CommuteMethod(proto.Enum):
-    r"""Method for commute."""
-    COMMUTE_METHOD_UNSPECIFIED = 0
-    DRIVING = 1
-    TRANSIT = 2
-    WALKING = 3
-    CYCLING = 4
-
-
-class TimestampRange(proto.Message):
-    r"""Message representing a period of time between two timestamps.
+class JobQuery(proto.Message):
+    r"""The query required to perform a search query.
 
     Attributes:
-        start_time (google.protobuf.timestamp_pb2.Timestamp):
-            Begin of the period (inclusive).
-        end_time (google.protobuf.timestamp_pb2.Timestamp):
-            End of the period (exclusive).
-    """
+        query (str):
+            The query string that matches against the job
+            title, description, and location fields.
 
-    start_time: timestamp_pb2.Timestamp = proto.Field(
-        proto.MESSAGE,
-        number=1,
-        message=timestamp_pb2.Timestamp,
-    )
-    end_time: timestamp_pb2.Timestamp = proto.Field(
-        proto.MESSAGE,
-        number=2,
-        message=timestamp_pb2.Timestamp,
-    )
-
-
-class Location(proto.Message):
-    r"""A resource that represents a location with full geographic
-    information.
-
-    Attributes:
-        location_type (google.cloud.talent_v4beta1.types.Location.LocationType):
-            The type of a location, which corresponds to the address
-            lines field of
-            [google.type.PostalAddress][google.type.PostalAddress]. For
-            example, "Downtown, Atlanta, GA, USA" has a type of
-            [LocationType.NEIGHBORHOOD][google.cloud.talent.v4beta1.Location.LocationType.NEIGHBORHOOD],
-            and "Kansas City, KS, USA" has a type of
-            [LocationType.LOCALITY][google.cloud.talent.v4beta1.Location.LocationType.LOCALITY].
-        postal_address (google.type.postal_address_pb2.PostalAddress):
-            Postal address of the location that includes
-            human readable information, such as postal
-            delivery and payments addresses. Given a postal
-            address, a postal service can deliver items to a
-            premises, P.O. Box, or other delivery location.
-        lat_lng (google.type.latlng_pb2.LatLng):
-            An object representing a latitude/longitude
-            pair.
-        radius_miles (float):
-            Radius in miles of the job location. This value is derived
-            from the location bounding box in which a circle with the
-            specified radius centered from
-            [google.type.LatLng][google.type.LatLng] covers the area
-            associated with the job location. For example, currently,
-            "Mountain View, CA, USA" has a radius of 6.17 miles.
+            The maximum number of allowed characters is 255.
+        query_language_code (str):
+            The language code of
+            [query][google.cloud.talent.v4beta1.JobQuery.query]. For
+            example, "en-US". This field helps to better interpret the
+            query.
+
+            If a value isn't specified, the query language code is
+            automatically detected, which may not be accurate.
+
+            Language code should be in BCP-47 format, such as "en-US" or
+            "sr-Latn". For more information, see `Tags for Identifying
+            Languages <https://tools.ietf.org/html/bcp47>`__.
+        companies (MutableSequence[str]):
+            This filter specifies the company entities to search
+            against.
+
+            If a value isn't specified, jobs are searched for against
+            all companies.
+
+            If multiple values are specified, jobs are searched against
+            the companies specified.
+
+            The format is
+            "projects/{project_id}/tenants/{tenant_id}/companies/{company_id}".
+            For example, "projects/foo/tenants/bar/companies/baz".
+
+            If tenant id is unspecified, the default tenant is used. For
+            example, "projects/foo/companies/bar".
+
+            At most 20 company filters are allowed.
+        location_filters (MutableSequence[google.cloud.talent_v4beta1.types.LocationFilter]):
+            The location filter specifies geo-regions containing the
+            jobs to search against. See
+            [LocationFilter][google.cloud.talent.v4beta1.LocationFilter]
+            for more information.
+
+            If a location value isn't specified, jobs fitting the other
+            search criteria are retrieved regardless of where they're
+            located.
+
+            If multiple values are specified, jobs are retrieved from
+            any of the specified locations. If different values are
+            specified for the
+            [LocationFilter.distance_in_miles][google.cloud.talent.v4beta1.LocationFilter.distance_in_miles]
+            parameter, the maximum provided distance is used for all
+            locations.
+
+            At most 5 location filters are allowed.
+        job_categories (MutableSequence[google.cloud.talent_v4beta1.types.JobCategory]):
+            The category filter specifies the categories of jobs to
+            search against. See
+            [JobCategory][google.cloud.talent.v4beta1.JobCategory] for
+            more information.
+
+            If a value isn't specified, jobs from any category are
+            searched against.
+
+            If multiple values are specified, jobs from any of the
+            specified categories are searched against.
+        commute_filter (google.cloud.talent_v4beta1.types.CommuteFilter):
+            Allows filtering jobs by commute time with different travel
+            methods (for example, driving or public transit).
+
+            Note: This only works when you specify a
+            [CommuteMethod][google.cloud.talent.v4beta1.CommuteMethod].
+            In this case,
+            [location_filters][google.cloud.talent.v4beta1.JobQuery.location_filters]
+            is ignored.
+
+            Currently we don't support sorting by commute time.
+        company_display_names (MutableSequence[str]):
+            This filter specifies the company
+            [Company.display_name][google.cloud.talent.v4beta1.Company.display_name]
+            of the jobs to search against. The company name must match
+            the value exactly.
+
+            Alternatively, the value being searched for can be wrapped
+            in different match operators. ``SUBSTRING_MATCH([value])``
+            The company name must contain a case insensitive substring
+            match of the value. Using this function may increase
+            latency.
+
+            Sample Value: ``SUBSTRING_MATCH(google)``
+
+            ``MULTI_WORD_TOKEN_MATCH([value])`` The value will be
+            treated as a multi word token and the company name must
+            contain a case insensitive match of the value. Using this
+            function may increase latency.
+
+            Sample Value: ``MULTI_WORD_TOKEN_MATCH(google)``
+
+            If a value isn't specified, jobs within the search results
+            are associated with any company.
+
+            If multiple values are specified, jobs within the search
+            results may be associated with any of the specified
+            companies.
+
+            At most 20 company display name filters are allowed.
+        compensation_filter (google.cloud.talent_v4beta1.types.CompensationFilter):
+            This search filter is applied only to
+            [Job.compensation_info][google.cloud.talent.v4beta1.Job.compensation_info].
+            For example, if the filter is specified as "Hourly job with
+            per-hour compensation > $15", only jobs meeting these
+            criteria are searched. If a filter isn't defined, all open
+            jobs are searched.
+        custom_attribute_filter (str):
+            This filter specifies a structured syntax to match against
+            the
+            [Job.custom_attributes][google.cloud.talent.v4beta1.Job.custom_attributes]
+            marked as ``filterable``.
+
+            The syntax for this expression is a subset of SQL syntax.
+
+            Supported operators are: ``=``, ``!=``, ``<``, ``<=``,
+            ``>``, and ``>=`` where the left of the operator is a custom
+            field key and the right of the operator is a number or a
+            quoted string. You must escape backslash (\) and quote (")
+            characters.
+
+            Supported functions are ``LOWER([field_name])`` to perform a
+            case insensitive match and ``EMPTY([field_name])`` to filter
+            on the existence of a key.
+
+            Boolean expressions (AND/OR/NOT) are supported up to 3
+            levels of nesting (for example, "((A AND B AND C) OR NOT D)
+            AND E"), a maximum of 100 comparisons or functions are
+            allowed in the expression. The expression must be < 10000
+            bytes in length.
+
+            Sample Query:
+            ``(LOWER(driving_license)="class \"a\"" OR EMPTY(driving_license)) AND driving_years > 10``
+        disable_spell_check (bool):
+            This flag controls the spell-check feature.
+            If false, the service attempts to correct a
+            misspelled query, for example, "enginee" is
+            corrected to "engineer".
+            Defaults to false: a spell check is performed.
+        employment_types (MutableSequence[google.cloud.talent_v4beta1.types.EmploymentType]):
+            The employment type filter specifies the employment type of
+            jobs to search against, such as
+            [EmploymentType.FULL_TIME][google.cloud.talent.v4beta1.EmploymentType.FULL_TIME].
+
+            If a value isn't specified, jobs in the search results
+            includes any employment type.
+
+            If multiple values are specified, jobs in the search results
+            include any of the specified employment types.
+        language_codes (MutableSequence[str]):
+            This filter specifies the locale of jobs to search against,
+            for example, "en-US".
+
+            If a value isn't specified, the search results can contain
+            jobs in any locale.
+
+            Language codes should be in BCP-47 format, such as "en-US"
+            or "sr-Latn". For more information, see `Tags for
+            Identifying
+            Languages <https://tools.ietf.org/html/bcp47>`__.
+
+            At most 10 language code filters are allowed.
+        publish_time_range (google.cloud.talent_v4beta1.types.TimestampRange):
+            Jobs published within a range specified by
+            this filter are searched against.
+        excluded_jobs (MutableSequence[str]):
+            This filter specifies a list of job names to
+            be excluded during search.
+            At most 400 excluded job names are allowed.
     """
 
-    class LocationType(proto.Enum):
-        r"""An enum which represents the type of a location."""
-        LOCATION_TYPE_UNSPECIFIED = 0
-        COUNTRY = 1
-        ADMINISTRATIVE_AREA = 2
-        SUB_ADMINISTRATIVE_AREA = 3
-        LOCALITY = 4
-        POSTAL_CODE = 5
-        SUB_LOCALITY = 6
-        SUB_LOCALITY_1 = 7
-        SUB_LOCALITY_2 = 8
-        NEIGHBORHOOD = 9
-        STREET_ADDRESS = 10
-
-    location_type: LocationType = proto.Field(
-        proto.ENUM,
+    query: str = proto.Field(
+        proto.STRING,
         number=1,
-        enum=LocationType,
     )
-    postal_address: postal_address_pb2.PostalAddress = proto.Field(
-        proto.MESSAGE,
+    query_language_code: str = proto.Field(
+        proto.STRING,
+        number=14,
+    )
+    companies: MutableSequence[str] = proto.RepeatedField(
+        proto.STRING,
         number=2,
-        message=postal_address_pb2.PostalAddress,
     )
-    lat_lng: latlng_pb2.LatLng = proto.Field(
+    location_filters: MutableSequence["LocationFilter"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
-        message=latlng_pb2.LatLng,
+        message="LocationFilter",
     )
-    radius_miles: float = proto.Field(
-        proto.DOUBLE,
+    job_categories: MutableSequence[common.JobCategory] = proto.RepeatedField(
+        proto.ENUM,
         number=4,
+        enum=common.JobCategory,
     )
-
-
-class RequestMetadata(proto.Message):
-    r"""Meta information related to the job searcher or entity
-    conducting the job search. This information is used to improve
-    the performance of the service.
-
-    Attributes:
-        domain (str):
-            Required if
-            [allow_missing_ids][google.cloud.talent.v4beta1.RequestMetadata.allow_missing_ids]
-            is unset or ``false``.
-
-            The client-defined scope or source of the service call,
-            which typically is the domain on which the service has been
-            implemented and is currently being run.
-
-            For example, if the service is being run by client Foo,
-            Inc., on job board www.foo.com and career site www.bar.com,
-            then this field is set to "foo.com" for use on the job
-            board, and "bar.com" for use on the career site.
-
-            Note that any improvements to the model for a particular
-            tenant site rely on this field being set correctly to a
-            unique domain.
-
-            The maximum number of allowed characters is 255.
-        session_id (str):
-            Required if
-            [allow_missing_ids][google.cloud.talent.v4beta1.RequestMetadata.allow_missing_ids]
-            is unset or ``false``.
-
-            A unique session identification string. A session is defined
-            as the duration of an end user's interaction with the
-            service over a certain period. Obfuscate this field for
-            privacy concerns before providing it to the service.
-
-            Note that any improvements to the model for a particular
-            tenant site rely on this field being set correctly to a
-            unique session ID.
-
-            The maximum number of allowed characters is 255.
-        user_id (str):
-            Required if
-            [allow_missing_ids][google.cloud.talent.v4beta1.RequestMetadata.allow_missing_ids]
-            is unset or ``false``.
-
-            A unique user identification string, as determined by the
-            client. To have the strongest positive impact on search
-            quality make sure the client-level is unique. Obfuscate this
-            field for privacy concerns before providing it to the
-            service.
-
-            Note that any improvements to the model for a particular
-            tenant site rely on this field being set correctly to a
-            unique user ID.
-
-            The maximum number of allowed characters is 255.
-        allow_missing_ids (bool):
-            Only set when any of
-            [domain][google.cloud.talent.v4beta1.RequestMetadata.domain],
-            [session_id][google.cloud.talent.v4beta1.RequestMetadata.session_id]
-            and
-            [user_id][google.cloud.talent.v4beta1.RequestMetadata.user_id]
-            isn't available for some reason. It is highly recommended
-            not to set this field and provide accurate
-            [domain][google.cloud.talent.v4beta1.RequestMetadata.domain],
-            [session_id][google.cloud.talent.v4beta1.RequestMetadata.session_id]
-            and
-            [user_id][google.cloud.talent.v4beta1.RequestMetadata.user_id]
-            for the best service experience.
-        device_info (google.cloud.talent_v4beta1.types.DeviceInfo):
-            The type of device used by the job seeker at
-            the time of the call to the service.
-    """
-
-    domain: str = proto.Field(
-        proto.STRING,
-        number=1,
+    commute_filter: "CommuteFilter" = proto.Field(
+        proto.MESSAGE,
+        number=5,
+        message="CommuteFilter",
     )
-    session_id: str = proto.Field(
+    company_display_names: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
-        number=2,
+        number=6,
+    )
+    compensation_filter: "CompensationFilter" = proto.Field(
+        proto.MESSAGE,
+        number=7,
+        message="CompensationFilter",
     )
-    user_id: str = proto.Field(
+    custom_attribute_filter: str = proto.Field(
         proto.STRING,
-        number=3,
+        number=8,
     )
-    allow_missing_ids: bool = proto.Field(
+    disable_spell_check: bool = proto.Field(
         proto.BOOL,
-        number=4,
+        number=9,
     )
-    device_info: "DeviceInfo" = proto.Field(
-        proto.MESSAGE,
-        number=5,
-        message="DeviceInfo",
+    employment_types: MutableSequence[common.EmploymentType] = proto.RepeatedField(
+        proto.ENUM,
+        number=10,
+        enum=common.EmploymentType,
     )
-
-
-class ResponseMetadata(proto.Message):
-    r"""Additional information returned to client, such as debugging
-    information.
-
-    Attributes:
-        request_id (str):
-            A unique id associated with this call.
-            This id is logged for tracking purposes.
-    """
-
-    request_id: str = proto.Field(
+    language_codes: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
-        number=1,
+        number=11,
     )
-
-
-class DeviceInfo(proto.Message):
-    r"""Device information collected from the job seeker, candidate,
-    or other entity conducting the job search. Providing this
-    information improves the quality of the search results across
-    devices.
-
-    Attributes:
-        device_type (google.cloud.talent_v4beta1.types.DeviceInfo.DeviceType):
-            Type of the device.
-        id (str):
-            A device-specific ID. The ID must be a unique
-            identifier that distinguishes the device from
-            other devices.
-    """
-
-    class DeviceType(proto.Enum):
-        r"""An enumeration describing an API access portal and exposure
-        mechanism.
-        """
-        DEVICE_TYPE_UNSPECIFIED = 0
-        WEB = 1
-        MOBILE_WEB = 2
-        ANDROID = 3
-        IOS = 4
-        BOT = 5
-        OTHER = 6
-
-    device_type: DeviceType = proto.Field(
-        proto.ENUM,
-        number=1,
-        enum=DeviceType,
+    publish_time_range: common.TimestampRange = proto.Field(
+        proto.MESSAGE,
+        number=12,
+        message=common.TimestampRange,
     )
-    id: str = proto.Field(
+    excluded_jobs: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
-        number=2,
+        number=13,
     )
 
 
-class CustomAttribute(proto.Message):
-    r"""Custom attribute values that are either filterable or
-    non-filterable.
+class LocationFilter(proto.Message):
+    r"""Geographic region of the search.
 
     Attributes:
-        string_values (MutableSequence[str]):
-            Exactly one of
-            [string_values][google.cloud.talent.v4beta1.CustomAttribute.string_values]
-            or
-            [long_values][google.cloud.talent.v4beta1.CustomAttribute.long_values]
-            must be specified.
-
-            This field is used to perform a string match
-            (``CASE_SENSITIVE_MATCH`` or ``CASE_INSENSITIVE_MATCH``)
-            search. For filterable ``string_value``\ s, a maximum total
-            number of 200 values is allowed, with each ``string_value``
-            has a byte size of no more than 500B. For unfilterable
-            ``string_values``, the maximum total byte size of
-            unfilterable ``string_values`` is 50KB.
-
-            Empty string isn't allowed.
-        long_values (MutableSequence[int]):
-            Exactly one of
-            [string_values][google.cloud.talent.v4beta1.CustomAttribute.string_values]
-            or
-            [long_values][google.cloud.talent.v4beta1.CustomAttribute.long_values]
-            must be specified.
-
-            This field is used to perform number range search. (``EQ``,
-            ``GT``, ``GE``, ``LE``, ``LT``) over filterable
-            ``long_value``.
-
-            Currently at most 1
-            [long_values][google.cloud.talent.v4beta1.CustomAttribute.long_values]
-            is supported.
-        filterable (bool):
-            If the ``filterable`` flag is true, the custom field values
-            may be used for custom attribute filters
-            [JobQuery.custom_attribute_filter][google.cloud.talent.v4beta1.JobQuery.custom_attribute_filter].
-            If false, these values may not be used for custom attribute
-            filters.
-
-            Default is false.
-        keyword_searchable (bool):
-            If the ``keyword_searchable`` flag is true, the keywords in
-            custom fields are searchable by keyword match. If false, the
-            values are not searchable by keyword match.
+        address (str):
+            The address name, such as "Mountain View" or
+            "Bay Area".
+        region_code (str):
+            CLDR region code of the country/region. This field may be
+            used in two ways:
+
+            1) If telecommute preference is not set, this field is used
+               address ambiguity of the user-input address. For example,
+               "Liverpool" may refer to "Liverpool, NY, US" or
+               "Liverpool, UK". This region code biases the address
+               resolution toward a specific country or territory. If
+               this field is not set, address resolution is biased
+               toward the United States by default.
+
+            2) If telecommute preference is set to TELECOMMUTE_ALLOWED,
+               the telecommute location filter will be limited to the
+               region specified in this field. If this field is not set,
+               the telecommute job locations will not be
 
-            Default is false.
-    """
+            See
+            https://unicode-org.github.io/cldr-staging/charts/latest/supplemental/territory_information.html
+            for details. Example: "CH" for Switzerland.
+        lat_lng (google.type.latlng_pb2.LatLng):
+            The latitude and longitude of the geographic center to
+            search from. This field is ignored if ``address`` is
+            provided.
+        distance_in_miles (float):
+            The distance_in_miles is applied when the location being
+            searched for is identified as a city or smaller. This field
+            is ignored if the location being searched for is a state or
+            larger.
+        telecommute_preference (google.cloud.talent_v4beta1.types.LocationFilter.TelecommutePreference):
+            Allows the client to return jobs without a set location,
+            specifically, telecommuting jobs (telecommuting is
+            considered by the service as a special location).
+            [Job.posting_region][google.cloud.talent.v4beta1.Job.posting_region]
+            indicates if a job permits telecommuting. If this field is
+            set to
+            [TelecommutePreference.TELECOMMUTE_ALLOWED][google.cloud.talent.v4beta1.LocationFilter.TelecommutePreference.TELECOMMUTE_ALLOWED],
+            telecommuting jobs are searched, and
+            [address][google.cloud.talent.v4beta1.LocationFilter.address]
+            and
+            [lat_lng][google.cloud.talent.v4beta1.LocationFilter.lat_lng]
+            are ignored. If not set or set to
+            [TelecommutePreference.TELECOMMUTE_EXCLUDED][google.cloud.talent.v4beta1.LocationFilter.TelecommutePreference.TELECOMMUTE_EXCLUDED],
+            the telecommute status of the jobs is ignored. Jobs that
+            have
+            [PostingRegion.TELECOMMUTE][google.cloud.talent.v4beta1.PostingRegion.TELECOMMUTE]
+            and have additional
+            [Job.addresses][google.cloud.talent.v4beta1.Job.addresses]
+            may still be matched based on other location filters using
+            [address][google.cloud.talent.v4beta1.LocationFilter.address]
+            or [latlng][].
+
+            This filter can be used by itself to search exclusively for
+            telecommuting jobs, or it can be combined with another
+            location filter to search for a combination of job
+            locations, such as "Mountain View" or "telecommuting" jobs.
+            However, when used in combination with other location
+            filters, telecommuting jobs can be treated as less relevant
+            than other jobs in the search response.
+
+            This field is only used for job search requests.
+        negated (bool):
+            Whether to apply negation to the filter so
+            profiles matching the filter are excluded.
+    """
+
+    class TelecommutePreference(proto.Enum):
+        r"""Specify whether to include telecommute jobs.
+
+        Values:
+            TELECOMMUTE_PREFERENCE_UNSPECIFIED (0):
+                Default value if the telecommute preference
+                isn't specified.
+            TELECOMMUTE_EXCLUDED (1):
+                Deprecated: Ignore telecommute status of jobs. Use
+                TELECOMMUTE_JOBS_EXCLUDED if want to exclude telecommute
+                jobs.
+            TELECOMMUTE_ALLOWED (2):
+                Allow telecommute jobs.
+            TELECOMMUTE_JOBS_EXCLUDED (3):
+                Exclude telecommute jobs.
+        """
+        TELECOMMUTE_PREFERENCE_UNSPECIFIED = 0
+        TELECOMMUTE_EXCLUDED = 1
+        TELECOMMUTE_ALLOWED = 2
+        TELECOMMUTE_JOBS_EXCLUDED = 3
 
-    string_values: MutableSequence[str] = proto.RepeatedField(
+    address: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    long_values: MutableSequence[int] = proto.RepeatedField(
-        proto.INT64,
+    region_code: str = proto.Field(
+        proto.STRING,
         number=2,
     )
-    filterable: bool = proto.Field(
-        proto.BOOL,
+    lat_lng: latlng_pb2.LatLng = proto.Field(
+        proto.MESSAGE,
         number=3,
+        message=latlng_pb2.LatLng,
     )
-    keyword_searchable: bool = proto.Field(
-        proto.BOOL,
+    distance_in_miles: float = proto.Field(
+        proto.DOUBLE,
         number=4,
     )
-
-
-class SpellingCorrection(proto.Message):
-    r"""Spell check result.
-
-    Attributes:
-        corrected (bool):
-            Indicates if the query was corrected by the
-            spell checker.
-        corrected_text (str):
-            Correction output consisting of the corrected
-            keyword string.
-        corrected_html (str):
-            Corrected output with html tags to highlight
-            the corrected words. Corrected words are called
-            out with the "<b><i>...</i></b>" html tags.
-            For example, the user input query is "software
-            enginear", where the second word, "enginear," is
-            incorrect. It should be "engineer". When
-            spelling correction is enabled, this value is
-            "software <b><i>engineer</i></b>".
-    """
-
-    corrected: bool = proto.Field(
-        proto.BOOL,
-        number=1,
-    )
-    corrected_text: str = proto.Field(
-        proto.STRING,
-        number=2,
+    telecommute_preference: TelecommutePreference = proto.Field(
+        proto.ENUM,
+        number=5,
+        enum=TelecommutePreference,
     )
-    corrected_html: str = proto.Field(
-        proto.STRING,
-        number=3,
+    negated: bool = proto.Field(
+        proto.BOOL,
+        number=6,
     )
 
 
-class CompensationInfo(proto.Message):
-    r"""Job compensation details.
+class CompensationFilter(proto.Message):
+    r"""Filter on job compensation type and amount.
 
     Attributes:
-        entries (MutableSequence[google.cloud.talent_v4beta1.types.CompensationInfo.CompensationEntry]):
-            Job compensation information.
-
-            At most one entry can be of type
-            [CompensationInfo.CompensationType.BASE][google.cloud.talent.v4beta1.CompensationInfo.CompensationType.BASE],
-            which is referred as **base compensation entry** for the
-            job.
-        annualized_base_compensation_range (google.cloud.talent_v4beta1.types.CompensationInfo.CompensationRange):
-            Output only. Annualized base compensation range. Computed as
-            base compensation entry's
-            [CompensationEntry.amount][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.amount]
-            times
-            [CompensationEntry.expected_units_per_year][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.expected_units_per_year].
-
-            See
-            [CompensationEntry][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry]
-            for explanation on compensation annualization.
-        annualized_total_compensation_range (google.cloud.talent_v4beta1.types.CompensationInfo.CompensationRange):
-            Output only. Annualized total compensation range. Computed
-            as all compensation entries'
-            [CompensationEntry.amount][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.amount]
-            times
-            [CompensationEntry.expected_units_per_year][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.expected_units_per_year].
-
-            See
-            [CompensationEntry][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry]
-            for explanation on compensation annualization.
-    """
-
-    class CompensationType(proto.Enum):
-        r"""The type of compensation.
-
-        For compensation amounts specified in non-monetary amounts, describe
-        the compensation scheme in the
-        [CompensationEntry.description][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.description].
-
-        For example, tipping format is described in
-        [CompensationEntry.description][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.description]
-        (for example, "expect 15-20% tips based on customer bill.") and an
-        estimate of the tips provided in
-        [CompensationEntry.amount][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.amount]
-        or
-        [CompensationEntry.range][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.range]
-        ($10 per hour).
-
-        For example, equity is described in
-        [CompensationEntry.description][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.description]
-        (for example, "1% - 2% equity vesting over 4 years, 1 year cliff")
-        and value estimated in
-        [CompensationEntry.amount][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.amount]
-        or
-        [CompensationEntry.range][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.range].
-        If no value estimate is possible, units are
-        [CompensationUnit.COMPENSATION_UNIT_UNSPECIFIED][google.cloud.talent.v4beta1.CompensationInfo.CompensationUnit.COMPENSATION_UNIT_UNSPECIFIED]
-        and then further clarified in
-        [CompensationEntry.description][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.description]
-        field.
-        """
-        COMPENSATION_TYPE_UNSPECIFIED = 0
-        BASE = 1
-        BONUS = 2
-        SIGNING_BONUS = 3
-        EQUITY = 4
-        PROFIT_SHARING = 5
-        COMMISSIONS = 6
-        TIPS = 7
-        OTHER_COMPENSATION_TYPE = 8
-
-    class CompensationUnit(proto.Enum):
-        r"""Pay frequency."""
-        COMPENSATION_UNIT_UNSPECIFIED = 0
-        HOURLY = 1
-        DAILY = 2
-        WEEKLY = 3
-        MONTHLY = 4
-        YEARLY = 5
-        ONE_TIME = 6
-        OTHER_COMPENSATION_UNIT = 7
-
-    class CompensationEntry(proto.Message):
-        r"""A compensation entry that represents one component of compensation,
-        such as base pay, bonus, or other compensation type.
-
-        Annualization: One compensation entry can be annualized if
-
-        -  it contains valid
-           [amount][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.amount]
-           or
-           [range][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.range].
-        -  and its
-           [expected_units_per_year][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.expected_units_per_year]
-           is set or can be derived. Its annualized range is determined as
-           ([amount][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.amount]
-           or
-           [range][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.range])
-           times
-           [expected_units_per_year][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.expected_units_per_year].
-
-        This message has `oneof`_ fields (mutually exclusive fields).
-        For each oneof, at most one member field can be set at the same time.
-        Setting any member of the oneof automatically clears all other
-        members.
-
-        .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
-
-        Attributes:
-            type_ (google.cloud.talent_v4beta1.types.CompensationInfo.CompensationType):
-                Compensation type.
-
-                Default is
-                [CompensationType.COMPENSATION_TYPE_UNSPECIFIED][google.cloud.talent.v4beta1.CompensationInfo.CompensationType.COMPENSATION_TYPE_UNSPECIFIED].
-            unit (google.cloud.talent_v4beta1.types.CompensationInfo.CompensationUnit):
-                Frequency of the specified amount.
-
-                Default is
-                [CompensationUnit.COMPENSATION_UNIT_UNSPECIFIED][google.cloud.talent.v4beta1.CompensationInfo.CompensationUnit.COMPENSATION_UNIT_UNSPECIFIED].
-            amount (google.type.money_pb2.Money):
-                Compensation amount.
-
-                This field is a member of `oneof`_ ``compensation_amount``.
-            range_ (google.cloud.talent_v4beta1.types.CompensationInfo.CompensationRange):
-                Compensation range.
-
-                This field is a member of `oneof`_ ``compensation_amount``.
-            description (str):
-                Compensation description.  For example, could
-                indicate equity terms or provide additional
-                context to an estimated bonus.
-            expected_units_per_year (google.protobuf.wrappers_pb2.DoubleValue):
-                Expected number of units paid each year. If not specified,
-                when
-                [Job.employment_types][google.cloud.talent.v4beta1.Job.employment_types]
-                is FULLTIME, a default value is inferred based on
-                [unit][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry.unit].
-                Default values:
-
-                -  HOURLY: 2080
-                -  DAILY: 260
-                -  WEEKLY: 52
-                -  MONTHLY: 12
-                -  ANNUAL: 1
-        """
-
-        type_: "CompensationInfo.CompensationType" = proto.Field(
-            proto.ENUM,
-            number=1,
-            enum="CompensationInfo.CompensationType",
-        )
-        unit: "CompensationInfo.CompensationUnit" = proto.Field(
-            proto.ENUM,
-            number=2,
-            enum="CompensationInfo.CompensationUnit",
-        )
-        amount: money_pb2.Money = proto.Field(
-            proto.MESSAGE,
-            number=3,
-            oneof="compensation_amount",
-            message=money_pb2.Money,
-        )
-        range_: "CompensationInfo.CompensationRange" = proto.Field(
-            proto.MESSAGE,
-            number=4,
-            oneof="compensation_amount",
-            message="CompensationInfo.CompensationRange",
-        )
-        description: str = proto.Field(
-            proto.STRING,
-            number=5,
-        )
-        expected_units_per_year: wrappers_pb2.DoubleValue = proto.Field(
-            proto.MESSAGE,
-            number=6,
-            message=wrappers_pb2.DoubleValue,
-        )
-
-    class CompensationRange(proto.Message):
-        r"""Compensation range.
-
-        Attributes:
-            max_compensation (google.type.money_pb2.Money):
-                The maximum amount of compensation. If left empty, the value
-                is set to a maximal compensation value and the currency code
-                is set to match the [currency
-                code][google.type.Money.currency_code] of min_compensation.
-            min_compensation (google.type.money_pb2.Money):
-                The minimum amount of compensation. If left empty, the value
-                is set to zero and the currency code is set to match the
-                [currency code][google.type.Money.currency_code] of
-                max_compensation.
+        type_ (google.cloud.talent_v4beta1.types.CompensationFilter.FilterType):
+            Required. Type of filter.
+        units (MutableSequence[google.cloud.talent_v4beta1.types.CompensationInfo.CompensationUnit]):
+            Required. Specify desired ``base compensation entry's``
+            [CompensationInfo.CompensationUnit][google.cloud.talent.v4beta1.CompensationInfo.CompensationUnit].
+        range_ (google.cloud.talent_v4beta1.types.CompensationInfo.CompensationRange):
+            Compensation range.
+        include_jobs_with_unspecified_compensation_range (bool):
+            If set to true, jobs with unspecified
+            compensation range fields are included.
+    """
+
+    class FilterType(proto.Enum):
+        r"""Specify the type of filtering.
+
+        Values:
+            FILTER_TYPE_UNSPECIFIED (0):
+                Filter type unspecified. Position holder,
+                INVALID, should never be used.
+            UNIT_ONLY (1):
+                Filter by ``base compensation entry's`` unit. A job is a
+                match if and only if the job contains a base
+                CompensationEntry and the base CompensationEntry's unit
+                matches provided
+                [units][google.cloud.talent.v4beta1.CompensationFilter.units].
+                Populate one or more
+                [units][google.cloud.talent.v4beta1.CompensationFilter.units].
+
+                See
+                [CompensationInfo.CompensationEntry][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry]
+                for definition of base compensation entry.
+            UNIT_AND_AMOUNT (2):
+                Filter by ``base compensation entry's`` unit and amount /
+                range. A job is a match if and only if the job contains a
+                base CompensationEntry, and the base entry's unit matches
+                provided
+                [CompensationUnit][google.cloud.talent.v4beta1.CompensationInfo.CompensationUnit]
+                and amount or range overlaps with provided
+                [CompensationRange][google.cloud.talent.v4beta1.CompensationInfo.CompensationRange].
+
+                See
+                [CompensationInfo.CompensationEntry][google.cloud.talent.v4beta1.CompensationInfo.CompensationEntry]
+                for definition of base compensation entry.
+
+                Set exactly one
+                [units][google.cloud.talent.v4beta1.CompensationFilter.units]
+                and populate
+                [range][google.cloud.talent.v4beta1.CompensationFilter.range].
+            ANNUALIZED_BASE_AMOUNT (3):
+                Filter by annualized base compensation amount and
+                ``base compensation entry's`` unit. Populate
+                [range][google.cloud.talent.v4beta1.CompensationFilter.range]
+                and zero or more
+                [units][google.cloud.talent.v4beta1.CompensationFilter.units].
+            ANNUALIZED_TOTAL_AMOUNT (4):
+                Filter by annualized total compensation amount and
+                ``base compensation entry's`` unit . Populate
+                [range][google.cloud.talent.v4beta1.CompensationFilter.range]
+                and zero or more
+                [units][google.cloud.talent.v4beta1.CompensationFilter.units].
         """
+        FILTER_TYPE_UNSPECIFIED = 0
+        UNIT_ONLY = 1
+        UNIT_AND_AMOUNT = 2
+        ANNUALIZED_BASE_AMOUNT = 3
+        ANNUALIZED_TOTAL_AMOUNT = 4
 
-        max_compensation: money_pb2.Money = proto.Field(
-            proto.MESSAGE,
-            number=2,
-            message=money_pb2.Money,
-        )
-        min_compensation: money_pb2.Money = proto.Field(
-            proto.MESSAGE,
-            number=1,
-            message=money_pb2.Money,
-        )
-
-    entries: MutableSequence[CompensationEntry] = proto.RepeatedField(
-        proto.MESSAGE,
+    type_: FilterType = proto.Field(
+        proto.ENUM,
         number=1,
-        message=CompensationEntry,
+        enum=FilterType,
     )
-    annualized_base_compensation_range: CompensationRange = proto.Field(
-        proto.MESSAGE,
+    units: MutableSequence[
+        common.CompensationInfo.CompensationUnit
+    ] = proto.RepeatedField(
+        proto.ENUM,
         number=2,
-        message=CompensationRange,
+        enum=common.CompensationInfo.CompensationUnit,
     )
-    annualized_total_compensation_range: CompensationRange = proto.Field(
+    range_: common.CompensationInfo.CompensationRange = proto.Field(
         proto.MESSAGE,
         number=3,
-        message=CompensationRange,
+        message=common.CompensationInfo.CompensationRange,
+    )
+    include_jobs_with_unspecified_compensation_range: bool = proto.Field(
+        proto.BOOL,
+        number=4,
     )
 
 
-class BatchOperationMetadata(proto.Message):
-    r"""Metadata used for long running operations returned by CTS batch
-    APIs. It's used to replace
-    [google.longrunning.Operation.metadata][google.longrunning.Operation.metadata].
+class CommuteFilter(proto.Message):
+    r"""Parameters needed for commute search.
 
-    Attributes:
-        state (google.cloud.talent_v4beta1.types.BatchOperationMetadata.State):
-            The state of a long running operation.
-        state_description (str):
-            More detailed information about operation
-            state.
-        success_count (int):
-            Count of successful item(s) inside an
-            operation.
-        failure_count (int):
-            Count of failed item(s) inside an operation.
-        total_count (int):
-            Count of total item(s) inside an operation.
-        create_time (google.protobuf.timestamp_pb2.Timestamp):
-            The time when the batch operation is created.
-        update_time (google.protobuf.timestamp_pb2.Timestamp):
-            The time when the batch operation status is updated. The
-            metadata and the
-            [update_time][google.cloud.talent.v4beta1.BatchOperationMetadata.update_time]
-            is refreshed every minute otherwise cached data is returned.
-        end_time (google.protobuf.timestamp_pb2.Timestamp):
-            The time when the batch operation is finished and
-            [google.longrunning.Operation.done][google.longrunning.Operation.done]
-            is set to ``true``.
-    """
+    This message has `oneof`_ fields (mutually exclusive fields).
+    For each oneof, at most one member field can be set at the same time.
+    Setting any member of the oneof automatically clears all other
+    members.
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
-    class State(proto.Enum):
-        r""""""
-        STATE_UNSPECIFIED = 0
-        INITIALIZING = 1
-        PROCESSING = 2
-        SUCCEEDED = 3
-        FAILED = 4
-        CANCELLING = 5
-        CANCELLED = 6
+    Attributes:
+        commute_method (google.cloud.talent_v4beta1.types.CommuteMethod):
+            Required. The method of transportation to
+            calculate the commute time for.
+        start_coordinates (google.type.latlng_pb2.LatLng):
+            Required. The latitude and longitude of the
+            location to calculate the commute time from.
+        travel_duration (google.protobuf.duration_pb2.Duration):
+            Required. The maximum travel time in seconds. The maximum
+            allowed value is ``3600s`` (one hour). Format is ``123s``.
+        allow_imprecise_addresses (bool):
+            If ``true``, jobs without street level addresses may also be
+            returned. For city level addresses, the city center is used.
+            For state and coarser level addresses, text matching is
+            used. If this field is set to ``false`` or isn't specified,
+            only jobs that include street level addresses will be
+            returned by commute search.
+        road_traffic (google.cloud.talent_v4beta1.types.CommuteFilter.RoadTraffic):
+            Specifies the traffic density to use when
+            calculating commute time.
+
+            This field is a member of `oneof`_ ``traffic_option``.
+        departure_time (google.type.timeofday_pb2.TimeOfDay):
+            The departure time used to calculate traffic impact,
+            represented as
+            [google.type.TimeOfDay][google.type.TimeOfDay] in local time
+            zone.
+
+            Currently traffic model is restricted to hour level
+            resolution.
+
+            This field is a member of `oneof`_ ``traffic_option``.
+    """
+
+    class RoadTraffic(proto.Enum):
+        r"""The traffic density to use when calculating commute time.
+
+        Values:
+            ROAD_TRAFFIC_UNSPECIFIED (0):
+                Road traffic situation isn't specified.
+            TRAFFIC_FREE (1):
+                Optimal commute time without considering any
+                traffic impact.
+            BUSY_HOUR (2):
+                Commute time calculation takes in account the
+                peak traffic impact.
+        """
+        ROAD_TRAFFIC_UNSPECIFIED = 0
+        TRAFFIC_FREE = 1
+        BUSY_HOUR = 2
 
-    state: State = proto.Field(
+    commute_method: common.CommuteMethod = proto.Field(
         proto.ENUM,
         number=1,
-        enum=State,
+        enum=common.CommuteMethod,
     )
-    state_description: str = proto.Field(
-        proto.STRING,
+    start_coordinates: latlng_pb2.LatLng = proto.Field(
+        proto.MESSAGE,
         number=2,
+        message=latlng_pb2.LatLng,
     )
-    success_count: int = proto.Field(
-        proto.INT32,
+    travel_duration: duration_pb2.Duration = proto.Field(
+        proto.MESSAGE,
         number=3,
+        message=duration_pb2.Duration,
     )
-    failure_count: int = proto.Field(
-        proto.INT32,
+    allow_imprecise_addresses: bool = proto.Field(
+        proto.BOOL,
         number=4,
     )
-    total_count: int = proto.Field(
-        proto.INT32,
+    road_traffic: RoadTraffic = proto.Field(
+        proto.ENUM,
         number=5,
+        oneof="traffic_option",
+        enum=RoadTraffic,
     )
-    create_time: timestamp_pb2.Timestamp = proto.Field(
+    departure_time: timeofday_pb2.TimeOfDay = proto.Field(
         proto.MESSAGE,
         number=6,
-        message=timestamp_pb2.Timestamp,
-    )
-    update_time: timestamp_pb2.Timestamp = proto.Field(
-        proto.MESSAGE,
-        number=7,
-        message=timestamp_pb2.Timestamp,
-    )
-    end_time: timestamp_pb2.Timestamp = proto.Field(
-        proto.MESSAGE,
-        number=8,
-        message=timestamp_pb2.Timestamp,
+        oneof="traffic_option",
+        message=timeofday_pb2.TimeOfDay,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/company.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/company.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/company_service.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/company_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/completion_service.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/completion_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -69,21 +69,64 @@
             [CompletionScope.PUBLIC][google.cloud.talent.v4beta1.CompleteQueryRequest.CompletionScope.PUBLIC].
         type_ (google.cloud.talent_v4beta1.types.CompleteQueryRequest.CompletionType):
             The completion topic. The default is
             [CompletionType.COMBINED][google.cloud.talent.v4beta1.CompleteQueryRequest.CompletionType.COMBINED].
     """
 
     class CompletionScope(proto.Enum):
-        r"""Enum to specify the scope of completion."""
+        r"""Enum to specify the scope of completion.
+
+        Values:
+            COMPLETION_SCOPE_UNSPECIFIED (0):
+                Default value.
+            TENANT (1):
+                Suggestions are based only on the data
+                provided by the client.
+            PUBLIC (2):
+                Suggestions are based on all jobs data in the
+                system that's visible to the client
+        """
         COMPLETION_SCOPE_UNSPECIFIED = 0
         TENANT = 1
         PUBLIC = 2
 
     class CompletionType(proto.Enum):
-        r"""Enum to specify auto-completion topics."""
+        r"""Enum to specify auto-completion topics.
+
+        Values:
+            COMPLETION_TYPE_UNSPECIFIED (0):
+                Default value.
+            JOB_TITLE (1):
+                Suggest job titles for jobs autocomplete.
+
+                For
+                [CompletionType.JOB_TITLE][google.cloud.talent.v4beta1.CompleteQueryRequest.CompletionType.JOB_TITLE]
+                type, only open jobs with the same
+                [language_codes][google.cloud.talent.v4beta1.CompleteQueryRequest.language_codes]
+                are returned.
+            COMPANY_NAME (2):
+                Suggest company names for jobs autocomplete.
+
+                For
+                [CompletionType.COMPANY_NAME][google.cloud.talent.v4beta1.CompleteQueryRequest.CompletionType.COMPANY_NAME]
+                type, only companies having open jobs with the same
+                [language_codes][google.cloud.talent.v4beta1.CompleteQueryRequest.language_codes]
+                are returned.
+            COMBINED (3):
+                Suggest both job titles and company names for jobs
+                autocomplete.
+
+                For
+                [CompletionType.COMBINED][google.cloud.talent.v4beta1.CompleteQueryRequest.CompletionType.COMBINED]
+                type, only open jobs with the same
+                [language_codes][google.cloud.talent.v4beta1.CompleteQueryRequest.language_codes]
+                or companies having open jobs with the same
+                [language_codes][google.cloud.talent.v4beta1.CompleteQueryRequest.language_codes]
+                are returned.
+        """
         COMPLETION_TYPE_UNSPECIFIED = 0
         JOB_TITLE = 1
         COMPANY_NAME = 2
         COMBINED = 3
 
     parent: str = proto.Field(
         proto.STRING,
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/event_service.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/histogram.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/histogram.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/job_service.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/job_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,45 @@
 
 class JobView(proto.Enum):
     r"""An enum that specifies the job attributes that are returned in the
     [MatchingJob.job][google.cloud.talent.v4beta1.SearchJobsResponse.MatchingJob.job]
     or
     [ListJobsResponse.jobs][google.cloud.talent.v4beta1.ListJobsResponse.jobs]
     fields.
+
+    Values:
+        JOB_VIEW_UNSPECIFIED (0):
+            Default value.
+        JOB_VIEW_ID_ONLY (1):
+            A ID only view of job, with following attributes:
+            [Job.name][google.cloud.talent.v4beta1.Job.name],
+            [Job.requisition_id][google.cloud.talent.v4beta1.Job.requisition_id],
+            [Job.language_code][google.cloud.talent.v4beta1.Job.language_code].
+        JOB_VIEW_MINIMAL (2):
+            A minimal view of the job, with the following attributes:
+            [Job.name][google.cloud.talent.v4beta1.Job.name],
+            [Job.requisition_id][google.cloud.talent.v4beta1.Job.requisition_id],
+            [Job.title][google.cloud.talent.v4beta1.Job.title],
+            [Job.company][google.cloud.talent.v4beta1.Job.company],
+            [Job.DerivedInfo.locations][google.cloud.talent.v4beta1.Job.DerivedInfo.locations],
+            [Job.language_code][google.cloud.talent.v4beta1.Job.language_code].
+        JOB_VIEW_SMALL (3):
+            A small view of the job, with the following attributes in
+            the search results:
+            [Job.name][google.cloud.talent.v4beta1.Job.name],
+            [Job.requisition_id][google.cloud.talent.v4beta1.Job.requisition_id],
+            [Job.title][google.cloud.talent.v4beta1.Job.title],
+            [Job.company][google.cloud.talent.v4beta1.Job.company],
+            [Job.DerivedInfo.locations][google.cloud.talent.v4beta1.Job.DerivedInfo.locations],
+            [Job.visibility][google.cloud.talent.v4beta1.Job.visibility],
+            [Job.language_code][google.cloud.talent.v4beta1.Job.language_code],
+            [Job.description][google.cloud.talent.v4beta1.Job.description].
+        JOB_VIEW_FULL (4):
+            All available attributes are included in the
+            search results.
     """
     JOB_VIEW_UNSPECIFIED = 0
     JOB_VIEW_ID_ONLY = 1
     JOB_VIEW_MINIMAL = 2
     JOB_VIEW_SMALL = 3
     JOB_VIEW_FULL = 4
 
@@ -615,27 +646,64 @@
             [KeywordMatchMode.KEYWORD_MATCH_ALL][google.cloud.talent.v4beta1.SearchJobsRequest.KeywordMatchMode.KEYWORD_MATCH_ALL]
             if no value is specified.
     """
 
     class SearchMode(proto.Enum):
         r"""A string-represented enumeration of the job search mode. The
         service operate differently for different modes of service.
+
+        Values:
+            SEARCH_MODE_UNSPECIFIED (0):
+                The mode of the search method isn't specified. The default
+                search behavior is identical to JOB_SEARCH search behavior.
+            JOB_SEARCH (1):
+                The job search matches against all jobs, and
+                featured jobs (jobs with promotionValue > 0) are
+                not specially handled.
+            FEATURED_JOB_SEARCH (2):
+                The job search matches only against featured
+                jobs (jobs with a promotionValue > 0). This
+                method doesn't return any jobs having a
+                promotionValue <= 0. The search results order is
+                determined by the promotionValue (jobs with a
+                higher promotionValue are returned higher up in
+                the search results), with relevance being used
+                as a tiebreaker.
         """
         SEARCH_MODE_UNSPECIFIED = 0
         JOB_SEARCH = 1
         FEATURED_JOB_SEARCH = 2
 
     class DiversificationLevel(proto.Enum):
         r"""Controls whether highly similar jobs are returned next to
         each other in the search results. Jobs are identified as highly
         similar based on their titles, job categories, and locations.
         Highly similar results are clustered so that only one
         representative job of the cluster is displayed to the job seeker
         higher up in the results, with the other jobs being displayed
         lower down in the results.
+
+        Values:
+            DIVERSIFICATION_LEVEL_UNSPECIFIED (0):
+                The diversification level isn't specified.
+            DISABLED (1):
+                Disables diversification. Jobs that would
+                normally be pushed to the last page would not
+                have their positions altered. This may result in
+                highly similar jobs appearing in sequence in the
+                search results.
+            SIMPLE (2):
+                Default diversifying behavior. The result
+                list is ordered so that highly similar results
+                are pushed to the end of the last page of search
+                results. If you are using pageToken to page
+                through the result set, latency might be lower
+                but we can't guarantee that all results are
+                returned. If you are using page offset, latency
+                might be higher but all results are returned.
         """
         DIVERSIFICATION_LEVEL_UNSPECIFIED = 0
         DISABLED = 1
         SIMPLE = 2
 
     class KeywordMatchMode(proto.Enum):
         r"""Controls what keyword matching behavior the search has. When keyword
@@ -651,14 +719,35 @@
         regardless of this enum's value.
 
         Use
         [Company.keyword_searchable_job_custom_attributes][google.cloud.talent.v4beta1.Company.keyword_searchable_job_custom_attributes]
         if company-specific globally matched custom field/attribute string
         values are needed. Enabling keyword match improves recall of
         subsequent search requests.
+
+        Values:
+            KEYWORD_MATCH_MODE_UNSPECIFIED (0):
+                The keyword match option isn't specified. Defaults to
+                [KeywordMatchMode.KEYWORD_MATCH_ALL][google.cloud.talent.v4beta1.SearchJobsRequest.KeywordMatchMode.KEYWORD_MATCH_ALL]
+                behavior.
+            KEYWORD_MATCH_DISABLED (1):
+                Disables keyword matching.
+            KEYWORD_MATCH_ALL (2):
+                Enable keyword matching over
+                [Job.title][google.cloud.talent.v4beta1.Job.title],
+                [Job.description][google.cloud.talent.v4beta1.Job.description],
+                [Job.company_display_name][google.cloud.talent.v4beta1.Job.company_display_name],
+                [Job.addresses][google.cloud.talent.v4beta1.Job.addresses],
+                [Job.qualifications][google.cloud.talent.v4beta1.Job.qualifications],
+                and keyword searchable
+                [Job.custom_attributes][google.cloud.talent.v4beta1.Job.custom_attributes]
+                fields.
+            KEYWORD_MATCH_TITLE_ONLY (3):
+                Only enable keyword matching over
+                [Job.title][google.cloud.talent.v4beta1.Job.title].
         """
         KEYWORD_MATCH_MODE_UNSPECIFIED = 0
         KEYWORD_MATCH_DISABLED = 1
         KEYWORD_MATCH_ALL = 2
         KEYWORD_MATCH_TITLE_ONLY = 3
 
     class CustomRankingInfo(proto.Message):
@@ -699,14 +788,49 @@
                 Sample ranking expression (year + 25) \* 0.25 - (freshness /
                 0.5)
         """
 
         class ImportanceLevel(proto.Enum):
             r"""The importance level for
             [CustomRankingInfo.ranking_expression][google.cloud.talent.v4beta1.SearchJobsRequest.CustomRankingInfo.ranking_expression].
+
+            Values:
+                IMPORTANCE_LEVEL_UNSPECIFIED (0):
+                    Default value if the importance level isn't
+                    specified.
+                NONE (1):
+                    The given ranking expression is of None
+                    importance, existing relevance score (determined
+                    by API algorithm) dominates job's final ranking
+                    position.
+                LOW (2):
+                    The given ranking expression is of Low
+                    importance in terms of job's final ranking
+                    position compared to existing relevance score
+                    (determined by API algorithm).
+                MILD (3):
+                    The given ranking expression is of Mild
+                    importance in terms of job's final ranking
+                    position compared to existing relevance score
+                    (determined by API algorithm).
+                MEDIUM (4):
+                    The given ranking expression is of Medium
+                    importance in terms of job's final ranking
+                    position compared to existing relevance score
+                    (determined by API algorithm).
+                HIGH (5):
+                    The given ranking expression is of High
+                    importance in terms of job's final ranking
+                    position compared to existing relevance score
+                    (determined by API algorithm).
+                EXTREME (6):
+                    The given ranking expression is of Extreme
+                    importance, and dominates job's final ranking
+                    position with existing relevance score
+                    (determined by API algorithm) ignored.
             """
             IMPORTANCE_LEVEL_UNSPECIFIED = 0
             NONE = 1
             LOW = 2
             MILD = 3
             MEDIUM = 4
             HIGH = 5
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/tenant.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/tenant.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
             service when a tenant is created.
 
             The format is "projects/{project_id}/tenants/{tenant_id}",
             for example, "projects/foo/tenants/bar".
         external_id (str):
             Required. Client side tenant identifier, used
             to uniquely identify the tenant.
+
             The maximum number of allowed characters is 255.
         usage_type (google.cloud.talent_v4beta1.types.Tenant.DataUsageType):
             Indicates whether data owned by this tenant may be used to
             provide product improvements across other tenants.
 
             Defaults behavior is
             [DataUsageType.ISOLATED][google.cloud.talent.v4beta1.Tenant.DataUsageType.ISOLATED]
@@ -62,14 +63,25 @@
             brackets and special symbols are not searchable as-is, and
             must be surrounded by quotes.
     """
 
     class DataUsageType(proto.Enum):
         r"""Enum that represents how user data owned by the tenant is
         used.
+
+        Values:
+            DATA_USAGE_TYPE_UNSPECIFIED (0):
+                Default value.
+            AGGREGATED (1):
+                Data owned by this tenant is used to improve
+                search/recommendation quality across tenants.
+            ISOLATED (2):
+                Data owned by this tenant is used to improve
+                search/recommendation quality for this tenant
+                only.
         """
         DATA_USAGE_TYPE_UNSPECIFIED = 0
         AGGREGATED = 1
         ISOLATED = 2
 
     name: str = proto.Field(
         proto.STRING,
```

### Comparing `google-cloud-talent-2.9.0/google/cloud/talent_v4beta1/types/tenant_service.py` & `google-cloud-talent-2.9.1/google/cloud/talent_v4beta1/types/tenant_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/google_cloud_talent.egg-info/PKG-INFO` & `google-cloud-talent-2.9.1/google_cloud_talent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-talent
-Version: 2.9.0
+Version: 2.9.1
 Summary: Google Cloud Talent API client library
 Home-page: https://github.com/googleapis/python-talent
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-talent-2.9.0/google_cloud_talent.egg-info/SOURCES.txt` & `google-cloud-talent-2.9.1/google_cloud_talent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/setup.py` & `google-cloud-talent-2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/__init__.py` & `google-cloud-talent-2.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/unit/__init__.py` & `google-cloud-talent-2.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/unit/gapic/__init__.py` & `google-cloud-talent-2.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4/__init__.py` & `google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4/test_company_service.py` & `google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4/test_company_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4/test_completion.py` & `google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4/test_completion.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4/test_event_service.py` & `google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4/test_event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4/test_job_service.py` & `google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4/test_job_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4/test_tenant_service.py` & `google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4/test_tenant_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4beta1/__init__.py` & `google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4beta1/test_company_service.py` & `google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4beta1/test_company_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4beta1/test_completion.py` & `google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4beta1/test_completion.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4beta1/test_event_service.py` & `google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4beta1/test_event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4beta1/test_job_service.py` & `google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4beta1/test_job_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-talent-2.9.0/tests/unit/gapic/talent_v4beta1/test_tenant_service.py` & `google-cloud-talent-2.9.1/tests/unit/gapic/talent_v4beta1/test_tenant_service.py`

 * *Files identical despite different names*

