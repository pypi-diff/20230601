# Comparing `tmp/pyfarmer-0.1.2.tar.gz` & `tmp/pyfarmer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfarmer-0.1.2.tar", max compression
+gzip compressed data, was "pyfarmer-1.0.1.tar", max compression
```

## Comparing `pyfarmer-0.1.2.tar` & `pyfarmer-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      259 2022-07-03 16:28:30.254229 pyfarmer-0.1.2/pyfarmer/__init__.py
--rwxr-xr-x   0        0        0    19480 2022-07-03 16:28:30.254229 pyfarmer-0.1.2/pyfarmer/_client.py
--rw-r--r--   0        0        0     4195 2022-07-03 16:28:30.254229 pyfarmer-0.1.2/pyfarmer/_pyfarmer.py
--rw-r--r--   0        0        0      147 2022-07-03 16:28:30.254229 pyfarmer-0.1.2/pyfarmer/_tmp.py
--rw-r--r--   0        0        0        0 2022-07-03 16:28:30.254229 pyfarmer-0.1.2/pyfarmer/py.typed
--rw-r--r--   0        0        0      943 2022-07-03 16:28:30.254229 pyfarmer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      636 2022-07-03 16:29:18.229169 pyfarmer-0.1.2/setup.py
--rw-r--r--   0        0        0      484 2022-07-03 16:29:18.229487 pyfarmer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      259 2023-06-01 18:16:39.024165 pyfarmer-1.0.1/pyfarmer/__init__.py
+-rwxr-xr-x   0        0        0    19480 2023-06-01 18:16:39.024165 pyfarmer-1.0.1/pyfarmer/_client.py
+-rw-r--r--   0        0        0     4301 2023-06-01 18:16:39.024165 pyfarmer-1.0.1/pyfarmer/_pyfarmer.py
+-rw-r--r--   0        0        0      147 2023-06-01 18:16:39.024165 pyfarmer-1.0.1/pyfarmer/_tmp.py
+-rw-r--r--   0        0        0        0 2023-06-01 18:16:39.024165 pyfarmer-1.0.1/pyfarmer/py.typed
+-rw-r--r--   0        0        0      688 2023-06-01 18:16:39.024165 pyfarmer-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 pyfarmer-1.0.1/PKG-INFO
```

### Comparing `pyfarmer-0.1.2/pyfarmer/_client.py` & `pyfarmer-1.0.1/pyfarmer/_client.py`

 * *Files identical despite different names*

### Comparing `pyfarmer-0.1.2/pyfarmer/_pyfarmer.py` & `pyfarmer-1.0.1/pyfarmer/_pyfarmer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 from argparse import ArgumentParser
-from collections.abc import Callable
+from collections.abc import Callable, Iterable
 from string import printable
 from typing import Any
 from subprocess import call
 from os.path import dirname, join, basename
-from requests import get
+from httpx import get
 from random import choice
 from traceback import print_exc, print_exception as print_except
 from tempfile import NamedTemporaryFile
 from sys import executable
 
 ip: str = ""
 
@@ -36,14 +36,19 @@
             pass
 
 
 def submit_flag(flag: str) -> None:
     print(flag, flush=True)
 
 
+def submit_flags(flags: Iterable[str]) -> None:
+    for flag in flags:
+        submit_flag(flag)
+
+
 def get_ids(url: str, service: str) -> list[str]:
     return get(url).json()[service][ip]
 
 
 def random_string(length: int = 16, charset: str = printable) -> str:
     return "".join(choice(charset) for _ in range(length))
```

