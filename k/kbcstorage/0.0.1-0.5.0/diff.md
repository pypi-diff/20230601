# Comparing `tmp/kbcstorage-0.0.1.tar.gz` & `tmp/kbcstorage-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbcstorage-0.0.1.tar", max compression
+gzip compressed data, was "kbcstorage-0.5.0.tar", last modified: Thu Mar  9 13:36:21 2023, max compression
```

## Comparing `kbcstorage-0.0.1.tar` & `kbcstorage-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,53 @@
--rw-r--r--   0        0        0     1078 2023-02-13 08:25:03.605916 kbcstorage-0.0.1/LICENSE
--rw-r--r--   0        0        0     3623 2023-02-13 08:25:03.606124 kbcstorage-0.0.1/README.md
--rw-r--r--   0        0        0      366 2023-02-13 08:38:46.100229 kbcstorage-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      243 2023-02-13 08:25:03.606477 kbcstorage-0.0.1/src/kbcstorage/__init__.py
--rw-r--r--   0        0        0     4701 2023-02-13 08:25:03.606627 kbcstorage-0.0.1/src/kbcstorage/base.py
--rw-r--r--   0        0        0     4835 2023-02-13 08:25:03.606754 kbcstorage-0.0.1/src/kbcstorage/buckets.py
--rw-r--r--   0        0        0      980 2023-02-13 08:25:03.606877 kbcstorage-0.0.1/src/kbcstorage/client.py
--rw-r--r--   0        0        0    11850 2023-02-13 08:25:03.607088 kbcstorage-0.0.1/src/kbcstorage/files.py
--rw-r--r--   0        0        0     3480 2023-02-13 08:25:03.607228 kbcstorage-0.0.1/src/kbcstorage/jobs.py
--rw-r--r--   0        0        0    23904 2023-02-13 08:25:03.607483 kbcstorage-0.0.1/src/kbcstorage/tables.py
--rw-r--r--   0        0        0        0 2023-02-13 08:25:03.607831 kbcstorage-0.0.1/src/kbcstorage/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-13 08:25:03.607945 kbcstorage-0.0.1/src/kbcstorage/tests/functional/__init__.py
--rw-r--r--   0        0        0     4065 2023-02-13 08:25:03.608085 kbcstorage-0.0.1/src/kbcstorage/tests/functional/test_base.py
--rw-r--r--   0        0        0     3394 2023-02-13 08:25:03.608213 kbcstorage-0.0.1/src/kbcstorage/tests/functional/test_buckets.py
--rw-r--r--   0        0        0     2240 2023-02-13 08:25:03.608343 kbcstorage-0.0.1/src/kbcstorage/tests/functional/test_client.py
--rw-r--r--   0        0        0     7448 2023-02-13 08:25:03.608472 kbcstorage-0.0.1/src/kbcstorage/tests/functional/test_files.py
--rw-r--r--   0        0        0    15742 2023-02-13 08:25:03.608646 kbcstorage-0.0.1/src/kbcstorage/tests/functional/test_tables.py
--rw-r--r--   0        0        0     7351 2023-02-13 08:25:03.608823 kbcstorage-0.0.1/src/kbcstorage/tests/functional/test_workspaces.py
--rw-r--r--   0        0        0        0 2023-02-13 08:25:03.608923 kbcstorage-0.0.1/src/kbcstorage/tests/mocks/__init__.py
--rw-r--r--   0        0        0     1936 2023-02-13 08:25:03.609037 kbcstorage-0.0.1/src/kbcstorage/tests/mocks/bucket_responses.py
--rw-r--r--   0        0        0     1775 2023-02-13 08:25:03.609161 kbcstorage-0.0.1/src/kbcstorage/tests/mocks/job_responses.py
--rw-r--r--   0        0        0     2074 2023-02-13 08:25:03.609270 kbcstorage-0.0.1/src/kbcstorage/tests/mocks/table_responses.py
--rw-r--r--   0        0        0     2428 2023-02-13 08:25:03.609413 kbcstorage-0.0.1/src/kbcstorage/tests/mocks/test_buckets.py
--rw-r--r--   0        0        0      334 2023-02-13 08:25:03.609518 kbcstorage-0.0.1/src/kbcstorage/tests/mocks/test_client.py
--rw-r--r--   0        0        0     4674 2023-02-13 08:25:03.609655 kbcstorage-0.0.1/src/kbcstorage/tests/mocks/test_jobs.py
--rw-r--r--   0        0        0      882 2023-02-13 08:25:03.609779 kbcstorage-0.0.1/src/kbcstorage/tests/mocks/test_tables.py
--rw-r--r--   0        0        0     8047 2023-02-13 08:25:03.609892 kbcstorage-0.0.1/src/kbcstorage/tests/mocks/test_workspaces.py
--rw-r--r--   0        0        0     2853 2023-02-13 08:25:03.609999 kbcstorage-0.0.1/src/kbcstorage/tests/mocks/workspace_responses.py
--rw-r--r--   0        0        0     6368 2023-02-13 08:25:03.607641 kbcstorage-0.0.1/src/kbcstorage/workspaces.py
--rw-r--r--   0        0        0     4560 1970-01-01 00:00:00.000000 kbcstorage-0.0.1/setup.py
--rw-r--r--   0        0        0     4288 1970-01-01 00:00:00.000000 kbcstorage-0.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.898647 kbcstorage-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.894647 kbcstorage-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.894647 kbcstorage-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-03-09 13:36:21.898647 kbcstorage-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      347 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.894647 kbcstorage-0.5.0/kbcstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23904 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/kbcstorage/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.894647 kbcstorage-0.5.0/kbcstorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-03-09 13:36:21.000000 kbcstorage-0.5.0/kbcstorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-09 13:36:21.000000 kbcstorage-0.5.0/kbcstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 13:36:21.000000 kbcstorage-0.5.0/kbcstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-09 13:36:21.000000 kbcstorage-0.5.0/kbcstorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-09 13:36:21.000000 kbcstorage-0.5.0/kbcstorage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 13:36:21.898647 kbcstorage-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.894647 kbcstorage-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.898647 kbcstorage-0.5.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/functional/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/functional/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/functional/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/functional/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/functional/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/functional/test_workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:21.898647 kbcstorage-0.5.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/bucket_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/job_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/table_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/test_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-09 13:36:09.000000 kbcstorage-0.5.0/tests/mocks/workspace_responses.py
```

### Comparing `kbcstorage-0.0.1/LICENSE` & `kbcstorage-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/README.md` & `kbcstorage-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/base.py` & `kbcstorage-0.5.0/kbcstorage/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -141,8 +141,10 @@
         headers.update(self._auth_header)
         r = requests.delete(headers=headers, *args, **kwargs)
         try:
             r.raise_for_status()
         except requests.HTTPError:
             # Handle different error codes
             raise
