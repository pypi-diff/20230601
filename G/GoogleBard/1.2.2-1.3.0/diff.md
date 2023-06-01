# Comparing `tmp/GoogleBard-1.2.2.tar.gz` & `tmp/GoogleBard-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-1.2.2.tar", last modified: Thu Jun  1 17:06:01 2023, max compression
+gzip compressed data, was "GoogleBard-1.3.0.tar", last modified: Thu Jun  1 17:39:12 2023, max compression
```

## Comparing `GoogleBard-1.2.2.tar` & `GoogleBard-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:01.429151 GoogleBard-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 17:05:39.000000 GoogleBard-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 17:06:01.429151 GoogleBard-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-01 17:05:39.000000 GoogleBard-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:06:01.429151 GoogleBard-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 17:05:39.000000 GoogleBard-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:01.429151 GoogleBard-1.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-06-01 17:05:39.000000 GoogleBard-1.2.2/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:01.429151 GoogleBard-1.2.2/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 17:06:01.000000 GoogleBard-1.2.2/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-01 17:06:01.000000 GoogleBard-1.2.2/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:06:01.000000 GoogleBard-1.2.2/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 17:06:01.000000 GoogleBard-1.2.2/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 17:06:01.000000 GoogleBard-1.2.2/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:39:12.500398 GoogleBard-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 17:38:49.000000 GoogleBard-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 17:39:12.500398 GoogleBard-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-01 17:38:49.000000 GoogleBard-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:39:12.500398 GoogleBard-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-01 17:38:49.000000 GoogleBard-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:39:12.496398 GoogleBard-1.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-06-01 17:38:49.000000 GoogleBard-1.3.0/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:39:12.500398 GoogleBard-1.3.0/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 17:39:12.000000 GoogleBard-1.3.0/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-01 17:39:12.000000 GoogleBard-1.3.0/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:39:12.000000 GoogleBard-1.3.0/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 17:39:12.000000 GoogleBard-1.3.0/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 17:39:12.000000 GoogleBard-1.3.0/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-1.2.2/LICENSE` & `GoogleBard-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.2.2/PKG-INFO` & `GoogleBard-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.2.2
+Version: 1.3.0
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GoogleBard-1.2.2/README.md` & `GoogleBard-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.2.2/setup.py` & `GoogleBard-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="1.2.2",
+    version="1.3.0",
     license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
     project_urls={"Bug Report": "https://github.com/acheong08/Bard/issues/new"},
