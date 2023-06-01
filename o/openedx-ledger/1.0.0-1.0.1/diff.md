# Comparing `tmp/openedx-ledger-1.0.0.tar.gz` & `tmp/openedx-ledger-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-ledger-1.0.0.tar", last modified: Tue May 30 20:48:33 2023, max compression
+gzip compressed data, was "openedx-ledger-1.0.1.tar", last modified: Thu Jun  1 18:08:10 2023, max compression
```

## Comparing `openedx-ledger-1.0.0.tar` & `openedx-ledger-1.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8698 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/openedx_ledger/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3884 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5394 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/openedx_ledger/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
--rw-r--r--   0 runner    (1001) docker     (122)    12708 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/0005_help_text_and_more_indices.py
--rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/0006_auto_20230404_1744.py
--rw-r--r--   0 runner    (1001) docker     (122)      468 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/0007_alter_externalfulfillmentprovider_name.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15825 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/openedx_ledger/signals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.502779 openedx-ledger-1.0.0/openedx_ledger/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/openedx_ledger/templates/edx_ledger/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/openedx_ledger/templates/edx_ledger/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/templates/edx_ledger/base.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/openedx_ledger/test_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/test_utils/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/openedx_ledger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8698 2023-05-30 20:48:33.000000 openedx-ledger-1.0.0/openedx_ledger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-05-30 20:48:33.000000 openedx-ledger-1.0.0/openedx_ledger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 20:48:33.000000 openedx-ledger-1.0.0/openedx_ledger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 20:48:33.000000 openedx-ledger-1.0.0/openedx_ledger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-30 20:48:33.000000 openedx-ledger-1.0.0/openedx_ledger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-30 20:48:33.000000 openedx-ledger-1.0.0/openedx_ledger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-30 20:48:33.510779 openedx-ledger-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5100 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7504 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8783 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.739527 openedx-ledger-1.0.1/openedx_ledger/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4859 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5394 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/openedx_ledger/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12708 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/0005_help_text_and_more_indices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/0006_auto_20230404_1744.py
+-rw-r--r--   0 runner    (1001) docker     (122)      468 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/0007_alter_externalfulfillmentprovider_name.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16107 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/openedx_ledger/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.735527 openedx-ledger-1.0.1/openedx_ledger/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/openedx_ledger/templates/edx_ledger/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/openedx_ledger/templates/edx_ledger/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/templates/edx_ledger/base.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/openedx_ledger/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/test_utils/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.739527 openedx-ledger-1.0.1/openedx_ledger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8783 2023-06-01 18:08:10.000000 openedx-ledger-1.0.1/openedx_ledger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-06-01 18:08:10.000000 openedx-ledger-1.0.1/openedx_ledger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 18:08:10.000000 openedx-ledger-1.0.1/openedx_ledger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 18:08:10.000000 openedx-ledger-1.0.1/openedx_ledger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-06-01 18:08:10.000000 openedx-ledger-1.0.1/openedx_ledger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-01 18:08:10.000000 openedx-ledger-1.0.1/openedx_ledger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5100 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7504 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/tests/test_utils.py
```

### Comparing `openedx-ledger-1.0.0/CHANGELOG.rst` & `openedx-ledger-1.0.1/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
+* Nothing unreleased
 
+[1.0.1]
+*******
+* make transaction and ledger admins friendlier
 
 [1.0.0]
 *******
 * Look for an ``lms_user_id`` key when generating transaction idempotency keys, not ``learner_id``.
 
 [0.4.0]
 *******
```

### Comparing `openedx-ledger-1.0.0/LICENSE.txt` & `openedx-ledger-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/PKG-INFO` & `openedx-ledger-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 1.0.0
+Version: 1.0.1
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -204,15 +204,19 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
+* Nothing unreleased
 
