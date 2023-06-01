# Comparing `tmp/google-cloud-speech-2.9.2.tar.gz` & `tmp/google-cloud-speech-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-speech-2.9.2.tar", last modified: Tue Jan 18 16:08:28 2022, max compression
+gzip compressed data, was "dist/google-cloud-speech-2.9.3.tar", last modified: Tue Oct  5 10:38:09 2021, max compression
```

## Comparing `google-cloud-speech-2.9.2.tar` & `google-cloud-speech-2.9.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.814717 google-cloud-speech-2.9.2/
--rw-rw-r--   0 root         (0)     1003    11358 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     3726 2022-01-18 16:08:28.814717 google-cloud-speech-2.9.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2913 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.798709 google-cloud-speech-2.9.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.802711 google-cloud-speech-2.9.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.802711 google-cloud-speech-2.9.2/google/cloud/speech/
--rw-rw-r--   0 root         (0)     1003     2704 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech/__init__.py
--rw-rw-r--   0 root         (0)     1003       80 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.802711 google-cloud-speech-2.9.2/google/cloud/speech_v1/
--rw-rw-r--   0 root         (0)     1003     2412 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1283 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003     4114 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1/helpers.py
--rw-rw-r--   0 root         (0)     1003       80 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.802711 google-cloud-speech-2.9.2/google/cloud/speech_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.806713 google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/
--rw-rw-r--   0 root         (0)     1003      737 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/__init__.py
--rw-rw-r--   0 root         (0)     1003    20565 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/async_client.py
--rw-rw-r--   0 root         (0)     1003    27467 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.806713 google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/transports/
--rw-rw-r--   0 root         (0)     1003     1122 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8877 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14862 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15257 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.806713 google-cloud-speech-2.9.2/google/cloud/speech_v1/types/
--rw-rw-r--   0 root         (0)     1003     1675 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    38679 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1/types/cloud_speech.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.806713 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/
--rw-rw-r--   0 root         (0)     1003     3996 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4123 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       80 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.806713 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.806713 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/
--rw-rw-r--   0 root         (0)     1003      753 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/__init__.py
--rw-rw-r--   0 root         (0)     1003    41436 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/async_client.py
--rw-rw-r--   0 root         (0)     1003    52211 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/client.py
--rw-rw-r--   0 root         (0)     1003    11321 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.806713 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/transports/
--rw-rw-r--   0 root         (0)     1003     1158 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10753 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/transports/base.py
--rw-rw-r--   0 root         (0)     1003    21909 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22482 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.810715 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/
--rw-rw-r--   0 root         (0)     1003      737 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/__init__.py
--rw-rw-r--   0 root         (0)     1003    20934 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/async_client.py
--rw-rw-r--   0 root         (0)     1003    28906 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.810715 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/transports/
--rw-rw-r--   0 root         (0)     1003     1122 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8884 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14890 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15285 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.810715 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/types/
--rw-rw-r--   0 root         (0)     1003     2620 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    46161 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/types/cloud_speech.py
--rw-rw-r--   0 root         (0)     1003     9805 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/types/cloud_speech_adaptation.py
--rw-rw-r--   0 root         (0)     1003     8487 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/types/resource.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.810715 google-cloud-speech-2.9.2/google_cloud_speech.egg-info/
--rw-r--r--   0 root         (0)     1003     3726 2022-01-18 16:08:28.000000 google-cloud-speech-2.9.2/google_cloud_speech.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2981 2022-01-18 16:08:28.000000 google-cloud-speech-2.9.2/google_cloud_speech.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-01-18 16:08:28.000000 google-cloud-speech-2.9.2/google_cloud_speech.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-01-18 16:08:28.000000 google-cloud-speech-2.9.2/google_cloud_speech.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-01-18 16:08:28.000000 google-cloud-speech-2.9.2/google_cloud_speech.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003       88 2022-01-18 16:08:28.000000 google-cloud-speech-2.9.2/google_cloud_speech.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-01-18 16:08:28.000000 google-cloud-speech-2.9.2/google_cloud_speech.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.810715 google-cloud-speech-2.9.2/scripts/
--rw-rw-r--   0 root         (0)     1003     6088 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/scripts/fixup_speech_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003     6672 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/scripts/fixup_speech_v1p1beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-01-18 16:08:28.814717 google-cloud-speech-2.9.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2975 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.810715 google-cloud-speech-2.9.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.802711 google-cloud-speech-2.9.2/tests/system/
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.802711 google-cloud-speech-2.9.2/tests/system/gapic/
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.810715 google-cloud-speech-2.9.2/tests/system/gapic/v1/
--rw-rw-r--   0 root         (0)     1003     2963 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/tests/system/gapic/v1/test_system_speech_v1.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.814717 google-cloud-speech-2.9.2/tests/system/gapic/v1p1beta1/
--rw-rw-r--   0 root         (0)     1003     3076 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/tests/system/gapic/v1p1beta1/test_system_speech_v1p1beta1.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.814717 google-cloud-speech-2.9.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.814717 google-cloud-speech-2.9.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.814717 google-cloud-speech-2.9.2/tests/unit/gapic/speech_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/tests/unit/gapic/speech_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    56131 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/tests/unit/gapic/speech_v1/test_speech.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-01-18 16:08:28.814717 google-cloud-speech-2.9.2/tests/unit/gapic/speech_v1p1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/tests/unit/gapic/speech_v1p1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   136555 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/tests/unit/gapic/speech_v1p1beta1/test_adaptation.py
--rw-rw-r--   0 root         (0)     1003    57776 2022-01-18 16:05:50.000000 google-cloud-speech-2.9.2/tests/unit/gapic/speech_v1p1beta1/test_speech.py
--rw-rw-r--   0 root         (0)     1003     1793 2022-01-18 16:05:49.000000 google-cloud-speech-2.9.2/tests/unit/test_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.344425 google-cloud-speech-2.9.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     3726 2021-10-05 10:38:09.344425 google-cloud-speech-2.9.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2913 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.332425 google-cloud-speech-2.9.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.332425 google-cloud-speech-2.9.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.336425 google-cloud-speech-2.9.3/google/cloud/speech/
+-rw-rw-r--   0 root         (0)     1003     2704 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech/__init__.py
+-rw-rw-r--   0 root         (0)     1003       80 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.336425 google-cloud-speech-2.9.3/google/cloud/speech_v1/
+-rw-rw-r--   0 root         (0)     1003     2412 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1283 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003     4114 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1/helpers.py
+-rw-rw-r--   0 root         (0)     1003       80 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.336425 google-cloud-speech-2.9.3/google/cloud/speech_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.336425 google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/
+-rw-rw-r--   0 root         (0)     1003      737 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20565 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27467 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.336425 google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/transports/
+-rw-rw-r--   0 root         (0)     1003     1122 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8877 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14862 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15257 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.336425 google-cloud-speech-2.9.3/google/cloud/speech_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1675 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38679 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1/types/cloud_speech.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.336425 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003     3996 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4123 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       80 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.340425 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.340425 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/
+-rw-rw-r--   0 root         (0)     1003      753 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41436 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/async_client.py
+-rw-rw-r--   0 root         (0)     1003    52211 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/client.py
+-rw-rw-r--   0 root         (0)     1003    11321 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.340425 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/transports/
+-rw-rw-r--   0 root         (0)     1003     1158 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10753 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    21909 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22482 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.340425 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/
+-rw-rw-r--   0 root         (0)     1003      737 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20934 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28906 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.340425 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/transports/
+-rw-rw-r--   0 root         (0)     1003     1122 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8884 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14890 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15285 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.340425 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2620 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    46161 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/types/cloud_speech.py
+-rw-rw-r--   0 root         (0)     1003     9805 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/types/cloud_speech_adaptation.py
+-rw-rw-r--   0 root         (0)     1003     8487 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/types/resource.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.344425 google-cloud-speech-2.9.3/google_cloud_speech.egg-info/
+-rw-r--r--   0 root         (0)     1003     3726 2021-10-05 10:38:09.000000 google-cloud-speech-2.9.3/google_cloud_speech.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2981 2021-10-05 10:38:09.000000 google-cloud-speech-2.9.3/google_cloud_speech.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2021-10-05 10:38:09.000000 google-cloud-speech-2.9.3/google_cloud_speech.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2021-10-05 10:38:09.000000 google-cloud-speech-2.9.3/google_cloud_speech.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2021-10-05 10:38:09.000000 google-cloud-speech-2.9.3/google_cloud_speech.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003       88 2021-10-05 10:38:09.000000 google-cloud-speech-2.9.3/google_cloud_speech.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2021-10-05 10:38:09.000000 google-cloud-speech-2.9.3/google_cloud_speech.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.344425 google-cloud-speech-2.9.3/scripts/
+-rw-rw-r--   0 root         (0)     1003     6088 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/scripts/fixup_speech_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003     6672 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/scripts/fixup_speech_v1p1beta1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2021-10-05 10:38:09.344425 google-cloud-speech-2.9.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2975 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.344425 google-cloud-speech-2.9.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.332425 google-cloud-speech-2.9.3/tests/system/
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.332425 google-cloud-speech-2.9.3/tests/system/gapic/
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.344425 google-cloud-speech-2.9.3/tests/system/gapic/v1/
+-rw-rw-r--   0 root         (0)     1003     2963 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/tests/system/gapic/v1/test_system_speech_v1.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.344425 google-cloud-speech-2.9.3/tests/system/gapic/v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003     3076 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/tests/system/gapic/v1p1beta1/test_system_speech_v1p1beta1.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.344425 google-cloud-speech-2.9.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.344425 google-cloud-speech-2.9.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.344425 google-cloud-speech-2.9.3/tests/unit/gapic/speech_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/tests/unit/gapic/speech_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    56131 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/tests/unit/gapic/speech_v1/test_speech.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:38:09.344425 google-cloud-speech-2.9.3/tests/unit/gapic/speech_v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/tests/unit/gapic/speech_v1p1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   136555 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/tests/unit/gapic/speech_v1p1beta1/test_adaptation.py
+-rw-rw-r--   0 root         (0)     1003    57776 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/tests/unit/gapic/speech_v1p1beta1/test_speech.py
+-rw-rw-r--   0 root         (0)     1003     1793 2021-10-05 10:35:35.000000 google-cloud-speech-2.9.3/tests/unit/test_helpers.py
```

### Comparing `google-cloud-speech-2.9.2/LICENSE` & `google-cloud-speech-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/MANIFEST.in` & `google-cloud-speech-2.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/PKG-INFO` & `google-cloud-speech-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-speech
-Version: 2.9.2
+Version: 2.9.3
 Summary: Google Cloud Speech API client library
 Home-page: https://github.com/googleapis/python-speech
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-speech-2.9.2/README.rst` & `google-cloud-speech-2.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech/__init__.py` & `google-cloud-speech-2.9.3/google/cloud/speech/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1/__init__.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1/gapic_metadata.json` & `google-cloud-speech-2.9.3/google/cloud/speech_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1/helpers.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1/helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1/services/__init__.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/__init__.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/async_client.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/client.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/transports/__init__.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/transports/base.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/transports/grpc.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1/services/speech/transports/grpc_asyncio.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1/services/speech/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1/types/__init__.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1/types/cloud_speech.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1/types/cloud_speech.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/__init__.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/gapic_metadata.json` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/__init__.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/__init__.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/async_client.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/client.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/pagers.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/transports/__init__.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/transports/base.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/transports/grpc.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/adaptation/transports/grpc_asyncio.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/adaptation/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/__init__.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/async_client.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/client.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/transports/__init__.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/transports/base.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/transports/grpc.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/services/speech/transports/grpc_asyncio.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/services/speech/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/types/__init__.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/types/cloud_speech.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/types/cloud_speech.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/types/cloud_speech_adaptation.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/types/cloud_speech_adaptation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google/cloud/speech_v1p1beta1/types/resource.py` & `google-cloud-speech-2.9.3/google/cloud/speech_v1p1beta1/types/resource.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/google_cloud_speech.egg-info/PKG-INFO` & `google-cloud-speech-2.9.3/google_cloud_speech.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-speech
-Version: 2.9.2
+Version: 2.9.3
 Summary: Google Cloud Speech API client library
 Home-page: https://github.com/googleapis/python-speech
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-speech-2.9.2/google_cloud_speech.egg-info/SOURCES.txt` & `google-cloud-speech-2.9.3/google_cloud_speech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/scripts/fixup_speech_v1_keywords.py` & `google-cloud-speech-2.9.3/scripts/fixup_speech_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/scripts/fixup_speech_v1p1beta1_keywords.py` & `google-cloud-speech-2.9.3/scripts/fixup_speech_v1p1beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/setup.py` & `google-cloud-speech-2.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import setuptools
 
 
 # Package metadata.
 
 name = "google-cloud-speech"
 description = "Google Cloud Speech API client library"
-version = "2.9.2"
+version = "2.9.3"
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     # NOTE: Maintainers, please do not require google-api-core>=2.x.x
```

