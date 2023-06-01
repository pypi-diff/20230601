# Comparing `tmp/character-encoding-utils-0.0.4.tar.gz` & `tmp/character-encoding-utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "character-encoding-utils-0.0.4.tar", last modified: Fri May 26 07:20:02 2023, max compression
+gzip compressed data, was "character-encoding-utils-0.0.5.tar", last modified: Thu Jun  1 07:10:49 2023, max compression
```

## Comparing `character-encoding-utils-0.0.4.tar` & `character-encoding-utils-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:20:02.418071 character-encoding-utils-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-26 07:20:02.418071 character-encoding-utils-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:20:02.418071 character-encoding-utils-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:20:02.410071 character-encoding-utils-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:20:02.414071 character-encoding-utils-0.0.4/src/character_encoding_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/src/character_encoding_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/src/character_encoding_utils/big5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/src/character_encoding_utils/gb2312.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/src/character_encoding_utils/ksx1001.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/src/character_encoding_utils/shiftjis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:20:02.414071 character-encoding-utils-0.0.4/src/character_encoding_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-26 07:20:02.000000 character-encoding-utils-0.0.4/src/character_encoding_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-26 07:20:02.000000 character-encoding-utils-0.0.4/src/character_encoding_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:20:02.000000 character-encoding-utils-0.0.4/src/character_encoding_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 07:20:02.000000 character-encoding-utils-0.0.4/src/character_encoding_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:20:02.418071 character-encoding-utils-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/tests/test_big5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/tests/test_gb2312.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/tests/test_ksx1001.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/tests/test_shiftjis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:49.610186 character-encoding-utils-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 07:10:34.000000 character-encoding-utils-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-01 07:10:49.610186 character-encoding-utils-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-01 07:10:34.000000 character-encoding-utils-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-01 07:10:34.000000 character-encoding-utils-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 07:10:49.610186 character-encoding-utils-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:49.606186 character-encoding-utils-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:49.610186 character-encoding-utils-0.0.5/src/character_encoding_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:34.000000 character-encoding-utils-0.0.5/src/character_encoding_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-01 07:10:34.000000 character-encoding-utils-0.0.5/src/character_encoding_utils/big5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-06-01 07:10:34.000000 character-encoding-utils-0.0.5/src/character_encoding_utils/gb2312.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-01 07:10:34.000000 character-encoding-utils-0.0.5/src/character_encoding_utils/ksx1001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-01 07:10:34.000000 character-encoding-utils-0.0.5/src/character_encoding_utils/shiftjis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:49.610186 character-encoding-utils-0.0.5/src/character_encoding_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-01 07:10:49.000000 character-encoding-utils-0.0.5/src/character_encoding_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-01 07:10:49.000000 character-encoding-utils-0.0.5/src/character_encoding_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:10:49.000000 character-encoding-utils-0.0.5/src/character_encoding_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 07:10:49.000000 character-encoding-utils-0.0.5/src/character_encoding_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:49.610186 character-encoding-utils-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-01 07:10:34.000000 character-encoding-utils-0.0.5/tests/test_big5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-01 07:10:34.000000 character-encoding-utils-0.0.5/tests/test_gb2312.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-01 07:10:34.000000 character-encoding-utils-0.0.5/tests/test_ksx1001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-01 07:10:34.000000 character-encoding-utils-0.0.5/tests/test_shiftjis.py
```

### Comparing `character-encoding-utils-0.0.4/LICENSE` & `character-encoding-utils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.4/PKG-INFO` & `character-encoding-utils-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: character-encoding-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Some character encoding utils.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/character-encoding-utils
 Project-URL: source, https://github.com/TakWolf/character-encoding-utils
 Project-URL: issues, https://github.com/TakWolf/character-encoding-utils/issues
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Character Encoding Utils
 