-        # Should delete return something on success?
+
+        if 'application/json' in r.headers.get('Content-Type', ''):
+            return r.json()
```

### Comparing `kbcstorage-0.0.1/src/kbcstorage/buckets.py` & `kbcstorage-0.5.0/kbcstorage/buckets.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Full documentation `here`.
 
 .. _here:
     http://docs.keboola.apiary.io/#reference/buckets/
 """
 from kbcstorage.base import Endpoint
+from kbcstorage.jobs import Jobs
 
 
 class Buckets(Endpoint):
     """
     Buckets Endpoint
     """
     def __init__(self, root_url, token):
@@ -96,32 +97,40 @@
             'stage': stage,
             'description': description,
             'backend': backend
         }
 
         return self._post(self.base_url, data=body)
 
-    def delete(self, bucket_id, force=False):
+    def delete(self, bucket_id, force=False, asynchronous=True):
         """
         Delete a bucket referenced by ``bucket_id``.
 
         By default, only empty buckets without dependencies (aliases etc) can
         be deleted. The optional ``force`` parameter allows for the deletion
         of non-empty buckets.
 
         Args:
             bucket_id (str): The id of the bucket to be deleted.
             force (bool): If ``True``, deletes the bucket even if it is not
                 empty. Default ``False``.
+            asynchronous (bool): if asynchronous then the
         """
         # How does the API handle it when force == False and the bucket is non-
         # empty?
         url = '{}/{}'.format(self.base_url, bucket_id)
-        params = {'force': force}
-        self._delete(url, params=params)
+        params = {'force': force, 'async': asynchronous}
+        if (asynchronous):
+            job = self._delete(url, params=params)
+            jobs = Jobs(self.root_url, self.token)
+            job = jobs.block_until_completed(job['id'])
+            if job['status'] == 'error':
+                raise RuntimeError(job['error']['message'])
+        else:
+            self._delete(url, params=params)
 
     def link(self, *args, **kwargs):
         """
         **Not implemented**
 
         Link an existing bucket from another project.
