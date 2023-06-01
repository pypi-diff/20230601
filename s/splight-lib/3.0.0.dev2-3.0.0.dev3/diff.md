# Comparing `tmp/splight-lib-3.0.0.dev2.tar.gz` & `tmp/splight-lib-3.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-3.0.0.dev2.tar", last modified: Tue May 23 15:04:23 2023, max compression
+gzip compressed data, was "splight-lib-3.0.0.dev3.tar", last modified: Thu Jun  1 12:19:24 2023, max compression
```

## Comparing `splight-lib-3.0.0.dev2.tar` & `splight-lib-3.0.0.dev3.tar`

### file list

```diff
@@ -1,94 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.524309 splight-lib-3.0.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-23 15:04:23.524309 splight-lib-3.0.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 15:04:23.524309 splight-lib-3.0.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.520309 splight-lib-3.0.0.dev2/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.520309 splight-lib-3.0.0.dev2/splight_lib/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/abstract/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.520309 splight-lib-3.0.0.dev2/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.520309 splight-lib-3.0.0.dev2/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.520309 splight-lib-3.0.0.dev2/splight_lib/client/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/communication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/communication/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/communication/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.520309 splight-lib-3.0.0.dev2/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/database/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/database/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.520309 splight-lib-3.0.0.dev2/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/datalake/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/datalake/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.520309 splight-lib-3.0.0.dev2/splight_lib/client/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/hub/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/client/hub/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.520309 splight-lib-3.0.0.dev2/splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/communication/event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.520309 splight-lib-3.0.0.dev2/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/component/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.520309 splight-lib-3.0.0.dev2/splight_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/logging/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/logging/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.524309 splight-lib-3.0.0.dev2/splight_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/models/setpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.524309 splight-lib-3.0.0.dev2/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.524309 splight-lib-3.0.0.dev2/splight_lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/utils/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-23 15:04:21.000000 splight-lib-3.0.0.dev2/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:04:23.520309 splight-lib-3.0.0.dev2/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-23 15:04:23.000000 splight-lib-3.0.0.dev2/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-23 15:04:23.000000 splight-lib-3.0.0.dev2/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:04:23.000000 splight-lib-3.0.0.dev2/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:04:23.000000 splight-lib-3.0.0.dev2/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-23 15:04:23.000000 splight-lib-3.0.0.dev2/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 15:04:23.000000 splight-lib-3.0.0.dev2/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.795172 splight-lib-3.0.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-01 12:19:24.795172 splight-lib-3.0.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:19:24.795172 splight-lib-3.0.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.791172 splight-lib-3.0.0.dev3/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.791172 splight-lib-3.0.0.dev3/splight_lib/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/abstract/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.791172 splight-lib-3.0.0.dev3/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.791172 splight-lib-3.0.0.dev3/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.791172 splight-lib-3.0.0.dev3/splight_lib/client/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/communication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/communication/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/communication/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.791172 splight-lib-3.0.0.dev3/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/database/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/database/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.791172 splight-lib-3.0.0.dev3/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/datalake/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/datalake/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.791172 splight-lib-3.0.0.dev3/splight_lib/client/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/hub/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/client/hub/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.791172 splight-lib-3.0.0.dev3/splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/communication/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.791172 splight-lib-3.0.0.dev3/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/component/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.795172 splight-lib-3.0.0.dev3/splight_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/logging/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/logging/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.795172 splight-lib-3.0.0.dev3/splight_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/models/setpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.795172 splight-lib-3.0.0.dev3/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.795172 splight-lib-3.0.0.dev3/splight_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.795172 splight-lib-3.0.0.dev3/splight_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/utils/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-01 12:19:23.000000 splight-lib-3.0.0.dev3/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:19:24.791172 splight-lib-3.0.0.dev3/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-01 12:19:24.000000 splight-lib-3.0.0.dev3/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-01 12:19:24.000000 splight-lib-3.0.0.dev3/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:19:24.000000 splight-lib-3.0.0.dev3/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:19:24.000000 splight-lib-3.0.0.dev3/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-01 12:19:24.000000 splight-lib-3.0.0.dev3/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 12:19:24.000000 splight-lib-3.0.0.dev3/splight_lib.egg-info/top_level.txt
```

### Comparing `splight-lib-3.0.0.dev2/PKG-INFO` & `splight-lib-3.0.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.0.0.dev2
+Version: 3.0.0.dev3
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.0.0.dev2/setup.py` & `splight-lib-3.0.0.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 test_requires = [
     "pytest==7.1.2",
     "mock==4.0.3",
 ]
 
 setup(
     name="splight-lib",
-    version="3.0.0.dev2",
+    version="3.0.0.dev3",
     author="Splight",
     author_email="factory@splight-ae.com",
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-3.0.0.dev2/splight_lib/abstract/client.py` & `splight-lib-3.0.0.dev3/splight_lib/abstract/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/auth/mac_auth.py` & `splight-lib-3.0.0.dev3/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/communication/abstract.py` & `splight-lib-3.0.0.dev3/splight_lib/client/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/communication/remote_client.py` & `splight-lib-3.0.0.dev3/splight_lib/client/communication/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/database/abstract.py` & `splight-lib-3.0.0.dev3/splight_lib/client/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/database/builder.py` & `splight-lib-3.0.0.dev3/splight_lib/client/database/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/database/classmap.py` & `splight-lib-3.0.0.dev3/splight_lib/client/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/database/local_client.py` & `splight-lib-3.0.0.dev3/splight_lib/client/database/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/database/remote_client.py` & `splight-lib-3.0.0.dev3/splight_lib/client/database/remote_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         self, url: furl, **kwargs
     ) -> Generator[PaginatedResponse, None, None]:
         next_page = kwargs["page"]
         while next_page:
             response = self._list(url, **kwargs)
             yield response
             next_page = (
-                response["next"].split("page=")[1]
+                furl(response["next"]).query.params["page"]
                 if response["next"]
                 else None
             )
             kwargs["page"] = next_page
 
     def _list(self, url: furl, **kwargs) -> PaginatedResponse:
         params = self._parse_params(**kwargs)
