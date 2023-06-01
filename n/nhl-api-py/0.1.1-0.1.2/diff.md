# Comparing `tmp/nhl_api_py-0.1.1.tar.gz` & `tmp/nhl_api_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhl_api_py-0.1.1.tar", max compression
+gzip compressed data, was "nhl_api_py-0.1.2.tar", max compression
```

## Comparing `nhl_api_py-0.1.1.tar` & `nhl_api_py-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      868 2023-06-01 17:27:20.959445 nhl_api_py-0.1.1/README.md
--rw-r--r--   0        0        0       32 2023-06-01 15:54:04.739415 nhl_api_py-0.1.1/nhlpy/__init__.py
--rw-r--r--   0        0        0      309 2023-06-01 16:00:57.059417 nhl_api_py-0.1.1/nhlpy/api/__init__.py
--rw-r--r--   0        0        0      472 2023-06-01 16:03:00.509418 nhl_api_py-0.1.1/nhlpy/api/core.py
--rw-r--r--   0        0        0      778 2023-06-01 17:09:37.399440 nhl_api_py-0.1.1/nhlpy/api/standings.py
--rw-r--r--   0        0        0      846 2023-06-01 16:57:52.189436 nhl_api_py-0.1.1/nhlpy/api/teams.py
--rw-r--r--   0        0        0      209 2023-06-01 17:01:57.729437 nhl_api_py-0.1.1/nhlpy/nhlclient.py
--rw-r--r--   0        0        0      637 2023-06-01 17:27:50.369445 nhl_api_py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 nhl_api_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      966 2023-06-01 21:42:25.752450 nhl_api_py-0.1.2/README.md
+-rw-r--r--   0        0        0       32 2023-06-01 15:54:04.739415 nhl_api_py-0.1.2/nhlpy/__init__.py
+-rw-r--r--   0        0        0      309 2023-06-01 16:00:57.059417 nhl_api_py-0.1.2/nhlpy/api/__init__.py
+-rw-r--r--   0        0        0      472 2023-06-01 16:03:00.509418 nhl_api_py-0.1.2/nhlpy/api/core.py
+-rw-r--r--   0        0        0      778 2023-06-01 17:09:37.399440 nhl_api_py-0.1.2/nhlpy/api/standings.py
+-rw-r--r--   0        0        0      846 2023-06-01 16:57:52.189436 nhl_api_py-0.1.2/nhlpy/api/teams.py
+-rw-r--r--   0        0        0      209 2023-06-01 17:01:57.729437 nhl_api_py-0.1.2/nhlpy/nhlclient.py
+-rw-r--r--   0        0        0     1257 2023-06-01 21:39:21.482451 nhl_api_py-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 nhl_api_py-0.1.2/PKG-INFO
```

### Comparing `nhl_api_py-0.1.1/README.md` & `nhl_api_py-0.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+[![PyPI version](https://badge.fury.io/py/nhl-api-py.svg)](https://badge.fury.io/py/nhl-api-py)
+
+
 # NHL-py-api
 
 NHL-py-api is a Python package that provides a simple wrapper around the 
 NHL API, allowing you to easily access and retrieve NHL data in your Python 
 applications.
 
 Note: This is very early, I created this to help me with some machine learning
@@ -9,15 +12,15 @@
 
 
 ## Installation
 
 You can install NHL-py-api using pip:
 
 ```shell
-pip install nhl-py-api
+pip install nhl-api-py
 ```
 
 - - -
 ## Usage
 
 ```python
 from nhlpy import NHLClient
```

### Comparing `nhl_api_py-0.1.1/nhlpy/api/standings.py` & `nhl_api_py-0.1.2/nhlpy/api/standings.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.1.1/nhlpy/api/teams.py` & `nhl_api_py-0.1.2/nhlpy/api/teams.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.1.1/PKG-INFO` & `nhl_api_py-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 Metadata-Version: 2.1
 Name: nhl-api-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: NHL API Wrapper.  For standings, team stats and outcomes.
+Home-page: https://github.com/coreyjs/nhl-api-py
+License: GPL-3.0-or-later
+Keywords: nhl,api,wrapper,hockey,sports
 Author: Corey Schaf
 Author-email: cschaf@gmail.com
 Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: httpx
+Project-URL: Repository, https://github.com/coreyjs/nhl-api-py
 Description-Content-Type: text/markdown
 
+[![PyPI version](https://badge.fury.io/py/nhl-api-py.svg)](https://badge.fury.io/py/nhl-api-py)
+
+
 # NHL-py-api
 
 NHL-py-api is a Python package that provides a simple wrapper around the 
 NHL API, allowing you to easily access and retrieve NHL data in your Python 
 applications.
 
 Note: This is very early, I created this to help me with some machine learning
@@ -24,15 +36,15 @@
 
 
 ## Installation
 
 You can install NHL-py-api using pip:
 
 ```shell
-pip install nhl-py-api
+pip install nhl-api-py
 ```
 
 - - -
 ## Usage
 
 ```python
 from nhlpy import NHLClient
```

