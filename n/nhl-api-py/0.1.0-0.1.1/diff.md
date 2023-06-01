# Comparing `tmp/nhl_api_py-0.1.0.tar.gz` & `tmp/nhl_api_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhl_api_py-0.1.0.tar", max compression
+gzip compressed data, was "nhl_api_py-0.1.1.tar", max compression
```

## Comparing `nhl_api_py-0.1.0.tar` & `nhl_api_py-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       45 2023-06-01 15:36:03.019409 nhl_api_py-0.1.0/README.md
--rw-r--r--   0        0        0       32 2023-06-01 15:54:04.739415 nhl_api_py-0.1.0/nhlpy/__init__.py
--rw-r--r--   0        0        0      309 2023-06-01 16:00:57.059417 nhl_api_py-0.1.0/nhlpy/api/__init__.py
--rw-r--r--   0        0        0      472 2023-06-01 16:03:00.509418 nhl_api_py-0.1.0/nhlpy/api/core.py
--rw-r--r--   0        0        0      778 2023-06-01 17:09:37.399440 nhl_api_py-0.1.0/nhlpy/api/standings.py
--rw-r--r--   0        0        0      846 2023-06-01 16:57:52.189436 nhl_api_py-0.1.0/nhlpy/api/teams.py
--rw-r--r--   0        0        0      209 2023-06-01 17:01:57.729437 nhl_api_py-0.1.0/nhlpy/nhlclient.py
--rw-r--r--   0        0        0      637 2023-06-01 17:20:22.399443 nhl_api_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 nhl_api_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      868 2023-06-01 17:27:20.959445 nhl_api_py-0.1.1/README.md
+-rw-r--r--   0        0        0       32 2023-06-01 15:54:04.739415 nhl_api_py-0.1.1/nhlpy/__init__.py
+-rw-r--r--   0        0        0      309 2023-06-01 16:00:57.059417 nhl_api_py-0.1.1/nhlpy/api/__init__.py
+-rw-r--r--   0        0        0      472 2023-06-01 16:03:00.509418 nhl_api_py-0.1.1/nhlpy/api/core.py
+-rw-r--r--   0        0        0      778 2023-06-01 17:09:37.399440 nhl_api_py-0.1.1/nhlpy/api/standings.py
+-rw-r--r--   0        0        0      846 2023-06-01 16:57:52.189436 nhl_api_py-0.1.1/nhlpy/api/teams.py
+-rw-r--r--   0        0        0      209 2023-06-01 17:01:57.729437 nhl_api_py-0.1.1/nhlpy/nhlclient.py
+-rw-r--r--   0        0        0      637 2023-06-01 17:27:50.369445 nhl_api_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 nhl_api_py-0.1.1/PKG-INFO
```

### Comparing `nhl_api_py-0.1.0/nhlpy/api/standings.py` & `nhl_api_py-0.1.1/nhlpy/api/standings.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.1.0/nhlpy/api/teams.py` & `nhl_api_py-0.1.1/nhlpy/api/teams.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.1.0/pyproject.toml` & `nhl_api_py-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nhl-api-py"
-version = "0.1.0"
+version = "0.1.1"
 description = "NHL API Wrapper.  For standings, team stats and outcomes."
 authors = ["Corey Schaf <cschaf@gmail.com>"]
 readme = "README.md"
 packages = [{include = "nhlpy"}]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