+[1.0.1]
+*******
+* make transaction and ledger admins friendlier
 
 [1.0.0]
 *******
 * Look for an ``lms_user_id`` key when generating transaction idempotency keys, not ``learner_id``.
 
 [0.4.0]
 *******
```

### Comparing `openedx-ledger-1.0.0/README.rst` & `openedx-ledger-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/openedx_ledger/admin.py` & `openedx-ledger-1.0.1/openedx_ledger/admin.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,47 +4,55 @@
 from django.conf import settings
 from django.contrib import admin
 from django.http import HttpResponseRedirect
 from django.urls import re_path, reverse
 from django_object_actions import DjangoObjectActions
 from simple_history.admin import SimpleHistoryAdmin
 
-from openedx_ledger import models, views
+from openedx_ledger import constants, models, views
 
 
 def can_modify():
-    getattr(settings, 'ALLOW_LEDGER_MODIFICATION', False)
+    return getattr(settings, 'ALLOW_LEDGER_MODIFICATION', False)
+
+
+def cents_to_usd_string(balance_in_cents):
+    """
+    Helper to convert cents as in int to dollars as a
+    nicely formatted string.
+    """
+    return "${:,.2f}".format(float(balance_in_cents) / constants.CENTS_PER_US_DOLLAR)
 
 
 @admin.register(models.Ledger)
 class LedgerAdmin(SimpleHistoryAdmin):
     """
     Admin configuration for the Ledger model.
     """
 
     class Meta:
         """
         Metaclass for LedgerAdmin.
         """
         model = models.Ledger
 
-    fields = ('uuid', 'idempotency_key', 'unit', 'balance', 'metadata')
+    fields = ('uuid', 'idempotency_key', 'unit', 'balance_usd', 'metadata')
     if can_modify():
-        readonly_fields = ('uuid', 'balance')
+        readonly_fields = ('uuid', 'balance_usd')
     else:
         readonly_fields = fields
 
     # Do not add balance here, it's a computed value.
     list_display = ('uuid', 'unit', 'idempotency_key')
 
-    def balance(self, obj):
+    def balance_usd(self, obj):
         """
         Passthrough function to calculate the ledger balance.
         """
-        return obj.balance()
+        return cents_to_usd_string(obj.balance())
 
 
 @admin.register(models.ExternalFulfillmentProvider)
 class ExternalFulfillmentProviderAdmin(SimpleHistoryAdmin):
     """
     Admin configuration for the ExternalFulfillmentProvider model.
     """
@@ -77,28 +85,61 @@
         """
         Metaclass for TransactionAdmin.
         """
 
         model = models.Transaction
         fields = '__all__'
 
-    search_fields = ('content_key', 'lms_user_id', 'uuid', 'external_reference__external_reference_id',)
-    _all_fields = [field.name for field in models.Transaction._meta.get_fields() if field.name != 'external_reference']
-    list_display = ('uuid', 'idempotency_key', 'quantity', 'state',)
+    search_fields = (
+        'content_key',
+        'lms_user_id',
+        'uuid',
+        'external_reference__external_reference_id',
+        'subsidy_access_policy_uuid',
+    )
+    _all_fields = [
+        field.name for field in models.Transaction._meta.get_fields()
+        if field.name != 'external_reference'
+    ]
+    _writable_fields = [
+        'fulfillment_identifier',
+    ]
+    list_display = (
+        'uuid',
+        'lms_user_id',
+        'content_key',
+        'subsidy_access_policy_uuid',
+        'quantity',
+        'state',
+        'modified',
+        'has_reversal',
+    )
+    list_filter = (
+        'state',
+    )
+
     if can_modify():
-        readonly_fields = (
-            'created',
-            'modified',
-        )
+        readonly_fields = [
+            field_name for field_name in _all_fields
+            if field_name not in ['fulfillment_identifier']
+        ]
     else:
         readonly_fields = _all_fields
     inlines = [ExternalTransactionReferenceInlineAdmin]
 