```

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/datalake/abstract.py` & `splight-lib-3.0.0.dev3/splight_lib/client/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/datalake/builder.py` & `splight-lib-3.0.0.dev3/splight_lib/client/datalake/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/datalake/local_client.py` & `splight-lib-3.0.0.dev3/splight_lib/client/datalake/local_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,16 +46,15 @@
             file_path=file_path, total_lines=self._TOTAL_DOCS
         )
         handler.write(instances)
         return instances
 
     def _raw_get(
         self,
-        resource_name: str,
-        collection: str,
+        resource_type: DLResource,
         limit_: int = 1000,
         skip_: int = 0,
         sort: Union[List, str] = ["timestamp__desc"],
         group_id: Optional[Union[List, str]] = None,
         group_fields: Optional[Union[List, str]] = None,
         tzinfo: timezone = timezone(timedelta()),
         **filters,
@@ -69,25 +68,65 @@
 
         file_path = os.path.join(
             self._base_path, self._get_file_name(collection)
         )
         handler = FixedLineNumberFileHandler(
             file_path=file_path, total_lines=self._TOTAL_DOCS
         )
-        documents = [
-            json.loads(doc) for doc in handler.read()[skip_ : skip_ + limit_]
-        ]
+        documents = [json.loads(doc) for doc in handler.read()]
+
+        filters = kwargs
+        filters.update({"output_format": resource_type.__name__})
         documents = self._filter(documents, filters=filters)
 
         reverse = False
         if "__desc" not in sort:
             reverse = True
         documents.sort(key=lambda x: x["timestamp"], reverse=reverse)
 
-        return documents
+        # TODO: review how to apply grouping
+        return [
+            resource_type.parse_obj(doc)
+            for doc in documents[skip_ : limit_ + 1]
+        ]
+
+    def get(
+        self,
+        resource_type: Type,
+        limit_: int = 50,
+        skip_: int = 0,
+        sort: Union[List, str] = ["timestamp__desc"],
+        group_id: Union[List, str] = [],
+        group_fields: Union[List, str] = [],
+        tzinfo: timezone = timezone(timedelta()),
+        **kwargs,
+    ) -> QuerySet:
+        logger.debug(
+            "Retrieving object of type %s from datalake.",
+            resource_type,
+            tags=LogTags.DATALAKE,
+        )
+
+        new_kwargs = {
+            "get_func": "_raw_get",
+            "count_func": "None",
+            "collection": resource_type.Meta.collection_name,
+            "resource_type": resource_type,
+            "limit_": limit_,
+            "skip_": skip_,
+            "sort": sort,
+            "group_id": group_id,
+            "group_fields": group_fields,
+            "tzinfo": tzinfo,
+        }
+        kwargs.update(new_kwargs)
+        return QuerySet(self, **kwargs)
+
+    def get_output(self, query: Query) -> List[Dict]:
+        raise NotImplementedError()
 
     def get_dataframe(
         self,
         resource_name: str,
         collection: str,
         sort: Union[List, str] = ["timestamp__desc"],
         group_id: Optional[Union[List, str]] = None,
```

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/datalake/remote_client.py` & `splight-lib-3.0.0.dev3/splight_lib/client/datalake/remote_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from datetime import timedelta, timezone
 from io import StringIO
 from tempfile import NamedTemporaryFile
 from typing import Dict, List, Optional, Union
 
 import pandas as pd
 from furl import furl
