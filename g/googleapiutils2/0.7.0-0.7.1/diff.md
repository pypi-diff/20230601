# Comparing `tmp/googleapiutils2-0.7.0.tar.gz` & `tmp/googleapiutils2-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.7.0.tar", max compression
+gzip compressed data, was "googleapiutils2-0.7.1.tar", max compression
```

## Comparing `googleapiutils2-0.7.0.tar` & `googleapiutils2-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.7.0/LICENSE
--rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.7.0/README.md
--rw-r--r--   0        0        0       96 2023-06-01 17:02:06.802855 googleapiutils2-0.7.0/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.7.0/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.7.0/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.7.0/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.7.0/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1040 2023-05-25 17:49:07.456779 googleapiutils2-0.7.0/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1178 2022-12-30 01:32:12.342148 googleapiutils2-0.7.0/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.7.0/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     7443 2023-06-01 17:26:02.003498 googleapiutils2-0.7.0/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    24151 2023-06-01 20:48:26.565632 googleapiutils2-0.7.0/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     5310 2023-06-01 18:17:35.266727 googleapiutils2-0.7.0/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     7497 2023-06-01 20:46:27.789563 googleapiutils2-0.7.0/googleapiutils2/utils.py
--rw-r--r--   0        0        0     1067 2023-06-01 20:55:40.347638 googleapiutils2-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.7.1/README.md
+-rw-r--r--   0        0        0       96 2023-06-01 17:02:06.802855 googleapiutils2-0.7.1/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.7.1/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.7.1/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.7.1/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.7.1/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1084 2023-06-01 21:02:11.670817 googleapiutils2-0.7.1/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.7.1/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.7.1/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     7442 2023-06-01 21:03:07.412995 googleapiutils2-0.7.1/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    24151 2023-06-01 20:48:26.565632 googleapiutils2-0.7.1/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     5310 2023-06-01 18:17:35.266727 googleapiutils2-0.7.1/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     7497 2023-06-01 20:46:27.789563 googleapiutils2-0.7.1/googleapiutils2/utils.py
+-rw-r--r--   0        0        0     1067 2023-06-01 21:03:20.344173 googleapiutils2-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.7.1/PKG-INFO
```

### Comparing `googleapiutils2-0.7.0/LICENSE` & `googleapiutils2-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.7.0/README.md` & `googleapiutils2-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.7.0/googleapiutils2/drive/drive.py` & `googleapiutils2-0.7.1/googleapiutils2/drive/drive.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.7.0/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.7.1/googleapiutils2/geocode/geocode.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
+from typing import *
 
 import requests
 from requests.exceptions import JSONDecodeError
 
 from ..utils import update_url_params
-from .misc import GeocodeResult
+
+if TYPE_CHECKING:
+    from .misc import GeocodeResult
 
 
 class Geocode:
     URL = "https://maps.googleapis.com/maps/api/geocode/json"
 
     def __init__(self, api_key: str):
         self.api_key = api_key
```

### Comparing `googleapiutils2-0.7.0/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.7.1/googleapiutils2/sheets/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from dataclasses import dataclass
 from enum import Enum
 from types import EllipsisType
 from typing import *
 
 from ..utils import to_base
 
-
 VERSION = "v4"
 
 DEFAULT_SHEET_NAME = "Sheet1"
 
 DEFAULT_SHEET_SHAPE = (1000, 26)
 
 SheetsValues = list[list[Any]] | list[dict[str | Any, Any]]
```

### Comparing `googleapiutils2-0.7.0/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.7.1/googleapiutils2/sheets/sheets.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.7.0/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.7.1/googleapiutils2/sheets/sheets_value_range.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.7.0/googleapiutils2/utils.py` & `googleapiutils2-0.7.1/googleapiutils2/utils.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.7.0/pyproject.toml` & `googleapiutils2-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.7.0"
+version = "0.7.1"
 description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 
 readme = "README.md"
 keywords = ["google", "googleapi", "googleapiutils2"]
 license = "MIT"
 repository = "https://github.com/mkbabb/googleapiutils2"
```

### Comparing `googleapiutils2-0.7.0/PKG-INFO` & `googleapiutils2-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleapiutils2
-Version: 0.7.0
+Version: 0.7.1
 Summary: Wrapper for Google's Python API.
 Home-page: https://github.com/mkbabb/googleapiutils2
 License: MIT
 Keywords: google,googleapi,googleapiutils2
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
```