+    @admin.display(ordering='reversal', description='Has a reversal')
+    def has_reversal(self, obj):
+        return bool(obj.get_reversal())
+
     change_actions = ('reverse_transaction',)
 
+    def get_queryset(self, request):
+        queryset = super().get_queryset(request)
+        return queryset.select_related('reversal')
+
     def reverse_transaction(self, request, obj):
         """
         Redirect to the reverse transaction view.
         """
         # url names coming from get_urls are prefixed with 'admin' namespace
         reverse_transaction_url = reverse("admin:reverse_transaction", args=(obj.uuid,))
         return HttpResponseRedirect(reverse_transaction_url)
```

### Comparing `openedx-ledger-1.0.0/openedx_ledger/api.py` & `openedx-ledger-1.0.1/openedx_ledger/api.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/openedx_ledger/migrations/0001_initial.py` & `openedx-ledger-1.0.1/openedx_ledger/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py` & `openedx-ledger-1.0.1/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/openedx_ledger/migrations/0003_field_updates_20230216_1605.py` & `openedx-ledger-1.0.1/openedx_ledger/migrations/0003_field_updates_20230216_1605.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py` & `openedx-ledger-1.0.1/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/openedx_ledger/migrations/0005_help_text_and_more_indices.py` & `openedx-ledger-1.0.1/openedx_ledger/migrations/0005_help_text_and_more_indices.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/openedx_ledger/migrations/0006_auto_20230404_1744.py` & `openedx-ledger-1.0.1/openedx_ledger/migrations/0006_auto_20230404_1744.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/openedx_ledger/models.py` & `openedx-ledger-1.0.1/openedx_ledger/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,14 +348,24 @@
     subsidy_access_policy_uuid = models.UUIDField(
         blank=True,
         null=True,
         help_text="A reference to the subsidy access policy which was used to create a transaction for the content."
     )
     history = HistoricalRecords()
 
+    def get_reversal(self):
+        """
+        Convenience method for fetching this transaction's related
+        reversal, or None if no such reversal exists.
+        """
+        try:
+            return self.reversal
+        except Reversal.DoesNotExist:
+            return None
+
 
 class ExternalFulfillmentProvider(TimeStampedModel):
     """
     Model of external fulfillment providers. This is used to track the external systems that are used to fulfill
     transactions.
 
     .. no_pii:
```

### Comparing `openedx-ledger-1.0.0/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html` & `openedx-ledger-1.0.1/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/openedx_ledger/templates/edx_ledger/base.html` & `openedx-ledger-1.0.1/openedx_ledger/templates/edx_ledger/base.html`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/openedx_ledger/test_utils/factories.py` & `openedx-ledger-1.0.1/openedx_ledger/test_utils/factories.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/openedx_ledger/utils.py` & `openedx-ledger-1.0.1/openedx_ledger/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/openedx_ledger/views.py` & `openedx-ledger-1.0.1/openedx_ledger/views.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/openedx_ledger.egg-info/PKG-INFO` & `openedx-ledger-1.0.1/openedx_ledger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 1.0.0
+Version: 1.0.1
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -204,15 +204,19 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
+* Nothing unreleased
 
+[1.0.1]
+*******
+* make transaction and ledger admins friendlier
 
 [1.0.0]
 *******
 * Look for an ``lms_user_id`` key when generating transaction idempotency keys, not ``learner_id``.
 
 [0.4.0]
 *******
```

### Comparing `openedx-ledger-1.0.0/openedx_ledger.egg-info/SOURCES.txt` & `openedx-ledger-1.0.1/openedx_ledger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/requirements/constraints.txt` & `openedx-ledger-1.0.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/setup.py` & `openedx-ledger-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/tests/test_api.py` & `openedx-ledger-1.0.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/tests/test_models.py` & `openedx-ledger-1.0.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.0/tests/test_utils.py` & `openedx-ledger-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