+from pydantic import BaseModel
 from retry import retry
-from splight_lib.abstract.client import AbstractRemoteClient
+from splight_abstract import AbstractRemoteClient
+from splight_abstract.datalake import (
+    AbstractDatalakeClient,
+)
 from splight_lib.auth import SplightAuthToken
-from splight_lib.client.datalake.abstract import AbstractDatalakeClient
 from splight_lib.client.exceptions import SPLIGHT_REQUEST_EXCEPTIONS
 from splight_lib.logging._internal import LogTags, get_splight_logger
 from splight_lib.restclient import SplightRestClient
 
 logger = get_splight_logger()
```

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/exceptions.py` & `splight-lib-3.0.0.dev3/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/file_handler.py` & `splight-lib-3.0.0.dev3/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/filter.py` & `splight-lib-3.0.0.dev3/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/client/hub/client.py` & `splight-lib-3.0.0.dev3/splight_lib/client/hub/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,37 @@
-from typing import Dict, List, Optional, Tuple, Type
+from typing import Dict, List, Optional, Tuple
 
 import requests
 from furl import furl
 from pydantic import BaseModel
 from splight_lib.auth import SplightAuthToken
 from splight_lib.client.hub.abstract import (
     AbstractHubClient,
     AbstractHubSubClient,
-    validate_client_resource_type,
 )
-from splight_lib.models.hub import HubComponent, HubComponentVersion
-from splight_lib.settings import settings
 
 
 class _SplightHubGenericClient(AbstractHubSubClient):
     _PREFIX: str = "v2/hub"
-    valid_classes = [
-        HubComponent,
-        HubComponentVersion,
-    ]
     _CLASS_MAP = {
-        HubComponent: "components",
-        HubComponentVersion: "component-versions",
+        'HubComponent': "components",
+        'HubComponentVersion': "component-versions",
     }
 
     def __init__(
         self,
         base_path: str,
+        api_host: str,
         headers: Optional[Dict[str, str]] = {},
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self._base_url = furl(
-            settings.SPLIGHT_PLATFORM_API_HOST,
+            api_host,
             path=f"{self._PREFIX}/{base_path}/",
         )
         self._session = requests.Session()
         self._session.headers.update(headers)
 
     def _get_url(self, resource_type: str, id: Optional[str] = None) -> furl:
         resource_type_prefix = self._CLASS_MAP.get(resource_type)
@@ -52,127 +46,129 @@
             if skip_ > 0:
                 kwargs["page"] = skip_ // limit_ + 1
         return kwargs
 
     def save(self, instance: BaseModel) -> BaseModel:
         raise NotImplementedError
 
-    @validate_client_resource_type
     def _get(
         self,
-        resource_type: Type,
+        resource_type: str,
         first: bool = False,
         limit_: int = -1,
         skip_: int = 0,
         **kwargs,
     ) -> List[BaseModel]:
         url = self._get_url(resource_type)
         params = self._get_params(limit_, skip_, **kwargs)
         response = self._session.get(url, params=params)
         assert (
             response.status_code == 200
         ), f"Failed to get components {response.content}"
-        queryset = [resource_type(**v) for v in response.json()["results"]]
+        queryset = response.json()["results"]
         if first:
             return queryset[0] if queryset else None
         return queryset
 
     def count(
         self,
-        resource_type: Type,
+        resource_type: str,
         first=False,
         limit_: int = -1,
         skip_: int = 0,
         **kwargs,
     ):
         url = self._get_url(resource_type)
         params = self._get_params(limit_=-1, skip_=-1, kwargs=kwargs)
         response = self._session.get(url, params=params)
         assert (
             response.status_code == 200
         ), f"Failed to get components {response.content}"
         return response.json()["count"]
 
-    def delete(self, resource_type: Type, id: str) -> None:
+    def delete(self, resource_type: str, id: str) -> None:
         url = self._get_url(resource_type, id)
         response = self._session.delete(url)
         assert (
             response.status_code == 204
         ), f"Failed to delete component {response.content}"
 
-    @validate_client_resource_type
-    def update(self, resource_type: Type, id: str, data: Dict) -> BaseModel:
+    def update(self, resource_type: str, id: str, data: Dict) -> BaseModel:
         url = self._get_url(resource_type, id)
         response = self._session.put(url, json=data)
         assert (
             response.status_code == 200
         ), f"Failed to update component. {response.content}"
         return resource_type(**response.json())
 
-    @validate_client_resource_type
     def partial_update(
-        self, resource_type: Type, id: str, data: Dict
+        self, resource_type: str, id: str, data: Dict
     ) -> BaseModel:
         url = self._get_url(resource_type, id)
         response = self._session.patch(url, json=data)
         assert (
             response.status_code == 200
         ), f"Failed to update component. {response.content}"
         return resource_type.parse_obj(response.json())
 
-    @validate_client_resource_type
-    def rebuild(self, resource_type: Type, id: str) -> None:
+    def rebuild(self, resource_type: str, id: str) -> None:
         url = self._get_url(resource_type, id)
         url = url / "rebuild/"
         response = self._session.post(url, headers=self.headers)
         assert (
             response.status_code == 204
         ), f"Failed to rebuild component. {response.content}"
 
 
 class SplightHubClient(AbstractHubClient):
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(
+        self,
+        access_key: str,
+        secret_key: str,
+        api_host: str,
+        *args, **kwargs
+    ) -> None:
         super().__init__()
         token = SplightAuthToken(
-            access_key=settings.SPLIGHT_ACCESS_ID,
-            secret_key=settings.SPLIGHT_SECRET_KEY,
+            access_key=access_key,
+            secret_key=secret_key,
         )
         self._all = _SplightHubGenericClient(
-            base_path="all", headers=token.header
+            base_path="all", headers=token.header, api_host=api_host
         )
         self._mine = _SplightHubGenericClient(
-            base_path="mine", headers=token.header
+            base_path="mine", headers=token.header, api_host=api_host
         )
         self._public = _SplightHubGenericClient(
-            base_path="public", headers=token.header
+            base_path="public", headers=token.header, api_host=api_host
         )
         self._private = _SplightHubGenericClient(
-            base_path="private", headers=token.header
+            base_path="private", headers=token.header, api_host=api_host
         )
         self._setup = _SplightHubGenericClient(
-            base_path="setup", headers=token.header
+            base_path="setup", headers=token.header, api_host=api_host
         )
-        self._host = furl(settings.SPLIGHT_PLATFORM_API_HOST)
+        self._host = furl(api_host)
         self._headers = token.header
 
     def upload(self, data: Dict, files: Dict) -> Tuple:
         url = self._host / "v2/hub/upload/"
         response = requests.post(
             url, files=files, data=data, headers=self._headers
         )
         status_code = response.status_code
         assert status_code == 201, "Unable to upload component to HUB"
-        return response.json(), status_code
+        return response.json()
 
     def download(self, data: Dict) -> Tuple:
         url = self._host / "v2/hub/download/"
         response = requests.post(url, data=data, headers=self._headers)
         status_code = response.status_code
         assert status_code == 200, "Unable to download component"
-        return response.content, status_code
+        return response.content
 
     @property
     def all(self) -> AbstractHubSubClient:
         return self._all
 
     @property
     def mine(self) -> AbstractHubSubClient:
```

