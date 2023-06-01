# Comparing `tmp/google-cloud-videointelligence-2.8.3.tar.gz` & `tmp/google-cloud-videointelligence-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-videointelligence-2.8.3.tar", last modified: Mon Oct 10 18:07:17 2022, max compression
+gzip compressed data, was "google-cloud-videointelligence-2.9.0.tar", last modified: Thu Dec 15 20:09:44 2022, max compression
```

## Comparing `google-cloud-videointelligence-2.8.3.tar` & `google-cloud-videointelligence-2.9.0.tar`

### file list

```diff
@@ -1,146 +1,150 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.440730 google-cloud-videointelligence-2.8.3/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5101 2022-10-10 18:07:17.440730 google-cloud-videointelligence-2.8.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4182 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.412719 google-cloud-videointelligence-2.8.3/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.416720 google-cloud-videointelligence-2.8.3/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.420722 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence/
--rw-rw-r--   0 root         (0)     1003     3283 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence/__init__.py
--rw-rw-r--   0 root         (0)     1003       91 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.420722 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/
--rw-rw-r--   0 root         (0)     1003     3111 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      839 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       91 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.420722 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.420722 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/
--rw-rw-r--   0 root         (0)     1003      809 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    16113 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    23916 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.420722 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/
--rw-rw-r--   0 root         (0)     1003     1291 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6838 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12701 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12988 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.420722 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/types/
--rw-rw-r--   0 root         (0)     1003     2893 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    55142 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/types/video_intelligence.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.424724 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/
--rw-rw-r--   0 root         (0)     1003     2011 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003      849 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       91 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.424724 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.424724 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/
--rw-rw-r--   0 root         (0)     1003      809 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    16167 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    23970 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.424724 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/
--rw-rw-r--   0 root         (0)     1003     1291 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6843 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12720 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13007 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.424724 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/types/
--rw-rw-r--   0 root         (0)     1003     1793 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    21995 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/types/video_intelligence.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.424724 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/
--rw-rw-r--   0 root         (0)     1003     2049 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003      853 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       91 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.424724 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.424724 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/
--rw-rw-r--   0 root         (0)     1003      809 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    16187 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    23990 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.428725 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/
--rw-rw-r--   0 root         (0)     1003     1291 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6845 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12724 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13011 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.428725 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1831 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    25853 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/types/video_intelligence.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.428725 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/
--rw-rw-r--   0 root         (0)     1003     2229 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003      853 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       91 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.428725 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.428725 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/
--rw-rw-r--   0 root         (0)     1003      809 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    16182 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    23985 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.428725 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/
--rw-rw-r--   0 root         (0)     1003     1291 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6845 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12724 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13011 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.432727 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/types/
--rw-rw-r--   0 root         (0)     1003     2011 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    27346 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/types/video_intelligence.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.432727 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/
--rw-rw-r--   0 root         (0)     1003     4362 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1482 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       91 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.432727 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.432727 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/
--rw-rw-r--   0 root         (0)     1003      845 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    14530 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    21812 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.432727 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/
--rw-rw-r--   0 root         (0)     1003     1378 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6761 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12136 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12373 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.432727 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/
--rw-rw-r--   0 root         (0)     1003      809 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    16162 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    23965 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.432727 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/
--rw-rw-r--   0 root         (0)     1003     1291 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6845 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12715 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13002 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.436729 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/types/
--rw-rw-r--   0 root         (0)     1003     3887 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    68381 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/types/video_intelligence.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.436729 google-cloud-videointelligence-2.8.3/google_cloud_videointelligence.egg-info/
--rw-r--r--   0 root         (0)     1003     5101 2022-10-10 18:07:17.000000 google-cloud-videointelligence-2.8.3/google_cloud_videointelligence.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     7138 2022-10-10 18:07:17.000000 google-cloud-videointelligence-2.8.3/google_cloud_videointelligence.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 18:07:17.000000 google-cloud-videointelligence-2.8.3/google_cloud_videointelligence.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-10 18:07:17.000000 google-cloud-videointelligence-2.8.3/google_cloud_videointelligence.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 18:07:17.000000 google-cloud-videointelligence-2.8.3/google_cloud_videointelligence.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      256 2022-10-10 18:07:17.000000 google-cloud-videointelligence-2.8.3/google_cloud_videointelligence.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-10 18:07:17.000000 google-cloud-videointelligence-2.8.3/google_cloud_videointelligence.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.436729 google-cloud-videointelligence-2.8.3/scripts/
--rw-rw-r--   0 root         (0)     1003     6068 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/scripts/fixup_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-10 18:07:17.440730 google-cloud-videointelligence-2.8.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2986 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.436729 google-cloud-videointelligence-2.8.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.436729 google-cloud-videointelligence-2.8.3/tests/system/
--rw-rw-r--   0 root         (0)     1003     1630 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/system/test_system.py
--rw-rw-r--   0 root         (0)     1003     2820 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/system/test_vpcsc.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.436729 google-cloud-videointelligence-2.8.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.436729 google-cloud-videointelligence-2.8.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.436729 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    60117 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1/test_video_intelligence_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.436729 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1beta2/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003    60147 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1beta2/test_video_intelligence_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.440730 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    60159 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p1beta1/test_video_intelligence_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.440730 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p2beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p2beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    60159 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p2beta1/test_video_intelligence_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:07:17.440730 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p3beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p3beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    56722 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p3beta1/test_streaming_video_intelligence_service.py
--rw-rw-r--   0 root         (0)     1003    60159 2022-10-10 18:03:44.000000 google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p3beta1/test_video_intelligence_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.248603 google-cloud-videointelligence-2.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5077 2022-12-15 20:09:44.248603 google-cloud-videointelligence-2.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4182 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.220589 google-cloud-videointelligence-2.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.224591 google-cloud-videointelligence-2.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.228593 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence/
+-rw-rw-r--   0 root         (0)     1003     3403 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.228593 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/
+-rw-rw-r--   0 root         (0)     1003     3231 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      839 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.228593 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.228593 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/
+-rw-rw-r--   0 root         (0)     1003      809 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16169 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    24080 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.228593 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1291 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6717 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12801 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13075 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.228593 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2893 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    58272 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/types/video_intelligence.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.232595 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/
+-rw-rw-r--   0 root         (0)     1003     2131 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003      849 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.232595 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.232595 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/
+-rw-rw-r--   0 root         (0)     1003      809 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16228 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    24139 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.232595 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1291 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6727 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12820 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13094 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.232595 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/types/
+-rw-rw-r--   0 root         (0)     1003     1793 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    23297 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/types/video_intelligence.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.232595 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003     2169 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      853 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.232595 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.232595 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/
+-rw-rw-r--   0 root         (0)     1003      809 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16250 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    24161 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.236597 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1291 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6731 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12824 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13098 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.236597 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1831 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27218 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/types/video_intelligence.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.236597 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/
+-rw-rw-r--   0 root         (0)     1003     2349 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      853 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.236597 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.236597 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/
+-rw-rw-r--   0 root         (0)     1003      809 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16245 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    24156 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.236597 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1291 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6731 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12824 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13098 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.236597 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2011 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28891 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/types/video_intelligence.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.236597 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/
+-rw-rw-r--   0 root         (0)     1003     4482 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1482 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.240599 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.240599 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/
+-rw-rw-r--   0 root         (0)     1003      845 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14512 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    21958 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.240599 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1378 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6647 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12236 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12460 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.240599 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/
+-rw-rw-r--   0 root         (0)     1003      809 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16225 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    24136 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.240599 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1291 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6731 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12815 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13089 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.240599 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/types/
+-rw-rw-r--   0 root         (0)     1003     3887 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    72104 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/types/video_intelligence.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.244601 google-cloud-videointelligence-2.9.0/google_cloud_videointelligence.egg-info/
+-rw-r--r--   0 root         (0)     1003     5077 2022-12-15 20:09:44.000000 google-cloud-videointelligence-2.9.0/google_cloud_videointelligence.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     7441 2022-12-15 20:09:44.000000 google-cloud-videointelligence-2.9.0/google_cloud_videointelligence.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-15 20:09:44.000000 google-cloud-videointelligence-2.9.0/google_cloud_videointelligence.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-12-15 20:09:44.000000 google-cloud-videointelligence-2.9.0/google_cloud_videointelligence.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-15 20:09:44.000000 google-cloud-videointelligence-2.9.0/google_cloud_videointelligence.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      257 2022-12-15 20:09:44.000000 google-cloud-videointelligence-2.9.0/google_cloud_videointelligence.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-12-15 20:09:44.000000 google-cloud-videointelligence-2.9.0/google_cloud_videointelligence.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2022-12-15 20:09:44.248603 google-cloud-videointelligence-2.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2907 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.244601 google-cloud-videointelligence-2.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.244601 google-cloud-videointelligence-2.9.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003     1630 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/system/test_system.py
+-rw-rw-r--   0 root         (0)     1003     2820 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/system/test_vpcsc.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.244601 google-cloud-videointelligence-2.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.244601 google-cloud-videointelligence-2.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.244601 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    60117 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1/test_video_intelligence_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.244601 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1beta2/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    60147 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1beta2/test_video_intelligence_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.244601 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    60159 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p1beta1/test_video_intelligence_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.244601 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p2beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p2beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    60159 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p2beta1/test_video_intelligence_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 20:09:44.244601 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p3beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p3beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    56722 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p3beta1/test_streaming_video_intelligence_service.py
+-rw-rw-r--   0 root         (0)     1003    60159 2022-12-15 20:06:25.000000 google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p3beta1/test_video_intelligence_service.py
```

### Comparing `google-cloud-videointelligence-2.8.3/LICENSE` & `google-cloud-videointelligence-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/MANIFEST.in` & `google-cloud-videointelligence-2.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/PKG-INFO` & `google-cloud-videointelligence-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: google-cloud-videointelligence
-Version: 2.8.3
-Summary: Google Cloud Video Intelligence API client library
+Version: 2.9.0
+Summary: Google Cloud Videointelligence API client library
 Home-page: https://github.com/googleapis/python-videointelligence
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
-Provides-Extra: libcst
 License-File: LICENSE
 
 Python Client for Video Intelligence API
 ========================================
 
 |stable| |pypi| |versions|
```

### Comparing `google-cloud-videointelligence-2.8.3/README.rst` & `google-cloud-videointelligence-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.videointelligence import gapic_version as package_version
 
