# Comparing `tmp/vector_vault-1.6.3.tar.gz` & `tmp/vector_vault-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.6.3.tar", last modified: Wed May 31 06:49:05 2023, max compression
+gzip compressed data, was "vector_vault-1.6.4.tar", last modified: Thu Jun  1 01:06:08 2023, max compression
```

## Comparing `vector_vault-1.6.3.tar` & `vector_vault-1.6.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-31 06:49:05.289125 vector_vault-1.6.3/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.3/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    21275 2023-05-31 06:49:05.289001 vector_vault-1.6.3/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    20550 2023-05-31 05:38:28.000000 vector_vault-1.6.3/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-31 06:49:05.289162 vector_vault-1.6.3/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-31 06:47:53.000000 vector_vault-1.6.3/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-31 06:49:05.285782 vector_vault-1.6.3/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    21275 2023-05-31 06:49:05.000000 vector_vault-1.6.3/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-05-31 06:49:05.000000 vector_vault-1.6.3/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-31 06:49:05.000000 vector_vault-1.6.3/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-31 06:49:05.000000 vector_vault-1.6.3/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-31 06:49:05.000000 vector_vault-1.6.3/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-31 06:49:05.288600 vector_vault-1.6.3/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.3/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6238 2023-05-28 06:54:07.000000 vector_vault-1.6.3/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3249 2023-05-31 06:45:39.000000 vector_vault-1.6.3/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1843 2023-05-30 20:06:58.000000 vector_vault-1.6.3/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.3/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1582 2023-05-31 06:45:44.000000 vector_vault-1.6.3/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.3/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18190 2023-05-31 06:45:53.000000 vector_vault-1.6.3/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.6.3/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.3/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 01:06:08.099679 vector_vault-1.6.4/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.4/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 01:06:08.099512 vector_vault-1.6.4/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.6.4/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-01 01:06:08.099717 vector_vault-1.6.4/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-01 01:04:34.000000 vector_vault-1.6.4/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 01:06:08.096159 vector_vault-1.6.4/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-01 01:06:08.000000 vector_vault-1.6.4/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-01 01:06:08.000000 vector_vault-1.6.4/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-01 01:06:08.000000 vector_vault-1.6.4/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-01 01:06:08.000000 vector_vault-1.6.4/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-01 01:06:08.000000 vector_vault-1.6.4/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-01 01:06:08.099104 vector_vault-1.6.4/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.4/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6238 2023-05-28 06:54:07.000000 vector_vault-1.6.4/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3249 2023-06-01 00:49:04.000000 vector_vault-1.6.4/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1843 2023-05-30 20:06:58.000000 vector_vault-1.6.4/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.4/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1582 2023-06-01 00:49:00.000000 vector_vault-1.6.4/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.4/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    18190 2023-06-01 00:49:07.000000 vector_vault-1.6.4/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.6.4/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.4/vectorvault/wrap.py
```

### Comparing `vector_vault-1.6.3/LICENSE` & `vector_vault-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.3/PKG-INFO` & `vector_vault-1.6.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.6.3
+Version: 1.6.4
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -254,16 +254,17 @@
     summary = vault.get_chat(summary, summary=True)
 ```
 ^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
 
 <br>
 <br>
 <br>
+<br>
 
-# Metadata
+# Metadata Made Easy
 
 Metadata is useful later, when you make a call to the vault and want to know specifics about the data you got back. To add metadata to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so the name field in the metadata always exists)
 ```
 meta = {
     'name': 'Lifestyle in LA',
     'country': 'United State',
     'city': 'LA' 
@@ -378,75 +379,14 @@
 
 - lab notes vault within chemistry vault
 ```
 lab_notes_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
 
 
-<br>
-
-## Real world usage:
-```
-user_input = input("What's your question?")
-
-# Get response from Language model
-vault_response = vault.get_chat(user_input, get_context=True, return_context=True)
-
-answer = vault_response['response']
-print("Question:", user_input, "\n\nAnswer:", answer)
-
-# show the context used to generate the answer
-for item in vault_response['context']:
-    print("\n\n", f"item {item['metadata']['item_id']}")
-    print(item['data'])
-
-```
-
->> Question: 
-What is a token broker? 
- 
->>Answer: 
-A token broker is a service that generates downscoped access tokens for token
-consumers to access or modify specific resources...
->>
-
->> item 33
-Various workloads (token consumers) in the same network will send authenticated
-requests to that broker for downscoped tokens to...
->>
- >>item 4
-Another reason to use downscoped credentials is to ensure tokens in flight...
->>
-
-
->>
->> item 37
-The following is an...
->>
-
-
-<br>
-
-```
-user_input2 = input("What's your next question?")
-
-history = user_input + answer
-
-# Get response from Language model
-vault_response = vault.get_chat(user_input2, history=history, get_context=True)
-
-print("Question:", user_input2, "\n\nAnswer:", vault_response2)
-```
->> Question: 
-How do I use it? 
- 
->>Answer: 
-You can use it by...
-
-
 
 <br>
 <br>
 <br>
 
 # Build an AI Cusomter Service Chat Bot
 <p align="center">
@@ -493,15 +433,15 @@
 ---
 <br>
 <br>
 
 
 
 ## Getting Started:
-Open the "examples" folder and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
+Open the [examples folder](https://github.com/John-Rood/VectorVault/tree/main/examples) and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
 
 <br>
 <br>
 
 ## Contact:
 ### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
```

### Comparing `vector_vault-1.6.3/README.md` & `vector_vault-1.6.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -235,16 +235,17 @@
     summary = vault.get_chat(summary, summary=True)
 ```
 ^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
 
 <br>
 <br>
 <br>
+<br>
 
-# Metadata
+# Metadata Made Easy
 
 Metadata is useful later, when you make a call to the vault and want to know specifics about the data you got back. To add metadata to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so the name field in the metadata always exists)
 ```
 meta = {
     'name': 'Lifestyle in LA',
     'country': 'United State',
     'city': 'LA' 
@@ -359,75 +360,14 @@
 
 - lab notes vault within chemistry vault
 ```
 lab_notes_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
 
 
-<br>
-
-## Real world usage:
-```
-user_input = input("What's your question?")
-
-# Get response from Language model
-vault_response = vault.get_chat(user_input, get_context=True, return_context=True)
-
-answer = vault_response['response']
-print("Question:", user_input, "\n\nAnswer:", answer)
-
-# show the context used to generate the answer
-for item in vault_response['context']:
-    print("\n\n", f"item {item['metadata']['item_id']}")
-    print(item['data'])
-
-```
-
->> Question: 
-What is a token broker? 
- 
->>Answer: 
-A token broker is a service that generates downscoped access tokens for token
-consumers to access or modify specific resources...
->>
-
->> item 33
-Various workloads (token consumers) in the same network will send authenticated
-requests to that broker for downscoped tokens to...
->>
- >>item 4
-Another reason to use downscoped credentials is to ensure tokens in flight...
->>
-
-
->>
->> item 37
-The following is an...
->>
-
-
-<br>
-
-```
-user_input2 = input("What's your next question?")
-
-history = user_input + answer
-
-# Get response from Language model
-vault_response = vault.get_chat(user_input2, history=history, get_context=True)
-
-print("Question:", user_input2, "\n\nAnswer:", vault_response2)
-```
->> Question: 
-How do I use it? 
- 
->>Answer: 
-You can use it by...
-
-
 
 <br>
 <br>
 <br>
 
 # Build an AI Cusomter Service Chat Bot
 <p align="center">
@@ -474,15 +414,15 @@
 ---
 <br>
 <br>
 
 
 
 ## Getting Started:
-Open the "examples" folder and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
+Open the [examples folder](https://github.com/John-Rood/VectorVault/tree/main/examples) and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
 
 <br>
 <br>
 
 ## Contact:
 ### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
```

### Comparing `vector_vault-1.6.3/setup.py` & `vector_vault-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.6.3",
+    version="1.6.4",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.6.3/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.6.4/vector_vault.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.6.3
+Version: 1.6.4
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -254,16 +254,17 @@
     summary = vault.get_chat(summary, summary=True)
 ```
 ^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
 
 <br>
 <br>
 <br>
+<br>
 
-# Metadata
+# Metadata Made Easy
 
 Metadata is useful later, when you make a call to the vault and want to know specifics about the data you got back. To add metadata to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so the name field in the metadata always exists)
 ```
 meta = {
     'name': 'Lifestyle in LA',
     'country': 'United State',
     'city': 'LA' 
@@ -378,75 +379,14 @@
 
 - lab notes vault within chemistry vault
 ```
 lab_notes_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
 
 
-<br>
-
-## Real world usage:
-```
-user_input = input("What's your question?")
-
-# Get response from Language model
-vault_response = vault.get_chat(user_input, get_context=True, return_context=True)
-
-answer = vault_response['response']
-print("Question:", user_input, "\n\nAnswer:", answer)
-
-# show the context used to generate the answer
-for item in vault_response['context']:
-    print("\n\n", f"item {item['metadata']['item_id']}")
-    print(item['data'])
-
-```
-
->> Question: 
-What is a token broker? 
- 
->>Answer: 
-A token broker is a service that generates downscoped access tokens for token
-consumers to access or modify specific resources...
->>
-
->> item 33
-Various workloads (token consumers) in the same network will send authenticated
-requests to that broker for downscoped tokens to...
->>
- >>item 4
-Another reason to use downscoped credentials is to ensure tokens in flight...
->>
-
-
->>
->> item 37
-The following is an...
->>
-
-
-<br>
-
-```
-user_input2 = input("What's your next question?")
-
-history = user_input + answer
-
-# Get response from Language model
-vault_response = vault.get_chat(user_input2, history=history, get_context=True)
-
-print("Question:", user_input2, "\n\nAnswer:", vault_response2)
-```
->> Question: 
-How do I use it? 
- 
->>Answer: 
-You can use it by...
-
-
 
 <br>
 <br>
 <br>
 
 # Build an AI Cusomter Service Chat Bot
 <p align="center">
@@ -493,15 +433,15 @@
 ---
 <br>
 <br>
 
 
 
 ## Getting Started:
-Open the "examples" folder and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
+Open the [examples folder](https://github.com/John-Rood/VectorVault/tree/main/examples) and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
 
 <br>
 <br>
 
 ## Contact:
 ### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
```

### Comparing `vector_vault-1.6.3/vectorvault/__init__.py` & `vector_vault-1.6.4/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.3/vectorvault/ai.py` & `vector_vault-1.6.4/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.3/vectorvault/cloudmanager.py` & `vector_vault-1.6.4/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.3/vectorvault/creds.py` & `vector_vault-1.6.4/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.3/vectorvault/download.py` & `vector_vault-1.6.4/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.3/vectorvault/itemize.py` & `vector_vault-1.6.4/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.3/vectorvault/signup.py` & `vector_vault-1.6.4/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.3/vectorvault/vault.py` & `vector_vault-1.6.4/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.3/vectorvault/vecreq.py` & `vector_vault-1.6.4/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.3/vectorvault/wrap.py` & `vector_vault-1.6.4/vectorvault/wrap.py`

 * *Files identical despite different names*

