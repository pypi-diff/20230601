# Comparing `tmp/dcentrapi-0.2.3.tar.gz` & `tmp/dcentrapi-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.2.3.tar", last modified: Wed May 31 13:36:43 2023, max compression
+gzip compressed data, was "dist/dcentrapi-0.2.4.tar", last modified: Thu Jun  1 15:26:29 2023, max compression
```

## Comparing `dcentrapi-0.2.3.tar` & `dcentrapi-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-31 13:36:43.440873 dcentrapi-0.2.3/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.2.3/LICENSE.rst
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-05-31 13:36:43.440712 dcentrapi-0.2.3/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.2.3/README.md
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-31 13:36:43.439937 dcentrapi-0.2.3/dcentrapi/
--rw-r--r--   0 nivshitrit   (501) staff       (20)      829 2023-05-24 09:45:16.000000 dcentrapi-0.2.3/dcentrapi/Base.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      280 2023-03-08 10:39:09.000000 dcentrapi-0.2.3/dcentrapi/__init__.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)       63 2023-05-31 13:36:41.000000 dcentrapi-0.2.3/dcentrapi/common.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     7885 2023-05-24 09:45:16.000000 dcentrapi-0.2.3/dcentrapi/eventPolling.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      491 2023-03-02 14:02:13.000000 dcentrapi-0.2.3/dcentrapi/gasMonitor.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.2.3/dcentrapi/merkleTree.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3850 2023-05-31 13:35:59.000000 dcentrapi-0.2.3/dcentrapi/rpcAggregation.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      804 2023-05-31 13:35:59.000000 dcentrapi-0.2.3/dcentrapi/web3Index.py
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-31 13:36:43.440544 dcentrapi-0.2.3/dcentrapi.egg-info/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-05-31 13:36:43.000000 dcentrapi-0.2.3/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)      379 2023-05-31 13:36:43.000000 dcentrapi-0.2.3/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-05-31 13:36:43.000000 dcentrapi-0.2.3/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-05-31 13:36:43.000000 dcentrapi-0.2.3/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-05-31 13:36:43.000000 dcentrapi-0.2.3/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-05-31 13:36:43.440983 dcentrapi-0.2.3/setup.cfg
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1167 2023-04-09 07:57:53.000000 dcentrapi-0.2.3/setup.py
+drwxr-xr-x   0 jovanvuleta   (501) staff       (20)        0 2023-06-01 15:26:29.671601 dcentrapi-0.2.4/
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     1073 2022-06-21 11:33:40.000000 dcentrapi-0.2.4/LICENSE.rst
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     6741 2023-06-01 15:26:29.671413 dcentrapi-0.2.4/PKG-INFO
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     6211 2022-09-26 09:54:00.000000 dcentrapi-0.2.4/README.md
+drwxr-xr-x   0 jovanvuleta   (501) staff       (20)        0 2023-06-01 15:26:29.670482 dcentrapi-0.2.4/dcentrapi/
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)      829 2023-05-09 15:11:33.000000 dcentrapi-0.2.4/dcentrapi/Base.py
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)      280 2023-05-09 13:35:14.000000 dcentrapi-0.2.4/dcentrapi/__init__.py
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)       63 2023-06-01 15:06:39.000000 dcentrapi-0.2.4/dcentrapi/common.py
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     8714 2023-06-01 15:10:16.000000 dcentrapi-0.2.4/dcentrapi/eventPolling.py
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)      491 2023-05-09 13:35:14.000000 dcentrapi-0.2.4/dcentrapi/gasMonitor.py
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     3078 2023-05-09 13:35:14.000000 dcentrapi-0.2.4/dcentrapi/merkleTree.py
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     3850 2023-06-01 14:51:58.000000 dcentrapi-0.2.4/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)      804 2023-06-01 14:51:58.000000 dcentrapi-0.2.4/dcentrapi/web3Index.py
+drwxr-xr-x   0 jovanvuleta   (501) staff       (20)        0 2023-06-01 15:26:29.671183 dcentrapi-0.2.4/dcentrapi.egg-info/
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     6741 2023-06-01 15:26:29.000000 dcentrapi-0.2.4/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)      379 2023-06-01 15:26:29.000000 dcentrapi-0.2.4/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)        1 2023-06-01 15:26:29.000000 dcentrapi-0.2.4/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)        9 2023-06-01 15:26:29.000000 dcentrapi-0.2.4/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)       10 2023-06-01 15:26:29.000000 dcentrapi-0.2.4/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)       38 2023-06-01 15:26:29.671656 dcentrapi-0.2.4/setup.cfg
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     1167 2023-05-09 13:35:14.000000 dcentrapi-0.2.4/setup.py
```

### Comparing `dcentrapi-0.2.3/LICENSE.rst` & `dcentrapi-0.2.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.3/PKG-INFO` & `dcentrapi-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.3
+Version: 0.2.4
 Summary: Dcentralab Pypi packages
-Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -105,9 +103,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

### Comparing `dcentrapi-0.2.3/README.md` & `dcentrapi-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.3/dcentrapi/Base.py` & `dcentrapi-0.2.4/dcentrapi/Base.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.3/dcentrapi/eventPolling.py` & `dcentrapi-0.2.4/dcentrapi/eventPolling.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,175 +1,212 @@
+from typing import Union, List, Dict
+
 import requests
 
 from dcentrapi.Base import Base
 
 
 class EventPolling(Base):
-    def get_collection(self, collection_name):
+    def get_collection(self, collection_name: str):
         url = self.url + "event_polling/collection"
         data = {"collection_name": collection_name}
         response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
-    def get_latest_contract_version(self, contract_name):
-        url = self.url + "event_polling/get_latest_contract_version"  # test comment for deployment trigger
+    def get_latest_contract_version(self, contract_name: str):
+        url = self.url + "event_polling/get_latest_contract_version"
         data = {"contract_name": contract_name}
         response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
     def register_user(self, user_name: str, collection_name: str):
         url = self.url + "event_polling/register_user"
         data = {
             "user_name": user_name,
             "collection_name": collection_name,
         }
         response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
     def subscribe_contract(
-        self, contract_name, contract_address, network, abi, collection_name, contract_version=None, git_tag=None
+        self,
+        contract_name: str,
+        contract_address: str,
+        network: str,
+        abi: Union[str, List[Dict[str, str]]],
+        collection_name: str,
+        contract_version: str,
+        git_tag: str = None,
+        webhook_url: str = None,
     ):
         url = self.url + "event_polling/subscribe_contract"
         data = {
             "contract_name": contract_name,
             "contract_address": contract_address,
             "contract_version": contract_version,
             "network": network,
             "collection_name": collection_name,
             "abi": abi,
             "git_tag": git_tag,
+            "webhook_url": webhook_url,
         }
         response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
-    def get_schema(self, contract_name, contract_version):
+    def get_schema(self, contract_name: str, contract_version: str):
         url = self.url + "event_polling/schema"
         data = {"contract_name": contract_name, "contract_version": contract_version}
         response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
     def get_events_sum_of_values_in_range(
-        self, collection_name, contract_address, event_name, field_name, start_time, end_time
+        self,
+        collection_name: str,
+        contract_address: str,
+        event_name: str,
+        field_name: str,
+        start_time: str,
+        end_time: str,
     ):
         url = self.url + "event_polling/events_sum_of_values_in_range"
         data = {
             "collection_name": collection_name,
             "contract_address": contract_address,
             "event_name": event_name,
             "field_name": field_name,
             "start_time": start_time,
             "end_time": end_time,
         }
