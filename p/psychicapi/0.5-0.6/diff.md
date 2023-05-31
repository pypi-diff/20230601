# Comparing `tmp/psychicapi-0.5.tar.gz` & `tmp/psychicapi-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychicapi-0.5.tar", last modified: Sun May 28 22:18:37 2023, max compression
+gzip compressed data, was "psychicapi-0.6.tar", last modified: Wed May 31 22:25:16 2023, max compression
```

## Comparing `psychicapi-0.5.tar` & `psychicapi-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-05-28 22:18:37.957611 psychicapi-0.5/
--rw-r--r--   0 jasonfan   (501) staff       (20)     1745 2023-05-28 22:18:37.957480 psychicapi-0.5/PKG-INFO
--rw-r--r--   0 jasonfan   (501) staff       (20)     1509 2023-05-28 19:19:43.000000 psychicapi-0.5/README.md
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-05-28 22:18:37.956445 psychicapi-0.5/psychicapi/
--rw-r--r--   0 jasonfan   (501) staff       (20)       41 2023-05-19 18:59:00.000000 psychicapi-0.5/psychicapi/__init__.py
--rw-r--r--   0 jasonfan   (501) staff       (20)     1732 2023-05-28 19:19:43.000000 psychicapi-0.5/psychicapi/psychic.py
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-05-28 22:18:37.957299 psychicapi-0.5/psychicapi.egg-info/
--rw-r--r--   0 jasonfan   (501) staff       (20)     1745 2023-05-28 22:18:37.000000 psychicapi-0.5/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 jasonfan   (501) staff       (20)      232 2023-05-28 22:18:37.000000 psychicapi-0.5/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)        1 2023-05-28 22:18:37.000000 psychicapi-0.5/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)        9 2023-05-28 22:18:37.000000 psychicapi-0.5/psychicapi.egg-info/requires.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)       11 2023-05-28 22:18:37.000000 psychicapi-0.5/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)       38 2023-05-28 22:18:37.957646 psychicapi-0.5/setup.cfg
--rw-r--r--   0 jasonfan   (501) staff       (20)      635 2023-05-28 22:15:38.000000 psychicapi-0.5/setup.py
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-05-31 22:25:16.542425 psychicapi-0.6/
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1774 2023-05-31 22:25:16.542214 psychicapi-0.6/PKG-INFO
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1509 2023-05-29 20:05:07.000000 psychicapi-0.6/README.md
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-05-31 22:25:16.540854 psychicapi-0.6/psychicapi/
+-rw-r--r--   0 jasonfan   (501) staff       (20)       41 2023-05-19 18:59:00.000000 psychicapi-0.6/psychicapi/__init__.py
+-rw-r--r--   0 jasonfan   (501) staff       (20)     2504 2023-05-31 15:17:19.000000 psychicapi-0.6/psychicapi/psychic.py
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-05-31 22:25:16.541931 psychicapi-0.6/psychicapi.egg-info/
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1774 2023-05-31 22:25:16.000000 psychicapi-0.6/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 jasonfan   (501) staff       (20)      232 2023-05-31 22:25:16.000000 psychicapi-0.6/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)        1 2023-05-31 22:25:16.000000 psychicapi-0.6/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)        9 2023-05-31 22:25:16.000000 psychicapi-0.6/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)       11 2023-05-31 22:25:16.000000 psychicapi-0.6/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)       38 2023-05-31 22:25:16.542479 psychicapi-0.6/setup.cfg
+-rw-r--r--   0 jasonfan   (501) staff       (20)      664 2023-05-31 22:24:28.000000 psychicapi-0.6/setup.py
```

### Comparing `psychicapi-0.5/PKG-INFO` & `psychicapi-0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: psychicapi
-Version: 0.5
-Summary: Psychic.dev is an open-source universal data connector for knowledgebases.
-Author: Ayan Bandyopadhyay
-Author-email: ayan@psychic.dev
-Description-Content-Type: text/markdown
-
 # Psychic
 
 `psychicapi` is the python client library for [Psychic](https://www.psychic.dev/).
 
 ## What is Psychic?
 
 Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Psychic API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
@@ -36,8 +28,8 @@
 connections = psychic.get_connections(connector_id=ConnectorId.notion, account_id=None)
 ```
 
 ### Retrieve documents from a connection
 
 ```
 docs = psychic.get_documents(ConnectorId.zendesk, "account_id")
-```
+```
```

### Comparing `psychicapi-0.5/README.md` & `psychicapi-0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: psychicapi
+Version: 0.6
+Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
+Author: Ayan Bandyopadhyay
+Author-email: ayan@psychic.dev
+Description-Content-Type: text/markdown
+
 # Psychic
 
 `psychicapi` is the python client library for [Psychic](https://www.psychic.dev/).
 
 ## What is Psychic?
 
 Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Psychic API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
@@ -28,8 +36,8 @@
 connections = psychic.get_connections(connector_id=ConnectorId.notion, account_id=None)
 ```
 
 ### Retrieve documents from a connection
 
 ```
 docs = psychic.get_documents(ConnectorId.zendesk, "account_id")
-```
+```
```

### Comparing `psychicapi-0.5/psychicapi/psychic.py` & `psychicapi-0.6/psychicapi/psychic.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import List, Optional, Dict
 
 class ConnectorId(Enum):
     notion = "notion"
     confluence = "confluence"
     zendesk = "zendesk"
     gdrive = "gdrive"
+    slack = "slack"
 
 class Psychic:
     def __init__(self, secret_key: str):
         self.api_url = "https://sidekick-ezml2kwdva-uc.a.run.app/"
         self.secret_key = secret_key
 
     def get_documents(self, connector_id: ConnectorId, account_id: str):
@@ -49,8 +50,30 @@
                 'Accept': 'application/json'
             }
         )
         if response.status_code == 200:
             documents = response.json()["connections"]
             return documents
         else:
+            return None
+        
+    def get_conversations(self, connector_id: ConnectorId, account_id: str, oldest_timestamp: Optional[int] = None):
+        body = {
+            "connector_id": connector_id.value,
+            "account_id": account_id,
+        }
+        if oldest_timestamp is not None:
+            body["oldest_timestamp"] = oldest_timestamp
+
+        response = requests.post(
+            self.api_url + "get-conversations",
+            json=body,
+            headers={
+                'Authorization': 'Bearer ' + self.secret_key,
+                'Accept': 'application/json'
+            }
+        )
+        if response.status_code == 200:
+            messages = response.json()["messages"]
+            return messages
+        else:
             return None
```

### Comparing `psychicapi-0.5/psychicapi.egg-info/PKG-INFO` & `psychicapi-0.6/psychicapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.5
-Summary: Psychic.dev is an open-source universal data connector for knowledgebases.
+Version: 0.6
+Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
 
 `psychicapi` is the python client library for [Psychic](https://www.psychic.dev/).
```

### Comparing `psychicapi-0.5/setup.py` & `psychicapi-0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='psychicapi',
-    version='0.5',
-    description='Psychic.dev is an open-source universal data connector for knowledgebases.',
+    version='0.6',
+    description='Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayan Bandyopadhyay',
     author_email='ayan@psychic.dev',
     packages=['psychicapi'],
     install_requires=[
         'requests',
```

