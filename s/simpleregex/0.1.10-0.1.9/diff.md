# Comparing `tmp/simpleregex-0.1.10.tar.gz` & `tmp/simpleregex-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleregex-0.1.10.tar", last modified: Thu Jun  1 08:18:02 2023, max compression
+gzip compressed data, was "simpleregex-0.1.9.tar", last modified: Thu May 25 12:01:46 2023, max compression
```

## Comparing `simpleregex-0.1.10.tar` & `simpleregex-0.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 08:18:02.193656 simpleregex-0.1.10/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2023-06-01 08:16:42.000000 simpleregex-0.1.10/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3189 2023-06-01 08:18:02.193656 simpleregex-0.1.10/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2012 2023-06-01 08:16:42.000000 simpleregex-0.1.10/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-01 08:18:02.193656 simpleregex-0.1.10/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1371 2023-06-01 08:16:42.000000 simpleregex-0.1.10/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 08:18:02.189656 simpleregex-0.1.10/simpleregex/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      499 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/consts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2414 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/func.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/models.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 08:18:02.193656 simpleregex-0.1.10/simpleregex/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/test_any_of_characters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8982 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/test_email.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      833 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/test_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1201 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/test_look_ahead.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1261 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/test_look_behind.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1277 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/test_models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/test_negate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/test_none_or_many.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      534 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/test_none_or_one.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/test_one_or_more.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1035 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/test_regex_or.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/test_regex_range.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/test_repeat.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      485 2023-06-01 08:16:42.000000 simpleregex-0.1.10/simpleregex/tests/test_times.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 08:18:02.189656 simpleregex-0.1.10/simpleregex.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3189 2023-06-01 08:18:02.000000 simpleregex-0.1.10/simpleregex.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-06-01 08:18:02.000000 simpleregex-0.1.10/simpleregex.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-01 08:18:02.000000 simpleregex-0.1.10/simpleregex.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-06-01 08:18:02.000000 simpleregex-0.1.10/simpleregex.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 12:01:46.479632 simpleregex-0.1.9/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2023-05-25 12:01:04.000000 simpleregex-0.1.9/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2751 2023-05-25 12:01:46.479632 simpleregex-0.1.9/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1575 2023-05-25 12:01:04.000000 simpleregex-0.1.9/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-25 12:01:46.479632 simpleregex-0.1.9/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1370 2023-05-25 12:01:04.000000 simpleregex-0.1.9/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 12:01:46.475632 simpleregex-0.1.9/simpleregex/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      499 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/consts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2276 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/func.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/models.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 12:01:46.475632 simpleregex-0.1.9/simpleregex/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/test_any_of_characters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8982 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/test_email.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      833 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/test_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1201 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/test_look_ahead.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1261 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/test_look_behind.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1277 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/test_models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/test_negate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      418 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/test_none_or_many.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/test_none_or_one.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/test_one_or_more.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1035 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/test_regex_or.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/test_regex_range.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      326 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/test_repeat.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      485 2023-05-25 12:01:04.000000 simpleregex-0.1.9/simpleregex/tests/test_times.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 12:01:46.475632 simpleregex-0.1.9/simpleregex.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2751 2023-05-25 12:01:46.000000 simpleregex-0.1.9/simpleregex.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-05-25 12:01:46.000000 simpleregex-0.1.9/simpleregex.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-25 12:01:46.000000 simpleregex-0.1.9/simpleregex.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-25 12:01:46.000000 simpleregex-0.1.9/simpleregex.egg-info/top_level.txt
```

### Comparing `simpleregex-0.1.10/LICENSE` & `simpleregex-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleregex-0.1.10/PKG-INFO` & `simpleregex-0.1.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleregex
-Version: 0.1.10
+Version: 0.1.9
 Summary: Wrapper for RegEx, made so the RegEx code will be understandable
 Home-page: https://github.com/netguru/SimpleRegEx
 Download-URL: https://pypi.org/project/simpleregex/
 Author: Netguru
 Author-email: hello@netguru.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://github.com/netguru/SimpleRegEx/blob/main/docs/index.md
@@ -44,52 +44,47 @@
 
 <p align="center">
   Readability counts. Even in regex.
 </p>
 
 <div align="center">
 
