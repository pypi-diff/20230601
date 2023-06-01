# Comparing `tmp/pypura-0.1.4.tar.gz` & `tmp/pypura-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypura-0.1.4.tar", max compression
+gzip compressed data, was "pypura-0.1.5.tar", max compression
```

## Comparing `pypura-0.1.4.tar` & `pypura-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-05-20 05:36:25.693183 pypura-0.1.4/LICENSE
--rw-r--r--   0        0        0       76 2023-05-20 05:36:25.693183 pypura-0.1.4/README.md
--rw-r--r--   0        0        0      747 2023-05-20 05:36:44.393699 pypura-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      251 2023-05-20 05:36:44.393699 pypura-0.1.4/pypura/__init__.py
--rw-r--r--   0        0        0     1447 2023-05-20 05:36:25.697183 pypura-0.1.4/pypura/const.py
--rw-r--r--   0        0        0      200 2023-05-20 05:36:25.697183 pypura-0.1.4/pypura/exceptions.py
--rw-r--r--   0        0        0     6705 2023-05-20 05:36:25.697183 pypura-0.1.4/pypura/pura.py
--rw-r--r--   0        0        0        0 2023-05-20 05:36:25.697183 pypura-0.1.4/pypura/py.typed
--rw-r--r--   0        0        0      717 2023-05-20 05:36:25.697183 pypura-0.1.4/pypura/utils.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 pypura-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-01 02:10:40.536047 pypura-0.1.5/LICENSE
+-rw-r--r--   0        0        0       76 2023-06-01 02:10:40.536047 pypura-0.1.5/README.md
+-rw-r--r--   0        0        0      747 2023-06-01 02:10:57.236236 pypura-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      251 2023-06-01 02:10:57.236236 pypura-0.1.5/pypura/__init__.py
+-rw-r--r--   0        0        0      414 2023-06-01 02:10:40.536047 pypura-0.1.5/pypura/const.py
+-rw-r--r--   0        0        0      200 2023-06-01 02:10:40.536047 pypura-0.1.5/pypura/exceptions.py
+-rw-r--r--   0        0        0    30567 2023-06-01 02:10:40.536047 pypura-0.1.5/pypura/fragrances.json
+-rw-r--r--   0        0        0     6705 2023-06-01 02:10:40.536047 pypura-0.1.5/pypura/pura.py
+-rw-r--r--   0        0        0        0 2023-06-01 02:10:40.536047 pypura-0.1.5/pypura/py.typed
+-rw-r--r--   0        0        0      803 2023-06-01 02:10:40.536047 pypura-0.1.5/pypura/utils.py
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 pypura-0.1.5/PKG-INFO
```

### Comparing `pypura-0.1.4/LICENSE` & `pypura-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypura-0.1.4/pyproject.toml` & `pypura-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypura"
-version = "0.1.4"
+version = "0.1.5"
 description = "Python package for interacting with Pura smart fragrance diffuser"
 authors = ["Nathan Spencer <natekspencer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 include = ["pypura/py.typed"]
 
 [tool.poetry.dependencies]
```

### Comparing `pypura-0.1.4/pypura/pura.py` & `pypura-0.1.5/pypura/pura.py`

 * *Files identical despite different names*

### Comparing `pypura-0.1.4/pypura/utils.py` & `pypura-0.1.5/pypura/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 from .const import FRAGRANCES
 
 _LOGGER = logging.getLogger(__name__)
 
 ENCODING: Final = "utf-8"
 ISSUE_URL: Final = "https://github.com/natekspencer/pypura/issues/1"
 
+FRAGRANCE_DICT = {f["sku"]: f for f in FRAGRANCES}
+
 
 def decode(value: str) -> str:
     """Decode a value."""
     return b64decode(value).decode(ENCODING)
 
 
 def fragrance_name(code: str) -> str:
     """Return fragrance name."""
-    if not (name := FRAGRANCES.get(code)):
+    if not (name := FRAGRANCE_DICT.get(code, {}).get("name")):
         _LOGGER.warning(
             "Unknown fragrance code '%s', please report this at %s", code, ISSUE_URL
         )
         name = f"Fragrance code: {code}"
-        FRAGRANCES[code] = name
+        FRAGRANCE_DICT[code] = {"name": name}
     return name
```

### Comparing `pypura-0.1.4/PKG-INFO` & `pypura-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypura
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package for interacting with Pura smart fragrance diffuser
 License: MIT
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