-    install_requires=["requests", "prompt_toolkit", "rich"],
+    install_requires=["prompt_toolkit", "rich", "httpx[socks]"],
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["Bard"],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `GoogleBard-1.2.2/src/Bard.py` & `GoogleBard-1.3.0/src/Bard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import argparse
 import json
 import os
 import random
 import re
 import string
 import sys
-import time
 
-import requests
+import httpx
+import asyncio
 from prompt_toolkit import prompt
 from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
 from prompt_toolkit.key_binding import KeyBindings
 from rich.console import Console
@@ -46,23 +46,56 @@
         if prompt_sess
         else prompt(multiline=True)
     )
 
 
 class Chatbot:
     """
+    Synchronous wrapper for the AsyncChatbot class.
+    """
+
+    def __init__(
+        self,
+        session_id: str,
+        proxy: dict = None,
+        timeout: int = 20,
+    ):
+        self.loop = asyncio.get_event_loop()
+        self.async_chatbot = self.loop.run_until_complete(
+            AsyncChatbot.create(session_id, proxy, timeout)
+        )
+
+    def save_conversation(self, file_path: str, conversation_name: str):
+        return self.loop.run_until_complete(
+            self.async_chatbot.save_conversation(file_path, conversation_name)
+        )
+
+    def load_conversations(self, file_path: str) -> List[Dict]:
+        return self.loop.run_until_complete(
+            self.async_chatbot.load_conversations(file_path)
+        )
+
+    def load_conversation(self, file_path: str, conversation_name: str) -> bool:
+        return self.loop.run_until_complete(
+            self.async_chatbot.load_conversation(file_path, conversation_name)
+        )
+
+    def ask(self, message: str) -> dict:
+        return self.loop.run_until_complete(self.async_chatbot.ask(message))
+
+
+class AsyncChatbot:
+    """
     A class to interact with Google Bard.
     Parameters
         session_id: str
             The __Secure-1PSID cookie.
         proxy: str
         timeout: int
             Request timeout in seconds.
-        session: requests.Session
-            Requests session object.
     """
 
     __slots__ = [
         "headers",
         "_reqid",
         "SNlM0e",
         "conversation_id",
@@ -75,15 +108,14 @@
     ]
 
     def __init__(
         self,
         session_id: str,
         proxy: dict = None,
         timeout: int = 20,
-        session: requests.Session = None,
     ):
         headers = {
             "Host": "bard.google.com",
             "X-Same-Domain": "1",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
             "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
             "Origin": "https://bard.google.com",
@@ -91,21 +123,31 @@
         }
         self._reqid = int("".join(random.choices(string.digits, k=4)))
         self.proxy = proxy
         self.conversation_id = ""
         self.response_id = ""
         self.choice_id = ""
         self.session_id = session_id
-        self.session = session or requests.Session()
+        self.session = httpx.AsyncClient(proxies=self.proxy)
         self.session.headers = headers
         self.session.cookies.set("__Secure-1PSID", session_id)
-        self.SNlM0e = self.__get_snlm0e()
         self.timeout = timeout
 
-    def save_conversation(self, file_path: str, conversation_name: str):
+    @classmethod
+    async def create(
+        cls,
+        session_id: str,
+        proxy: dict = None,
+        timeout: int = 20,
+    ) -> "AsyncChatbot":
+        instance = cls(session_id, proxy, timeout)
+        instance.SNlM0e = await instance.__get_snlm0e()
+        return instance
+
+    async def save_conversation(self, file_path: str, conversation_name: str):
         conversations = self.load_conversations(file_path)
         conversation_details = {
             {
                 "conversation_name": conversation_name,
                 "_reqid": self._reqid,
                 "conversation_id": self.conversation_id,
                 "response_id": self.response_id,
@@ -114,59 +156,58 @@
             },
         }
         conversations.append(conversation_details)
 
         with open(file_path, "w", encoding="utf-8") as f:
             json.dump(conversations, f, indent=4)
 
-    def load_conversations(self, file_path: str) -> List[Dict]:
+    async def load_conversations(self, file_path: str) -> List[Dict]:
         # Check if file exists
         if not os.path.isfile(file_path):
             return []
         with open(file_path, encoding="utf-8") as f:
             return json.load(f)
 
-    def load_conversation(self, file_path: str, conversation_name: str) -> bool:
+    async def load_conversation(self, file_path: str, conversation_name: str) -> bool:
         """
         Loads a conversation from history file. Returns whether the conversation was found.
         """
         conversations = self.load_conversations(file_path)
         for conversation in conversations:
             if conversation["conversation_name"] == conversation_name:
                 self._reqid = conversation["_reqid"]
                 self.conversation_id = conversation["conversation_id"]
                 self.response_id = conversation["response_id"]
                 self.choice_id = conversation["choice_id"]
                 self.SNlM0e = conversation["SNlM0e"]
                 return True
         return False
 
-    def __get_snlm0e(self):
+    async def __get_snlm0e(self):
         # Find "SNlM0e":"<ID>"
         if not self.session_id or self.session_id[-1] != ".":
             raise Exception(
                 "__Secure-1PSID value must end with a single dot. Enter correct __Secure-1PSID value.",
             )
-        resp = self.session.get(
+        resp = await self.session.get(
             "https://bard.google.com/",
             timeout=10,
-            proxies=self.proxy,
         )
         if resp.status_code != 200:
             raise Exception(
                 f"Response code not 200. Response Status is {resp.status_code}",
             )
         SNlM0e = re.search(r"SNlM0e\":\"(.*?)\"", resp.text)
         if not SNlM0e:
             raise Exception(
                 "SNlM0e value not found in response. Check __Secure-1PSID value.",
             )
         return SNlM0e.group(1)
 
-    def ask(self, message: str) -> dict:
+    async def ask(self, message: str) -> dict:
         """
         Send a message to Google Bard and return the response.
         :param message: The message to send to Google Bard.
         :return: A dict containing the response from Google Bard.
         """
         # url params
         params = {
@@ -181,20 +222,19 @@
             None,
             [self.conversation_id, self.response_id, self.choice_id],
         ]
         data = {
             "f.req": json.dumps([None, json.dumps(message_struct)]),
             "at": self.SNlM0e,
         }
-        resp = self.session.post(
+        resp = await self.session.post(
             "https://bard.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate",
             params=params,
             data=data,
             timeout=self.timeout,
-            proxies=self.proxy,
         )
         chat_data = json.loads(resp.content.splitlines()[3])[0][2]
         if not chat_data:
             return {"content": f"Google Bard encountered an error: {resp.content}."}
         json_chat_data = json.loads(chat_data)
         images = set()
         if len(json_chat_data) >= 3:
```

### Comparing `GoogleBard-1.2.2/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-1.3.0/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.2.2
+Version: 1.3.0
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

