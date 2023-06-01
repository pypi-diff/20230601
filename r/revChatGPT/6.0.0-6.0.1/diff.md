# Comparing `tmp/revChatGPT-6.0.0.tar.gz` & `tmp/revChatGPT-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.0.0.tar", last modified: Wed May 31 09:30:09 2023, max compression
+gzip compressed data, was "revChatGPT-6.0.1.tar", last modified: Thu Jun  1 08:11:30 2023, max compression
```

## Comparing `revChatGPT-6.0.0.tar` & `revChatGPT-6.0.1.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:30:09.190348 revChatGPT-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-31 09:30:09.190348 revChatGPT-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-05-31 09:30:09.000000 revChatGPT-6.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 09:30:09.190348 revChatGPT-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:30:09.186348 revChatGPT-6.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:30:09.186348 revChatGPT-6.0.0/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    54844 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:30:09.190348 revChatGPT-6.0.0/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:30:09.190348 revChatGPT-6.0.0/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-31 09:30:09.000000 revChatGPT-6.0.0/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-31 09:30:09.000000 revChatGPT-6.0.0/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:30:09.000000 revChatGPT-6.0.0/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 09:30:09.000000 revChatGPT-6.0.0/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 09:30:09.000000 revChatGPT-6.0.0/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:30:09.190348 revChatGPT-6.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-31 09:29:39.000000 revChatGPT-6.0.0/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:30.650598 revChatGPT-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-01 08:11:00.000000 revChatGPT-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-01 08:11:30.650598 revChatGPT-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-01 08:11:30.000000 revChatGPT-6.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 08:11:30.654598 revChatGPT-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-01 08:11:00.000000 revChatGPT-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:30.646598 revChatGPT-6.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:30.650598 revChatGPT-6.0.1/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    49692 2023-06-01 08:11:00.000000 revChatGPT-6.0.1/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-06-01 08:11:00.000000 revChatGPT-6.0.1/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-01 08:11:00.000000 revChatGPT-6.0.1/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-01 08:11:00.000000 revChatGPT-6.0.1/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:30.650598 revChatGPT-6.0.1/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-01 08:11:00.000000 revChatGPT-6.0.1/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-01 08:11:00.000000 revChatGPT-6.0.1/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-01 08:11:00.000000 revChatGPT-6.0.1/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:30.650598 revChatGPT-6.0.1/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-01 08:11:30.000000 revChatGPT-6.0.1/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-01 08:11:30.000000 revChatGPT-6.0.1/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:11:30.000000 revChatGPT-6.0.1/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-01 08:11:30.000000 revChatGPT-6.0.1/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 08:11:30.000000 revChatGPT-6.0.1/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:11:30.650598 revChatGPT-6.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-01 08:11:00.000000 revChatGPT-6.0.1/tests/test_recipient.py
```

### Comparing `revChatGPT-6.0.0/LICENSE` & `revChatGPT-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.0/PKG-INFO` & `revChatGPT-6.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.0.0
+Version: 6.0.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.0.0/README.md` & `revChatGPT-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.0/setup.py` & `revChatGPT-6.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.0.0",
+    version="6.0.1",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.0.0/src/revChatGPT/V1.py` & `revChatGPT-6.0.1/src/revChatGPT/V1.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,34 +5,31 @@
 
 import base64
 import binascii
 import contextlib
 import datetime
 import json
 import logging
-import tempfile
 import time
 import uuid
 from functools import wraps
 from os import environ
 from os import getenv
 from pathlib import Path
 from typing import AsyncGenerator
 from typing import Generator
 from typing import NoReturn
 
 import httpx
-from curl_cffi import requests
+import requests
+from httpx import AsyncClient
 from OpenAIAuth import Auth0 as Authenticator
 
 from . import __version__
 from . import typings as t
