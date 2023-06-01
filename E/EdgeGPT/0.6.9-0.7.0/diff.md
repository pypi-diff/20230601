# Comparing `tmp/EdgeGPT-0.6.9.tar.gz` & `tmp/EdgeGPT-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.6.9.tar", last modified: Mon May 29 02:18:30 2023, max compression
+gzip compressed data, was "EdgeGPT-0.7.0.tar", last modified: Thu Jun  1 09:03:51 2023, max compression
```

## Comparing `EdgeGPT-0.6.9.tar` & `EdgeGPT-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:18:30.036017 EdgeGPT-0.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-29 02:17:53.000000 EdgeGPT-0.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-29 02:18:30.036017 EdgeGPT-0.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-29 02:18:29.000000 EdgeGPT-0.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 02:18:30.036017 EdgeGPT-0.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-29 02:17:53.000000 EdgeGPT-0.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:18:30.036017 EdgeGPT-0.6.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:18:30.036017 EdgeGPT-0.6.9/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-29 02:18:30.000000 EdgeGPT-0.6.9/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 02:18:30.000000 EdgeGPT-0.6.9/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:18:30.000000 EdgeGPT-0.6.9/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-29 02:18:30.000000 EdgeGPT-0.6.9/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 02:18:30.000000 EdgeGPT-0.6.9/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 02:18:30.000000 EdgeGPT-0.6.9/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39337 2023-05-29 02:17:53.000000 EdgeGPT-0.6.9/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-29 02:17:53.000000 EdgeGPT-0.6.9/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:51.180593 EdgeGPT-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-01 09:03:20.000000 EdgeGPT-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-01 09:03:51.180593 EdgeGPT-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-06-01 09:03:51.000000 EdgeGPT-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 09:03:51.184593 EdgeGPT-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-01 09:03:20.000000 EdgeGPT-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:51.180593 EdgeGPT-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:03:51.180593 EdgeGPT-0.7.0/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-01 09:03:51.000000 EdgeGPT-0.7.0/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-01 09:03:51.000000 EdgeGPT-0.7.0/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:03:51.000000 EdgeGPT-0.7.0/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 09:03:51.000000 EdgeGPT-0.7.0/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 09:03:51.000000 EdgeGPT-0.7.0/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 09:03:51.000000 EdgeGPT-0.7.0/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    43424 2023-06-01 09:03:20.000000 EdgeGPT-0.7.0/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-01 09:03:20.000000 EdgeGPT-0.7.0/src/ImageGen.py
```

### Comparing `EdgeGPT-0.6.9/LICENSE` & `EdgeGPT-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.6.9/PKG-INFO` & `EdgeGPT-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.6.9
+Version: 0.7.0
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -104,27 +104,36 @@
         EdgeGPT - A demo of reverse engineering the Bing GPT chatbot
         Repo: github.com/acheong08/EdgeGPT
         By: Antonio Cheong
 
         !help for help
 
         Type !exit to exit
-        Enter twice to send message or set --enter-once to send one line message
 
-usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [--style {creative,balanced,precise}]
+usage: EdgeGPT.py [-h] [--enter-once] [--search-result] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK]
+                  [--style {creative,balanced,precise}] [--prompt PROMPT] [--cookie-file COOKIE_FILE]
+                  [--history-file HISTORY_FILE] [--locale LOCALE]
 
 options:
   -h, --help            show this help message and exit
   --enter-once