```

### Comparing `kbcstorage-0.0.1/src/kbcstorage/client.py` & `kbcstorage-0.5.0/kbcstorage/client.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/files.py` & `kbcstorage-0.5.0/kbcstorage/files.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/jobs.py` & `kbcstorage-0.5.0/kbcstorage/jobs.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tables.py` & `kbcstorage-0.5.0/kbcstorage/tables.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tests/functional/test_base.py` & `kbcstorage-0.5.0/tests/functional/test_base.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tests/functional/test_buckets.py` & `kbcstorage-0.5.0/tests/functional/test_buckets.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         self.buckets = Buckets(os.getenv('KBC_TEST_API_URL'),
                                os.getenv('KBC_TEST_TOKEN'))
         try:
             self.buckets.delete('in.c-py-test-buckets', force=True)
         except exceptions.HTTPError as e:
             if e.response.status_code != 404:
                 raise
+
         # https://github.com/boto/boto3/issues/454
         warnings.simplefilter("ignore", ResourceWarning)
 
     def tearDown(self):
         try:
             self.buckets.delete('in.c-py-test-buckets', force=True)
         except exceptions.HTTPError as e:
```

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tests/functional/test_client.py` & `kbcstorage-0.5.0/tests/functional/test_client.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tests/functional/test_files.py` & `kbcstorage-0.5.0/tests/functional/test_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from kbcstorage.buckets import Buckets
 from kbcstorage.files import Files
 from kbcstorage.tables import Tables
 
 
 class TestFiles(unittest.TestCase):
     def setUp(self):
-
         # timeout for files from previous tests to appear
         time.sleep(1)
         self.files = Files(os.getenv('KBC_TEST_API_URL'),
                            os.getenv('KBC_TEST_TOKEN'))
         files = self.files.list(tags=['py-test'])
         for file in files:
             self.files.delete(file['id'])
```

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tests/functional/test_tables.py` & `kbcstorage-0.5.0/tests/functional/test_tables.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tests/functional/test_workspaces.py` & `kbcstorage-0.5.0/tests/functional/test_workspaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
             if e.response.status_code != 404:
                 raise
         try:
             self.buckets.delete('in.c-py-test-buckets', force=True)
         except exceptions.HTTPError as e:
             if e.response.status_code != 404:
                 raise
+
         # https://github.com/boto/boto3/issues/454
         warnings.simplefilter("ignore", ResourceWarning)
 
     def tearDown(self):
         try:
             if hasattr(self, 'workspace_id'):
                 self.workspaces.delete(self.workspace_id)
```

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tests/mocks/bucket_responses.py` & `kbcstorage-0.5.0/tests/mocks/bucket_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tests/mocks/job_responses.py` & `kbcstorage-0.5.0/tests/mocks/job_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tests/mocks/table_responses.py` & `kbcstorage-0.5.0/tests/mocks/table_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tests/mocks/test_buckets.py` & `kbcstorage-0.5.0/tests/mocks/test_buckets.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,20 +46,20 @@
     def test_delete(self):
         """
         Buckets mock deletes bucket by id.
         """
         responses.add(
             responses.Response(
                 method='DELETE',
-                url='https://connection.keboola.com/v2/storage/buckets/1',
+                url='https://connection.keboola.com/v2/storage/buckets/1?force=False&async=False',
                 json={}
             )
         )
         bucket_id = '1'
-        deleted_detail = self.buckets.delete(bucket_id)
+        deleted_detail = self.buckets.delete(bucket_id, asynchronous=False)
         assert deleted_detail is None
 
     @responses.activate
     def test_create(self):
         """
         Buckets mock creates new bucket.
         """
```

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tests/mocks/test_jobs.py` & `kbcstorage-0.5.0/tests/mocks/test_jobs.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tests/mocks/test_tables.py` & `kbcstorage-0.5.0/tests/mocks/test_tables.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tests/mocks/test_workspaces.py` & `kbcstorage-0.5.0/tests/mocks/test_workspaces.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/tests/mocks/workspace_responses.py` & `kbcstorage-0.5.0/tests/mocks/workspace_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/src/kbcstorage/workspaces.py` & `kbcstorage-0.5.0/kbcstorage/workspaces.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.0.1/setup.py` & `kbcstorage-0.5.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,118 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: kbcstorage
+Version: 0.5.0
+Home-page: https://github.com/keboola/sapi-python-client
+Download-URL: https://github.com/keboola/sapi-python-client
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE.txt
 
