# Comparing `tmp/edx-enterprise-subsidy-client-0.3.4.tar.gz` & `tmp/edx-enterprise-subsidy-client-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-subsidy-client-0.3.4.tar", last modified: Tue May 30 15:52:52 2023, max compression
+gzip compressed data, was "edx-enterprise-subsidy-client-0.3.5.tar", last modified: Wed May 31 22:10:58 2023, max compression
```

## Comparing `edx-enterprise-subsidy-client-0.3.4.tar` & `edx-enterprise-subsidy-client-0.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 15:52:52.456090 edx-enterprise-subsidy-client-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1998 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9022 2023-05-30 15:52:52.456090 edx-enterprise-subsidy-client-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 15:52:52.456090 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10723 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 15:52:52.456090 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9022 2023-05-30 15:52:52.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-05-30 15:52:52.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 15:52:52.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 15:52:52.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-30 15:52:52.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-30 15:52:52.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 15:52:52.456090 edx-enterprise-subsidy-client-0.3.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-30 15:52:52.456090 edx-enterprise-subsidy-client-0.3.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 15:52:52.456090 edx-enterprise-subsidy-client-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3275 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 22:10:58.041805 edx-enterprise-subsidy-client-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9096 2023-05-31 22:10:58.041805 edx-enterprise-subsidy-client-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 22:10:58.041805 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11487 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 22:10:58.041805 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9096 2023-05-31 22:10:58.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-05-31 22:10:58.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 22:10:58.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 22:10:58.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-31 22:10:58.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-31 22:10:58.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 22:10:58.041805 edx-enterprise-subsidy-client-0.3.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-31 22:10:58.041805 edx-enterprise-subsidy-client-0.3.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 22:10:58.041805 edx-enterprise-subsidy-client-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3275 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/tests/test_client.py
```

### Comparing `edx-enterprise-subsidy-client-0.3.4/CHANGELOG.rst` & `edx-enterprise-subsidy-client-0.3.5/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.5]
+*******
+* feat: pass idempotency key during transaction creation
+
 [0.3.3]
 *******
 * allow additional query params, like ``page_size``, to be passed through to listing endpoints.
 
 [0.3.3]
 *******
 * admin-list transactions will also be filtered by ``created`` state by default.
```

### Comparing `edx-enterprise-subsidy-client-0.3.4/LICENSE` & `edx-enterprise-subsidy-client-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.4/LICENSE.txt` & `edx-enterprise-subsidy-client-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.4/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.3.4
+Version: 0.3.5
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -223,14 +223,18 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.5]
+*******
+* feat: pass idempotency key during transaction creation
+
 [0.3.3]
 *******
 * allow additional query params, like ``page_size``, to be passed through to listing endpoints.
 
 [0.3.3]
 *******
 * admin-list transactions will also be filtered by ``created`` state by default.
```

### Comparing `edx-enterprise-subsidy-client-0.3.4/README.rst` & `edx-enterprise-subsidy-client-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client/client.py` & `edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -282,24 +282,43 @@
         response = self.client.get(
             self.TRANSACTIONS_LIST_ENDPOINT.format(subsidy_uuid=subsidy_uuid),
             params=query_params,
         )
         response.raise_for_status()
         return response.json()
 
-    def create_subsidy_transaction(self, subsidy_uuid, lms_user_id, content_key, subsidy_access_policy_uuid, metadata):
+    def create_subsidy_transaction(
+        self,
+        subsidy_uuid,
+        lms_user_id,
+        content_key,
+        subsidy_access_policy_uuid,
+        metadata,
+        idempotency_key=None,
+    ):
         """
         Creates a transaction in the given subsidy, requires operator-level permissions.
+
+        Raises:
+            requests.exceptions.HTTPError:
+                - 403 Forbidden: If auth failed.
+                - 429 Too Many Requests: If the ledger was locked (resource contention, try again later).
+                - 422 Unprocessable Entity: Catchall status for anything that prevented the transaction from being
+                  created.  Reasons include, but are not limited to:
+                      * Redemption of the given content_key would have exceeded the ledger balance.
+                      * The given content_key is not in any catalog for this customer.
         """
         request_payload = {
             'subsidy_uuid': str(subsidy_uuid),
             'lms_user_id': lms_user_id,
             'content_key': content_key,
             'subsidy_access_policy_uuid': str(subsidy_access_policy_uuid),
             'metadata': metadata,
         }
+        if idempotency_key:
+            request_payload['idempotency_key'] = idempotency_key
         response = self.client.post(
             self.TRANSACTIONS_LIST_ENDPOINT.format(subsidy_uuid=subsidy_uuid),
             json=request_payload,
         )
         response.raise_for_status()
         return response.json()
```

### Comparing `edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.3.4
+Version: 0.3.5
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -223,14 +223,18 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.5]
+*******
+* feat: pass idempotency key during transaction creation
+
 [0.3.3]
 *******
 * allow additional query params, like ``page_size``, to be passed through to listing endpoints.
 
 [0.3.3]
 *******
 * admin-list transactions will also be filtered by ``created`` state by default.
```

### Comparing `edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/SOURCES.txt` & `edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.4/requirements/constraints.txt` & `edx-enterprise-subsidy-client-0.3.5/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.4/setup.py` & `edx-enterprise-subsidy-client-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.4/tests/test_client.py` & `edx-enterprise-subsidy-client-0.3.5/tests/test_client.py`

 * *Files identical despite different names*