+  --search-result
   --no-stream
   --rich
   --proxy PROXY         Proxy URL (e.g. socks5://127.0.0.1:1080)
+  --wss-link WSS_LINK   WSS URL(e.g. wss://sydney.bing.com/sydney/ChatHub)
   --style {creative,balanced,precise}
-  --cookie-file [path/to/cookies.json]
+  --prompt PROMPT       prompt to start with
+  --cookie-file COOKIE_FILE
+                        path to cookie file
+  --history-file HISTORY_FILE
+                        path to history file
+  --locale LOCALE       your locale (e.g. en-US, zh-CN, en-IE, en-GB)
 ```
+(China/US/UK/Norway has enhanced support for locale)
 
 ## Running in Python
 
 ### 1. The `Chatbot` class and `asyncio` for more granular control
 
 Use Async for the best experience, for example:
 
@@ -146,14 +155,16 @@
 
 ### 2) The `Query` and `Cookie` helper classes
 
   </summary>
 
 Create a simple Bing Chat AI query (using the 'precise' conversation style by default) and see just the main text output rather than the whole API response:
 
+Remeber to store your cookies in a specific format: `bing_cookie_*.json`.
+  
 ```python
 from EdgeGPT import Query, Cookie
 
 q = Query("What are you? Give your answer as Python code")
 print(q)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.9 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.7.0 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -33,49 +33,54 @@
 the extension 8. Click "Export" on the bottom right, then "Export as JSON"
 (This saves your cookies to clipboard) 9. Paste your cookies into a file
 `cookies.json` ### In code: ```python cookies = json.loads(open("./path/to/
 cookies.json", encoding="utf-8").read()) bot = await Chatbot.create
 (cookies=cookies) ``` ## Running from the Command Line ``` $ python3 -m EdgeGPT
 -h EdgeGPT - A demo of reverse engineering the Bing GPT chatbot Repo:
 github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help Type !exit to
-exit Enter twice to send message or set --enter-once to send one line message
-usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [-
--style {creative,balanced,precise}] options: -h, --help show this help message
-and exit --enter-once --no-stream --rich --proxy PROXY Proxy URL (e.g. socks5:/
-/127.0.0.1:1080) --style {creative,balanced,precise} --cookie-file [path/to/
-cookies.json] ``` ## Running in Python ### 1. The `Chatbot` class and `asyncio`
-for more granular control Use Async for the best experience, for example:
-```python import asyncio from EdgeGPT import Chatbot, ConversationStyle async
-def main(): bot = await Chatbot.create() # Passing cookies is optional print
-(await bot.ask(prompt="Hello world",
-conversation_style=ConversationStyle.creative)) await bot.close() if __name__
-== "__main__": asyncio.run(main()) ```   ### 2) The `Query` and `Cookie` helper
-classes  Create a simple Bing Chat AI query (using the 'precise' conversation
-style by default) and see just the main text output rather than the whole API
-response: ```python from EdgeGPT import Query, Cookie q = Query("What are you?
-Give your answer as Python code") print(q) ``` Or change the conversation style
-or cookie file to be used: ```python q = Query( "What are you? Give your answer
-as Python code", style="creative", # or 'balanced' cookies="./
-bing_cookies_alternative.json" ) ``` Quickly extract the text output, code
-snippets, list of sources/references, or suggested follow-on questions using
-the following attributes: ```python q.output q.code q.suggestions q.sources #
-for the full json output q.sources_dict # for a dictionary of titles and urls
-``` Get the orginal prompt and the conversation style you specified: ```python
-q.prompt q.style repr(q) ``` Access previous Queries made since importing
-`Query`: ```python Query.index # A list of Query objects; updated dynamically
-Query.request_count # A tally of requests made using each cookie file ``` And
-finally, the `Cookie` class supports multiple cookie files, so if you create
-additional cookie files with the naming convention `bing_cookies_*.json`, your
-queries will automatically try using the next file (alphabetically) if you've
-exceeded your daily quota of requests (currently set at 200). Here are the main
-attributes which you can access: ```python Cookie.current_file_index
-Cookie.dirpath Cookie.search_pattern # default is `bing_cookies_*.json`
-Cookie.files() # list as files that match .search_pattern
-Cookie.current_filepath Cookie.current_data Cookie.import_next()
-Cookie.image_token Cookie.ignore_files ```  --- ## Running with Docker This
+exit usage: EdgeGPT.py [-h] [--enter-once] [--search-result] [--no-stream] [--
+rich] [--proxy PROXY] [--wss-link WSS_LINK] [--style
+{creative,balanced,precise}] [--prompt PROMPT] [--cookie-file COOKIE_FILE] [--
+history-file HISTORY_FILE] [--locale LOCALE] options: -h, --help show this help
+message and exit --enter-once --search-result --no-stream --rich --proxy PROXY
+Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-link WSS_LINK WSS URL(e.g. wss:/
+/sydney.bing.com/sydney/ChatHub) --style {creative,balanced,precise} --prompt
+PROMPT prompt to start with --cookie-file COOKIE_FILE path to cookie file --
+history-file HISTORY_FILE path to history file --locale LOCALE your locale
+(e.g. en-US, zh-CN, en-IE, en-GB) ``` (China/US/UK/Norway has enhanced support
+for locale) ## Running in Python ### 1. The `Chatbot` class and `asyncio` for
+more granular control Use Async for the best experience, for example: ```python
+import asyncio from EdgeGPT import Chatbot, ConversationStyle async def main():
+bot = await Chatbot.create() # Passing cookies is optional print(await bot.ask
+(prompt="Hello world", conversation_style=ConversationStyle.creative)) await
+bot.close() if __name__ == "__main__": asyncio.run(main()) ```   ### 2) The
+`Query` and `Cookie` helper classes  Create a simple Bing Chat AI query (using
+the 'precise' conversation style by default) and see just the main text output
+rather than the whole API response: Remeber to store your cookies in a specific
+format: `bing_cookie_*.json`. ```python from EdgeGPT import Query, Cookie q =
+Query("What are you? Give your answer as Python code") print(q) ``` Or change
+the conversation style or cookie file to be used: ```python q = Query( "What
+are you? Give your answer as Python code", style="creative", # or 'balanced'
+cookies="./bing_cookies_alternative.json" ) ``` Quickly extract the text
+output, code snippets, list of sources/references, or suggested follow-on
+questions using the following attributes: ```python q.output q.code
+q.suggestions q.sources # for the full json output q.sources_dict # for a
+dictionary of titles and urls ``` Get the orginal prompt and the conversation
+style you specified: ```python q.prompt q.style repr(q) ``` Access previous
+Queries made since importing `Query`: ```python Query.index # A list of Query
+objects; updated dynamically Query.request_count # A tally of requests made
+using each cookie file ``` And finally, the `Cookie` class supports multiple
+cookie files, so if you create additional cookie files with the naming
+convention `bing_cookies_*.json`, your queries will automatically try using the
+next file (alphabetically) if you've exceeded your daily quota of requests
+(currently set at 200). Here are the main attributes which you can access:
+```python Cookie.current_file_index Cookie.dirpath Cookie.search_pattern #
+default is `bing_cookies_*.json` Cookie.files() # list as files that match
+.search_pattern Cookie.current_filepath Cookie.current_data Cookie.import_next
+() Cookie.image_token Cookie.ignore_files ```  --- ## Running with Docker This
 assumes you have a file cookies.json in your current working directory ```bash
 docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
 cookies.json' ghcr.io/acheong08/edgegpt ``` You can add any extra flags as
 following ```bash docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -
 e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative
 ```    # Image generator  ## Running from the Command Line ```bash $ python3 -
 m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --
```

### Comparing `EdgeGPT-0.6.9/README.md` & `EdgeGPT-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -180,408 +180,442 @@
 00000b30: 0a20 2020 2020 2020 2052 6570 6f3a 2067  .        Repo: g
 00000b40: 6974 6875 622e 636f 6d2f 6163 6865 6f6e  ithub.com/acheon
 00000b50: 6730 382f 4564 6765 4750 540a 2020 2020  g08/EdgeGPT.    
 00000b60: 2020 2020 4279 3a20 416e 746f 6e69 6f20      By: Antonio 
 00000b70: 4368 656f 6e67 0a0a 2020 2020 2020 2020  Cheong..        
 00000b80: 2168 656c 7020 666f 7220 6865 6c70 0a0a  !help for help..
 00000b90: 2020 2020 2020 2020 5479 7065 2021 6578          Type !ex
-00000ba0: 6974 2074 6f20 6578 6974 0a20 2020 2020  it to exit.     
-00000bb0: 2020 2045 6e74 6572 2074 7769 6365 2074     Enter twice t
-00000bc0: 6f20 7365 6e64 206d 6573 7361 6765 206f  o send message o
-00000bd0: 7220 7365 7420 2d2d 656e 7465 722d 6f6e  r set --enter-on
-00000be0: 6365 2074 6f20 7365 6e64 206f 6e65 206c  ce to send one l
-00000bf0: 696e 6520 6d65 7373 6167 650a 0a75 7361  ine message..usa
-00000c00: 6765 3a20 4564 6765 4750 542e 7079 205b  ge: EdgeGPT.py [
-00000c10: 2d68 5d20 5b2d 2d65 6e74 6572 2d6f 6e63  -h] [--enter-onc
-00000c20: 655d 205b 2d2d 6e6f 2d73 7472 6561 6d5d  e] [--no-stream]
-00000c30: 205b 2d2d 7269 6368 5d20 5b2d 2d70 726f   [--rich] [--pro
-00000c40: 7879 2050 524f 5859 5d20 5b2d 2d73 7479  xy PROXY] [--sty
-00000c50: 6c65 207b 6372 6561 7469 7665 2c62 616c  le {creative,bal
-00000c60: 616e 6365 642c 7072 6563 6973 657d 5d0a  anced,precise}].
-00000c70: 0a6f 7074 696f 6e73 3a0a 2020 2d68 2c20  .options:.  -h, 
-00000c80: 2d2d 6865 6c70 2020 2020 2020 2020 2020  --help          
-00000c90: 2020 7368 6f77 2074 6869 7320 6865 6c70    show this help
-00000ca0: 206d 6573 7361 6765 2061 6e64 2065 7869   message and exi
-00000cb0: 740a 2020 2d2d 656e 7465 722d 6f6e 6365  t.  --enter-once
-00000cc0: 0a20 202d 2d6e 6f2d 7374 7265 616d 0a20  .  --no-stream. 
-00000cd0: 202d 2d72 6963 680a 2020 2d2d 7072 6f78   --rich.  --prox
-00000ce0: 7920 5052 4f58 5920 2020 2020 2020 2020  y PROXY         
-00000cf0: 5072 6f78 7920 5552 4c20 2865 2e67 2e20  Proxy URL (e.g. 
-00000d00: 736f 636b 7335 3a2f 2f31 3237 2e30 2e30  socks5://127.0.0
-00000d10: 2e31 3a31 3038 3029 0a20 202d 2d73 7479  .1:1080).  --sty
-00000d20: 6c65 207b 6372 6561 7469 7665 2c62 616c  le {creative,bal
-00000d30: 616e 6365 642c 7072 6563 6973 657d 0a20  anced,precise}. 
-00000d40: 202d 2d63 6f6f 6b69 652d 6669 6c65 205b   --cookie-file [
-00000d50: 7061 7468 2f74 6f2f 636f 6f6b 6965 732e  path/to/cookies.
-00000d60: 6a73 6f6e 5d0a 6060 600a 0a23 2320 5275  json].```..## Ru
-00000d70: 6e6e 696e 6720 696e 2050 7974 686f 6e0a  nning in Python.
-00000d80: 0a23 2323 2031 2e20 5468 6520 6043 6861  .### 1. The `Cha
-00000d90: 7462 6f74 6020 636c 6173 7320 616e 6420  tbot` class and 
-00000da0: 6061 7379 6e63 696f 6020 666f 7220 6d6f  `asyncio` for mo
-00000db0: 7265 2067 7261 6e75 6c61 7220 636f 6e74  re granular cont
-00000dc0: 726f 6c0a 0a55 7365 2041 7379 6e63 2066  rol..Use Async f
-00000dd0: 6f72 2074 6865 2062 6573 7420 6578 7065  or the best expe
-00000de0: 7269 656e 6365 2c20 666f 7220 6578 616d  rience, for exam
-00000df0: 706c 653a 0a0a 6060 6070 7974 686f 6e0a  ple:..```python.
-00000e00: 696d 706f 7274 2061 7379 6e63 696f 0a66  import asyncio.f
-00000e10: 726f 6d20 4564 6765 4750 5420 696d 706f  rom EdgeGPT impo
-00000e20: 7274 2043 6861 7462 6f74 2c20 436f 6e76  rt Chatbot, Conv
-00000e30: 6572 7361 7469 6f6e 5374 796c 650a 0a61  ersationStyle..a
-00000e40: 7379 6e63 2064 6566 206d 6169 6e28 293a  sync def main():
-00000e50: 0a20 2020 2062 6f74 203d 2061 7761 6974  .    bot = await
-00000e60: 2043 6861 7462 6f74 2e63 7265 6174 6528   Chatbot.create(
-00000e70: 2920 2320 5061 7373 696e 6720 636f 6f6b  ) # Passing cook
-00000e80: 6965 7320 6973 206f 7074 696f 6e61 6c0a  ies is optional.
-00000e90: 2020 2020 7072 696e 7428 6177 6169 7420      print(await 
-00000ea0: 626f 742e 6173 6b28 7072 6f6d 7074 3d22  bot.ask(prompt="
-00000eb0: 4865 6c6c 6f20 776f 726c 6422 2c20 636f  Hello world", co
-00000ec0: 6e76 6572 7361 7469 6f6e 5f73 7479 6c65  nversation_style
-00000ed0: 3d43 6f6e 7665 7273 6174 696f 6e53 7479  =ConversationSty
-00000ee0: 6c65 2e63 7265 6174 6976 6529 290a 2020  le.creative)).  
-00000ef0: 2020 6177 6169 7420 626f 742e 636c 6f73    await bot.clos
-00000f00: 6528 290a 0a69 6620 5f5f 6e61 6d65 5f5f  e()..if __name__
-00000f10: 203d 3d20 225f 5f6d 6169 6e5f 5f22 3a0a   == "__main__":.
-00000f20: 2020 2020 6173 796e 6369 6f2e 7275 6e28      asyncio.run(
-00000f30: 6d61 696e 2829 290a 6060 600a 0a3c 6465  main()).```..<de
-00000f40: 7461 696c 733e 0a3c 7375 6d6d 6172 793e  tails>.<summary>
-00000f50: 0a0a 2323 2320 3229 2054 6865 2060 5175  ..### 2) The `Qu
-00000f60: 6572 7960 2061 6e64 2060 436f 6f6b 6965  ery` and `Cookie
-00000f70: 6020 6865 6c70 6572 2063 6c61 7373 6573  ` helper classes
-00000f80: 0a0a 2020 3c2f 7375 6d6d 6172 793e 0a0a  ..  </summary>..
-00000f90: 4372 6561 7465 2061 2073 696d 706c 6520  Create a simple 
-00000fa0: 4269 6e67 2043 6861 7420 4149 2071 7565  Bing Chat AI que
-00000fb0: 7279 2028 7573 696e 6720 7468 6520 2770  ry (using the 'p
-00000fc0: 7265 6369 7365 2720 636f 6e76 6572 7361  recise' conversa
-00000fd0: 7469 6f6e 2073 7479 6c65 2062 7920 6465  tion style by de
-00000fe0: 6661 756c 7429 2061 6e64 2073 6565 206a  fault) and see j
-00000ff0: 7573 7420 7468 6520 6d61 696e 2074 6578  ust the main tex
-00001000: 7420 6f75 7470 7574 2072 6174 6865 7220  t output rather 
-00001010: 7468 616e 2074 6865 2077 686f 6c65 2041  than the whole A
-00001020: 5049 2072 6573 706f 6e73 653a 0a0a 6060  PI response:..``
-00001030: 6070 7974 686f 6e0a 6672 6f6d 2045 6467  `python.from Edg
-00001040: 6547 5054 2069 6d70 6f72 7420 5175 6572  eGPT import Quer
-00001050: 792c 2043 6f6f 6b69 650a 0a71 203d 2051  y, Cookie..q = Q
-00001060: 7565 7279 2822 5768 6174 2061 7265 2079  uery("What are y
-00001070: 6f75 3f20 4769 7665 2079 6f75 7220 616e  ou? Give your an
-00001080: 7377 6572 2061 7320 5079 7468 6f6e 2063  swer as Python c
-00001090: 6f64 6522 290a 7072 696e 7428 7129 0a60  ode").print(q).`
-000010a0: 6060 0a0a 4f72 2063 6861 6e67 6520 7468  ``..Or change th
-000010b0: 6520 636f 6e76 6572 7361 7469 6f6e 2073  e conversation s
-000010c0: 7479 6c65 206f 7220 636f 6f6b 6965 2066  tyle or cookie f
-000010d0: 696c 6520 746f 2062 6520 7573 6564 3a0a  ile to be used:.
-000010e0: 0a60 6060 7079 7468 6f6e 0a71 203d 2051  .```python.q = Q
-000010f0: 7565 7279 280a 2020 2257 6861 7420 6172  uery(.  "What ar
-00001100: 6520 796f 753f 2047 6976 6520 796f 7572  e you? Give your
-00001110: 2061 6e73 7765 7220 6173 2050 7974 686f   answer as Pytho
-00001120: 6e20 636f 6465 222c 0a20 2073 7479 6c65  n code",.  style
-00001130: 3d22 6372 6561 7469 7665 222c 2020 2320  ="creative",  # 
-00001140: 6f72 2027 6261 6c61 6e63 6564 270a 2020  or 'balanced'.  
-00001150: 636f 6f6b 6965 733d 222e 2f62 696e 675f  cookies="./bing_
-00001160: 636f 6f6b 6965 735f 616c 7465 726e 6174  cookies_alternat
-00001170: 6976 652e 6a73 6f6e 220a 290a 6060 600a  ive.json".).```.
-00001180: 0a51 7569 636b 6c79 2065 7874 7261 6374  .Quickly extract
-00001190: 2074 6865 2074 6578 7420 6f75 7470 7574   the text output
-000011a0: 2c20 636f 6465 2073 6e69 7070 6574 732c  , code snippets,
-000011b0: 206c 6973 7420 6f66 2073 6f75 7263 6573   list of sources
-000011c0: 2f72 6566 6572 656e 6365 732c 206f 7220  /references, or 
-000011d0: 7375 6767 6573 7465 6420 666f 6c6c 6f77  suggested follow
-000011e0: 2d6f 6e20 7175 6573 7469 6f6e 7320 7573  -on questions us
-000011f0: 696e 6720 7468 6520 666f 6c6c 6f77 696e  ing the followin
-00001200: 6720 6174 7472 6962 7574 6573 3a0a 0a60  g attributes:..`
-00001210: 6060 7079 7468 6f6e 0a71 2e6f 7574 7075  ``python.q.outpu
-00001220: 740a 712e 636f 6465 0a71 2e73 7567 6765  t.q.code.q.sugge
-00001230: 7374 696f 6e73 0a71 2e73 6f75 7263 6573  stions.q.sources
-00001240: 2020 2020 2020 2023 2066 6f72 2074 6865         # for the
-00001250: 2066 756c 6c20 6a73 6f6e 206f 7574 7075   full json outpu
-00001260: 740a 712e 736f 7572 6365 735f 6469 6374  t.q.sources_dict
-00001270: 2020 2320 666f 7220 6120 6469 6374 696f    # for a dictio
-00001280: 6e61 7279 206f 6620 7469 746c 6573 2061  nary of titles a
-00001290: 6e64 2075 726c 730a 6060 600a 0a47 6574  nd urls.```..Get
-000012a0: 2074 6865 206f 7267 696e 616c 2070 726f   the orginal pro
-000012b0: 6d70 7420 616e 6420 7468 6520 636f 6e76  mpt and the conv
-000012c0: 6572 7361 7469 6f6e 2073 7479 6c65 2079  ersation style y
-000012d0: 6f75 2073 7065 6369 6669 6564 3a0a 0a60  ou specified:..`
-000012e0: 6060 7079 7468 6f6e 0a71 2e70 726f 6d70  ``python.q.promp
-000012f0: 740a 712e 7374 796c 650a 7265 7072 2871  t.q.style.repr(q
-00001300: 290a 6060 600a 0a41 6363 6573 7320 7072  ).```..Access pr
-00001310: 6576 696f 7573 2051 7565 7269 6573 206d  evious Queries m
-00001320: 6164 6520 7369 6e63 6520 696d 706f 7274  ade since import
-00001330: 696e 6720 6051 7565 7279 603a 0a0a 6060  ing `Query`:..``
-00001340: 6070 7974 686f 6e0a 5175 6572 792e 696e  `python.Query.in
-00001350: 6465 7820 2023 2041 206c 6973 7420 6f66  dex  # A list of
-00001360: 2051 7565 7279 206f 626a 6563 7473 3b20   Query objects; 
-00001370: 7570 6461 7465 6420 6479 6e61 6d69 6361  updated dynamica
-00001380: 6c6c 790a 5175 6572 792e 7265 7175 6573  lly.Query.reques
-00001390: 745f 636f 756e 7420 2023 2041 2074 616c  t_count  # A tal
-000013a0: 6c79 206f 6620 7265 7175 6573 7473 206d  ly of requests m
-000013b0: 6164 6520 7573 696e 6720 6561 6368 2063  ade using each c
-000013c0: 6f6f 6b69 6520 6669 6c65 0a60 6060 0a0a  ookie file.```..
-000013d0: 416e 6420 6669 6e61 6c6c 792c 2074 6865  And finally, the
-000013e0: 2060 436f 6f6b 6965 6020 636c 6173 7320   `Cookie` class 
-000013f0: 7375 7070 6f72 7473 206d 756c 7469 706c  supports multipl
-00001400: 6520 636f 6f6b 6965 2066 696c 6573 2c20  e cookie files, 
-00001410: 736f 2069 6620 796f 7520 6372 6561 7465  so if you create
-00001420: 2061 6464 6974 696f 6e61 6c20 636f 6f6b   additional cook
-00001430: 6965 2066 696c 6573 2077 6974 6820 7468  ie files with th
-00001440: 6520 6e61 6d69 6e67 2063 6f6e 7665 6e74  e naming convent
-00001450: 696f 6e20 6062 696e 675f 636f 6f6b 6965  ion `bing_cookie
-00001460: 735f 2a2e 6a73 6f6e 602c 2079 6f75 7220  s_*.json`, your 
-00001470: 7175 6572 6965 7320 7769 6c6c 2061 7574  queries will aut
-00001480: 6f6d 6174 6963 616c 6c79 2074 7279 2075  omatically try u
-00001490: 7369 6e67 2074 6865 206e 6578 7420 6669  sing the next fi
-000014a0: 6c65 2028 616c 7068 6162 6574 6963 616c  le (alphabetical
-000014b0: 6c79 2920 6966 2079 6f75 2776 6520 6578  ly) if you've ex
-000014c0: 6365 6564 6564 2079 6f75 7220 6461 696c  ceeded your dail
-000014d0: 7920 7175 6f74 6120 6f66 2072 6571 7565  y quota of reque
-000014e0: 7374 7320 2863 7572 7265 6e74 6c79 2073  sts (currently s
-000014f0: 6574 2061 7420 3230 3029 2e0a 0a48 6572  et at 200)...Her
-00001500: 6520 6172 6520 7468 6520 6d61 696e 2061  e are the main a
-00001510: 7474 7269 6275 7465 7320 7768 6963 6820  ttributes which 
-00001520: 796f 7520 6361 6e20 6163 6365 7373 3a0a  you can access:.
-00001530: 0a60 6060 7079 7468 6f6e 0a43 6f6f 6b69  .```python.Cooki
-00001540: 652e 6375 7272 656e 745f 6669 6c65 5f69  e.current_file_i
-00001550: 6e64 6578 0a43 6f6f 6b69 652e 6469 7270  ndex.Cookie.dirp
-00001560: 6174 680a 436f 6f6b 6965 2e73 6561 7263  ath.Cookie.searc
-00001570: 685f 7061 7474 6572 6e20 2023 2064 6566  h_pattern  # def
-00001580: 6175 6c74 2069 7320 6062 696e 675f 636f  ault is `bing_co
-00001590: 6f6b 6965 735f 2a2e 6a73 6f6e 600a 436f  okies_*.json`.Co
-000015a0: 6f6b 6965 2e66 696c 6573 2829 2020 2320  okie.files()  # 
-000015b0: 6c69 7374 2061 7320 6669 6c65 7320 7468  list as files th
-000015c0: 6174 206d 6174 6368 202e 7365 6172 6368  at match .search
-000015d0: 5f70 6174 7465 726e 0a43 6f6f 6b69 652e  _pattern.Cookie.
-000015e0: 6375 7272 656e 745f 6669 6c65 7061 7468  current_filepath
-000015f0: 0a43 6f6f 6b69 652e 6375 7272 656e 745f  .Cookie.current_
-00001600: 6461 7461 0a43 6f6f 6b69 652e 696d 706f  data.Cookie.impo
-00001610: 7274 5f6e 6578 7428 290a 436f 6f6b 6965  rt_next().Cookie
-00001620: 2e69 6d61 6765 5f74 6f6b 656e 0a43 6f6f  .image_token.Coo
-00001630: 6b69 652e 6967 6e6f 7265 5f66 696c 6573  kie.ignore_files
-00001640: 0a60 6060 0a0a 3c2f 6465 7461 696c 733e  .```..</details>
-00001650: 0a0a 2d2d 2d0a 0a23 2320 5275 6e6e 696e  ..---..## Runnin
-00001660: 6720 7769 7468 2044 6f63 6b65 720a 0a54  g with Docker..T
-00001670: 6869 7320 6173 7375 6d65 7320 796f 7520  his assumes you 
-00001680: 6861 7665 2061 2066 696c 6520 636f 6f6b  have a file cook
-00001690: 6965 732e 6a73 6f6e 2069 6e20 796f 7572  ies.json in your
-000016a0: 2063 7572 7265 6e74 2077 6f72 6b69 6e67   current working
-000016b0: 2064 6972 6563 746f 7279 0a0a 6060 6062   directory..```b
-000016c0: 6173 680a 0a64 6f63 6b65 7220 7275 6e20  ash..docker run 
-000016d0: 2d2d 726d 202d 6974 202d 7620 2428 7077  --rm -it -v $(pw
-000016e0: 6429 2f63 6f6f 6b69 6573 2e6a 736f 6e3a  d)/cookies.json:
-000016f0: 2f63 6f6f 6b69 6573 2e6a 736f 6e3a 726f  /cookies.json:ro
-00001700: 202d 6520 434f 4f4b 4945 5f46 494c 453d   -e COOKIE_FILE=
-00001710: 272f 636f 6f6b 6965 732e 6a73 6f6e 2720  '/cookies.json' 
-00001720: 6768 6372 2e69 6f2f 6163 6865 6f6e 6730  ghcr.io/acheong0
-00001730: 382f 6564 6765 6770 740a 6060 600a 0a59  8/edgegpt.```..Y
-00001740: 6f75 2063 616e 2061 6464 2061 6e79 2065  ou can add any e
-00001750: 7874 7261 2066 6c61 6773 2061 7320 666f  xtra flags as fo
-00001760: 6c6c 6f77 696e 670a 0a60 6060 6261 7368  llowing..```bash
-00001770: 0a0a 646f 636b 6572 2072 756e 202d 2d72  ..docker run --r
-00001780: 6d20 2d69 7420 2d76 2024 2870 7764 292f  m -it -v $(pwd)/
-00001790: 636f 6f6b 6965 732e 6a73 6f6e 3a2f 636f  cookies.json:/co
-000017a0: 6f6b 6965 732e 6a73 6f6e 3a72 6f20 2d65  okies.json:ro -e
-000017b0: 2043 4f4f 4b49 455f 4649 4c45 3d27 2f63   COOKIE_FILE='/c
-000017c0: 6f6f 6b69 6573 2e6a 736f 6e27 2067 6863  ookies.json' ghc
-000017d0: 722e 696f 2f61 6368 656f 6e67 3038 2f65  r.io/acheong08/e
-000017e0: 6467 6567 7074 202d 2d72 6963 6820 2d2d  dgegpt --rich --
-000017f0: 7374 796c 6520 6372 6561 7469 7665 0a60  style creative.`
-00001800: 6060 0a0a 3c2f 6465 7461 696c 733e 0a0a  ``..</details>..
-00001810: 3c64 6574 6169 6c73 3e0a 0a3c 7375 6d6d  <details>..<summ
-00001820: 6172 793e 0a0a 2320 496d 6167 6520 6765  ary>..# Image ge
-00001830: 6e65 7261 746f 720a 0a3c 2f73 756d 6d61  nerator..</summa
-00001840: 7279 3e0a 0a23 2320 5275 6e6e 696e 6720  ry>..## Running 
-00001850: 6672 6f6d 2074 6865 2043 6f6d 6d61 6e64  from the Command
-00001860: 204c 696e 650a 0a60 6060 6261 7368 0a24   Line..```bash.$
-00001870: 2070 7974 686f 6e33 202d 6d20 496d 6167   python3 -m Imag
-00001880: 6547 656e 202d 680a 7573 6167 653a 2049  eGen -h.usage: I
-00001890: 6d61 6765 4765 6e2e 7079 205b 2d68 5d20  mageGen.py [-h] 
-000018a0: 5b2d 5520 555d 205b 2d2d 636f 6f6b 6965  [-U U] [--cookie
-000018b0: 2d66 696c 6520 434f 4f4b 4945 5f46 494c  -file COOKIE_FIL
-000018c0: 455d 202d 2d70 726f 6d70 7420 5052 4f4d  E] --prompt PROM
-000018d0: 5054 205b 2d2d 6f75 7470 7574 2d64 6972  PT [--output-dir
-000018e0: 204f 5554 5055 545f 4449 525d 205b 2d2d   OUTPUT_DIR] [--
-000018f0: 7175 6965 745d 205b 2d2d 6173 796e 6369  quiet] [--asynci
-00001900: 6f5d 0a0a 6f70 7469 6f6e 616c 2061 7267  o]..optional arg
-00001910: 756d 656e 7473 3a0a 2020 2d68 2c20 2d2d  uments:.  -h, --
-00001920: 6865 6c70 2020 2020 2020 2020 2020 2020  help            
-00001930: 7368 6f77 2074 6869 7320 6865 6c70 206d  show this help m
-00001940: 6573 7361 6765 2061 6e64 2065 7869 740a  essage and exit.
-00001950: 2020 2d55 2055 2020 2020 2020 2020 2020    -U U          
-00001960: 2020 2020 2020 2020 4175 7468 2063 6f6f          Auth coo
-00001970: 6b69 6520 6672 6f6d 2062 726f 7773 6572  kie from browser
-00001980: 0a20 202d 2d63 6f6f 6b69 652d 6669 6c65  .  --cookie-file
-00001990: 2043 4f4f 4b49 455f 4649 4c45 0a20 2020   COOKIE_FILE.   
-000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019b0: 2020 2020 2046 696c 6520 636f 6e74 6169       File contai
-000019c0: 6e69 6e67 2061 7574 6820 636f 6f6b 6965  ning auth cookie
-000019d0: 0a20 202d 2d70 726f 6d70 7420 5052 4f4d  .  --prompt PROM
-000019e0: 5054 2020 2020 2020 2050 726f 6d70 7420  PT       Prompt 
-000019f0: 746f 2067 656e 6572 6174 6520 696d 6167  to generate imag
-00001a00: 6573 2066 6f72 0a20 202d 2d6f 7574 7075  es for.  --outpu
-00001a10: 742d 6469 7220 4f55 5450 5554 5f44 4952  t-dir OUTPUT_DIR
-00001a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001a30: 2020 2020 2020 2020 204f 7574 7075 7420           Output 
-00001a40: 6469 7265 6374 6f72 790a 2020 2d2d 7175  directory.  --qu
-00001a50: 6965 7420 2020 2020 2020 2020 2020 2020  iet             
-00001a60: 2020 4469 7361 626c 6520 7069 7065 6c69    Disable pipeli
-00001a70: 6e65 206d 6573 7361 6765 730a 2020 2d2d  ne messages.  --
-00001a80: 6173 796e 6369 6f20 2020 2020 2020 2020  asyncio         
-00001a90: 2020 2020 5275 6e20 496d 6167 6547 656e      Run ImageGen
-00001aa0: 2075 7369 6e67 2061 7379 6e63 696f 0a60   using asyncio.`
-00001ab0: 6060 0a0a 2323 2052 756e 6e69 6e67 2069  ``..## Running i
-00001ac0: 6e20 5079 7468 6f6e 0a0a 2323 2320 3129  n Python..### 1)
-00001ad0: 2054 6865 2060 496d 6167 6551 7565 7279   The `ImageQuery
-00001ae0: 6020 6865 6c70 6572 2063 6c61 7373 0a0a  ` helper class..
-00001af0: 4765 6e65 7261 7465 2069 6d61 6765 7320  Generate images 
-00001b00: 6261 7365 6420 6f6e 2061 2073 696d 706c  based on a simpl
-00001b10: 6520 7072 6f6d 7074 2061 6e64 2064 6f77  e prompt and dow
-00001b20: 6e6c 6f61 6420 746f 2074 6865 2063 7572  nload to the cur
-00001b30: 7265 6e74 2077 6f72 6b69 6e67 2064 6972  rent working dir
-00001b40: 6563 746f 7279 3a0a 0a60 6060 7079 7468  ectory:..```pyth
-00001b50: 6f6e 0a66 726f 6d20 4564 6765 4750 5420  on.from EdgeGPT 
-00001b60: 696d 706f 7274 2049 6d61 6765 5175 6572  import ImageQuer
-00001b70: 790a 0a71 3d49 6d61 6765 5175 6572 7928  y..q=ImageQuery(
-00001b80: 224d 6565 726b 6174 7320 6174 2061 2067  "Meerkats at a g
-00001b90: 6172 6465 6e20 7061 7274 7920 696e 2044  arden party in D
-00001ba0: 6576 6f6e 2229 0a60 6060 0a0a 4368 616e  evon").```..Chan
-00001bb0: 6765 2074 6865 2064 6f77 6e6c 6f61 6420  ge the download 
-00001bc0: 6469 7265 6374 6f72 7920 666f 7220 616c  directory for al
-00001bd0: 6c20 6675 7475 7265 2069 6d61 6765 7320  l future images 
-00001be0: 696e 2074 6869 7320 7365 7373 696f 6e3a  in this session:
-00001bf0: 0a0a 6060 600a 5175 6572 792e 696d 6167  ..```.Query.imag
-00001c00: 655f 6469 7270 6174 6820 3d20 5061 7468  e_dirpath = Path
-00001c10: 2822 2e2f 746f 5f61 6e6f 7468 6572 5f66  ("./to_another_f
-00001c20: 6f6c 6465 7222 290a 6060 600a 0a23 2323  older").```..###
-00001c30: 2032 2920 5468 6520 6049 6d61 6765 4765   2) The `ImageGe
-00001c40: 6e60 2063 6c61 7373 2061 6e64 2060 6173  n` class and `as
-00001c50: 796e 6369 6f60 2066 6f72 206d 6f72 6520  yncio` for more 
-00001c60: 6772 616e 756c 6172 2063 6f6e 7472 6f6c  granular control
-00001c70: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-00001c80: 2049 6d61 6765 4765 6e20 696d 706f 7274   ImageGen import
-00001c90: 2049 6d61 6765 4765 6e0a 696d 706f 7274   ImageGen.import
-00001ca0: 2061 7267 7061 7273 650a 696d 706f 7274   argparse.import
-00001cb0: 206a 736f 6e0a 0a61 7379 6e63 2064 6566   json..async def
-00001cc0: 2061 7379 6e63 5f69 6d61 6765 5f67 656e   async_image_gen
-00001cd0: 2861 7267 7329 202d 3e20 4e6f 6e65 3a0a  (args) -> None:.
-00001ce0: 2020 2020 6173 796e 6320 7769 7468 2049      async with I
-00001cf0: 6d61 6765 4765 6e41 7379 6e63 2861 7267  mageGenAsync(arg
-00001d00: 732e 552c 2061 7267 732e 7175 6965 7429  s.U, args.quiet)
-00001d10: 2061 7320 696d 6167 655f 6765 6e65 7261   as image_genera
-00001d20: 746f 723a 0a20 2020 2020 2020 2069 6d61  tor:.        ima
-00001d30: 6765 7320 3d20 6177 6169 7420 696d 6167  ges = await imag
-00001d40: 655f 6765 6e65 7261 746f 722e 6765 745f  e_generator.get_
-00001d50: 696d 6167 6573 2861 7267 732e 7072 6f6d  images(args.prom
-00001d60: 7074 290a 2020 2020 2020 2020 6177 6169  pt).        awai
-00001d70: 7420 696d 6167 655f 6765 6e65 7261 746f  t image_generato
-00001d80: 722e 7361 7665 5f69 6d61 6765 7328 696d  r.save_images(im
-00001d90: 6167 6573 2c20 6f75 7470 7574 5f64 6972  ages, output_dir
-00001da0: 3d61 7267 732e 6f75 7470 7574 5f64 6972  =args.output_dir
-00001db0: 290a 0a69 6620 5f5f 6e61 6d65 5f5f 203d  )..if __name__ =
-00001dc0: 3d20 225f 5f6d 6169 6e5f 5f22 3a0a 2020  = "__main__":.  
-00001dd0: 2020 7061 7273 6572 203d 2061 7267 7061    parser = argpa
-00001de0: 7273 652e 4172 6775 6d65 6e74 5061 7273  rse.ArgumentPars
-00001df0: 6572 2829 0a20 2020 2070 6172 7365 722e  er().    parser.
-00001e00: 6164 645f 6172 6775 6d65 6e74 2822 2d55  add_argument("-U
-00001e10: 222c 2068 656c 703d 2241 7574 6820 636f  ", help="Auth co
-00001e20: 6f6b 6965 2066 726f 6d20 6272 6f77 7365  okie from browse
-00001e30: 7222 2c20 7479 7065 3d73 7472 290a 2020  r", type=str).  
-00001e40: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-00001e50: 756d 656e 7428 222d 2d63 6f6f 6b69 652d  ument("--cookie-
-00001e60: 6669 6c65 222c 2068 656c 703d 2246 696c  file", help="Fil
-00001e70: 6520 636f 6e74 6169 6e69 6e67 2061 7574  e containing aut
-00001e80: 6820 636f 6f6b 6965 222c 2074 7970 653d  h cookie", type=
-00001e90: 7374 7229 0a20 2020 2070 6172 7365 722e  str).    parser.
-00001ea0: 6164 645f 6172 6775 6d65 6e74 280a 2020  add_argument(.  
-00001eb0: 2020 2020 2020 222d 2d70 726f 6d70 7422        "--prompt"
-00001ec0: 2c0a 2020 2020 2020 2020 6865 6c70 3d22  ,.        help="
-00001ed0: 5072 6f6d 7074 2074 6f20 6765 6e65 7261  Prompt to genera
-00001ee0: 7465 2069 6d61 6765 7320 666f 7222 2c0a  te images for",.
-00001ef0: 2020 2020 2020 2020 7479 7065 3d73 7472          type=str
-00001f00: 2c0a 2020 2020 2020 2020 7265 7175 6972  ,.        requir
-00001f10: 6564 3d54 7275 652c 0a20 2020 2029 0a20  ed=True,.    ). 
-00001f20: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
-00001f30: 6775 6d65 6e74 280a 2020 2020 2020 2020  gument(.        
-00001f40: 222d 2d6f 7574 7075 742d 6469 7222 2c0a  "--output-dir",.
-00001f50: 2020 2020 2020 2020 6865 6c70 3d22 4f75          help="Ou
-00001f60: 7470 7574 2064 6972 6563 746f 7279 222c  tput directory",
-00001f70: 0a20 2020 2020 2020 2074 7970 653d 7374  .        type=st
-00001f80: 722c 0a20 2020 2020 2020 2064 6566 6175  r,.        defau
-00001f90: 6c74 3d22 2e2f 6f75 7470 7574 222c 0a20  lt="./output",. 
-00001fa0: 2020 2029 0a20 2020 2070 6172 7365 722e     ).    parser.
-00001fb0: 6164 645f 6172 6775 6d65 6e74 280a 2020  add_argument(.  
-00001fc0: 2020 2020 2020 222d 2d71 7569 6574 222c        "--quiet",
-00001fd0: 2068 656c 703d 2244 6973 6162 6c65 2070   help="Disable p
-00001fe0: 6970 656c 696e 6520 6d65 7373 6167 6573  ipeline messages
-00001ff0: 222c 2061 6374 696f 6e3d 2273 746f 7265  ", action="store
-00002000: 5f74 7275 6522 0a20 2020 2029 0a20 2020  _true".    ).   
-00002010: 2070 6172 7365 722e 6164 645f 6172 6775   parser.add_argu
-00002020: 6d65 6e74 280a 2020 2020 2020 2020 222d  ment(.        "-
-00002030: 2d61 7379 6e63 696f 222c 2068 656c 703d  -asyncio", help=
-00002040: 2252 756e 2049 6d61 6765 4765 6e20 7573  "Run ImageGen us
-00002050: 696e 6720 6173 796e 6369 6f22 2c20 6163  ing asyncio", ac
-00002060: 7469 6f6e 3d22 7374 6f72 655f 7472 7565  tion="store_true
-00002070: 220a 2020 2020 290a 2020 2020 6172 6773  ".    ).    args
-00002080: 203d 2070 6172 7365 722e 7061 7273 655f   = parser.parse_
-00002090: 6172 6773 2829 0a20 2020 2023 204c 6f61  args().    # Loa
-000020a0: 6420 6175 7468 2063 6f6f 6b69 650a 2020  d auth cookie.  
-000020b0: 2020 7769 7468 206f 7065 6e28 6172 6773    with open(args
-000020c0: 2e63 6f6f 6b69 655f 6669 6c65 2c20 656e  .cookie_file, en
-000020d0: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
-000020e0: 6173 2066 696c 653a 0a20 2020 2020 2020  as file:.       
-000020f0: 2063 6f6f 6b69 655f 6a73 6f6e 203d 206a   cookie_json = j
-00002100: 736f 6e2e 6c6f 6164 2866 696c 6529 0a20  son.load(file). 
-00002110: 2020 2020 2020 2066 6f72 2063 6f6f 6b69         for cooki
-00002120: 6520 696e 2063 6f6f 6b69 655f 6a73 6f6e  e in cookie_json
-00002130: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00002140: 2063 6f6f 6b69 652e 6765 7428 226e 616d   cookie.get("nam
-00002150: 6522 2920 3d3d 2022 5f55 223a 0a20 2020  e") == "_U":.   
-00002160: 2020 2020 2020 2020 2020 2020 2061 7267               arg
-00002170: 732e 5520 3d20 636f 6f6b 6965 2e67 6574  s.U = cookie.get
-00002180: 2822 7661 6c75 6522 290a 2020 2020 2020  ("value").      
-00002190: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-000021a0: 0a20 2020 2069 6620 6172 6773 2e55 2069  .    if args.U i
-000021b0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-000021c0: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
-000021d0: 2243 6f75 6c64 206e 6f74 2066 696e 6420  "Could not find 
-000021e0: 6175 7468 2063 6f6f 6b69 6522 290a 0a20  auth cookie").. 
-000021f0: 2020 2069 6620 6e6f 7420 6172 6773 2e61     if not args.a
-00002200: 7379 6e63 696f 3a0a 2020 2020 2020 2020  syncio:.        
-00002210: 2320 4372 6561 7465 2069 6d61 6765 2067  # Create image g
-00002220: 656e 6572 6174 6f72 0a20 2020 2020 2020  enerator.       
-00002230: 2069 6d61 6765 5f67 656e 6572 6174 6f72   image_generator
-00002240: 203d 2049 6d61 6765 4765 6e28 6172 6773   = ImageGen(args
-00002250: 2e55 2c20 6172 6773 2e71 7569 6574 290a  .U, args.quiet).
-00002260: 2020 2020 2020 2020 696d 6167 655f 6765          image_ge
-00002270: 6e65 7261 746f 722e 7361 7665 5f69 6d61  nerator.save_ima
-00002280: 6765 7328 0a20 2020 2020 2020 2020 2020  ges(.           
-00002290: 2069 6d61 6765 5f67 656e 6572 6174 6f72   image_generator
-000022a0: 2e67 6574 5f69 6d61 6765 7328 6172 6773  .get_images(args
-000022b0: 2e70 726f 6d70 7429 2c0a 2020 2020 2020  .prompt),.      
-000022c0: 2020 2020 2020 6f75 7470 7574 5f64 6972        output_dir
-000022d0: 3d61 7267 732e 6f75 7470 7574 5f64 6972  =args.output_dir
-000022e0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-000022f0: 656c 7365 3a0a 2020 2020 2020 2020 6173  else:.        as
-00002300: 796e 6369 6f2e 7275 6e28 6173 796e 635f  yncio.run(async_
-00002310: 696d 6167 655f 6765 6e28 6172 6773 2929  image_gen(args))
-00002320: 0a0a 6060 600a 0a3c 2f64 6574 6169 6c73  ..```..</details
-00002330: 3e0a 0a23 2053 7461 7220 4869 7374 6f72  >..# Star Histor
-00002340: 790a 0a5b 215b 5374 6172 2048 6973 746f  y..[![Star Histo
-00002350: 7279 2043 6861 7274 5d28 6874 7470 733a  ry Chart](https:
-00002360: 2f2f 6170 692e 7374 6172 2d68 6973 746f  //api.star-histo
-00002370: 7279 2e63 6f6d 2f73 7667 3f72 6570 6f73  ry.com/svg?repos
-00002380: 3d61 6368 656f 6e67 3038 2f45 6467 6547  =acheong08/EdgeG
-00002390: 5054 2674 7970 653d 4461 7465 295d 2868  PT&type=Date)](h
-000023a0: 7474 7073 3a2f 2f73 7461 722d 6869 7374  ttps://star-hist
-000023b0: 6f72 792e 636f 6d2f 2361 6368 656f 6e67  ory.com/#acheong
-000023c0: 3038 2f45 6467 6547 5054 2644 6174 6529  08/EdgeGPT&Date)
-000023d0: 0a0a 2320 436f 6e74 7269 6275 746f 7273  ..# Contributors
-000023e0: 0a0a 5468 6973 2070 726f 6a65 6374 2065  ..This project e
-000023f0: 7869 7374 7320 7468 616e 6b73 2074 6f20  xists thanks to 
-00002400: 616c 6c20 7468 6520 7065 6f70 6c65 2077  all the people w
-00002410: 686f 2063 6f6e 7472 6962 7574 652e 0a0a  ho contribute...
-00002420: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00002430: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6368  //github.com/ach
-00002440: 656f 6e67 3038 2f45 6467 6547 5054 2f67  eong08/EdgeGPT/g
-00002450: 7261 7068 732f 636f 6e74 7269 6275 746f  raphs/contributo
-00002460: 7273 223e 0a20 203c 696d 6720 7372 633d  rs">.  <img src=
-00002470: 2268 7474 7073 3a2f 2f63 6f6e 7472 6962  "https://contrib
-00002480: 2e72 6f63 6b73 2f69 6d61 6765 3f72 6570  .rocks/image?rep
-00002490: 6f3d 6163 6865 6f6e 6730 382f 4564 6765  o=acheong08/Edge
-000024a0: 4750 5422 202f 3e0a 203c 2f61 3e0a       GPT" />. </a>.
+00000ba0: 6974 2074 6f20 6578 6974 0a0a 7573 6167  it to exit..usag
+00000bb0: 653a 2045 6467 6547 5054 2e70 7920 5b2d  e: EdgeGPT.py [-
+00000bc0: 685d 205b 2d2d 656e 7465 722d 6f6e 6365  h] [--enter-once
+00000bd0: 5d20 5b2d 2d73 6561 7263 682d 7265 7375  ] [--search-resu
+00000be0: 6c74 5d20 5b2d 2d6e 6f2d 7374 7265 616d  lt] [--no-stream
+00000bf0: 5d20 5b2d 2d72 6963 685d 205b 2d2d 7072  ] [--rich] [--pr
+00000c00: 6f78 7920 5052 4f58 595d 205b 2d2d 7773  oxy PROXY] [--ws
+00000c10: 732d 6c69 6e6b 2057 5353 5f4c 494e 4b5d  s-link WSS_LINK]
+00000c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000c30: 2020 205b 2d2d 7374 796c 6520 7b63 7265     [--style {cre
+00000c40: 6174 6976 652c 6261 6c61 6e63 6564 2c70  ative,balanced,p
+00000c50: 7265 6369 7365 7d5d 205b 2d2d 7072 6f6d  recise}] [--prom
+00000c60: 7074 2050 524f 4d50 545d 205b 2d2d 636f  pt PROMPT] [--co
+00000c70: 6f6b 6965 2d66 696c 6520 434f 4f4b 4945  okie-file COOKIE
+00000c80: 5f46 494c 455d 0a20 2020 2020 2020 2020  _FILE].         
+00000c90: 2020 2020 2020 2020 205b 2d2d 6869 7374           [--hist
+00000ca0: 6f72 792d 6669 6c65 2048 4953 544f 5259  ory-file HISTORY
+00000cb0: 5f46 494c 455d 205b 2d2d 6c6f 6361 6c65  _FILE] [--locale
+00000cc0: 204c 4f43 414c 455d 0a0a 6f70 7469 6f6e   LOCALE]..option
+00000cd0: 733a 0a20 202d 682c 202d 2d68 656c 7020  s:.  -h, --help 
+00000ce0: 2020 2020 2020 2020 2020 2073 686f 7720             show 
+00000cf0: 7468 6973 2068 656c 7020 6d65 7373 6167  this help messag
+00000d00: 6520 616e 6420 6578 6974 0a20 202d 2d65  e and exit.  --e
+00000d10: 6e74 6572 2d6f 6e63 650a 2020 2d2d 7365  nter-once.  --se
+00000d20: 6172 6368 2d72 6573 756c 740a 2020 2d2d  arch-result.  --
+00000d30: 6e6f 2d73 7472 6561 6d0a 2020 2d2d 7269  no-stream.  --ri
+00000d40: 6368 0a20 202d 2d70 726f 7879 2050 524f  ch.  --proxy PRO
+00000d50: 5859 2020 2020 2020 2020 2050 726f 7879  XY         Proxy
+00000d60: 2055 524c 2028 652e 672e 2073 6f63 6b73   URL (e.g. socks
+00000d70: 353a 2f2f 3132 372e 302e 302e 313a 3130  5://127.0.0.1:10
+00000d80: 3830 290a 2020 2d2d 7773 732d 6c69 6e6b  80).  --wss-link
+00000d90: 2057 5353 5f4c 494e 4b20 2020 5753 5320   WSS_LINK   WSS 
+00000da0: 5552 4c28 652e 672e 2077 7373 3a2f 2f73  URL(e.g. wss://s
+00000db0: 7964 6e65 792e 6269 6e67 2e63 6f6d 2f73  ydney.bing.com/s
+00000dc0: 7964 6e65 792f 4368 6174 4875 6229 0a20  ydney/ChatHub). 
+00000dd0: 202d 2d73 7479 6c65 207b 6372 6561 7469   --style {creati
+00000de0: 7665 2c62 616c 616e 6365 642c 7072 6563  ve,balanced,prec
+00000df0: 6973 657d 0a20 202d 2d70 726f 6d70 7420  ise}.  --prompt 
+00000e00: 5052 4f4d 5054 2020 2020 2020 2070 726f  PROMPT       pro
+00000e10: 6d70 7420 746f 2073 7461 7274 2077 6974  mpt to start wit
+00000e20: 680a 2020 2d2d 636f 6f6b 6965 2d66 696c  h.  --cookie-fil
+00000e30: 6520 434f 4f4b 4945 5f46 494c 450a 2020  e COOKIE_FILE.  
+00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e50: 2020 2020 2020 7061 7468 2074 6f20 636f        path to co
+00000e60: 6f6b 6965 2066 696c 650a 2020 2d2d 6869  okie file.  --hi
+00000e70: 7374 6f72 792d 6669 6c65 2048 4953 544f  story-file HISTO
+00000e80: 5259 5f46 494c 450a 2020 2020 2020 2020  RY_FILE.        
+00000e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ea0: 7061 7468 2074 6f20 6869 7374 6f72 7920  path to history 
+00000eb0: 6669 6c65 0a20 202d 2d6c 6f63 616c 6520  file.  --locale 
+00000ec0: 4c4f 4341 4c45 2020 2020 2020 2079 6f75  LOCALE       you
+00000ed0: 7220 6c6f 6361 6c65 2028 652e 672e 2065  r locale (e.g. e
+00000ee0: 6e2d 5553 2c20 7a68 2d43 4e2c 2065 6e2d  n-US, zh-CN, en-
+00000ef0: 4945 2c20 656e 2d47 4229 0a60 6060 0a28  IE, en-GB).```.(
+00000f00: 4368 696e 612f 5553 2f55 4b2f 4e6f 7277  China/US/UK/Norw
+00000f10: 6179 2068 6173 2065 6e68 616e 6365 6420  ay has enhanced 
+00000f20: 7375 7070 6f72 7420 666f 7220 6c6f 6361  support for loca
+00000f30: 6c65 290a 0a23 2320 5275 6e6e 696e 6720  le)..## Running 
+00000f40: 696e 2050 7974 686f 6e0a 0a23 2323 2031  in Python..### 1
+00000f50: 2e20 5468 6520 6043 6861 7462 6f74 6020  . The `Chatbot` 
+00000f60: 636c 6173 7320 616e 6420 6061 7379 6e63  class and `async
+00000f70: 696f 6020 666f 7220 6d6f 7265 2067 7261  io` for more gra
+00000f80: 6e75 6c61 7220 636f 6e74 726f 6c0a 0a55  nular control..U
+00000f90: 7365 2041 7379 6e63 2066 6f72 2074 6865  se Async for the
+00000fa0: 2062 6573 7420 6578 7065 7269 656e 6365   best experience
+00000fb0: 2c20 666f 7220 6578 616d 706c 653a 0a0a  , for example:..
+00000fc0: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00000fd0: 2061 7379 6e63 696f 0a66 726f 6d20 4564   asyncio.from Ed
+00000fe0: 6765 4750 5420 696d 706f 7274 2043 6861  geGPT import Cha
+00000ff0: 7462 6f74 2c20 436f 6e76 6572 7361 7469  tbot, Conversati
+00001000: 6f6e 5374 796c 650a 0a61 7379 6e63 2064  onStyle..async d
+00001010: 6566 206d 6169 6e28 293a 0a20 2020 2062  ef main():.    b
+00001020: 6f74 203d 2061 7761 6974 2043 6861 7462  ot = await Chatb
+00001030: 6f74 2e63 7265 6174 6528 2920 2320 5061  ot.create() # Pa
+00001040: 7373 696e 6720 636f 6f6b 6965 7320 6973  ssing cookies is
+00001050: 206f 7074 696f 6e61 6c0a 2020 2020 7072   optional.    pr
+00001060: 696e 7428 6177 6169 7420 626f 742e 6173  int(await bot.as
+00001070: 6b28 7072 6f6d 7074 3d22 4865 6c6c 6f20  k(prompt="Hello 
+00001080: 776f 726c 6422 2c20 636f 6e76 6572 7361  world", conversa
+00001090: 7469 6f6e 5f73 7479 6c65 3d43 6f6e 7665  tion_style=Conve
+000010a0: 7273 6174 696f 6e53 7479 6c65 2e63 7265  rsationStyle.cre
+000010b0: 6174 6976 6529 290a 2020 2020 6177 6169  ative)).    awai
+000010c0: 7420 626f 742e 636c 6f73 6528 290a 0a69  t bot.close()..i
+000010d0: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 225f  f __name__ == "_
+000010e0: 5f6d 6169 6e5f 5f22 3a0a 2020 2020 6173  _main__":.    as
+000010f0: 796e 6369 6f2e 7275 6e28 6d61 696e 2829  yncio.run(main()
+00001100: 290a 6060 600a 0a3c 6465 7461 696c 733e  ).```..<details>
+00001110: 0a3c 7375 6d6d 6172 793e 0a0a 2323 2320  .<summary>..### 
+00001120: 3229 2054 6865 2060 5175 6572 7960 2061  2) The `Query` a
+00001130: 6e64 2060 436f 6f6b 6965 6020 6865 6c70  nd `Cookie` help
+00001140: 6572 2063 6c61 7373 6573 0a0a 2020 3c2f  er classes..  </
+00001150: 7375 6d6d 6172 793e 0a0a 4372 6561 7465  summary>..Create
+00001160: 2061 2073 696d 706c 6520 4269 6e67 2043   a simple Bing C
+00001170: 6861 7420 4149 2071 7565 7279 2028 7573  hat AI query (us
+00001180: 696e 6720 7468 6520 2770 7265 6369 7365  ing the 'precise
+00001190: 2720 636f 6e76 6572 7361 7469 6f6e 2073  ' conversation s
+000011a0: 7479 6c65 2062 7920 6465 6661 756c 7429  tyle by default)
+000011b0: 2061 6e64 2073 6565 206a 7573 7420 7468   and see just th
+000011c0: 6520 6d61 696e 2074 6578 7420 6f75 7470  e main text outp
+000011d0: 7574 2072 6174 6865 7220 7468 616e 2074  ut rather than t
+000011e0: 6865 2077 686f 6c65 2041 5049 2072 6573  he whole API res
+000011f0: 706f 6e73 653a 0a0a 5265 6d65 6265 7220  ponse:..Remeber 
+00001200: 746f 2073 746f 7265 2079 6f75 7220 636f  to store your co
+00001210: 6f6b 6965 7320 696e 2061 2073 7065 6369  okies in a speci
+00001220: 6669 6320 666f 726d 6174 3a20 6062 696e  fic format: `bin
+00001230: 675f 636f 6f6b 6965 5f2a 2e6a 736f 6e60  g_cookie_*.json`
+00001240: 2e0a 2020 0a60 6060 7079 7468 6f6e 0a66  ..  .```python.f
+00001250: 726f 6d20 4564 6765 4750 5420 696d 706f  rom EdgeGPT impo
+00001260: 7274 2051 7565 7279 2c20 436f 6f6b 6965  rt Query, Cookie
+00001270: 0a0a 7120 3d20 5175 6572 7928 2257 6861  ..q = Query("Wha
+00001280: 7420 6172 6520 796f 753f 2047 6976 6520  t are you? Give 
+00001290: 796f 7572 2061 6e73 7765 7220 6173 2050  your answer as P
+000012a0: 7974 686f 6e20 636f 6465 2229 0a70 7269  ython code").pri
+000012b0: 6e74 2871 290a 6060 600a 0a4f 7220 6368  nt(q).```..Or ch
+000012c0: 616e 6765 2074 6865 2063 6f6e 7665 7273  ange the convers
+000012d0: 6174 696f 6e20 7374 796c 6520 6f72 2063  ation style or c
+000012e0: 6f6f 6b69 6520 6669 6c65 2074 6f20 6265  ookie file to be
+000012f0: 2075 7365 643a 0a0a 6060 6070 7974 686f   used:..```pytho
+00001300: 6e0a 7120 3d20 5175 6572 7928 0a20 2022  n.q = Query(.  "
+00001310: 5768 6174 2061 7265 2079 6f75 3f20 4769  What are you? Gi
+00001320: 7665 2079 6f75 7220 616e 7377 6572 2061  ve your answer a
+00001330: 7320 5079 7468 6f6e 2063 6f64 6522 2c0a  s Python code",.
+00001340: 2020 7374 796c 653d 2263 7265 6174 6976    style="creativ
+00001350: 6522 2c20 2023 206f 7220 2762 616c 616e  e",  # or 'balan
+00001360: 6365 6427 0a20 2063 6f6f 6b69 6573 3d22  ced'.  cookies="
+00001370: 2e2f 6269 6e67 5f63 6f6f 6b69 6573 5f61  ./bing_cookies_a
+00001380: 6c74 6572 6e61 7469 7665 2e6a 736f 6e22  lternative.json"
+00001390: 0a29 0a60 6060 0a0a 5175 6963 6b6c 7920  .).```..Quickly 
+000013a0: 6578 7472 6163 7420 7468 6520 7465 7874  extract the text
+000013b0: 206f 7574 7075 742c 2063 6f64 6520 736e   output, code sn
+000013c0: 6970 7065 7473 2c20 6c69 7374 206f 6620  ippets, list of 
+000013d0: 736f 7572 6365 732f 7265 6665 7265 6e63  sources/referenc
+000013e0: 6573 2c20 6f72 2073 7567 6765 7374 6564  es, or suggested
+000013f0: 2066 6f6c 6c6f 772d 6f6e 2071 7565 7374   follow-on quest
+00001400: 696f 6e73 2075 7369 6e67 2074 6865 2066  ions using the f
+00001410: 6f6c 6c6f 7769 6e67 2061 7474 7269 6275  ollowing attribu
+00001420: 7465 733a 0a0a 6060 6070 7974 686f 6e0a  tes:..```python.
+00001430: 712e 6f75 7470 7574 0a71 2e63 6f64 650a  q.output.q.code.
+00001440: 712e 7375 6767 6573 7469 6f6e 730a 712e  q.suggestions.q.
+00001450: 736f 7572 6365 7320 2020 2020 2020 2320  sources       # 
+00001460: 666f 7220 7468 6520 6675 6c6c 206a 736f  for the full jso
+00001470: 6e20 6f75 7470 7574 0a71 2e73 6f75 7263  n output.q.sourc
+00001480: 6573 5f64 6963 7420 2023 2066 6f72 2061  es_dict  # for a
+00001490: 2064 6963 7469 6f6e 6172 7920 6f66 2074   dictionary of t
+000014a0: 6974 6c65 7320 616e 6420 7572 6c73 0a60  itles and urls.`
+000014b0: 6060 0a0a 4765 7420 7468 6520 6f72 6769  ``..Get the orgi
+000014c0: 6e61 6c20 7072 6f6d 7074 2061 6e64 2074  nal prompt and t
+000014d0: 6865 2063 6f6e 7665 7273 6174 696f 6e20  he conversation 
+000014e0: 7374 796c 6520 796f 7520 7370 6563 6966  style you specif
+000014f0: 6965 643a 0a0a 6060 6070 7974 686f 6e0a  ied:..```python.
+00001500: 712e 7072 6f6d 7074 0a71 2e73 7479 6c65  q.prompt.q.style
+00001510: 0a72 6570 7228 7129 0a60 6060 0a0a 4163  .repr(q).```..Ac
+00001520: 6365 7373 2070 7265 7669 6f75 7320 5175  cess previous Qu
+00001530: 6572 6965 7320 6d61 6465 2073 696e 6365  eries made since
+00001540: 2069 6d70 6f72 7469 6e67 2060 5175 6572   importing `Quer
+00001550: 7960 3a0a 0a60 6060 7079 7468 6f6e 0a51  y`:..```python.Q
+00001560: 7565 7279 2e69 6e64 6578 2020 2320 4120  uery.index  # A 
+00001570: 6c69 7374 206f 6620 5175 6572 7920 6f62  list of Query ob
+00001580: 6a65 6374 733b 2075 7064 6174 6564 2064  jects; updated d
+00001590: 796e 616d 6963 616c 6c79 0a51 7565 7279  ynamically.Query
+000015a0: 2e72 6571 7565 7374 5f63 6f75 6e74 2020  .request_count  
+000015b0: 2320 4120 7461 6c6c 7920 6f66 2072 6571  # A tally of req
+000015c0: 7565 7374 7320 6d61 6465 2075 7369 6e67  uests made using
+000015d0: 2065 6163 6820 636f 6f6b 6965 2066 696c   each cookie fil
+000015e0: 650a 6060 600a 0a41 6e64 2066 696e 616c  e.```..And final
+000015f0: 6c79 2c20 7468 6520 6043 6f6f 6b69 6560  ly, the `Cookie`
+00001600: 2063 6c61 7373 2073 7570 706f 7274 7320   class supports 
+00001610: 6d75 6c74 6970 6c65 2063 6f6f 6b69 6520  multiple cookie 
+00001620: 6669 6c65 732c 2073 6f20 6966 2079 6f75  files, so if you
+00001630: 2063 7265 6174 6520 6164 6469 7469 6f6e   create addition
+00001640: 616c 2063 6f6f 6b69 6520 6669 6c65 7320  al cookie files 
+00001650: 7769 7468 2074 6865 206e 616d 696e 6720  with the naming 
+00001660: 636f 6e76 656e 7469 6f6e 2060 6269 6e67  convention `bing
+00001670: 5f63 6f6f 6b69 6573 5f2a 2e6a 736f 6e60  _cookies_*.json`
+00001680: 2c20 796f 7572 2071 7565 7269 6573 2077  , your queries w
+00001690: 696c 6c20 6175 746f 6d61 7469 6361 6c6c  ill automaticall
+000016a0: 7920 7472 7920 7573 696e 6720 7468 6520  y try using the 
+000016b0: 6e65 7874 2066 696c 6520 2861 6c70 6861  next file (alpha
+000016c0: 6265 7469 6361 6c6c 7929 2069 6620 796f  betically) if yo
+000016d0: 7527 7665 2065 7863 6565 6465 6420 796f  u've exceeded yo
+000016e0: 7572 2064 6169 6c79 2071 756f 7461 206f  ur daily quota o
+000016f0: 6620 7265 7175 6573 7473 2028 6375 7272  f requests (curr
+00001700: 656e 746c 7920 7365 7420 6174 2032 3030  ently set at 200
+00001710: 292e 0a0a 4865 7265 2061 7265 2074 6865  )...Here are the
+00001720: 206d 6169 6e20 6174 7472 6962 7574 6573   main attributes
+00001730: 2077 6869 6368 2079 6f75 2063 616e 2061   which you can a
+00001740: 6363 6573 733a 0a0a 6060 6070 7974 686f  ccess:..```pytho
+00001750: 6e0a 436f 6f6b 6965 2e63 7572 7265 6e74  n.Cookie.current
+00001760: 5f66 696c 655f 696e 6465 780a 436f 6f6b  _file_index.Cook
+00001770: 6965 2e64 6972 7061 7468 0a43 6f6f 6b69  ie.dirpath.Cooki
+00001780: 652e 7365 6172 6368 5f70 6174 7465 726e  e.search_pattern
+00001790: 2020 2320 6465 6661 756c 7420 6973 2060    # default is `
+000017a0: 6269 6e67 5f63 6f6f 6b69 6573 5f2a 2e6a  bing_cookies_*.j
+000017b0: 736f 6e60 0a43 6f6f 6b69 652e 6669 6c65  son`.Cookie.file
+000017c0: 7328 2920 2023 206c 6973 7420 6173 2066  s()  # list as f
+000017d0: 696c 6573 2074 6861 7420 6d61 7463 6820  iles that match 
+000017e0: 2e73 6561 7263 685f 7061 7474 6572 6e0a  .search_pattern.
+000017f0: 436f 6f6b 6965 2e63 7572 7265 6e74 5f66  Cookie.current_f
+00001800: 696c 6570 6174 680a 436f 6f6b 6965 2e63  ilepath.Cookie.c
+00001810: 7572 7265 6e74 5f64 6174 610a 436f 6f6b  urrent_data.Cook
+00001820: 6965 2e69 6d70 6f72 745f 6e65 7874 2829  ie.import_next()
+00001830: 0a43 6f6f 6b69 652e 696d 6167 655f 746f  .Cookie.image_to
+00001840: 6b65 6e0a 436f 6f6b 6965 2e69 676e 6f72  ken.Cookie.ignor
+00001850: 655f 6669 6c65 730a 6060 600a 0a3c 2f64  e_files.```..</d
+00001860: 6574 6169 6c73 3e0a 0a2d 2d2d 0a0a 2323  etails>..---..##
+00001870: 2052 756e 6e69 6e67 2077 6974 6820 446f   Running with Do
+00001880: 636b 6572 0a0a 5468 6973 2061 7373 756d  cker..This assum
+00001890: 6573 2079 6f75 2068 6176 6520 6120 6669  es you have a fi
+000018a0: 6c65 2063 6f6f 6b69 6573 2e6a 736f 6e20  le cookies.json 
+000018b0: 696e 2079 6f75 7220 6375 7272 656e 7420  in your current 
+000018c0: 776f 726b 696e 6720 6469 7265 6374 6f72  working director
+000018d0: 790a 0a60 6060 6261 7368 0a0a 646f 636b  y..```bash..dock
+000018e0: 6572 2072 756e 202d 2d72 6d20 2d69 7420  er run --rm -it 
+000018f0: 2d76 2024 2870 7764 292f 636f 6f6b 6965  -v $(pwd)/cookie
+00001900: 732e 6a73 6f6e 3a2f 636f 6f6b 6965 732e  s.json:/cookies.
+00001910: 6a73 6f6e 3a72 6f20 2d65 2043 4f4f 4b49  json:ro -e COOKI
+00001920: 455f 4649 4c45 3d27 2f63 6f6f 6b69 6573  E_FILE='/cookies
+00001930: 2e6a 736f 6e27 2067 6863 722e 696f 2f61  .json' ghcr.io/a
+00001940: 6368 656f 6e67 3038 2f65 6467 6567 7074  cheong08/edgegpt
+00001950: 0a60 6060 0a0a 596f 7520 6361 6e20 6164  .```..You can ad
+00001960: 6420 616e 7920 6578 7472 6120 666c 6167  d any extra flag
+00001970: 7320 6173 2066 6f6c 6c6f 7769 6e67 0a0a  s as following..
+00001980: 6060 6062 6173 680a 0a64 6f63 6b65 7220  ```bash..docker 
+00001990: 7275 6e20 2d2d 726d 202d 6974 202d 7620  run --rm -it -v 
+000019a0: 2428 7077 6429 2f63 6f6f 6b69 6573 2e6a  $(pwd)/cookies.j
+000019b0: 736f 6e3a 2f63 6f6f 6b69 6573 2e6a 736f  son:/cookies.jso
+000019c0: 6e3a 726f 202d 6520 434f 4f4b 4945 5f46  n:ro -e COOKIE_F
+000019d0: 494c 453d 272f 636f 6f6b 6965 732e 6a73  ILE='/cookies.js
+000019e0: 6f6e 2720 6768 6372 2e69 6f2f 6163 6865  on' ghcr.io/ache
+000019f0: 6f6e 6730 382f 6564 6765 6770 7420 2d2d  ong08/edgegpt --
+00001a00: 7269 6368 202d 2d73 7479 6c65 2063 7265  rich --style cre
+00001a10: 6174 6976 650a 6060 600a 0a3c 2f64 6574  ative.```..</det
+00001a20: 6169 6c73 3e0a 0a3c 6465 7461 696c 733e  ails>..<details>
+00001a30: 0a0a 3c73 756d 6d61 7279 3e0a 0a23 2049  ..<summary>..# I
+00001a40: 6d61 6765 2067 656e 6572 6174 6f72 0a0a  mage generator..
+00001a50: 3c2f 7375 6d6d 6172 793e 0a0a 2323 2052  </summary>..## R
+00001a60: 756e 6e69 6e67 2066 726f 6d20 7468 6520  unning from the 
+00001a70: 436f 6d6d 616e 6420 4c69 6e65 0a0a 6060  Command Line..``
+00001a80: 6062 6173 680a 2420 7079 7468 6f6e 3320  `bash.$ python3 
+00001a90: 2d6d 2049 6d61 6765 4765 6e20 2d68 0a75  -m ImageGen -h.u
+00001aa0: 7361 6765 3a20 496d 6167 6547 656e 2e70  sage: ImageGen.p
+00001ab0: 7920 5b2d 685d 205b 2d55 2055 5d20 5b2d  y [-h] [-U U] [-
+00001ac0: 2d63 6f6f 6b69 652d 6669 6c65 2043 4f4f  -cookie-file COO
+00001ad0: 4b49 455f 4649 4c45 5d20 2d2d 7072 6f6d  KIE_FILE] --prom
+00001ae0: 7074 2050 524f 4d50 5420 5b2d 2d6f 7574  pt PROMPT [--out
+00001af0: 7075 742d 6469 7220 4f55 5450 5554 5f44  put-dir OUTPUT_D
+00001b00: 4952 5d20 5b2d 2d71 7569 6574 5d20 5b2d  IR] [--quiet] [-
+00001b10: 2d61 7379 6e63 696f 5d0a 0a6f 7074 696f  -asyncio]..optio
+00001b20: 6e61 6c20 6172 6775 6d65 6e74 733a 0a20  nal arguments:. 
+00001b30: 202d 682c 202d 2d68 656c 7020 2020 2020   -h, --help     
+00001b40: 2020 2020 2020 2073 686f 7720 7468 6973         show this
+00001b50: 2068 656c 7020 6d65 7373 6167 6520 616e   help message an
+00001b60: 6420 6578 6974 0a20 202d 5520 5520 2020  d exit.  -U U   
+00001b70: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+00001b80: 7574 6820 636f 6f6b 6965 2066 726f 6d20  uth cookie from 
+00001b90: 6272 6f77 7365 720a 2020 2d2d 636f 6f6b  browser.  --cook
+00001ba0: 6965 2d66 696c 6520 434f 4f4b 4945 5f46  ie-file COOKIE_F
+00001bb0: 494c 450a 2020 2020 2020 2020 2020 2020  ILE.            
+00001bc0: 2020 2020 2020 2020 2020 2020 4669 6c65              File
+00001bd0: 2063 6f6e 7461 696e 696e 6720 6175 7468   containing auth
+00001be0: 2063 6f6f 6b69 650a 2020 2d2d 7072 6f6d   cookie.  --prom
+00001bf0: 7074 2050 524f 4d50 5420 2020 2020 2020  pt PROMPT       
+00001c00: 5072 6f6d 7074 2074 6f20 6765 6e65 7261  Prompt to genera
+00001c10: 7465 2069 6d61 6765 7320 666f 720a 2020  te images for.  
+00001c20: 2d2d 6f75 7470 7574 2d64 6972 204f 5554  --output-dir OUT
+00001c30: 5055 545f 4449 520a 2020 2020 2020 2020  PUT_DIR.        
+00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c50: 4f75 7470 7574 2064 6972 6563 746f 7279  Output directory
+00001c60: 0a20 202d 2d71 7569 6574 2020 2020 2020  .  --quiet      
+00001c70: 2020 2020 2020 2020 2044 6973 6162 6c65           Disable
+00001c80: 2070 6970 656c 696e 6520 6d65 7373 6167   pipeline messag
+00001c90: 6573 0a20 202d 2d61 7379 6e63 696f 2020  es.  --asyncio  
+00001ca0: 2020 2020 2020 2020 2020 2052 756e 2049             Run I
+00001cb0: 6d61 6765 4765 6e20 7573 696e 6720 6173  mageGen using as
+00001cc0: 796e 6369 6f0a 6060 600a 0a23 2320 5275  yncio.```..## Ru
+00001cd0: 6e6e 696e 6720 696e 2050 7974 686f 6e0a  nning in Python.
+00001ce0: 0a23 2323 2031 2920 5468 6520 6049 6d61  .### 1) The `Ima
+00001cf0: 6765 5175 6572 7960 2068 656c 7065 7220  geQuery` helper 
+00001d00: 636c 6173 730a 0a47 656e 6572 6174 6520  class..Generate 
+00001d10: 696d 6167 6573 2062 6173 6564 206f 6e20  images based on 
+00001d20: 6120 7369 6d70 6c65 2070 726f 6d70 7420  a simple prompt 
+00001d30: 616e 6420 646f 776e 6c6f 6164 2074 6f20  and download to 
+00001d40: 7468 6520 6375 7272 656e 7420 776f 726b  the current work
+00001d50: 696e 6720 6469 7265 6374 6f72 793a 0a0a  ing directory:..
+00001d60: 6060 6070 7974 686f 6e0a 6672 6f6d 2045  ```python.from E
+00001d70: 6467 6547 5054 2069 6d70 6f72 7420 496d  dgeGPT import Im
+00001d80: 6167 6551 7565 7279 0a0a 713d 496d 6167  ageQuery..q=Imag
+00001d90: 6551 7565 7279 2822 4d65 6572 6b61 7473  eQuery("Meerkats
+00001da0: 2061 7420 6120 6761 7264 656e 2070 6172   at a garden par
+00001db0: 7479 2069 6e20 4465 766f 6e22 290a 6060  ty in Devon").``
+00001dc0: 600a 0a43 6861 6e67 6520 7468 6520 646f  `..Change the do
+00001dd0: 776e 6c6f 6164 2064 6972 6563 746f 7279  wnload directory
+00001de0: 2066 6f72 2061 6c6c 2066 7574 7572 6520   for all future 
+00001df0: 696d 6167 6573 2069 6e20 7468 6973 2073  images in this s
+00001e00: 6573 7369 6f6e 3a0a 0a60 6060 0a51 7565  ession:..```.Que
+00001e10: 7279 2e69 6d61 6765 5f64 6972 7061 7468  ry.image_dirpath
+00001e20: 203d 2050 6174 6828 222e 2f74 6f5f 616e   = Path("./to_an
+00001e30: 6f74 6865 725f 666f 6c64 6572 2229 0a60  other_folder").`
+00001e40: 6060 0a0a 2323 2320 3229 2054 6865 2060  ``..### 2) The `
+00001e50: 496d 6167 6547 656e 6020 636c 6173 7320  ImageGen` class 
+00001e60: 616e 6420 6061 7379 6e63 696f 6020 666f  and `asyncio` fo
+00001e70: 7220 6d6f 7265 2067 7261 6e75 6c61 7220  r more granular 
+00001e80: 636f 6e74 726f 6c0a 0a60 6060 7079 7468  control..```pyth
+00001e90: 6f6e 0a66 726f 6d20 496d 6167 6547 656e  on.from ImageGen
+00001ea0: 2069 6d70 6f72 7420 496d 6167 6547 656e   import ImageGen
+00001eb0: 0a69 6d70 6f72 7420 6172 6770 6172 7365  .import argparse
+00001ec0: 0a69 6d70 6f72 7420 6a73 6f6e 0a0a 6173  .import json..as
+00001ed0: 796e 6320 6465 6620 6173 796e 635f 696d  ync def async_im
+00001ee0: 6167 655f 6765 6e28 6172 6773 2920 2d3e  age_gen(args) ->
+00001ef0: 204e 6f6e 653a 0a20 2020 2061 7379 6e63   None:.    async
+00001f00: 2077 6974 6820 496d 6167 6547 656e 4173   with ImageGenAs
+00001f10: 796e 6328 6172 6773 2e55 2c20 6172 6773  ync(args.U, args
+00001f20: 2e71 7569 6574 2920 6173 2069 6d61 6765  .quiet) as image
+00001f30: 5f67 656e 6572 6174 6f72 3a0a 2020 2020  _generator:.    
+00001f40: 2020 2020 696d 6167 6573 203d 2061 7761      images = awa
+00001f50: 6974 2069 6d61 6765 5f67 656e 6572 6174  it image_generat
+00001f60: 6f72 2e67 6574 5f69 6d61 6765 7328 6172  or.get_images(ar
+00001f70: 6773 2e70 726f 6d70 7429 0a20 2020 2020  gs.prompt).     
+00001f80: 2020 2061 7761 6974 2069 6d61 6765 5f67     await image_g
+00001f90: 656e 6572 6174 6f72 2e73 6176 655f 696d  enerator.save_im
+00001fa0: 6167 6573 2869 6d61 6765 732c 206f 7574  ages(images, out
+00001fb0: 7075 745f 6469 723d 6172 6773 2e6f 7574  put_dir=args.out
+00001fc0: 7075 745f 6469 7229 0a0a 6966 205f 5f6e  put_dir)..if __n
+00001fd0: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
+00001fe0: 5f5f 223a 0a20 2020 2070 6172 7365 7220  __":.    parser 
+00001ff0: 3d20 6172 6770 6172 7365 2e41 7267 756d  = argparse.Argum
+00002000: 656e 7450 6172 7365 7228 290a 2020 2020  entParser().    
+00002010: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
+00002020: 656e 7428 222d 5522 2c20 6865 6c70 3d22  ent("-U", help="
+00002030: 4175 7468 2063 6f6f 6b69 6520 6672 6f6d  Auth cookie from
+00002040: 2062 726f 7773 6572 222c 2074 7970 653d   browser", type=
+00002050: 7374 7229 0a20 2020 2070 6172 7365 722e  str).    parser.
+00002060: 6164 645f 6172 6775 6d65 6e74 2822 2d2d  add_argument("--
+00002070: 636f 6f6b 6965 2d66 696c 6522 2c20 6865  cookie-file", he
+00002080: 6c70 3d22 4669 6c65 2063 6f6e 7461 696e  lp="File contain
+00002090: 696e 6720 6175 7468 2063 6f6f 6b69 6522  ing auth cookie"
+000020a0: 2c20 7479 7065 3d73 7472 290a 2020 2020  , type=str).    
+000020b0: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
+000020c0: 656e 7428 0a20 2020 2020 2020 2022 2d2d  ent(.        "--
+000020d0: 7072 6f6d 7074 222c 0a20 2020 2020 2020  prompt",.       
+000020e0: 2068 656c 703d 2250 726f 6d70 7420 746f   help="Prompt to
+000020f0: 2067 656e 6572 6174 6520 696d 6167 6573   generate images
+00002100: 2066 6f72 222c 0a20 2020 2020 2020 2074   for",.        t
+00002110: 7970 653d 7374 722c 0a20 2020 2020 2020  ype=str,.       
+00002120: 2072 6571 7569 7265 643d 5472 7565 2c0a   required=True,.
+00002130: 2020 2020 290a 2020 2020 7061 7273 6572      ).    parser
+00002140: 2e61 6464 5f61 7267 756d 656e 7428 0a20  .add_argument(. 
+00002150: 2020 2020 2020 2022 2d2d 6f75 7470 7574         "--output
+00002160: 2d64 6972 222c 0a20 2020 2020 2020 2068  -dir",.        h
+00002170: 656c 703d 224f 7574 7075 7420 6469 7265  elp="Output dire
+00002180: 6374 6f72 7922 2c0a 2020 2020 2020 2020  ctory",.        
+00002190: 7479 7065 3d73 7472 2c0a 2020 2020 2020  type=str,.      
+000021a0: 2020 6465 6661 756c 743d 222e 2f6f 7574    default="./out
+000021b0: 7075 7422 2c0a 2020 2020 290a 2020 2020  put",.    ).    
+000021c0: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
+000021d0: 656e 7428 0a20 2020 2020 2020 2022 2d2d  ent(.        "--
+000021e0: 7175 6965 7422 2c20 6865 6c70 3d22 4469  quiet", help="Di
+000021f0: 7361 626c 6520 7069 7065 6c69 6e65 206d  sable pipeline m
+00002200: 6573 7361 6765 7322 2c20 6163 7469 6f6e  essages", action
+00002210: 3d22 7374 6f72 655f 7472 7565 220a 2020  ="store_true".  
+00002220: 2020 290a 2020 2020 7061 7273 6572 2e61    ).    parser.a
+00002230: 6464 5f61 7267 756d 656e 7428 0a20 2020  dd_argument(.   
+00002240: 2020 2020 2022 2d2d 6173 796e 6369 6f22       "--asyncio"
+00002250: 2c20 6865 6c70 3d22 5275 6e20 496d 6167  , help="Run Imag
+00002260: 6547 656e 2075 7369 6e67 2061 7379 6e63  eGen using async
+00002270: 696f 222c 2061 6374 696f 6e3d 2273 746f  io", action="sto
+00002280: 7265 5f74 7275 6522 0a20 2020 2029 0a20  re_true".    ). 
+00002290: 2020 2061 7267 7320 3d20 7061 7273 6572     args = parser
+000022a0: 2e70 6172 7365 5f61 7267 7328 290a 2020  .parse_args().  
+000022b0: 2020 2320 4c6f 6164 2061 7574 6820 636f    # Load auth co
+000022c0: 6f6b 6965 0a20 2020 2077 6974 6820 6f70  okie.    with op
+000022d0: 656e 2861 7267 732e 636f 6f6b 6965 5f66  en(args.cookie_f
+000022e0: 696c 652c 2065 6e63 6f64 696e 673d 2275  ile, encoding="u
+000022f0: 7466 2d38 2229 2061 7320 6669 6c65 3a0a  tf-8") as file:.
+00002300: 2020 2020 2020 2020 636f 6f6b 6965 5f6a          cookie_j
+00002310: 736f 6e20 3d20 6a73 6f6e 2e6c 6f61 6428  son = json.load(
+00002320: 6669 6c65 290a 2020 2020 2020 2020 666f  file).        fo
+00002330: 7220 636f 6f6b 6965 2069 6e20 636f 6f6b  r cookie in cook
+00002340: 6965 5f6a 736f 6e3a 0a20 2020 2020 2020  ie_json:.       
+00002350: 2020 2020 2069 6620 636f 6f6b 6965 2e67       if cookie.g
+00002360: 6574 2822 6e61 6d65 2229 203d 3d20 225f  et("name") == "_
+00002370: 5522 3a0a 2020 2020 2020 2020 2020 2020  U":.            
+00002380: 2020 2020 6172 6773 2e55 203d 2063 6f6f      args.U = coo
+00002390: 6b69 652e 6765 7428 2276 616c 7565 2229  kie.get("value")
+000023a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000023b0: 2062 7265 616b 0a0a 2020 2020 6966 2061   break..    if a
+000023c0: 7267 732e 5520 6973 204e 6f6e 653a 0a20  rgs.U is None:. 
+000023d0: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
+000023e0: 6570 7469 6f6e 2822 436f 756c 6420 6e6f  eption("Could no
+000023f0: 7420 6669 6e64 2061 7574 6820 636f 6f6b  t find auth cook
+00002400: 6965 2229 0a0a 2020 2020 6966 206e 6f74  ie")..    if not
+00002410: 2061 7267 732e 6173 796e 6369 6f3a 0a20   args.asyncio:. 
+00002420: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
+00002430: 696d 6167 6520 6765 6e65 7261 746f 720a  image generator.
+00002440: 2020 2020 2020 2020 696d 6167 655f 6765          image_ge
+00002450: 6e65 7261 746f 7220 3d20 496d 6167 6547  nerator = ImageG
+00002460: 656e 2861 7267 732e 552c 2061 7267 732e  en(args.U, args.
+00002470: 7175 6965 7429 0a20 2020 2020 2020 2069  quiet).        i
+00002480: 6d61 6765 5f67 656e 6572 6174 6f72 2e73  mage_generator.s
+00002490: 6176 655f 696d 6167 6573 280a 2020 2020  ave_images(.    
+000024a0: 2020 2020 2020 2020 696d 6167 655f 6765          image_ge
+000024b0: 6e65 7261 746f 722e 6765 745f 696d 6167  nerator.get_imag
+000024c0: 6573 2861 7267 732e 7072 6f6d 7074 292c  es(args.prompt),
+000024d0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+000024e0: 7075 745f 6469 723d 6172 6773 2e6f 7574  put_dir=args.out
+000024f0: 7075 745f 6469 722c 0a20 2020 2020 2020  put_dir,.       
+00002500: 2029 0a20 2020 2065 6c73 653a 0a20 2020   ).    else:.   
+00002510: 2020 2020 2061 7379 6e63 696f 2e72 756e       asyncio.run
+00002520: 2861 7379 6e63 5f69 6d61 6765 5f67 656e  (async_image_gen
+00002530: 2861 7267 7329 290a 0a60 6060 0a0a 3c2f  (args))..```..</
+00002540: 6465 7461 696c 733e 0a0a 2320 5374 6172  details>..# Star
+00002550: 2048 6973 746f 7279 0a0a 5b21 5b53 7461   History..[![Sta
+00002560: 7220 4869 7374 6f72 7920 4368 6172 745d  r History Chart]
+00002570: 2868 7474 7073 3a2f 2f61 7069 2e73 7461  (https://api.sta
+00002580: 722d 6869 7374 6f72 792e 636f 6d2f 7376  r-history.com/sv
+00002590: 673f 7265 706f 733d 6163 6865 6f6e 6730  g?repos=acheong0
+000025a0: 382f 4564 6765 4750 5426 7479 7065 3d44  8/EdgeGPT&type=D
+000025b0: 6174 6529 5d28 6874 7470 733a 2f2f 7374  ate)](https://st
+000025c0: 6172 2d68 6973 746f 7279 2e63 6f6d 2f23  ar-history.com/#
+000025d0: 6163 6865 6f6e 6730 382f 4564 6765 4750  acheong08/EdgeGP
+000025e0: 5426 4461 7465 290a 0a23 2043 6f6e 7472  T&Date)..# Contr
+000025f0: 6962 7574 6f72 730a 0a54 6869 7320 7072  ibutors..This pr
+00002600: 6f6a 6563 7420 6578 6973 7473 2074 6861  oject exists tha
+00002610: 6e6b 7320 746f 2061 6c6c 2074 6865 2070  nks to all the p
+00002620: 656f 706c 6520 7768 6f20 636f 6e74 7269  eople who contri
+00002630: 6275 7465 2e0a 0a20 3c61 2068 7265 663d  bute... <a href=
+00002640: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00002650: 636f 6d2f 6163 6865 6f6e 6730 382f 4564  com/acheong08/Ed
+00002660: 6765 4750 542f 6772 6170 6873 2f63 6f6e  geGPT/graphs/con
+00002670: 7472 6962 7574 6f72 7322 3e0a 2020 3c69  tributors">.  <i
+00002680: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00002690: 636f 6e74 7269 622e 726f 636b 732f 696d  contrib.rocks/im
+000026a0: 6167 653f 7265 706f 3d61 6368 656f 6e67  age?repo=acheong
+000026b0: 3038 2f45 6467 6547 5054 2220 2f3e 0a20  08/EdgeGPT" />. 
+000026c0: 3c2f 613e 0a                             </a>.
```

### Comparing `EdgeGPT-0.6.9/setup.py` & `EdgeGPT-0.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.6.9",
+    version="0.7.0",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
@@ -24,20 +24,21 @@
     entry_points={
         "console_scripts": [
             "edge-gpt = EdgeGPT:main",
             "edge-gpt-image = ImageGen:main",
         ],
     },
     install_requires=[
-        "httpx",
+        "httpx[socks]>=0.24.0",
         "websockets",
         "rich",
         "certifi",
         "prompt_toolkit",
         "requests",
+        "aiofiles",
         "BingImageCreator>=0.3.0",
     ],
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["EdgeGPT", "ImageGen"],
     classifiers=[
         "License :: OSI Approved :: The Unlicense (Unlicense)",
```

### Comparing `EdgeGPT-0.6.9/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.7.0/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.6.9
+Version: 0.7.0
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -104,27 +104,36 @@
         EdgeGPT - A demo of reverse engineering the Bing GPT chatbot
         Repo: github.com/acheong08/EdgeGPT
         By: Antonio Cheong
 
         !help for help
 
         Type !exit to exit
-        Enter twice to send message or set --enter-once to send one line message
 
-usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [--style {creative,balanced,precise}]
+usage: EdgeGPT.py [-h] [--enter-once] [--search-result] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK]
+                  [--style {creative,balanced,precise}] [--prompt PROMPT] [--cookie-file COOKIE_FILE]
+                  [--history-file HISTORY_FILE] [--locale LOCALE]
 
 options:
   -h, --help            show this help message and exit
   --enter-once
+  --search-result
   --no-stream
   --rich
   --proxy PROXY         Proxy URL (e.g. socks5://127.0.0.1:1080)
+  --wss-link WSS_LINK   WSS URL(e.g. wss://sydney.bing.com/sydney/ChatHub)
   --style {creative,balanced,precise}
-  --cookie-file [path/to/cookies.json]
+  --prompt PROMPT       prompt to start with
+  --cookie-file COOKIE_FILE
+                        path to cookie file
+  --history-file HISTORY_FILE
+                        path to history file
+  --locale LOCALE       your locale (e.g. en-US, zh-CN, en-IE, en-GB)
 ```
+(China/US/UK/Norway has enhanced support for locale)
 
 ## Running in Python
 
 ### 1. The `Chatbot` class and `asyncio` for more granular control
 
 Use Async for the best experience, for example:
 
@@ -146,14 +155,16 @@
 
 ### 2) The `Query` and `Cookie` helper classes
 
   </summary>
 
 Create a simple Bing Chat AI query (using the 'precise' conversation style by default) and see just the main text output rather than the whole API response:
 
+Remeber to store your cookies in a specific format: `bing_cookie_*.json`.
+  
 ```python
 from EdgeGPT import Query, Cookie
 
 q = Query("What are you? Give your answer as Python code")
 print(q)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.9 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.7.0 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -33,49 +33,54 @@
 the extension 8. Click "Export" on the bottom right, then "Export as JSON"
 (This saves your cookies to clipboard) 9. Paste your cookies into a file
 `cookies.json` ### In code: ```python cookies = json.loads(open("./path/to/
 cookies.json", encoding="utf-8").read()) bot = await Chatbot.create
 (cookies=cookies) ``` ## Running from the Command Line ``` $ python3 -m EdgeGPT
 -h EdgeGPT - A demo of reverse engineering the Bing GPT chatbot Repo:
 github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help Type !exit to
-exit Enter twice to send message or set --enter-once to send one line message
-usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [-
--style {creative,balanced,precise}] options: -h, --help show this help message
-and exit --enter-once --no-stream --rich --proxy PROXY Proxy URL (e.g. socks5:/
-/127.0.0.1:1080) --style {creative,balanced,precise} --cookie-file [path/to/
-cookies.json] ``` ## Running in Python ### 1. The `Chatbot` class and `asyncio`
-for more granular control Use Async for the best experience, for example:
-```python import asyncio from EdgeGPT import Chatbot, ConversationStyle async
-def main(): bot = await Chatbot.create() # Passing cookies is optional print
-(await bot.ask(prompt="Hello world",
-conversation_style=ConversationStyle.creative)) await bot.close() if __name__
-== "__main__": asyncio.run(main()) ```   ### 2) The `Query` and `Cookie` helper
-classes  Create a simple Bing Chat AI query (using the 'precise' conversation
-style by default) and see just the main text output rather than the whole API
-response: ```python from EdgeGPT import Query, Cookie q = Query("What are you?
-Give your answer as Python code") print(q) ``` Or change the conversation style
-or cookie file to be used: ```python q = Query( "What are you? Give your answer
-as Python code", style="creative", # or 'balanced' cookies="./
-bing_cookies_alternative.json" ) ``` Quickly extract the text output, code
-snippets, list of sources/references, or suggested follow-on questions using
-the following attributes: ```python q.output q.code q.suggestions q.sources #
-for the full json output q.sources_dict # for a dictionary of titles and urls
-``` Get the orginal prompt and the conversation style you specified: ```python
-q.prompt q.style repr(q) ``` Access previous Queries made since importing
-`Query`: ```python Query.index # A list of Query objects; updated dynamically
-Query.request_count # A tally of requests made using each cookie file ``` And
-finally, the `Cookie` class supports multiple cookie files, so if you create
-additional cookie files with the naming convention `bing_cookies_*.json`, your
-queries will automatically try using the next file (alphabetically) if you've
-exceeded your daily quota of requests (currently set at 200). Here are the main
-attributes which you can access: ```python Cookie.current_file_index
-Cookie.dirpath Cookie.search_pattern # default is `bing_cookies_*.json`
-Cookie.files() # list as files that match .search_pattern
-Cookie.current_filepath Cookie.current_data Cookie.import_next()
-Cookie.image_token Cookie.ignore_files ```  --- ## Running with Docker This
+exit usage: EdgeGPT.py [-h] [--enter-once] [--search-result] [--no-stream] [--
+rich] [--proxy PROXY] [--wss-link WSS_LINK] [--style
+{creative,balanced,precise}] [--prompt PROMPT] [--cookie-file COOKIE_FILE] [--
+history-file HISTORY_FILE] [--locale LOCALE] options: -h, --help show this help
+message and exit --enter-once --search-result --no-stream --rich --proxy PROXY
+Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-link WSS_LINK WSS URL(e.g. wss:/
+/sydney.bing.com/sydney/ChatHub) --style {creative,balanced,precise} --prompt
+PROMPT prompt to start with --cookie-file COOKIE_FILE path to cookie file --
+history-file HISTORY_FILE path to history file --locale LOCALE your locale
+(e.g. en-US, zh-CN, en-IE, en-GB) ``` (China/US/UK/Norway has enhanced support
+for locale) ## Running in Python ### 1. The `Chatbot` class and `asyncio` for
+more granular control Use Async for the best experience, for example: ```python
+import asyncio from EdgeGPT import Chatbot, ConversationStyle async def main():
+bot = await Chatbot.create() # Passing cookies is optional print(await bot.ask
+(prompt="Hello world", conversation_style=ConversationStyle.creative)) await
+bot.close() if __name__ == "__main__": asyncio.run(main()) ```   ### 2) The
+`Query` and `Cookie` helper classes  Create a simple Bing Chat AI query (using
+the 'precise' conversation style by default) and see just the main text output
+rather than the whole API response: Remeber to store your cookies in a specific
+format: `bing_cookie_*.json`. ```python from EdgeGPT import Query, Cookie q =
+Query("What are you? Give your answer as Python code") print(q) ``` Or change
+the conversation style or cookie file to be used: ```python q = Query( "What
+are you? Give your answer as Python code", style="creative", # or 'balanced'
+cookies="./bing_cookies_alternative.json" ) ``` Quickly extract the text
+output, code snippets, list of sources/references, or suggested follow-on
+questions using the following attributes: ```python q.output q.code
+q.suggestions q.sources # for the full json output q.sources_dict # for a
+dictionary of titles and urls ``` Get the orginal prompt and the conversation
+style you specified: ```python q.prompt q.style repr(q) ``` Access previous
+Queries made since importing `Query`: ```python Query.index # A list of Query
+objects; updated dynamically Query.request_count # A tally of requests made
+using each cookie file ``` And finally, the `Cookie` class supports multiple
+cookie files, so if you create additional cookie files with the naming
+convention `bing_cookies_*.json`, your queries will automatically try using the
+next file (alphabetically) if you've exceeded your daily quota of requests
+(currently set at 200). Here are the main attributes which you can access:
+```python Cookie.current_file_index Cookie.dirpath Cookie.search_pattern #
+default is `bing_cookies_*.json` Cookie.files() # list as files that match
+.search_pattern Cookie.current_filepath Cookie.current_data Cookie.import_next
+() Cookie.image_token Cookie.ignore_files ```  --- ## Running with Docker This
 assumes you have a file cookies.json in your current working directory ```bash
 docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
 cookies.json' ghcr.io/acheong08/edgegpt ``` You can add any extra flags as
 following ```bash docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -
 e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative
 ```    # Image generator  ## Running from the Command Line ```bash $ python3 -
 m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --
```

### Comparing `EdgeGPT-0.6.9/src/EdgeGPT.py` & `EdgeGPT-0.7.0/src/EdgeGPT.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Main.py
 """
 from __future__ import annotations
 
 import argparse
 import asyncio
+import aiofiles
 import json
 import os
 import random
 import re
 import ssl
 import sys
 import time
@@ -96,14 +97,105 @@
 ssl_context.load_verify_locations(certifi.where())
 
 
 class NotAllowedToAccess(Exception):
     pass
 
 
+class LocationHint(Enum):
+    USA = {
+        "locale": "en-US",
+        "LocationHint": [
+            {
+                "country": "United States",
+                "state": "California",
+                "city": "Los Angeles",
+                "timezoneoffset": 8,
+                "countryConfidence": 8,
+                "Center": {
+                    "Latitude": 34.0536909,
+                    "Longitude": -118.242766,
+                },
+                "RegionType": 2,
+                "SourceType": 1,
+            }
+        ],
+    }
+    CHINA = {
+        "locale": "zh-CN",
+        "LocationHint": [
+            {
+                "country": "China",
+                "state": "",
+                "city": "Beijing",
+                "timezoneoffset": 8,
+                "countryConfidence": 8,
+                "Center": {
+                    "Latitude": 39.9042,
+                    "Longitude": 116.4074,
+                },
+                "RegionType": 2,
+                "SourceType": 1,
+            }
+        ],
+    }
+    EU = {
+        "locale": "en-IE",
+        "LocationHint": [
+            {
+                "country": "Norway",
+                "state": "",
+                "city": "Oslo",
+                "timezoneoffset": 1,
+                "countryConfidence": 8,
+                "Center": {
+                    "Latitude": 59.9139,
+                    "Longitude": 10.7522,
+                },
+                "RegionType": 2,
+                "SourceType": 1,
+            }
+        ],
+    }
+    UK = {
+        "locale": "en-GB",
+        "LocationHint": [
+            {
+                "country": "United Kingdom",
+                "state": "",
+                "city": "London",
+                "timezoneoffset": 0,
+                "countryConfidence": 8,
+                "Center": {
+                    "Latitude": 51.5074,
+                    "Longitude": -0.1278,
+                },
+                "RegionType": 2,
+                "SourceType": 1,
+            },
+        ],
+    }
+
+
+LOCATION_HINT_TYPES = Optional[Union[LocationHint, Literal["USA", "CHINA", "EU", "UK"]]]
+
+
+def get_location_hint_from_locale(locale: str) -> dict | None:
+    if locale == "en-US":
+        return LocationHint.USA.value
+    elif locale == "zh-CN":
+        return LocationHint.CHINA.value
+    elif locale == "en-GB":
+        return LocationHint.UK.value
+    elif locale == "en-IE":
+        return LocationHint.EU.value
+    else:
+        return None
+
+
 class ConversationStyle(Enum):
     creative = [
         "nlu_direct_response_filter",
         "deepleo",
         "disable_emoji_spoken_text",
         "responsible_ai_policy_235",
         "enablemm",
@@ -197,14 +289,15 @@
     def update(
         self,
         prompt: str,
         conversation_style: CONVERSATION_STYLE_TYPE,
         options: list | None = None,
         webpage_context: str | None = None,
         search_result: bool = False,
+        locale: str = "en-US",
     ) -> None:
         """
         Updates request object
         """
         if options is None:
             options = [
                 "deepleo",
@@ -224,38 +317,46 @@
                     "allowedMessageTypes": [
                         "Chat",
                         "Disengaged",
                         "AdsQuery",
                         "SemanticSerp",
                         "GenerateContentQuery",
                         "SearchQuery",
+                        "ActionRequest",
+                        "Context",
+                        "Progress",
+                        "AdsQuery",
+                        "SemanticSerp",
                     ],
                     "sliceIds": [
-                        "chk1cf",
-                        "nopreloadsscf",
-                        "winlongmsg2tf",
-                        "perfimpcomb",
-                        "sugdivdis",
-                        "sydnoinputt",
-                        "wpcssopt",
-                        "wintone2tf",
-                        "0404sydicnbs0",
-                        "405suggbs0",
-                        "scctl",
-                        "330uaugs0",
-                        "0329resp",
-                        "udscahrfon",
-                        "udstrblm5",
-                        "404e2ewrt",
-                        "408nodedups0",
-                        "403tvlansgnd",
+                        "winmuid3tf",
+                        "osbsdusgreccf",
+                        "ttstmout",
+                        "crchatrev",
+                        "winlongmsgtf",
+                        "ctrlworkpay",
+                        "norespwtf",
+                        "tempcacheread",
+                        "temptacache",
+                        "505scss0",
+                        "508jbcars0",
+                        "515enbotdets0",
+                        "5082tsports",
+                        "515vaoprvs",
+                        "424dagslnv1s0",
+                        "kcimgattcf",
+                        "427startpms0",
                     ],
                     "traceId": _get_ran_hex(32),
                     "isStartOfSession": self.invocation_id == 0,
                     "message": {
+                        "locale": locale,
+                        "market": locale,
+                        "region": locale[-2:],  # en-US -> US
+                        "locationHints": get_location_hint_from_locale(locale),
                         "author": "user",
                         "inputMethod": "Keyboard",
                         "text": prompt,
                         "messageType": "Chat",
                     },
                     "conversationSignature": self.conversation_signature,
                     "participant": {
@@ -441,14 +542,15 @@
         prompt: str,
         wss_link: str,
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         options: dict = None,
         webpage_context: str | None = None,
         search_result: bool = False,
+        locale: bool = False,
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
         timeout = aiohttp.ClientTimeout(total=900)
         self.session = aiohttp.ClientSession(timeout=timeout)
 
@@ -467,14 +569,15 @@
             # Construct a ChatHub request
             self.request.update(
                 prompt=prompt,
                 conversation_style=conversation_style,
                 options=options,
                 webpage_context=webpage_context,
                 search_result=search_result,
+                locale=locale,
             )
         else:
             async with httpx.AsyncClient() as client:
                 response = await client.post(
                     "https://sydney.bing.com/sydney/UpdateConversation/",
                     json={
                         "messages": [
@@ -633,33 +736,49 @@
         self.chat_hub = _ChatHub(
             await _Conversation.create(self.proxy, cookies=cookies),
             proxy=self.proxy,
             cookies=cookies,
         )
         return self
 
+    async def save_conversation(self, filename: str) -> None:
+        """
+        Save the conversation to a file
+        """
+        async with aiofiles.open(filename, "w") as f:
+            f.write(json.dumps(self.chat_hub.struct))
+
+    async def load_conversation(self, filename: str) -> None:
+        """
+        Load the conversation from a file
+        """
+        async with aiofiles.open(filename, "r") as f:
+            self.chat_hub.struct = json.loads(await f.read())
+
     async def ask(
         self,
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         options: dict = None,
         webpage_context: str | None = None,
         search_result: bool = False,
+        locale: bool = False,
     ) -> dict:
         """
         Ask a question to the bot
         """
         async for final, response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             options=options,
             webpage_context=webpage_context,
             search_result=search_result,
+            locale=locale,
         ):
             if final:
                 return response
         await self.chat_hub.wss.close()
         return {}
 
     async def ask_stream(
@@ -667,26 +786,28 @@
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         options: dict = None,
         webpage_context: str | None = None,
         search_result: bool = False,
+        locale: bool = False,
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
         async for response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             raw=raw,
             options=options,
             webpage_context=webpage_context,
             search_result=search_result,
+            locale=locale,
         ):
             yield response
 
     async def close(self) -> None:
         """
         Close the connection
         """
@@ -808,27 +929,31 @@
         p_hist("Bot:")
         if args.no_stream:
             response = (
                 await bot.ask(
                     prompt=question,
                     conversation_style=args.style,
                     wss_link=args.wss_link,
+                    search_result=args.search_result,
+                    locale=args.locale,
                 )
             )["item"]["messages"][1]["adaptiveCards"][0]["body"][0]["text"]
             print(response)
             p_hist(response)
         else:
             wrote = 0
             if args.rich:
                 md = Markdown("")
                 with Live(md, auto_refresh=False) as live:
                     async for final, response in bot.ask_stream(
                         prompt=question,
                         conversation_style=args.style,
                         wss_link=args.wss_link,
+                        search_result=args.search_result,
+                        locale=args.locale,
                     ):
                         if not final:
                             if not wrote:
                                 p_hist(response, end="")
                             else:
                                 p_hist(response[wrote:], end="")
                             if wrote > len(response):
@@ -838,14 +963,16 @@
                             md = Markdown(response)
                             live.update(md, refresh=True)
             else:
                 async for final, response in bot.ask_stream(
                     prompt=question,
                     conversation_style=args.style,
                     wss_link=args.wss_link,
+                    search_result=args.search_result,
+                    locale=args.locale,
                 ):
                     if not final:
                         if not wrote:
                             print(response, end="", flush=True)
                             p_hist(response, end="")
                         else:
                             print(response[wrote:], end="", flush=True)
@@ -868,14 +995,15 @@
         !help for help
 
         Type !exit to exit
     """,
     )
     parser = argparse.ArgumentParser()
     parser.add_argument("--enter-once", action="store_true")
+    parser.add_argument("--search-result", action="store_true")
     parser.add_argument("--no-stream", action="store_true")
     parser.add_argument("--rich", action="store_true")
     parser.add_argument(
         "--proxy",
         help="Proxy URL (e.g. socks5://127.0.0.1:1080)",
         type=str,
     )
@@ -907,14 +1035,21 @@
     parser.add_argument(
         "--history-file",
         type=str,
         default="",
         required=False,
         help="path to history file",
     )
+    parser.add_argument(
+        "--locale",
+        type=str,
+        default="en-US",
+        required=False,
+        help="your locale",
+    )
     args = parser.parse_args()
     asyncio.run(async_main(args))
 
 
 class Cookie:
     """
     Convenience class for Bing Cookie files, data, and configuration. This Class
@@ -923,14 +1058,15 @@
     account per day) are exceeded.
     """
 
     current_file_index = 0
     dirpath = Path("./").resolve()
     search_pattern = "bing_cookies_*.json"
     ignore_files = set()
+    current_filepath: dict | None = None
 
     @classmethod
     def fetch_default(cls, path=None):
         from selenium import webdriver
         from selenium.webdriver.common.by import By
 
         driver = webdriver.Edge()
@@ -963,25 +1099,24 @@
 
           .current_filepath
           .current_data
           .image_token
         """
         try:
             cls.current_filepath = cls.files()[cls.current_file_index]
-        except IndexError:
+        except IndexError as exc:
             print(
                 "> Please set Cookie.current_filepath to a valid cookie file, then run Cookie.import_data()",
             )
-            return
+            raise "No valid cookie file found." from exc
         print(f"> Importing cookies from: {cls.current_filepath.name}")
         with open(cls.current_filepath, encoding="utf-8") as file:
             cls.current_data = json.load(file)
         cls.image_token = [x for x in cls.current_data if x.get("name") == "_U"]
         cls.image_token = cls.image_token[0].get("value")
-        return cls.current_data
 
     @classmethod
     def import_next(cls):
         """
         Cycle through to the next cookies file.  Import it.  Mark the previous
         file to be ignored for the remainder of the current session.
         """
@@ -1064,16 +1199,17 @@
 
     async def send_to_bing(self, echo=True, echo_prompt=False):
         """Creat, submit, then close a Chatbot instance.  Return the response"""
         retries = len(Cookie.files())
         while retries:
             try:
                 # Read the cookies file
-                cookie_data = Cookie.import_data()
-                bot = await Chatbot.create(proxy=self.proxy, cookies=cookie_data)
+                bot = await Chatbot.create(
+                    proxy=self.proxy, cookies=Cookie.current_data
+                )
                 if echo_prompt:
                     print(f"> {self.prompt}=")
                 if echo:
                     print("> Waiting for response...")
                 if self.style.lower() not in "creative balanced precise".split():
                     self.style = "precise"
                 response = await bot.ask(
```