### Comparing `splight-lib-3.0.0.dev2/splight_lib/communication/event_handler.py` & `splight-lib-3.0.0.dev3/splight_lib/communication/event_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/component/abstract.py` & `splight-lib-3.0.0.dev3/splight_lib/component/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/component/exceptions.py` & `splight-lib-3.0.0.dev3/splight_lib/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/component/spec.py` & `splight-lib-3.0.0.dev3/splight_lib/component/spec.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/encryption.py` & `splight-lib-3.0.0.dev3/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/execution.py` & `splight-lib-3.0.0.dev3/splight_lib/execution.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/logging/_internal.py` & `splight-lib-3.0.0.dev3/splight_lib/logging/_internal.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/logging/component.py` & `splight-lib-3.0.0.dev3/splight_lib/logging/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/logging/logging.py` & `splight-lib-3.0.0.dev3/splight_lib/logging/logging.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/models/__init__.py` & `splight-lib-3.0.0.dev3/splight_lib/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,29 +3,25 @@
 from splight_lib.models.attribute import Attribute
 from splight_lib.models.component import (
     Component,
     ComponentObject,
     ComponentObjectInstance,
 )
 from splight_lib.models.file import File
-from splight_lib.models.hub import HubComponent, HubComponentVersion
-from splight_lib.models.native import Boolean, Number, String
 from splight_lib.models.query import Query
