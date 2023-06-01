# Comparing `tmp/unidata-blocks-0.0.2.tar.gz` & `tmp/unidata-blocks-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unidata-blocks-0.0.2.tar", last modified: Tue May 16 07:57:49 2023, max compression
+gzip compressed data, was "unidata-blocks-0.0.3.tar", last modified: Thu Jun  1 03:30:11 2023, max compression
```

## Comparing `unidata-blocks-0.0.2.tar` & `unidata-blocks-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 07:57:32.000000 unidata-blocks-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-16 07:57:32.000000 unidata-blocks-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-16 07:57:32.000000 unidata-blocks-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/src/unidata_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-16 07:57:32.000000 unidata-blocks-0.0.2/src/unidata_blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/src/unidata_blocks/unidata/
--rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-05-16 07:57:32.000000 unidata-blocks-0.0.2/src/unidata_blocks/unidata/Blocks.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/src/unidata_blocks/unidata/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-05-16 07:57:32.000000 unidata-blocks-0.0.2/src/unidata_blocks/unidata/i18n/zh-cn.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/src/unidata_blocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-16 07:57:49.000000 unidata-blocks-0.0.2/src/unidata_blocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 07:57:49.000000 unidata-blocks-0.0.2/src/unidata_blocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 07:57:49.000000 unidata-blocks-0.0.2/src/unidata_blocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 07:57:49.000000 unidata-blocks-0.0.2/src/unidata_blocks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-16 07:57:32.000000 unidata-blocks-0.0.2/tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 03:30:01.000000 unidata-blocks-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-01 03:30:01.000000 unidata-blocks-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-01 03:30:01.000000 unidata-blocks-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/src/unidata_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-01 03:30:01.000000 unidata-blocks-0.0.3/src/unidata_blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/src/unidata_blocks/unidata/
+-rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-06-01 03:30:01.000000 unidata-blocks-0.0.3/src/unidata_blocks/unidata/Blocks.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/src/unidata_blocks/unidata/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-06-01 03:30:01.000000 unidata-blocks-0.0.3/src/unidata_blocks/unidata/i18n/zh-cn.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/src/unidata_blocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-01 03:30:11.000000 unidata-blocks-0.0.3/src/unidata_blocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-01 03:30:11.000000 unidata-blocks-0.0.3/src/unidata_blocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 03:30:11.000000 unidata-blocks-0.0.3/src/unidata_blocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 03:30:11.000000 unidata-blocks-0.0.3/src/unidata_blocks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-01 03:30:01.000000 unidata-blocks-0.0.3/tests/test_query.py
```

### Comparing `unidata-blocks-0.0.2/LICENSE` & `unidata-blocks-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unidata-blocks-0.0.2/PKG-INFO` & `unidata-blocks-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidata-blocks
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library that helps query unicode blocks by Blocks.txt.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/unidata-blocks
 Project-URL: source, https://github.com/TakWolf/unidata-blocks
 Project-URL: issues, https://github.com/TakWolf/unidata-blocks/issues
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Unidata Blocks
 
