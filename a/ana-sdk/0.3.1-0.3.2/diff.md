# Comparing `tmp/ana_sdk-0.3.1.tar.gz` & `tmp/ana_sdk-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ana_sdk-0.3.1.tar", max compression
+gzip compressed data, was "ana_sdk-0.3.2.tar", max compression
```

## Comparing `ana_sdk-0.3.1.tar` & `ana_sdk-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.3.1/ana_sdk/__init__.py
--rw-r--r--   0        0        0    14808 2023-05-26 19:18:50.065571 ana_sdk-0.3.1/ana_sdk/ana.py
--rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.3.1/ana_sdk/clients/__init__.py
--rw-r--r--   0        0        0     4523 2023-05-23 02:57:33.535000 ana_sdk-0.3.1/ana_sdk/clients/ana_data_client.py
--rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.3.1/ana_sdk/clients/base_client.py
--rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.3.1/ana_sdk/clients/dashboard_api_client.py
--rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.3.1/ana_sdk/clients/oauth_client.py
--rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.3.1/ana_sdk/clients/rpa_api_client.py
--rw-r--r--   0        0        0      744 2023-05-25 20:23:48.737805 ana_sdk-0.3.1/ana_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0     4934 2023-05-25 23:15:52.044789 ana_sdk-0.3.1/ana_sdk/result_factory.py
--rw-r--r--   0        0        0      463 2023-05-26 19:19:33.555958 ana_sdk-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.3.1/README.md
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.3.2/ana_sdk/__init__.py
+-rw-r--r--   0        0        0    14316 2023-06-01 13:25:48.030161 ana_sdk-0.3.2/ana_sdk/ana.py
+-rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.3.2/ana_sdk/clients/__init__.py
+-rw-r--r--   0        0        0     4523 2023-05-23 02:57:33.535000 ana_sdk-0.3.2/ana_sdk/clients/ana_data_client.py
+-rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.3.2/ana_sdk/clients/base_client.py
+-rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.3.2/ana_sdk/clients/dashboard_api_client.py
+-rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.3.2/ana_sdk/clients/oauth_client.py
+-rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.3.2/ana_sdk/clients/rpa_api_client.py
+-rw-r--r--   0        0        0      744 2023-05-25 20:23:48.737805 ana_sdk-0.3.2/ana_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0     4934 2023-05-25 23:15:52.044789 ana_sdk-0.3.2/ana_sdk/result_factory.py
+-rw-r--r--   0        0        0      463 2023-06-01 13:26:35.079901 ana_sdk-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.3.2/README.md
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.3.2/PKG-INFO
```

### Comparing `ana_sdk-0.3.1/ana_sdk/ana.py` & `ana_sdk-0.3.2/ana_sdk/ana.py`

 * *Files 3% similar despite different names*

```diff
@@ -306,38 +306,24 @@
             dict | None: Um dicionário contendo informações sobre a
             tarefa concluída, se a tarefa for encontrada e estiver
             concluída com sucesso ou falha. Retorna None se a tarefa
             não for encontrada.
 
         Raises:
             requests.HTTPError: Se ocorrer um erro durante a consulta
-            à API de status de tasks ou o limite de tentativas for
-            excedido.
+            à API de status de tasks.
         """
 
-        max_attempts = 10
-        not_found_count = 0
         finished = False
         task = None
 
         while not finished:
-            try:
-                task = self.rpa.get_task(task_id)
-                if task.get("status") in ("SUCCESS", "FAILURE"):
-                    finished = True
-            
-            except HTTPError as e:
-                if e.response.status_code == 404:
-                    if not_found_count < max_attempts:
-                        not_found_count += 1
-                        time.sleep(5)
-                    else:
-                        raise e
-                else:
-                    raise e
+            task = self.rpa.get_task(task_id)
+            if task.get("status") in ("SUCCESS", "FAILURE"):
+                finished = True
 
         return task
 
     def execute(
         self,
         mope: str,
         data: dict,
```

### Comparing `ana_sdk-0.3.1/ana_sdk/clients/ana_data_client.py` & `ana_sdk-0.3.2/ana_sdk/clients/ana_data_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.1/ana_sdk/clients/base_client.py` & `ana_sdk-0.3.2/ana_sdk/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.1/ana_sdk/clients/dashboard_api_client.py` & `ana_sdk-0.3.2/ana_sdk/clients/dashboard_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.1/ana_sdk/clients/oauth_client.py` & `ana_sdk-0.3.2/ana_sdk/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.1/ana_sdk/clients/rpa_api_client.py` & `ana_sdk-0.3.2/ana_sdk/clients/rpa_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.1/ana_sdk/exceptions/__init__.py` & `ana_sdk-0.3.2/ana_sdk/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.1/ana_sdk/result_factory.py` & `ana_sdk-0.3.2/ana_sdk/result_factory.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.1/README.md` & `ana_sdk-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.1/PKG-INFO` & `ana_sdk-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ana-sdk
-Version: 0.3.1
+Version: 0.3.2
 Summary: SDK que visa fornecer uma interface para interagir com os serviços ANA.
 License: MIT
 Author: Jovane Mafort
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