### Comparing `google-cloud-speech-2.9.2/tests/__init__.py` & `google-cloud-speech-2.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/tests/system/gapic/v1/test_system_speech_v1.py` & `google-cloud-speech-2.9.3/tests/system/gapic/v1/test_system_speech_v1.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/tests/system/gapic/v1p1beta1/test_system_speech_v1p1beta1.py` & `google-cloud-speech-2.9.3/tests/system/gapic/v1p1beta1/test_system_speech_v1p1beta1.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/tests/unit/__init__.py` & `google-cloud-speech-2.9.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/tests/unit/gapic/__init__.py` & `google-cloud-speech-2.9.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/tests/unit/gapic/speech_v1/__init__.py` & `google-cloud-speech-2.9.3/tests/unit/gapic/speech_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/tests/unit/gapic/speech_v1/test_speech.py` & `google-cloud-speech-2.9.3/tests/unit/gapic/speech_v1/test_speech.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/tests/unit/gapic/speech_v1p1beta1/__init__.py` & `google-cloud-speech-2.9.3/tests/unit/gapic/speech_v1p1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/tests/unit/gapic/speech_v1p1beta1/test_adaptation.py` & `google-cloud-speech-2.9.3/tests/unit/gapic/speech_v1p1beta1/test_adaptation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/tests/unit/gapic/speech_v1p1beta1/test_speech.py` & `google-cloud-speech-2.9.3/tests/unit/gapic/speech_v1p1beta1/test_speech.py`

 * *Files identical despite different names*

### Comparing `google-cloud-speech-2.9.2/tests/unit/test_helpers.py` & `google-cloud-speech-2.9.3/tests/unit/test_helpers.py`

 * *Files identical despite different names*