+[![Python](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/character-encoding-utils)](https://pypi.org/project/character-encoding-utils/)
 
 Some [character encoding](https://en.wikipedia.org/wiki/Character_encoding) utils.
 
 Now support:
 
 - [GB2312](https://en.wikipedia.org/wiki/GB_2312)
```

### Comparing `character-encoding-utils-0.0.4/README.md` & `character-encoding-utils-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Character Encoding Utils
 
+[![Python](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/character-encoding-utils)](https://pypi.org/project/character-encoding-utils/)
 
 Some [character encoding](https://en.wikipedia.org/wiki/Character_encoding) utils.
 
 Now support:
 
 - [GB2312](https://en.wikipedia.org/wiki/GB_2312)
```

### Comparing `character-encoding-utils-0.0.4/pyproject.toml` & `character-encoding-utils-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "character-encoding-utils"
-version = "0.0.4"
+version = "0.0.5"
 description = "Some character encoding utils."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `character-encoding-utils-0.0.4/src/character_encoding_utils/big5.py` & `character-encoding-utils-0.0.5/src/character_encoding_utils/big5.py`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.4/src/character_encoding_utils/gb2312.py` & `character-encoding-utils-0.0.5/src/character_encoding_utils/gb2312.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-_euc_offset = 0xA0
+_EUC_OFFSET = 0xA0
 
 
 class GB2312Exception(Exception):
     pass
 
 
 class GB2312EncodeError(GB2312Exception):
@@ -63,24 +63,24 @@
         raise GB2312Exception('Must be one character')
     try:
         bs = encode(c)
     except GB2312EncodeError as e:
         raise GB2312Exception(f"'{c}' is not a 'gb2312' character") from e
     if len(bs) == 1:
         raise GB2312Exception(f"'{c}' is a ascii character")
-    row = bs[0] - _euc_offset
-    col = bs[1] - _euc_offset
+    row = bs[0] - _EUC_OFFSET
+    col = bs[1] - _EUC_OFFSET
     return row, col
 
 
 def query_chr(row: int, col: int) -> str:
     if row < 1 or row > 94 or col < 1 or col > 94:
         raise GB2312Exception(f"'row' and 'col' must between 1 and 94")
     try:
-        return decode(bytes([row + _euc_offset, col + _euc_offset]))
+        return decode(bytes([row + _EUC_OFFSET, col + _EUC_OFFSET]))
     except GB2312DecodeError as e:
         raise GB2312Exception(f"'gb2312' coord at ({row}, {col}) is undefined'") from e
 
 
 def get_categories() -> list[str]:
     return ['other', 'level-1', 'level-2']
```

### Comparing `character-encoding-utils-0.0.4/src/character_encoding_utils/ksx1001.py` & `character-encoding-utils-0.0.5/src/character_encoding_utils/ksx1001.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-_euc_offset = 0xA0
+_EUC_OFFSET = 0xA0
 
 
 class KSX1001Exception(Exception):
     pass
 
 
 class KSX1001EncodeError(KSX1001Exception):
@@ -79,24 +79,24 @@
         bs = encode(c)
     except KSX1001EncodeError as e:
         raise KSX1001Exception(f"'{c}' is not a 'ksx1001' character") from e
     if len(bs) == 1:
         raise KSX1001Exception(f"'{c}' is a ascii character")
     elif bs.startswith(b'\xa4\xd4') and len(bs) > 2:
         raise KSX1001Exception(f"'{c}' is not a 'ksx1001' character")
-    row = bs[0] - _euc_offset
-    col = bs[1] - _euc_offset
+    row = bs[0] - _EUC_OFFSET
+    col = bs[1] - _EUC_OFFSET
     return row, col
 
 
 def query_chr(row: int, col: int):
     if row < 1 or row > 94 or col < 1 or col > 94:
         raise KSX1001Exception(f"'row' and 'col' must between 1 and 94")
     try:
-        return decode(bytes([row + _euc_offset, col + _euc_offset]))
+        return decode(bytes([row + _EUC_OFFSET, col + _EUC_OFFSET]))
     except KSX1001DecodeError as e:
         raise KSX1001Exception(f"'ksx1001' coord at ({row}, {col}) is undefined'") from e
 
 
 def get_categories() -> list[str]:
     return ['other', 'syllable', 'hanja']
```

### Comparing `character-encoding-utils-0.0.4/src/character_encoding_utils/shiftjis.py` & `character-encoding-utils-0.0.5/src/character_encoding_utils/shiftjis.py`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.4/src/character_encoding_utils.egg-info/PKG-INFO` & `character-encoding-utils-0.0.5/src/character_encoding_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: character-encoding-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Some character encoding utils.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/character-encoding-utils
 Project-URL: source, https://github.com/TakWolf/character-encoding-utils
 Project-URL: issues, https://github.com/TakWolf/character-encoding-utils/issues
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Character Encoding Utils
 
+[![Python](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/character-encoding-utils)](https://pypi.org/project/character-encoding-utils/)
 
 Some [character encoding](https://en.wikipedia.org/wiki/Character_encoding) utils.
 
 Now support:
 
 - [GB2312](https://en.wikipedia.org/wiki/GB_2312)
```

### Comparing `character-encoding-utils-0.0.4/src/character_encoding_utils.egg-info/SOURCES.txt` & `character-encoding-utils-0.0.5/src/character_encoding_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.4/tests/test_big5.py` & `character-encoding-utils-0.0.5/tests/test_big5.py`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.4/tests/test_gb2312.py` & `character-encoding-utils-0.0.5/tests/test_gb2312.py`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.4/tests/test_ksx1001.py` & `character-encoding-utils-0.0.5/tests/test_ksx1001.py`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.4/tests/test_shiftjis.py` & `character-encoding-utils-0.0.5/tests/test_shiftjis.py`

 * *Files identical despite different names*

