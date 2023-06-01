# Comparing `tmp/GoogleBard-1.2.1.tar.gz` & `tmp/GoogleBard-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-1.2.1.tar", last modified: Thu Jun  1 04:34:53 2023, max compression
+gzip compressed data, was "GoogleBard-1.2.2.tar", last modified: Thu Jun  1 17:06:01 2023, max compression
```

## Comparing `GoogleBard-1.2.1.tar` & `GoogleBard-1.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:34:53.831040 GoogleBard-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 04:34:32.000000 GoogleBard-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 04:34:53.827041 GoogleBard-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-01 04:34:32.000000 GoogleBard-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 04:34:53.831040 GoogleBard-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 04:34:32.000000 GoogleBard-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:34:53.827041 GoogleBard-1.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-01 04:34:32.000000 GoogleBard-1.2.1/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 04:34:53.827041 GoogleBard-1.2.1/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 04:34:53.000000 GoogleBard-1.2.1/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-01 04:34:53.000000 GoogleBard-1.2.1/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 04:34:53.000000 GoogleBard-1.2.1/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 04:34:53.000000 GoogleBard-1.2.1/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 04:34:53.000000 GoogleBard-1.2.1/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:01.429151 GoogleBard-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 17:05:39.000000 GoogleBard-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 17:06:01.429151 GoogleBard-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-01 17:05:39.000000 GoogleBard-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:06:01.429151 GoogleBard-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 17:05:39.000000 GoogleBard-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:01.429151 GoogleBard-1.2.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-06-01 17:05:39.000000 GoogleBard-1.2.2/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:01.429151 GoogleBard-1.2.2/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 17:06:01.000000 GoogleBard-1.2.2/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-01 17:06:01.000000 GoogleBard-1.2.2/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:06:01.000000 GoogleBard-1.2.2/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 17:06:01.000000 GoogleBard-1.2.2/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 17:06:01.000000 GoogleBard-1.2.2/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-1.2.1/LICENSE` & `GoogleBard-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.2.1/PKG-INFO` & `GoogleBard-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.2.1
+Version: 1.2.2
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GoogleBard-1.2.1/README.md` & `GoogleBard-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.2.1/setup.py` & `GoogleBard-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="1.2.1",
+    version="1.2.2",
     license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
```

### Comparing `GoogleBard-1.2.1/src/Bard.py` & `GoogleBard-1.2.2/src/Bard.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
 from prompt_toolkit.key_binding import KeyBindings
 from rich.console import Console
 from rich.markdown import Markdown
 
+from typing import List, Dict
+
 
 def __create_session() -> PromptSession:
     return PromptSession(history=InMemoryHistory())
 
 
 def __create_completer(commands: list, pattern_str: str = "$") -> WordCompleter:
     return WordCompleter(words=commands, pattern=re.compile(pattern_str))
@@ -112,15 +114,15 @@
             },
         }
         conversations.append(conversation_details)
 
         with open(file_path, "w", encoding="utf-8") as f:
             json.dump(conversations, f, indent=4)
 
-    def load_conversations(self, file_path: str) -> list[dict]:
+    def load_conversations(self, file_path: str) -> List[Dict]:
         # Check if file exists
         if not os.path.isfile(file_path):
             return []
         with open(file_path, encoding="utf-8") as f:
             return json.load(f)
 
     def load_conversation(self, file_path: str, conversation_name: str) -> bool:
```

### Comparing `GoogleBard-1.2.1/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-1.2.2/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.2.1
+Version: 1.2.2
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

