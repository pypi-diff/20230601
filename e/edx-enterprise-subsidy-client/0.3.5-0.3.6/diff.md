# Comparing `tmp/edx-enterprise-subsidy-client-0.3.5.tar.gz` & `tmp/edx-enterprise-subsidy-client-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-subsidy-client-0.3.5.tar", last modified: Wed May 31 22:10:58 2023, max compression
+gzip compressed data, was "edx-enterprise-subsidy-client-0.3.6.tar", last modified: Thu Jun  1 07:21:15 2023, max compression
```

## Comparing `edx-enterprise-subsidy-client-0.3.5.tar` & `edx-enterprise-subsidy-client-0.3.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 22:10:58.041805 edx-enterprise-subsidy-client-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9096 2023-05-31 22:10:58.041805 edx-enterprise-subsidy-client-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 22:10:58.041805 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11487 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 22:10:58.041805 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9096 2023-05-31 22:10:58.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-05-31 22:10:58.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 22:10:58.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 22:10:58.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-31 22:10:58.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-31 22:10:58.000000 edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 22:10:58.041805 edx-enterprise-subsidy-client-0.3.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-31 22:10:58.041805 edx-enterprise-subsidy-client-0.3.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 22:10:58.041805 edx-enterprise-subsidy-client-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3275 2023-05-31 22:10:53.000000 edx-enterprise-subsidy-client-0.3.5/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 07:21:15.535397 edx-enterprise-subsidy-client-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     2155 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9179 2023-06-01 07:21:15.535397 edx-enterprise-subsidy-client-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 07:21:15.535397 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11665 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 07:21:15.535397 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9179 2023-06-01 07:21:15.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-06-01 07:21:15.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 07:21:15.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 07:21:15.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-01 07:21:15.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-01 07:21:15.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 07:21:15.535397 edx-enterprise-subsidy-client-0.3.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-01 07:21:15.539397 edx-enterprise-subsidy-client-0.3.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 07:21:15.535397 edx-enterprise-subsidy-client-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3275 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/tests/test_client.py
```

### Comparing `edx-enterprise-subsidy-client-0.3.5/CHANGELOG.rst` & `edx-enterprise-subsidy-client-0.3.6/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.6]
+*******
+
+* feat: pass idempotency key during transaction creation (pt. 2)
+
 [0.3.5]
 *******
 * feat: pass idempotency key during transaction creation
 
 [0.3.3]
 *******
 * allow additional query params, like ``page_size``, to be passed through to listing endpoints.
```

### Comparing `edx-enterprise-subsidy-client-0.3.5/LICENSE` & `edx-enterprise-subsidy-client-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.5/LICENSE.txt` & `edx-enterprise-subsidy-client-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.5/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.3.5
+Version: 0.3.6
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -223,14 +223,19 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.6]
+*******
+
+* feat: pass idempotency key during transaction creation (pt. 2)
+
 [0.3.5]
 *******
 * feat: pass idempotency key during transaction creation
 
 [0.3.3]
 *******
 * allow additional query params, like ``page_size``, to be passed through to listing endpoints.
```

### Comparing `edx-enterprise-subsidy-client-0.3.5/README.rst` & `edx-enterprise-subsidy-client-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client/client.py` & `edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,25 +189,35 @@
         """
         response = self.client.get(
             self.TRANSACTIONS_ENDPOINT + f'{transaction_uuid}/'
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
         TODO: add docstring.
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
             self.TRANSACTIONS_ENDPOINT,
             json=request_payload,
         )
         response.raise_for_status()
         return response.json()
```

### Comparing `edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.3.5
+Version: 0.3.6
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -223,14 +223,19 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.6]
+*******
+
+* feat: pass idempotency key during transaction creation (pt. 2)
+
 [0.3.5]
 *******
 * feat: pass idempotency key during transaction creation
 
 [0.3.3]
 *******
 * allow additional query params, like ``page_size``, to be passed through to listing endpoints.
```

### Comparing `edx-enterprise-subsidy-client-0.3.5/edx_enterprise_subsidy_client.egg-info/SOURCES.txt` & `edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.5/requirements/constraints.txt` & `edx-enterprise-subsidy-client-0.3.6/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.5/setup.py` & `edx-enterprise-subsidy-client-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.5/tests/test_client.py` & `edx-enterprise-subsidy-client-0.3.6/tests/test_client.py`

 * *Files identical despite different names*

