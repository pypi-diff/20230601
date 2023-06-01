# Comparing `tmp/sw_product_lib-0.6.0.tar.gz` & `tmp/sw_product_lib-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sw_product_lib-0.6.0.tar", max compression
+gzip compressed data, was "sw_product_lib-0.6.1.tar", max compression
```

## Comparing `sw_product_lib-0.6.0.tar` & `sw_product_lib-0.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1097 2023-05-17 14:43:24.294646 sw_product_lib-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       87 2023-05-17 14:43:24.294646 sw_product_lib-0.6.0/sw_product_lib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 14:43:24.294646 sw_product_lib-0.6.0/sw_product_lib/client/__init__.py
--rw-r--r--   0        0        0    10691 2023-05-17 14:43:24.294646 sw_product_lib-0.6.0/sw_product_lib/client/backend.py
--rw-r--r--   0        0        0     3885 2023-05-17 14:43:24.294646 sw_product_lib-0.6.0/sw_product_lib/client/billing.py
--rw-r--r--   0        0        0     7180 2023-05-17 14:43:24.294646 sw_product_lib-0.6.0/sw_product_lib/client/job.py
--rw-r--r--   0        0        0     2186 2023-05-17 14:43:24.294646 sw_product_lib-0.6.0/sw_product_lib/client/resource.py
--rw-r--r--   0        0        0        0 2023-05-17 14:43:24.294646 sw_product_lib-0.6.0/sw_product_lib/platform/__init__.py
--rw-r--r--   0        0        0      331 2023-05-17 14:43:24.294646 sw_product_lib-0.6.0/sw_product_lib/platform/gql.py
--rw-r--r--   0        0        0    24528 2023-05-17 14:43:24.294646 sw_product_lib-0.6.0/sw_product_lib/service.py
--rw-r--r--   0        0        0    21473 2023-05-17 14:43:24.294646 sw_product_lib-0.6.0/sw_product_lib/types/job.py
--rw-r--r--   0        0        0     8702 2023-05-17 14:43:24.294646 sw_product_lib-0.6.0/sw_product_lib/types/resource.py
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 sw_product_lib-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-06-01 18:06:24.143186 sw_product_lib-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-06-01 18:06:24.143186 sw_product_lib-0.6.1/sw_product_lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 18:06:24.143186 sw_product_lib-0.6.1/sw_product_lib/client/__init__.py
+-rw-r--r--   0        0        0    10691 2023-06-01 18:06:24.143186 sw_product_lib-0.6.1/sw_product_lib/client/backend.py
+-rw-r--r--   0        0        0     3885 2023-06-01 18:06:24.143186 sw_product_lib-0.6.1/sw_product_lib/client/billing.py
+-rw-r--r--   0        0        0     7180 2023-06-01 18:06:24.143186 sw_product_lib-0.6.1/sw_product_lib/client/job.py
+-rw-r--r--   0        0        0     2186 2023-06-01 18:06:24.143186 sw_product_lib-0.6.1/sw_product_lib/client/resource.py
+-rw-r--r--   0        0        0        0 2023-06-01 18:06:24.143186 sw_product_lib-0.6.1/sw_product_lib/platform/__init__.py
+-rw-r--r--   0        0        0      331 2023-06-01 18:06:24.143186 sw_product_lib-0.6.1/sw_product_lib/platform/gql.py
+-rw-r--r--   0        0        0    24528 2023-06-01 18:06:24.143186 sw_product_lib-0.6.1/sw_product_lib/service.py
+-rw-r--r--   0        0        0    21913 2023-06-01 18:06:24.143186 sw_product_lib-0.6.1/sw_product_lib/types/job.py
+-rw-r--r--   0        0        0     8702 2023-06-01 18:06:24.143186 sw_product_lib-0.6.1/sw_product_lib/types/resource.py
+-rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 sw_product_lib-0.6.1/PKG-INFO
```

### Comparing `sw_product_lib-0.6.0/pyproject.toml` & `sw_product_lib-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 per-file-ignores = [
     "__init__.py:F401",
     "./docs/*:E402"
 ]
 
 [tool.poetry]
 name = "sw-product-lib"
-version = "0.6.0"
+version = "0.6.1"
 description = "Python library for Strangeworks products to interact with the Strangeworks Platform"
 authors = ["Strangeworks Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "^12.4.4"
```

### Comparing `sw_product_lib-0.6.0/sw_product_lib/client/backend.py` & `sw_product_lib-0.6.1/sw_product_lib/client/backend.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.0/sw_product_lib/client/billing.py` & `sw_product_lib-0.6.1/sw_product_lib/client/billing.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.0/sw_product_lib/client/job.py` & `sw_product_lib-0.6.1/sw_product_lib/client/job.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.0/sw_product_lib/client/resource.py` & `sw_product_lib-0.6.1/sw_product_lib/client/resource.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.0/sw_product_lib/service.py` & `sw_product_lib-0.6.1/sw_product_lib/service.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.0/sw_product_lib/types/job.py` & `sw_product_lib-0.6.1/sw_product_lib/types/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,21 @@
 class Job(JobBase):
     def __init__(
         self,
         parentJob: Optional[Dict[str, Any]] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
-        self.parent_job_slug = None if parentJob is None else parentJob.get("slug")
+        # if the job is from a graphql query, then the parent job slug will be in
+        # parentJob.
+        # if its from a job object represented as a dictionary, then the parent job
+        # slug will be in kwargs as parent_job_slug.
+        self.parent_job_slug = (
+            parentJob.get("slug") if parentJob else kwargs.get("parent_job_slug")
+        )
 
     def as_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
 class File(FileBase):
     def as_dict(self) -> Dict[str, Any]:
@@ -269,14 +275,20 @@
 get_job_request = Operation(
     query="""
     query job($resource_slug: String!, $job_slug: String!) {
         job(resourceSlug: $resource_slug, jobSlug: $job_slug) {
             id
             childJobs {
                 id
+                slug
+                status
+                isTerminalState
+                remoteStatus
+                jobDataSchema
+                jobData
             }
             externalIdentifier
             slug
             status
             isTerminalState
             remoteStatus
             jobDataSchema
@@ -717,11 +729,11 @@
     sub_job = requests.post(
         url=resource.proxy_url(base_url=base_url, path=path),
         headers={
             "Authorization": f"bearer {proxy_auth_token}",
             "x-resource-api-token": api_key,
             "x-strangeworks-parent-job-slug": parent_job_slug,
         },
-        data=data,
+        json=data,
     )
 
     return sub_job
```

### Comparing `sw_product_lib-0.6.0/sw_product_lib/types/resource.py` & `sw_product_lib-0.6.1/sw_product_lib/types/resource.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.0/PKG-INFO` & `sw_product_lib-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sw-product-lib
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python library for Strangeworks products to interact with the Strangeworks Platform
 License: Apache-2.0
 Author: Strangeworks Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