-        response = requests.get(url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
-    def get_collection_sum_of_values_in_range(self, collection_name, event_name, field_name, start_time, end_time):
+    def get_collection_sum_of_values_in_range(
+        self, collection_name: str, event_name: str, field_name: str, start_time: str, end_time: str
+    ):
         url = self.url + "event_polling/collection_sum_of_values_in_range"
         data = {
             "collection_name": collection_name,
             "event_name": event_name,
             "field_name": field_name,
             "start_time": start_time,
             "end_time": end_time,
         }
-        response = requests.get(url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
-    def get_collection_contracts_sum_of_values(self, collection_name, event_name, field_name, start_time, end_time):
+    def get_collection_contracts_sum_of_values(
+        self, collection_name: str, event_name: str, field_name: str, start_time: str, end_time: str
+    ):
         url = self.url + "event_polling/collection_contracts_sum_of_values"
         data = {
             "collection_name": collection_name,
             "event_name": event_name,
             "field_name": field_name,
             "start_time": start_time,
             "end_time": end_time,
         }
-        response = requests.get(url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
-    def get_collection_daily_nof_transactions(self, collection_name, start_time, end_time):
+    def get_collection_daily_nof_transactions(self, collection_name: str, start_time: str, end_time: str):
         url = self.url + "event_polling/collection_daily_nof_transactions"
         data = {"collection_name": collection_name, "start_time": start_time, "end_time": end_time}
-        response = requests.get(url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
-    def get_collection_nof_transactions(self, collection_name):
+    def get_collection_nof_transactions(self, collection_name: str):
         url = self.url + "event_polling/collection_nof_transactions"
         data = {"collection_name": collection_name}
-        response = requests.get(url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
     def get_collection_nof_transactions_by_time(self, collection_name, start_time, end_time):
         url = self.url + "event_polling/collection_nof_transactions_by_time"
         data = {"collection_name": collection_name, "start_time": start_time, "end_time": end_time}
         response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
-    def get_collection_nof_users_in_time_range(self, collection_name, start_time, end_time):
+    def get_collection_nof_users_in_time_range(self, collection_name: str, start_time: str, end_time: str):
         url = self.url + "event_polling/collection_nof_users_in_time_range"
         data = {"collection_name": collection_name, "start_time": start_time, "end_time": end_time}
         response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
-    def get_contract_nof_transactions(self, collection_name, contract_address):
+    def get_contract_nof_transactions(self, collection_name: str, contract_address: str):
         url = self.url + "event_polling/contract_nof_transactions"
         data = {"collection_name": collection_name, "contract_address": contract_address}
-        response = requests.get(url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
-    def get_collection_users_in_time_range(self, collection_name, start_time, end_time):
+    def get_collection_users_in_time_range(self, collection_name: str, start_time: str, end_time: str):
         url = self.url + "event_polling/collection_users_in_time_range"
         data = {"collection_name": collection_name, "start_time": start_time, "end_time": end_time}
-        response = requests.get(url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
-    def get_contract_users_in_time_range(self, collection_name, contract_address, start_time, end_time):
+    def get_contract_users_in_time_range(
+        self, collection_name: str, contract_address: str, start_time: str, end_time: str
+    ):
         url = self.url + "event_polling/contract_users_in_time_range"
         data = {
             "collection_name": collection_name,
             "contract_address": contract_address,
             "start_time": start_time,
             "end_time": end_time,
         }
-        response = requests.get(url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
     def get_contracts_events_info(
-        self, collection_name, contract_addresses, event_names, user_web3_addresses=None, start_time=None, end_time=None
+        self,
+        collection_name: str,
+        contract_addresses: [str],
+        event_names: [str],
+        user_web3_addresses=None,
+        start_time=None,
+        end_time=None,
+        incentive_id: str = None,
+        user_address: str = None,
+        sort: str = None,
     ):
         url = self.url + "event_polling/contracts_events_info"
         data = {
             "collection_name": collection_name,
             "contract_addresses": contract_addresses,
             "start_time": start_time,
             "end_time": end_time,
             "user_web3_addresses": user_web3_addresses,
             "event_names": event_names,
+            "incentive_id": incentive_id,
+            "user_address": user_address,
+            "sort": sort,
         }
-        response = requests.get(url, params=data, headers=self.headers)
+        response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
-    def get_nof_contracts_events_unique_transactions(self, collection_name, contract_addresses, event_names):
+    def get_nof_contracts_events_unique_transactions(
+        self, collection_name: str, contract_addresses: str, event_names: str
+    ):
         url = self.url + "event_polling/contracts_events_info"
         data = {
             "collection_name": collection_name,
             "contract_addresses": contract_addresses,
             "event_names": event_names,
         }
-        response = requests.get(url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
-    def get_nof_token_transfers(self, contract_addresses):
+    def get_nof_token_transfers(self, contract_addresses: [str]):
         url = self.url + "event_polling/token_transfers"
         data = {"contract_addresses": contract_addresses}
-        response = requests.get(url, params=data, headers=self.headers)
+        response = requests.get(url=url, params=data, headers=self.headers)
         return response.json()
 
-    def get_event_details(self, collection_name, list_of_events, event_parameter):
+    def get_event_details(self, collection_name: str, list_of_events: [str], event_parameter: str):
         url = self.url + "event_polling/get_event_details"
         data = {
             "collection_name": collection_name,
             "list_of_events": list_of_events,
             "event_parameter": event_parameter,
         }
-        response = requests.post(url, json=data, headers=self.headers)
+        response = requests.post(url=url, json=data, headers=self.headers)
         return response.json()
```

### Comparing `dcentrapi-0.2.3/dcentrapi/merkleTree.py` & `dcentrapi-0.2.4/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.3/dcentrapi/rpcAggregation.py` & `dcentrapi-0.2.4/dcentrapi/rpcAggregation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.3/dcentrapi/web3Index.py` & `dcentrapi-0.2.4/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.3/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.2.4/dcentrapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.3
+Version: 0.2.4
 Summary: Dcentralab Pypi packages
-Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -105,9 +103,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

### Comparing `dcentrapi-0.2.3/setup.py` & `dcentrapi-0.2.4/setup.py`

 * *Files identical despite different names*