+from splight_lib.models.native import Number, String, Boolean
 from splight_lib.models.secret import Secret
 from splight_lib.models.setpoint import SetPoint
 
 __all__ = [
     Alert,
     AlertCondition,
     Asset,
     Attribute,
     Boolean,
-    Component,
-    ComponentObject,
-    ComponentObjectInstance,
     File,
     HubComponent,
     HubComponentVersion,
     Number,
     Query,
     String,
     Secret,
```

### Comparing `splight-lib-3.0.0.dev2/splight_lib/models/alert.py` & `splight-lib-3.0.0.dev3/splight_lib/models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/models/asset.py` & `splight-lib-3.0.0.dev3/splight_lib/models/asset.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/models/base.py` & `splight-lib-3.0.0.dev3/splight_lib/models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import json
-from datetime import datetime, timezone
-from typing import ClassVar, Dict, List, Optional, Set, Tuple
-
-import pandas as pd
-from pydantic import BaseModel, Field, PrivateAttr
+from typing import Dict, List, Optional
+from pydantic import BaseModel, PrivateAttr, Field
+from splight_abstract.database import AbstractDatabaseClient
+from splight_abstract.datalake import AbstractDatalakeClient
 from splight_lib.client.database import DatabaseClientBuilder
 from splight_lib.client.database.abstract import AbstractDatabaseClient
 from splight_lib.client.datalake import DatalakeClientBuilder
 from splight_lib.client.datalake.abstract import AbstractDatalakeClient
 from splight_lib.settings import settings
```

### Comparing `splight-lib-3.0.0.dev2/splight_lib/models/communication.py` & `splight-lib-3.0.0.dev3/splight_lib/models/communication.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/models/component.py` & `splight-lib-3.0.0.dev3/splight_lib/models/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 
 
 class PrivacyPolicy(LowercaseStrEnum):
     PUBLIC = auto()
     PRIVATE = auto()
 
+warnings.filterwarnings("ignore", category=RuntimeWarning)
+
+
+class PrivacyPolicy(LowercaseStrEnum):
+    PUBLIC = auto()
+    PRIVATE = auto()
+
 
 class ComponentType(LowercaseStrEnum):
     ALGORITHM = auto()
     NETWORK = auto()
     CONNECTOR = auto()
     SIMULATOR = auto()
     OTHER = auto()
```

### Comparing `splight-lib-3.0.0.dev2/splight_lib/models/event.py` & `splight-lib-3.0.0.dev3/splight_lib/models/event.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/models/file.py` & `splight-lib-3.0.0.dev3/splight_lib/models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/models/native.py` & `splight-lib-3.0.0.dev3/splight_lib/models/native.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/models/query.py` & `splight-lib-3.0.0.dev3/splight_lib/models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/models/setpoint.py` & `splight-lib-3.0.0.dev3/splight_lib/models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/restclient/client.py` & `splight-lib-3.0.0.dev3/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/restclient/exceptions.py` & `splight-lib-3.0.0.dev3/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/restclient/types.py` & `splight-lib-3.0.0.dev3/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/settings.py` & `splight-lib-3.0.0.dev3/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/utils/custom_model.py` & `splight-lib-3.0.0.dev3/splight_lib/utils/custom_model.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib/webhook.py` & `splight-lib-3.0.0.dev3/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev2/splight_lib.egg-info/PKG-INFO` & `splight-lib-3.0.0.dev3/splight_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.0.0.dev2
+Version: 3.0.0.dev3
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.0.0.dev2/splight_lib.egg-info/SOURCES.txt` & `splight-lib-3.0.0.dev3/splight_lib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -68,9 +68,11 @@
 splight_lib/models/query.py
 splight_lib/models/secret.py
 splight_lib/models/setpoint.py
 splight_lib/restclient/__init__.py
 splight_lib/restclient/client.py
 splight_lib/restclient/exceptions.py
 splight_lib/restclient/types.py
+splight_lib/testing/__init__.py
 splight_lib/utils/__init__.py
-splight_lib/utils/custom_model.py
+splight_lib/utils/custom_model.py
+splight_lib/utils/hub.py
```