-[Documentation](https://github.com/netguru/SimpleRegEx/blob/main/docs/index.md) &nbsp;|&nbsp;
+[Documentation](./docs/index.md) &nbsp;|&nbsp;
 [About](#about) &nbsp;|&nbsp;
 [Installation](#installation) &nbsp;|&nbsp;
-[Contributing](https://github.com/netguru/SimpleRegEx/blob/main/docs/CONTRIBUTING.md) &nbsp;
+[Contributing](./docs/CONTRIBUTING.md) &nbsp;
 
 </div>
 
-# <a name="about"></a>About
+# About
 
 This tool is a wrapper for RegEx in python (`import re`), which introduces pattern
 functions in place of unreadable text patterns.
 
 This tool is inspired by the [Magic Regex](https://github.com/danielroe/magic-regexp) tool.
 
 # In Use
 
 Usage example can be found
 in [unit tests](https://github.com/netguru/SimpleRegEx/blob/main/simpleregex/tests/test_email.py).
 
-# <a name="installation"></a>Installation
+# Installation
 
 ```
 pip install simpleregex
 ```
 
 # Release
 
-To bump a package version go to [setup.py](https://github.com/netguru/SimpleRegEx/blob/main/setup.py) and
-change `version` variable.
+To bump a package version use poetry. Examples can be found
+in [poetry docs](https://python-poetry.org/docs/cli/#version).
 
-Create new release on GitHub and tag it with the same version as in `setup.py`.
-
-The release process to `testpypi` and `pypi` is manually triggered on CircleCi.
-After successful merge to main and creation of new release tag, go to
-[CircleCi](https://app.circleci.com/pipelines/github/netguru/SimpleRegEx?branch=main) and trigger new pipeline with
-following boolean parameters:
-- `pypi_publish: true` - this will push package to `pypi`
-- `testpypi_publish: true` - this will push package to `testpypi`
+The release process is automated on circle ci.
+Merge to main branch will deploy automated release to test.pypi.org.
+To release the new package version to pypi.org create a tag for selected version `v\d+\.\d+\.\d+`.
 
 # Support
 
 Supported python versions:
 
 - 3.11
 - 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simpleregex Version: 0.1.10 Summary: Wrapper for
+Metadata-Version: 2.1 Name: simpleregex Version: 0.1.9 Summary: Wrapper for
 RegEx, made so the RegEx code will be understandable Home-page: https://
 github.com/netguru/SimpleRegEx Download-URL: https://pypi.org/project/
 simpleregex/ Author: Netguru Author-email: hello@netguru.com License: BSD-3-
 Clause Project-URL: Documentation, https://github.com/netguru/SimpleRegEx/blob/
 main/docs/index.md Project-URL: Source, https://github.com/netguru/SimpleRegEx
 Project-URL: Tracker, https://github.com/netguru/SimpleRegEx/issues Classifier:
 Environment :: MacOS X Classifier: Environment :: Win32 (MS Windows)
@@ -16,25 +16,20 @@
 Content-Type: text/markdown License-File: LICENSE
                           ****** Simple RegEx ******
                                [CircleCI status]
 
                     Brought with â¤ï¸ by  [Netguru_logo]
 # Introduction
                       Readability counts. Even in regex.
-[Documentation](https://github.com/netguru/SimpleRegEx/blob/main/docs/index.md)
- |  [About](#about)  |  [Installation](#installation)  |  [Contributing](https:
-      //github.com/netguru/SimpleRegEx/blob/main/docs/CONTRIBUTING.md)  
+    [Documentation](./docs/index.md)  |  [About](#about)  |  [Installation]
+         (#installation)  |  [Contributing](./docs/CONTRIBUTING.md)  
 # About This tool is a wrapper for RegEx in python (`import re`), which
 introduces pattern functions in place of unreadable text patterns. This tool is
 inspired by the [Magic Regex](https://github.com/danielroe/magic-regexp) tool.
 # In Use Usage example can be found in [unit tests](https://github.com/netguru/
 SimpleRegEx/blob/main/simpleregex/tests/test_email.py). # Installation ``` pip
-install simpleregex ``` # Release To bump a package version go to [setup.py]
-(https://github.com/netguru/SimpleRegEx/blob/main/setup.py) and change
-`version` variable. Create new release on GitHub and tag it with the same
-version as in `setup.py`. The release process to `testpypi` and `pypi` is
-manually triggered on CircleCi. After successful merge to main and creation of
-new release tag, go to [CircleCi](https://app.circleci.com/pipelines/github/
-netguru/SimpleRegEx?branch=main) and trigger new pipeline with following
-boolean parameters: - `pypi_publish: true` - this will push package to `pypi` -
-`testpypi_publish: true` - this will push package to `testpypi` # Support
-Supported python versions: - 3.11 - 3.10 - 3.9 - 3.8
+install simpleregex ``` # Release To bump a package version use poetry.
+Examples can be found in [poetry docs](https://python-poetry.org/docs/cli/
+#version). The release process is automated on circle ci. Merge to main branch
+will deploy automated release to test.pypi.org. To release the new package
+version to pypi.org create a tag for selected version `v\d+\.\d+\.\d+`. #
+Support Supported python versions: - 3.11 - 3.10 - 3.9 - 3.8
```

### Comparing `simpleregex-0.1.10/setup.py` & `simpleregex-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup_info = dict(
     name="simpleregex",
-    version="0.1.10",
+    version="0.1.9",
     author="Netguru",
     author_email="hello@netguru.com",
     url="https://github.com/netguru/SimpleRegEx",
     download_url="https://pypi.org/project/simpleregex/",
     project_urls={
         "Documentation": "https://github.com/netguru/SimpleRegEx/blob/main/docs/index.md",
         "Source": "https://github.com/netguru/SimpleRegEx",
```

### Comparing `simpleregex-0.1.10/simpleregex/func.py` & `simpleregex-0.1.9/simpleregex/func.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 from typing import Union
 
 from simpleregex.models import ensure_regex
 from simpleregex.models import RegEx
 
 
 def none_or_many(what: RegEx):
-    what = ensure_regex(what)
-    return RegEx(_patterns=[f"({what.pattern})*"])
+    return ensure_regex(what) + "*"
 
 
 def one_or_more(what: RegEx):
-    what = ensure_regex(what)
-    return RegEx(_patterns=[f"({what.pattern})+"])
+    return ensure_regex(what) + "+"
 
 
 def none_or_one(what: RegEx):
     return ensure_regex(what) + "?"
 
 
 def regex_range(min: str, max: str):
@@ -62,32 +60,31 @@
         else:
             what += ensure_regex(item)
     return what + "]"
 
 
 def times(what: RegEx, min: int, max: int = None):
     """
-    Repeat a pattern between {min} and {max} times.
+    Repeate a pattern between {min} and {max} times.
     """
     what = ensure_regex(what)
     return what + (f"{{{min},}}" if max is None else f"{{{min},{max}}}")
 
 
 def repeat(what: RegEx, count: int):
     """
-    Repeat a pattern {count} times.
+    Repeate a pattern {count} times.
     """
-    what = ensure_regex(what)
-    return RegEx(_patterns=[f"({what.pattern}){{{count}}}"])
+    return ensure_regex(what) + f"{{{count}}}"
 
 
 def negate(what: RegEx):
     """
     Negate either exact characters or ranges.
-    To negate entire expressions, utilize negative lookarounds.
+    To Negate whole expressions use negative lookarounds.
     """
     what = ensure_regex(what)
     if what._patterns[0] == "[":
         what._patterns.insert(1, "^")
         return what
     else:
         return _wrap_regex(what, f"[^", "]")
```

### Comparing `simpleregex-0.1.10/simpleregex/models.py` & `simpleregex-0.1.9/simpleregex/models.py`

 * *Files identical despite different names*

### Comparing `simpleregex-0.1.10/simpleregex/tests/test_any_of_characters.py` & `simpleregex-0.1.9/simpleregex/tests/test_any_of_characters.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,22 +16,22 @@
         re_match = (
             any_of_characters(["a", "b"]).compile().search("ZzAbaaabbbaaa")
         )
         assert re_match[0] == "b"
 
     def test_string(self):
         """
-        any_of_characters should also accept string instead of list
+        any_of_characters should also except string instead of list
         """
         re_match = any_of_characters("ab").compile().search("ZzAbaaabbbaaa")
         assert re_match[0] == "b"
 
     def test_with_regex_range(self):
         """
-        any_of_characters should also accept regex range object
+        any_of_characters should also except regex range object
         """
         regex = any_of_characters(
             [
                 regex_range("a", "z"),
                 regex_range(
                     0,
                     9,
@@ -43,15 +43,15 @@
         assert regex.pattern == "[a-z0-9-]"
 
         re_match = regex.search("ZzAbaaabbbaaa")
         assert re_match[0] == "z"
 
     def test_with_regex_object(self):
         """
-        any_of_characters should also accept regex object
+        any_of_characters should also except regex object
         """
         regex = any_of_characters(
             [RegEx("a-z"), RegEx(["0", "-", "9"]), "-"]
         ).compile()
 
         assert regex.pattern == "[a-z0-9-]"
```

### Comparing `simpleregex-0.1.10/simpleregex/tests/test_email.py` & `simpleregex-0.1.9/simpleregex/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `simpleregex-0.1.10/simpleregex/tests/test_group.py` & `simpleregex-0.1.9/simpleregex/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `simpleregex-0.1.10/simpleregex/tests/test_look_ahead.py` & `simpleregex-0.1.9/simpleregex/tests/test_look_ahead.py`

 * *Files identical despite different names*

### Comparing `simpleregex-0.1.10/simpleregex/tests/test_look_behind.py` & `simpleregex-0.1.9/simpleregex/tests/test_look_behind.py`

 * *Files identical despite different names*

### Comparing `simpleregex-0.1.10/simpleregex/tests/test_models.py` & `simpleregex-0.1.9/simpleregex/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `simpleregex-0.1.10/simpleregex/tests/test_negate.py` & `simpleregex-0.1.9/simpleregex/tests/test_negate.py`

 * *Files identical despite different names*

### Comparing `simpleregex-0.1.10/simpleregex/tests/test_regex_or.py` & `simpleregex-0.1.9/simpleregex/tests/test_regex_or.py`

 * *Files identical despite different names*

### Comparing `simpleregex-0.1.10/simpleregex.egg-info/PKG-INFO` & `simpleregex-0.1.9/simpleregex.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleregex
-Version: 0.1.10
+Version: 0.1.9
 Summary: Wrapper for RegEx, made so the RegEx code will be understandable
 Home-page: https://github.com/netguru/SimpleRegEx
 Download-URL: https://pypi.org/project/simpleregex/
 Author: Netguru
 Author-email: hello@netguru.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://github.com/netguru/SimpleRegEx/blob/main/docs/index.md
@@ -44,52 +44,47 @@
 
 <p align="center">
   Readability counts. Even in regex.
 </p>
 
 <div align="center">
 
-[Documentation](https://github.com/netguru/SimpleRegEx/blob/main/docs/index.md) &nbsp;|&nbsp;
+[Documentation](./docs/index.md) &nbsp;|&nbsp;
 [About](#about) &nbsp;|&nbsp;
 [Installation](#installation) &nbsp;|&nbsp;
-[Contributing](https://github.com/netguru/SimpleRegEx/blob/main/docs/CONTRIBUTING.md) &nbsp;
+[Contributing](./docs/CONTRIBUTING.md) &nbsp;
 
 </div>
 
-# <a name="about"></a>About
+# About
 
 This tool is a wrapper for RegEx in python (`import re`), which introduces pattern
 functions in place of unreadable text patterns.
 
 This tool is inspired by the [Magic Regex](https://github.com/danielroe/magic-regexp) tool.
 
 # In Use
 
 Usage example can be found
 in [unit tests](https://github.com/netguru/SimpleRegEx/blob/main/simpleregex/tests/test_email.py).
 
-# <a name="installation"></a>Installation
+# Installation
 
 ```
 pip install simpleregex
 ```
 
 # Release
 
-To bump a package version go to [setup.py](https://github.com/netguru/SimpleRegEx/blob/main/setup.py) and
-change `version` variable.
+To bump a package version use poetry. Examples can be found
+in [poetry docs](https://python-poetry.org/docs/cli/#version).
 
-Create new release on GitHub and tag it with the same version as in `setup.py`.
-
-The release process to `testpypi` and `pypi` is manually triggered on CircleCi.
-After successful merge to main and creation of new release tag, go to
-[CircleCi](https://app.circleci.com/pipelines/github/netguru/SimpleRegEx?branch=main) and trigger new pipeline with
-following boolean parameters:
-- `pypi_publish: true` - this will push package to `pypi`
-- `testpypi_publish: true` - this will push package to `testpypi`
+The release process is automated on circle ci.
+Merge to main branch will deploy automated release to test.pypi.org.
+To release the new package version to pypi.org create a tag for selected version `v\d+\.\d+\.\d+`.
 
 # Support
 
 Supported python versions:
 
 - 3.11
 - 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simpleregex Version: 0.1.10 Summary: Wrapper for
+Metadata-Version: 2.1 Name: simpleregex Version: 0.1.9 Summary: Wrapper for
 RegEx, made so the RegEx code will be understandable Home-page: https://
 github.com/netguru/SimpleRegEx Download-URL: https://pypi.org/project/
 simpleregex/ Author: Netguru Author-email: hello@netguru.com License: BSD-3-
 Clause Project-URL: Documentation, https://github.com/netguru/SimpleRegEx/blob/
 main/docs/index.md Project-URL: Source, https://github.com/netguru/SimpleRegEx
 Project-URL: Tracker, https://github.com/netguru/SimpleRegEx/issues Classifier:
 Environment :: MacOS X Classifier: Environment :: Win32 (MS Windows)
@@ -16,25 +16,20 @@
 Content-Type: text/markdown License-File: LICENSE
                           ****** Simple RegEx ******
                                [CircleCI status]
 
                     Brought with â¤ï¸ by  [Netguru_logo]
 # Introduction
                       Readability counts. Even in regex.
-[Documentation](https://github.com/netguru/SimpleRegEx/blob/main/docs/index.md)
- |  [About](#about)  |  [Installation](#installation)  |  [Contributing](https:
-      //github.com/netguru/SimpleRegEx/blob/main/docs/CONTRIBUTING.md)  
+    [Documentation](./docs/index.md)  |  [About](#about)  |  [Installation]
+         (#installation)  |  [Contributing](./docs/CONTRIBUTING.md)  
 # About This tool is a wrapper for RegEx in python (`import re`), which
 introduces pattern functions in place of unreadable text patterns. This tool is
 inspired by the [Magic Regex](https://github.com/danielroe/magic-regexp) tool.
 # In Use Usage example can be found in [unit tests](https://github.com/netguru/
 SimpleRegEx/blob/main/simpleregex/tests/test_email.py). # Installation ``` pip
-install simpleregex ``` # Release To bump a package version go to [setup.py]
-(https://github.com/netguru/SimpleRegEx/blob/main/setup.py) and change
-`version` variable. Create new release on GitHub and tag it with the same
-version as in `setup.py`. The release process to `testpypi` and `pypi` is
-manually triggered on CircleCi. After successful merge to main and creation of
-new release tag, go to [CircleCi](https://app.circleci.com/pipelines/github/
-netguru/SimpleRegEx?branch=main) and trigger new pipeline with following
-boolean parameters: - `pypi_publish: true` - this will push package to `pypi` -
-`testpypi_publish: true` - this will push package to `testpypi` # Support
-Supported python versions: - 3.11 - 3.10 - 3.9 - 3.8
+install simpleregex ``` # Release To bump a package version use poetry.
+Examples can be found in [poetry docs](https://python-poetry.org/docs/cli/
+#version). The release process is automated on circle ci. Merge to main branch
+will deploy automated release to test.pypi.org. To release the new package
+version to pypi.org create a tag for selected version `v\d+\.\d+\.\d+`. #
+Support Supported python versions: - 3.11 - 3.10 - 3.9 - 3.8
```

### Comparing `simpleregex-0.1.10/simpleregex.egg-info/SOURCES.txt` & `simpleregex-0.1.9/simpleregex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