-from .recipient import PythonRecipient
-from .recipient import Recipient
-from .recipient import RecipientManager
 from .utils import create_completer
 from .utils import create_session
 from .utils import get_input
 
 if __name__ == "__main__":
     logging.basicConfig(
         format="%(asctime)s - %(name)s - %(levelname)s - %(funcName)s - %(message)s",
@@ -76,28 +73,24 @@
             return out
 
         return wrapper
 
     return decorator
 
 
-BASE_URL = (
-    environ.get("CHATGPT_BASE_URL") or "https://bypass.churchless.tech/"
-)  # "https://chat.openai.com/backend-api/"
+BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://bypass.churchless.tech/"
 
 bcolors = t.Colors()
 
 
 class Chatbot:
     """
     Chatbot class for ChatGPT
     """
 
-    recipients: RecipientManager
-
     @logger(is_timed=True)
     def __init__(
         self,
         config: dict[str, str],
         conversation_id: str | None = None,
         parent_id: str | None = None,
         lazy_loading: bool = True,
@@ -112,14 +105,15 @@
                     "proxy": "<proxy_url_string>",
                     "model": "<model_name>",
                     "plugin": "<plugin_id>",
                 }
                 More details on these are available at https://github.com/acheong08/ChatGPT#configuration
             conversation_id (str | None, optional): Id of the conversation to continue on. Defaults to None.
             parent_id (str | None, optional): Id of the previous response message to continue on. Defaults to None.
+            session_client (_type_, optional): _description_. Defaults to None.
 
         Raises:
             Exception: _description_
         """
         user_home = getenv("HOME")
         if user_home is None:
             user_home = Path().cwd()
@@ -130,15 +124,14 @@
                 Path(user_home, ".config").mkdir()
             if not Path(user_home, ".config", "revChatGPT").exists():
                 Path(user_home, ".config", "revChatGPT").mkdir()
             self.cache_path = Path(user_home, ".config", "revChatGPT", "cache.json")
 
         self.config = config
         self.session = requests.Session()
-
         if "email" in config and "password" in config:
             try:
                 cached_access_token = self.__get_cached_access_token(
                     self.config.get("email", None),
                 )
             except t.Error as error:
                 if error.code == 5:
@@ -151,42 +144,33 @@
             if not isinstance(config["proxy"], str):
                 error = TypeError("Proxy must be a string!")
                 raise error
             proxies = {
                 "http": config["proxy"],
                 "https": config["proxy"],
             }
-            self.session.proxies = proxies
+            if isinstance(self.session, AsyncClient):
+                proxies = {
+                    "http://": config["proxy"],
+                    "https://": config["proxy"],
+                }
+                self.session = AsyncClient(proxies=proxies)  # type: ignore
+            else:
+                self.session.proxies.update(proxies)
 
         self.conversation_id = conversation_id or config.get("conversation_id", None)
         self.parent_id = parent_id or config.get("parent_id", None)
         self.conversation_mapping = {}
         self.conversation_id_prev_queue = []
         self.parent_id_prev_queue = []
         self.lazy_loading = lazy_loading
-        self.recipients = RecipientManager()
+        self.base_url = base_url or BASE_URL
         self.disable_history = config.get("disable_history", False)
 
         self.__check_credentials()
-        # Check if chat.openai.com is reachable
-        if not base_url:
-            response = self.session.get(
-                "https://chat.openai.com/backend-api/accounts/check",
-                impersonate="safari15_5",
-            )
-            if response.status_code != 200:
-                print(
-                    f"Using bypass.churchless.tech backend due to status code {response.status_code}"
-                )
-                self.base_url = BASE_URL
-            else:
-                print("Using chat.openai.com backend")
-                self.base_url = "https://chat.openai.com/backend-api/"
-        else:
-            self.base_url = base_url
 
     @logger(is_timed=True)
     def __check_credentials(self) -> None:
         """Check login info and perform login
 
         Any one of the following is sufficient for login. Multiple login info can be provided at the same time and they will be used in the order listed below.
             - access_token
@@ -349,32 +333,26 @@
         log.debug("Sending the payload")
 
         cid, pid = data["conversation_id"], data["parent_message_id"]
         model, message = None, ""
 
         self.conversation_id_prev_queue.append(cid)
         self.parent_id_prev_queue.append(pid)
-
-        conversation_stream = self.handle_conversation_stream(step=1)
-
-        with open(conversation_stream.name, "wb") as response_file:
-            response = self.session.post(
-                url=f"{self.base_url}conversation",
-                data=json.dumps(data),
-                timeout=timeout,
-                impersonate="safari15_5",
-                content_callback=response_file.write,  # a hack around curl_cffi not supporting stream=True
-            )
+        response = self.session.post(
+            url=f"{self.base_url}conversation",
+            data=json.dumps(data),
+            timeout=timeout,
+            stream=True,
+        )
         self.__check_response(response)
 
         finish_details = None
-
-        response_lst = self.handle_conversation_stream(file=conversation_stream, step=2)
-
-        for line in response_lst:
+        for line in response.iter_lines():
+            # remove b' and ' at the beginning and end and ignore case
+            line = str(line)[2:-1]
             if line.lower() == "internal server error":
                 log.error(f"Internal Server Error: {line}")
                 error = t.Error(
                     source="ask",
                     message="Internal Server Error",
                     code=t.ErrorType.SERVER_ERROR,
                 )
@@ -382,20 +360,18 @@
             if not line or line is None:
                 continue
             if "data: " in line:
                 line = line[6:]
             if line == "[DONE]":
                 break
 
-            """
-            # this seems to just cut off parts of some messages
+            # DO NOT REMOVE THIS
             line = line.replace('\\"', '"')
             line = line.replace("\\'", "'")
             line = line.replace("\\\\", "\\")
-            """
 
             try:
                 line = json.loads(line)
             except json.decoder.JSONDecodeError:
                 continue
             if not self.__check_fields(line):
                 raise ValueError(f"Field missing. Details: {str(line)}")
@@ -682,51 +658,53 @@
 
         Args:
             response (_type_): _description_
 
         Raises:
             Error: _description_
         """
-        if response.status_code != 200:
+        try:
+            response.raise_for_status()
+        except requests.exceptions.HTTPError as ex:
             error = t.Error(
                 source="OpenAI",
                 message=response.text,
                 code=response.status_code,
             )
-            raise error
+            raise error from ex
 
     @logger(is_timed=True)
     def get_conversations(
         self,
         offset: int = 0,
         limit: int = 20,
         encoding: str | None = None,
     ) -> list:
         """
         Get conversations
         :param offset: Integer
         :param limit: Integer
         """
         url = f"{self.base_url}conversations?offset={offset}&limit={limit}"
-        response = self.session.get(url, impersonate="safari15_5")
+        response = self.session.get(url)
         self.__check_response(response)
         if encoding is not None:
             response.encoding = encoding
         data = json.loads(response.text)
         return data["items"]
 
     @logger(is_timed=True)
     def get_msg_history(self, convo_id: str, encoding: str | None = None) -> list:
         """
         Get message history
         :param id: UUID of conversation
         :param encoding: String
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = self.session.get(url, impersonate="safari15_5")
+        response = self.session.get(url)
         self.__check_response(response)
         if encoding is not None:
             response.encoding = encoding
         return json.loads(response.text)
 
     @logger(is_timed=True)
     def gen_title(self, convo_id: str, message_id: str) -> str:
@@ -734,53 +712,46 @@
         Generate title for conversation
         """
         response = self.session.post(
             f"{self.base_url}conversation/gen_title/{convo_id}",
             data=json.dumps(
                 {"message_id": message_id, "model": "text-davinci-002-render"},
             ),
-            impersonate="safari15_5",
         )
         self.__check_response(response)
         return response.json().get("title", "Error generating title")
 
     @logger(is_timed=True)
     def change_title(self, convo_id: str, title: str) -> None:
         """
         Change title of conversation
         :param id: UUID of conversation
         :param title: String
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = self.session.patch(
-            url, data=json.dumps({"title": title}), impersonate="safari15_5"
-        )
+        response = self.session.patch(url, data=json.dumps({"title": title}))
         self.__check_response(response)
 
     @logger(is_timed=True)
     def delete_conversation(self, convo_id: str) -> None:
         """
         Delete conversation
         :param id: UUID of conversation
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = self.session.patch(
-            url, data='{"is_visible": false}', impersonate="safari15_5"
-        )
+        response = self.session.patch(url, data='{"is_visible": false}')
         self.__check_response(response)
 
     @logger(is_timed=True)
     def clear_conversations(self) -> None:
         """
         Delete all conversations
         """
         url = f"{self.base_url}conversations"
-        response = self.session.patch(
-            url, data='{"is_visible": false}', impersonate="safari15_5"
-        )
+        response = self.session.patch(url, data='{"is_visible": false}')
         self.__check_response(response)
 
     @logger(is_timed=False)
     def __map_conversations(self) -> None:
         conversations = self.get_conversations()
         histories = [self.get_msg_history(x["id"]) for x in conversations]
         for x, y in zip(conversations, histories):
@@ -806,39 +777,26 @@
         for _ in range(num):
             self.conversation_id = self.conversation_id_prev_queue.pop()
             self.parent_id = self.parent_id_prev_queue.pop()
 
     @logger(is_timed=True)
     def get_plugins(self, offset: int = 0, limit: int = 250, status: str = "approved"):
         url = f"{self.base_url}aip/p?offset={offset}&limit={limit}&statuses={status}"
-        response = self.session.get(url, impersonate="safari15_5")
+        response = self.session.get(url)
         self.__check_response(response)
         # Parse as JSON
         return json.loads(response.text)
 
     @logger(is_timed=True)
     def install_plugin(self, plugin_id: str):
         url = f"{self.base_url}aip/p/{plugin_id}/user-settings"
         payload = {"is_installed": True}
-        response = self.session.patch(
-            url, data=json.dumps(payload), impersonate="safari15_5"
-        )
+        response = self.session.patch(url, data=json.dumps(payload))
         self.__check_response(response)
 
-    @logger(is_timed=False)
-    def handle_conversation_stream(self, file=None, step: int = 1):
-        if step == 1:
-            return tempfile.NamedTemporaryFile(delete=False)
-        elif step == 2 and file:
-            with open(file.name) as response_file:
-                response_lst = response_file.read().splitlines()
-            file.close()
-            Path(file.name).unlink()
-            return response_lst
-
 
 class AsyncChatbot(Chatbot):
     """Async Chatbot class for ChatGPT"""
 
     def __init__(
         self,
         config: dict,
@@ -862,81 +820,62 @@
         self.session.headers = headers_transfer
 
     async def __send_request(
         self,
         data: dict,
         auto_continue: bool = False,
         timeout: float = 360,
-            **kwargs
     ) -> AsyncGenerator[dict, None]:
         cid, pid = data["conversation_id"], data["parent_message_id"]
 
         self.conversation_id_prev_queue.append(cid)
         self.parent_id_prev_queue.append(pid)
         message = ""
 
         finish_details = None
         response = None
-
-        conversation_stream = self.handle_conversation_stream(step=1)
-
-        async with self.session as s:
-            with open(conversation_stream.name, "wb") as response_file:
-                response = await s.post(
-                    url=f"{self.base_url}conversation",
-                    data=json.dumps(data),
-                    timeout=timeout,
-                    impersonate="safari15_5",
-                    content_callback=response_file.write,
-                )
+        async with self.session.stream(
+            method="POST",
+            url=f"{self.base_url}conversation",
+            data=json.dumps(data),
+            timeout=timeout,
+        ) as response:
             await self.__check_response(response)
-
-            response_lst = self.handle_conversation_stream(
-                file=conversation_stream, step=2
-            )
-
-            for line in response_lst:
-                if line.lower() == "internal server error":
-                    log.error(f"Internal Server Error: {line}")
-                    error = t.Error(
-                        source="ask",
-                        message="Internal Server Error",
-                        code=t.ErrorType.SERVER_ERROR,
-                    )
-                    raise error
+            async for line in response.aiter_lines():
                 if not line or line is None:
                     continue
                 if "data: " in line:
                     line = line[6:]
                 if "[DONE]" in line:
                     break
 
-                """
-                # this seems to just cut off parts of some messages
+                # DO NOT REMOVE THIS
                 line = line.replace('\\"', '"')
                 line = line.replace("\\'", "'")
                 line = line.replace("\\\\", "\\")
-                """
 
                 try:
                     line = json.loads(line)
                 except json.decoder.JSONDecodeError:
                     continue
                 if not self.__check_fields(line):
                     raise ValueError(f"Field missing. Details: {str(line)}")
                 if line.get("message").get("author").get("role") != "assistant":
                     continue
 
+                message: str = line["message"]["content"]["parts"][0]
                 cid = line["conversation_id"]
                 pid = line["message"]["id"]
                 metadata = line["message"].get("metadata", {})
                 message_exists = False
                 author = {}
                 if line.get("message"):
-                    author = metadata.get("author", {}) or line["message"].get("author", {})
+                    author = metadata.get("author", {}) or line["message"].get(
+                        "author", {}
+                    )
                     if line["message"].get("content"):
                         if line["message"]["content"].get("parts"):
                             if len(line["message"]["content"]["parts"]) > 0:
                                 message_exists = True
                 message: str = (
                     line["message"]["content"]["parts"][0] if message_exists else ""
                 )
@@ -1047,23 +986,23 @@
             data=data,
             auto_continue=auto_continue,
             timeout=timeout,
         ):
             yield msg
 
     async def ask(
-            self,
-            prompt: str,
-            conversation_id: str | None = None,
-            parent_id: str = "",
-            model: str = "",
-            plugin_ids: list = [],
-            auto_continue: bool = False,
-            timeout: int = 360,
-            **kwargs,
+        self,
+        prompt: str,
+        conversation_id: str | None = None,
+        parent_id: str = "",
+        model: str = "",
+        plugin_ids: list = [],
+        auto_continue: bool = False,
+        timeout: int = 360,
+        **kwargs,
     ) -> AsyncGenerator[dict, None]:
         """Ask a question to the chatbot
 
         Args:
             prompt (str): The question to ask
             conversation_id (str | None, optional): UUID for the conversation to continue on. Defaults to None.
             parent_id (str, optional): UUID for the message to continue on. Defaults to "".
@@ -1179,30 +1118,30 @@
     async def get_conversations(self, offset: int = 0, limit: int = 20) -> list:
         """
         Get conversations
         :param offset: Integer
         :param limit: Integer
         """
         url = f"{self.base_url}conversations?offset={offset}&limit={limit}"
-        response = await self.session.get(url, impersonate="safari15_5")
+        response = await self.session.get(url)
         await self.__check_response(response)
         data = json.loads(response.text)
         return data["items"]
 
     async def get_msg_history(
         self,
         convo_id: str,
         encoding: str | None = "utf-8",
     ) -> dict:
         """
         Get message history
         :param id: UUID of conversation
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = await self.session.get(url, impersonate="safari15_5")
+        response = await self.session.get(url)
         if encoding is not None:
             response.encoding = encoding
             await self.__check_response(response)
             return json.loads(response.text)
         return None
 
     async def gen_title(self, convo_id: str, message_id: str) -> None:
@@ -1211,49 +1150,42 @@
         """
         url = f"{self.base_url}conversation/gen_title/{convo_id}"
         response = await self.session.post(
             url,
             data=json.dumps(
                 {"message_id": message_id, "model": "text-davinci-002-render"},
             ),
-            impersonate="safari15_5",
         )
         await self.__check_response(response)
 
     async def change_title(self, convo_id: str, title: str) -> None:
         """
         Change title of conversation
         :param convo_id: UUID of conversation
         :param title: String
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = await self.session.patch(
-            url, data=f'{{"title": "{title}"}}', impersonate="safari15_5"
-        )
+        response = await self.session.patch(url, data=f'{{"title": "{title}"}}')
         await self.__check_response(response)
 
     async def delete_conversation(self, convo_id: str) -> None:
         """
         Delete conversation
         :param convo_id: UUID of conversation
         """
         url = f"{self.base_url}conversation/{convo_id}"
-        response = await self.session.patch(
-            url, data='{"is_visible": false}', impersonate="safari15_5"
-        )
+        response = await self.session.patch(url, data='{"is_visible": false}')
         await self.__check_response(response)
 
     async def clear_conversations(self) -> None:
         """
         Delete all conversations
         """
         url = f"{self.base_url}conversations"
-        response = await self.session.patch(
-            url, data='{"is_visible": false}', impersonate="safari15_5"
-        )
+        response = await self.session.patch(url, data='{"is_visible": false}')
         await self.__check_response(response)
 
     async def __map_conversations(self) -> None:
         conversations = await self.get_conversations()
         histories = [await self.get_msg_history(x["id"]) for x in conversations]
         for x, y in zip(conversations, histories):
             self.conversation_mapping[x["id"]] = y["current_node"]
@@ -1310,16 +1242,14 @@
     Main function for the chatGPT program.
     """
     chatbot = Chatbot(
         config,
         conversation_id=config.get("conversation_id"),
         parent_id=config.get("parent_id"),
     )
-    plugins: dict[str, Recipient] = {}
-    chatbot.recipients["python"] = PythonRecipient
 
     def handle_commands(command: str) -> bool:
         if command == "!help":
             print(
                 """
             !help - Show this message
             !reset - Forget the current conversation
@@ -1365,36 +1295,17 @@
             prev_text = ""
             for data in chatbot.continue_write():
                 message = data["message"][len(prev_text) :]
                 print(message, end="", flush=True)
                 prev_text = data["message"]
             print(bcolors.ENDC)
             print()
-        elif command == "!plugins":
-            print("Plugins:")
-            for plugin, docs in chatbot.recipients.available_recipients.items():
-                print(" [x] " if plugin in plugins else " [ ] ", plugin, ": ", docs)
-            print()
-        elif command.startswith("!switch"):
-            try:
-                plugin = command.split(" ")[1]
-                if plugin in plugins:
-                    del plugins[plugin]
-                else:
-                    plugins[plugin] = chatbot.recipients[plugin]()
-                print(
-                    f"Plugin {plugin} has been "
-                    + ("enabled" if plugin in plugins else "disabled"),
-                )
-                print()
-            except IndexError:
-                log.exception("Please include plugin name in command")
-                print("Please include plugin name in command")
         elif command == "!exit":
-            chatbot.session.close()
+            if isinstance(chatbot.session, httpx.AsyncClient):
+                chatbot.session.aclose()
             exit()
         else:
             return False
         return True
 
     session = create_session()
     completer = create_completer(
@@ -1408,59 +1319,28 @@
             "!continue",
             "!plugins",
             "!switch",
         ],
     )
     print()
     try:
-        msg = {}
         result = {}
-        times = 0
         while True:
-            if not msg:
-                times = 0
-                print(f"{bcolors.OKBLUE + bcolors.BOLD}You: {bcolors.ENDC}")
+            print(f"{bcolors.OKBLUE + bcolors.BOLD}You: {bcolors.ENDC}")
 
-                prompt = get_input(session=session, completer=completer)
-                if prompt.startswith("!") and handle_commands(prompt):
-                    continue
-                if not chatbot.conversation_id and plugins:
-                    prompt = (
-                        (
-                            f"""You are ChatGPT.
-
-Knowledge cutoff: 2021-09
-Current date: {datetime.datetime.now().strftime("%Y-%m-%d")}
-
-###Available Tools:
-"""
-                            + ";".join(plugins)
-                            + "\n\n"
-                            + "\n\n".join([i.API_DOCS for i in plugins.values()])
-                        )
-                        + "\n\n\n\n"
-                        + prompt
-                    )
-                msg = {
-                    "id": str(uuid.uuid4()),
-                    "author": {"role": "user"},
-                    "content": {"content_type": "text", "parts": [prompt]},
-                }
-            else:
-                print(
-                    f"{bcolors.OKCYAN + bcolors.BOLD}{result['recipient'] if result['recipient'] != 'user' else 'You'}: {bcolors.ENDC}",
-                )
-                print(msg["content"]["parts"][0])
+            prompt = get_input(session=session, completer=completer)
+            if prompt.startswith("!") and handle_commands(prompt):
+                continue
 
             print()
             print(f"{bcolors.OKGREEN + bcolors.BOLD}Chatbot: {bcolors.ENDC}")
             if chatbot.config.get("model") == "gpt-4-browsing":
                 print("Browsing takes a while, please wait...")
             prev_text = ""
-            for data in chatbot.post_messages([msg], auto_continue=True):
+            for data in chatbot.ask(prompt=prompt, auto_continue=True):
                 if data["recipient"] != "all":
                     continue
                 result = data
                 message = data["message"][len(prev_text) :]
                 print(message, end="", flush=True)
                 prev_text = data["message"]
             print(bcolors.ENDC)
@@ -1472,32 +1352,14 @@
                 )
                 for citation in result["citations"]:
                     print(
                         f'{citation["metadata"]["title"]}: {citation["metadata"]["url"]}',
                     )
                 print()
 
-            msg = {}
-            if not result.get("end_turn", True):
-                times += 1
-                if times >= 5:
-                    continue
-                api = plugins.get(result["recipient"])
-                if not api:
-                    msg = {
-                        "id": str(uuid.uuid4()),
-                        "author": {"role": "user"},
-                        "content": {
-                            "content_type": "text",
-                            "parts": [f"Error: No plugin {result['recipient']} found"],
-                        },
-                    }
-                    continue
-                msg = api.process(result)
-
     except (KeyboardInterrupt, EOFError):
         exit()
     except Exception as exc:
         error = t.CLIError("command line program unknown error")
         raise error from exc
```

### Comparing `revChatGPT-6.0.0/src/revChatGPT/V3.py` & `revChatGPT-6.0.1/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.0/src/revChatGPT/__init__.py` & `revChatGPT-6.0.1/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.0/src/revChatGPT/__main__.py` & `revChatGPT-6.0.1/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.0/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.0.1/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.0/src/revChatGPT/typings.py` & `revChatGPT-6.0.1/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.0/src/revChatGPT/utils.py` & `revChatGPT-6.0.1/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.0.0/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.0.1/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.0.0
+Version: 6.0.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.0.0/tests/test_recipient.py` & `revChatGPT-6.0.1/tests/test_recipient.py`

 * *Files identical despite different names*

