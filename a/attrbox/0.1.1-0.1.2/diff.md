# Comparing `tmp/attrbox-0.1.1.tar.gz` & `tmp/attrbox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attrbox-0.1.1.tar", last modified: Thu Sep 23 20:44:26 2021, max compression
+gzip compressed data, was "attrbox-0.1.2.tar", last modified: Thu Jun  1 05:06:42 2023, max compression
```

## Comparing `attrbox-0.1.1.tar` & `attrbox-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 20:44:26.985776 attrbox-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2021-09-23 20:44:10.000000 attrbox-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2021-09-23 20:44:26.985776 attrbox-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2021-09-23 20:44:10.000000 attrbox-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-09-23 20:44:10.000000 attrbox-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-09-23 20:44:26.985776 attrbox-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2021-09-23 20:44:10.000000 attrbox-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 20:44:26.981775 attrbox-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 20:44:26.981775 attrbox-0.1.1/src/attrbox/
--rw-r--r--   0 runner    (1001) docker     (121)      333 2021-09-23 20:44:10.000000 attrbox-0.1.1/src/attrbox/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2021-09-23 20:44:10.000000 attrbox-0.1.1/src/attrbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5117 2021-09-23 20:44:10.000000 attrbox-0.1.1/src/attrbox/attrdict.py
--rw-r--r--   0 runner    (1001) docker     (121)     2372 2021-09-23 20:44:10.000000 attrbox-0.1.1/src/attrbox/attrlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2021-09-23 20:44:10.000000 attrbox-0.1.1/src/attrbox/jsend.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 20:44:26.985776 attrbox-0.1.1/src/attrbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2021-09-23 20:44:26.000000 attrbox-0.1.1/src/attrbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      392 2021-09-23 20:44:26.000000 attrbox-0.1.1/src/attrbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-23 20:44:26.000000 attrbox-0.1.1/src/attrbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-09-23 20:44:26.000000 attrbox-0.1.1/src/attrbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-09-23 20:44:26.000000 attrbox-0.1.1/src/attrbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 20:44:26.985776 attrbox-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)      971 2021-09-23 20:44:10.000000 attrbox-0.1.1/test/test_attrdict.py
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2021-09-23 20:44:10.000000 attrbox-0.1.1/test/test_dict_merge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:06:42.731005 attrbox-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-01 05:06:27.000000 attrbox-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-06-01 05:06:42.731005 attrbox-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-01 05:06:27.000000 attrbox-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-01 05:06:27.000000 attrbox-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 05:06:42.731005 attrbox-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:06:42.727005 attrbox-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:06:42.731005 attrbox-0.1.2/src/attrbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-01 05:06:27.000000 attrbox-0.1.2/src/attrbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-06-01 05:06:27.000000 attrbox-0.1.2/src/attrbox/attrdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-06-01 05:06:27.000000 attrbox-0.1.2/src/attrbox/attrlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-06-01 05:06:27.000000 attrbox-0.1.2/src/attrbox/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-06-01 05:06:27.000000 attrbox-0.1.2/src/attrbox/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-01 05:06:27.000000 attrbox-0.1.2/src/attrbox/fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-01 05:06:27.000000 attrbox-0.1.2/src/attrbox/jsend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:06:42.731005 attrbox-0.1.2/src/attrbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-06-01 05:06:42.000000 attrbox-0.1.2/src/attrbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-01 05:06:42.000000 attrbox-0.1.2/src/attrbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 05:06:42.000000 attrbox-0.1.2/src/attrbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-01 05:06:42.000000 attrbox-0.1.2/src/attrbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 05:06:42.000000 attrbox-0.1.2/src/attrbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:06:42.731005 attrbox-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-01 05:06:27.000000 attrbox-0.1.2/test/test_attrdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-01 05:06:27.000000 attrbox-0.1.2/test/test_fn_set_path.py
```

### Comparing `attrbox-0.1.1/LICENSE.md` & `attrbox-0.1.2/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2021 Metaist LLC.
+Copyright 2023 Metaist LLC.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `attrbox-0.1.1/src/attrbox/jsend.py` & `attrbox-0.1.2/src/attrbox/jsend.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # coding: utf-8
 """Standard JSON responses."""
 
 # native
+from __future__ import annotations
 from typing import Any, Dict, Optional
 
 # pkg
 from .attrdict import AttrDict
 
 # Response status
 STATUS_SUCCESS = "success"
@@ -15,20 +16,20 @@
 
 Msg = Optional[str]
 
 
 class JSend(AttrDict):
     """Service response object.
 
-    This object loosely conforms to the JSend specification:
-    <https://labs.omniti.com/labs/jsend>
+    This object loosely conforms to the
+    [JSend specification](https://labs.omniti.com/labs/jsend).
     """
 
     def __init__(self, *args: Any, **kwargs: Dict[str, Any]):
-        """Construct a response.
+        """Construct a JSend object.
 
         Examples:
             >>> result = JSend()
             >>> result.ok
             True
             >>> result.status == 'success'
             True
@@ -36,22 +37,22 @@
             True
             >>> result == {'ok': True, 'status': 'success', 'data': None}
             True
         """
         self.update(ok=True, status=STATUS_SUCCESS, data=None)
         super().__init__(*args, **kwargs)
 
-    def fail(self, message: Msg = None) -> "JSend":
+    def fail(self, message: Msg = None) -> JSend:
         """Indicate a controlled failure.
 
         Args:
             message (str): human-readable explanation of the failure
 
         Returns:
-            (JSend): self for chaining
+            JSend: self for chaining
 
         Examples:
             >>> result = JSend()
             >>> msg = 'Missing a phone number.'
             >>> result.fail(msg) is result
             True
             >>> result.ok is False
@@ -60,23 +61,23 @@
             True
             >>> result.message == msg
             True
         """
         self.update(ok=False, status=STATUS_FAIL, message=message)
         return self
 
-    def error(self, message: Msg = None, code: Optional[Any] = None) -> "JSend":
+    def error(self, message: Msg = None, code: Optional[Any] = None) -> JSend:
         """Indicate an uncontrolled error.
 
         Args:
             message (str): human-readable explanation of the error
-            code (any): technical indication of the error
+            code (Any, optional): technical indication of the error
 
         Returns:
-            (JSend): self for chaining
+            JSend: self for chaining
 
         Examples:
             >>> result = JSend()
             >>> msg = 'No such file [file.text].'
             >>> code = 13
             >>> result.error(msg, code) is result
             True
@@ -88,22 +89,22 @@
             True
             >>> result.code == code
             True
         """
         self.update(ok=False, status=STATUS_ERROR, message=message, code=code)
         return self
 
-    def success(self, data: Any = None) -> "JSend":
+    def success(self, data: Optional[Any] = None) -> JSend:
         """Indicate a successful response.
 
         Args:
-            data (any): response payload
+            data (Any, optional): response payload
 
         Returns:
-            (JSend): self for chaining
+            JSend: self for chaining
 
         Examples:
             >>> data = "Works"
             >>> result = JSend()
             >>> result.success(data) is result
             True
             >>> result.data == data
```

