# Comparing `tmp/alibabacloud_openitag20220616-1.0.1.tar.gz` & `tmp/alibabacloud_openitag20220616-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_openitag20220616-1.0.1.tar", last modified: Thu Sep 15 07:28:33 2022, max compression
+gzip compressed data, was "dist/alibabacloud_openitag20220616-1.0.2.tar", last modified: Thu Jun  1 07:15:49 2023, max compression
```

## Comparing `alibabacloud_openitag20220616-1.0.1.tar` & `alibabacloud_openitag20220616-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 07:28:33.000000 alibabacloud_openitag20220616-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       35 2022-09-15 07:28:32.000000 alibabacloud_openitag20220616-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-09-15 07:28:32.000000 alibabacloud_openitag20220616-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-09-15 07:28:32.000000 alibabacloud_openitag20220616-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2022-09-15 07:28:33.000000 alibabacloud_openitag20220616-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2022-09-15 07:28:32.000000 alibabacloud_openitag20220616-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2022-09-15 07:28:32.000000 alibabacloud_openitag20220616-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 07:28:33.000000 alibabacloud_openitag20220616-1.0.1/alibabacloud_openitag20220616/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-15 07:28:32.000000 alibabacloud_openitag20220616-1.0.1/alibabacloud_openitag20220616/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112075 2022-09-15 07:28:32.000000 alibabacloud_openitag20220616-1.0.1/alibabacloud_openitag20220616/client.py
--rw-r--r--   0 root         (0) root         (0)   267468 2022-09-15 07:28:32.000000 alibabacloud_openitag20220616-1.0.1/alibabacloud_openitag20220616/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 07:28:33.000000 alibabacloud_openitag20220616-1.0.1/alibabacloud_openitag20220616.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2022-09-15 07:28:32.000000 alibabacloud_openitag20220616-1.0.1/alibabacloud_openitag20220616.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2022-09-15 07:28:33.000000 alibabacloud_openitag20220616-1.0.1/alibabacloud_openitag20220616.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-15 07:28:32.000000 alibabacloud_openitag20220616-1.0.1/alibabacloud_openitag20220616.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-09-15 07:28:32.000000 alibabacloud_openitag20220616-1.0.1/alibabacloud_openitag20220616.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-09-15 07:28:32.000000 alibabacloud_openitag20220616-1.0.1/alibabacloud_openitag20220616.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-15 07:28:33.000000 alibabacloud_openitag20220616-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2022-09-15 07:28:32.000000 alibabacloud_openitag20220616-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:15:49.000000 alibabacloud_openitag20220616-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-01 07:15:48.000000 alibabacloud_openitag20220616-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-01 07:15:48.000000 alibabacloud_openitag20220616-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-01 07:15:48.000000 alibabacloud_openitag20220616-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-01 07:15:49.000000 alibabacloud_openitag20220616-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-06-01 07:15:48.000000 alibabacloud_openitag20220616-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-06-01 07:15:48.000000 alibabacloud_openitag20220616-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:15:49.000000 alibabacloud_openitag20220616-1.0.2/alibabacloud_openitag20220616/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-01 07:15:48.000000 alibabacloud_openitag20220616-1.0.2/alibabacloud_openitag20220616/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   111947 2023-06-01 07:15:48.000000 alibabacloud_openitag20220616-1.0.2/alibabacloud_openitag20220616/client.py
+-rw-r--r--   0 root         (0) root         (0)   268966 2023-06-01 07:15:48.000000 alibabacloud_openitag20220616-1.0.2/alibabacloud_openitag20220616/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:15:49.000000 alibabacloud_openitag20220616-1.0.2/alibabacloud_openitag20220616.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-01 07:15:49.000000 alibabacloud_openitag20220616-1.0.2/alibabacloud_openitag20220616.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-01 07:15:49.000000 alibabacloud_openitag20220616-1.0.2/alibabacloud_openitag20220616.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 07:15:49.000000 alibabacloud_openitag20220616-1.0.2/alibabacloud_openitag20220616.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-01 07:15:49.000000 alibabacloud_openitag20220616-1.0.2/alibabacloud_openitag20220616.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-01 07:15:49.000000 alibabacloud_openitag20220616-1.0.2/alibabacloud_openitag20220616.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-01 07:15:49.000000 alibabacloud_openitag20220616-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-06-01 07:15:48.000000 alibabacloud_openitag20220616-1.0.2/setup.py
```

### Comparing `alibabacloud_openitag20220616-1.0.1/LICENSE` & `alibabacloud_openitag20220616-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_openitag20220616-1.0.1/PKG-INFO` & `alibabacloud_openitag20220616-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_openitag20220616
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud OpenITag (20220616) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_openitag20220616-1.0.1/README-CN.md` & `alibabacloud_openitag20220616-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_openitag20220616-1.0.1/README.md` & `alibabacloud_openitag20220616-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_openitag20220616-1.0.1/alibabacloud_openitag20220616/client.py` & `alibabacloud_openitag20220616-1.0.2/alibabacloud_openitag20220616/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,36 +37,14 @@
     ) -> str:
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
-    def add_work_node_workforce(
-        self,
-        tenant_id: str,
-        task_id: str,
-        work_node_id: str,
-        request: open_itag_20220616_models.AddWorkNodeWorkforceRequest,
-    ) -> open_itag_20220616_models.AddWorkNodeWorkforceResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.add_work_node_workforce_with_options(tenant_id, task_id, work_node_id, request, headers, runtime)
-
-    async def add_work_node_workforce_async(
-        self,
-        tenant_id: str,
-        task_id: str,
-        work_node_id: str,
-        request: open_itag_20220616_models.AddWorkNodeWorkforceRequest,
-    ) -> open_itag_20220616_models.AddWorkNodeWorkforceResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.add_work_node_workforce_with_options_async(tenant_id, task_id, work_node_id, request, headers, runtime)
-
     def add_work_node_workforce_with_options(
         self,
         tenant_id: str,
         task_id: str,
         work_node_id: str,
         request: open_itag_20220616_models.AddWorkNodeWorkforceRequest,
         headers: Dict[str, str],
@@ -125,43 +103,47 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.AddWorkNodeWorkforceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def create_task(
+    def add_work_node_workforce(
         self,
         tenant_id: str,
-        request: open_itag_20220616_models.CreateTaskRequest,
-    ) -> open_itag_20220616_models.CreateTaskResponse:
+        task_id: str,
+        work_node_id: str,
+        request: open_itag_20220616_models.AddWorkNodeWorkforceRequest,
+    ) -> open_itag_20220616_models.AddWorkNodeWorkforceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.create_task_with_options(tenant_id, request, headers, runtime)
+        return self.add_work_node_workforce_with_options(tenant_id, task_id, work_node_id, request, headers, runtime)
 
-    async def create_task_async(
+    async def add_work_node_workforce_async(
         self,
         tenant_id: str,
-        request: open_itag_20220616_models.CreateTaskRequest,
-    ) -> open_itag_20220616_models.CreateTaskResponse:
+        task_id: str,
+        work_node_id: str,
+        request: open_itag_20220616_models.AddWorkNodeWorkforceRequest,
+    ) -> open_itag_20220616_models.AddWorkNodeWorkforceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.create_task_with_options_async(tenant_id, request, headers, runtime)
+        return await self.add_work_node_workforce_with_options_async(tenant_id, task_id, work_node_id, request, headers, runtime)
 
     def create_task_with_options(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateTaskRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.CreateTaskResponse:
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(TeaCore.to_map(request.body))
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateTask',
             version='2022-06-16',
             protocol='HTTPS',
             pathname=f'/openapi/api/v1/tenants/{OpenApiUtilClient.get_encode_param(tenant_id)}/tasks',
             method='POST',
@@ -181,15 +163,15 @@
         request: open_itag_20220616_models.CreateTaskRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.CreateTaskResponse:
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(TeaCore.to_map(request.body))
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateTask',
             version='2022-06-16',
             protocol='HTTPS',
             pathname=f'/openapi/api/v1/tenants/{OpenApiUtilClient.get_encode_param(tenant_id)}/tasks',
             method='POST',
@@ -199,43 +181,43 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.CreateTaskResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def create_template(
+    def create_task(
         self,
         tenant_id: str,
-        request: open_itag_20220616_models.CreateTemplateRequest,
-    ) -> open_itag_20220616_models.CreateTemplateResponse:
+        request: open_itag_20220616_models.CreateTaskRequest,
+    ) -> open_itag_20220616_models.CreateTaskResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.create_template_with_options(tenant_id, request, headers, runtime)
+        return self.create_task_with_options(tenant_id, request, headers, runtime)
 
-    async def create_template_async(
+    async def create_task_async(
         self,
         tenant_id: str,
-        request: open_itag_20220616_models.CreateTemplateRequest,
-    ) -> open_itag_20220616_models.CreateTemplateResponse:
+        request: open_itag_20220616_models.CreateTaskRequest,
+    ) -> open_itag_20220616_models.CreateTaskResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.create_template_with_options_async(tenant_id, request, headers, runtime)
+        return await self.create_task_with_options_async(tenant_id, request, headers, runtime)
 
     def create_template_with_options(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateTemplateRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.CreateTemplateResponse:
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(TeaCore.to_map(request.body))
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateTemplate',
             version='2022-06-16',
             protocol='HTTPS',
             pathname=f'/openapi/api/v1/tenants/{OpenApiUtilClient.get_encode_param(tenant_id)}/templates',
             method='POST',
@@ -255,15 +237,15 @@
         request: open_itag_20220616_models.CreateTemplateRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.CreateTemplateResponse:
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(TeaCore.to_map(request.body))
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateTemplate',
             version='2022-06-16',
             protocol='HTTPS',
             pathname=f'/openapi/api/v1/tenants/{OpenApiUtilClient.get_encode_param(tenant_id)}/templates',
             method='POST',
@@ -273,31 +255,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.CreateTemplateResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def create_user(
+    def create_template(
         self,
         tenant_id: str,
-        request: open_itag_20220616_models.CreateUserRequest,
-    ) -> open_itag_20220616_models.CreateUserResponse:
+        request: open_itag_20220616_models.CreateTemplateRequest,
+    ) -> open_itag_20220616_models.CreateTemplateResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.create_user_with_options(tenant_id, request, headers, runtime)
+        return self.create_template_with_options(tenant_id, request, headers, runtime)
 
-    async def create_user_async(
+    async def create_template_async(
         self,
         tenant_id: str,
-        request: open_itag_20220616_models.CreateUserRequest,
-    ) -> open_itag_20220616_models.CreateUserResponse:
+        request: open_itag_20220616_models.CreateTemplateRequest,
+    ) -> open_itag_20220616_models.CreateTemplateResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.create_user_with_options_async(tenant_id, request, headers, runtime)
+        return await self.create_template_with_options_async(tenant_id, request, headers, runtime)
 
     def create_user_with_options(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateUserRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -365,31 +347,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.CreateUserResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def delete_task(
+    def create_user(
         self,
         tenant_id: str,
-        task_id: str,
-    ) -> open_itag_20220616_models.DeleteTaskResponse:
+        request: open_itag_20220616_models.CreateUserRequest,
+    ) -> open_itag_20220616_models.CreateUserResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.delete_task_with_options(tenant_id, task_id, headers, runtime)
+        return self.create_user_with_options(tenant_id, request, headers, runtime)
 
-    async def delete_task_async(
+    async def create_user_async(
         self,
         tenant_id: str,
-        task_id: str,
-    ) -> open_itag_20220616_models.DeleteTaskResponse:
+        request: open_itag_20220616_models.CreateUserRequest,
+    ) -> open_itag_20220616_models.CreateUserResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.delete_task_with_options_async(tenant_id, task_id, headers, runtime)
+        return await self.create_user_with_options_async(tenant_id, request, headers, runtime)
 
     def delete_task_with_options(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -435,31 +417,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.DeleteTaskResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def delete_template(
+    def delete_task(
         self,
         tenant_id: str,
-        template_id: str,
-    ) -> open_itag_20220616_models.DeleteTemplateResponse:
+        task_id: str,
+    ) -> open_itag_20220616_models.DeleteTaskResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.delete_template_with_options(tenant_id, template_id, headers, runtime)
+        return self.delete_task_with_options(tenant_id, task_id, headers, runtime)
 
-    async def delete_template_async(
+    async def delete_task_async(
         self,
         tenant_id: str,
-        template_id: str,
-    ) -> open_itag_20220616_models.DeleteTemplateResponse:
+        task_id: str,
+    ) -> open_itag_20220616_models.DeleteTaskResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.delete_template_with_options_async(tenant_id, template_id, headers, runtime)
+        return await self.delete_task_with_options_async(tenant_id, task_id, headers, runtime)
 
     def delete_template_with_options(
         self,
         tenant_id: str,
         template_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -505,31 +487,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.DeleteTemplateResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def delete_user(
+    def delete_template(
         self,
         tenant_id: str,
-        user_id: str,
-    ) -> open_itag_20220616_models.DeleteUserResponse:
+        template_id: str,
+    ) -> open_itag_20220616_models.DeleteTemplateResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.delete_user_with_options(tenant_id, user_id, headers, runtime)
+        return self.delete_template_with_options(tenant_id, template_id, headers, runtime)
 
-    async def delete_user_async(
+    async def delete_template_async(
         self,
         tenant_id: str,
-        user_id: str,
-    ) -> open_itag_20220616_models.DeleteUserResponse:
+        template_id: str,
+    ) -> open_itag_20220616_models.DeleteTemplateResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.delete_user_with_options_async(tenant_id, user_id, headers, runtime)
+        return await self.delete_template_with_options_async(tenant_id, template_id, headers, runtime)
 
     def delete_user_with_options(
         self,
         tenant_id: str,
         user_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -575,33 +557,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.DeleteUserResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def export_annotations(
+    def delete_user(
         self,
         tenant_id: str,
-        task_id: str,
-        request: open_itag_20220616_models.ExportAnnotationsRequest,
-    ) -> open_itag_20220616_models.ExportAnnotationsResponse:
+        user_id: str,
+    ) -> open_itag_20220616_models.DeleteUserResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.export_annotations_with_options(tenant_id, task_id, request, headers, runtime)
+        return self.delete_user_with_options(tenant_id, user_id, headers, runtime)
 
-    async def export_annotations_async(
+    async def delete_user_async(
         self,
         tenant_id: str,
-        task_id: str,
-        request: open_itag_20220616_models.ExportAnnotationsRequest,
-    ) -> open_itag_20220616_models.ExportAnnotationsResponse:
+        user_id: str,
+    ) -> open_itag_20220616_models.DeleteUserResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.export_annotations_with_options_async(tenant_id, task_id, request, headers, runtime)
+        return await self.delete_user_with_options_async(tenant_id, user_id, headers, runtime)
 
     def export_annotations_with_options(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.ExportAnnotationsRequest,
         headers: Dict[str, str],
@@ -667,33 +647,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ExportAnnotationsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_job(
+    def export_annotations(
         self,
         tenant_id: str,
-        job_id: str,
-        request: open_itag_20220616_models.GetJobRequest,
-    ) -> open_itag_20220616_models.GetJobResponse:
+        task_id: str,
+        request: open_itag_20220616_models.ExportAnnotationsRequest,
+    ) -> open_itag_20220616_models.ExportAnnotationsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_job_with_options(tenant_id, job_id, request, headers, runtime)
+        return self.export_annotations_with_options(tenant_id, task_id, request, headers, runtime)
 
-    async def get_job_async(
+    async def export_annotations_async(
         self,
         tenant_id: str,
-        job_id: str,
-        request: open_itag_20220616_models.GetJobRequest,
-    ) -> open_itag_20220616_models.GetJobResponse:
+        task_id: str,
+        request: open_itag_20220616_models.ExportAnnotationsRequest,
+    ) -> open_itag_20220616_models.ExportAnnotationsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_job_with_options_async(tenant_id, job_id, request, headers, runtime)
+        return await self.export_annotations_with_options_async(tenant_id, task_id, request, headers, runtime)
 
     def get_job_with_options(
         self,
         tenant_id: str,
         job_id: str,
         request: open_itag_20220616_models.GetJobRequest,
         headers: Dict[str, str],
@@ -751,33 +731,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetJobResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_subtask(
+    def get_job(
         self,
         tenant_id: str,
-        task_id: str,
-        subtask_id: str,
-    ) -> open_itag_20220616_models.GetSubtaskResponse:
+        job_id: str,
+        request: open_itag_20220616_models.GetJobRequest,
+    ) -> open_itag_20220616_models.GetJobResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_subtask_with_options(tenant_id, task_id, subtask_id, headers, runtime)
+        return self.get_job_with_options(tenant_id, job_id, request, headers, runtime)
 
-    async def get_subtask_async(
+    async def get_job_async(
         self,
         tenant_id: str,
-        task_id: str,
-        subtask_id: str,
-    ) -> open_itag_20220616_models.GetSubtaskResponse:
+        job_id: str,
+        request: open_itag_20220616_models.GetJobRequest,
+    ) -> open_itag_20220616_models.GetJobResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_subtask_with_options_async(tenant_id, task_id, subtask_id, headers, runtime)
+        return await self.get_job_with_options_async(tenant_id, job_id, request, headers, runtime)
 
     def get_subtask_with_options(
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
         headers: Dict[str, str],
@@ -825,35 +805,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetSubtaskResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_subtask_item(
+    def get_subtask(
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
-        item_id: str,
-    ) -> open_itag_20220616_models.GetSubtaskItemResponse:
+    ) -> open_itag_20220616_models.GetSubtaskResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_subtask_item_with_options(tenant_id, task_id, subtask_id, item_id, headers, runtime)
+        return self.get_subtask_with_options(tenant_id, task_id, subtask_id, headers, runtime)
 
-    async def get_subtask_item_async(
+    async def get_subtask_async(
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
-        item_id: str,
-    ) -> open_itag_20220616_models.GetSubtaskItemResponse:
+    ) -> open_itag_20220616_models.GetSubtaskResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_subtask_item_with_options_async(tenant_id, task_id, subtask_id, item_id, headers, runtime)
+        return await self.get_subtask_with_options_async(tenant_id, task_id, subtask_id, headers, runtime)
 
     def get_subtask_item_with_options(
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
         item_id: str,
@@ -903,31 +881,35 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetSubtaskItemResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_task(
+    def get_subtask_item(
         self,
         tenant_id: str,
         task_id: str,
-    ) -> open_itag_20220616_models.GetTaskResponse:
+        subtask_id: str,
+        item_id: str,
+    ) -> open_itag_20220616_models.GetSubtaskItemResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_with_options(tenant_id, task_id, headers, runtime)
+        return self.get_subtask_item_with_options(tenant_id, task_id, subtask_id, item_id, headers, runtime)
 
-    async def get_task_async(
+    async def get_subtask_item_async(
         self,
         tenant_id: str,
         task_id: str,
-    ) -> open_itag_20220616_models.GetTaskResponse:
+        subtask_id: str,
+        item_id: str,
+    ) -> open_itag_20220616_models.GetSubtaskItemResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_task_with_options_async(tenant_id, task_id, headers, runtime)
+        return await self.get_subtask_item_with_options_async(tenant_id, task_id, subtask_id, item_id, headers, runtime)
 
     def get_task_with_options(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -973,33 +955,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_task_statistics(
+    def get_task(
         self,
         tenant_id: str,
         task_id: str,
-        request: open_itag_20220616_models.GetTaskStatisticsRequest,
-    ) -> open_itag_20220616_models.GetTaskStatisticsResponse:
+    ) -> open_itag_20220616_models.GetTaskResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_statistics_with_options(tenant_id, task_id, request, headers, runtime)
+        return self.get_task_with_options(tenant_id, task_id, headers, runtime)
 
-    async def get_task_statistics_async(
+    async def get_task_async(
         self,
         tenant_id: str,
         task_id: str,
-        request: open_itag_20220616_models.GetTaskStatisticsRequest,
-    ) -> open_itag_20220616_models.GetTaskStatisticsResponse:
+    ) -> open_itag_20220616_models.GetTaskResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_task_statistics_with_options_async(tenant_id, task_id, request, headers, runtime)
+        return await self.get_task_with_options_async(tenant_id, task_id, headers, runtime)
 
     def get_task_statistics_with_options(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.GetTaskStatisticsRequest,
         headers: Dict[str, str],
@@ -1057,31 +1037,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskStatisticsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_task_status(
+    def get_task_statistics(
         self,
         tenant_id: str,
         task_id: str,
-    ) -> open_itag_20220616_models.GetTaskStatusResponse:
+        request: open_itag_20220616_models.GetTaskStatisticsRequest,
+    ) -> open_itag_20220616_models.GetTaskStatisticsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_status_with_options(tenant_id, task_id, headers, runtime)
+        return self.get_task_statistics_with_options(tenant_id, task_id, request, headers, runtime)
 
-    async def get_task_status_async(
+    async def get_task_statistics_async(
         self,
         tenant_id: str,
         task_id: str,
-    ) -> open_itag_20220616_models.GetTaskStatusResponse:
+        request: open_itag_20220616_models.GetTaskStatisticsRequest,
+    ) -> open_itag_20220616_models.GetTaskStatisticsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_task_status_with_options_async(tenant_id, task_id, headers, runtime)
+        return await self.get_task_statistics_with_options_async(tenant_id, task_id, request, headers, runtime)
 
     def get_task_status_with_options(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -1127,31 +1109,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskStatusResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_task_template(
+    def get_task_status(
         self,
         tenant_id: str,
         task_id: str,
-    ) -> open_itag_20220616_models.GetTaskTemplateResponse:
+    ) -> open_itag_20220616_models.GetTaskStatusResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_template_with_options(tenant_id, task_id, headers, runtime)
+        return self.get_task_status_with_options(tenant_id, task_id, headers, runtime)
 
-    async def get_task_template_async(
+    async def get_task_status_async(
         self,
         tenant_id: str,
         task_id: str,
-    ) -> open_itag_20220616_models.GetTaskTemplateResponse:
+    ) -> open_itag_20220616_models.GetTaskStatusResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_task_template_with_options_async(tenant_id, task_id, headers, runtime)
+        return await self.get_task_status_with_options_async(tenant_id, task_id, headers, runtime)
 
     def get_task_template_with_options(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -1197,31 +1179,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskTemplateResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_task_template_questions(
+    def get_task_template(
         self,
         tenant_id: str,
         task_id: str,
-    ) -> open_itag_20220616_models.GetTaskTemplateQuestionsResponse:
+    ) -> open_itag_20220616_models.GetTaskTemplateResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_template_questions_with_options(tenant_id, task_id, headers, runtime)
+        return self.get_task_template_with_options(tenant_id, task_id, headers, runtime)
 
-    async def get_task_template_questions_async(
+    async def get_task_template_async(
         self,
         tenant_id: str,
         task_id: str,
-    ) -> open_itag_20220616_models.GetTaskTemplateQuestionsResponse:
+    ) -> open_itag_20220616_models.GetTaskTemplateResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_task_template_questions_with_options_async(tenant_id, task_id, headers, runtime)
+        return await self.get_task_template_with_options_async(tenant_id, task_id, headers, runtime)
 
     def get_task_template_questions_with_options(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -1267,31 +1249,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskTemplateQuestionsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_task_template_views(
+    def get_task_template_questions(
         self,
         tenant_id: str,
         task_id: str,
-    ) -> open_itag_20220616_models.GetTaskTemplateViewsResponse:
+    ) -> open_itag_20220616_models.GetTaskTemplateQuestionsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_template_views_with_options(tenant_id, task_id, headers, runtime)
+        return self.get_task_template_questions_with_options(tenant_id, task_id, headers, runtime)
 
-    async def get_task_template_views_async(
+    async def get_task_template_questions_async(
         self,
         tenant_id: str,
         task_id: str,
-    ) -> open_itag_20220616_models.GetTaskTemplateViewsResponse:
+    ) -> open_itag_20220616_models.GetTaskTemplateQuestionsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_task_template_views_with_options_async(tenant_id, task_id, headers, runtime)
+        return await self.get_task_template_questions_with_options_async(tenant_id, task_id, headers, runtime)
 
     def get_task_template_views_with_options(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -1337,31 +1319,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskTemplateViewsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_task_workforce(
+    def get_task_template_views(
         self,
         tenant_id: str,
         task_id: str,
-    ) -> open_itag_20220616_models.GetTaskWorkforceResponse:
+    ) -> open_itag_20220616_models.GetTaskTemplateViewsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_workforce_with_options(tenant_id, task_id, headers, runtime)
+        return self.get_task_template_views_with_options(tenant_id, task_id, headers, runtime)
 
-    async def get_task_workforce_async(
+    async def get_task_template_views_async(
         self,
         tenant_id: str,
         task_id: str,
-    ) -> open_itag_20220616_models.GetTaskWorkforceResponse:
+    ) -> open_itag_20220616_models.GetTaskTemplateViewsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_task_workforce_with_options_async(tenant_id, task_id, headers, runtime)
+        return await self.get_task_template_views_with_options_async(tenant_id, task_id, headers, runtime)
 
     def get_task_workforce_with_options(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -1407,33 +1389,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskWorkforceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_task_workforce_statistic(
+    def get_task_workforce(
         self,
         tenant_id: str,
         task_id: str,
-        request: open_itag_20220616_models.GetTaskWorkforceStatisticRequest,
-    ) -> open_itag_20220616_models.GetTaskWorkforceStatisticResponse:
+    ) -> open_itag_20220616_models.GetTaskWorkforceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_workforce_statistic_with_options(tenant_id, task_id, request, headers, runtime)
+        return self.get_task_workforce_with_options(tenant_id, task_id, headers, runtime)
 
-    async def get_task_workforce_statistic_async(
+    async def get_task_workforce_async(
         self,
         tenant_id: str,
         task_id: str,
-        request: open_itag_20220616_models.GetTaskWorkforceStatisticRequest,
-    ) -> open_itag_20220616_models.GetTaskWorkforceStatisticResponse:
+    ) -> open_itag_20220616_models.GetTaskWorkforceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_task_workforce_statistic_with_options_async(tenant_id, task_id, request, headers, runtime)
+        return await self.get_task_workforce_with_options_async(tenant_id, task_id, headers, runtime)
 
     def get_task_workforce_statistic_with_options(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.GetTaskWorkforceStatisticRequest,
         headers: Dict[str, str],
@@ -1499,31 +1479,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskWorkforceStatisticResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_template(
+    def get_task_workforce_statistic(
         self,
         tenant_id: str,
-        template_id: str,
-    ) -> open_itag_20220616_models.GetTemplateResponse:
+        task_id: str,
+        request: open_itag_20220616_models.GetTaskWorkforceStatisticRequest,
+    ) -> open_itag_20220616_models.GetTaskWorkforceStatisticResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_template_with_options(tenant_id, template_id, headers, runtime)
+        return self.get_task_workforce_statistic_with_options(tenant_id, task_id, request, headers, runtime)
 
-    async def get_template_async(
+    async def get_task_workforce_statistic_async(
         self,
         tenant_id: str,
-        template_id: str,
-    ) -> open_itag_20220616_models.GetTemplateResponse:
+        task_id: str,
+        request: open_itag_20220616_models.GetTaskWorkforceStatisticRequest,
+    ) -> open_itag_20220616_models.GetTaskWorkforceStatisticResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_template_with_options_async(tenant_id, template_id, headers, runtime)
+        return await self.get_task_workforce_statistic_with_options_async(tenant_id, task_id, request, headers, runtime)
 
     def get_template_with_options(
         self,
         tenant_id: str,
         template_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -1569,31 +1551,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTemplateResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_template_questions(
+    def get_template(
         self,
         tenant_id: str,
         template_id: str,
-    ) -> open_itag_20220616_models.GetTemplateQuestionsResponse:
+    ) -> open_itag_20220616_models.GetTemplateResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_template_questions_with_options(tenant_id, template_id, headers, runtime)
+        return self.get_template_with_options(tenant_id, template_id, headers, runtime)
 
-    async def get_template_questions_async(
+    async def get_template_async(
         self,
         tenant_id: str,
         template_id: str,
-    ) -> open_itag_20220616_models.GetTemplateQuestionsResponse:
+    ) -> open_itag_20220616_models.GetTemplateResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_template_questions_with_options_async(tenant_id, template_id, headers, runtime)
+        return await self.get_template_with_options_async(tenant_id, template_id, headers, runtime)
 
     def get_template_questions_with_options(
         self,
         tenant_id: str,
         template_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -1639,31 +1621,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTemplateQuestionsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_template_view(
+    def get_template_questions(
         self,
         tenant_id: str,
         template_id: str,
-    ) -> open_itag_20220616_models.GetTemplateViewResponse:
+    ) -> open_itag_20220616_models.GetTemplateQuestionsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_template_view_with_options(tenant_id, template_id, headers, runtime)
+        return self.get_template_questions_with_options(tenant_id, template_id, headers, runtime)
 
-    async def get_template_view_async(
+    async def get_template_questions_async(
         self,
         tenant_id: str,
         template_id: str,
-    ) -> open_itag_20220616_models.GetTemplateViewResponse:
+    ) -> open_itag_20220616_models.GetTemplateQuestionsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_template_view_with_options_async(tenant_id, template_id, headers, runtime)
+        return await self.get_template_questions_with_options_async(tenant_id, template_id, headers, runtime)
 
     def get_template_view_with_options(
         self,
         tenant_id: str,
         template_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -1709,29 +1691,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTemplateViewResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_tenant(
+    def get_template_view(
         self,
         tenant_id: str,
-    ) -> open_itag_20220616_models.GetTenantResponse:
+        template_id: str,
+    ) -> open_itag_20220616_models.GetTemplateViewResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_tenant_with_options(tenant_id, headers, runtime)
+        return self.get_template_view_with_options(tenant_id, template_id, headers, runtime)
 
-    async def get_tenant_async(
+    async def get_template_view_async(
         self,
         tenant_id: str,
-    ) -> open_itag_20220616_models.GetTenantResponse:
+        template_id: str,
+    ) -> open_itag_20220616_models.GetTemplateViewResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_tenant_with_options_async(tenant_id, headers, runtime)
+        return await self.get_template_view_with_options_async(tenant_id, template_id, headers, runtime)
 
     def get_tenant_with_options(
         self,
         tenant_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTenantResponse:
@@ -1775,31 +1759,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTenantResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_user(
+    def get_tenant(
         self,
         tenant_id: str,
-        user_id: str,
-    ) -> open_itag_20220616_models.GetUserResponse:
+    ) -> open_itag_20220616_models.GetTenantResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_user_with_options(tenant_id, user_id, headers, runtime)
+        return self.get_tenant_with_options(tenant_id, headers, runtime)
 
-    async def get_user_async(
+    async def get_tenant_async(
         self,
         tenant_id: str,
-        user_id: str,
-    ) -> open_itag_20220616_models.GetUserResponse:
+    ) -> open_itag_20220616_models.GetTenantResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_user_with_options_async(tenant_id, user_id, headers, runtime)
+        return await self.get_tenant_with_options_async(tenant_id, headers, runtime)
 
     def get_user_with_options(
         self,
         tenant_id: str,
         user_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -1845,31 +1827,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetUserResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_jobs(
+    def get_user(
         self,
         tenant_id: str,
-        request: open_itag_20220616_models.ListJobsRequest,
-    ) -> open_itag_20220616_models.ListJobsResponse:
+        user_id: str,
+    ) -> open_itag_20220616_models.GetUserResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_jobs_with_options(tenant_id, request, headers, runtime)
+        return self.get_user_with_options(tenant_id, user_id, headers, runtime)
 
-    async def list_jobs_async(
+    async def get_user_async(
         self,
         tenant_id: str,
-        request: open_itag_20220616_models.ListJobsRequest,
-    ) -> open_itag_20220616_models.ListJobsResponse:
+        user_id: str,
+    ) -> open_itag_20220616_models.GetUserResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_jobs_with_options_async(tenant_id, request, headers, runtime)
+        return await self.get_user_with_options_async(tenant_id, user_id, headers, runtime)
 
     def list_jobs_with_options(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListJobsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -1933,35 +1915,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ListJobsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_subtask_items(
+    def list_jobs(
         self,
         tenant_id: str,
-        task_id: str,
-        subtask_id: str,
-        request: open_itag_20220616_models.ListSubtaskItemsRequest,
-    ) -> open_itag_20220616_models.ListSubtaskItemsResponse:
+        request: open_itag_20220616_models.ListJobsRequest,
+    ) -> open_itag_20220616_models.ListJobsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_subtask_items_with_options(tenant_id, task_id, subtask_id, request, headers, runtime)
+        return self.list_jobs_with_options(tenant_id, request, headers, runtime)
 
-    async def list_subtask_items_async(
+    async def list_jobs_async(
         self,
         tenant_id: str,
-        task_id: str,
-        subtask_id: str,
-        request: open_itag_20220616_models.ListSubtaskItemsRequest,
-    ) -> open_itag_20220616_models.ListSubtaskItemsResponse:
+        request: open_itag_20220616_models.ListJobsRequest,
+    ) -> open_itag_20220616_models.ListJobsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_subtask_items_with_options_async(tenant_id, task_id, subtask_id, request, headers, runtime)
+        return await self.list_jobs_with_options_async(tenant_id, request, headers, runtime)
 
     def list_subtask_items_with_options(
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
         request: open_itag_20220616_models.ListSubtaskItemsRequest,
@@ -2025,33 +2003,35 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ListSubtaskItemsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_subtasks(
+    def list_subtask_items(
         self,
         tenant_id: str,
         task_id: str,
-        request: open_itag_20220616_models.ListSubtasksRequest,
-    ) -> open_itag_20220616_models.ListSubtasksResponse:
+        subtask_id: str,
+        request: open_itag_20220616_models.ListSubtaskItemsRequest,
+    ) -> open_itag_20220616_models.ListSubtaskItemsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_subtasks_with_options(tenant_id, task_id, request, headers, runtime)
+        return self.list_subtask_items_with_options(tenant_id, task_id, subtask_id, request, headers, runtime)
 
-    async def list_subtasks_async(
+    async def list_subtask_items_async(
         self,
         tenant_id: str,
         task_id: str,
-        request: open_itag_20220616_models.ListSubtasksRequest,
-    ) -> open_itag_20220616_models.ListSubtasksResponse:
+        subtask_id: str,
+        request: open_itag_20220616_models.ListSubtaskItemsRequest,
+    ) -> open_itag_20220616_models.ListSubtaskItemsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_subtasks_with_options_async(tenant_id, task_id, request, headers, runtime)
+        return await self.list_subtask_items_with_options_async(tenant_id, task_id, subtask_id, request, headers, runtime)
 
     def list_subtasks_with_options(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.ListSubtasksRequest,
         headers: Dict[str, str],
@@ -2113,31 +2093,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ListSubtasksResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_tasks(
+    def list_subtasks(
         self,
         tenant_id: str,
-        request: open_itag_20220616_models.ListTasksRequest,
-    ) -> open_itag_20220616_models.ListTasksResponse:
+        task_id: str,
+        request: open_itag_20220616_models.ListSubtasksRequest,
+    ) -> open_itag_20220616_models.ListSubtasksResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_tasks_with_options(tenant_id, request, headers, runtime)
+        return self.list_subtasks_with_options(tenant_id, task_id, request, headers, runtime)
 
-    async def list_tasks_async(
+    async def list_subtasks_async(
         self,
         tenant_id: str,
-        request: open_itag_20220616_models.ListTasksRequest,
-    ) -> open_itag_20220616_models.ListTasksResponse:
+        task_id: str,
+        request: open_itag_20220616_models.ListSubtasksRequest,
+    ) -> open_itag_20220616_models.ListSubtasksResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_tasks_with_options_async(tenant_id, request, headers, runtime)
+        return await self.list_subtasks_with_options_async(tenant_id, task_id, request, headers, runtime)
 
     def list_tasks_with_options(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListTasksRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -2197,31 +2179,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ListTasksResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_templates(
+    def list_tasks(
         self,
         tenant_id: str,
-        request: open_itag_20220616_models.ListTemplatesRequest,
-    ) -> open_itag_20220616_models.ListTemplatesResponse:
+        request: open_itag_20220616_models.ListTasksRequest,
+    ) -> open_itag_20220616_models.ListTasksResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_templates_with_options(tenant_id, request, headers, runtime)
+        return self.list_tasks_with_options(tenant_id, request, headers, runtime)
 
-    async def list_templates_async(
+    async def list_tasks_async(
         self,
         tenant_id: str,
-        request: open_itag_20220616_models.ListTemplatesRequest,
-    ) -> open_itag_20220616_models.ListTemplatesResponse:
+        request: open_itag_20220616_models.ListTasksRequest,
+    ) -> open_itag_20220616_models.ListTasksResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_templates_with_options_async(tenant_id, request, headers, runtime)
+        return await self.list_tasks_with_options_async(tenant_id, request, headers, runtime)
 
     def list_templates_with_options(
         self,
         tenant_id: str,
         tmp_req: open_itag_20220616_models.ListTemplatesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -2297,29 +2279,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ListTemplatesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_tenants(
+    def list_templates(
         self,
-        request: open_itag_20220616_models.ListTenantsRequest,
-    ) -> open_itag_20220616_models.ListTenantsResponse:
+        tenant_id: str,
+        request: open_itag_20220616_models.ListTemplatesRequest,
+    ) -> open_itag_20220616_models.ListTemplatesResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_tenants_with_options(request, headers, runtime)
+        return self.list_templates_with_options(tenant_id, request, headers, runtime)
 
-    async def list_tenants_async(
+    async def list_templates_async(
         self,
-        request: open_itag_20220616_models.ListTenantsRequest,
-    ) -> open_itag_20220616_models.ListTenantsResponse:
+        tenant_id: str,
+        request: open_itag_20220616_models.ListTemplatesRequest,
+    ) -> open_itag_20220616_models.ListTemplatesResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_tenants_with_options_async(request, headers, runtime)
+        return await self.list_templates_with_options_async(tenant_id, request, headers, runtime)
 
     def list_tenants_with_options(
         self,
         request: open_itag_20220616_models.ListTenantsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListTenantsResponse:
@@ -2377,31 +2361,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ListTenantsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_users(
+    def list_tenants(
         self,
-        tenant_id: str,
-        request: open_itag_20220616_models.ListUsersRequest,
-    ) -> open_itag_20220616_models.ListUsersResponse:
+        request: open_itag_20220616_models.ListTenantsRequest,
+    ) -> open_itag_20220616_models.ListTenantsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_users_with_options(tenant_id, request, headers, runtime)
+        return self.list_tenants_with_options(request, headers, runtime)
 
-    async def list_users_async(
+    async def list_tenants_async(
         self,
-        tenant_id: str,
-        request: open_itag_20220616_models.ListUsersRequest,
-    ) -> open_itag_20220616_models.ListUsersResponse:
+        request: open_itag_20220616_models.ListTenantsRequest,
+    ) -> open_itag_20220616_models.ListTenantsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_users_with_options_async(tenant_id, request, headers, runtime)
+        return await self.list_tenants_with_options_async(request, headers, runtime)
 
     def list_users_with_options(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListUsersRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -2461,35 +2443,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ListUsersResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def remove_work_node_workforce(
+    def list_users(
         self,
         tenant_id: str,
-        task_id: str,
-        work_node_id: str,
-        request: open_itag_20220616_models.RemoveWorkNodeWorkforceRequest,
-    ) -> open_itag_20220616_models.RemoveWorkNodeWorkforceResponse:
+        request: open_itag_20220616_models.ListUsersRequest,
+    ) -> open_itag_20220616_models.ListUsersResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.remove_work_node_workforce_with_options(tenant_id, task_id, work_node_id, request, headers, runtime)
+        return self.list_users_with_options(tenant_id, request, headers, runtime)
 
-    async def remove_work_node_workforce_async(
+    async def list_users_async(
         self,
         tenant_id: str,
-        task_id: str,
-        work_node_id: str,
-        request: open_itag_20220616_models.RemoveWorkNodeWorkforceRequest,
-    ) -> open_itag_20220616_models.RemoveWorkNodeWorkforceResponse:
+        request: open_itag_20220616_models.ListUsersRequest,
+    ) -> open_itag_20220616_models.ListUsersResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.remove_work_node_workforce_with_options_async(tenant_id, task_id, work_node_id, request, headers, runtime)
+        return await self.list_users_with_options_async(tenant_id, request, headers, runtime)
 
     def remove_work_node_workforce_with_options(
         self,
         tenant_id: str,
         task_id: str,
         work_node_id: str,
         request: open_itag_20220616_models.RemoveWorkNodeWorkforceRequest,
@@ -2549,46 +2527,48 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.RemoveWorkNodeWorkforceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def update_task(
+    def remove_work_node_workforce(
         self,
         tenant_id: str,
         task_id: str,
-        request: open_itag_20220616_models.UpdateTaskRequest,
-    ) -> open_itag_20220616_models.UpdateTaskResponse:
+        work_node_id: str,
+        request: open_itag_20220616_models.RemoveWorkNodeWorkforceRequest,
+    ) -> open_itag_20220616_models.RemoveWorkNodeWorkforceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.update_task_with_options(tenant_id, task_id, request, headers, runtime)
+        return self.remove_work_node_workforce_with_options(tenant_id, task_id, work_node_id, request, headers, runtime)
 
-    async def update_task_async(
+    async def remove_work_node_workforce_async(
         self,
         tenant_id: str,
         task_id: str,
-        request: open_itag_20220616_models.UpdateTaskRequest,
-    ) -> open_itag_20220616_models.UpdateTaskResponse:
+        work_node_id: str,
+        request: open_itag_20220616_models.RemoveWorkNodeWorkforceRequest,
+    ) -> open_itag_20220616_models.RemoveWorkNodeWorkforceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.update_task_with_options_async(tenant_id, task_id, request, headers, runtime)
+        return await self.remove_work_node_workforce_with_options_async(tenant_id, task_id, work_node_id, request, headers, runtime)
 
     def update_task_with_options(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.UpdateTaskRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.UpdateTaskResponse:
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(TeaCore.to_map(request.body))
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='UpdateTask',
             version='2022-06-16',
             protocol='HTTPS',
             pathname=f'/openapi/api/v1/tenants/{OpenApiUtilClient.get_encode_param(tenant_id)}/tasks/{OpenApiUtilClient.get_encode_param(task_id)}',
             method='PUT',
@@ -2609,15 +2589,15 @@
         request: open_itag_20220616_models.UpdateTaskRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.UpdateTaskResponse:
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(TeaCore.to_map(request.body))
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='UpdateTask',
             version='2022-06-16',
             protocol='HTTPS',
             pathname=f'/openapi/api/v1/tenants/{OpenApiUtilClient.get_encode_param(tenant_id)}/tasks/{OpenApiUtilClient.get_encode_param(task_id)}',
             method='PUT',
@@ -2627,33 +2607,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.UpdateTaskResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def update_task_workforce(
+    def update_task(
         self,
         tenant_id: str,
         task_id: str,
-        request: open_itag_20220616_models.UpdateTaskWorkforceRequest,
-    ) -> open_itag_20220616_models.UpdateTaskWorkforceResponse:
+        request: open_itag_20220616_models.UpdateTaskRequest,
+    ) -> open_itag_20220616_models.UpdateTaskResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.update_task_workforce_with_options(tenant_id, task_id, request, headers, runtime)
+        return self.update_task_with_options(tenant_id, task_id, request, headers, runtime)
 
-    async def update_task_workforce_async(
+    async def update_task_async(
         self,
         tenant_id: str,
         task_id: str,
-        request: open_itag_20220616_models.UpdateTaskWorkforceRequest,
-    ) -> open_itag_20220616_models.UpdateTaskWorkforceResponse:
+        request: open_itag_20220616_models.UpdateTaskRequest,
+    ) -> open_itag_20220616_models.UpdateTaskResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.update_task_workforce_with_options_async(tenant_id, task_id, request, headers, runtime)
+        return await self.update_task_with_options_async(tenant_id, task_id, request, headers, runtime)
 
     def update_task_workforce_with_options(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.UpdateTaskWorkforceRequest,
         headers: Dict[str, str],
@@ -2711,46 +2691,46 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.UpdateTaskWorkforceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def update_template(
+    def update_task_workforce(
         self,
         tenant_id: str,
-        template_id: str,
-        request: open_itag_20220616_models.UpdateTemplateRequest,
-    ) -> open_itag_20220616_models.UpdateTemplateResponse:
+        task_id: str,
+        request: open_itag_20220616_models.UpdateTaskWorkforceRequest,
+    ) -> open_itag_20220616_models.UpdateTaskWorkforceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.update_template_with_options(tenant_id, template_id, request, headers, runtime)
+        return self.update_task_workforce_with_options(tenant_id, task_id, request, headers, runtime)
 
-    async def update_template_async(
+    async def update_task_workforce_async(
         self,
         tenant_id: str,
-        template_id: str,
-        request: open_itag_20220616_models.UpdateTemplateRequest,
-    ) -> open_itag_20220616_models.UpdateTemplateResponse:
+        task_id: str,
+        request: open_itag_20220616_models.UpdateTaskWorkforceRequest,
+    ) -> open_itag_20220616_models.UpdateTaskWorkforceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.update_template_with_options_async(tenant_id, template_id, request, headers, runtime)
+        return await self.update_task_workforce_with_options_async(tenant_id, task_id, request, headers, runtime)
 
     def update_template_with_options(
         self,
         tenant_id: str,
         template_id: str,
         request: open_itag_20220616_models.UpdateTemplateRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.UpdateTemplateResponse:
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(TeaCore.to_map(request.body))
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='UpdateTemplate',
             version='2022-06-16',
             protocol='HTTPS',
             pathname=f'/openapi/api/v1/tenants/{OpenApiUtilClient.get_encode_param(tenant_id)}/templates/{OpenApiUtilClient.get_encode_param(template_id)}',
             method='PUT',
@@ -2771,15 +2751,15 @@
         request: open_itag_20220616_models.UpdateTemplateRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.UpdateTemplateResponse:
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            body=OpenApiUtilClient.parse_to_map(TeaCore.to_map(request.body))
+            body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='UpdateTemplate',
             version='2022-06-16',
             protocol='HTTPS',
             pathname=f'/openapi/api/v1/tenants/{OpenApiUtilClient.get_encode_param(tenant_id)}/templates/{OpenApiUtilClient.get_encode_param(template_id)}',
             method='PUT',
@@ -2789,31 +2769,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.UpdateTemplateResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def update_tenant(
+    def update_template(
         self,
         tenant_id: str,
-        request: open_itag_20220616_models.UpdateTenantRequest,
-    ) -> open_itag_20220616_models.UpdateTenantResponse:
+        template_id: str,
+        request: open_itag_20220616_models.UpdateTemplateRequest,
+    ) -> open_itag_20220616_models.UpdateTemplateResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.update_tenant_with_options(tenant_id, request, headers, runtime)
+        return self.update_template_with_options(tenant_id, template_id, request, headers, runtime)
 
-    async def update_tenant_async(
+    async def update_template_async(
         self,
         tenant_id: str,
-        request: open_itag_20220616_models.UpdateTenantRequest,
-    ) -> open_itag_20220616_models.UpdateTenantResponse:
+        template_id: str,
+        request: open_itag_20220616_models.UpdateTemplateRequest,
+    ) -> open_itag_20220616_models.UpdateTemplateResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.update_tenant_with_options_async(tenant_id, request, headers, runtime)
+        return await self.update_template_with_options_async(tenant_id, template_id, request, headers, runtime)
 
     def update_tenant_with_options(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.UpdateTenantRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -2873,33 +2855,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.UpdateTenantResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def update_user(
+    def update_tenant(
         self,
         tenant_id: str,
-        user_id: str,
-        request: open_itag_20220616_models.UpdateUserRequest,
-    ) -> open_itag_20220616_models.UpdateUserResponse:
+        request: open_itag_20220616_models.UpdateTenantRequest,
+    ) -> open_itag_20220616_models.UpdateTenantResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.update_user_with_options(tenant_id, user_id, request, headers, runtime)
+        return self.update_tenant_with_options(tenant_id, request, headers, runtime)
 
-    async def update_user_async(
+    async def update_tenant_async(
         self,
         tenant_id: str,
-        user_id: str,
-        request: open_itag_20220616_models.UpdateUserRequest,
-    ) -> open_itag_20220616_models.UpdateUserResponse:
+        request: open_itag_20220616_models.UpdateTenantRequest,
+    ) -> open_itag_20220616_models.UpdateTenantResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.update_user_with_options_async(tenant_id, user_id, request, headers, runtime)
+        return await self.update_tenant_with_options_async(tenant_id, request, headers, runtime)
 
     def update_user_with_options(
         self,
         tenant_id: str,
         user_id: str,
         request: open_itag_20220616_models.UpdateUserRequest,
         headers: Dict[str, str],
@@ -2960,7 +2940,27 @@
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.UpdateUserResponse(),
             await self.call_api_async(params, req, runtime)
         )
+
+    def update_user(
+        self,
+        tenant_id: str,
+        user_id: str,
+        request: open_itag_20220616_models.UpdateUserRequest,
+    ) -> open_itag_20220616_models.UpdateUserResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_user_with_options(tenant_id, user_id, request, headers, runtime)
+
+    async def update_user_async(
+        self,
+        tenant_id: str,
+        user_id: str,
+        request: open_itag_20220616_models.UpdateUserRequest,
+    ) -> open_itag_20220616_models.UpdateUserResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.update_user_with_options_async(tenant_id, user_id, request, headers, runtime)
```

### Comparing `alibabacloud_openitag20220616-1.0.1/alibabacloud_openitag20220616/models.py` & `alibabacloud_openitag20220616-1.0.2/alibabacloud_openitag20220616/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,40 +374,75 @@
                 temp_model = TaskTemplateOptionConfig()
                 self.template_option_map[k] = temp_model.from_map(v)
         if m.get('TemplateRelationId') is not None:
             self.template_relation_id = m.get('TemplateRelationId')
         return self
 
 
+class CreateTaskDetailVoteInfo(TeaModel):
+    def __init__(
+        self,
+        min_vote: int = None,
+        vote_num: int = None,
+    ):
+        self.min_vote = min_vote
+        self.vote_num = vote_num
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.min_vote is not None:
+            result['MinVote'] = self.min_vote
+        if self.vote_num is not None:
+            result['VoteNum'] = self.vote_num
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('MinVote') is not None:
+            self.min_vote = m.get('MinVote')
+        if m.get('VoteNum') is not None:
+            self.vote_num = m.get('VoteNum')
+        return self
+
+
 class CreateTaskDetail(TeaModel):
     def __init__(
         self,
         admins: CreateTaskDetailAdmins = None,
         allow_append_data: bool = None,
         assign_config: TaskAssginConfig = None,
         dataset_proxy_relations: List[DatasetProxyConfig] = None,
         exif: Dict[str, Any] = None,
         tags: List[str] = None,
         task_name: str = None,
         task_template_config: TaskTemplateConfig = None,
         task_workflow: List[CreateTaskDetailTaskWorkflow] = None,
         template_id: str = None,
         uuid: str = None,
+        vote_configs: Dict[str, CreateTaskDetailVoteInfo] = None,
     ):
         self.admins = admins
         self.allow_append_data = allow_append_data
         self.assign_config = assign_config
         self.dataset_proxy_relations = dataset_proxy_relations
         self.exif = exif
         self.tags = tags
         self.task_name = task_name
         self.task_template_config = task_template_config
         self.task_workflow = task_workflow
         self.template_id = template_id
         self.uuid = uuid
+        self.vote_configs = vote_configs
 
     def validate(self):
         if self.admins:
             self.admins.validate()
         if self.assign_config:
             self.assign_config.validate()
         if self.dataset_proxy_relations:
@@ -416,14 +451,18 @@
                     k.validate()
         if self.task_template_config:
             self.task_template_config.validate()
         if self.task_workflow:
             for k in self.task_workflow:
                 if k:
                     k.validate()
+        if self.vote_configs:
+            for v in self.vote_configs.values():
+                if v:
+                    v.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -449,14 +488,18 @@
         if self.task_workflow is not None:
             for k in self.task_workflow:
                 result['TaskWorkflow'].append(k.to_map() if k else None)
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
         if self.uuid is not None:
             result['UUID'] = self.uuid
+        result['VoteConfigs'] = {}
+        if self.vote_configs is not None:
+            for k, v in self.vote_configs.items():
+                result['VoteConfigs'][k] = v.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Admins') is not None:
             temp_model = CreateTaskDetailAdmins()
             self.admins = temp_model.from_map(m['Admins'])
@@ -484,14 +527,19 @@
             for k in m.get('TaskWorkflow'):
                 temp_model = CreateTaskDetailTaskWorkflow()
                 self.task_workflow.append(temp_model.from_map(k))
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
         if m.get('UUID') is not None:
             self.uuid = m.get('UUID')
+        self.vote_configs = {}
+        if m.get('VoteConfigs') is not None:
+            for k, v in m.get('VoteConfigs').items():
+                temp_model = CreateTaskDetailVoteInfo()
+                self.vote_configs[k] = temp_model.from_map(v)
         return self
 
 
 class FlowJobInfo(TeaModel):
     def __init__(
         self,
         display: bool = None,
```

### Comparing `alibabacloud_openitag20220616-1.0.1/alibabacloud_openitag20220616.egg-info/PKG-INFO` & `alibabacloud_openitag20220616-1.0.2/alibabacloud_openitag20220616.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-openitag20220616
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud OpenITag (20220616) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_openitag20220616-1.0.1/setup.py` & `alibabacloud_openitag20220616-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_openitag20220616.
 
-Created on 15/09/2022
+Created on 01/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_openitag20220616"
 NAME = "alibabacloud_openitag20220616" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud OpenITag (20220616) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

