# Comparing `tmp/freeGPT-1.1.3.tar.gz` & `tmp/freeGPT-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-4bhwh_th\freeGPT-1.1.3.tar", last modified: Fri May 26 13:20:15 2023, max compression
+gzip compressed data, was "freeGPT-1.1.4.tar", last modified: Thu Jun  1 07:46:53 2023, max compression
```

## Comparing `freeGPT-1.1.3.tar` & `freeGPT-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 13:20:15.886983 freeGPT-1.1.3/
--rw-rw-rw-   0        0        0    35149 2023-05-26 13:18:55.000000 freeGPT-1.1.3/LICENSE
--rw-rw-rw-   0        0        0       98 2023-05-26 13:18:55.000000 freeGPT-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2958 2023-05-26 13:20:15.886983 freeGPT-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1953 2023-05-26 13:18:55.000000 freeGPT-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 13:20:15.871358 freeGPT-1.1.3/freeGPT/
--rw-rw-rw-   0        0        0     1868 2023-05-26 13:18:55.000000 freeGPT-1.1.3/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 13:20:15.886983 freeGPT-1.1.3/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     5181 2023-05-26 13:18:55.000000 freeGPT-1.1.3/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 13:20:15.886983 freeGPT-1.1.3/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     6915 2023-05-26 13:18:55.000000 freeGPT-1.1.3/freeGPT/gpt4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 13:20:15.886983 freeGPT-1.1.3/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     2958 2023-05-26 13:20:15.000000 freeGPT-1.1.3/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-05-26 13:20:15.000000 freeGPT-1.1.3/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 13:20:15.000000 freeGPT-1.1.3/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-26 13:20:15.000000 freeGPT-1.1.3/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-26 13:20:15.000000 freeGPT-1.1.3/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 13:20:15.886983 freeGPT-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1416 2023-05-26 13:18:55.000000 freeGPT-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 07:46:53.186462 freeGPT-1.1.4/
+-rw-rw-rw-   0        0        0    35149 2023-06-01 07:16:24.000000 freeGPT-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-06-01 07:16:24.000000 freeGPT-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3226 2023-06-01 07:46:53.186462 freeGPT-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2166 2023-06-01 07:16:24.000000 freeGPT-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 07:46:53.186462 freeGPT-1.1.4/freeGPT/
+-rw-rw-rw-   0        0        0     2340 2023-06-01 07:16:24.000000 freeGPT-1.1.4/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 07:46:53.186462 freeGPT-1.1.4/freeGPT/alpaca/
+-rw-rw-rw-   0        0        0     1530 2023-06-01 07:16:24.000000 freeGPT-1.1.4/freeGPT/alpaca/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 07:46:53.186462 freeGPT-1.1.4/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     5187 2023-06-01 07:16:24.000000 freeGPT-1.1.4/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 07:46:53.186462 freeGPT-1.1.4/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     6827 2023-06-01 07:16:24.000000 freeGPT-1.1.4/freeGPT/gpt4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 07:46:53.186462 freeGPT-1.1.4/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     3226 2023-06-01 07:46:53.000000 freeGPT-1.1.4/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-06-01 07:46:53.000000 freeGPT-1.1.4/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 07:46:53.000000 freeGPT-1.1.4/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-01 07:46:53.000000 freeGPT-1.1.4/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-01 07:46:53.000000 freeGPT-1.1.4/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 07:46:53.186462 freeGPT-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1518 2023-06-01 07:16:24.000000 freeGPT-1.1.4/setup.py
```

### Comparing `freeGPT-1.1.3/LICENSE` & `freeGPT-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.3/PKG-INFO` & `freeGPT-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.3
-Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
+Version: 1.1.4
+Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
-Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
+Keywords: artificial-intelligence,machine-learning,ai-models,chatllama,gpt4free,freegpt,chatgpt,python,alpaca,openai,gpt3,gpt4,gpt,py,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -22,15 +22,15 @@
 
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
 [![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
-*Get started by doing: `pip install freeGPT`*
+*Get started by doing: `pip install freeGPT==1.1.3`*
 
 ## Source:
 *Models with .web have internet access on.*
 <br>
 | Models            | Websites                                 |
 | ----------------- | -----------------------------------------|
 | gpt3              | [you.com](https://you.com)               |
@@ -39,35 +39,43 @@
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Make GPT-3 & GPT-4 models with web access.
-- [ ] Add a text to image generation model
-- [ ] Make a discord bot
+- [x] Add a non-GPT model.
+- [ ] Add a text to image generation model.
+- [ ] Make a discord bot.
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
 ## Examples:
 
-#### GPT-3:
+#### Alpaca-7b:
+```python
+from freeGPT import alpaca
 
+while True:
+    prompt = input("👦 > ")
+    resp = alpaca.Completion.create(prompt=prompt)
+    print(f"🤖 > {resp}")
+```
+#### GPT-3:
 ```python
 from freeGPT import gpt3
 
 while True:
     prompt = input("👦 > ")
     resp = gpt3.Completion.create(prompt=prompt)
     print(f"🤖 > {resp['text']}")
 ```
 #### GPT-4:
-
 ```python
 # Uhh, sorry but gpt4 is kinda broken currently, will maybe get fixed in the next update.
 from freeGPT import gpt4
 
 while True:
     token = Account.create(logging=True)
     prompt = input("👦 > ")
```

### Comparing `freeGPT-1.1.3/README.md` & `freeGPT-1.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
 [![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
-*Get started by doing: `pip install freeGPT`*
+*Get started by doing: `pip install freeGPT==1.1.3`*
 
 ## Source:
 *Models with .web have internet access on.*
 <br>
 | Models            | Websites                                 |
 | ----------------- | -----------------------------------------|
 | gpt3              | [you.com](https://you.com)               |
@@ -17,35 +17,43 @@
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Make GPT-3 & GPT-4 models with web access.
-- [ ] Add a text to image generation model
-- [ ] Make a discord bot
+- [x] Add a non-GPT model.
+- [ ] Add a text to image generation model.
+- [ ] Make a discord bot.
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
 ## Examples:
 
-#### GPT-3:
+#### Alpaca-7b:
+```python
+from freeGPT import alpaca
 
+while True:
+    prompt = input("👦 > ")
+    resp = alpaca.Completion.create(prompt=prompt)
+    print(f"🤖 > {resp}")
+```
+#### GPT-3:
 ```python
 from freeGPT import gpt3
 
 while True:
     prompt = input("👦 > ")
     resp = gpt3.Completion.create(prompt=prompt)
     print(f"🤖 > {resp['text']}")
 ```
 #### GPT-4:
-
 ```python
 # Uhh, sorry but gpt4 is kinda broken currently, will maybe get fixed in the next update.
 from freeGPT import gpt4
 
 while True:
     token = Account.create(logging=True)
     prompt = input("👦 > ")
```

### Comparing `freeGPT-1.1.3/freeGPT/__init__.py` & `freeGPT-1.1.4/freeGPT/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from enum import Enum
-from freeGPT import gpt3, gpt4
+from freeGPT import gpt3, gpt4, alpaca
 
 __author__ = "Ruu3f"
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 __all__ = ["Provider", "Completion"]
 
 
 class Provider(Enum):
     """Enum class representing the available GPT providers."""
 
+    ALPACA = "alpaca"
     GPT3 = "gpt3"
     GPT4 = "gpt4"
 
 
 class Completion:
     """Class for generating completions using different GPT providers."""
 
@@ -28,37 +29,52 @@
 
         Returns:
             str: The generated completion text.
 
         Raises:
             Exception: If the provider doesn't exist.
         """
-        if provider == Provider.GPT3:
-            return Completion.__gpt3_service(prompt, **kwargs)
+        if provider == Provider.ALPACA:
+            return Completion._alpaca_service(prompt, **kwargs)
+        elif provider == Provider.GPT3:
+            return Completion._gpt3_service(prompt, **kwargs)
         elif provider == Provider.GPT4:
-            return Completion.__gpt4_service(prompt, **kwargs)
+            return Completion._gpt4_service(prompt, **kwargs)
         else:
             raise Exception("Provider doesn't exist. Please check it again.")
 
     @staticmethod
-    def __gpt3_service(prompt: str) -> str:
+    def _alpaca_service(prompt: str) -> str:
+        """
+        Generates a completion using the Alpaca provider.
+
+        Args:
+            prompt (str): The prompt text for completion.
+
+        Returns:
+            str: The generated completion text.
+        """
+        return alpaca.Completion.create(prompt=prompt)
+
+    @staticmethod
+    def _gpt3_service(prompt: str) -> str:
         """
         Generates a completion using the GPT-3 provider.
 
         Args:
             prompt (str): The prompt text for completion.
 
         Returns:
             str: The generated completion text.
         """
         resp = gpt3.Completion.create(prompt=prompt)
         return resp["text"]
 
     @staticmethod
-    def __gpt4_service(prompt: str) -> str:
+    def _gpt4_service(prompt: str) -> str:
         """
         Generates a completion using the GPT-4 provider.
 
         Args:
             prompt (str): The prompt text for completion.
 
         Returns:
```

### Comparing `freeGPT-1.1.3/freeGPT/gpt3/__init__.py` & `freeGPT-1.1.4/freeGPT/gpt3/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import os, re, json
+import re, json, subprocess
 
 try:
     from tls_client import Session
 except:
-    os.system("pip install tls_client --no-cache-dir")
+    subprocess.check_call(["pip", "install", "tls_client --no-cache-dir"])
 from uuid import uuid4
 from pydantic import BaseModel
 from fake_useragent import UserAgent
 from typing import Optional, List, Dict, Any
 
 
 class Completion:
@@ -79,15 +79,15 @@
                 if query_trace_id is None
                 else query_trace_id,
                 "chat": str(chat),
             },
         )
 
         if "youChatToken" not in response.text:
-            raise Exception("Unable to get the response, please try again later.")
+            raise Exception("Unable to fetch the response.")
 
         you_chat_serp_results = re.search(
             r"(?<=event: youChatSerpResults\ndata:)(.*\n)*?(?=event: )", response.text
         ).group()
         third_party_search_results = re.search(
             r"(?<=event: thirdPartySearchResults\ndata:)(.*\n)*?(?=event: )",
             response.text,
```

### Comparing `freeGPT-1.1.3/freeGPT/gpt4/__init__.py` & `freeGPT-1.1.4/freeGPT/gpt4/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import os, re, json
+import re, json, subprocess
 
 try:
     from tls_client import Session
 except ImportError:
-    os.system("pip install tls_client --no-cache-dir")
+    subprocess.check_call(["pip", "install", "tls_client --no-cache-dir"])
+
 from uuid import uuid4
 from requests import post
 from time import time, sleep
 from fake_useragent import UserAgent
 from pymailtm import MailTm, Message
 from typing import Any, List, Generator, Optional
 from pydantic import BaseModel
@@ -112,17 +113,14 @@
 
         response = client.get(
             "https://clerk.forefront.ai/v1/client?_clerk_js_version=4.38.4"
         )
 
         token = response.json()["response"]["sessions"][0]["last_active_token"]["jwt"]
 
-        with open("accounts.txt", "a") as f:
-            f.write(f"{mail_address}:{token}\n")
-
         if logging:
             print(time() - start)
 
         return token
 
 
 class Completion:
@@ -218,8 +216,8 @@
                             "completion_tokens": len(token),
                             "total_tokens": len(prompt) + len(token),
                         },
                     }
                 )
                 return final_response
 
-        raise Exception("Unable to get the response, please try again later.")
+        raise Exception("Unable to fetch the response.")
```

### Comparing `freeGPT-1.1.3/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.1.4/freeGPT.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.3
-Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
+Version: 1.1.4
+Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
-Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
+Keywords: artificial-intelligence,machine-learning,ai-models,chatllama,gpt4free,freegpt,chatgpt,python,alpaca,openai,gpt3,gpt4,gpt,py,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -22,15 +22,15 @@
 
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
 [![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
-*Get started by doing: `pip install freeGPT`*
+*Get started by doing: `pip install freeGPT==1.1.3`*
 
 ## Source:
 *Models with .web have internet access on.*
 <br>
 | Models            | Websites                                 |
 | ----------------- | -----------------------------------------|
 | gpt3              | [you.com](https://you.com)               |
@@ -39,35 +39,43 @@
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Make GPT-3 & GPT-4 models with web access.
-- [ ] Add a text to image generation model
-- [ ] Make a discord bot
+- [x] Add a non-GPT model.
+- [ ] Add a text to image generation model.
+- [ ] Make a discord bot.
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
 ## Examples:
 
-#### GPT-3:
+#### Alpaca-7b:
+```python
+from freeGPT import alpaca
 
+while True:
+    prompt = input("👦 > ")
+    resp = alpaca.Completion.create(prompt=prompt)
+    print(f"🤖 > {resp}")
+```
+#### GPT-3:
 ```python
 from freeGPT import gpt3
 
 while True:
     prompt = input("👦 > ")
     resp = gpt3.Completion.create(prompt=prompt)
     print(f"🤖 > {resp['text']}")
 ```
 #### GPT-4:
-
 ```python
 # Uhh, sorry but gpt4 is kinda broken currently, will maybe get fixed in the next update.
 from freeGPT import gpt4
 
 while True:
     token = Account.create(logging=True)
     prompt = input("👦 > ")
```

### Comparing `freeGPT-1.1.3/setup.py` & `freeGPT-1.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.1.3",
-    description="freeGPT is a Python package that gives free access to GPT3 and GPT4 models.",
+    version="1.1.4",
+    description="freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
         "artificial-intelligence",
         "machine-learning",
         "ai-models",
+        "chatllama",
+        "gpt4free",
         "freegpt",
         "chatgpt",
+        "python",
+        "alpaca",
         "openai",
-        "gpt3"
-        "gpt4"
+        "gpt3",
+        "gpt4",
         "gpt",
+        "py",
         "ai",
     ],
     python_requires=">=3.6",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

