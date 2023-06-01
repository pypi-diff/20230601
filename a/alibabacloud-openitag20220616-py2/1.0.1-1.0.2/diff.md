# Comparing `tmp/alibabacloud_openitag20220616_py2-1.0.1.tar.gz` & `tmp/alibabacloud_openitag20220616_py2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_openitag20220616_py2-1.0.1.tar", last modified: Thu Sep 15 07:28:00 2022, max compression
+gzip compressed data, was "dist/alibabacloud_openitag20220616_py2-1.0.2.tar", last modified: Thu Jun  1 07:15:27 2023, max compression
```

## Comparing `alibabacloud_openitag20220616_py2-1.0.1.tar` & `alibabacloud_openitag20220616_py2-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       35 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/alibabacloud_openitag20220616/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/alibabacloud_openitag20220616/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46430 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/alibabacloud_openitag20220616/client.py
--rw-r--r--   0 root         (0) root         (0)   267650 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/alibabacloud_openitag20220616/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/alibabacloud_openitag20220616_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/alibabacloud_openitag20220616_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/alibabacloud_openitag20220616_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/alibabacloud_openitag20220616_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/alibabacloud_openitag20220616_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/alibabacloud_openitag20220616_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2022-09-15 07:28:00.000000 alibabacloud_openitag20220616_py2-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:15:27.000000 alibabacloud_openitag20220616_py2-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-01 07:15:26.000000 alibabacloud_openitag20220616_py2-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-01 07:15:26.000000 alibabacloud_openitag20220616_py2-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-01 07:15:26.000000 alibabacloud_openitag20220616_py2-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-06-01 07:15:27.000000 alibabacloud_openitag20220616_py2-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-06-01 07:15:26.000000 alibabacloud_openitag20220616_py2-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-01 07:15:26.000000 alibabacloud_openitag20220616_py2-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:15:27.000000 alibabacloud_openitag20220616_py2-1.0.2/alibabacloud_openitag20220616/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-01 07:15:26.000000 alibabacloud_openitag20220616_py2-1.0.2/alibabacloud_openitag20220616/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46366 2023-06-01 07:15:26.000000 alibabacloud_openitag20220616_py2-1.0.2/alibabacloud_openitag20220616/client.py
+-rw-r--r--   0 root         (0) root         (0)   269151 2023-06-01 07:15:26.000000 alibabacloud_openitag20220616_py2-1.0.2/alibabacloud_openitag20220616/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:15:27.000000 alibabacloud_openitag20220616_py2-1.0.2/alibabacloud_openitag20220616_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-06-01 07:15:27.000000 alibabacloud_openitag20220616_py2-1.0.2/alibabacloud_openitag20220616_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-01 07:15:27.000000 alibabacloud_openitag20220616_py2-1.0.2/alibabacloud_openitag20220616_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 07:15:27.000000 alibabacloud_openitag20220616_py2-1.0.2/alibabacloud_openitag20220616_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-01 07:15:27.000000 alibabacloud_openitag20220616_py2-1.0.2/alibabacloud_openitag20220616_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-01 07:15:27.000000 alibabacloud_openitag20220616_py2-1.0.2/alibabacloud_openitag20220616_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-01 07:15:27.000000 alibabacloud_openitag20220616_py2-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-06-01 07:15:26.000000 alibabacloud_openitag20220616_py2-1.0.2/setup.py
```

### Comparing `alibabacloud_openitag20220616_py2-1.0.1/LICENSE` & `alibabacloud_openitag20220616_py2-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_openitag20220616_py2-1.0.1/PKG-INFO` & `alibabacloud_openitag20220616_py2-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_openitag20220616_py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud OpenITag (20220616) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_openitag20220616_py2-1.0.1/README-CN.md` & `alibabacloud_openitag20220616_py2-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_openitag20220616_py2-1.0.1/README.md` & `alibabacloud_openitag20220616_py2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_openitag20220616_py2-1.0.1/alibabacloud_openitag20220616/client.py` & `alibabacloud_openitag20220616_py2-1.0.2/alibabacloud_openitag20220616/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,19 +27,14 @@
     def get_endpoint(self, product_id, region_id, endpoint_rule, network, suffix, endpoint_map, endpoint):
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
-    def add_work_node_workforce(self, tenant_id, task_id, work_node_id, request):
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.add_work_node_workforce_with_options(tenant_id, task_id, work_node_id, request, headers, runtime)
-
     def add_work_node_workforce_with_options(self, tenant_id, task_id, work_node_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.user_ids):
             body['UserIds'] = request.user_ids
         req = open_api_models.OpenApiRequest(
             headers=headers,
@@ -57,24 +52,24 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.AddWorkNodeWorkforceResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def create_task(self, tenant_id, request):
+    def add_work_node_workforce(self, tenant_id, task_id, work_node_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.create_task_with_options(tenant_id, request, headers, runtime)
+        return self.add_work_node_workforce_with_options(tenant_id, task_id, work_node_id, request, headers, runtime)
 
     def create_task_with_options(self, tenant_id, request, headers, runtime):
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
             pathname='/openapi/api/v1/tenants/%s/tasks' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(tenant_id)),
             method='POST',
@@ -84,24 +79,24 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.CreateTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def create_template(self, tenant_id, request):
+    def create_task(self, tenant_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.create_template_with_options(tenant_id, request, headers, runtime)
+        return self.create_task_with_options(tenant_id, request, headers, runtime)
 
     def create_template_with_options(self, tenant_id, request, headers, runtime):
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
             pathname='/openapi/api/v1/tenants/%s/templates' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(tenant_id)),
             method='POST',
@@ -111,18 +106,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.CreateTemplateResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def create_user(self, tenant_id, request):
+    def create_template(self, tenant_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.create_user_with_options(tenant_id, request, headers, runtime)
+        return self.create_template_with_options(tenant_id, request, headers, runtime)
 
     def create_user_with_options(self, tenant_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.account_no):
             body['AccountNo'] = request.account_no
         if not UtilClient.is_unset(request.account_type):
@@ -147,18 +142,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.CreateUserResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def delete_task(self, tenant_id, task_id):
+    def create_user(self, tenant_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.delete_task_with_options(tenant_id, task_id, headers, runtime)
+        return self.create_user_with_options(tenant_id, request, headers, runtime)
 
     def delete_task_with_options(self, tenant_id, task_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteTask',
@@ -172,18 +167,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.DeleteTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def delete_template(self, tenant_id, template_id):
+    def delete_task(self, tenant_id, task_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.delete_template_with_options(tenant_id, template_id, headers, runtime)
+        return self.delete_task_with_options(tenant_id, task_id, headers, runtime)
 
     def delete_template_with_options(self, tenant_id, template_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteTemplate',
@@ -197,18 +192,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.DeleteTemplateResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def delete_user(self, tenant_id, user_id):
+    def delete_template(self, tenant_id, template_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.delete_user_with_options(tenant_id, user_id, headers, runtime)
+        return self.delete_template_with_options(tenant_id, template_id, headers, runtime)
 
     def delete_user_with_options(self, tenant_id, user_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteUser',
@@ -222,18 +217,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.DeleteUserResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def export_annotations(self, tenant_id, task_id, request):
+    def delete_user(self, tenant_id, user_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.export_annotations_with_options(tenant_id, task_id, request, headers, runtime)
+        return self.delete_user_with_options(tenant_id, user_id, headers, runtime)
 
     def export_annotations_with_options(self, tenant_id, task_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.oss_path):
             query['OssPath'] = request.oss_path
         if not UtilClient.is_unset(request.register_dataset):
@@ -256,18 +251,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ExportAnnotationsResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_job(self, tenant_id, job_id, request):
+    def export_annotations(self, tenant_id, task_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_job_with_options(tenant_id, job_id, request, headers, runtime)
+        return self.export_annotations_with_options(tenant_id, task_id, request, headers, runtime)
 
     def get_job_with_options(self, tenant_id, job_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.job_type):
             query['JobType'] = request.job_type
         req = open_api_models.OpenApiRequest(
@@ -286,18 +281,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetJobResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_subtask(self, tenant_id, task_id, subtask_id):
+    def get_job(self, tenant_id, job_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_subtask_with_options(tenant_id, task_id, subtask_id, headers, runtime)
+        return self.get_job_with_options(tenant_id, job_id, request, headers, runtime)
 
     def get_subtask_with_options(self, tenant_id, task_id, subtask_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetSubtask',
@@ -311,18 +306,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetSubtaskResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_subtask_item(self, tenant_id, task_id, subtask_id, item_id):
+    def get_subtask(self, tenant_id, task_id, subtask_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_subtask_item_with_options(tenant_id, task_id, subtask_id, item_id, headers, runtime)
+        return self.get_subtask_with_options(tenant_id, task_id, subtask_id, headers, runtime)
 
     def get_subtask_item_with_options(self, tenant_id, task_id, subtask_id, item_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetSubtaskItem',
@@ -336,18 +331,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetSubtaskItemResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_task(self, tenant_id, task_id):
+    def get_subtask_item(self, tenant_id, task_id, subtask_id, item_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_with_options(tenant_id, task_id, headers, runtime)
+        return self.get_subtask_item_with_options(tenant_id, task_id, subtask_id, item_id, headers, runtime)
 
     def get_task_with_options(self, tenant_id, task_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTask',
@@ -361,18 +356,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_task_statistics(self, tenant_id, task_id, request):
+    def get_task(self, tenant_id, task_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_statistics_with_options(tenant_id, task_id, request, headers, runtime)
+        return self.get_task_with_options(tenant_id, task_id, headers, runtime)
 
     def get_task_statistics_with_options(self, tenant_id, task_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.stat_type):
             query['StatType'] = request.stat_type
         req = open_api_models.OpenApiRequest(
@@ -391,18 +386,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskStatisticsResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_task_status(self, tenant_id, task_id):
+    def get_task_statistics(self, tenant_id, task_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_status_with_options(tenant_id, task_id, headers, runtime)
+        return self.get_task_statistics_with_options(tenant_id, task_id, request, headers, runtime)
 
     def get_task_status_with_options(self, tenant_id, task_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskStatus',
@@ -416,18 +411,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskStatusResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_task_template(self, tenant_id, task_id):
+    def get_task_status(self, tenant_id, task_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_template_with_options(tenant_id, task_id, headers, runtime)
+        return self.get_task_status_with_options(tenant_id, task_id, headers, runtime)
 
     def get_task_template_with_options(self, tenant_id, task_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskTemplate',
@@ -441,18 +436,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskTemplateResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_task_template_questions(self, tenant_id, task_id):
+    def get_task_template(self, tenant_id, task_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_template_questions_with_options(tenant_id, task_id, headers, runtime)
+        return self.get_task_template_with_options(tenant_id, task_id, headers, runtime)
 
     def get_task_template_questions_with_options(self, tenant_id, task_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskTemplateQuestions',
@@ -466,18 +461,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskTemplateQuestionsResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_task_template_views(self, tenant_id, task_id):
+    def get_task_template_questions(self, tenant_id, task_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_template_views_with_options(tenant_id, task_id, headers, runtime)
+        return self.get_task_template_questions_with_options(tenant_id, task_id, headers, runtime)
 
     def get_task_template_views_with_options(self, tenant_id, task_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskTemplateViews',
@@ -491,18 +486,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskTemplateViewsResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_task_workforce(self, tenant_id, task_id):
+    def get_task_template_views(self, tenant_id, task_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_workforce_with_options(tenant_id, task_id, headers, runtime)
+        return self.get_task_template_views_with_options(tenant_id, task_id, headers, runtime)
 
     def get_task_workforce_with_options(self, tenant_id, task_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskWorkforce',
@@ -516,18 +511,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskWorkforceResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_task_workforce_statistic(self, tenant_id, task_id, request):
+    def get_task_workforce(self, tenant_id, task_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_task_workforce_statistic_with_options(tenant_id, task_id, request, headers, runtime)
+        return self.get_task_workforce_with_options(tenant_id, task_id, headers, runtime)
 
     def get_task_workforce_statistic_with_options(self, tenant_id, task_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -550,18 +545,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTaskWorkforceStatisticResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_template(self, tenant_id, template_id):
+    def get_task_workforce_statistic(self, tenant_id, task_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_template_with_options(tenant_id, template_id, headers, runtime)
+        return self.get_task_workforce_statistic_with_options(tenant_id, task_id, request, headers, runtime)
 
     def get_template_with_options(self, tenant_id, template_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTemplate',
@@ -575,18 +570,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTemplateResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_template_questions(self, tenant_id, template_id):
+    def get_template(self, tenant_id, template_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_template_questions_with_options(tenant_id, template_id, headers, runtime)
+        return self.get_template_with_options(tenant_id, template_id, headers, runtime)
 
     def get_template_questions_with_options(self, tenant_id, template_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTemplateQuestions',
@@ -600,18 +595,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTemplateQuestionsResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_template_view(self, tenant_id, template_id):
+    def get_template_questions(self, tenant_id, template_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_template_view_with_options(tenant_id, template_id, headers, runtime)
+        return self.get_template_questions_with_options(tenant_id, template_id, headers, runtime)
 
     def get_template_view_with_options(self, tenant_id, template_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTemplateView',
@@ -625,18 +620,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTemplateViewResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_tenant(self, tenant_id):
+    def get_template_view(self, tenant_id, template_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_tenant_with_options(tenant_id, headers, runtime)
+        return self.get_template_view_with_options(tenant_id, template_id, headers, runtime)
 
     def get_tenant_with_options(self, tenant_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTenant',
@@ -650,18 +645,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetTenantResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_user(self, tenant_id, user_id):
+    def get_tenant(self, tenant_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_user_with_options(tenant_id, user_id, headers, runtime)
+        return self.get_tenant_with_options(tenant_id, headers, runtime)
 
     def get_user_with_options(self, tenant_id, user_id, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetUser',
@@ -675,18 +670,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.GetUserResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def list_jobs(self, tenant_id, request):
+    def get_user(self, tenant_id, user_id):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_jobs_with_options(tenant_id, request, headers, runtime)
+        return self.get_user_with_options(tenant_id, user_id, headers, runtime)
 
     def list_jobs_with_options(self, tenant_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.job_type):
             query['JobType'] = request.job_type
         if not UtilClient.is_unset(request.page_number):
@@ -709,18 +704,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ListJobsResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def list_subtask_items(self, tenant_id, task_id, subtask_id, request):
+    def list_jobs(self, tenant_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_subtask_items_with_options(tenant_id, task_id, subtask_id, request, headers, runtime)
+        return self.list_jobs_with_options(tenant_id, request, headers, runtime)
 
     def list_subtask_items_with_options(self, tenant_id, task_id, subtask_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -741,18 +736,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ListSubtaskItemsResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def list_subtasks(self, tenant_id, task_id, request):
+    def list_subtask_items(self, tenant_id, task_id, subtask_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_subtasks_with_options(tenant_id, task_id, request, headers, runtime)
+        return self.list_subtask_items_with_options(tenant_id, task_id, subtask_id, request, headers, runtime)
 
     def list_subtasks_with_options(self, tenant_id, task_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -773,18 +768,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ListSubtasksResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def list_tasks(self, tenant_id, request):
+    def list_subtasks(self, tenant_id, task_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_tasks_with_options(tenant_id, request, headers, runtime)
+        return self.list_subtasks_with_options(tenant_id, task_id, request, headers, runtime)
 
     def list_tasks_with_options(self, tenant_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -805,18 +800,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ListTasksResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def list_templates(self, tenant_id, request):
+    def list_tasks(self, tenant_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_templates_with_options(tenant_id, request, headers, runtime)
+        return self.list_tasks_with_options(tenant_id, request, headers, runtime)
 
     def list_templates_with_options(self, tenant_id, tmp_req, headers, runtime):
         UtilClient.validate_model(tmp_req)
         request = open_itag_20220616_models.ListTemplatesShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.types):
             request.types_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.types, 'Types', 'simple')
@@ -845,18 +840,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ListTemplatesResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def list_tenants(self, request):
+    def list_templates(self, tenant_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_tenants_with_options(request, headers, runtime)
+        return self.list_templates_with_options(tenant_id, request, headers, runtime)
 
     def list_tenants_with_options(self, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -877,18 +872,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ListTenantsResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def list_users(self, tenant_id, request):
+    def list_tenants(self, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_users_with_options(tenant_id, request, headers, runtime)
+        return self.list_tenants_with_options(request, headers, runtime)
 
     def list_users_with_options(self, tenant_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -909,18 +904,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.ListUsersResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def remove_work_node_workforce(self, tenant_id, task_id, work_node_id, request):
+    def list_users(self, tenant_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.remove_work_node_workforce_with_options(tenant_id, task_id, work_node_id, request, headers, runtime)
+        return self.list_users_with_options(tenant_id, request, headers, runtime)
 
     def remove_work_node_workforce_with_options(self, tenant_id, task_id, work_node_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.user_ids):
             body['UserIds'] = request.user_ids
         req = open_api_models.OpenApiRequest(
@@ -939,24 +934,24 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.RemoveWorkNodeWorkforceResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def update_task(self, tenant_id, task_id, request):
+    def remove_work_node_workforce(self, tenant_id, task_id, work_node_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.update_task_with_options(tenant_id, task_id, request, headers, runtime)
+        return self.remove_work_node_workforce_with_options(tenant_id, task_id, work_node_id, request, headers, runtime)
 
     def update_task_with_options(self, tenant_id, task_id, request, headers, runtime):
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
             pathname='/openapi/api/v1/tenants/%s/tasks/%s' % (TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(tenant_id)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(task_id))),
             method='PUT',
@@ -966,18 +961,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.UpdateTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def update_task_workforce(self, tenant_id, task_id, request):
+    def update_task(self, tenant_id, task_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.update_task_workforce_with_options(tenant_id, task_id, request, headers, runtime)
+        return self.update_task_with_options(tenant_id, task_id, request, headers, runtime)
 
     def update_task_workforce_with_options(self, tenant_id, task_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.workforce):
             body['Workforce'] = request.workforce
         req = open_api_models.OpenApiRequest(
@@ -996,24 +991,24 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.UpdateTaskWorkforceResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def update_template(self, tenant_id, template_id, request):
+    def update_task_workforce(self, tenant_id, task_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.update_template_with_options(tenant_id, template_id, request, headers, runtime)
+        return self.update_task_workforce_with_options(tenant_id, task_id, request, headers, runtime)
 
     def update_template_with_options(self, tenant_id, template_id, request, headers, runtime):
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
             pathname='/openapi/api/v1/tenants/%s/templates/%s' % (TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(tenant_id)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(template_id))),
             method='PUT',
@@ -1023,18 +1018,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.UpdateTemplateResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def update_tenant(self, tenant_id, request):
+    def update_template(self, tenant_id, template_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.update_tenant_with_options(tenant_id, request, headers, runtime)
+        return self.update_template_with_options(tenant_id, template_id, request, headers, runtime)
 
     def update_tenant_with_options(self, tenant_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.tenant_name):
@@ -1055,18 +1050,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.UpdateTenantResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def update_user(self, tenant_id, user_id, request):
+    def update_tenant(self, tenant_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.update_user_with_options(tenant_id, user_id, request, headers, runtime)
+        return self.update_tenant_with_options(tenant_id, request, headers, runtime)
 
     def update_user_with_options(self, tenant_id, user_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.role):
             body['Role'] = request.role
         if not UtilClient.is_unset(request.user_name):
@@ -1086,7 +1081,12 @@
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             open_itag_20220616_models.UpdateUserResponse(),
             self.call_api(params, req, runtime)
         )
+
+    def update_user(self, tenant_id, user_id, request):
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_user_with_options(tenant_id, user_id, request, headers, runtime)
```

### Comparing `alibabacloud_openitag20220616_py2-1.0.1/alibabacloud_openitag20220616/models.py` & `alibabacloud_openitag20220616_py2-1.0.2/alibabacloud_openitag20220616/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,26 +58,27 @@
             self.node_name = m.get('NodeName')
         return self
 
 
 class CreateTaskDetail(TeaModel):
     def __init__(self, admins=None, allow_append_data=None, assign_config=None, dataset_proxy_relations=None,
                  exif=None, tags=None, task_name=None, task_template_config=None, task_workflow=None, template_id=None,
-                 uuid=None):
+                 uuid=None, vote_configs=None):
         self.admins = admins  # type: CreateTaskDetailAdmins
         self.allow_append_data = allow_append_data  # type: bool
         self.assign_config = assign_config  # type: TaskAssginConfig
         self.dataset_proxy_relations = dataset_proxy_relations  # type: list[DatasetProxyConfig]
         self.exif = exif  # type: dict[str, any]
         self.tags = tags  # type: list[str]
         self.task_name = task_name  # type: str
         self.task_template_config = task_template_config  # type: TaskTemplateConfig
         self.task_workflow = task_workflow  # type: list[CreateTaskDetailTaskWorkflow]
         self.template_id = template_id  # type: str
         self.uuid = uuid  # type: str
+        self.vote_configs = vote_configs  # type: dict[str, CreateTaskDetailVoteInfo]
 
     def validate(self):
         if self.admins:
             self.admins.validate()
         if self.assign_config:
             self.assign_config.validate()
         if self.dataset_proxy_relations:
@@ -86,14 +87,18 @@
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
         _map = super(CreateTaskDetail, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -119,14 +124,18 @@
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Admins') is not None:
             temp_model = CreateTaskDetailAdmins()
             self.admins = temp_model.from_map(m['Admins'])
@@ -154,14 +163,48 @@
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
+        return self
+
+
+class CreateTaskDetailVoteInfo(TeaModel):
+    def __init__(self, min_vote=None, vote_num=None):
+        self.min_vote = min_vote  # type: long
+        self.vote_num = vote_num  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateTaskDetailVoteInfo, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('MinVote') is not None:
+            self.min_vote = m.get('MinVote')
+        if m.get('VoteNum') is not None:
+            self.vote_num = m.get('VoteNum')
         return self
 
 
 class DatasetProxyConfig(TeaModel):
     def __init__(self, dataset_type=None, source=None, source_dataset_id=None):
         self.dataset_type = dataset_type  # type: str
         self.source = source  # type: str
```

### Comparing `alibabacloud_openitag20220616_py2-1.0.1/alibabacloud_openitag20220616_py2.egg-info/PKG-INFO` & `alibabacloud_openitag20220616_py2-1.0.2/alibabacloud_openitag20220616_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-openitag20220616-py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud OpenITag (20220616) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_openitag20220616_py2-1.0.1/setup.py` & `alibabacloud_openitag20220616_py2-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_openitag20220616_py2.
 
-Created on 15/09/2022
+Created on 01/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_openitag20220616"
 NAME = "alibabacloud_openitag20220616_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud OpenITag (20220616) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.6, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.3, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