-package_dir = \
-{'': 'src'}
+[![Build Status](https://travis-ci.org/keboola/sapi-python-client.svg?branch=master)](https://travis-ci.org/keboola/sapi-python-client)
 
-packages = \
-['kbcstorage',
- 'kbcstorage.tests',
- 'kbcstorage.tests.functional',
- 'kbcstorage.tests.mocks']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['azure-storage-blob>=12.14.1,<13.0.0',
- 'boto3>=1.26.69,<2.0.0',
- 'requests>=2.28.2,<3.0.0']
-
-setup_kwargs = {
-    'name': 'kbcstorage',
-    'version': '0.0.1',
-    'description': 'Keboola Storage API',
-    'long_description': "[![Build Status](https://travis-ci.org/keboola/sapi-python-client.svg?branch=master)](https://travis-ci.org/keboola/sapi-python-client)\n\n# Python client for the Keboola Storage API\nClient for using [Keboola Connection Storage API](http://docs.keboola.apiary.io/). This API client provides client methods to get data from KBC and store data in KBC. The endpoints \nfor working with buckets, tables and workspaces are covered.\n\n## Install\n\n`$ pip3 install git+https://github.com/keboola/sapi-python-client.git`\n\nor \n\n```bash\n$ git clone https://github.com/keboola/sapi-python-client.git && cd sapi-python-client\n$ python setup.py install\n```\n\n## Client Class Usage\n```\nfrom kbcstorage.client import Client\n\nclient = Client('https://connection.keboola.com', 'your-token')\n\n# get table data into local file\nclient.tables.export_to_file(table_id='in.c-demo.some-table', path_name='/data/')\n\n# save data\nclient.tables.create(name='some-table-2', bucket_id='in.c-demo', file_path='/data/some-table')\n\n# list buckets\nclient.buckets.list()\n\n# list bucket tables\nclient.buckets.list_tables('in.c-demo')\n\n# get table info\nclient.tables.detail('in.c-demo.some-table')\n\n```\n\n## Endpoint Classes Usage \n```\nfrom kbcstorage.tables import Tables\nfrom kbcstorage.buckets import Buckets\n\ntables = Tables('https://connection.keboola.com', 'your-token')\n\n# get table data into local file\ntables.export_to_file(table_id='in.c-demo.some-table', path_name='/data/')\n\n# save data\ntables.create(name='some-table-2', bucket_id='in.c-demo', file_path='/data/some-table')\n\n# list buckets\nbuckets = Buckets('https://connection.keboola.com', 'your-token')\nbuckets.list()\n\n# list bucket tables\nbuckets.list_tables('in.c-demo')\n\n# get table info\ntables.detail('in.c-demo.some-table')\n\n```\n\n## Docker image\nDocker image with pre-installed library is also available, run it via:\n\n```\ndocker run -i -t quay.io/keboola/sapi-python-client\n```\n\n## Tests\n\n```bash\n$ git clone https://github.com/keboola/sapi-python-client.git && cd sapi-python-client\n$ python setup.py test\n```\n\nor \n\n```bash\n$ docker-compose run --rm -e KBC_TEST_TOKEN -e KBC_TEST_API_URL sapi-python-client -m unittest discover\n```\n\n## Contribution Guide\nThe client is far from supporting the entire API, all contributions are very welcome. New API endpoints should \nbe implemeneted in their own class extending `Endpoint`. Naming conventions should follow existing naming conventions\nor those of the [API](http://docs.keboola.apiary.io/#). If the method contains some processing of the request or response, consult the corresponing [PHP implementation](https://github.com/keboola/storage-api-php-client) for reference. New code should be covered by tests.\n\nNote that if you submit a PR from your own forked repository, the automated functional tests will fail. This is limitation of [Travis](https://docs.travis-ci.com/user/pull-requests/#Pull-Requests-and-Security-Restrictions). Either run the tests locally (set `KBC_TEST_TOKEN` (your token to test project) and `KBC_TEST_API_URL` (https://connection.keboola.com) variables) or ask for access. In case, you need a project for local testing, feel free to [ask for one](https://developers.keboola.com/#development-project).\n\nThe recommended workflow for making a pull request is:\n\n```bash\ngit clone https://github.com/keboola/sapi-python-client.git\ngit checkout master\ngit pull\ngit checkout -b my-new-feature\n# work on branch my-new-feature\ngit push origin my-new-feature:my-new-feature\n```\n\nThis will create a new branch which can be used to make a pull request for your new feature.\n\n## License\n\nMIT licensed, see [LICENSE](./LICENSE) file.\n",
-    'author': 'Lukas Langr',
-    'author_email': 'lukas.langr@datasentics.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+# Python client for the Keboola Storage API
+Client for using [Keboola Connection Storage API](http://docs.keboola.apiary.io/). This API client provides client methods to get data from KBC and store data in KBC. The endpoints 
+for working with buckets, tables and workspaces are covered.
 
+## Install
 
-setup(**setup_kwargs)
+`$ pip3 install git+https://github.com/keboola/sapi-python-client.git`
+
+or 
+
+```bash
+$ git clone https://github.com/keboola/sapi-python-client.git && cd sapi-python-client
+$ python setup.py install
+```
+
+## Client Class Usage
+```
+from kbcstorage.client import Client
+
+client = Client('https://connection.keboola.com', 'your-token')
+
+# get table data into local file
+client.tables.export_to_file(table_id='in.c-demo.some-table', path_name='/data/')
+
+# save data
+client.tables.create(name='some-table-2', bucket_id='in.c-demo', file_path='/data/some-table')
+
+# list buckets
+client.buckets.list()
+
+# list bucket tables
+client.buckets.list_tables('in.c-demo')
+
+# get table info
+client.tables.detail('in.c-demo.some-table')
+
+```
+
+## Endpoint Classes Usage 
+```
+from kbcstorage.tables import Tables
+from kbcstorage.buckets import Buckets
+
+tables = Tables('https://connection.keboola.com', 'your-token')
+
+# get table data into local file
+tables.export_to_file(table_id='in.c-demo.some-table', path_name='/data/')
+
+# save data
+tables.create(name='some-table-2', bucket_id='in.c-demo', file_path='/data/some-table')
+
+# list buckets
+buckets = Buckets('https://connection.keboola.com', 'your-token')
+buckets.list()
+
+# list bucket tables
+buckets.list_tables('in.c-demo')
+
+# get table info
+tables.detail('in.c-demo.some-table')
+
+```
+
+## Docker image
+Docker image with pre-installed library is also available, run it via:
+
+```
+docker run -i -t quay.io/keboola/sapi-python-client
+```
+
+## Tests
+
+```bash
+$ git clone https://github.com/keboola/sapi-python-client.git && cd sapi-python-client
+$ python setup.py test
+```
+
+or 
+
+```bash
+$ docker-compose run --rm -e KBC_TEST_TOKEN -e KBC_TEST_API_URL sapi-python-client -m unittest discover
+```
+
+## Contribution Guide
+The client is far from supporting the entire API, all contributions are very welcome. New API endpoints should 
+be implemeneted in their own class extending `Endpoint`. Naming conventions should follow existing naming conventions
+or those of the [API](http://docs.keboola.apiary.io/#). If the method contains some processing of the request or response, consult the corresponing [PHP implementation](https://github.com/keboola/storage-api-php-client) for reference. New code should be covered by tests.
+
+Note that if you submit a PR from your own forked repository, the automated functional tests will fail. This is limitation of [Travis](https://docs.travis-ci.com/user/pull-requests/#Pull-Requests-and-Security-Restrictions). Either run the tests locally (set `KBC_TEST_TOKEN` (your token to test project) and `KBC_TEST_API_URL` (https://connection.keboola.com) variables) or ask for access. In case, you need a project for local testing, feel free to [ask for one](https://developers.keboola.com/#development-project).
+
+The recommended workflow for making a pull request is:
+
+```bash
+git clone https://github.com/keboola/sapi-python-client.git
+git checkout master
+git pull
+git checkout -b my-new-feature
+# work on branch my-new-feature
+git push origin my-new-feature:my-new-feature
+```
+
+This will create a new branch which can be used to make a pull request for your new feature.
+
+## License
+
+MIT licensed, see [LICENSE](./LICENSE) file.
```

### Comparing `kbcstorage-0.0.1/PKG-INFO` & `kbcstorage-0.5.0/kbcstorage.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,16 @@
 Metadata-Version: 2.1
 Name: kbcstorage
-Version: 0.0.1
-Summary: Keboola Storage API
+Version: 0.5.0
+Home-page: https://github.com/keboola/sapi-python-client
+Download-URL: https://github.com/keboola/sapi-python-client
 License: MIT
-Author: Lukas Langr
-Author-email: lukas.langr@datasentics.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: azure-storage-blob (>=12.14.1,<13.0.0)
-Requires-Dist: boto3 (>=1.26.69,<2.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE.txt
 
 [![Build Status](https://travis-ci.org/keboola/sapi-python-client.svg?branch=master)](https://travis-ci.org/keboola/sapi-python-client)
 
 # Python client for the Keboola Storage API
 Client for using [Keboola Connection Storage API](http://docs.keboola.apiary.io/). This API client provides client methods to get data from KBC and store data in KBC. The endpoints 
 for working with buckets, tables and workspaces are covered.
 
@@ -121,8 +112,7 @@
 ```
 
 This will create a new branch which can be used to make a pull request for your new feature.
 
 ## License
 
 MIT licensed, see [LICENSE](./LICENSE) file.
-
```