+[![Python](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/unidata-blocks)](https://pypi.org/project/unidata-blocks/)
 
 A library that helps query unicode blocks by [Blocks.txt](https://www.unicode.org/Public/UNIDATA/Blocks.txt).
 
 ## Installation
 
 ```commandline
```

### Comparing `unidata-blocks-0.0.2/README.md` & `unidata-blocks-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Unidata Blocks
 
+[![Python](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/unidata-blocks)](https://pypi.org/project/unidata-blocks/)
 
 A library that helps query unicode blocks by [Blocks.txt](https://www.unicode.org/Public/UNIDATA/Blocks.txt).
 
 ## Installation
 
 ```commandline
```

### Comparing `unidata-blocks-0.0.2/pyproject.toml` & `unidata-blocks-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "unidata-blocks"
-version = "0.0.2"
+version = "0.0.3"
 description = "A library that helps query unicode blocks by Blocks.txt."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `unidata-blocks-0.0.2/src/unidata_blocks/__init__.py` & `unidata-blocks-0.0.3/src/unidata_blocks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pkgutil
 import re
 
-_locale_to_localized_names = {}
+_locale_to_localized_names: dict[str, dict[str, str]] = {}
 
 
 def _get_localized_names(locale: str) -> dict[str, str]:
-    locale = locale.lower().replace('_', '-')
     if locale in _locale_to_localized_names:
         return _locale_to_localized_names[locale]
     localized_names = {}
     try:
         data = pkgutil.get_data(__package__, f'unidata/i18n/{locale}.txt')
     except FileNotFoundError:
         data = None
@@ -38,14 +37,15 @@
             if c.isprintable():
                 self.printable_count += 1
 
     def __str__(self):
         return f'{self.code_start:04X}..{self.code_end:04X}; {self.name}'
 
     def name_localized(self, locale: str) -> str | None:
+        locale = locale.lower().replace('_', '-')
         if locale == 'en':
             return self.name
         return _get_localized_names(locale).get(self.name, None)
 
 
 def _load_blocks() -> tuple[str, list[UnicodeBlock]]:
     blocks = []
@@ -59,28 +59,32 @@
         code_start = int(tokens[0], 16)
         code_end = int(tokens[1], 16)
         name = tokens[2]
         blocks.append(UnicodeBlock(code_start, code_end, name))
     return version, blocks
 
 
+def _normalize_block_name(name: str) -> str:
+    return name.lower().replace('-', ' ').replace('_', ' ')
+
+
 unicode_version, _blocks = _load_blocks()
-_name_to_block = {block.name.lower().replace(' ', '_').replace('-', '_'): block for block in _blocks}
+_name_to_block: dict[str, UnicodeBlock] = {_normalize_block_name(block.name): block for block in _blocks}
 
 
 def get_block_by_code_point(code_point: int) -> UnicodeBlock | None:
     if _blocks[0].code_start <= code_point <= _blocks[-1].code_end:
         for block in _blocks:
             if block.code_start <= code_point <= block.code_end:
                 return block
     return None
 
 
 def get_block_by_name(name: str) -> UnicodeBlock | None:
-    return _name_to_block.get(name.lower().replace(' ', '_').replace('-', '_'), None)
+    return _name_to_block.get(_normalize_block_name(name), None)
 
 
 def get_block_by_chr(c: str) -> UnicodeBlock | None:
     return get_block_by_code_point(ord(c))
 
 
 def get_blocks() -> list[UnicodeBlock]:
```

### Comparing `unidata-blocks-0.0.2/src/unidata_blocks/unidata/Blocks.txt` & `unidata-blocks-0.0.3/src/unidata_blocks/unidata/Blocks.txt`

 * *Files identical despite different names*

### Comparing `unidata-blocks-0.0.2/src/unidata_blocks/unidata/i18n/zh-cn.txt` & `unidata-blocks-0.0.3/src/unidata_blocks/unidata/i18n/zh-cn.txt`

 * *Files identical despite different names*

### Comparing `unidata-blocks-0.0.2/src/unidata_blocks.egg-info/PKG-INFO` & `unidata-blocks-0.0.3/src/unidata_blocks.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidata-blocks
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library that helps query unicode blocks by Blocks.txt.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/unidata-blocks
 Project-URL: source, https://github.com/TakWolf/unidata-blocks
 Project-URL: issues, https://github.com/TakWolf/unidata-blocks/issues
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Unidata Blocks
 
+[![Python](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/unidata-blocks)](https://pypi.org/project/unidata-blocks/)
 
 A library that helps query unicode blocks by [Blocks.txt](https://www.unicode.org/Public/UNIDATA/Blocks.txt).
 
 ## Installation
 
 ```commandline
```

### Comparing `unidata-blocks-0.0.2/tests/test_query.py` & `unidata-blocks-0.0.3/tests/test_query.py`

 * *Files 11% similar despite different names*

```diff
@@ -70,16 +70,18 @@
     block = unidata_blocks.get_block_by_code_point(0x100000)
     assert str(block) == '100000..10FFFF; Supplementary Private Use Area-B'
 
 
 def test_i18n():
     block = unidata_blocks.get_block_by_code_point(0x0000)
     assert block.name_localized('en') == 'Basic Latin'
+    assert block.name_localized('EN') == 'Basic Latin'
     assert block.name_localized('zh-cn') == '基本拉丁'
     assert block.name_localized('ZH_CN') == '基本拉丁'
     assert block.name_localized('no-locale') is None
 
     block = unidata_blocks.get_block_by_code_point(0x4E00)
     assert block.name_localized('en') == 'CJK Unified Ideographs'
+    assert block.name_localized('EN') == 'CJK Unified Ideographs'
     assert block.name_localized('zh-cn') == '中日韩统一表意文字'
     assert block.name_localized('ZH_CN') == '中日韩统一表意文字'
     assert block.name_localized('no-locale') is None
```

