# Comparing `tmp/ana_sdk-0.3.4.tar.gz` & `tmp/ana_sdk-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ana_sdk-0.3.4.tar", max compression
+gzip compressed data, was "ana_sdk-0.3.5.tar", max compression
```

## Comparing `ana_sdk-0.3.4.tar` & `ana_sdk-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.3.4/ana_sdk/__init__.py
--rw-r--r--   0        0        0    14341 2023-06-01 16:55:36.813888 ana_sdk-0.3.4/ana_sdk/ana.py
--rw-r--r--   0        0        0      138 2023-06-01 17:01:33.190199 ana_sdk-0.3.4/ana_sdk/clients/__init__.py
--rw-r--r--   0        0        0     4481 2023-06-01 16:51:10.550667 ana_sdk-0.3.4/ana_sdk/clients/ana_data_client.py
--rw-r--r--   0        0        0     1725 2023-06-01 16:58:50.036423 ana_sdk-0.3.4/ana_sdk/clients/base_client.py
--rw-r--r--   0        0        0     4634 2023-06-01 17:00:04.904107 ana_sdk-0.3.4/ana_sdk/clients/dashboard_api_client.py
--rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.3.4/ana_sdk/clients/oauth_client.py
--rw-r--r--   0        0        0     3218 2023-06-01 16:57:50.848033 ana_sdk-0.3.4/ana_sdk/clients/rpa_api_client.py
--rw-r--r--   0        0        0      744 2023-05-25 20:23:48.737805 ana_sdk-0.3.4/ana_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0      670 2023-06-01 17:03:26.358183 ana_sdk-0.3.4/ana_sdk/requests_auth.py
--rw-r--r--   0        0        0     4934 2023-05-25 23:15:52.044789 ana_sdk-0.3.4/ana_sdk/result_factory.py
--rw-r--r--   0        0        0      463 2023-06-01 17:03:47.926134 ana_sdk-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.3.4/README.md
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.3.5/ana_sdk/__init__.py
+-rw-r--r--   0        0        0    14341 2023-06-01 16:55:36.813888 ana_sdk-0.3.5/ana_sdk/ana.py
+-rw-r--r--   0        0        0      138 2023-06-01 17:01:33.190199 ana_sdk-0.3.5/ana_sdk/clients/__init__.py
+-rw-r--r--   0        0        0     4480 2023-06-01 17:05:04.633378 ana_sdk-0.3.5/ana_sdk/clients/ana_data_client.py
+-rw-r--r--   0        0        0     1725 2023-06-01 16:58:50.036423 ana_sdk-0.3.5/ana_sdk/clients/base_client.py
+-rw-r--r--   0        0        0     4634 2023-06-01 17:00:04.904107 ana_sdk-0.3.5/ana_sdk/clients/dashboard_api_client.py
+-rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.3.5/ana_sdk/clients/oauth_client.py
+-rw-r--r--   0        0        0     3218 2023-06-01 16:57:50.848033 ana_sdk-0.3.5/ana_sdk/clients/rpa_api_client.py
+-rw-r--r--   0        0        0      744 2023-05-25 20:23:48.737805 ana_sdk-0.3.5/ana_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0      670 2023-06-01 17:03:26.358183 ana_sdk-0.3.5/ana_sdk/requests_auth.py
+-rw-r--r--   0        0        0     4934 2023-05-25 23:15:52.044789 ana_sdk-0.3.5/ana_sdk/result_factory.py
+-rw-r--r--   0        0        0      463 2023-06-01 17:05:20.318515 ana_sdk-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.3.5/README.md
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.3.5/PKG-INFO
```

### Comparing `ana_sdk-0.3.4/ana_sdk/ana.py` & `ana_sdk-0.3.5/ana_sdk/ana.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.4/ana_sdk/clients/ana_data_client.py` & `ana_sdk-0.3.5/ana_sdk/clients/ana_data_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             password_ana (str): Senha para autenticação na API do ANA Data.
             oauth_token_full_url (str): URL completa do endpoint de obtenção do token.
         """
 
         self.ana_data_base_url = ana_data_base_url
         self._auth = RefreshAuth(email_ana, password_ana, oauth_token_full_url)
         self.session = requests.Session()
-        self._session.auth = self._auth
+        self.session.auth = self._auth
     
     def _get_all_content(self, url: str) -> list[dict] | dict:
         """
         Obtém todo o conteúdo paginado de uma URL.
 
         Args:
             url (str): A URL para obter o conteúdo.
```

### Comparing `ana_sdk-0.3.4/ana_sdk/clients/base_client.py` & `ana_sdk-0.3.5/ana_sdk/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.4/ana_sdk/clients/dashboard_api_client.py` & `ana_sdk-0.3.5/ana_sdk/clients/dashboard_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.4/ana_sdk/clients/oauth_client.py` & `ana_sdk-0.3.5/ana_sdk/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.4/ana_sdk/clients/rpa_api_client.py` & `ana_sdk-0.3.5/ana_sdk/clients/rpa_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.4/ana_sdk/exceptions/__init__.py` & `ana_sdk-0.3.5/ana_sdk/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.4/ana_sdk/requests_auth.py` & `ana_sdk-0.3.5/ana_sdk/requests_auth.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.4/ana_sdk/result_factory.py` & `ana_sdk-0.3.5/ana_sdk/result_factory.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.4/README.md` & `ana_sdk-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.3.4/PKG-INFO` & `ana_sdk-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ana-sdk
-Version: 0.3.4
+Version: 0.3.5
 Summary: SDK que visa fornecer uma interface para interagir com os serviços ANA.
 License: MIT
 Author: Jovane Mafort
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