-from google.cloud.videointelligence_v1.services.video_intelligence_service.async_client import (
+__version__ = package_version.__version__
+
+
+from .services.video_intelligence_service import (
     VideoIntelligenceServiceAsyncClient,
-)
-from google.cloud.videointelligence_v1.services.video_intelligence_service.client import (
     VideoIntelligenceServiceClient,
 )
-from google.cloud.videointelligence_v1.types.video_intelligence import (
+from .types.video_intelligence import (
     AnnotateVideoProgress,
     AnnotateVideoRequest,
     AnnotateVideoResponse,
     DetectedAttribute,
     DetectedLandmark,
     Entity,
     ExplicitContentAnnotation,
@@ -66,15 +68,14 @@
     VideoAnnotationResults,
     VideoContext,
     VideoSegment,
     WordInfo,
 )
 
 __all__ = (
-    "VideoIntelligenceServiceClient",
     "VideoIntelligenceServiceAsyncClient",
     "AnnotateVideoProgress",
     "AnnotateVideoRequest",
     "AnnotateVideoResponse",
     "DetectedAttribute",
     "DetectedLandmark",
     "Entity",
@@ -82,18 +83,21 @@
     "ExplicitContentDetectionConfig",
     "ExplicitContentFrame",
     "FaceAnnotation",
     "FaceDetectionAnnotation",
     "FaceDetectionConfig",
     "FaceFrame",
     "FaceSegment",
+    "Feature",
     "LabelAnnotation",
     "LabelDetectionConfig",
+    "LabelDetectionMode",
     "LabelFrame",
     "LabelSegment",
+    "Likelihood",
     "LogoRecognitionAnnotation",
     "NormalizedBoundingBox",
     "NormalizedBoundingPoly",
     "NormalizedVertex",
     "ObjectTrackingAnnotation",
     "ObjectTrackingConfig",
     "ObjectTrackingFrame",
@@ -109,13 +113,11 @@
     "TextFrame",
     "TextSegment",
     "TimestampedObject",
     "Track",
     "VideoAnnotationProgress",
     "VideoAnnotationResults",
     "VideoContext",
+    "VideoIntelligenceServiceClient",
     "VideoSegment",
     "WordInfo",
-    "Feature",
-    "LabelDetectionMode",
-    "Likelihood",
 )
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,20 +9,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.videointelligence import gapic_version as package_version
 
-from .services.video_intelligence_service import (
+__version__ = package_version.__version__
+
+
+from google.cloud.videointelligence_v1.services.video_intelligence_service.async_client import (
     VideoIntelligenceServiceAsyncClient,
+)
+from google.cloud.videointelligence_v1.services.video_intelligence_service.client import (
     VideoIntelligenceServiceClient,
 )
-from .types.video_intelligence import (
+from google.cloud.videointelligence_v1.types.video_intelligence import (
     AnnotateVideoProgress,
     AnnotateVideoRequest,
     AnnotateVideoResponse,
     DetectedAttribute,
     DetectedLandmark,
     Entity,
     ExplicitContentAnnotation,
@@ -64,14 +70,15 @@
     VideoAnnotationResults,
     VideoContext,
     VideoSegment,
     WordInfo,
 )
 
 __all__ = (
+    "VideoIntelligenceServiceClient",
     "VideoIntelligenceServiceAsyncClient",
     "AnnotateVideoProgress",
     "AnnotateVideoRequest",
     "AnnotateVideoResponse",
     "DetectedAttribute",
     "DetectedLandmark",
     "Entity",
@@ -79,21 +86,18 @@
     "ExplicitContentDetectionConfig",
     "ExplicitContentFrame",
     "FaceAnnotation",
     "FaceDetectionAnnotation",
     "FaceDetectionConfig",
     "FaceFrame",
     "FaceSegment",
-    "Feature",
     "LabelAnnotation",
     "LabelDetectionConfig",
-    "LabelDetectionMode",
     "LabelFrame",
     "LabelSegment",
-    "Likelihood",
     "LogoRecognitionAnnotation",
     "NormalizedBoundingBox",
     "NormalizedBoundingPoly",
     "NormalizedVertex",
     "ObjectTrackingAnnotation",
     "ObjectTrackingConfig",
     "ObjectTrackingFrame",
@@ -109,11 +113,13 @@
     "TextFrame",
     "TextSegment",
     "TimestampedObject",
     "Track",
     "VideoAnnotationProgress",
     "VideoAnnotationResults",
     "VideoContext",
-    "VideoIntelligenceServiceClient",
     "VideoSegment",
     "WordInfo",
+    "Feature",
+    "LabelDetectionMode",
+    "Likelihood",
 )
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/gapic_metadata.json` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/async_client.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,34 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.videointelligence_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
@@ -160,17 +171,17 @@
         type(VideoIntelligenceServiceClient).get_transport_class,
         type(VideoIntelligenceServiceClient),
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, VideoIntelligenceServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the video intelligence service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -206,20 +217,20 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def annotate_video(
         self,
-        request: Union[video_intelligence.AnnotateVideoRequest, dict] = None,
+        request: Optional[Union[video_intelligence.AnnotateVideoRequest, dict]] = None,
         *,
-        input_uri: str = None,
-        features: Sequence[video_intelligence.Feature] = None,
+        input_uri: Optional[str] = None,
+        features: Optional[MutableSequence[video_intelligence.Feature]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Performs asynchronous video annotation. Progress and results can
         be retrieved through the ``google.longrunning.Operations``
         interface. ``Operation.metadata`` contains
         ``AnnotateVideoProgress`` (progress). ``Operation.response``
         contains ``AnnotateVideoResponse`` (results).
@@ -237,29 +248,29 @@
 
             async def sample_annotate_video():
                 # Create a client
                 client = videointelligence_v1.VideoIntelligenceServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = videointelligence_v1.AnnotateVideoRequest(
-                    features="PERSON_DETECTION",
+                    features=['PERSON_DETECTION'],
                 )
 
                 # Make the request
                 operation = client.annotate_video(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.videointelligence_v1.types.AnnotateVideoRequest, dict]):
+            request (Optional[Union[google.cloud.videointelligence_v1.types.AnnotateVideoRequest, dict]]):
                 The request object. Video annotation request.
             input_uri (:class:`str`):
                 Input video location. Currently, only `Cloud
                 Storage <https://cloud.google.com/storage/>`__ URIs are
                 supported. URIs must be specified in the following
                 format: ``gs://bucket-id/object-id`` (other URI formats
                 return
@@ -272,15 +283,15 @@
                 If unset, the input video should be embedded in the
                 request as ``input_content``. If set, ``input_content``
                 must be unset.
 
                 This corresponds to the ``input_uri`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            features (:class:`Sequence[google.cloud.videointelligence_v1.types.Feature]`):
+            features (:class:`MutableSequence[google.cloud.videointelligence_v1.types.Feature]`):
                 Required. Requested video annotation
                 features.
 
                 This corresponds to the ``features`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -357,18 +368,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("VideoIntelligenceServiceAsyncClient",)
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/client.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,36 +12,48 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.videointelligence_v1beta2 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 
-from google.cloud.videointelligence_v1.types import video_intelligence
+from google.cloud.videointelligence_v1beta2.types import video_intelligence
 
 from .transports.base import DEFAULT_CLIENT_INFO, VideoIntelligenceServiceTransport
 from .transports.grpc import VideoIntelligenceServiceGrpcTransport
 from .transports.grpc_asyncio import VideoIntelligenceServiceGrpcAsyncIOTransport
 
 
 class VideoIntelligenceServiceClientMeta(type):
@@ -56,15 +68,15 @@
         OrderedDict()
     )  # type: Dict[str, Type[VideoIntelligenceServiceTransport]]
     _transport_registry["grpc"] = VideoIntelligenceServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = VideoIntelligenceServiceGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[VideoIntelligenceServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -77,15 +89,15 @@
 
         # No transport is requested; return the default (that is, the first one
         # in the dictionary).
         return next(iter(cls._transport_registry.values()))
 
 
 class VideoIntelligenceServiceClient(metaclass=VideoIntelligenceServiceClientMeta):
-    """Service that implements the Video Intelligence API."""
+    """Service that implements Google Cloud Video Intelligence API."""
 
     @staticmethod
     def _get_default_mtls_endpoint(api_endpoint):
         """Converts api endpoint to mTLS endpoint.
 
         Convert "*.sandbox.googleapis.com" and "*.googleapis.com" to
         "*.mtls.sandbox.googleapis.com" and "*.mtls.googleapis.com" respectively.
@@ -309,30 +321,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, VideoIntelligenceServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, VideoIntelligenceServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the video intelligence service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, VideoIntelligenceServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -354,14 +366,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -406,20 +419,20 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def annotate_video(
         self,
-        request: Union[video_intelligence.AnnotateVideoRequest, dict] = None,
+        request: Optional[Union[video_intelligence.AnnotateVideoRequest, dict]] = None,
         *,
-        input_uri: str = None,
-        features: Sequence[video_intelligence.Feature] = None,
+        input_uri: Optional[str] = None,
+        features: Optional[MutableSequence[video_intelligence.Feature]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Performs asynchronous video annotation. Progress and results can
         be retrieved through the ``google.longrunning.Operations``
         interface. ``Operation.metadata`` contains
         ``AnnotateVideoProgress`` (progress). ``Operation.response``
         contains ``AnnotateVideoResponse`` (results).
@@ -429,58 +442,58 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import videointelligence_v1
+            from google.cloud import videointelligence_v1beta2
 
             def sample_annotate_video():
                 # Create a client
-                client = videointelligence_v1.VideoIntelligenceServiceClient()
+                client = videointelligence_v1beta2.VideoIntelligenceServiceClient()
 
                 # Initialize request argument(s)
-                request = videointelligence_v1.AnnotateVideoRequest(
-                    features="PERSON_DETECTION",
+                request = videointelligence_v1beta2.AnnotateVideoRequest(
+                    features=['FACE_DETECTION'],
                 )
 
                 # Make the request
                 operation = client.annotate_video(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.videointelligence_v1.types.AnnotateVideoRequest, dict]):
+            request (Union[google.cloud.videointelligence_v1beta2.types.AnnotateVideoRequest, dict]):
                 The request object. Video annotation request.
             input_uri (str):
-                Input video location. Currently, only `Cloud
+                Input video location. Currently, only `Google Cloud
                 Storage <https://cloud.google.com/storage/>`__ URIs are
-                supported. URIs must be specified in the following
+                supported, which must be specified in the following
                 format: ``gs://bucket-id/object-id`` (other URI formats
                 return
                 [google.rpc.Code.INVALID_ARGUMENT][google.rpc.Code.INVALID_ARGUMENT]).
                 For more information, see `Request
                 URIs <https://cloud.google.com/storage/docs/request-endpoints>`__.
-                To identify multiple videos, a video URI may include
-                wildcards in the ``object-id``. Supported wildcards: '*'
+                A video URI may include wildcards in ``object-id``, and
+                thus identify multiple videos. Supported wildcards: '*'
                 to match 0 or more characters; '?' to match 1 character.
                 If unset, the input video should be embedded in the
                 request as ``input_content``. If set, ``input_content``
-                must be unset.
+                should be unset.
 
                 This corresponds to the ``input_uri`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            features (Sequence[google.cloud.videointelligence_v1.types.Feature]):
+            features (MutableSequence[google.cloud.videointelligence_v1beta2.types.Feature]):
                 Required. Requested video annotation
                 features.
 
                 This corresponds to the ``features`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -489,15 +502,15 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.videointelligence_v1.types.AnnotateVideoResponse` Video annotation response. Included in the response
+                The result type for the operation will be :class:`google.cloud.videointelligence_v1beta2.types.AnnotateVideoResponse` Video annotation response. Included in the response
                    field of the Operation returned by the GetOperation
                    call of the google::longrunning::Operations service.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -554,18 +567,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("VideoIntelligenceServiceClient",)
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/base.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,40 +20,35 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1, operations_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
 
-from google.cloud.videointelligence_v1.types import video_intelligence
+from google.cloud.videointelligence_v1p3beta1 import gapic_version as package_version
+from google.cloud.videointelligence_v1p3beta1.types import video_intelligence
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class VideoIntelligenceServiceTransport(abc.ABC):
     """Abstract transport class for VideoIntelligenceService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "videointelligence.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/grpc.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -178,16 +178,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/grpc_asyncio.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from google.api_core import gapic_v1, grpc_helpers_async, operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
-from google.cloud.videointelligence_v1.types import video_intelligence
+from google.cloud.videointelligence_v1p3beta1.types import video_intelligence
 
 from .base import DEFAULT_CLIENT_INFO, VideoIntelligenceServiceTransport
 from .grpc import VideoIntelligenceServiceGrpcTransport
 
 
 class VideoIntelligenceServiceGrpcAsyncIOTransport(VideoIntelligenceServiceTransport):
     """gRPC AsyncIO backend transport for VideoIntelligenceService.
@@ -45,15 +45,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -88,23 +88,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
@@ -271,15 +271,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "annotate_video" not in self._stubs:
             self._stubs["annotate_video"] = self.grpc_channel.unary_unary(
-                "/google.cloud.videointelligence.v1.VideoIntelligenceService/AnnotateVideo",
+                "/google.cloud.videointelligence.v1p3beta1.VideoIntelligenceService/AnnotateVideo",
                 request_serializer=video_intelligence.AnnotateVideoRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["annotate_video"]
 
     def close(self):
         return self.grpc_channel.close()
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/types/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1/types/video_intelligence.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/types/video_intelligence.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.videointelligence.v1",
@@ -120,15 +122,15 @@
             match 0 or more characters; '?' to match 1 character. If
             unset, the input video should be embedded in the request as
             ``input_content``. If set, ``input_content`` must be unset.
         input_content (bytes):
             The video data bytes. If unset, the input video(s) should be
             specified via the ``input_uri``. If set, ``input_uri`` must
             be unset.
-        features (Sequence[google.cloud.videointelligence_v1.types.Feature]):
+        features (MutableSequence[google.cloud.videointelligence_v1.types.Feature]):
             Required. Requested video annotation
             features.
         video_context (google.cloud.videointelligence_v1.types.VideoContext):
             Additional video context and/or
             feature-specific parameters.
         output_uri (str):
             Optional. Location where the output (in JSON format) should
@@ -142,47 +144,47 @@
         location_id (str):
             Optional. Cloud region where annotation should take place.
             Supported cloud regions are: ``us-east1``, ``us-west1``,
             ``europe-west1``, ``asia-east1``. If no region is specified,
             the region will be determined based on video file location.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    input_content = proto.Field(
+    input_content: bytes = proto.Field(
         proto.BYTES,
         number=6,
     )
-    features = proto.RepeatedField(
+    features: MutableSequence["Feature"] = proto.RepeatedField(
         proto.ENUM,
         number=2,
         enum="Feature",
     )
-    video_context = proto.Field(
+    video_context: "VideoContext" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="VideoContext",
     )
-    output_uri = proto.Field(
+    output_uri: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    location_id = proto.Field(
+    location_id: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class VideoContext(proto.Message):
     r"""Video context and/or feature-specific parameters.
 
     Attributes:
-        segments (Sequence[google.cloud.videointelligence_v1.types.VideoSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1.types.VideoSegment]):
             Video segments to annotate. The segments may
             overlap and are not required to be contiguous or
             span the whole video. If unspecified, each video
             is treated as a single segment.
         label_detection_config (google.cloud.videointelligence_v1.types.LabelDetectionConfig):
             Config for LABEL_DETECTION.
         shot_change_detection_config (google.cloud.videointelligence_v1.types.ShotChangeDetectionConfig):
@@ -197,55 +199,55 @@
             Config for TEXT_DETECTION.
         person_detection_config (google.cloud.videointelligence_v1.types.PersonDetectionConfig):
             Config for PERSON_DETECTION.
         object_tracking_config (google.cloud.videointelligence_v1.types.ObjectTrackingConfig):
             Config for OBJECT_TRACKING.
     """
 
-    segments = proto.RepeatedField(
+    segments: MutableSequence["VideoSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    label_detection_config = proto.Field(
+    label_detection_config: "LabelDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="LabelDetectionConfig",
     )
-    shot_change_detection_config = proto.Field(
+    shot_change_detection_config: "ShotChangeDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="ShotChangeDetectionConfig",
     )
-    explicit_content_detection_config = proto.Field(
+    explicit_content_detection_config: "ExplicitContentDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="ExplicitContentDetectionConfig",
     )
-    face_detection_config = proto.Field(
+    face_detection_config: "FaceDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="FaceDetectionConfig",
     )
-    speech_transcription_config = proto.Field(
+    speech_transcription_config: "SpeechTranscriptionConfig" = proto.Field(
         proto.MESSAGE,
         number=6,
         message="SpeechTranscriptionConfig",
     )
-    text_detection_config = proto.Field(
+    text_detection_config: "TextDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=8,
         message="TextDetectionConfig",
     )
-    person_detection_config = proto.Field(
+    person_detection_config: "PersonDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=11,
         message="PersonDetectionConfig",
     )
-    object_tracking_config = proto.Field(
+    object_tracking_config: "ObjectTrackingConfig" = proto.Field(
         proto.MESSAGE,
         number=13,
         message="ObjectTrackingConfig",
     )
 
 
 class LabelDetectionConfig(proto.Message):
@@ -279,32 +281,32 @@
             set to 0.3 by default. The valid range for this threshold is
             [0.1, 0.9]. Any value set outside of this range will be
             clipped. Note: For best results, follow the default
             threshold. We will update the default threshold everytime
             when we release a new model.
     """
 
-    label_detection_mode = proto.Field(
+    label_detection_mode: "LabelDetectionMode" = proto.Field(
         proto.ENUM,
         number=1,
         enum="LabelDetectionMode",
     )
-    stationary_camera = proto.Field(
+    stationary_camera: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    frame_confidence_threshold = proto.Field(
+    frame_confidence_threshold: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
-    video_confidence_threshold = proto.Field(
+    video_confidence_threshold: float = proto.Field(
         proto.FLOAT,
         number=5,
     )
 
 
 class ShotChangeDetectionConfig(proto.Message):
     r"""Config for SHOT_CHANGE_DETECTION.
@@ -312,15 +314,15 @@
     Attributes:
         model (str):
             Model to use for shot change detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ObjectTrackingConfig(proto.Message):
     r"""Config for OBJECT_TRACKING.
@@ -328,15 +330,15 @@
     Attributes:
         model (str):
             Model to use for object tracking.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class FaceDetectionConfig(proto.Message):
     r"""Config for FACE_DETECTION.
@@ -351,23 +353,23 @@
             face annotation output.
         include_attributes (bool):
             Whether to enable face attributes detection, such as
             glasses, dark_glasses, mouth_open etc. Ignored if
             'include_bounding_boxes' is set to false.
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    include_bounding_boxes = proto.Field(
+    include_bounding_boxes: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
-    include_attributes = proto.Field(
+    include_attributes: bool = proto.Field(
         proto.BOOL,
         number=5,
     )
 
 
 class PersonDetectionConfig(proto.Message):
     r"""Config for PERSON_DETECTION.
@@ -382,23 +384,23 @@
         include_attributes (bool):
             Whether to enable person attributes detection, such as cloth
             color (black, blue, etc), type (coat, dress, etc), pattern
             (plain, floral, etc), hair, etc. Ignored if
             'include_bounding_boxes' is set to false.
     """
 
-    include_bounding_boxes = proto.Field(
+    include_bounding_boxes: bool = proto.Field(
         proto.BOOL,
         number=1,
     )
-    include_pose_landmarks = proto.Field(
+    include_pose_landmarks: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
-    include_attributes = proto.Field(
+    include_attributes: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
 
 
 class ExplicitContentDetectionConfig(proto.Message):
     r"""Config for EXPLICIT_CONTENT_DETECTION.
@@ -406,44 +408,44 @@
     Attributes:
         model (str):
             Model to use for explicit content detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class TextDetectionConfig(proto.Message):
     r"""Config for TEXT_DETECTION.
 
     Attributes:
-        language_hints (Sequence[str]):
+        language_hints (MutableSequence[str]):
             Language hint can be specified if the
             language to be detected is known a priori. It
             can increase the accuracy of the detection.
             Language hint must be language code in BCP-47
             format.
 
             Automatic language detection is performed if no
             hint is provided.
         model (str):
             Model to use for text detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    language_hints = proto.RepeatedField(
+    language_hints: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=1,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class VideoSegment(proto.Message):
     r"""Video segment.
@@ -455,20 +457,20 @@
             (inclusive).
         end_time_offset (google.protobuf.duration_pb2.Duration):
             Time-offset, relative to the beginning of the
             video, corresponding to the end of the segment
             (inclusive).
     """
 
-    start_time_offset = proto.Field(
+    start_time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    end_time_offset = proto.Field(
+    end_time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class LabelSegment(proto.Message):
@@ -477,20 +479,20 @@
     Attributes:
         segment (google.cloud.videointelligence_v1.types.VideoSegment):
             Video segment where a label was detected.
         confidence (float):
             Confidence that the label is accurate. Range: [0, 1].
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class LabelFrame(proto.Message):
     r"""Video frame level annotation results for label detection.
@@ -500,20 +502,20 @@
             Time-offset, relative to the beginning of the
             video, corresponding to the video frame for this
             location.
         confidence (float):
             Confidence that the label is accurate. Range: [0, 1].
     """
 
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class Entity(proto.Message):
     r"""Detected entity from video analysis.
@@ -525,69 +527,69 @@
             API <https://developers.google.com/knowledge-graph/>`__.
         description (str):
             Textual description, e.g., ``Fixed-gear bicycle``.
         language_code (str):
             Language code for ``description`` in BCP-47 format.
     """
 
-    entity_id = proto.Field(
+    entity_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class LabelAnnotation(proto.Message):
     r"""Label annotation.
 
     Attributes:
         entity (google.cloud.videointelligence_v1.types.Entity):
             Detected entity.
-        category_entities (Sequence[google.cloud.videointelligence_v1.types.Entity]):
+        category_entities (MutableSequence[google.cloud.videointelligence_v1.types.Entity]):
             Common categories for the detected entity. For example, when
             the label is ``Terrier``, the category is likely ``dog``.
             And in some cases there might be more than one categories
             e.g., ``Terrier`` could also be a ``pet``.
-        segments (Sequence[google.cloud.videointelligence_v1.types.LabelSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1.types.LabelSegment]):
             All video segments where a label was
             detected.
-        frames (Sequence[google.cloud.videointelligence_v1.types.LabelFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1.types.LabelFrame]):
             All video frames where a label was detected.
         version (str):
             Feature version.
     """
 
-    entity = proto.Field(
+    entity: "Entity" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Entity",
     )
-    category_entities = proto.RepeatedField(
+    category_entities: MutableSequence["Entity"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="Entity",
     )
-    segments = proto.RepeatedField(
+    segments: MutableSequence["LabelSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="LabelSegment",
     )
-    frames = proto.RepeatedField(
+    frames: MutableSequence["LabelFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="LabelFrame",
     )
-    version = proto.Field(
+    version: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class ExplicitContentFrame(proto.Message):
     r"""Video frame level annotation results for explicit content.
@@ -597,45 +599,45 @@
             Time-offset, relative to the beginning of the
             video, corresponding to the video frame for this
             location.
         pornography_likelihood (google.cloud.videointelligence_v1.types.Likelihood):
             Likelihood of the pornography content..
     """
 
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    pornography_likelihood = proto.Field(
+    pornography_likelihood: "Likelihood" = proto.Field(
         proto.ENUM,
         number=2,
         enum="Likelihood",
     )
 
 
 class ExplicitContentAnnotation(proto.Message):
     r"""Explicit content annotation (based on per-frame visual
     signals only). If no explicit content has been detected in a
     frame, no annotations are present for that frame.
 
     Attributes:
-        frames (Sequence[google.cloud.videointelligence_v1.types.ExplicitContentFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1.types.ExplicitContentFrame]):
             All video frames where explicit content was
             detected.
         version (str):
             Feature version.
     """
 
-    frames = proto.RepeatedField(
+    frames: MutableSequence["ExplicitContentFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="ExplicitContentFrame",
     )
-    version = proto.Field(
+    version: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class NormalizedBoundingBox(proto.Message):
     r"""Normalized bounding box. The normalized vertex coordinates are
@@ -648,145 +650,147 @@
             Top Y coordinate.
         right (float):
             Right X coordinate.
         bottom (float):
             Bottom Y coordinate.
     """
 
-    left = proto.Field(
+    left: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    top = proto.Field(
+    top: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    right = proto.Field(
+    right: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
-    bottom = proto.Field(
+    bottom: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
 
 
 class FaceDetectionAnnotation(proto.Message):
     r"""Face detection annotation.
 
     Attributes:
-        tracks (Sequence[google.cloud.videointelligence_v1.types.Track]):
+        tracks (MutableSequence[google.cloud.videointelligence_v1.types.Track]):
             The face tracks with attributes.
         thumbnail (bytes):
             The thumbnail of a person's face.
         version (str):
             Feature version.
     """
 
-    tracks = proto.RepeatedField(
+    tracks: MutableSequence["Track"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="Track",
     )
-    thumbnail = proto.Field(
+    thumbnail: bytes = proto.Field(
         proto.BYTES,
         number=4,
     )
-    version = proto.Field(
+    version: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class PersonDetectionAnnotation(proto.Message):
     r"""Person detection annotation per video.
 
     Attributes:
-        tracks (Sequence[google.cloud.videointelligence_v1.types.Track]):
+        tracks (MutableSequence[google.cloud.videointelligence_v1.types.Track]):
             The detected tracks of a person.
         version (str):
             Feature version.
     """
 
-    tracks = proto.RepeatedField(
+    tracks: MutableSequence["Track"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="Track",
     )
-    version = proto.Field(
+    version: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class FaceSegment(proto.Message):
     r"""Video segment level annotation results for face detection.
 
     Attributes:
         segment (google.cloud.videointelligence_v1.types.VideoSegment):
             Video segment where a face was detected.
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
 
 
 class FaceFrame(proto.Message):
     r"""Deprecated. No effect.
 
     Attributes:
-        normalized_bounding_boxes (Sequence[google.cloud.videointelligence_v1.types.NormalizedBoundingBox]):
+        normalized_bounding_boxes (MutableSequence[google.cloud.videointelligence_v1.types.NormalizedBoundingBox]):
             Normalized Bounding boxes in a frame.
             There can be more than one boxes if the same
             face is detected in multiple locations within
             the current frame.
         time_offset (google.protobuf.duration_pb2.Duration):
             Time-offset, relative to the beginning of the
             video, corresponding to the video frame for this
             location.
     """
 
-    normalized_bounding_boxes = proto.RepeatedField(
+    normalized_bounding_boxes: MutableSequence[
+        "NormalizedBoundingBox"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="NormalizedBoundingBox",
     )
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class FaceAnnotation(proto.Message):
     r"""Deprecated. No effect.
 
     Attributes:
         thumbnail (bytes):
             Thumbnail of a representative face view (in
             JPEG format).
-        segments (Sequence[google.cloud.videointelligence_v1.types.FaceSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1.types.FaceSegment]):
             All video segments where a face was detected.
-        frames (Sequence[google.cloud.videointelligence_v1.types.FaceFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1.types.FaceFrame]):
             All video frames where a face was detected.
     """
 
-    thumbnail = proto.Field(
+    thumbnail: bytes = proto.Field(
         proto.BYTES,
         number=1,
     )
-    segments = proto.RepeatedField(
+    segments: MutableSequence["FaceSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="FaceSegment",
     )
-    frames = proto.RepeatedField(
+    frames: MutableSequence["FaceFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="FaceFrame",
     )
 
 
 class TimestampedObject(proto.Message):
@@ -797,75 +801,75 @@
         normalized_bounding_box (google.cloud.videointelligence_v1.types.NormalizedBoundingBox):
             Normalized Bounding box in a frame, where the
             object is located.
         time_offset (google.protobuf.duration_pb2.Duration):
             Time-offset, relative to the beginning of the
             video, corresponding to the video frame for this
             object.
-        attributes (Sequence[google.cloud.videointelligence_v1.types.DetectedAttribute]):
+        attributes (MutableSequence[google.cloud.videointelligence_v1.types.DetectedAttribute]):
             Optional. The attributes of the object in the
             bounding box.
-        landmarks (Sequence[google.cloud.videointelligence_v1.types.DetectedLandmark]):
+        landmarks (MutableSequence[google.cloud.videointelligence_v1.types.DetectedLandmark]):
             Optional. The detected landmarks.
     """
 
-    normalized_bounding_box = proto.Field(
+    normalized_bounding_box: "NormalizedBoundingBox" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="NormalizedBoundingBox",
     )
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
-    attributes = proto.RepeatedField(
+    attributes: MutableSequence["DetectedAttribute"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="DetectedAttribute",
     )
-    landmarks = proto.RepeatedField(
+    landmarks: MutableSequence["DetectedLandmark"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="DetectedLandmark",
     )
 
 
 class Track(proto.Message):
     r"""A track of an object instance.
 
     Attributes:
         segment (google.cloud.videointelligence_v1.types.VideoSegment):
             Video segment of a track.
-        timestamped_objects (Sequence[google.cloud.videointelligence_v1.types.TimestampedObject]):
+        timestamped_objects (MutableSequence[google.cloud.videointelligence_v1.types.TimestampedObject]):
             The object with timestamp and attributes per
             frame in the track.
-        attributes (Sequence[google.cloud.videointelligence_v1.types.DetectedAttribute]):
+        attributes (MutableSequence[google.cloud.videointelligence_v1.types.DetectedAttribute]):
             Optional. Attributes in the track level.
         confidence (float):
             Optional. The confidence score of the tracked
             object.
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    timestamped_objects = proto.RepeatedField(
+    timestamped_objects: MutableSequence["TimestampedObject"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="TimestampedObject",
     )
-    attributes = proto.RepeatedField(
+    attributes: MutableSequence["DetectedAttribute"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="DetectedAttribute",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
 
 
 class DetectedAttribute(proto.Message):
     r"""A generic detected attribute represented by name in string
@@ -880,23 +884,23 @@
             Detected attribute confidence. Range [0, 1].
         value (str):
             Text value of the detection result. For
             example, the value for "HairColor" can be
             "black", "blonde", etc.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    value = proto.Field(
+    value: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class DetectedLandmark(proto.Message):
     r"""A generic detected landmark represented by name in string
@@ -911,196 +915,208 @@
             the normalized image coordindate system. The
             normalized coordinates have the range from 0 to
             1.
         confidence (float):
             The confidence score of the detected landmark. Range [0, 1].
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    point = proto.Field(
+    point: "NormalizedVertex" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="NormalizedVertex",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
 
 
 class VideoAnnotationResults(proto.Message):
     r"""Annotation results for a single video.
 
     Attributes:
         input_uri (str):
             Video file location in `Cloud
             Storage <https://cloud.google.com/storage/>`__.
         segment (google.cloud.videointelligence_v1.types.VideoSegment):
             Video segment on which the annotation is run.
-        segment_label_annotations (Sequence[google.cloud.videointelligence_v1.types.LabelAnnotation]):
+        segment_label_annotations (MutableSequence[google.cloud.videointelligence_v1.types.LabelAnnotation]):
             Topical label annotations on video level or
             user-specified segment level. There is exactly
             one element for each unique label.
-        segment_presence_label_annotations (Sequence[google.cloud.videointelligence_v1.types.LabelAnnotation]):
+        segment_presence_label_annotations (MutableSequence[google.cloud.videointelligence_v1.types.LabelAnnotation]):
             Presence label annotations on video level or user-specified
             segment level. There is exactly one element for each unique
             label. Compared to the existing topical
             ``segment_label_annotations``, this field presents more
             fine-grained, segment-level labels detected in video content
             and is made available only when the client sets
             ``LabelDetectionConfig.model`` to "builtin/latest" in the
             request.
-        shot_label_annotations (Sequence[google.cloud.videointelligence_v1.types.LabelAnnotation]):
+        shot_label_annotations (MutableSequence[google.cloud.videointelligence_v1.types.LabelAnnotation]):
             Topical label annotations on shot level.
             There is exactly one element for each unique
             label.
-        shot_presence_label_annotations (Sequence[google.cloud.videointelligence_v1.types.LabelAnnotation]):
+        shot_presence_label_annotations (MutableSequence[google.cloud.videointelligence_v1.types.LabelAnnotation]):
             Presence label annotations on shot level. There is exactly
             one element for each unique label. Compared to the existing
             topical ``shot_label_annotations``, this field presents more
             fine-grained, shot-level labels detected in video content
             and is made available only when the client sets
             ``LabelDetectionConfig.model`` to "builtin/latest" in the
             request.
-        frame_label_annotations (Sequence[google.cloud.videointelligence_v1.types.LabelAnnotation]):
+        frame_label_annotations (MutableSequence[google.cloud.videointelligence_v1.types.LabelAnnotation]):
             Label annotations on frame level.
             There is exactly one element for each unique
             label.
-        face_annotations (Sequence[google.cloud.videointelligence_v1.types.FaceAnnotation]):
+        face_annotations (MutableSequence[google.cloud.videointelligence_v1.types.FaceAnnotation]):
             Deprecated. Please use ``face_detection_annotations``
             instead.
-        face_detection_annotations (Sequence[google.cloud.videointelligence_v1.types.FaceDetectionAnnotation]):
+        face_detection_annotations (MutableSequence[google.cloud.videointelligence_v1.types.FaceDetectionAnnotation]):
             Face detection annotations.
-        shot_annotations (Sequence[google.cloud.videointelligence_v1.types.VideoSegment]):
+        shot_annotations (MutableSequence[google.cloud.videointelligence_v1.types.VideoSegment]):
             Shot annotations. Each shot is represented as
             a video segment.
         explicit_annotation (google.cloud.videointelligence_v1.types.ExplicitContentAnnotation):
             Explicit content annotation.
-        speech_transcriptions (Sequence[google.cloud.videointelligence_v1.types.SpeechTranscription]):
+        speech_transcriptions (MutableSequence[google.cloud.videointelligence_v1.types.SpeechTranscription]):
             Speech transcription.
-        text_annotations (Sequence[google.cloud.videointelligence_v1.types.TextAnnotation]):
+        text_annotations (MutableSequence[google.cloud.videointelligence_v1.types.TextAnnotation]):
             OCR text detection and tracking.
             Annotations for list of detected text snippets.
             Each will have list of frame information
             associated with it.
-        object_annotations (Sequence[google.cloud.videointelligence_v1.types.ObjectTrackingAnnotation]):
+        object_annotations (MutableSequence[google.cloud.videointelligence_v1.types.ObjectTrackingAnnotation]):
             Annotations for list of objects detected and
             tracked in video.
-        logo_recognition_annotations (Sequence[google.cloud.videointelligence_v1.types.LogoRecognitionAnnotation]):
+        logo_recognition_annotations (MutableSequence[google.cloud.videointelligence_v1.types.LogoRecognitionAnnotation]):
             Annotations for list of logos detected,
             tracked and recognized in video.
-        person_detection_annotations (Sequence[google.cloud.videointelligence_v1.types.PersonDetectionAnnotation]):
+        person_detection_annotations (MutableSequence[google.cloud.videointelligence_v1.types.PersonDetectionAnnotation]):
             Person detection annotations.
         error (google.rpc.status_pb2.Status):
             If set, indicates an error. Note that for a single
             ``AnnotateVideoRequest`` some videos may succeed and some
             may fail.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=10,
         message="VideoSegment",
     )
-    segment_label_annotations = proto.RepeatedField(
+    segment_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="LabelAnnotation",
     )
-    segment_presence_label_annotations = proto.RepeatedField(
+    segment_presence_label_annotations: MutableSequence[
+        "LabelAnnotation"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=23,
         message="LabelAnnotation",
     )
-    shot_label_annotations = proto.RepeatedField(
+    shot_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="LabelAnnotation",
     )
-    shot_presence_label_annotations = proto.RepeatedField(
+    shot_presence_label_annotations: MutableSequence[
+        "LabelAnnotation"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=24,
         message="LabelAnnotation",
     )
-    frame_label_annotations = proto.RepeatedField(
+    frame_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="LabelAnnotation",
     )
-    face_annotations = proto.RepeatedField(
+    face_annotations: MutableSequence["FaceAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=5,
         message="FaceAnnotation",
     )
-    face_detection_annotations = proto.RepeatedField(
+    face_detection_annotations: MutableSequence[
+        "FaceDetectionAnnotation"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=13,
         message="FaceDetectionAnnotation",
     )
-    shot_annotations = proto.RepeatedField(
+    shot_annotations: MutableSequence["VideoSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=6,
         message="VideoSegment",
     )
-    explicit_annotation = proto.Field(
+    explicit_annotation: "ExplicitContentAnnotation" = proto.Field(
         proto.MESSAGE,
         number=7,
         message="ExplicitContentAnnotation",
     )
-    speech_transcriptions = proto.RepeatedField(
+    speech_transcriptions: MutableSequence["SpeechTranscription"] = proto.RepeatedField(
         proto.MESSAGE,
         number=11,
         message="SpeechTranscription",
     )
-    text_annotations = proto.RepeatedField(
+    text_annotations: MutableSequence["TextAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=12,
         message="TextAnnotation",
     )
-    object_annotations = proto.RepeatedField(
+    object_annotations: MutableSequence[
+        "ObjectTrackingAnnotation"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=14,
         message="ObjectTrackingAnnotation",
     )
-    logo_recognition_annotations = proto.RepeatedField(
+    logo_recognition_annotations: MutableSequence[
+        "LogoRecognitionAnnotation"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=19,
         message="LogoRecognitionAnnotation",
     )
-    person_detection_annotations = proto.RepeatedField(
+    person_detection_annotations: MutableSequence[
+        "PersonDetectionAnnotation"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=20,
         message="PersonDetectionAnnotation",
     )
-    error = proto.Field(
+    error: status_pb2.Status = proto.Field(
         proto.MESSAGE,
         number=9,
         message=status_pb2.Status,
     )
 
 
 class AnnotateVideoResponse(proto.Message):
     r"""Video annotation response. Included in the ``response`` field of the
     ``Operation`` returned by the ``GetOperation`` call of the
     ``google::longrunning::Operations`` service.
 
     Attributes:
-        annotation_results (Sequence[google.cloud.videointelligence_v1.types.VideoAnnotationResults]):
+        annotation_results (MutableSequence[google.cloud.videointelligence_v1.types.VideoAnnotationResults]):
             Annotation results for all videos specified in
             ``AnnotateVideoRequest``.
     """
 
-    annotation_results = proto.RepeatedField(
+    annotation_results: MutableSequence["VideoAnnotationResults"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoAnnotationResults",
     )
 
 
 class VideoAnnotationProgress(proto.Message):
@@ -1121,56 +1137,58 @@
             Specifies which feature is being tracked if
             the request contains more than one feature.
         segment (google.cloud.videointelligence_v1.types.VideoSegment):
             Specifies which segment is being tracked if
             the request contains more than one segment.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    progress_percent = proto.Field(
+    progress_percent: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    start_time = proto.Field(
+    start_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
-    feature = proto.Field(
+    feature: "Feature" = proto.Field(
         proto.ENUM,
         number=5,
         enum="Feature",
     )
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=6,
         message="VideoSegment",
     )
 
 
 class AnnotateVideoProgress(proto.Message):
     r"""Video annotation progress. Included in the ``metadata`` field of the
     ``Operation`` returned by the ``GetOperation`` call of the
     ``google::longrunning::Operations`` service.
 
     Attributes:
-        annotation_progress (Sequence[google.cloud.videointelligence_v1.types.VideoAnnotationProgress]):
+        annotation_progress (MutableSequence[google.cloud.videointelligence_v1.types.VideoAnnotationProgress]):
             Progress metadata for all videos specified in
             ``AnnotateVideoRequest``.
     """
 
-    annotation_progress = proto.RepeatedField(
+    annotation_progress: MutableSequence[
+        "VideoAnnotationProgress"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoAnnotationProgress",
     )
 
 
 class SpeechTranscriptionConfig(proto.Message):
@@ -1193,29 +1211,29 @@
             will return a maximum of one.
         filter_profanity (bool):
             Optional. If set to ``true``, the server will attempt to
             filter out profanities, replacing all but the initial
             character in each filtered word with asterisks, e.g. "f***".
             If set to ``false`` or omitted, profanities won't be
             filtered out.
-        speech_contexts (Sequence[google.cloud.videointelligence_v1.types.SpeechContext]):
+        speech_contexts (MutableSequence[google.cloud.videointelligence_v1.types.SpeechContext]):
             Optional. A means to provide context to
             assist the speech recognition.
         enable_automatic_punctuation (bool):
             Optional. If 'true', adds punctuation to
             recognition result hypotheses. This feature is
             only available in select languages. Setting this
             for requests in other languages has no effect at
             all. The default 'false' value does not add
             punctuation to result hypotheses. NOTE: "This is
             currently offered as an experimental service,
             complimentary to all users. In the future this
             may be exclusively available as a premium
             feature.".
-        audio_tracks (Sequence[int]):
+        audio_tracks (MutableSequence[int]):
             Optional. For file formats, such as MXF or
             MKV, supporting multiple audio tracks, specify
             up to two tracks. Default: track 0.
         enable_speaker_diarization (bool):
             Optional. If 'true', enables speaker detection for each
             recognized word in the top alternative of the recognition
             result using a speaker_tag provided in the WordInfo. Note:
@@ -1231,100 +1249,100 @@
         enable_word_confidence (bool):
             Optional. If ``true``, the top result includes a list of
             words and the confidence for those words. If ``false``, no
             word-level confidence information is returned. The default
             is ``false``.
     """
 
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    max_alternatives = proto.Field(
+    max_alternatives: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    filter_profanity = proto.Field(
+    filter_profanity: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
-    speech_contexts = proto.RepeatedField(
+    speech_contexts: MutableSequence["SpeechContext"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="SpeechContext",
     )
-    enable_automatic_punctuation = proto.Field(
+    enable_automatic_punctuation: bool = proto.Field(
         proto.BOOL,
         number=5,
     )
-    audio_tracks = proto.RepeatedField(
+    audio_tracks: MutableSequence[int] = proto.RepeatedField(
         proto.INT32,
         number=6,
     )
-    enable_speaker_diarization = proto.Field(
+    enable_speaker_diarization: bool = proto.Field(
         proto.BOOL,
         number=7,
     )
-    diarization_speaker_count = proto.Field(
+    diarization_speaker_count: int = proto.Field(
         proto.INT32,
         number=8,
     )
-    enable_word_confidence = proto.Field(
+    enable_word_confidence: bool = proto.Field(
         proto.BOOL,
         number=9,
     )
 
 
 class SpeechContext(proto.Message):
     r"""Provides "hints" to the speech recognizer to favor specific
     words and phrases in the results.
 
     Attributes:
-        phrases (Sequence[str]):
+        phrases (MutableSequence[str]):
             Optional. A list of strings containing words and phrases
             "hints" so that the speech recognition is more likely to
             recognize them. This can be used to improve the accuracy for
             specific words and phrases, for example, if specific
             commands are typically spoken by the user. This can also be
             used to add additional words to the vocabulary of the
             recognizer. See `usage
             limits <https://cloud.google.com/speech/limits#content>`__.
     """
 
-    phrases = proto.RepeatedField(
+    phrases: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=1,
     )
 
 
 class SpeechTranscription(proto.Message):
     r"""A speech recognition result corresponding to a portion of the
     audio.
 
     Attributes:
-        alternatives (Sequence[google.cloud.videointelligence_v1.types.SpeechRecognitionAlternative]):
+        alternatives (MutableSequence[google.cloud.videointelligence_v1.types.SpeechRecognitionAlternative]):
             May contain one or more recognition hypotheses (up to the
             maximum specified in ``max_alternatives``). These
             alternatives are ordered in terms of accuracy, with the top
             (first) alternative being the most probable, as ranked by
             the recognizer.
         language_code (str):
             Output only. The
             `BCP-47 <https://www.rfc-editor.org/rfc/bcp/bcp47.txt>`__
             language tag of the language in this result. This language
             code was detected to have the most likelihood of being
             spoken in the audio.
     """
 
-    alternatives = proto.RepeatedField(
+    alternatives: MutableSequence["SpeechRecognitionAlternative"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="SpeechRecognitionAlternative",
     )
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class SpeechRecognitionAlternative(proto.Message):
     r"""Alternative hypotheses (a.k.a. n-best list).
@@ -1337,30 +1355,30 @@
             Output only. The confidence estimate between 0.0 and 1.0. A
             higher number indicates an estimated greater likelihood that
             the recognized words are correct. This field is set only for
             the top alternative. This field is not guaranteed to be
             accurate and users should not rely on it to be always
             provided. The default of 0.0 is a sentinel value indicating
             ``confidence`` was not set.
-        words (Sequence[google.cloud.videointelligence_v1.types.WordInfo]):
+        words (MutableSequence[google.cloud.videointelligence_v1.types.WordInfo]):
             Output only. A list of word-specific information for each
             recognized word. Note: When ``enable_speaker_diarization``
             is set to true, you will see all the words from the
             beginning of the audio.
     """
 
-    transcript = proto.Field(
+    transcript: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    words = proto.RepeatedField(
+    words: MutableSequence["WordInfo"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="WordInfo",
     )
 
 
 class WordInfo(proto.Message):
@@ -1396,33 +1414,33 @@
             Output only. A distinct integer value is assigned for every
             speaker within the audio. This field specifies which one of
             those speakers was detected to have spoken this word. Value
             ranges from 1 up to diarization_speaker_count, and is only
             set if speaker diarization is enabled.
     """
 
-    start_time = proto.Field(
+    start_time: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    end_time = proto.Field(
+    end_time: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
-    word = proto.Field(
+    word: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
-    speaker_tag = proto.Field(
+    speaker_tag: int = proto.Field(
         proto.INT32,
         number=5,
     )
 
 
 class NormalizedVertex(proto.Message):
     r"""A vertex represents a 2D point in the image.
@@ -1432,19 +1450,19 @@
     Attributes:
         x (float):
             X coordinate.
         y (float):
             Y coordinate.
     """
 
-    x = proto.Field(
+    x: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    y = proto.Field(
+    y: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class NormalizedBoundingPoly(proto.Message):
     r"""Normalized bounding polygon for text (that might not be aligned with
@@ -1457,19 +1475,19 @@
     it becomes: 2----3 \| \| 1----0
 
     and the vertex order will still be (0, 1, 2, 3). Note that values
     can be less than 0, or greater than 1 due to trignometric
     calculations for location of the box.
 
     Attributes:
-        vertices (Sequence[google.cloud.videointelligence_v1.types.NormalizedVertex]):
+        vertices (MutableSequence[google.cloud.videointelligence_v1.types.NormalizedVertex]):
             Normalized vertices of the bounding polygon.
     """
 
-    vertices = proto.RepeatedField(
+    vertices: MutableSequence["NormalizedVertex"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="NormalizedVertex",
     )
 
 
 class TextSegment(proto.Message):
@@ -1479,29 +1497,29 @@
         segment (google.cloud.videointelligence_v1.types.VideoSegment):
             Video segment where a text snippet was
             detected.
         confidence (float):
             Confidence for the track of detected text. It
             is calculated as the highest over all frames
             where OCR detected text appears.
-        frames (Sequence[google.cloud.videointelligence_v1.types.TextFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1.types.TextFrame]):
             Information related to the frames where OCR
             detected text appears.
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    frames = proto.RepeatedField(
+    frames: MutableSequence["TextFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="TextFrame",
     )
 
 
 class TextFrame(proto.Message):
@@ -1513,51 +1531,51 @@
         rotated_bounding_box (google.cloud.videointelligence_v1.types.NormalizedBoundingPoly):
             Bounding polygon of the detected text for
             this frame.
         time_offset (google.protobuf.duration_pb2.Duration):
             Timestamp of this frame.
     """
 
-    rotated_bounding_box = proto.Field(
+    rotated_bounding_box: "NormalizedBoundingPoly" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="NormalizedBoundingPoly",
     )
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class TextAnnotation(proto.Message):
     r"""Annotations related to one detected OCR text snippet. This
     will contain the corresponding text, confidence value, and frame
     level information for each detection.
 
     Attributes:
         text (str):
             The detected text.
-        segments (Sequence[google.cloud.videointelligence_v1.types.TextSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1.types.TextSegment]):
             All video segments where OCR detected text
             appears.
         version (str):
             Feature version.
     """
 
-    text = proto.Field(
+    text: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    segments = proto.RepeatedField(
+    segments: MutableSequence["TextSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="TextSegment",
     )
-    version = proto.Field(
+    version: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class ObjectTrackingFrame(proto.Message):
     r"""Video frame level annotations for object detection and
@@ -1568,20 +1586,20 @@
         normalized_bounding_box (google.cloud.videointelligence_v1.types.NormalizedBoundingBox):
             The normalized bounding box location of this
             object track for the frame.
         time_offset (google.protobuf.duration_pb2.Duration):
             The timestamp of the frame in microseconds.
     """
 
-    normalized_bounding_box = proto.Field(
+    normalized_bounding_box: "NormalizedBoundingBox" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="NormalizedBoundingBox",
     )
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class ObjectTrackingAnnotation(proto.Message):
@@ -1612,87 +1630,87 @@
             This field is a member of `oneof`_ ``track_info``.
         entity (google.cloud.videointelligence_v1.types.Entity):
             Entity to specify the object category that
             this track is labeled as.
         confidence (float):
             Object category's labeling confidence of this
             track.
-        frames (Sequence[google.cloud.videointelligence_v1.types.ObjectTrackingFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1.types.ObjectTrackingFrame]):
             Information corresponding to all frames where
             this object track appears. Non-streaming batch
             mode: it may be one or multiple
             ObjectTrackingFrame messages in frames.
             Streaming mode: it can only be one
             ObjectTrackingFrame message in frames.
         version (str):
             Feature version.
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="track_info",
         message="VideoSegment",
     )
-    track_id = proto.Field(
+    track_id: int = proto.Field(
         proto.INT64,
         number=5,
         oneof="track_info",
     )
-    entity = proto.Field(
+    entity: "Entity" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Entity",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
-    frames = proto.RepeatedField(
+    frames: MutableSequence["ObjectTrackingFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="ObjectTrackingFrame",
     )
-    version = proto.Field(
+    version: str = proto.Field(
         proto.STRING,
         number=6,
     )
 
 
 class LogoRecognitionAnnotation(proto.Message):
     r"""Annotation corresponding to one detected, tracked and
     recognized logo class.
 
     Attributes:
         entity (google.cloud.videointelligence_v1.types.Entity):
             Entity category information to specify the
             logo class that all the logo tracks within this
             LogoRecognitionAnnotation are recognized as.
-        tracks (Sequence[google.cloud.videointelligence_v1.types.Track]):
+        tracks (MutableSequence[google.cloud.videointelligence_v1.types.Track]):
             All logo tracks where the recognized logo
             appears. Each track corresponds to one logo
             instance appearing in consecutive frames.
-        segments (Sequence[google.cloud.videointelligence_v1.types.VideoSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1.types.VideoSegment]):
             All video segments where the recognized logo
             appears. There might be multiple instances of
             the same logo class appearing in one
             VideoSegment.
     """
 
-    entity = proto.Field(
+    entity: "Entity" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Entity",
     )
-    tracks = proto.RepeatedField(
+    tracks: MutableSequence["Track"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="Track",
     )
-    segments = proto.RepeatedField(
+    segments: MutableSequence["VideoSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="VideoSegment",
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.videointelligence import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from .services.video_intelligence_service import (
     VideoIntelligenceServiceAsyncClient,
     VideoIntelligenceServiceClient,
 )
 from .types.video_intelligence import (
     AnnotateVideoProgress,
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/gapic_metadata.json` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/async_client.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,34 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.videointelligence_v1beta2 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
@@ -160,17 +171,17 @@
         type(VideoIntelligenceServiceClient).get_transport_class,
         type(VideoIntelligenceServiceClient),
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, VideoIntelligenceServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the video intelligence service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -206,20 +217,20 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def annotate_video(
         self,
-        request: Union[video_intelligence.AnnotateVideoRequest, dict] = None,
+        request: Optional[Union[video_intelligence.AnnotateVideoRequest, dict]] = None,
         *,
-        input_uri: str = None,
-        features: Sequence[video_intelligence.Feature] = None,
+        input_uri: Optional[str] = None,
+        features: Optional[MutableSequence[video_intelligence.Feature]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Performs asynchronous video annotation. Progress and results can
         be retrieved through the ``google.longrunning.Operations``
         interface. ``Operation.metadata`` contains
         ``AnnotateVideoProgress`` (progress). ``Operation.response``
         contains ``AnnotateVideoResponse`` (results).
@@ -237,29 +248,29 @@
 
             async def sample_annotate_video():
                 # Create a client
                 client = videointelligence_v1beta2.VideoIntelligenceServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = videointelligence_v1beta2.AnnotateVideoRequest(
-                    features="FACE_DETECTION",
+                    features=['FACE_DETECTION'],
                 )
 
                 # Make the request
                 operation = client.annotate_video(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.videointelligence_v1beta2.types.AnnotateVideoRequest, dict]):
+            request (Optional[Union[google.cloud.videointelligence_v1beta2.types.AnnotateVideoRequest, dict]]):
                 The request object. Video annotation request.
             input_uri (:class:`str`):
                 Input video location. Currently, only `Google Cloud
                 Storage <https://cloud.google.com/storage/>`__ URIs are
                 supported, which must be specified in the following
                 format: ``gs://bucket-id/object-id`` (other URI formats
                 return
@@ -272,15 +283,15 @@
                 If unset, the input video should be embedded in the
                 request as ``input_content``. If set, ``input_content``
                 should be unset.
 
                 This corresponds to the ``input_uri`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            features (:class:`Sequence[google.cloud.videointelligence_v1beta2.types.Feature]`):
+            features (:class:`MutableSequence[google.cloud.videointelligence_v1beta2.types.Feature]`):
                 Required. Requested video annotation
                 features.
 
                 This corresponds to the ``features`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -357,18 +368,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("VideoIntelligenceServiceAsyncClient",)
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/client.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,36 +12,48 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.videointelligence_v1p2beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 
-from google.cloud.videointelligence_v1beta2.types import video_intelligence
+from google.cloud.videointelligence_v1p2beta1.types import video_intelligence
 
 from .transports.base import DEFAULT_CLIENT_INFO, VideoIntelligenceServiceTransport
 from .transports.grpc import VideoIntelligenceServiceGrpcTransport
 from .transports.grpc_asyncio import VideoIntelligenceServiceGrpcAsyncIOTransport
 
 
 class VideoIntelligenceServiceClientMeta(type):
@@ -56,15 +68,15 @@
         OrderedDict()
     )  # type: Dict[str, Type[VideoIntelligenceServiceTransport]]
     _transport_registry["grpc"] = VideoIntelligenceServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = VideoIntelligenceServiceGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[VideoIntelligenceServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -309,30 +321,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, VideoIntelligenceServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, VideoIntelligenceServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the video intelligence service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, VideoIntelligenceServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -354,14 +366,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -406,20 +419,20 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def annotate_video(
         self,
-        request: Union[video_intelligence.AnnotateVideoRequest, dict] = None,
+        request: Optional[Union[video_intelligence.AnnotateVideoRequest, dict]] = None,
         *,
-        input_uri: str = None,
-        features: Sequence[video_intelligence.Feature] = None,
+        input_uri: Optional[str] = None,
+        features: Optional[MutableSequence[video_intelligence.Feature]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Performs asynchronous video annotation. Progress and results can
         be retrieved through the ``google.longrunning.Operations``
         interface. ``Operation.metadata`` contains
         ``AnnotateVideoProgress`` (progress). ``Operation.response``
         contains ``AnnotateVideoResponse`` (results).
@@ -429,37 +442,37 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import videointelligence_v1beta2
+            from google.cloud import videointelligence_v1p2beta1
 
             def sample_annotate_video():
                 # Create a client
-                client = videointelligence_v1beta2.VideoIntelligenceServiceClient()
+                client = videointelligence_v1p2beta1.VideoIntelligenceServiceClient()
 
                 # Initialize request argument(s)
-                request = videointelligence_v1beta2.AnnotateVideoRequest(
-                    features="FACE_DETECTION",
+                request = videointelligence_v1p2beta1.AnnotateVideoRequest(
+                    features=['OBJECT_TRACKING'],
                 )
 
                 # Make the request
                 operation = client.annotate_video(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.videointelligence_v1beta2.types.AnnotateVideoRequest, dict]):
+            request (Union[google.cloud.videointelligence_v1p2beta1.types.AnnotateVideoRequest, dict]):
                 The request object. Video annotation request.
             input_uri (str):
                 Input video location. Currently, only `Google Cloud
                 Storage <https://cloud.google.com/storage/>`__ URIs are
                 supported, which must be specified in the following
                 format: ``gs://bucket-id/object-id`` (other URI formats
                 return
@@ -472,15 +485,15 @@
                 If unset, the input video should be embedded in the
                 request as ``input_content``. If set, ``input_content``
                 should be unset.
 
                 This corresponds to the ``input_uri`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            features (Sequence[google.cloud.videointelligence_v1beta2.types.Feature]):
+            features (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.Feature]):
                 Required. Requested video annotation
                 features.
 
                 This corresponds to the ``features`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -489,15 +502,15 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.videointelligence_v1beta2.types.AnnotateVideoResponse` Video annotation response. Included in the response
+                The result type for the operation will be :class:`google.cloud.videointelligence_v1p2beta1.types.AnnotateVideoResponse` Video annotation response. Included in the response
                    field of the Operation returned by the GetOperation
                    call of the google::longrunning::Operations service.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -554,18 +567,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("VideoIntelligenceServiceClient",)
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/base.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,40 +20,35 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1, operations_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
 
-from google.cloud.videointelligence_v1beta2.types import video_intelligence
+from google.cloud.videointelligence_v1 import gapic_version as package_version
+from google.cloud.videointelligence_v1.types import video_intelligence
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class VideoIntelligenceServiceTransport(abc.ABC):
     """Abstract transport class for VideoIntelligenceService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "videointelligence.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/grpc.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 from google.api_core import gapic_v1, grpc_helpers, operations_v1
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 import grpc  # type: ignore
 
-from google.cloud.videointelligence_v1beta2.types import video_intelligence
+from google.cloud.videointelligence_v1p3beta1.types import video_intelligence
 
 from .base import DEFAULT_CLIENT_INFO, VideoIntelligenceServiceTransport
 
 
 class VideoIntelligenceServiceGrpcTransport(VideoIntelligenceServiceTransport):
     """gRPC backend transport for VideoIntelligenceService.
 
-    Service that implements Google Cloud Video Intelligence API.
+    Service that implements the Video Intelligence API.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
@@ -43,22 +43,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -178,16 +178,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
@@ -264,15 +264,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "annotate_video" not in self._stubs:
             self._stubs["annotate_video"] = self.grpc_channel.unary_unary(
-                "/google.cloud.videointelligence.v1beta2.VideoIntelligenceService/AnnotateVideo",
+                "/google.cloud.videointelligence.v1p3beta1.VideoIntelligenceService/AnnotateVideo",
                 request_serializer=video_intelligence.AnnotateVideoRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["annotate_video"]
 
     def close(self):
         self.grpc_channel.close()
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/grpc_asyncio.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/transports/grpc_asyncio.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 from google.api_core import gapic_v1, grpc_helpers_async, operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
-from google.cloud.videointelligence_v1beta2.types import video_intelligence
+from google.cloud.videointelligence_v1.types import video_intelligence
 
 from .base import DEFAULT_CLIENT_INFO, VideoIntelligenceServiceTransport
 from .grpc import VideoIntelligenceServiceGrpcTransport
 
 
 class VideoIntelligenceServiceGrpcAsyncIOTransport(VideoIntelligenceServiceTransport):
     """gRPC AsyncIO backend transport for VideoIntelligenceService.
 
-    Service that implements Google Cloud Video Intelligence API.
+    Service that implements the Video Intelligence API.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
@@ -45,15 +45,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -88,23 +88,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
@@ -271,15 +271,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "annotate_video" not in self._stubs:
             self._stubs["annotate_video"] = self.grpc_channel.unary_unary(
-                "/google.cloud.videointelligence.v1beta2.VideoIntelligenceService/AnnotateVideo",
+                "/google.cloud.videointelligence.v1.VideoIntelligenceService/AnnotateVideo",
                 request_serializer=video_intelligence.AnnotateVideoRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["annotate_video"]
 
     def close(self):
         return self.grpc_channel.close()
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/types/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1beta2/types/video_intelligence.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/types/video_intelligence.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.videointelligence.v1beta2",
@@ -94,15 +96,15 @@
             the input video should be embedded in the request as
             ``input_content``. If set, ``input_content`` should be
             unset.
         input_content (bytes):
             The video data bytes. If unset, the input video(s) should be
             specified via ``input_uri``. If set, ``input_uri`` should be
             unset.
-        features (Sequence[google.cloud.videointelligence_v1beta2.types.Feature]):
+        features (MutableSequence[google.cloud.videointelligence_v1beta2.types.Feature]):
             Required. Requested video annotation
             features.
         video_context (google.cloud.videointelligence_v1beta2.types.VideoContext):
             Additional video context and/or
             feature-specific parameters.
         output_uri (str):
             Optional. Location where the output (in JSON format) should
@@ -116,82 +118,82 @@
         location_id (str):
             Optional. Cloud region where annotation should take place.
             Supported cloud regions: ``us-east1``, ``us-west1``,
             ``europe-west1``, ``asia-east1``. If no region is specified,
             a region will be determined based on video file location.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    input_content = proto.Field(
+    input_content: bytes = proto.Field(
         proto.BYTES,
         number=6,
     )
-    features = proto.RepeatedField(
+    features: MutableSequence["Feature"] = proto.RepeatedField(
         proto.ENUM,
         number=2,
         enum="Feature",
     )
-    video_context = proto.Field(
+    video_context: "VideoContext" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="VideoContext",
     )
-    output_uri = proto.Field(
+    output_uri: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    location_id = proto.Field(
+    location_id: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class VideoContext(proto.Message):
     r"""Video context and/or feature-specific parameters.
 
     Attributes:
-        segments (Sequence[google.cloud.videointelligence_v1beta2.types.VideoSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1beta2.types.VideoSegment]):
             Video segments to annotate. The segments may
             overlap and are not required to be contiguous or
             span the whole video. If unspecified, each video
             is treated as a single segment.
         label_detection_config (google.cloud.videointelligence_v1beta2.types.LabelDetectionConfig):
             Config for LABEL_DETECTION.
         shot_change_detection_config (google.cloud.videointelligence_v1beta2.types.ShotChangeDetectionConfig):
             Config for SHOT_CHANGE_DETECTION.
         explicit_content_detection_config (google.cloud.videointelligence_v1beta2.types.ExplicitContentDetectionConfig):
             Config for EXPLICIT_CONTENT_DETECTION.
         face_detection_config (google.cloud.videointelligence_v1beta2.types.FaceDetectionConfig):
             Config for FACE_DETECTION.
     """
 
-    segments = proto.RepeatedField(
+    segments: MutableSequence["VideoSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    label_detection_config = proto.Field(
+    label_detection_config: "LabelDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="LabelDetectionConfig",
     )
-    shot_change_detection_config = proto.Field(
+    shot_change_detection_config: "ShotChangeDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="ShotChangeDetectionConfig",
     )
-    explicit_content_detection_config = proto.Field(
+    explicit_content_detection_config: "ExplicitContentDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="ExplicitContentDetectionConfig",
     )
-    face_detection_config = proto.Field(
+    face_detection_config: "FaceDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="FaceDetectionConfig",
     )
 
 
 class LabelDetectionConfig(proto.Message):
@@ -209,24 +211,24 @@
             ``SHOT_AND_FRAME_MODE`` enabled.
         model (str):
             Model to use for label detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    label_detection_mode = proto.Field(
+    label_detection_mode: "LabelDetectionMode" = proto.Field(
         proto.ENUM,
         number=1,
         enum="LabelDetectionMode",
     )
-    stationary_camera = proto.Field(
+    stationary_camera: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class ShotChangeDetectionConfig(proto.Message):
     r"""Config for SHOT_CHANGE_DETECTION.
@@ -234,15 +236,15 @@
     Attributes:
         model (str):
             Model to use for shot change detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ExplicitContentDetectionConfig(proto.Message):
     r"""Config for EXPLICIT_CONTENT_DETECTION.
@@ -250,15 +252,15 @@
     Attributes:
         model (str):
             Model to use for explicit content detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class FaceDetectionConfig(proto.Message):
     r"""Config for FACE_DETECTION.
@@ -269,19 +271,19 @@
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
         include_bounding_boxes (bool):
             Whether bounding boxes be included in the
             face annotation output.
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    include_bounding_boxes = proto.Field(
+    include_bounding_boxes: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
 
 
 class VideoSegment(proto.Message):
     r"""Video segment.
@@ -293,20 +295,20 @@
             (inclusive).
         end_time_offset (google.protobuf.duration_pb2.Duration):
             Time-offset, relative to the beginning of the
             video, corresponding to the end of the segment
             (inclusive).
     """
 
-    start_time_offset = proto.Field(
+    start_time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    end_time_offset = proto.Field(
+    end_time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class LabelSegment(proto.Message):
@@ -315,20 +317,20 @@
     Attributes:
         segment (google.cloud.videointelligence_v1beta2.types.VideoSegment):
             Video segment where a label was detected.
         confidence (float):
             Confidence that the label is accurate. Range: [0, 1].
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class LabelFrame(proto.Message):
     r"""Video frame level annotation results for label detection.
@@ -338,20 +340,20 @@
             Time-offset, relative to the beginning of the
             video, corresponding to the video frame for this
             location.
         confidence (float):
             Confidence that the label is accurate. Range: [0, 1].
     """
 
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class Entity(proto.Message):
     r"""Detected entity from video analysis.
@@ -363,62 +365,62 @@
             API <https://developers.google.com/knowledge-graph/>`__.
         description (str):
             Textual description, e.g. ``Fixed-gear bicycle``.
         language_code (str):
             Language code for ``description`` in BCP-47 format.
     """
 
-    entity_id = proto.Field(
+    entity_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class LabelAnnotation(proto.Message):
     r"""Label annotation.
 
     Attributes:
         entity (google.cloud.videointelligence_v1beta2.types.Entity):
             Detected entity.
-        category_entities (Sequence[google.cloud.videointelligence_v1beta2.types.Entity]):
+        category_entities (MutableSequence[google.cloud.videointelligence_v1beta2.types.Entity]):
             Common categories for the detected entity. E.g. when the
             label is ``Terrier`` the category is likely ``dog``. And in
             some cases there might be more than one categories e.g.
             ``Terrier`` could also be a ``pet``.
-        segments (Sequence[google.cloud.videointelligence_v1beta2.types.LabelSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1beta2.types.LabelSegment]):
             All video segments where a label was
             detected.
-        frames (Sequence[google.cloud.videointelligence_v1beta2.types.LabelFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1beta2.types.LabelFrame]):
             All video frames where a label was detected.
     """
 
-    entity = proto.Field(
+    entity: "Entity" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Entity",
     )
-    category_entities = proto.RepeatedField(
+    category_entities: MutableSequence["Entity"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="Entity",
     )
-    segments = proto.RepeatedField(
+    segments: MutableSequence["LabelSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="LabelSegment",
     )
-    frames = proto.RepeatedField(
+    frames: MutableSequence["LabelFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="LabelFrame",
     )
 
 
 class ExplicitContentFrame(proto.Message):
@@ -429,38 +431,38 @@
             Time-offset, relative to the beginning of the
             video, corresponding to the video frame for this
             location.
         pornography_likelihood (google.cloud.videointelligence_v1beta2.types.Likelihood):
             Likelihood of the pornography content..
     """
 
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    pornography_likelihood = proto.Field(
+    pornography_likelihood: "Likelihood" = proto.Field(
         proto.ENUM,
         number=2,
         enum="Likelihood",
     )
 
 
 class ExplicitContentAnnotation(proto.Message):
     r"""Explicit content annotation (based on per-frame visual
     signals only). If no explicit content has been detected in a
     frame, no annotations are present for that frame.
 
     Attributes:
-        frames (Sequence[google.cloud.videointelligence_v1beta2.types.ExplicitContentFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1beta2.types.ExplicitContentFrame]):
             All video frames where explicit content was
             detected.
     """
 
-    frames = proto.RepeatedField(
+    frames: MutableSequence["ExplicitContentFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="ExplicitContentFrame",
     )
 
 
 class NormalizedBoundingBox(proto.Message):
@@ -474,189 +476,191 @@
             Top Y coordinate.
         right (float):
             Right X coordinate.
         bottom (float):
             Bottom Y coordinate.
     """
 
-    left = proto.Field(
+    left: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    top = proto.Field(
+    top: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    right = proto.Field(
+    right: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
-    bottom = proto.Field(
+    bottom: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
 
 
 class FaceSegment(proto.Message):
     r"""Video segment level annotation results for face detection.
 
     Attributes:
         segment (google.cloud.videointelligence_v1beta2.types.VideoSegment):
             Video segment where a face was detected.
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
 
 
 class FaceFrame(proto.Message):
     r"""Video frame level annotation results for face detection.
 
     Attributes:
-        normalized_bounding_boxes (Sequence[google.cloud.videointelligence_v1beta2.types.NormalizedBoundingBox]):
+        normalized_bounding_boxes (MutableSequence[google.cloud.videointelligence_v1beta2.types.NormalizedBoundingBox]):
             Normalized Bounding boxes in a frame.
             There can be more than one boxes if the same
             face is detected in multiple locations within
             the current frame.
         time_offset (google.protobuf.duration_pb2.Duration):
             Time-offset, relative to the beginning of the
             video, corresponding to the video frame for this
             location.
     """
 
-    normalized_bounding_boxes = proto.RepeatedField(
+    normalized_bounding_boxes: MutableSequence[
+        "NormalizedBoundingBox"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="NormalizedBoundingBox",
     )
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class FaceAnnotation(proto.Message):
     r"""Face annotation.
 
     Attributes:
         thumbnail (bytes):
             Thumbnail of a representative face view (in
             JPEG format).
-        segments (Sequence[google.cloud.videointelligence_v1beta2.types.FaceSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1beta2.types.FaceSegment]):
             All video segments where a face was detected.
-        frames (Sequence[google.cloud.videointelligence_v1beta2.types.FaceFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1beta2.types.FaceFrame]):
             All video frames where a face was detected.
     """
 
-    thumbnail = proto.Field(
+    thumbnail: bytes = proto.Field(
         proto.BYTES,
         number=1,
     )
-    segments = proto.RepeatedField(
+    segments: MutableSequence["FaceSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="FaceSegment",
     )
-    frames = proto.RepeatedField(
+    frames: MutableSequence["FaceFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="FaceFrame",
     )
 
 
 class VideoAnnotationResults(proto.Message):
     r"""Annotation results for a single video.
 
     Attributes:
         input_uri (str):
             Video file location in `Google Cloud
             Storage <https://cloud.google.com/storage/>`__.
-        segment_label_annotations (Sequence[google.cloud.videointelligence_v1beta2.types.LabelAnnotation]):
+        segment_label_annotations (MutableSequence[google.cloud.videointelligence_v1beta2.types.LabelAnnotation]):
             Label annotations on video level or user
             specified segment level. There is exactly one
             element for each unique label.
-        shot_label_annotations (Sequence[google.cloud.videointelligence_v1beta2.types.LabelAnnotation]):
+        shot_label_annotations (MutableSequence[google.cloud.videointelligence_v1beta2.types.LabelAnnotation]):
             Label annotations on shot level.
             There is exactly one element for each unique
             label.
-        frame_label_annotations (Sequence[google.cloud.videointelligence_v1beta2.types.LabelAnnotation]):
+        frame_label_annotations (MutableSequence[google.cloud.videointelligence_v1beta2.types.LabelAnnotation]):
             Label annotations on frame level.
             There is exactly one element for each unique
             label.
-        face_annotations (Sequence[google.cloud.videointelligence_v1beta2.types.FaceAnnotation]):
+        face_annotations (MutableSequence[google.cloud.videointelligence_v1beta2.types.FaceAnnotation]):
             Face annotations. There is exactly one
             element for each unique face.
-        shot_annotations (Sequence[google.cloud.videointelligence_v1beta2.types.VideoSegment]):
+        shot_annotations (MutableSequence[google.cloud.videointelligence_v1beta2.types.VideoSegment]):
             Shot annotations. Each shot is represented as
             a video segment.
         explicit_annotation (google.cloud.videointelligence_v1beta2.types.ExplicitContentAnnotation):
             Explicit content annotation.
         error (google.rpc.status_pb2.Status):
             If set, indicates an error. Note that for a single
             ``AnnotateVideoRequest`` some videos may succeed and some
             may fail.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    segment_label_annotations = proto.RepeatedField(
+    segment_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="LabelAnnotation",
     )
-    shot_label_annotations = proto.RepeatedField(
+    shot_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="LabelAnnotation",
     )
-    frame_label_annotations = proto.RepeatedField(
+    frame_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="LabelAnnotation",
     )
-    face_annotations = proto.RepeatedField(
+    face_annotations: MutableSequence["FaceAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=5,
         message="FaceAnnotation",
     )
-    shot_annotations = proto.RepeatedField(
+    shot_annotations: MutableSequence["VideoSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=6,
         message="VideoSegment",
     )
-    explicit_annotation = proto.Field(
+    explicit_annotation: "ExplicitContentAnnotation" = proto.Field(
         proto.MESSAGE,
         number=7,
         message="ExplicitContentAnnotation",
     )
-    error = proto.Field(
+    error: status_pb2.Status = proto.Field(
         proto.MESSAGE,
         number=9,
         message=status_pb2.Status,
     )
 
 
 class AnnotateVideoResponse(proto.Message):
     r"""Video annotation response. Included in the ``response`` field of the
     ``Operation`` returned by the ``GetOperation`` call of the
     ``google::longrunning::Operations`` service.
 
     Attributes:
-        annotation_results (Sequence[google.cloud.videointelligence_v1beta2.types.VideoAnnotationResults]):
+        annotation_results (MutableSequence[google.cloud.videointelligence_v1beta2.types.VideoAnnotationResults]):
             Annotation results for all videos specified in
             ``AnnotateVideoRequest``.
     """
 
-    annotation_results = proto.RepeatedField(
+    annotation_results: MutableSequence["VideoAnnotationResults"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoAnnotationResults",
     )
 
 
 class VideoAnnotationProgress(proto.Message):
@@ -671,46 +675,48 @@
             Guaranteed to be 100 when fully processed.
         start_time (google.protobuf.timestamp_pb2.Timestamp):
             Time when the request was received.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Time of the most recent update.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    progress_percent = proto.Field(
+    progress_percent: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    start_time = proto.Field(
+    start_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class AnnotateVideoProgress(proto.Message):
     r"""Video annotation progress. Included in the ``metadata`` field of the
     ``Operation`` returned by the ``GetOperation`` call of the
     ``google::longrunning::Operations`` service.
 
     Attributes:
-        annotation_progress (Sequence[google.cloud.videointelligence_v1beta2.types.VideoAnnotationProgress]):
+        annotation_progress (MutableSequence[google.cloud.videointelligence_v1beta2.types.VideoAnnotationProgress]):
             Progress metadata for all videos specified in
             ``AnnotateVideoRequest``.
     """
 
-    annotation_progress = proto.RepeatedField(
+    annotation_progress: MutableSequence[
+        "VideoAnnotationProgress"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoAnnotationProgress",
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.videointelligence import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from .services.video_intelligence_service import (
     VideoIntelligenceServiceAsyncClient,
     VideoIntelligenceServiceClient,
 )
 from .types.video_intelligence import (
     AnnotateVideoProgress,
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/gapic_metadata.json` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/async_client.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,33 +12,44 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.videointelligence_v1p2beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 
-from google.cloud.videointelligence_v1p1beta1.types import video_intelligence
+from google.cloud.videointelligence_v1p2beta1.types import video_intelligence
 
 from .client import VideoIntelligenceServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, VideoIntelligenceServiceTransport
 from .transports.grpc_asyncio import VideoIntelligenceServiceGrpcAsyncIOTransport
 
 
 class VideoIntelligenceServiceAsyncClient:
@@ -160,17 +171,17 @@
         type(VideoIntelligenceServiceClient).get_transport_class,
         type(VideoIntelligenceServiceClient),
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, VideoIntelligenceServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the video intelligence service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -206,20 +217,20 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def annotate_video(
         self,
-        request: Union[video_intelligence.AnnotateVideoRequest, dict] = None,
+        request: Optional[Union[video_intelligence.AnnotateVideoRequest, dict]] = None,
         *,
-        input_uri: str = None,
-        features: Sequence[video_intelligence.Feature] = None,
+        input_uri: Optional[str] = None,
+        features: Optional[MutableSequence[video_intelligence.Feature]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Performs asynchronous video annotation. Progress and results can
         be retrieved through the ``google.longrunning.Operations``
         interface. ``Operation.metadata`` contains
         ``AnnotateVideoProgress`` (progress). ``Operation.response``
         contains ``AnnotateVideoResponse`` (results).
@@ -229,37 +240,37 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import videointelligence_v1p1beta1
+            from google.cloud import videointelligence_v1p2beta1
 
             async def sample_annotate_video():
                 # Create a client
-                client = videointelligence_v1p1beta1.VideoIntelligenceServiceAsyncClient()
+                client = videointelligence_v1p2beta1.VideoIntelligenceServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = videointelligence_v1p1beta1.AnnotateVideoRequest(
-                    features="SPEECH_TRANSCRIPTION",
+                request = videointelligence_v1p2beta1.AnnotateVideoRequest(
+                    features=['OBJECT_TRACKING'],
                 )
 
                 # Make the request
                 operation = client.annotate_video(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.videointelligence_v1p1beta1.types.AnnotateVideoRequest, dict]):
+            request (Optional[Union[google.cloud.videointelligence_v1p2beta1.types.AnnotateVideoRequest, dict]]):
                 The request object. Video annotation request.
             input_uri (:class:`str`):
                 Input video location. Currently, only `Google Cloud
                 Storage <https://cloud.google.com/storage/>`__ URIs are
                 supported, which must be specified in the following
                 format: ``gs://bucket-id/object-id`` (other URI formats
                 return
@@ -272,15 +283,15 @@
                 If unset, the input video should be embedded in the
                 request as ``input_content``. If set, ``input_content``
                 should be unset.
 
                 This corresponds to the ``input_uri`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            features (:class:`Sequence[google.cloud.videointelligence_v1p1beta1.types.Feature]`):
+            features (:class:`MutableSequence[google.cloud.videointelligence_v1p2beta1.types.Feature]`):
                 Required. Requested video annotation
                 features.
 
                 This corresponds to the ``features`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -289,15 +300,15 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.videointelligence_v1p1beta1.types.AnnotateVideoResponse` Video annotation response. Included in the response
+                The result type for the operation will be :class:`google.cloud.videointelligence_v1p2beta1.types.AnnotateVideoResponse` Video annotation response. Included in the response
                    field of the Operation returned by the GetOperation
                    call of the google::longrunning::Operations service.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -357,18 +368,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("VideoIntelligenceServiceAsyncClient",)
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/client.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1/services/video_intelligence_service/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,36 +12,48 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.videointelligence_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 
-from google.cloud.videointelligence_v1p1beta1.types import video_intelligence
+from google.cloud.videointelligence_v1.types import video_intelligence
 
 from .transports.base import DEFAULT_CLIENT_INFO, VideoIntelligenceServiceTransport
 from .transports.grpc import VideoIntelligenceServiceGrpcTransport
 from .transports.grpc_asyncio import VideoIntelligenceServiceGrpcAsyncIOTransport
 
 
 class VideoIntelligenceServiceClientMeta(type):
@@ -56,15 +68,15 @@
         OrderedDict()
     )  # type: Dict[str, Type[VideoIntelligenceServiceTransport]]
     _transport_registry["grpc"] = VideoIntelligenceServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = VideoIntelligenceServiceGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[VideoIntelligenceServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -77,15 +89,15 @@
 
         # No transport is requested; return the default (that is, the first one
         # in the dictionary).
         return next(iter(cls._transport_registry.values()))
 
 
 class VideoIntelligenceServiceClient(metaclass=VideoIntelligenceServiceClientMeta):
-    """Service that implements Google Cloud Video Intelligence API."""
+    """Service that implements the Video Intelligence API."""
 
     @staticmethod
     def _get_default_mtls_endpoint(api_endpoint):
         """Converts api endpoint to mTLS endpoint.
 
         Convert "*.sandbox.googleapis.com" and "*.googleapis.com" to
         "*.mtls.sandbox.googleapis.com" and "*.mtls.googleapis.com" respectively.
@@ -309,30 +321,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, VideoIntelligenceServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, VideoIntelligenceServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the video intelligence service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, VideoIntelligenceServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -354,14 +366,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -406,20 +419,20 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def annotate_video(
         self,
-        request: Union[video_intelligence.AnnotateVideoRequest, dict] = None,
+        request: Optional[Union[video_intelligence.AnnotateVideoRequest, dict]] = None,
         *,
-        input_uri: str = None,
-        features: Sequence[video_intelligence.Feature] = None,
+        input_uri: Optional[str] = None,
+        features: Optional[MutableSequence[video_intelligence.Feature]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Performs asynchronous video annotation. Progress and results can
         be retrieved through the ``google.longrunning.Operations``
         interface. ``Operation.metadata`` contains
         ``AnnotateVideoProgress`` (progress). ``Operation.response``
         contains ``AnnotateVideoResponse`` (results).
@@ -429,58 +442,58 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import videointelligence_v1p1beta1
+            from google.cloud import videointelligence_v1
 
             def sample_annotate_video():
                 # Create a client
-                client = videointelligence_v1p1beta1.VideoIntelligenceServiceClient()
+                client = videointelligence_v1.VideoIntelligenceServiceClient()
 
                 # Initialize request argument(s)
-                request = videointelligence_v1p1beta1.AnnotateVideoRequest(
-                    features="SPEECH_TRANSCRIPTION",
+                request = videointelligence_v1.AnnotateVideoRequest(
+                    features=['PERSON_DETECTION'],
                 )
 
                 # Make the request
                 operation = client.annotate_video(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.videointelligence_v1p1beta1.types.AnnotateVideoRequest, dict]):
+            request (Union[google.cloud.videointelligence_v1.types.AnnotateVideoRequest, dict]):
                 The request object. Video annotation request.
             input_uri (str):
-                Input video location. Currently, only `Google Cloud
+                Input video location. Currently, only `Cloud
                 Storage <https://cloud.google.com/storage/>`__ URIs are
-                supported, which must be specified in the following
+                supported. URIs must be specified in the following
                 format: ``gs://bucket-id/object-id`` (other URI formats
                 return
                 [google.rpc.Code.INVALID_ARGUMENT][google.rpc.Code.INVALID_ARGUMENT]).
                 For more information, see `Request
                 URIs <https://cloud.google.com/storage/docs/request-endpoints>`__.
-                A video URI may include wildcards in ``object-id``, and
-                thus identify multiple videos. Supported wildcards: '*'
+                To identify multiple videos, a video URI may include
+                wildcards in the ``object-id``. Supported wildcards: '*'
                 to match 0 or more characters; '?' to match 1 character.
                 If unset, the input video should be embedded in the
                 request as ``input_content``. If set, ``input_content``
-                should be unset.
+                must be unset.
 
                 This corresponds to the ``input_uri`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            features (Sequence[google.cloud.videointelligence_v1p1beta1.types.Feature]):
+            features (MutableSequence[google.cloud.videointelligence_v1.types.Feature]):
                 Required. Requested video annotation
                 features.
 
                 This corresponds to the ``features`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -489,15 +502,15 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.videointelligence_v1p1beta1.types.AnnotateVideoResponse` Video annotation response. Included in the response
+                The result type for the operation will be :class:`google.cloud.videointelligence_v1.types.AnnotateVideoResponse` Video annotation response. Included in the response
                    field of the Operation returned by the GetOperation
                    call of the google::longrunning::Operations service.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -554,18 +567,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("VideoIntelligenceServiceClient",)
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/base.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,40 +20,35 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1, operations_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
 
-from google.cloud.videointelligence_v1p1beta1.types import video_intelligence
+from google.cloud.videointelligence_v1beta2 import gapic_version as package_version
+from google.cloud.videointelligence_v1beta2.types import video_intelligence
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class VideoIntelligenceServiceTransport(abc.ABC):
     """Abstract transport class for VideoIntelligenceService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "videointelligence.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/grpc.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/grpc_asyncio.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,56 +9,101 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
-from google.api_core import gapic_v1, grpc_helpers, operations_v1
-import google.auth  # type: ignore
+from google.api_core import gapic_v1, grpc_helpers_async, operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 import grpc  # type: ignore
+from grpc.experimental import aio  # type: ignore
 
-from google.cloud.videointelligence_v1p1beta1.types import video_intelligence
+from google.cloud.videointelligence_v1beta2.types import video_intelligence
 
 from .base import DEFAULT_CLIENT_INFO, VideoIntelligenceServiceTransport
+from .grpc import VideoIntelligenceServiceGrpcTransport
 
 
-class VideoIntelligenceServiceGrpcTransport(VideoIntelligenceServiceTransport):
-    """gRPC backend transport for VideoIntelligenceService.
+class VideoIntelligenceServiceGrpcAsyncIOTransport(VideoIntelligenceServiceTransport):
+    """gRPC AsyncIO backend transport for VideoIntelligenceService.
 
     Service that implements Google Cloud Video Intelligence API.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
     """
 
-    _stubs: Dict[str, Callable]
+    _grpc_channel: aio.Channel
+    _stubs: Dict[str, Callable] = {}
+
+    @classmethod
+    def create_channel(
+        cls,
+        host: str = "videointelligence.googleapis.com",
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        quota_project_id: Optional[str] = None,
+        **kwargs,
+    ) -> aio.Channel:
+        """Create and return a gRPC AsyncIO channel object.
+        Args:
+            host (Optional[str]): The host for the channel to use.
+            credentials (Optional[~.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify this application to the service. If
+                none are specified, the client will attempt to ascertain
+                the credentials from the environment.
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is ignored if ``channel`` is provided.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            kwargs (Optional[dict]): Keyword arguments, which are passed to the
+                channel creation.
+        Returns:
+            aio.Channel: A gRPC AsyncIO channel object.
+        """
+
+        return grpc_helpers_async.create_channel(
+            host,
+            credentials=credentials,
+            credentials_file=credentials_file,
+            quota_project_id=quota_project_id,
+            default_scopes=cls.AUTH_SCOPES,
+            scopes=scopes,
+            default_host=cls.DEFAULT_HOST,
+            **kwargs,
+        )
 
     def __init__(
         self,
         *,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -70,17 +115,18 @@
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
                 This argument is ignored if ``channel`` is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
                 This argument is ignored if ``channel`` is provided.
-            scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                ignored if ``channel`` is provided.
-            channel (Optional[grpc.Channel]): A ``Channel`` instance through
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            channel (Optional[aio.Channel]): A ``Channel`` instance through
                 which to make calls.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
@@ -99,36 +145,35 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
 
         Raises:
-          google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
+            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
               creation failed for any reason.
           google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
               and ``credentials_file`` are passed.
         """
         self._grpc_channel = None
         self._ssl_channel_credentials = ssl_channel_credentials
         self._stubs: Dict[str, Callable] = {}
-        self._operations_client: Optional[operations_v1.OperationsClient] = None
+        self._operations_client: Optional[operations_v1.OperationsAsyncClient] = None
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
         if channel:
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
-
         else:
             if api_mtls_endpoint:
                 host = api_mtls_endpoint
 
                 # Create SSL credentials with client_cert_source or application
                 # default SSL credentials.
                 if client_cert_source:
@@ -174,112 +219,70 @@
                     ("grpc.max_receive_message_length", -1),
                 ],
             )
 
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
-    @classmethod
-    def create_channel(
-        cls,
-        host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Optional[Sequence[str]] = None,
-        quota_project_id: Optional[str] = None,
-        **kwargs,
-    ) -> grpc.Channel:
-        """Create and return a gRPC channel object.
-        Args:
-            host (Optional[str]): The host for the channel to use.
-            credentials (Optional[~.Credentials]): The
-                authorization credentials to attach to requests. These
-                credentials identify this application to the service. If
-                none are specified, the client will attempt to ascertain
-                the credentials from the environment.
-            credentials_file (Optional[str]): A file with credentials that can
-                be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is mutually exclusive with credentials.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            quota_project_id (Optional[str]): An optional project to use for billing
-                and quota.
-            kwargs (Optional[dict]): Keyword arguments, which are passed to the
-                channel creation.
-        Returns:
-            grpc.Channel: A gRPC channel object.
+    @property
+    def grpc_channel(self) -> aio.Channel:
+        """Create the channel designed to connect to this service.
 
-        Raises:
-            google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
-              and ``credentials_file`` are passed.
+        This property caches on the instance; repeated calls return
+        the same channel.
         """
-
-        return grpc_helpers.create_channel(
-            host,
-            credentials=credentials,
-            credentials_file=credentials_file,
-            quota_project_id=quota_project_id,
-            default_scopes=cls.AUTH_SCOPES,
-            scopes=scopes,
-            default_host=cls.DEFAULT_HOST,
-            **kwargs,
-        )
-
-    @property
-    def grpc_channel(self) -> grpc.Channel:
-        """Return the channel designed to connect to this service."""
+        # Return the channel from cache.
         return self._grpc_channel
 
     @property
-    def operations_client(self) -> operations_v1.OperationsClient:
+    def operations_client(self) -> operations_v1.OperationsAsyncClient:
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
         # Quick check: Only create a new client if we do not already have one.
         if self._operations_client is None:
-            self._operations_client = operations_v1.OperationsClient(self.grpc_channel)
+            self._operations_client = operations_v1.OperationsAsyncClient(
+                self.grpc_channel
+            )
 
         # Return the client from cache.
         return self._operations_client
 
     @property
     def annotate_video(
         self,
-    ) -> Callable[[video_intelligence.AnnotateVideoRequest], operations_pb2.Operation]:
+    ) -> Callable[
+        [video_intelligence.AnnotateVideoRequest], Awaitable[operations_pb2.Operation]
+    ]:
         r"""Return a callable for the annotate video method over gRPC.
 
         Performs asynchronous video annotation. Progress and results can
         be retrieved through the ``google.longrunning.Operations``
         interface. ``Operation.metadata`` contains
         ``AnnotateVideoProgress`` (progress). ``Operation.response``
         contains ``AnnotateVideoResponse`` (results).
 
         Returns:
             Callable[[~.AnnotateVideoRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "annotate_video" not in self._stubs:
             self._stubs["annotate_video"] = self.grpc_channel.unary_unary(
-                "/google.cloud.videointelligence.v1p1beta1.VideoIntelligenceService/AnnotateVideo",
+                "/google.cloud.videointelligence.v1beta2.VideoIntelligenceService/AnnotateVideo",
                 request_serializer=video_intelligence.AnnotateVideoRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["annotate_video"]
 
     def close(self):
-        self.grpc_channel.close()
-
-    @property
-    def kind(self) -> str:
-        return "grpc"
+        return self.grpc_channel.close()
 
 
-__all__ = ("VideoIntelligenceServiceGrpcTransport",)
+__all__ = ("VideoIntelligenceServiceGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/grpc_asyncio.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/grpc_asyncio.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -88,23 +88,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/types/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p1beta1/types/video_intelligence.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/types/video_intelligence.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.videointelligence.v1p1beta1",
@@ -94,15 +96,15 @@
             the input video should be embedded in the request as
             ``input_content``. If set, ``input_content`` should be
             unset.
         input_content (bytes):
             The video data bytes. If unset, the input video(s) should be
             specified via ``input_uri``. If set, ``input_uri`` should be
             unset.
-        features (Sequence[google.cloud.videointelligence_v1p1beta1.types.Feature]):
+        features (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.Feature]):
             Required. Requested video annotation
             features.
         video_context (google.cloud.videointelligence_v1p1beta1.types.VideoContext):
             Additional video context and/or
             feature-specific parameters.
         output_uri (str):
             Optional. Location where the output (in JSON format) should
@@ -116,82 +118,82 @@
         location_id (str):
             Optional. Cloud region where annotation should take place.
             Supported cloud regions: ``us-east1``, ``us-west1``,
             ``europe-west1``, ``asia-east1``. If no region is specified,
             a region will be determined based on video file location.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    input_content = proto.Field(
+    input_content: bytes = proto.Field(
         proto.BYTES,
         number=6,
     )
-    features = proto.RepeatedField(
+    features: MutableSequence["Feature"] = proto.RepeatedField(
         proto.ENUM,
         number=2,
         enum="Feature",
     )
-    video_context = proto.Field(
+    video_context: "VideoContext" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="VideoContext",
     )
-    output_uri = proto.Field(
+    output_uri: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    location_id = proto.Field(
+    location_id: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class VideoContext(proto.Message):
     r"""Video context and/or feature-specific parameters.
 
     Attributes:
-        segments (Sequence[google.cloud.videointelligence_v1p1beta1.types.VideoSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.VideoSegment]):
             Video segments to annotate. The segments may
             overlap and are not required to be contiguous or
             span the whole video. If unspecified, each video
             is treated as a single segment.
         label_detection_config (google.cloud.videointelligence_v1p1beta1.types.LabelDetectionConfig):
             Config for LABEL_DETECTION.
         shot_change_detection_config (google.cloud.videointelligence_v1p1beta1.types.ShotChangeDetectionConfig):
             Config for SHOT_CHANGE_DETECTION.
         explicit_content_detection_config (google.cloud.videointelligence_v1p1beta1.types.ExplicitContentDetectionConfig):
             Config for EXPLICIT_CONTENT_DETECTION.
         speech_transcription_config (google.cloud.videointelligence_v1p1beta1.types.SpeechTranscriptionConfig):
             Config for SPEECH_TRANSCRIPTION.
     """
 
-    segments = proto.RepeatedField(
+    segments: MutableSequence["VideoSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    label_detection_config = proto.Field(
+    label_detection_config: "LabelDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="LabelDetectionConfig",
     )
-    shot_change_detection_config = proto.Field(
+    shot_change_detection_config: "ShotChangeDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="ShotChangeDetectionConfig",
     )
-    explicit_content_detection_config = proto.Field(
+    explicit_content_detection_config: "ExplicitContentDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="ExplicitContentDetectionConfig",
     )
-    speech_transcription_config = proto.Field(
+    speech_transcription_config: "SpeechTranscriptionConfig" = proto.Field(
         proto.MESSAGE,
         number=6,
         message="SpeechTranscriptionConfig",
     )
 
 
 class LabelDetectionConfig(proto.Message):
@@ -209,24 +211,24 @@
             ``SHOT_AND_FRAME_MODE`` enabled.
         model (str):
             Model to use for label detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    label_detection_mode = proto.Field(
+    label_detection_mode: "LabelDetectionMode" = proto.Field(
         proto.ENUM,
         number=1,
         enum="LabelDetectionMode",
     )
-    stationary_camera = proto.Field(
+    stationary_camera: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class ShotChangeDetectionConfig(proto.Message):
     r"""Config for SHOT_CHANGE_DETECTION.
@@ -234,15 +236,15 @@
     Attributes:
         model (str):
             Model to use for shot change detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ExplicitContentDetectionConfig(proto.Message):
     r"""Config for EXPLICIT_CONTENT_DETECTION.
@@ -250,15 +252,15 @@
     Attributes:
         model (str):
             Model to use for explicit content detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class VideoSegment(proto.Message):
     r"""Video segment.
@@ -270,20 +272,20 @@
             (inclusive).
         end_time_offset (google.protobuf.duration_pb2.Duration):
             Time-offset, relative to the beginning of the
             video, corresponding to the end of the segment
             (inclusive).
     """
 
-    start_time_offset = proto.Field(
+    start_time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    end_time_offset = proto.Field(
+    end_time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class LabelSegment(proto.Message):
@@ -292,20 +294,20 @@
     Attributes:
         segment (google.cloud.videointelligence_v1p1beta1.types.VideoSegment):
             Video segment where a label was detected.
         confidence (float):
             Confidence that the label is accurate. Range: [0, 1].
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class LabelFrame(proto.Message):
     r"""Video frame level annotation results for label detection.
@@ -315,20 +317,20 @@
             Time-offset, relative to the beginning of the
             video, corresponding to the video frame for this
             location.
         confidence (float):
             Confidence that the label is accurate. Range: [0, 1].
     """
 
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class Entity(proto.Message):
     r"""Detected entity from video analysis.
@@ -340,62 +342,62 @@
             API <https://developers.google.com/knowledge-graph/>`__.
         description (str):
             Textual description, e.g. ``Fixed-gear bicycle``.
         language_code (str):
             Language code for ``description`` in BCP-47 format.
     """
 
-    entity_id = proto.Field(
+    entity_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class LabelAnnotation(proto.Message):
     r"""Label annotation.
 
     Attributes:
         entity (google.cloud.videointelligence_v1p1beta1.types.Entity):
             Detected entity.
-        category_entities (Sequence[google.cloud.videointelligence_v1p1beta1.types.Entity]):
+        category_entities (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.Entity]):
             Common categories for the detected entity. E.g. when the
             label is ``Terrier`` the category is likely ``dog``. And in
             some cases there might be more than one categories e.g.
             ``Terrier`` could also be a ``pet``.
-        segments (Sequence[google.cloud.videointelligence_v1p1beta1.types.LabelSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.LabelSegment]):
             All video segments where a label was
             detected.
-        frames (Sequence[google.cloud.videointelligence_v1p1beta1.types.LabelFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.LabelFrame]):
             All video frames where a label was detected.
     """
 
-    entity = proto.Field(
+    entity: "Entity" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Entity",
     )
-    category_entities = proto.RepeatedField(
+    category_entities: MutableSequence["Entity"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="Entity",
     )
-    segments = proto.RepeatedField(
+    segments: MutableSequence["LabelSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="LabelSegment",
     )
-    frames = proto.RepeatedField(
+    frames: MutableSequence["LabelFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="LabelFrame",
     )
 
 
 class ExplicitContentFrame(proto.Message):
@@ -406,129 +408,129 @@
             Time-offset, relative to the beginning of the
             video, corresponding to the video frame for this
             location.
         pornography_likelihood (google.cloud.videointelligence_v1p1beta1.types.Likelihood):
             Likelihood of the pornography content..
     """
 
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    pornography_likelihood = proto.Field(
+    pornography_likelihood: "Likelihood" = proto.Field(
         proto.ENUM,
         number=2,
         enum="Likelihood",
     )
 
 
 class ExplicitContentAnnotation(proto.Message):
     r"""Explicit content annotation (based on per-frame visual
     signals only). If no explicit content has been detected in a
     frame, no annotations are present for that frame.
 
     Attributes:
-        frames (Sequence[google.cloud.videointelligence_v1p1beta1.types.ExplicitContentFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.ExplicitContentFrame]):
             All video frames where explicit content was
             detected.
     """
 
-    frames = proto.RepeatedField(
+    frames: MutableSequence["ExplicitContentFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="ExplicitContentFrame",
     )
 
 
 class VideoAnnotationResults(proto.Message):
     r"""Annotation results for a single video.
 
     Attributes:
         input_uri (str):
             Output only. Video file location in `Google Cloud
             Storage <https://cloud.google.com/storage/>`__.
-        segment_label_annotations (Sequence[google.cloud.videointelligence_v1p1beta1.types.LabelAnnotation]):
+        segment_label_annotations (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.LabelAnnotation]):
             Label annotations on video level or user
             specified segment level. There is exactly one
             element for each unique label.
-        shot_label_annotations (Sequence[google.cloud.videointelligence_v1p1beta1.types.LabelAnnotation]):
+        shot_label_annotations (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.LabelAnnotation]):
             Label annotations on shot level.
             There is exactly one element for each unique
             label.
-        frame_label_annotations (Sequence[google.cloud.videointelligence_v1p1beta1.types.LabelAnnotation]):
+        frame_label_annotations (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.LabelAnnotation]):
             Label annotations on frame level.
             There is exactly one element for each unique
             label.
-        shot_annotations (Sequence[google.cloud.videointelligence_v1p1beta1.types.VideoSegment]):
+        shot_annotations (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.VideoSegment]):
             Shot annotations. Each shot is represented as
             a video segment.
         explicit_annotation (google.cloud.videointelligence_v1p1beta1.types.ExplicitContentAnnotation):
             Explicit content annotation.
-        speech_transcriptions (Sequence[google.cloud.videointelligence_v1p1beta1.types.SpeechTranscription]):
+        speech_transcriptions (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.SpeechTranscription]):
             Speech transcription.
         error (google.rpc.status_pb2.Status):
             Output only. If set, indicates an error. Note that for a
             single ``AnnotateVideoRequest`` some videos may succeed and
             some may fail.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    segment_label_annotations = proto.RepeatedField(
+    segment_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="LabelAnnotation",
     )
-    shot_label_annotations = proto.RepeatedField(
+    shot_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="LabelAnnotation",
     )
-    frame_label_annotations = proto.RepeatedField(
+    frame_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="LabelAnnotation",
     )
-    shot_annotations = proto.RepeatedField(
+    shot_annotations: MutableSequence["VideoSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=6,
         message="VideoSegment",
     )
-    explicit_annotation = proto.Field(
+    explicit_annotation: "ExplicitContentAnnotation" = proto.Field(
         proto.MESSAGE,
         number=7,
         message="ExplicitContentAnnotation",
     )
-    speech_transcriptions = proto.RepeatedField(
+    speech_transcriptions: MutableSequence["SpeechTranscription"] = proto.RepeatedField(
         proto.MESSAGE,
         number=11,
         message="SpeechTranscription",
     )
-    error = proto.Field(
+    error: status_pb2.Status = proto.Field(
         proto.MESSAGE,
         number=9,
         message=status_pb2.Status,
     )
 
 
 class AnnotateVideoResponse(proto.Message):
     r"""Video annotation response. Included in the ``response`` field of the
     ``Operation`` returned by the ``GetOperation`` call of the
     ``google::longrunning::Operations`` service.
 
     Attributes:
-        annotation_results (Sequence[google.cloud.videointelligence_v1p1beta1.types.VideoAnnotationResults]):
+        annotation_results (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.VideoAnnotationResults]):
             Annotation results for all videos specified in
             ``AnnotateVideoRequest``.
     """
 
-    annotation_results = proto.RepeatedField(
+    annotation_results: MutableSequence["VideoAnnotationResults"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoAnnotationResults",
     )
 
 
 class VideoAnnotationProgress(proto.Message):
@@ -545,46 +547,48 @@
         start_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time when the request was
             received.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time of the most recent update.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    progress_percent = proto.Field(
+    progress_percent: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    start_time = proto.Field(
+    start_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class AnnotateVideoProgress(proto.Message):
     r"""Video annotation progress. Included in the ``metadata`` field of the
     ``Operation`` returned by the ``GetOperation`` call of the
     ``google::longrunning::Operations`` service.
 
     Attributes:
-        annotation_progress (Sequence[google.cloud.videointelligence_v1p1beta1.types.VideoAnnotationProgress]):
+        annotation_progress (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.VideoAnnotationProgress]):
             Progress metadata for all videos specified in
             ``AnnotateVideoRequest``.
     """
 
-    annotation_progress = proto.RepeatedField(
+    annotation_progress: MutableSequence[
+        "VideoAnnotationProgress"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoAnnotationProgress",
     )
 
 
 class SpeechTranscriptionConfig(proto.Message):
@@ -607,97 +611,97 @@
             will return a maximum of one.
         filter_profanity (bool):
             Optional. If set to ``true``, the server will attempt to
             filter out profanities, replacing all but the initial
             character in each filtered word with asterisks, e.g. "f***".
             If set to ``false`` or omitted, profanities won't be
             filtered out.
-        speech_contexts (Sequence[google.cloud.videointelligence_v1p1beta1.types.SpeechContext]):
+        speech_contexts (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.SpeechContext]):
             Optional. A means to provide context to
             assist the speech recognition.
         enable_automatic_punctuation (bool):
             Optional. If 'true', adds punctuation to
             recognition result hypotheses. This feature is
             only available in select languages. Setting this
             for requests in other languages has no effect at
             all. The default 'false' value does not add
             punctuation to result hypotheses. NOTE: "This is
             currently offered as an experimental service,
             complimentary to all users. In the future this
             may be exclusively available as a premium
             feature.".
-        audio_tracks (Sequence[int]):
+        audio_tracks (MutableSequence[int]):
             Optional. For file formats, such as MXF or
             MKV, supporting multiple audio tracks, specify
             up to two tracks. Default: track 0.
     """
 
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    max_alternatives = proto.Field(
+    max_alternatives: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    filter_profanity = proto.Field(
+    filter_profanity: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
-    speech_contexts = proto.RepeatedField(
+    speech_contexts: MutableSequence["SpeechContext"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="SpeechContext",
     )
-    enable_automatic_punctuation = proto.Field(
+    enable_automatic_punctuation: bool = proto.Field(
         proto.BOOL,
         number=5,
     )
-    audio_tracks = proto.RepeatedField(
+    audio_tracks: MutableSequence[int] = proto.RepeatedField(
         proto.INT32,
         number=6,
     )
 
 
 class SpeechContext(proto.Message):
     r"""Provides "hints" to the speech recognizer to favor specific
     words and phrases in the results.
 
     Attributes:
-        phrases (Sequence[str]):
+        phrases (MutableSequence[str]):
             Optional. A list of strings containing words and phrases
             "hints" so that the speech recognition is more likely to
             recognize them. This can be used to improve the accuracy for
             specific words and phrases, for example, if specific
             commands are typically spoken by the user. This can also be
             used to add additional words to the vocabulary of the
             recognizer. See `usage
             limits <https://cloud.google.com/speech/limits#content>`__.
     """
 
-    phrases = proto.RepeatedField(
+    phrases: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=1,
     )
 
 
 class SpeechTranscription(proto.Message):
     r"""A speech recognition result corresponding to a portion of the
     audio.
 
     Attributes:
-        alternatives (Sequence[google.cloud.videointelligence_v1p1beta1.types.SpeechRecognitionAlternative]):
+        alternatives (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.SpeechRecognitionAlternative]):
             May contain one or more recognition hypotheses (up to the
             maximum specified in ``max_alternatives``). These
             alternatives are ordered in terms of accuracy, with the top
             (first) alternative being the most probable, as ranked by
             the recognizer.
     """
 
-    alternatives = proto.RepeatedField(
+    alternatives: MutableSequence["SpeechRecognitionAlternative"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="SpeechRecognitionAlternative",
     )
 
 
 class SpeechRecognitionAlternative(proto.Message):
@@ -711,28 +715,28 @@
             Output only. The confidence estimate between 0.0 and 1.0. A
             higher number indicates an estimated greater likelihood that
             the recognized words are correct. This field is set only for
             the top alternative. This field is not guaranteed to be
             accurate and users should not rely on it to be always
             provided. The default of 0.0 is a sentinel value indicating
             ``confidence`` was not set.
-        words (Sequence[google.cloud.videointelligence_v1p1beta1.types.WordInfo]):
+        words (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.WordInfo]):
             Output only. A list of word-specific
             information for each recognized word.
     """
 
-    transcript = proto.Field(
+    transcript: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    words = proto.RepeatedField(
+    words: MutableSequence["WordInfo"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="WordInfo",
     )
 
 
 class WordInfo(proto.Message):
@@ -754,24 +758,24 @@
             only in the top hypothesis. This is an experimental feature
             and the accuracy of the time offset can vary.
         word (str):
             Output only. The word corresponding to this
             set of information.
     """
 
-    start_time = proto.Field(
+    start_time: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    end_time = proto.Field(
+    end_time: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
-    word = proto.Field(
+    word: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.videointelligence import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from .services.video_intelligence_service import (
     VideoIntelligenceServiceAsyncClient,
     VideoIntelligenceServiceClient,
 )
 from .types.video_intelligence import (
     AnnotateVideoProgress,
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/gapic_metadata.json` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/async_client.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,41 +12,52 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.videointelligence_v1p3beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 
-from google.cloud.videointelligence_v1p2beta1.types import video_intelligence
+from google.cloud.videointelligence_v1p3beta1.types import video_intelligence
 
 from .client import VideoIntelligenceServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, VideoIntelligenceServiceTransport
 from .transports.grpc_asyncio import VideoIntelligenceServiceGrpcAsyncIOTransport
 
 
 class VideoIntelligenceServiceAsyncClient:
-    """Service that implements Google Cloud Video Intelligence API."""
+    """Service that implements the Video Intelligence API."""
 
     _client: VideoIntelligenceServiceClient
 
     DEFAULT_ENDPOINT = VideoIntelligenceServiceClient.DEFAULT_ENDPOINT
     DEFAULT_MTLS_ENDPOINT = VideoIntelligenceServiceClient.DEFAULT_MTLS_ENDPOINT
 
     common_billing_account_path = staticmethod(
@@ -160,17 +171,17 @@
         type(VideoIntelligenceServiceClient).get_transport_class,
         type(VideoIntelligenceServiceClient),
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, VideoIntelligenceServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the video intelligence service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -206,20 +217,20 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def annotate_video(
         self,
-        request: Union[video_intelligence.AnnotateVideoRequest, dict] = None,
+        request: Optional[Union[video_intelligence.AnnotateVideoRequest, dict]] = None,
         *,
-        input_uri: str = None,
-        features: Sequence[video_intelligence.Feature] = None,
+        input_uri: Optional[str] = None,
+        features: Optional[MutableSequence[video_intelligence.Feature]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Performs asynchronous video annotation. Progress and results can
         be retrieved through the ``google.longrunning.Operations``
         interface. ``Operation.metadata`` contains
         ``AnnotateVideoProgress`` (progress). ``Operation.response``
         contains ``AnnotateVideoResponse`` (results).
@@ -229,58 +240,58 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import videointelligence_v1p2beta1
+            from google.cloud import videointelligence_v1p3beta1
 
             async def sample_annotate_video():
                 # Create a client
-                client = videointelligence_v1p2beta1.VideoIntelligenceServiceAsyncClient()
+                client = videointelligence_v1p3beta1.VideoIntelligenceServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = videointelligence_v1p2beta1.AnnotateVideoRequest(
-                    features="OBJECT_TRACKING",
+                request = videointelligence_v1p3beta1.AnnotateVideoRequest(
+                    features=['PERSON_DETECTION'],
                 )
 
                 # Make the request
                 operation = client.annotate_video(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.videointelligence_v1p2beta1.types.AnnotateVideoRequest, dict]):
+            request (Optional[Union[google.cloud.videointelligence_v1p3beta1.types.AnnotateVideoRequest, dict]]):
                 The request object. Video annotation request.
             input_uri (:class:`str`):
-                Input video location. Currently, only `Google Cloud
+                Input video location. Currently, only `Cloud
                 Storage <https://cloud.google.com/storage/>`__ URIs are
-                supported, which must be specified in the following
+                supported. URIs must be specified in the following
                 format: ``gs://bucket-id/object-id`` (other URI formats
                 return
                 [google.rpc.Code.INVALID_ARGUMENT][google.rpc.Code.INVALID_ARGUMENT]).
                 For more information, see `Request
                 URIs <https://cloud.google.com/storage/docs/request-endpoints>`__.
-                A video URI may include wildcards in ``object-id``, and
-                thus identify multiple videos. Supported wildcards: '*'
+                To identify multiple videos, a video URI may include
+                wildcards in the ``object-id``. Supported wildcards: '*'
                 to match 0 or more characters; '?' to match 1 character.
                 If unset, the input video should be embedded in the
                 request as ``input_content``. If set, ``input_content``
-                should be unset.
+                must be unset.
 
                 This corresponds to the ``input_uri`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            features (:class:`Sequence[google.cloud.videointelligence_v1p2beta1.types.Feature]`):
+            features (:class:`MutableSequence[google.cloud.videointelligence_v1p3beta1.types.Feature]`):
                 Required. Requested video annotation
                 features.
 
                 This corresponds to the ``features`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -289,15 +300,15 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.videointelligence_v1p2beta1.types.AnnotateVideoResponse` Video annotation response. Included in the response
+                The result type for the operation will be :class:`google.cloud.videointelligence_v1p3beta1.types.AnnotateVideoResponse` Video annotation response. Included in the response
                    field of the Operation returned by the GetOperation
                    call of the google::longrunning::Operations service.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -357,18 +368,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("VideoIntelligenceServiceAsyncClient",)
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/client.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,36 +12,48 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.videointelligence_v1p3beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 
-from google.cloud.videointelligence_v1p2beta1.types import video_intelligence
+from google.cloud.videointelligence_v1p3beta1.types import video_intelligence
 
 from .transports.base import DEFAULT_CLIENT_INFO, VideoIntelligenceServiceTransport
 from .transports.grpc import VideoIntelligenceServiceGrpcTransport
 from .transports.grpc_asyncio import VideoIntelligenceServiceGrpcAsyncIOTransport
 
 
 class VideoIntelligenceServiceClientMeta(type):
@@ -56,15 +68,15 @@
         OrderedDict()
     )  # type: Dict[str, Type[VideoIntelligenceServiceTransport]]
     _transport_registry["grpc"] = VideoIntelligenceServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = VideoIntelligenceServiceGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[VideoIntelligenceServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -77,15 +89,15 @@
 
         # No transport is requested; return the default (that is, the first one
         # in the dictionary).
         return next(iter(cls._transport_registry.values()))
 
 
 class VideoIntelligenceServiceClient(metaclass=VideoIntelligenceServiceClientMeta):
-    """Service that implements Google Cloud Video Intelligence API."""
+    """Service that implements the Video Intelligence API."""
 
     @staticmethod
     def _get_default_mtls_endpoint(api_endpoint):
         """Converts api endpoint to mTLS endpoint.
 
         Convert "*.sandbox.googleapis.com" and "*.googleapis.com" to
         "*.mtls.sandbox.googleapis.com" and "*.mtls.googleapis.com" respectively.
@@ -309,30 +321,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, VideoIntelligenceServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, VideoIntelligenceServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the video intelligence service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, VideoIntelligenceServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -354,14 +366,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -406,20 +419,20 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def annotate_video(
         self,
-        request: Union[video_intelligence.AnnotateVideoRequest, dict] = None,
+        request: Optional[Union[video_intelligence.AnnotateVideoRequest, dict]] = None,
         *,
-        input_uri: str = None,
-        features: Sequence[video_intelligence.Feature] = None,
+        input_uri: Optional[str] = None,
+        features: Optional[MutableSequence[video_intelligence.Feature]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Performs asynchronous video annotation. Progress and results can
         be retrieved through the ``google.longrunning.Operations``
         interface. ``Operation.metadata`` contains
         ``AnnotateVideoProgress`` (progress). ``Operation.response``
         contains ``AnnotateVideoResponse`` (results).
@@ -429,58 +442,58 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import videointelligence_v1p2beta1
+            from google.cloud import videointelligence_v1p3beta1
 
             def sample_annotate_video():
                 # Create a client
-                client = videointelligence_v1p2beta1.VideoIntelligenceServiceClient()
+                client = videointelligence_v1p3beta1.VideoIntelligenceServiceClient()
 
                 # Initialize request argument(s)
-                request = videointelligence_v1p2beta1.AnnotateVideoRequest(
-                    features="OBJECT_TRACKING",
+                request = videointelligence_v1p3beta1.AnnotateVideoRequest(
+                    features=['PERSON_DETECTION'],
                 )
 
                 # Make the request
                 operation = client.annotate_video(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.videointelligence_v1p2beta1.types.AnnotateVideoRequest, dict]):
+            request (Union[google.cloud.videointelligence_v1p3beta1.types.AnnotateVideoRequest, dict]):
                 The request object. Video annotation request.
             input_uri (str):
-                Input video location. Currently, only `Google Cloud
+                Input video location. Currently, only `Cloud
                 Storage <https://cloud.google.com/storage/>`__ URIs are
-                supported, which must be specified in the following
+                supported. URIs must be specified in the following
                 format: ``gs://bucket-id/object-id`` (other URI formats
                 return
                 [google.rpc.Code.INVALID_ARGUMENT][google.rpc.Code.INVALID_ARGUMENT]).
                 For more information, see `Request
                 URIs <https://cloud.google.com/storage/docs/request-endpoints>`__.
-                A video URI may include wildcards in ``object-id``, and
-                thus identify multiple videos. Supported wildcards: '*'
+                To identify multiple videos, a video URI may include
+                wildcards in the ``object-id``. Supported wildcards: '*'
                 to match 0 or more characters; '?' to match 1 character.
                 If unset, the input video should be embedded in the
                 request as ``input_content``. If set, ``input_content``
-                should be unset.
+                must be unset.
 
                 This corresponds to the ``input_uri`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            features (Sequence[google.cloud.videointelligence_v1p2beta1.types.Feature]):
+            features (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.Feature]):
                 Required. Requested video annotation
                 features.
 
                 This corresponds to the ``features`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -489,15 +502,15 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.videointelligence_v1p2beta1.types.AnnotateVideoResponse` Video annotation response. Included in the response
+                The result type for the operation will be :class:`google.cloud.videointelligence_v1p3beta1.types.AnnotateVideoResponse` Video annotation response. Included in the response
                    field of the Operation returned by the GetOperation
                    call of the google::longrunning::Operations service.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -554,18 +567,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("VideoIntelligenceServiceClient",)
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/base.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,40 +20,35 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1, operations_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
 
-from google.cloud.videointelligence_v1p2beta1.types import video_intelligence
+from google.cloud.videointelligence_v1p1beta1 import gapic_version as package_version
+from google.cloud.videointelligence_v1p1beta1.types import video_intelligence
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class VideoIntelligenceServiceTransport(abc.ABC):
     """Abstract transport class for VideoIntelligenceService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "videointelligence.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/grpc.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -178,16 +178,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/grpc_asyncio.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/grpc_asyncio.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -88,23 +88,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/types/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p2beta1/types/video_intelligence.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/types/video_intelligence.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.videointelligence.v1p2beta1",
@@ -99,15 +101,15 @@
             the input video should be embedded in the request as
             ``input_content``. If set, ``input_content`` should be
             unset.
         input_content (bytes):
             The video data bytes. If unset, the input video(s) should be
             specified via ``input_uri``. If set, ``input_uri`` should be
             unset.
-        features (Sequence[google.cloud.videointelligence_v1p2beta1.types.Feature]):
+        features (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.Feature]):
             Required. Requested video annotation
             features.
         video_context (google.cloud.videointelligence_v1p2beta1.types.VideoContext):
             Additional video context and/or
             feature-specific parameters.
         output_uri (str):
             Optional. Location where the output (in JSON format) should
@@ -121,82 +123,82 @@
         location_id (str):
             Optional. Cloud region where annotation should take place.
             Supported cloud regions: ``us-east1``, ``us-west1``,
             ``europe-west1``, ``asia-east1``. If no region is specified,
             a region will be determined based on video file location.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    input_content = proto.Field(
+    input_content: bytes = proto.Field(
         proto.BYTES,
         number=6,
     )
-    features = proto.RepeatedField(
+    features: MutableSequence["Feature"] = proto.RepeatedField(
         proto.ENUM,
         number=2,
         enum="Feature",
     )
-    video_context = proto.Field(
+    video_context: "VideoContext" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="VideoContext",
     )
-    output_uri = proto.Field(
+    output_uri: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    location_id = proto.Field(
+    location_id: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class VideoContext(proto.Message):
     r"""Video context and/or feature-specific parameters.
 
     Attributes:
-        segments (Sequence[google.cloud.videointelligence_v1p2beta1.types.VideoSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.VideoSegment]):
             Video segments to annotate. The segments may
             overlap and are not required to be contiguous or
             span the whole video. If unspecified, each video
             is treated as a single segment.
         label_detection_config (google.cloud.videointelligence_v1p2beta1.types.LabelDetectionConfig):
             Config for LABEL_DETECTION.
         shot_change_detection_config (google.cloud.videointelligence_v1p2beta1.types.ShotChangeDetectionConfig):
             Config for SHOT_CHANGE_DETECTION.
         explicit_content_detection_config (google.cloud.videointelligence_v1p2beta1.types.ExplicitContentDetectionConfig):
             Config for EXPLICIT_CONTENT_DETECTION.
         text_detection_config (google.cloud.videointelligence_v1p2beta1.types.TextDetectionConfig):
             Config for TEXT_DETECTION.
     """
 
-    segments = proto.RepeatedField(
+    segments: MutableSequence["VideoSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    label_detection_config = proto.Field(
+    label_detection_config: "LabelDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="LabelDetectionConfig",
     )
-    shot_change_detection_config = proto.Field(
+    shot_change_detection_config: "ShotChangeDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="ShotChangeDetectionConfig",
     )
-    explicit_content_detection_config = proto.Field(
+    explicit_content_detection_config: "ExplicitContentDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="ExplicitContentDetectionConfig",
     )
-    text_detection_config = proto.Field(
+    text_detection_config: "TextDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=8,
         message="TextDetectionConfig",
     )
 
 
 class LabelDetectionConfig(proto.Message):
@@ -214,24 +216,24 @@
             ``SHOT_AND_FRAME_MODE`` enabled.
         model (str):
             Model to use for label detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    label_detection_mode = proto.Field(
+    label_detection_mode: "LabelDetectionMode" = proto.Field(
         proto.ENUM,
         number=1,
         enum="LabelDetectionMode",
     )
-    stationary_camera = proto.Field(
+    stationary_camera: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class ShotChangeDetectionConfig(proto.Message):
     r"""Config for SHOT_CHANGE_DETECTION.
@@ -239,15 +241,15 @@
     Attributes:
         model (str):
             Model to use for shot change detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ExplicitContentDetectionConfig(proto.Message):
     r"""Config for EXPLICIT_CONTENT_DETECTION.
@@ -255,36 +257,36 @@
     Attributes:
         model (str):
             Model to use for explicit content detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class TextDetectionConfig(proto.Message):
     r"""Config for TEXT_DETECTION.
 
     Attributes:
-        language_hints (Sequence[str]):
+        language_hints (MutableSequence[str]):
             Language hint can be specified if the
             language to be detected is known a priori. It
             can increase the accuracy of the detection.
             Language hint must be language code in BCP-47
             format.
 
             Automatic language detection is performed if no
             hint is provided.
     """
 
-    language_hints = proto.RepeatedField(
+    language_hints: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=1,
     )
 
 
 class VideoSegment(proto.Message):
     r"""Video segment.
@@ -296,20 +298,20 @@
             (inclusive).
         end_time_offset (google.protobuf.duration_pb2.Duration):
             Time-offset, relative to the beginning of the
             video, corresponding to the end of the segment
             (inclusive).
     """
 
-    start_time_offset = proto.Field(
+    start_time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    end_time_offset = proto.Field(
+    end_time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class LabelSegment(proto.Message):
@@ -318,20 +320,20 @@
     Attributes:
         segment (google.cloud.videointelligence_v1p2beta1.types.VideoSegment):
             Video segment where a label was detected.
         confidence (float):
             Confidence that the label is accurate. Range: [0, 1].
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class LabelFrame(proto.Message):
     r"""Video frame level annotation results for label detection.
@@ -341,20 +343,20 @@
             Time-offset, relative to the beginning of the
             video, corresponding to the video frame for this
             location.
         confidence (float):
             Confidence that the label is accurate. Range: [0, 1].
     """
 
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class Entity(proto.Message):
     r"""Detected entity from video analysis.
@@ -366,62 +368,62 @@
             API <https://developers.google.com/knowledge-graph/>`__.
         description (str):
             Textual description, e.g. ``Fixed-gear bicycle``.
         language_code (str):
             Language code for ``description`` in BCP-47 format.
     """
 
-    entity_id = proto.Field(
+    entity_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class LabelAnnotation(proto.Message):
     r"""Label annotation.
 
     Attributes:
         entity (google.cloud.videointelligence_v1p2beta1.types.Entity):
             Detected entity.
-        category_entities (Sequence[google.cloud.videointelligence_v1p2beta1.types.Entity]):
+        category_entities (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.Entity]):
             Common categories for the detected entity. E.g. when the
             label is ``Terrier`` the category is likely ``dog``. And in
             some cases there might be more than one categories e.g.
             ``Terrier`` could also be a ``pet``.
-        segments (Sequence[google.cloud.videointelligence_v1p2beta1.types.LabelSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.LabelSegment]):
             All video segments where a label was
             detected.
-        frames (Sequence[google.cloud.videointelligence_v1p2beta1.types.LabelFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.LabelFrame]):
             All video frames where a label was detected.
     """
 
-    entity = proto.Field(
+    entity: "Entity" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Entity",
     )
-    category_entities = proto.RepeatedField(
+    category_entities: MutableSequence["Entity"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="Entity",
     )
-    segments = proto.RepeatedField(
+    segments: MutableSequence["LabelSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="LabelSegment",
     )
-    frames = proto.RepeatedField(
+    frames: MutableSequence["LabelFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="LabelFrame",
     )
 
 
 class ExplicitContentFrame(proto.Message):
@@ -432,38 +434,38 @@
             Time-offset, relative to the beginning of the
             video, corresponding to the video frame for this
             location.
         pornography_likelihood (google.cloud.videointelligence_v1p2beta1.types.Likelihood):
             Likelihood of the pornography content..
     """
 
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    pornography_likelihood = proto.Field(
+    pornography_likelihood: "Likelihood" = proto.Field(
         proto.ENUM,
         number=2,
         enum="Likelihood",
     )
 
 
 class ExplicitContentAnnotation(proto.Message):
     r"""Explicit content annotation (based on per-frame visual
     signals only). If no explicit content has been detected in a
     frame, no annotations are present for that frame.
 
     Attributes:
-        frames (Sequence[google.cloud.videointelligence_v1p2beta1.types.ExplicitContentFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.ExplicitContentFrame]):
             All video frames where explicit content was
             detected.
     """
 
-    frames = proto.RepeatedField(
+    frames: MutableSequence["ExplicitContentFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="ExplicitContentFrame",
     )
 
 
 class NormalizedBoundingBox(proto.Message):
@@ -477,128 +479,130 @@
             Top Y coordinate.
         right (float):
             Right X coordinate.
         bottom (float):
             Bottom Y coordinate.
     """
 
-    left = proto.Field(
+    left: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    top = proto.Field(
+    top: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    right = proto.Field(
+    right: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
-    bottom = proto.Field(
+    bottom: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
 
 
 class VideoAnnotationResults(proto.Message):
     r"""Annotation results for a single video.
 
     Attributes:
         input_uri (str):
             Video file location in `Google Cloud
             Storage <https://cloud.google.com/storage/>`__.
-        segment_label_annotations (Sequence[google.cloud.videointelligence_v1p2beta1.types.LabelAnnotation]):
+        segment_label_annotations (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.LabelAnnotation]):
             Label annotations on video level or user
             specified segment level. There is exactly one
             element for each unique label.
-        shot_label_annotations (Sequence[google.cloud.videointelligence_v1p2beta1.types.LabelAnnotation]):
+        shot_label_annotations (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.LabelAnnotation]):
             Label annotations on shot level.
             There is exactly one element for each unique
             label.
-        frame_label_annotations (Sequence[google.cloud.videointelligence_v1p2beta1.types.LabelAnnotation]):
+        frame_label_annotations (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.LabelAnnotation]):
             Label annotations on frame level.
             There is exactly one element for each unique
             label.
-        shot_annotations (Sequence[google.cloud.videointelligence_v1p2beta1.types.VideoSegment]):
+        shot_annotations (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.VideoSegment]):
             Shot annotations. Each shot is represented as
             a video segment.
         explicit_annotation (google.cloud.videointelligence_v1p2beta1.types.ExplicitContentAnnotation):
             Explicit content annotation.
-        text_annotations (Sequence[google.cloud.videointelligence_v1p2beta1.types.TextAnnotation]):
+        text_annotations (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.TextAnnotation]):
             OCR text detection and tracking.
             Annotations for list of detected text snippets.
             Each will have list of frame information
             associated with it.
-        object_annotations (Sequence[google.cloud.videointelligence_v1p2beta1.types.ObjectTrackingAnnotation]):
+        object_annotations (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.ObjectTrackingAnnotation]):
             Annotations for list of objects detected and
             tracked in video.
         error (google.rpc.status_pb2.Status):
             If set, indicates an error. Note that for a single
             ``AnnotateVideoRequest`` some videos may succeed and some
             may fail.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    segment_label_annotations = proto.RepeatedField(
+    segment_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="LabelAnnotation",
     )
-    shot_label_annotations = proto.RepeatedField(
+    shot_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="LabelAnnotation",
     )
-    frame_label_annotations = proto.RepeatedField(
+    frame_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="LabelAnnotation",
     )
-    shot_annotations = proto.RepeatedField(
+    shot_annotations: MutableSequence["VideoSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=6,
         message="VideoSegment",
     )
-    explicit_annotation = proto.Field(
+    explicit_annotation: "ExplicitContentAnnotation" = proto.Field(
         proto.MESSAGE,
         number=7,
         message="ExplicitContentAnnotation",
     )
-    text_annotations = proto.RepeatedField(
+    text_annotations: MutableSequence["TextAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=12,
         message="TextAnnotation",
     )
-    object_annotations = proto.RepeatedField(
+    object_annotations: MutableSequence[
+        "ObjectTrackingAnnotation"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=14,
         message="ObjectTrackingAnnotation",
     )
-    error = proto.Field(
+    error: status_pb2.Status = proto.Field(
         proto.MESSAGE,
         number=9,
         message=status_pb2.Status,
     )
 
 
 class AnnotateVideoResponse(proto.Message):
     r"""Video annotation response. Included in the ``response`` field of the
     ``Operation`` returned by the ``GetOperation`` call of the
     ``google::longrunning::Operations`` service.
 
     Attributes:
-        annotation_results (Sequence[google.cloud.videointelligence_v1p2beta1.types.VideoAnnotationResults]):
+        annotation_results (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.VideoAnnotationResults]):
             Annotation results for all videos specified in
             ``AnnotateVideoRequest``.
     """
 
-    annotation_results = proto.RepeatedField(
+    annotation_results: MutableSequence["VideoAnnotationResults"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoAnnotationResults",
     )
 
 
 class VideoAnnotationProgress(proto.Message):
@@ -613,46 +617,48 @@
             Guaranteed to be 100 when fully processed.
         start_time (google.protobuf.timestamp_pb2.Timestamp):
             Time when the request was received.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Time of the most recent update.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    progress_percent = proto.Field(
+    progress_percent: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    start_time = proto.Field(
+    start_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class AnnotateVideoProgress(proto.Message):
     r"""Video annotation progress. Included in the ``metadata`` field of the
     ``Operation`` returned by the ``GetOperation`` call of the
     ``google::longrunning::Operations`` service.
 
     Attributes:
-        annotation_progress (Sequence[google.cloud.videointelligence_v1p2beta1.types.VideoAnnotationProgress]):
+        annotation_progress (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.VideoAnnotationProgress]):
             Progress metadata for all videos specified in
             ``AnnotateVideoRequest``.
     """
 
-    annotation_progress = proto.RepeatedField(
+    annotation_progress: MutableSequence[
+        "VideoAnnotationProgress"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoAnnotationProgress",
     )
 
 
 class NormalizedVertex(proto.Message):
@@ -663,19 +669,19 @@
     Attributes:
         x (float):
             X coordinate.
         y (float):
             Y coordinate.
     """
 
-    x = proto.Field(
+    x: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    y = proto.Field(
+    y: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class NormalizedBoundingPoly(proto.Message):
     r"""Normalized bounding polygon for text (that might not be aligned with
@@ -688,19 +694,19 @@
     it becomes: 2----3 \| \| 1----0
 
     and the vertex order will still be (0, 1, 2, 3). Note that values
     can be less than 0, or greater than 1 due to trignometric
     calculations for location of the box.
 
     Attributes:
-        vertices (Sequence[google.cloud.videointelligence_v1p2beta1.types.NormalizedVertex]):
+        vertices (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.NormalizedVertex]):
             Normalized vertices of the bounding polygon.
     """
 
-    vertices = proto.RepeatedField(
+    vertices: MutableSequence["NormalizedVertex"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="NormalizedVertex",
     )
 
 
 class TextSegment(proto.Message):
@@ -710,29 +716,29 @@
         segment (google.cloud.videointelligence_v1p2beta1.types.VideoSegment):
             Video segment where a text snippet was
             detected.
         confidence (float):
             Confidence for the track of detected text. It
             is calculated as the highest over all frames
             where OCR detected text appears.
-        frames (Sequence[google.cloud.videointelligence_v1p2beta1.types.TextFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.TextFrame]):
             Information related to the frames where OCR
             detected text appears.
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    frames = proto.RepeatedField(
+    frames: MutableSequence["TextFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="TextFrame",
     )
 
 
 class TextFrame(proto.Message):
@@ -744,44 +750,44 @@
         rotated_bounding_box (google.cloud.videointelligence_v1p2beta1.types.NormalizedBoundingPoly):
             Bounding polygon of the detected text for
             this frame.
         time_offset (google.protobuf.duration_pb2.Duration):
             Timestamp of this frame.
     """
 
-    rotated_bounding_box = proto.Field(
+    rotated_bounding_box: "NormalizedBoundingPoly" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="NormalizedBoundingPoly",
     )
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class TextAnnotation(proto.Message):
     r"""Annotations related to one detected OCR text snippet. This
     will contain the corresponding text, confidence value, and frame
     level information for each detection.
 
     Attributes:
         text (str):
             The detected text.
-        segments (Sequence[google.cloud.videointelligence_v1p2beta1.types.TextSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.TextSegment]):
             All video segments where OCR detected text
             appears.
     """
 
-    text = proto.Field(
+    text: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    segments = proto.RepeatedField(
+    segments: MutableSequence["TextSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="TextSegment",
     )
 
 
 class ObjectTrackingFrame(proto.Message):
@@ -793,20 +799,20 @@
         normalized_bounding_box (google.cloud.videointelligence_v1p2beta1.types.NormalizedBoundingBox):
             The normalized bounding box location of this
             object track for the frame.
         time_offset (google.protobuf.duration_pb2.Duration):
             The timestamp of the frame in microseconds.
     """
 
-    normalized_bounding_box = proto.Field(
+    normalized_bounding_box: "NormalizedBoundingBox" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="NormalizedBoundingBox",
     )
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class ObjectTrackingAnnotation(proto.Message):
@@ -837,40 +843,40 @@
             This field is a member of `oneof`_ ``track_info``.
         entity (google.cloud.videointelligence_v1p2beta1.types.Entity):
             Entity to specify the object category that
             this track is labeled as.
         confidence (float):
             Object category's labeling confidence of this
             track.
-        frames (Sequence[google.cloud.videointelligence_v1p2beta1.types.ObjectTrackingFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1p2beta1.types.ObjectTrackingFrame]):
             Information corresponding to all frames where
             this object track appears.
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="track_info",
         message="VideoSegment",
     )
-    track_id = proto.Field(
+    track_id: int = proto.Field(
         proto.INT64,
         number=5,
         oneof="track_info",
     )
-    entity = proto.Field(
+    entity: "Entity" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Entity",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
-    frames = proto.RepeatedField(
+    frames: MutableSequence["ObjectTrackingFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="ObjectTrackingFrame",
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.videointelligence import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from .services.streaming_video_intelligence_service import (
     StreamingVideoIntelligenceServiceAsyncClient,
     StreamingVideoIntelligenceServiceClient,
 )
 from .services.video_intelligence_service import (
     VideoIntelligenceServiceAsyncClient,
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/gapic_metadata.json` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/async_client.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,28 +18,31 @@
 import re
 from typing import (
     AsyncIterable,
     AsyncIterator,
     Awaitable,
     Dict,
     Mapping,
+    MutableMapping,
+    MutableSequence,
     Optional,
     Sequence,
     Tuple,
     Type,
     Union,
 )
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.videointelligence_v1p3beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.rpc import status_pb2  # type: ignore
@@ -179,19 +182,19 @@
         type(StreamingVideoIntelligenceServiceClient).get_transport_class,
         type(StreamingVideoIntelligenceServiceClient),
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[
             str, StreamingVideoIntelligenceServiceTransport
         ] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the streaming video intelligence service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -227,20 +230,20 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     def streaming_annotate_video(
         self,
-        requests: AsyncIterator[
-            video_intelligence.StreamingAnnotateVideoRequest
+        requests: Optional[
+            AsyncIterator[video_intelligence.StreamingAnnotateVideoRequest]
         ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> Awaitable[AsyncIterable[video_intelligence.StreamingAnnotateVideoResponse]]:
         r"""Performs video annotation with bidirectional
         streaming: emitting results while sending video/audio
         bytes. This method is only available via the gRPC API
         (not REST).
 
@@ -335,18 +338,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("StreamingVideoIntelligenceServiceAsyncClient",)
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/client.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,31 +17,35 @@
 import os
 import re
 from typing import (
     Dict,
     Iterable,
     Iterator,
     Mapping,
+    MutableMapping,
+    MutableSequence,
     Optional,
     Sequence,
     Tuple,
     Type,
     Union,
+    cast,
 )
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.videointelligence_v1p3beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.rpc import status_pb2  # type: ignore
@@ -72,15 +76,15 @@
     _transport_registry["grpc"] = StreamingVideoIntelligenceServiceGrpcTransport
     _transport_registry[
         "grpc_asyncio"
     ] = StreamingVideoIntelligenceServiceGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[StreamingVideoIntelligenceServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -327,30 +331,32 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, StreamingVideoIntelligenceServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[
+            Union[str, StreamingVideoIntelligenceServiceTransport]
+        ] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the streaming video intelligence service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, StreamingVideoIntelligenceServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -372,14 +378,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -424,18 +431,20 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def streaming_annotate_video(
         self,
-        requests: Iterator[video_intelligence.StreamingAnnotateVideoRequest] = None,
+        requests: Optional[
+            Iterator[video_intelligence.StreamingAnnotateVideoRequest]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> Iterable[video_intelligence.StreamingAnnotateVideoResponse]:
         r"""Performs video annotation with bidirectional
         streaming: emitting results while sending video/audio
         bytes. This method is only available via the gRPC API
         (not REST).
 
@@ -523,18 +532,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("StreamingVideoIntelligenceServiceClient",)
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/base.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,40 +19,35 @@
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
 
+from google.cloud.videointelligence_v1p3beta1 import gapic_version as package_version
 from google.cloud.videointelligence_v1p3beta1.types import video_intelligence
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class StreamingVideoIntelligenceServiceTransport(abc.ABC):
     """Abstract transport class for StreamingVideoIntelligenceService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "videointelligence.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/grpc.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,22 +44,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -178,16 +178,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/grpc_asyncio.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -89,23 +89,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/async_client.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,41 +12,52 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.videointelligence_v1p1beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 
-from google.cloud.videointelligence_v1p3beta1.types import video_intelligence
+from google.cloud.videointelligence_v1p1beta1.types import video_intelligence
 
 from .client import VideoIntelligenceServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, VideoIntelligenceServiceTransport
 from .transports.grpc_asyncio import VideoIntelligenceServiceGrpcAsyncIOTransport
 
 
 class VideoIntelligenceServiceAsyncClient:
-    """Service that implements the Video Intelligence API."""
+    """Service that implements Google Cloud Video Intelligence API."""
 
     _client: VideoIntelligenceServiceClient
 
     DEFAULT_ENDPOINT = VideoIntelligenceServiceClient.DEFAULT_ENDPOINT
     DEFAULT_MTLS_ENDPOINT = VideoIntelligenceServiceClient.DEFAULT_MTLS_ENDPOINT
 
     common_billing_account_path = staticmethod(
@@ -160,17 +171,17 @@
         type(VideoIntelligenceServiceClient).get_transport_class,
         type(VideoIntelligenceServiceClient),
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, VideoIntelligenceServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the video intelligence service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -206,20 +217,20 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def annotate_video(
         self,
-        request: Union[video_intelligence.AnnotateVideoRequest, dict] = None,
+        request: Optional[Union[video_intelligence.AnnotateVideoRequest, dict]] = None,
         *,
-        input_uri: str = None,
-        features: Sequence[video_intelligence.Feature] = None,
+        input_uri: Optional[str] = None,
+        features: Optional[MutableSequence[video_intelligence.Feature]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Performs asynchronous video annotation. Progress and results can
         be retrieved through the ``google.longrunning.Operations``
         interface. ``Operation.metadata`` contains
         ``AnnotateVideoProgress`` (progress). ``Operation.response``
         contains ``AnnotateVideoResponse`` (results).
@@ -229,58 +240,58 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import videointelligence_v1p3beta1
+            from google.cloud import videointelligence_v1p1beta1
 
             async def sample_annotate_video():
                 # Create a client
-                client = videointelligence_v1p3beta1.VideoIntelligenceServiceAsyncClient()
+                client = videointelligence_v1p1beta1.VideoIntelligenceServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = videointelligence_v1p3beta1.AnnotateVideoRequest(
-                    features="PERSON_DETECTION",
+                request = videointelligence_v1p1beta1.AnnotateVideoRequest(
+                    features=['SPEECH_TRANSCRIPTION'],
                 )
 
                 # Make the request
                 operation = client.annotate_video(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.videointelligence_v1p3beta1.types.AnnotateVideoRequest, dict]):
+            request (Optional[Union[google.cloud.videointelligence_v1p1beta1.types.AnnotateVideoRequest, dict]]):
                 The request object. Video annotation request.
             input_uri (:class:`str`):
-                Input video location. Currently, only `Cloud
+                Input video location. Currently, only `Google Cloud
                 Storage <https://cloud.google.com/storage/>`__ URIs are
-                supported. URIs must be specified in the following
+                supported, which must be specified in the following
                 format: ``gs://bucket-id/object-id`` (other URI formats
                 return
                 [google.rpc.Code.INVALID_ARGUMENT][google.rpc.Code.INVALID_ARGUMENT]).
                 For more information, see `Request
                 URIs <https://cloud.google.com/storage/docs/request-endpoints>`__.
-                To identify multiple videos, a video URI may include
-                wildcards in the ``object-id``. Supported wildcards: '*'
+                A video URI may include wildcards in ``object-id``, and
+                thus identify multiple videos. Supported wildcards: '*'
                 to match 0 or more characters; '?' to match 1 character.
                 If unset, the input video should be embedded in the
                 request as ``input_content``. If set, ``input_content``
-                must be unset.
+                should be unset.
 
                 This corresponds to the ``input_uri`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            features (:class:`Sequence[google.cloud.videointelligence_v1p3beta1.types.Feature]`):
+            features (:class:`MutableSequence[google.cloud.videointelligence_v1p1beta1.types.Feature]`):
                 Required. Requested video annotation
                 features.
 
                 This corresponds to the ``features`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -289,15 +300,15 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.videointelligence_v1p3beta1.types.AnnotateVideoResponse` Video annotation response. Included in the response
+                The result type for the operation will be :class:`google.cloud.videointelligence_v1p1beta1.types.AnnotateVideoResponse` Video annotation response. Included in the response
                    field of the Operation returned by the GetOperation
                    call of the google::longrunning::Operations service.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -357,18 +368,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("VideoIntelligenceServiceAsyncClient",)
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/client.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,36 +12,48 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.videointelligence_v1p1beta1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 
-from google.cloud.videointelligence_v1p3beta1.types import video_intelligence
+from google.cloud.videointelligence_v1p1beta1.types import video_intelligence
 
 from .transports.base import DEFAULT_CLIENT_INFO, VideoIntelligenceServiceTransport
 from .transports.grpc import VideoIntelligenceServiceGrpcTransport
 from .transports.grpc_asyncio import VideoIntelligenceServiceGrpcAsyncIOTransport
 
 
 class VideoIntelligenceServiceClientMeta(type):
@@ -56,15 +68,15 @@
         OrderedDict()
     )  # type: Dict[str, Type[VideoIntelligenceServiceTransport]]
     _transport_registry["grpc"] = VideoIntelligenceServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = VideoIntelligenceServiceGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[VideoIntelligenceServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -77,15 +89,15 @@
 
         # No transport is requested; return the default (that is, the first one
         # in the dictionary).
         return next(iter(cls._transport_registry.values()))
 
 
 class VideoIntelligenceServiceClient(metaclass=VideoIntelligenceServiceClientMeta):
-    """Service that implements the Video Intelligence API."""
+    """Service that implements Google Cloud Video Intelligence API."""
 
     @staticmethod
     def _get_default_mtls_endpoint(api_endpoint):
         """Converts api endpoint to mTLS endpoint.
 
         Convert "*.sandbox.googleapis.com" and "*.googleapis.com" to
         "*.mtls.sandbox.googleapis.com" and "*.mtls.googleapis.com" respectively.
@@ -309,30 +321,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, VideoIntelligenceServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, VideoIntelligenceServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the video intelligence service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, VideoIntelligenceServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -354,14 +366,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -406,20 +419,20 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def annotate_video(
         self,
-        request: Union[video_intelligence.AnnotateVideoRequest, dict] = None,
+        request: Optional[Union[video_intelligence.AnnotateVideoRequest, dict]] = None,
         *,
-        input_uri: str = None,
-        features: Sequence[video_intelligence.Feature] = None,
+        input_uri: Optional[str] = None,
+        features: Optional[MutableSequence[video_intelligence.Feature]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Performs asynchronous video annotation. Progress and results can
         be retrieved through the ``google.longrunning.Operations``
         interface. ``Operation.metadata`` contains
         ``AnnotateVideoProgress`` (progress). ``Operation.response``
         contains ``AnnotateVideoResponse`` (results).
@@ -429,58 +442,58 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import videointelligence_v1p3beta1
+            from google.cloud import videointelligence_v1p1beta1
 
             def sample_annotate_video():
                 # Create a client
-                client = videointelligence_v1p3beta1.VideoIntelligenceServiceClient()
+                client = videointelligence_v1p1beta1.VideoIntelligenceServiceClient()
 
                 # Initialize request argument(s)
-                request = videointelligence_v1p3beta1.AnnotateVideoRequest(
-                    features="PERSON_DETECTION",
+                request = videointelligence_v1p1beta1.AnnotateVideoRequest(
+                    features=['SPEECH_TRANSCRIPTION'],
                 )
 
                 # Make the request
                 operation = client.annotate_video(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.videointelligence_v1p3beta1.types.AnnotateVideoRequest, dict]):
+            request (Union[google.cloud.videointelligence_v1p1beta1.types.AnnotateVideoRequest, dict]):
                 The request object. Video annotation request.
             input_uri (str):
-                Input video location. Currently, only `Cloud
+                Input video location. Currently, only `Google Cloud
                 Storage <https://cloud.google.com/storage/>`__ URIs are
-                supported. URIs must be specified in the following
+                supported, which must be specified in the following
                 format: ``gs://bucket-id/object-id`` (other URI formats
                 return
                 [google.rpc.Code.INVALID_ARGUMENT][google.rpc.Code.INVALID_ARGUMENT]).
                 For more information, see `Request
                 URIs <https://cloud.google.com/storage/docs/request-endpoints>`__.
-                To identify multiple videos, a video URI may include
-                wildcards in the ``object-id``. Supported wildcards: '*'
+                A video URI may include wildcards in ``object-id``, and
+                thus identify multiple videos. Supported wildcards: '*'
                 to match 0 or more characters; '?' to match 1 character.
                 If unset, the input video should be embedded in the
                 request as ``input_content``. If set, ``input_content``
-                must be unset.
+                should be unset.
 
                 This corresponds to the ``input_uri`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            features (Sequence[google.cloud.videointelligence_v1p3beta1.types.Feature]):
+            features (MutableSequence[google.cloud.videointelligence_v1p1beta1.types.Feature]):
                 Required. Requested video annotation
                 features.
 
                 This corresponds to the ``features`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -489,15 +502,15 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.videointelligence_v1p3beta1.types.AnnotateVideoResponse` Video annotation response. Included in the response
+                The result type for the operation will be :class:`google.cloud.videointelligence_v1p1beta1.types.AnnotateVideoResponse` Video annotation response. Included in the response
                    field of the Operation returned by the GetOperation
                    call of the google::longrunning::Operations service.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -554,18 +567,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("VideoIntelligenceServiceClient",)
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/base.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,40 +20,35 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1, operations_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
 
-from google.cloud.videointelligence_v1p3beta1.types import video_intelligence
+from google.cloud.videointelligence_v1p2beta1 import gapic_version as package_version
+from google.cloud.videointelligence_v1p2beta1.types import video_intelligence
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-videointelligence",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class VideoIntelligenceServiceTransport(abc.ABC):
     """Abstract transport class for VideoIntelligenceService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "videointelligence.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/grpc.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 from google.api_core import gapic_v1, grpc_helpers, operations_v1
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 import grpc  # type: ignore
 
-from google.cloud.videointelligence_v1p3beta1.types import video_intelligence
+from google.cloud.videointelligence_v1p1beta1.types import video_intelligence
 
 from .base import DEFAULT_CLIENT_INFO, VideoIntelligenceServiceTransport
 
 
 class VideoIntelligenceServiceGrpcTransport(VideoIntelligenceServiceTransport):
     """gRPC backend transport for VideoIntelligenceService.
 
-    Service that implements the Video Intelligence API.
+    Service that implements Google Cloud Video Intelligence API.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
@@ -43,22 +43,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -178,16 +178,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
@@ -264,15 +264,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "annotate_video" not in self._stubs:
             self._stubs["annotate_video"] = self.grpc_channel.unary_unary(
-                "/google.cloud.videointelligence.v1p3beta1.VideoIntelligenceService/AnnotateVideo",
+                "/google.cloud.videointelligence.v1p1beta1.VideoIntelligenceService/AnnotateVideo",
                 request_serializer=video_intelligence.AnnotateVideoRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["annotate_video"]
 
     def close(self):
         self.grpc_channel.close()
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/services/video_intelligence_service/transports/grpc_asyncio.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,102 +9,57 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
-from google.api_core import gapic_v1, grpc_helpers_async, operations_v1
+from google.api_core import gapic_v1, grpc_helpers, operations_v1
+import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 import grpc  # type: ignore
-from grpc.experimental import aio  # type: ignore
 
-from google.cloud.videointelligence_v1p3beta1.types import video_intelligence
+from google.cloud.videointelligence_v1beta2.types import video_intelligence
 
 from .base import DEFAULT_CLIENT_INFO, VideoIntelligenceServiceTransport
-from .grpc import VideoIntelligenceServiceGrpcTransport
 
 
-class VideoIntelligenceServiceGrpcAsyncIOTransport(VideoIntelligenceServiceTransport):
-    """gRPC AsyncIO backend transport for VideoIntelligenceService.
+class VideoIntelligenceServiceGrpcTransport(VideoIntelligenceServiceTransport):
+    """gRPC backend transport for VideoIntelligenceService.
 
-    Service that implements the Video Intelligence API.
+    Service that implements Google Cloud Video Intelligence API.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
     """
 
-    _grpc_channel: aio.Channel
-    _stubs: Dict[str, Callable] = {}
-
-    @classmethod
-    def create_channel(
-        cls,
-        host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: Optional[str] = None,
-        scopes: Optional[Sequence[str]] = None,
-        quota_project_id: Optional[str] = None,
-        **kwargs,
-    ) -> aio.Channel:
-        """Create and return a gRPC AsyncIO channel object.
-        Args:
-            host (Optional[str]): The host for the channel to use.
-            credentials (Optional[~.Credentials]): The
-                authorization credentials to attach to requests. These
-                credentials identify this application to the service. If
-                none are specified, the client will attempt to ascertain
-                the credentials from the environment.
-            credentials_file (Optional[str]): A file with credentials that can
-                be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            quota_project_id (Optional[str]): An optional project to use for billing
-                and quota.
-            kwargs (Optional[dict]): Keyword arguments, which are passed to the
-                channel creation.
-        Returns:
-            aio.Channel: A gRPC AsyncIO channel object.
-        """
-
-        return grpc_helpers_async.create_channel(
-            host,
-            credentials=credentials,
-            credentials_file=credentials_file,
-            quota_project_id=quota_project_id,
-            default_scopes=cls.AUTH_SCOPES,
-            scopes=scopes,
-            default_host=cls.DEFAULT_HOST,
-            **kwargs,
-        )
+    _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "videointelligence.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
@@ -115,18 +70,17 @@
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
                 This argument is ignored if ``channel`` is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
                 This argument is ignored if ``channel`` is provided.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            channel (Optional[aio.Channel]): A ``Channel`` instance through
+            scopes (Optional(Sequence[str])): A list of scopes. This argument is
+                ignored if ``channel`` is provided.
+            channel (Optional[grpc.Channel]): A ``Channel`` instance through
                 which to make calls.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
@@ -145,35 +99,36 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
 
         Raises:
-            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
+          google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
               creation failed for any reason.
           google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
               and ``credentials_file`` are passed.
         """
         self._grpc_channel = None
         self._ssl_channel_credentials = ssl_channel_credentials
         self._stubs: Dict[str, Callable] = {}
-        self._operations_client: Optional[operations_v1.OperationsAsyncClient] = None
+        self._operations_client: Optional[operations_v1.OperationsClient] = None
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
         if channel:
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
+
         else:
             if api_mtls_endpoint:
                 host = api_mtls_endpoint
 
                 # Create SSL credentials with client_cert_source or application
                 # default SSL credentials.
                 if client_cert_source:
@@ -219,70 +174,112 @@
                     ("grpc.max_receive_message_length", -1),
                 ],
             )
 
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
-    @property
-    def grpc_channel(self) -> aio.Channel:
-        """Create the channel designed to connect to this service.
+    @classmethod
+    def create_channel(
+        cls,
+        host: str = "videointelligence.googleapis.com",
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        quota_project_id: Optional[str] = None,
+        **kwargs,
+    ) -> grpc.Channel:
+        """Create and return a gRPC channel object.
+        Args:
+            host (Optional[str]): The host for the channel to use.
+            credentials (Optional[~.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify this application to the service. If
+                none are specified, the client will attempt to ascertain
+                the credentials from the environment.
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is mutually exclusive with credentials.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            kwargs (Optional[dict]): Keyword arguments, which are passed to the
+                channel creation.
+        Returns:
+            grpc.Channel: A gRPC channel object.
 
-        This property caches on the instance; repeated calls return
-        the same channel.
+        Raises:
+            google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
+              and ``credentials_file`` are passed.
         """
-        # Return the channel from cache.
+
+        return grpc_helpers.create_channel(
+            host,
+            credentials=credentials,
+            credentials_file=credentials_file,
+            quota_project_id=quota_project_id,
+            default_scopes=cls.AUTH_SCOPES,
+            scopes=scopes,
+            default_host=cls.DEFAULT_HOST,
+            **kwargs,
+        )
+
+    @property
+    def grpc_channel(self) -> grpc.Channel:
+        """Return the channel designed to connect to this service."""
         return self._grpc_channel
 
     @property
-    def operations_client(self) -> operations_v1.OperationsAsyncClient:
+    def operations_client(self) -> operations_v1.OperationsClient:
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
         # Quick check: Only create a new client if we do not already have one.
         if self._operations_client is None:
-            self._operations_client = operations_v1.OperationsAsyncClient(
-                self.grpc_channel
-            )
+            self._operations_client = operations_v1.OperationsClient(self.grpc_channel)
 
         # Return the client from cache.
         return self._operations_client
 
     @property
     def annotate_video(
         self,
-    ) -> Callable[
-        [video_intelligence.AnnotateVideoRequest], Awaitable[operations_pb2.Operation]
-    ]:
+    ) -> Callable[[video_intelligence.AnnotateVideoRequest], operations_pb2.Operation]:
         r"""Return a callable for the annotate video method over gRPC.
 
         Performs asynchronous video annotation. Progress and results can
         be retrieved through the ``google.longrunning.Operations``
         interface. ``Operation.metadata`` contains
         ``AnnotateVideoProgress`` (progress). ``Operation.response``
         contains ``AnnotateVideoResponse`` (results).
 
         Returns:
             Callable[[~.AnnotateVideoRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "annotate_video" not in self._stubs:
             self._stubs["annotate_video"] = self.grpc_channel.unary_unary(
-                "/google.cloud.videointelligence.v1p3beta1.VideoIntelligenceService/AnnotateVideo",
+                "/google.cloud.videointelligence.v1beta2.VideoIntelligenceService/AnnotateVideo",
                 request_serializer=video_intelligence.AnnotateVideoRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["annotate_video"]
 
     def close(self):
-        return self.grpc_channel.close()
+        self.grpc_channel.close()
+
+    @property
+    def kind(self) -> str:
+        return "grpc"
 
 
-__all__ = ("VideoIntelligenceServiceGrpcAsyncIOTransport",)
+__all__ = ("VideoIntelligenceServiceGrpcTransport",)
```

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/types/__init__.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/google/cloud/videointelligence_v1p3beta1/types/video_intelligence.py` & `google-cloud-videointelligence-2.9.0/google/cloud/videointelligence_v1p3beta1/types/video_intelligence.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.videointelligence.v1p3beta1",
@@ -146,15 +148,15 @@
             match 0 or more characters; '?' to match 1 character. If
             unset, the input video should be embedded in the request as
             ``input_content``. If set, ``input_content`` must be unset.
         input_content (bytes):
             The video data bytes. If unset, the input video(s) should be
             specified via the ``input_uri``. If set, ``input_uri`` must
             be unset.
-        features (Sequence[google.cloud.videointelligence_v1p3beta1.types.Feature]):
+        features (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.Feature]):
             Required. Requested video annotation
             features.
         video_context (google.cloud.videointelligence_v1p3beta1.types.VideoContext):
             Additional video context and/or
             feature-specific parameters.
         output_uri (str):
             Optional. Location where the output (in JSON format) should
@@ -168,47 +170,47 @@
         location_id (str):
             Optional. Cloud region where annotation should take place.
             Supported cloud regions are: ``us-east1``, ``us-west1``,
             ``europe-west1``, ``asia-east1``. If no region is specified,
             the region will be determined based on video file location.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    input_content = proto.Field(
+    input_content: bytes = proto.Field(
         proto.BYTES,
         number=6,
     )
-    features = proto.RepeatedField(
+    features: MutableSequence["Feature"] = proto.RepeatedField(
         proto.ENUM,
         number=2,
         enum="Feature",
     )
-    video_context = proto.Field(
+    video_context: "VideoContext" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="VideoContext",
     )
-    output_uri = proto.Field(
+    output_uri: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    location_id = proto.Field(
+    location_id: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class VideoContext(proto.Message):
     r"""Video context and/or feature-specific parameters.
 
     Attributes:
-        segments (Sequence[google.cloud.videointelligence_v1p3beta1.types.VideoSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.VideoSegment]):
             Video segments to annotate. The segments may
             overlap and are not required to be contiguous or
             span the whole video. If unspecified, each video
             is treated as a single segment.
         label_detection_config (google.cloud.videointelligence_v1p3beta1.types.LabelDetectionConfig):
             Config for LABEL_DETECTION.
         shot_change_detection_config (google.cloud.videointelligence_v1p3beta1.types.ShotChangeDetectionConfig):
@@ -223,55 +225,55 @@
             Config for TEXT_DETECTION.
         person_detection_config (google.cloud.videointelligence_v1p3beta1.types.PersonDetectionConfig):
             Config for PERSON_DETECTION.
         object_tracking_config (google.cloud.videointelligence_v1p3beta1.types.ObjectTrackingConfig):
             Config for OBJECT_TRACKING.
     """
 
-    segments = proto.RepeatedField(
+    segments: MutableSequence["VideoSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    label_detection_config = proto.Field(
+    label_detection_config: "LabelDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="LabelDetectionConfig",
     )
-    shot_change_detection_config = proto.Field(
+    shot_change_detection_config: "ShotChangeDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="ShotChangeDetectionConfig",
     )
-    explicit_content_detection_config = proto.Field(
+    explicit_content_detection_config: "ExplicitContentDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="ExplicitContentDetectionConfig",
     )
-    face_detection_config = proto.Field(
+    face_detection_config: "FaceDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="FaceDetectionConfig",
     )
-    speech_transcription_config = proto.Field(
+    speech_transcription_config: "SpeechTranscriptionConfig" = proto.Field(
         proto.MESSAGE,
         number=6,
         message="SpeechTranscriptionConfig",
     )
-    text_detection_config = proto.Field(
+    text_detection_config: "TextDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=8,
         message="TextDetectionConfig",
     )
-    person_detection_config = proto.Field(
+    person_detection_config: "PersonDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=11,
         message="PersonDetectionConfig",
     )
-    object_tracking_config = proto.Field(
+    object_tracking_config: "ObjectTrackingConfig" = proto.Field(
         proto.MESSAGE,
         number=13,
         message="ObjectTrackingConfig",
     )
 
 
 class LabelDetectionConfig(proto.Message):
@@ -305,32 +307,32 @@
             set to 0.3 by default. The valid range for this threshold is
             [0.1, 0.9]. Any value set outside of this range will be
             clipped. Note: For best results, follow the default
             threshold. We will update the default threshold everytime
             when we release a new model.
     """
 
-    label_detection_mode = proto.Field(
+    label_detection_mode: "LabelDetectionMode" = proto.Field(
         proto.ENUM,
         number=1,
         enum="LabelDetectionMode",
     )
-    stationary_camera = proto.Field(
+    stationary_camera: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    frame_confidence_threshold = proto.Field(
+    frame_confidence_threshold: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
-    video_confidence_threshold = proto.Field(
+    video_confidence_threshold: float = proto.Field(
         proto.FLOAT,
         number=5,
     )
 
 
 class ShotChangeDetectionConfig(proto.Message):
     r"""Config for SHOT_CHANGE_DETECTION.
@@ -338,15 +340,15 @@
     Attributes:
         model (str):
             Model to use for shot change detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ObjectTrackingConfig(proto.Message):
     r"""Config for OBJECT_TRACKING.
@@ -354,15 +356,15 @@
     Attributes:
         model (str):
             Model to use for object tracking.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ExplicitContentDetectionConfig(proto.Message):
     r"""Config for EXPLICIT_CONTENT_DETECTION.
@@ -370,15 +372,15 @@
     Attributes:
         model (str):
             Model to use for explicit content detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class FaceDetectionConfig(proto.Message):
     r"""Config for FACE_DETECTION.
@@ -393,23 +395,23 @@
             face annotation output.
         include_attributes (bool):
             Whether to enable face attributes detection, such as
             glasses, dark_glasses, mouth_open etc. Ignored if
             'include_bounding_boxes' is set to false.
     """
 
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    include_bounding_boxes = proto.Field(
+    include_bounding_boxes: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
-    include_attributes = proto.Field(
+    include_attributes: bool = proto.Field(
         proto.BOOL,
         number=5,
     )
 
 
 class PersonDetectionConfig(proto.Message):
     r"""Config for PERSON_DETECTION.
@@ -424,52 +426,52 @@
         include_attributes (bool):
             Whether to enable person attributes detection, such as cloth
             color (black, blue, etc), type (coat, dress, etc), pattern
             (plain, floral, etc), hair, etc. Ignored if
             'include_bounding_boxes' is set to false.
     """
 
-    include_bounding_boxes = proto.Field(
+    include_bounding_boxes: bool = proto.Field(
         proto.BOOL,
         number=1,
     )
-    include_pose_landmarks = proto.Field(
+    include_pose_landmarks: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
-    include_attributes = proto.Field(
+    include_attributes: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
 
 
 class TextDetectionConfig(proto.Message):
     r"""Config for TEXT_DETECTION.
 
     Attributes:
-        language_hints (Sequence[str]):
+        language_hints (MutableSequence[str]):
             Language hint can be specified if the
             language to be detected is known a priori. It
             can increase the accuracy of the detection.
             Language hint must be language code in BCP-47
             format.
 
             Automatic language detection is performed if no
             hint is provided.
         model (str):
             Model to use for text detection.
             Supported values: "builtin/stable" (the default
             if unset) and "builtin/latest".
     """
 
-    language_hints = proto.RepeatedField(
+    language_hints: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=1,
     )
-    model = proto.Field(
+    model: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class VideoSegment(proto.Message):
     r"""Video segment.
@@ -481,20 +483,20 @@
             (inclusive).
         end_time_offset (google.protobuf.duration_pb2.Duration):
             Time-offset, relative to the beginning of the
             video, corresponding to the end of the segment
             (inclusive).
     """
 
-    start_time_offset = proto.Field(
+    start_time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    end_time_offset = proto.Field(
+    end_time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class LabelSegment(proto.Message):
@@ -503,20 +505,20 @@
     Attributes:
         segment (google.cloud.videointelligence_v1p3beta1.types.VideoSegment):
             Video segment where a label was detected.
         confidence (float):
             Confidence that the label is accurate. Range: [0, 1].
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class LabelFrame(proto.Message):
     r"""Video frame level annotation results for label detection.
@@ -526,20 +528,20 @@
             Time-offset, relative to the beginning of the
             video, corresponding to the video frame for this
             location.
         confidence (float):
             Confidence that the label is accurate. Range: [0, 1].
     """
 
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class Entity(proto.Message):
     r"""Detected entity from video analysis.
@@ -551,62 +553,62 @@
             API <https://developers.google.com/knowledge-graph/>`__.
         description (str):
             Textual description, e.g., ``Fixed-gear bicycle``.
         language_code (str):
             Language code for ``description`` in BCP-47 format.
     """
 
-    entity_id = proto.Field(
+    entity_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class LabelAnnotation(proto.Message):
     r"""Label annotation.
 
     Attributes:
         entity (google.cloud.videointelligence_v1p3beta1.types.Entity):
             Detected entity.
-        category_entities (Sequence[google.cloud.videointelligence_v1p3beta1.types.Entity]):
+        category_entities (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.Entity]):
             Common categories for the detected entity. For example, when
             the label is ``Terrier``, the category is likely ``dog``.
             And in some cases there might be more than one categories
             e.g., ``Terrier`` could also be a ``pet``.
-        segments (Sequence[google.cloud.videointelligence_v1p3beta1.types.LabelSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.LabelSegment]):
             All video segments where a label was
             detected.
-        frames (Sequence[google.cloud.videointelligence_v1p3beta1.types.LabelFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.LabelFrame]):
             All video frames where a label was detected.
     """
 
-    entity = proto.Field(
+    entity: "Entity" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Entity",
     )
-    category_entities = proto.RepeatedField(
+    category_entities: MutableSequence["Entity"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="Entity",
     )
-    segments = proto.RepeatedField(
+    segments: MutableSequence["LabelSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="LabelSegment",
     )
-    frames = proto.RepeatedField(
+    frames: MutableSequence["LabelFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="LabelFrame",
     )
 
 
 class ExplicitContentFrame(proto.Message):
@@ -617,38 +619,38 @@
             Time-offset, relative to the beginning of the
             video, corresponding to the video frame for this
             location.
         pornography_likelihood (google.cloud.videointelligence_v1p3beta1.types.Likelihood):
             Likelihood of the pornography content..
     """
 
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    pornography_likelihood = proto.Field(
+    pornography_likelihood: "Likelihood" = proto.Field(
         proto.ENUM,
         number=2,
         enum="Likelihood",
     )
 
 
 class ExplicitContentAnnotation(proto.Message):
     r"""Explicit content annotation (based on per-frame visual
     signals only). If no explicit content has been detected in a
     frame, no annotations are present for that frame.
 
     Attributes:
-        frames (Sequence[google.cloud.videointelligence_v1p3beta1.types.ExplicitContentFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.ExplicitContentFrame]):
             All video frames where explicit content was
             detected.
     """
 
-    frames = proto.RepeatedField(
+    frames: MutableSequence["ExplicitContentFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="ExplicitContentFrame",
     )
 
 
 class NormalizedBoundingBox(proto.Message):
@@ -662,27 +664,27 @@
             Top Y coordinate.
         right (float):
             Right X coordinate.
         bottom (float):
             Bottom Y coordinate.
     """
 
-    left = proto.Field(
+    left: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    top = proto.Field(
+    top: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    right = proto.Field(
+    right: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
-    bottom = proto.Field(
+    bottom: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
 
 
 class TimestampedObject(proto.Message):
     r"""For tracking related features. An object at time_offset with
@@ -692,75 +694,75 @@
         normalized_bounding_box (google.cloud.videointelligence_v1p3beta1.types.NormalizedBoundingBox):
             Normalized Bounding box in a frame, where the
             object is located.
         time_offset (google.protobuf.duration_pb2.Duration):
             Time-offset, relative to the beginning of the
             video, corresponding to the video frame for this
             object.
-        attributes (Sequence[google.cloud.videointelligence_v1p3beta1.types.DetectedAttribute]):
+        attributes (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.DetectedAttribute]):
             Optional. The attributes of the object in the
             bounding box.
-        landmarks (Sequence[google.cloud.videointelligence_v1p3beta1.types.DetectedLandmark]):
+        landmarks (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.DetectedLandmark]):
             Optional. The detected landmarks.
     """
 
-    normalized_bounding_box = proto.Field(
+    normalized_bounding_box: "NormalizedBoundingBox" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="NormalizedBoundingBox",
     )
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
-    attributes = proto.RepeatedField(
+    attributes: MutableSequence["DetectedAttribute"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="DetectedAttribute",
     )
-    landmarks = proto.RepeatedField(
+    landmarks: MutableSequence["DetectedLandmark"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="DetectedLandmark",
     )
 
 
 class Track(proto.Message):
     r"""A track of an object instance.
 
     Attributes:
         segment (google.cloud.videointelligence_v1p3beta1.types.VideoSegment):
             Video segment of a track.
-        timestamped_objects (Sequence[google.cloud.videointelligence_v1p3beta1.types.TimestampedObject]):
+        timestamped_objects (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.TimestampedObject]):
             The object with timestamp and attributes per
             frame in the track.
-        attributes (Sequence[google.cloud.videointelligence_v1p3beta1.types.DetectedAttribute]):
+        attributes (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.DetectedAttribute]):
             Optional. Attributes in the track level.
         confidence (float):
             Optional. The confidence score of the tracked
             object.
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    timestamped_objects = proto.RepeatedField(
+    timestamped_objects: MutableSequence["TimestampedObject"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="TimestampedObject",
     )
-    attributes = proto.RepeatedField(
+    attributes: MutableSequence["DetectedAttribute"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="DetectedAttribute",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
 
 
 class DetectedAttribute(proto.Message):
     r"""A generic detected attribute represented by name in string
@@ -775,23 +777,23 @@
             Detected attribute confidence. Range [0, 1].
         value (str):
             Text value of the detection result. For
             example, the value for "HairColor" can be
             "black", "blonde", etc.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    value = proto.Field(
+    value: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class Celebrity(proto.Message):
     r"""Celebrity definition.
@@ -805,35 +807,35 @@
         display_name (str):
             The celebrity name.
         description (str):
             Textual description of additional information
             about the celebrity, if applicable.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class CelebrityTrack(proto.Message):
     r"""The annotation result of a celebrity face track.
     RecognizedCelebrity field could be empty if the face track does
     not have any matched celebrities.
 
     Attributes:
-        celebrities (Sequence[google.cloud.videointelligence_v1p3beta1.types.CelebrityTrack.RecognizedCelebrity]):
+        celebrities (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.CelebrityTrack.RecognizedCelebrity]):
             Top N match of the celebrities for the face
             in this track.
         face_track (google.cloud.videointelligence_v1p3beta1.types.Track):
             A track of a person's face.
     """
 
     class RecognizedCelebrity(proto.Message):
@@ -842,47 +844,47 @@
         Attributes:
             celebrity (google.cloud.videointelligence_v1p3beta1.types.Celebrity):
                 The recognized celebrity.
             confidence (float):
                 Recognition confidence. Range [0, 1].
         """
 
-        celebrity = proto.Field(
+        celebrity: "Celebrity" = proto.Field(
             proto.MESSAGE,
             number=1,
             message="Celebrity",
         )
-        confidence = proto.Field(
+        confidence: float = proto.Field(
             proto.FLOAT,
             number=2,
         )
 
-    celebrities = proto.RepeatedField(
+    celebrities: MutableSequence[RecognizedCelebrity] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=RecognizedCelebrity,
     )
-    face_track = proto.Field(
+    face_track: "Track" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="Track",
     )
 
 
 class CelebrityRecognitionAnnotation(proto.Message):
     r"""Celebrity recognition annotation per video.
 
     Attributes:
-        celebrity_tracks (Sequence[google.cloud.videointelligence_v1p3beta1.types.CelebrityTrack]):
+        celebrity_tracks (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.CelebrityTrack]):
             The tracks detected from the input video,
             including recognized celebrities and other
             detected faces in the video.
     """
 
-    celebrity_tracks = proto.RepeatedField(
+    celebrity_tracks: MutableSequence["CelebrityTrack"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="CelebrityTrack",
     )
 
 
 class DetectedLandmark(proto.Message):
@@ -898,59 +900,59 @@
             the normalized image coordindate system. The
             normalized coordinates have the range from 0 to
             1.
         confidence (float):
             The confidence score of the detected landmark. Range [0, 1].
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    point = proto.Field(
+    point: "NormalizedVertex" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="NormalizedVertex",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
 
 
 class FaceDetectionAnnotation(proto.Message):
     r"""Face detection annotation.
 
     Attributes:
-        tracks (Sequence[google.cloud.videointelligence_v1p3beta1.types.Track]):
+        tracks (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.Track]):
             The face tracks with attributes.
         thumbnail (bytes):
             The thumbnail of a person's face.
     """
 
-    tracks = proto.RepeatedField(
+    tracks: MutableSequence["Track"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="Track",
     )
-    thumbnail = proto.Field(
+    thumbnail: bytes = proto.Field(
         proto.BYTES,
         number=4,
     )
 
 
 class PersonDetectionAnnotation(proto.Message):
     r"""Person detection annotation per video.
 
     Attributes:
-        tracks (Sequence[google.cloud.videointelligence_v1p3beta1.types.Track]):
+        tracks (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.Track]):
             The detected tracks of a person.
     """
 
-    tracks = proto.RepeatedField(
+    tracks: MutableSequence["Track"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="Track",
     )
 
 
 class VideoAnnotationResults(proto.Message):
@@ -958,171 +960,183 @@
 
     Attributes:
         input_uri (str):
             Video file location in `Cloud
             Storage <https://cloud.google.com/storage/>`__.
         segment (google.cloud.videointelligence_v1p3beta1.types.VideoSegment):
             Video segment on which the annotation is run.
-        segment_label_annotations (Sequence[google.cloud.videointelligence_v1p3beta1.types.LabelAnnotation]):
+        segment_label_annotations (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.LabelAnnotation]):
             Topical label annotations on video level or
             user-specified segment level. There is exactly
             one element for each unique label.
-        segment_presence_label_annotations (Sequence[google.cloud.videointelligence_v1p3beta1.types.LabelAnnotation]):
+        segment_presence_label_annotations (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.LabelAnnotation]):
             Presence label annotations on video level or user-specified
             segment level. There is exactly one element for each unique
             label. Compared to the existing topical
             ``segment_label_annotations``, this field presents more
             fine-grained, segment-level labels detected in video content
             and is made available only when the client sets
             ``LabelDetectionConfig.model`` to "builtin/latest" in the
             request.
-        shot_label_annotations (Sequence[google.cloud.videointelligence_v1p3beta1.types.LabelAnnotation]):
+        shot_label_annotations (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.LabelAnnotation]):
             Topical label annotations on shot level.
             There is exactly one element for each unique
             label.
-        shot_presence_label_annotations (Sequence[google.cloud.videointelligence_v1p3beta1.types.LabelAnnotation]):
+        shot_presence_label_annotations (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.LabelAnnotation]):
             Presence label annotations on shot level. There is exactly
             one element for each unique label. Compared to the existing
             topical ``shot_label_annotations``, this field presents more
             fine-grained, shot-level labels detected in video content
             and is made available only when the client sets
             ``LabelDetectionConfig.model`` to "builtin/latest" in the
             request.
-        frame_label_annotations (Sequence[google.cloud.videointelligence_v1p3beta1.types.LabelAnnotation]):
+        frame_label_annotations (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.LabelAnnotation]):
             Label annotations on frame level.
             There is exactly one element for each unique
             label.
-        face_detection_annotations (Sequence[google.cloud.videointelligence_v1p3beta1.types.FaceDetectionAnnotation]):
+        face_detection_annotations (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.FaceDetectionAnnotation]):
             Face detection annotations.
-        shot_annotations (Sequence[google.cloud.videointelligence_v1p3beta1.types.VideoSegment]):
+        shot_annotations (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.VideoSegment]):
             Shot annotations. Each shot is represented as
             a video segment.
         explicit_annotation (google.cloud.videointelligence_v1p3beta1.types.ExplicitContentAnnotation):
             Explicit content annotation.
-        speech_transcriptions (Sequence[google.cloud.videointelligence_v1p3beta1.types.SpeechTranscription]):
+        speech_transcriptions (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.SpeechTranscription]):
             Speech transcription.
-        text_annotations (Sequence[google.cloud.videointelligence_v1p3beta1.types.TextAnnotation]):
+        text_annotations (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.TextAnnotation]):
             OCR text detection and tracking.
             Annotations for list of detected text snippets.
             Each will have list of frame information
             associated with it.
-        object_annotations (Sequence[google.cloud.videointelligence_v1p3beta1.types.ObjectTrackingAnnotation]):
+        object_annotations (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.ObjectTrackingAnnotation]):
             Annotations for list of objects detected and
             tracked in video.
-        logo_recognition_annotations (Sequence[google.cloud.videointelligence_v1p3beta1.types.LogoRecognitionAnnotation]):
+        logo_recognition_annotations (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.LogoRecognitionAnnotation]):
             Annotations for list of logos detected,
             tracked and recognized in video.
-        person_detection_annotations (Sequence[google.cloud.videointelligence_v1p3beta1.types.PersonDetectionAnnotation]):
+        person_detection_annotations (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.PersonDetectionAnnotation]):
             Person detection annotations.
         celebrity_recognition_annotations (google.cloud.videointelligence_v1p3beta1.types.CelebrityRecognitionAnnotation):
             Celebrity recognition annotations.
         error (google.rpc.status_pb2.Status):
             If set, indicates an error. Note that for a single
             ``AnnotateVideoRequest`` some videos may succeed and some
             may fail.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=10,
         message="VideoSegment",
     )
-    segment_label_annotations = proto.RepeatedField(
+    segment_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="LabelAnnotation",
     )
-    segment_presence_label_annotations = proto.RepeatedField(
+    segment_presence_label_annotations: MutableSequence[
+        "LabelAnnotation"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=23,
         message="LabelAnnotation",
     )
-    shot_label_annotations = proto.RepeatedField(
+    shot_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="LabelAnnotation",
     )
-    shot_presence_label_annotations = proto.RepeatedField(
+    shot_presence_label_annotations: MutableSequence[
+        "LabelAnnotation"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=24,
         message="LabelAnnotation",
     )
-    frame_label_annotations = proto.RepeatedField(
+    frame_label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="LabelAnnotation",
     )
-    face_detection_annotations = proto.RepeatedField(
+    face_detection_annotations: MutableSequence[
+        "FaceDetectionAnnotation"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=13,
         message="FaceDetectionAnnotation",
     )
-    shot_annotations = proto.RepeatedField(
+    shot_annotations: MutableSequence["VideoSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=6,
         message="VideoSegment",
     )
-    explicit_annotation = proto.Field(
+    explicit_annotation: "ExplicitContentAnnotation" = proto.Field(
         proto.MESSAGE,
         number=7,
         message="ExplicitContentAnnotation",
     )
-    speech_transcriptions = proto.RepeatedField(
+    speech_transcriptions: MutableSequence["SpeechTranscription"] = proto.RepeatedField(
         proto.MESSAGE,
         number=11,
         message="SpeechTranscription",
     )
-    text_annotations = proto.RepeatedField(
+    text_annotations: MutableSequence["TextAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=12,
         message="TextAnnotation",
     )
-    object_annotations = proto.RepeatedField(
+    object_annotations: MutableSequence[
+        "ObjectTrackingAnnotation"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=14,
         message="ObjectTrackingAnnotation",
     )
-    logo_recognition_annotations = proto.RepeatedField(
+    logo_recognition_annotations: MutableSequence[
+        "LogoRecognitionAnnotation"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=19,
         message="LogoRecognitionAnnotation",
     )
-    person_detection_annotations = proto.RepeatedField(
+    person_detection_annotations: MutableSequence[
+        "PersonDetectionAnnotation"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=20,
         message="PersonDetectionAnnotation",
     )
-    celebrity_recognition_annotations = proto.Field(
+    celebrity_recognition_annotations: "CelebrityRecognitionAnnotation" = proto.Field(
         proto.MESSAGE,
         number=21,
         message="CelebrityRecognitionAnnotation",
     )
-    error = proto.Field(
+    error: status_pb2.Status = proto.Field(
         proto.MESSAGE,
         number=9,
         message=status_pb2.Status,
     )
 
 
 class AnnotateVideoResponse(proto.Message):
     r"""Video annotation response. Included in the ``response`` field of the
     ``Operation`` returned by the ``GetOperation`` call of the
     ``google::longrunning::Operations`` service.
 
     Attributes:
-        annotation_results (Sequence[google.cloud.videointelligence_v1p3beta1.types.VideoAnnotationResults]):
+        annotation_results (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.VideoAnnotationResults]):
             Annotation results for all videos specified in
             ``AnnotateVideoRequest``.
     """
 
-    annotation_results = proto.RepeatedField(
+    annotation_results: MutableSequence["VideoAnnotationResults"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoAnnotationResults",
     )
 
 
 class VideoAnnotationProgress(proto.Message):
@@ -1143,56 +1157,58 @@
             Specifies which feature is being tracked if
             the request contains more than one feature.
         segment (google.cloud.videointelligence_v1p3beta1.types.VideoSegment):
             Specifies which segment is being tracked if
             the request contains more than one segment.
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    progress_percent = proto.Field(
+    progress_percent: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    start_time = proto.Field(
+    start_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
-    feature = proto.Field(
+    feature: "Feature" = proto.Field(
         proto.ENUM,
         number=5,
         enum="Feature",
     )
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=6,
         message="VideoSegment",
     )
 
 
 class AnnotateVideoProgress(proto.Message):
     r"""Video annotation progress. Included in the ``metadata`` field of the
     ``Operation`` returned by the ``GetOperation`` call of the
     ``google::longrunning::Operations`` service.
 
     Attributes:
-        annotation_progress (Sequence[google.cloud.videointelligence_v1p3beta1.types.VideoAnnotationProgress]):
+        annotation_progress (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.VideoAnnotationProgress]):
             Progress metadata for all videos specified in
             ``AnnotateVideoRequest``.
     """
 
-    annotation_progress = proto.RepeatedField(
+    annotation_progress: MutableSequence[
+        "VideoAnnotationProgress"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoAnnotationProgress",
     )
 
 
 class SpeechTranscriptionConfig(proto.Message):
@@ -1215,29 +1231,29 @@
             will return a maximum of one.
         filter_profanity (bool):
             Optional. If set to ``true``, the server will attempt to
             filter out profanities, replacing all but the initial
             character in each filtered word with asterisks, e.g. "f***".
             If set to ``false`` or omitted, profanities won't be
             filtered out.
-        speech_contexts (Sequence[google.cloud.videointelligence_v1p3beta1.types.SpeechContext]):
+        speech_contexts (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.SpeechContext]):
             Optional. A means to provide context to
             assist the speech recognition.
         enable_automatic_punctuation (bool):
             Optional. If 'true', adds punctuation to
             recognition result hypotheses. This feature is
             only available in select languages. Setting this
             for requests in other languages has no effect at
             all. The default 'false' value does not add
             punctuation to result hypotheses. NOTE: "This is
             currently offered as an experimental service,
             complimentary to all users. In the future this
             may be exclusively available as a premium
             feature.".
-        audio_tracks (Sequence[int]):
+        audio_tracks (MutableSequence[int]):
             Optional. For file formats, such as MXF or
             MKV, supporting multiple audio tracks, specify
             up to two tracks. Default: track 0.
         enable_speaker_diarization (bool):
             Optional. If 'true', enables speaker detection for each
             recognized word in the top alternative of the recognition
             result using a speaker_tag provided in the WordInfo. Note:
@@ -1253,100 +1269,100 @@
         enable_word_confidence (bool):
             Optional. If ``true``, the top result includes a list of
             words and the confidence for those words. If ``false``, no
             word-level confidence information is returned. The default
             is ``false``.
     """
 
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    max_alternatives = proto.Field(
+    max_alternatives: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    filter_profanity = proto.Field(
+    filter_profanity: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
-    speech_contexts = proto.RepeatedField(
+    speech_contexts: MutableSequence["SpeechContext"] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="SpeechContext",
     )
-    enable_automatic_punctuation = proto.Field(
+    enable_automatic_punctuation: bool = proto.Field(
         proto.BOOL,
         number=5,
     )
-    audio_tracks = proto.RepeatedField(
+    audio_tracks: MutableSequence[int] = proto.RepeatedField(
         proto.INT32,
         number=6,
     )
-    enable_speaker_diarization = proto.Field(
+    enable_speaker_diarization: bool = proto.Field(
         proto.BOOL,
         number=7,
     )
-    diarization_speaker_count = proto.Field(
+    diarization_speaker_count: int = proto.Field(
         proto.INT32,
         number=8,
     )
-    enable_word_confidence = proto.Field(
+    enable_word_confidence: bool = proto.Field(
         proto.BOOL,
         number=9,
     )
 
 
 class SpeechContext(proto.Message):
     r"""Provides "hints" to the speech recognizer to favor specific
     words and phrases in the results.
 
     Attributes:
-        phrases (Sequence[str]):
+        phrases (MutableSequence[str]):
             Optional. A list of strings containing words and phrases
             "hints" so that the speech recognition is more likely to
             recognize them. This can be used to improve the accuracy for
             specific words and phrases, for example, if specific
             commands are typically spoken by the user. This can also be
             used to add additional words to the vocabulary of the
             recognizer. See `usage
             limits <https://cloud.google.com/speech/limits#content>`__.
     """
 
-    phrases = proto.RepeatedField(
+    phrases: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=1,
     )
 
 
 class SpeechTranscription(proto.Message):
     r"""A speech recognition result corresponding to a portion of the
     audio.
 
     Attributes:
-        alternatives (Sequence[google.cloud.videointelligence_v1p3beta1.types.SpeechRecognitionAlternative]):
+        alternatives (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.SpeechRecognitionAlternative]):
             May contain one or more recognition hypotheses (up to the
             maximum specified in ``max_alternatives``). These
             alternatives are ordered in terms of accuracy, with the top
             (first) alternative being the most probable, as ranked by
             the recognizer.
         language_code (str):
             Output only. The
             `BCP-47 <https://www.rfc-editor.org/rfc/bcp/bcp47.txt>`__
             language tag of the language in this result. This language
             code was detected to have the most likelihood of being
             spoken in the audio.
     """
 
-    alternatives = proto.RepeatedField(
+    alternatives: MutableSequence["SpeechRecognitionAlternative"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="SpeechRecognitionAlternative",
     )
-    language_code = proto.Field(
+    language_code: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class SpeechRecognitionAlternative(proto.Message):
     r"""Alternative hypotheses (a.k.a. n-best list).
@@ -1359,30 +1375,30 @@
             Output only. The confidence estimate between 0.0 and 1.0. A
             higher number indicates an estimated greater likelihood that
             the recognized words are correct. This field is set only for
             the top alternative. This field is not guaranteed to be
             accurate and users should not rely on it to be always
             provided. The default of 0.0 is a sentinel value indicating
             ``confidence`` was not set.
-        words (Sequence[google.cloud.videointelligence_v1p3beta1.types.WordInfo]):
+        words (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.WordInfo]):
             Output only. A list of word-specific information for each
             recognized word. Note: When ``enable_speaker_diarization``
             is set to true, you will see all the words from the
             beginning of the audio.
     """
 
-    transcript = proto.Field(
+    transcript: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    words = proto.RepeatedField(
+    words: MutableSequence["WordInfo"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="WordInfo",
     )
 
 
 class WordInfo(proto.Message):
@@ -1418,33 +1434,33 @@
             Output only. A distinct integer value is assigned for every
             speaker within the audio. This field specifies which one of
             those speakers was detected to have spoken this word. Value
             ranges from 1 up to diarization_speaker_count, and is only
             set if speaker diarization is enabled.
     """
 
-    start_time = proto.Field(
+    start_time: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    end_time = proto.Field(
+    end_time: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
-    word = proto.Field(
+    word: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
-    speaker_tag = proto.Field(
+    speaker_tag: int = proto.Field(
         proto.INT32,
         number=5,
     )
 
 
 class NormalizedVertex(proto.Message):
     r"""A vertex represents a 2D point in the image.
@@ -1454,19 +1470,19 @@
     Attributes:
         x (float):
             X coordinate.
         y (float):
             Y coordinate.
     """
 
-    x = proto.Field(
+    x: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    y = proto.Field(
+    y: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class NormalizedBoundingPoly(proto.Message):
     r"""Normalized bounding polygon for text (that might not be aligned with
@@ -1479,19 +1495,19 @@
     it becomes: 2----3 \| \| 1----0
 
     and the vertex order will still be (0, 1, 2, 3). Note that values
     can be less than 0, or greater than 1 due to trignometric
     calculations for location of the box.
 
     Attributes:
-        vertices (Sequence[google.cloud.videointelligence_v1p3beta1.types.NormalizedVertex]):
+        vertices (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.NormalizedVertex]):
             Normalized vertices of the bounding polygon.
     """
 
-    vertices = proto.RepeatedField(
+    vertices: MutableSequence["NormalizedVertex"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="NormalizedVertex",
     )
 
 
 class TextSegment(proto.Message):
@@ -1501,29 +1517,29 @@
         segment (google.cloud.videointelligence_v1p3beta1.types.VideoSegment):
             Video segment where a text snippet was
             detected.
         confidence (float):
             Confidence for the track of detected text. It
             is calculated as the highest over all frames
             where OCR detected text appears.
-        frames (Sequence[google.cloud.videointelligence_v1p3beta1.types.TextFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.TextFrame]):
             Information related to the frames where OCR
             detected text appears.
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    frames = proto.RepeatedField(
+    frames: MutableSequence["TextFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="TextFrame",
     )
 
 
 class TextFrame(proto.Message):
@@ -1535,44 +1551,44 @@
         rotated_bounding_box (google.cloud.videointelligence_v1p3beta1.types.NormalizedBoundingPoly):
             Bounding polygon of the detected text for
             this frame.
         time_offset (google.protobuf.duration_pb2.Duration):
             Timestamp of this frame.
     """
 
-    rotated_bounding_box = proto.Field(
+    rotated_bounding_box: "NormalizedBoundingPoly" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="NormalizedBoundingPoly",
     )
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class TextAnnotation(proto.Message):
     r"""Annotations related to one detected OCR text snippet. This
     will contain the corresponding text, confidence value, and frame
     level information for each detection.
 
     Attributes:
         text (str):
             The detected text.
-        segments (Sequence[google.cloud.videointelligence_v1p3beta1.types.TextSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.TextSegment]):
             All video segments where OCR detected text
             appears.
     """
 
-    text = proto.Field(
+    text: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    segments = proto.RepeatedField(
+    segments: MutableSequence["TextSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="TextSegment",
     )
 
 
 class ObjectTrackingFrame(proto.Message):
@@ -1584,20 +1600,20 @@
         normalized_bounding_box (google.cloud.videointelligence_v1p3beta1.types.NormalizedBoundingBox):
             The normalized bounding box location of this
             object track for the frame.
         time_offset (google.protobuf.duration_pb2.Duration):
             The timestamp of the frame in microseconds.
     """
 
-    normalized_bounding_box = proto.Field(
+    normalized_bounding_box: "NormalizedBoundingBox" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="NormalizedBoundingBox",
     )
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 class ObjectTrackingAnnotation(proto.Message):
@@ -1628,44 +1644,44 @@
             This field is a member of `oneof`_ ``track_info``.
         entity (google.cloud.videointelligence_v1p3beta1.types.Entity):
             Entity to specify the object category that
             this track is labeled as.
         confidence (float):
             Object category's labeling confidence of this
             track.
-        frames (Sequence[google.cloud.videointelligence_v1p3beta1.types.ObjectTrackingFrame]):
+        frames (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.ObjectTrackingFrame]):
             Information corresponding to all frames where
             this object track appears. Non-streaming batch
             mode: it may be one or multiple
             ObjectTrackingFrame messages in frames.
             Streaming mode: it can only be one
             ObjectTrackingFrame message in frames.
     """
 
-    segment = proto.Field(
+    segment: "VideoSegment" = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="track_info",
         message="VideoSegment",
     )
-    track_id = proto.Field(
+    track_id: int = proto.Field(
         proto.INT64,
         number=5,
         oneof="track_info",
     )
-    entity = proto.Field(
+    entity: "Entity" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Entity",
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
-    frames = proto.RepeatedField(
+    frames: MutableSequence["ObjectTrackingFrame"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="ObjectTrackingFrame",
     )
 
 
 class LogoRecognitionAnnotation(proto.Message):
@@ -1673,36 +1689,36 @@
     recognized logo class.
 
     Attributes:
         entity (google.cloud.videointelligence_v1p3beta1.types.Entity):
             Entity category information to specify the
             logo class that all the logo tracks within this
             LogoRecognitionAnnotation are recognized as.
-        tracks (Sequence[google.cloud.videointelligence_v1p3beta1.types.Track]):
+        tracks (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.Track]):
             All logo tracks where the recognized logo
             appears. Each track corresponds to one logo
             instance appearing in consecutive frames.
-        segments (Sequence[google.cloud.videointelligence_v1p3beta1.types.VideoSegment]):
+        segments (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.VideoSegment]):
             All video segments where the recognized logo
             appears. There might be multiple instances of
             the same logo class appearing in one
             VideoSegment.
     """
 
-    entity = proto.Field(
+    entity: "Entity" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Entity",
     )
-    tracks = proto.RepeatedField(
+    tracks: MutableSequence["Track"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="Track",
     )
-    segments = proto.RepeatedField(
+    segments: MutableSequence["VideoSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="VideoSegment",
     )
 
 
 class StreamingAnnotateVideoRequest(proto.Message):
@@ -1736,21 +1752,21 @@
             ``AnnotateStreamingVideoRequest`` messages must only contain
             ``input_content`` field. Note: as with all bytes fields,
             protobuffers use a pure binary representation (not base64).
 
             This field is a member of `oneof`_ ``streaming_request``.
     """
 
-    video_config = proto.Field(
+    video_config: "StreamingVideoConfig" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="streaming_request",
         message="StreamingVideoConfig",
     )
-    input_content = proto.Field(
+    input_content: bytes = proto.Field(
         proto.BYTES,
         number=2,
         oneof="streaming_request",
     )
 
 
 class StreamingVideoConfig(proto.Message):
@@ -1796,62 +1812,66 @@
         feature (google.cloud.videointelligence_v1p3beta1.types.StreamingFeature):
             Requested annotation feature.
         storage_config (google.cloud.videointelligence_v1p3beta1.types.StreamingStorageConfig):
             Streaming storage option. By default: storage
             is disabled.
     """
 
-    shot_change_detection_config = proto.Field(
+    shot_change_detection_config: "StreamingShotChangeDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="streaming_config",
         message="StreamingShotChangeDetectionConfig",
     )
-    label_detection_config = proto.Field(
+    label_detection_config: "StreamingLabelDetectionConfig" = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="streaming_config",
         message="StreamingLabelDetectionConfig",
     )
-    explicit_content_detection_config = proto.Field(
-        proto.MESSAGE,
-        number=4,
-        oneof="streaming_config",
-        message="StreamingExplicitContentDetectionConfig",
+    explicit_content_detection_config: "StreamingExplicitContentDetectionConfig" = (
+        proto.Field(
+            proto.MESSAGE,
+            number=4,
+            oneof="streaming_config",
+            message="StreamingExplicitContentDetectionConfig",
+        )
     )
-    object_tracking_config = proto.Field(
+    object_tracking_config: "StreamingObjectTrackingConfig" = proto.Field(
         proto.MESSAGE,
         number=5,
         oneof="streaming_config",
         message="StreamingObjectTrackingConfig",
     )
-    automl_action_recognition_config = proto.Field(
-        proto.MESSAGE,
-        number=23,
-        oneof="streaming_config",
-        message="StreamingAutomlActionRecognitionConfig",
+    automl_action_recognition_config: "StreamingAutomlActionRecognitionConfig" = (
+        proto.Field(
+            proto.MESSAGE,
+            number=23,
+            oneof="streaming_config",
+            message="StreamingAutomlActionRecognitionConfig",
+        )
     )
-    automl_classification_config = proto.Field(
+    automl_classification_config: "StreamingAutomlClassificationConfig" = proto.Field(
         proto.MESSAGE,
         number=21,
         oneof="streaming_config",
         message="StreamingAutomlClassificationConfig",
     )
-    automl_object_tracking_config = proto.Field(
+    automl_object_tracking_config: "StreamingAutomlObjectTrackingConfig" = proto.Field(
         proto.MESSAGE,
         number=22,
         oneof="streaming_config",
         message="StreamingAutomlObjectTrackingConfig",
     )
-    feature = proto.Field(
+    feature: "StreamingFeature" = proto.Field(
         proto.ENUM,
         number=1,
         enum="StreamingFeature",
     )
-    storage_config = proto.Field(
+    storage_config: "StreamingStorageConfig" = proto.Field(
         proto.MESSAGE,
         number=30,
         message="StreamingStorageConfig",
     )
 
 
 class StreamingAnnotateVideoResponse(proto.Message):
@@ -1869,62 +1889,64 @@
         annotation_results_uri (str):
             Google Cloud Storage(GCS) URI that stores annotation results
             of one streaming session in JSON format. It is the
             annotation_result_storage_directory from the request
             followed by '/cloud_project_number-session_id'.
     """
 
-    error = proto.Field(
+    error: status_pb2.Status = proto.Field(
         proto.MESSAGE,
         number=1,
         message=status_pb2.Status,
     )
-    annotation_results = proto.Field(
+    annotation_results: "StreamingVideoAnnotationResults" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="StreamingVideoAnnotationResults",
     )
-    annotation_results_uri = proto.Field(
+    annotation_results_uri: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class StreamingVideoAnnotationResults(proto.Message):
     r"""Streaming annotation results corresponding to a portion of
     the video that is currently being processed.
 
     Attributes:
-        shot_annotations (Sequence[google.cloud.videointelligence_v1p3beta1.types.VideoSegment]):
+        shot_annotations (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.VideoSegment]):
             Shot annotation results. Each shot is
             represented as a video segment.
-        label_annotations (Sequence[google.cloud.videointelligence_v1p3beta1.types.LabelAnnotation]):
+        label_annotations (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.LabelAnnotation]):
             Label annotation results.
         explicit_annotation (google.cloud.videointelligence_v1p3beta1.types.ExplicitContentAnnotation):
             Explicit content annotation results.
-        object_annotations (Sequence[google.cloud.videointelligence_v1p3beta1.types.ObjectTrackingAnnotation]):
+        object_annotations (MutableSequence[google.cloud.videointelligence_v1p3beta1.types.ObjectTrackingAnnotation]):
             Object tracking results.
     """
 
-    shot_annotations = proto.RepeatedField(
+    shot_annotations: MutableSequence["VideoSegment"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="VideoSegment",
     )
-    label_annotations = proto.RepeatedField(
+    label_annotations: MutableSequence["LabelAnnotation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="LabelAnnotation",
     )
-    explicit_annotation = proto.Field(
+    explicit_annotation: "ExplicitContentAnnotation" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="ExplicitContentAnnotation",
     )
-    object_annotations = proto.RepeatedField(
+    object_annotations: MutableSequence[
+        "ObjectTrackingAnnotation"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="ObjectTrackingAnnotation",
     )
 
 
 class StreamingShotChangeDetectionConfig(proto.Message):
@@ -1938,15 +1960,15 @@
         stationary_camera (bool):
             Whether the video has been captured from a
             stationary (i.e. non-moving) camera. When set to
             true, might improve detection accuracy for
             moving objects. Default: false.
     """
 
-    stationary_camera = proto.Field(
+    stationary_camera: bool = proto.Field(
         proto.BOOL,
         number=1,
     )
 
 
 class StreamingExplicitContentDetectionConfig(proto.Message):
     r"""Config for STREAMING_EXPLICIT_CONTENT_DETECTION."""
@@ -1961,45 +1983,45 @@
 
     Attributes:
         model_name (str):
             Resource name of AutoML model. Format:
             ``projects/{project_id}/locations/{location_id}/models/{model_id}``
     """
 
-    model_name = proto.Field(
+    model_name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class StreamingAutomlClassificationConfig(proto.Message):
     r"""Config for STREAMING_AUTOML_CLASSIFICATION.
 
     Attributes:
         model_name (str):
             Resource name of AutoML model. Format:
             ``projects/{project_number}/locations/{location_id}/models/{model_id}``
     """
 
-    model_name = proto.Field(
+    model_name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class StreamingAutomlObjectTrackingConfig(proto.Message):
     r"""Config for STREAMING_AUTOML_OBJECT_TRACKING.
 
     Attributes:
         model_name (str):
             Resource name of AutoML model. Format:
             ``projects/{project_id}/locations/{location_id}/models/{model_id}``
     """
 
-    model_name = proto.Field(
+    model_name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class StreamingStorageConfig(proto.Message):
     r"""Config for streaming storage option.
@@ -2019,18 +2041,18 @@
             should be a valid Cloud Storage bucket created by client and
             bucket permission shall also be configured properly.
             ``object-id`` can be arbitrary string that make sense to
             client. Other URI formats will return error and cause Cloud
             Storage write failure.
     """
 
-    enable_storage_annotation_result = proto.Field(
+    enable_storage_annotation_result: bool = proto.Field(
         proto.BOOL,
         number=1,
     )
-    annotation_result_storage_directory = proto.Field(
+    annotation_result_storage_directory: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-videointelligence-2.8.3/google_cloud_videointelligence.egg-info/PKG-INFO` & `google-cloud-videointelligence-2.9.0/google_cloud_videointelligence.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: google-cloud-videointelligence
-Version: 2.8.3
-Summary: Google Cloud Video Intelligence API client library
+Version: 2.9.0
+Summary: Google Cloud Videointelligence API client library
 Home-page: https://github.com/googleapis/python-videointelligence
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
-Provides-Extra: libcst
 License-File: LICENSE
 
 Python Client for Video Intelligence API
 ========================================
 
 |stable| |pypi| |versions|
```

### Comparing `google-cloud-videointelligence-2.8.3/google_cloud_videointelligence.egg-info/SOURCES.txt` & `google-cloud-videointelligence-2.9.0/google_cloud_videointelligence.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,68 +1,74 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 google/cloud/videointelligence/__init__.py
+google/cloud/videointelligence/gapic_version.py
 google/cloud/videointelligence/py.typed
 google/cloud/videointelligence_v1/__init__.py
 google/cloud/videointelligence_v1/gapic_metadata.json
+google/cloud/videointelligence_v1/gapic_version.py
 google/cloud/videointelligence_v1/py.typed
 google/cloud/videointelligence_v1/services/__init__.py
 google/cloud/videointelligence_v1/services/video_intelligence_service/__init__.py
 google/cloud/videointelligence_v1/services/video_intelligence_service/async_client.py
 google/cloud/videointelligence_v1/services/video_intelligence_service/client.py
 google/cloud/videointelligence_v1/services/video_intelligence_service/transports/__init__.py
 google/cloud/videointelligence_v1/services/video_intelligence_service/transports/base.py
 google/cloud/videointelligence_v1/services/video_intelligence_service/transports/grpc.py
 google/cloud/videointelligence_v1/services/video_intelligence_service/transports/grpc_asyncio.py
 google/cloud/videointelligence_v1/types/__init__.py
 google/cloud/videointelligence_v1/types/video_intelligence.py
 google/cloud/videointelligence_v1beta2/__init__.py
 google/cloud/videointelligence_v1beta2/gapic_metadata.json
+google/cloud/videointelligence_v1beta2/gapic_version.py
 google/cloud/videointelligence_v1beta2/py.typed
 google/cloud/videointelligence_v1beta2/services/__init__.py
 google/cloud/videointelligence_v1beta2/services/video_intelligence_service/__init__.py
 google/cloud/videointelligence_v1beta2/services/video_intelligence_service/async_client.py
 google/cloud/videointelligence_v1beta2/services/video_intelligence_service/client.py
 google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/__init__.py
 google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/base.py
 google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/grpc.py
 google/cloud/videointelligence_v1beta2/services/video_intelligence_service/transports/grpc_asyncio.py
 google/cloud/videointelligence_v1beta2/types/__init__.py
 google/cloud/videointelligence_v1beta2/types/video_intelligence.py
 google/cloud/videointelligence_v1p1beta1/__init__.py
 google/cloud/videointelligence_v1p1beta1/gapic_metadata.json
+google/cloud/videointelligence_v1p1beta1/gapic_version.py
 google/cloud/videointelligence_v1p1beta1/py.typed
 google/cloud/videointelligence_v1p1beta1/services/__init__.py
 google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/__init__.py
 google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/async_client.py
 google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/client.py
 google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/__init__.py
 google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/base.py
 google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/grpc.py
 google/cloud/videointelligence_v1p1beta1/services/video_intelligence_service/transports/grpc_asyncio.py
 google/cloud/videointelligence_v1p1beta1/types/__init__.py
 google/cloud/videointelligence_v1p1beta1/types/video_intelligence.py
 google/cloud/videointelligence_v1p2beta1/__init__.py
 google/cloud/videointelligence_v1p2beta1/gapic_metadata.json
+google/cloud/videointelligence_v1p2beta1/gapic_version.py
 google/cloud/videointelligence_v1p2beta1/py.typed
 google/cloud/videointelligence_v1p2beta1/services/__init__.py
 google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/__init__.py
 google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/async_client.py
 google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/client.py
 google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/__init__.py
 google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/base.py
 google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/grpc.py
 google/cloud/videointelligence_v1p2beta1/services/video_intelligence_service/transports/grpc_asyncio.py
 google/cloud/videointelligence_v1p2beta1/types/__init__.py
 google/cloud/videointelligence_v1p2beta1/types/video_intelligence.py
 google/cloud/videointelligence_v1p3beta1/__init__.py
 google/cloud/videointelligence_v1p3beta1/gapic_metadata.json
+google/cloud/videointelligence_v1p3beta1/gapic_version.py
 google/cloud/videointelligence_v1p3beta1/py.typed
 google/cloud/videointelligence_v1p3beta1/services/__init__.py
 google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/__init__.py
 google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/async_client.py
 google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/client.py
 google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/__init__.py
 google/cloud/videointelligence_v1p3beta1/services/streaming_video_intelligence_service/transports/base.py
@@ -80,15 +86,14 @@
 google_cloud_videointelligence.egg-info/PKG-INFO
 google_cloud_videointelligence.egg-info/SOURCES.txt
 google_cloud_videointelligence.egg-info/dependency_links.txt
 google_cloud_videointelligence.egg-info/namespace_packages.txt
 google_cloud_videointelligence.egg-info/not-zip-safe
 google_cloud_videointelligence.egg-info/requires.txt
 google_cloud_videointelligence.egg-info/top_level.txt
-scripts/fixup_keywords.py
 tests/__init__.py
 tests/system/test_system.py
 tests/system/test_vpcsc.py
 tests/unit/__init__.py
 tests/unit/gapic/__init__.py
 tests/unit/gapic/videointelligence_v1/__init__.py
 tests/unit/gapic/videointelligence_v1/test_video_intelligence_service.py
```

### Comparing `google-cloud-videointelligence-2.8.3/setup.py` & `google-cloud-videointelligence-2.9.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,78 @@
-# Copyright 2018 Google LLC
+# -*- coding: utf-8 -*-
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+#
 import io
 import os
 
-import setuptools
+import setuptools  # type: ignore
 
-# Package metadata.
+package_root = os.path.abspath(os.path.dirname(__file__))
 
 name = "google-cloud-videointelligence"
-description = "Google Cloud Video Intelligence API client library"
-version = "2.8.3"
-# Should be one of:
-# 'Development Status :: 3 - Alpha'
-# 'Development Status :: 4 - Beta'
-# 'Development Status :: 5 - Production/Stable'
-release_status = "Development Status :: 5 - Production/Stable"
+
+
+description = "Google Cloud Videointelligence API client library"
+
+version = {}
+with open(
+    os.path.join(package_root, "google/cloud/videointelligence/gapic_version.py")
+) as fp:
+    exec(fp.read(), version)
+version = version["__version__"]
+
+if version[0] == "0":
+    release_status = "Development Status :: 4 - Beta"
+else:
+    release_status = "Development Status :: 5 - Production/Stable"
+
 dependencies = [
-    "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
+    "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-extras = {"libcst": "libcst >= 0.2.5"}
-scripts = ["scripts/fixup_keywords.py"]
-
-
-# Setup boilerplate below this line.
+url = "https://github.com/googleapis/python-videointelligence"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
-# Only include packages under the 'google' namespace. Do not include tests,
-# benchmarks, etc.
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("google")
 ]
 
-# Determine which namespaces are needed.
 namespaces = ["google"]
 if "google.cloud" in packages:
     namespaces.append("google.cloud")
 
-
 setuptools.setup(
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
     author_email="googleapis-packages@google.com",
     license="Apache 2.0",
-    url="https://github.com/googleapis/python-videointelligence",
+    url=url,
     classifiers=[
         release_status,
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
@@ -78,15 +80,13 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "Topic :: Internet",
     ],
     platforms="Posix; MacOS X; Windows",
     packages=packages,
+    python_requires=">=3.7",
     namespace_packages=namespaces,
     install_requires=dependencies,
-    extras_require=extras,
-    python_requires=">=3.7",
-    scripts=scripts,
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `google-cloud-videointelligence-2.8.3/tests/__init__.py` & `google-cloud-videointelligence-2.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/system/test_system.py` & `google-cloud-videointelligence-2.9.0/tests/system/test_system.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/system/test_vpcsc.py` & `google-cloud-videointelligence-2.9.0/tests/system/test_vpcsc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/unit/__init__.py` & `google-cloud-videointelligence-2.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/unit/gapic/__init__.py` & `google-cloud-videointelligence-2.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1/__init__.py` & `google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1/test_video_intelligence_service.py` & `google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1/test_video_intelligence_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1beta2/__init__.py` & `google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1beta2/test_video_intelligence_service.py` & `google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1beta2/test_video_intelligence_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p1beta1/__init__.py` & `google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p1beta1/test_video_intelligence_service.py` & `google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p1beta1/test_video_intelligence_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p2beta1/__init__.py` & `google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p2beta1/test_video_intelligence_service.py` & `google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p2beta1/test_video_intelligence_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p3beta1/__init__.py` & `google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p3beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p3beta1/test_streaming_video_intelligence_service.py` & `google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p3beta1/test_streaming_video_intelligence_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-videointelligence-2.8.3/tests/unit/gapic/videointelligence_v1p3beta1/test_video_intelligence_service.py` & `google-cloud-videointelligence-2.9.0/tests/unit/gapic/videointelligence_v1p3beta1/test_video_intelligence_service.py`

 * *Files identical despite different names*

