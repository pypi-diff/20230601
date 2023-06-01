# Comparing `tmp/escapyde-0.2.1.tar.gz` & `tmp/escapyde-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "escapyde-0.2.1.tar", max compression
+gzip compressed data, was "escapyde-0.2.2.tar", max compression
```

## Comparing `escapyde-0.2.1.tar` & `escapyde-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     4027 2023-02-09 05:05:02.312796 escapyde-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-02-09 05:05:02.312796 escapyde-0.2.1/LICENSE
--rw-r--r--   0        0        0      754 2023-02-09 05:05:02.312796 escapyde-0.2.1/README.md
--rw-r--r--   0        0        0      108 2023-02-09 05:05:02.312796 escapyde-0.2.1/escapyde/__init__.py
--rw-r--r--   0        0        0     2352 2023-02-09 05:05:02.312796 escapyde-0.2.1/escapyde/ansi.py
--rw-r--r--   0        0        0     2423 2023-02-09 05:05:02.312796 escapyde-0.2.1/escapyde/colours.py
--rw-r--r--   0        0        0        0 2023-02-09 05:05:02.312796 escapyde-0.2.1/escapyde/examples/__init__.py
--rw-r--r--   0        0        0     2441 2023-02-09 05:05:02.312796 escapyde-0.2.1/escapyde/examples/text.py
--rw-r--r--   0        0        0     2478 2023-02-09 05:05:02.312796 escapyde-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 escapyde-0.2.1/setup.py
--rw-r--r--   0        0        0     2957 1970-01-01 00:00:00.000000 escapyde-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4199 2023-06-01 20:39:50.043884 escapyde-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-06-01 20:39:50.043884 escapyde-0.2.2/LICENSE
+-rw-r--r--   0        0        0      754 2023-06-01 20:39:50.043884 escapyde-0.2.2/README.md
+-rw-r--r--   0        0        0      124 2023-06-01 20:39:50.043884 escapyde-0.2.2/escapyde/__init__.py
+-rw-r--r--   0        0        0     2550 2023-06-01 20:39:50.043884 escapyde-0.2.2/escapyde/ansi.py
+-rw-r--r--   0        0        0     2434 2023-06-01 20:39:50.043884 escapyde-0.2.2/escapyde/colours.py
+-rw-r--r--   0        0        0        0 2023-06-01 20:39:50.043884 escapyde-0.2.2/escapyde/examples/__init__.py
+-rw-r--r--   0        0        0     2441 2023-06-01 20:39:50.043884 escapyde-0.2.2/escapyde/examples/text.py
+-rw-r--r--   0        0        0     3640 2023-06-01 20:39:50.043884 escapyde-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2771 1970-01-01 00:00:00.000000 escapyde-0.2.2/PKG-INFO
```

### Comparing `escapyde-0.2.1/CHANGELOG.md` & `escapyde-0.2.2/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -45,33 +45,46 @@
 - Updated localisation files
 
 -->
 
 <!--
 _______________________________________________________________________________
 
-## [0.2.1] - 2023-02-09
+## [0.2.2] - 2023-06-01
 
-Updated metadata files, workflows, and dependencies.
+Updated dependencies, and added `py.typed` to show the package
+is type-hinted.
 
 ### Added
 
-- Added a whole bunch of new workflows
-- Added Dependabot auto-updates
-- Added a pull request template
+- Added `py.typed`
 
 ### Changed
 
 - Updated dependencies
-- Updated some metadata
 
 -->
 
 _______________________________________________________________________________
 
+## [0.2.2] - 2023-06-01
+
+Updated dependencies, and added `py.typed` to show the package
+is type-hinted.
+
+### Added
+
+- Added `py.typed`
+
+### Changed
+
+- Updated dependencies
+
+_______________________________________________________________________________
+
 ## [0.2.1] - 2023-02-09
 
 Updated metadata files, workflows, and dependencies.
 
 ### Added
 
 - Added a whole bunch of new workflows
```

### Comparing `escapyde-0.2.1/LICENSE` & `escapyde-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `escapyde-0.2.1/README.md` & `escapyde-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # escapyde
 
 Yet another ANSI escape sequence library for Python - now modernised!
 
 ## Installation
 
-The package is readily available on PyPI. There are no dependencies, but Python 3.6 or newer is required.
+The package is readily available on PyPI. There are no dependencies, but Python 3.9 or newer is required.
 
 On Windows:
 
 ```sh
 py -m pip install escapyde
 ```
```

### Comparing `escapyde-0.2.1/escapyde/ansi.py` & `escapyde-0.2.2/escapyde/ansi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,86 @@
 """Main ANSI Escape sequence class"""
 
-from typing import Any, Dict, Iterable, Optional
+from __future__ import annotations
 
-__all__ = ('AnsiEscape', 'escape_format',)
+from typing import TYPE_CHECKING, Any
+
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+
+__all__ = ('AnsiEscape', 'escape_format')
 
 _CLEAR: str = '\033[0m'
 
 
 class AnsiEscape:
     """Wrapper for ANSI escape sequences that makes use of operators as syntactic sugar"""
 
-    def __init__(self, colour: Optional[Iterable[int]] = None):
+    def __init__(self: AnsiEscape, colour: Iterable[int] | None = None) -> None:
         self.sequence: str = f'\033[{";".join(str(rgb) for rgb in colour)}m' if colour is not None else ''
-        self.string: Optional[str] = None
+        self.string: str | None = None
 
-    def __str__(self) -> str:
+    def __str__(self: AnsiEscape) -> str:
         if self.string:
             return self.sequence + self.string + _CLEAR
 
         return ''
 
-    def __or__(self, other: Any) -> 'AnsiEscape':
+    def __or__(self: AnsiEscape, other: Any) -> AnsiEscape:
         if isinstance(other, AnsiEscape):
             self.sequence += other.sequence
             return self
 
         self.string = str(other)
         return self
 
-    def __ror__(self, other: Any) -> 'AnsiEscape':
+    def __ror__(self: AnsiEscape, other: Any) -> AnsiEscape:
         return self.__or__(other)
 
 
-def escape_format(string: str, escape_map: Dict[str, AnsiEscape], case_sensitive: bool=False) -> str:
+def escape_format(string: str, escape_map: dict[str, AnsiEscape], case_sensitive: bool = False) -> str:
     """
     Maps a dictionary of substrings => escape sequences to the given string,
     returning a new string with the sequences applied to all
     found substrings.
 
     Example:
 
+    import escapyde as esc
+
     COLOURS = {
         'red': esc.FRED,
         'green': esc.FGREEN,
         'yellow': esc.FYELLOW,
         'blue': esc.FBLUE,
         'magenta': esc.FMAGENTA,
         'cyan': esc.FCYAN,
         'white': esc.FWHITE,
         'black': esc.FBLACK,
     }
 
     text = \"\"\"Hello, red world! The sun is bright yellow, and the sky cyan blue.
     Green, lush fields are all around us.\"\"\"
 
-    print(escape_format(text, COLOURS))  # Would print all mapped words in their respective colours
+    print(esc.escape_format(text, COLOURS))  # Would print all mapped words in their respective colours
 
     Inspired by: https://www.reddit.com/r/learnpython/comments/rvcg0l/print_colour_in_terminal/hr73v3f/
     """
 
     lines = string.splitlines()
     for line_idx, line in enumerate(lines):
 
         words = line.split(' ')
         for substring, escape in escape_map.items():
 
             for idx, word in enumerate(words):
 
                 if not case_sensitive:
-                    substring = substring.lower()
-                    word = word.lower()
+                    substring = substring.lower()  # noqa: PLW2901
+                    word = word.lower()  # noqa: PLW2901
 
                 if word.startswith(substring):
                     words[idx] = f'{escape | word[:len(substring)]}{word[len(substring):]}'
 
         lines[line_idx] = ' '.join(words)
 
     return '\n'.join(lines)
```

### Comparing `escapyde-0.2.1/escapyde/colours.py` & `escapyde-0.2.2/escapyde/colours.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Sequences for colours and text formatting"""
 
-from typing import Dict, Iterable
+from collections.abc import Iterable
 
-from .ansi import AnsiEscape
+from escapyde.ansi import AnsiEscape
 
 __all__ = (
     'FBLACK', 'FRED', 'FGREEN', 'FYELLOW',
     'FBLUE', 'FMAGENTA', 'FCYAN', 'FWHITE',
     'BBLACK', 'BRED', 'BGREEN', 'BYELLOW',
     'BBLUE', 'BMAGENTA', 'BCYAN', 'BWHITE',
     'CLEAR',
 )
 
-sequence_table: Dict[str, Iterable[int]] = {
+sequence_table: dict[str, Iterable[int]] = {
     # Dark colours
 
     # Foreground
     'fg_black': (0, 30),
     'fg_red': (0, 31),
     'fg_green': (0, 32),
     'fg_yellow': (0, 33),
```

### Comparing `escapyde-0.2.1/escapyde/examples/text.py` & `escapyde-0.2.2/escapyde/examples/text.py`

 * *Files identical despite different names*

### Comparing `escapyde-0.2.1/PKG-INFO` & `escapyde-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 Metadata-Version: 2.1
 Name: escapyde
-Version: 0.2.1
+Version: 0.2.2
 Summary: Yet another ANSI escape sequence library for Python - now modernised!
 Home-page: https://pypi.org/project/escapyde/
 License: MIT
-Keywords: ansi,console,terminal,escape,sequence
+Keywords: ansi,console,terminal,escape,sequence,colour,color
 Author: Lari Liuhamo
 Author-email: lari.liuhamo+pypi@gmail.com
 Maintainer: Lari Liuhamo
 Maintainer-email: lari.liuhamo+pypi@gmail.com
-Requires-Python: >=3.7.2,<4.0
+Requires-Python: >=3.9.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: IronPython
 Classifier: Programming Language :: Python :: Implementation :: Jython
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: Stackless
 Classifier: Topic :: Artistic Software
@@ -46,15 +42,15 @@
 
 # escapyde
 
 Yet another ANSI escape sequence library for Python - now modernised!
 
 ## Installation
 
-The package is readily available on PyPI. There are no dependencies, but Python 3.6 or newer is required.
+The package is readily available on PyPI. There are no dependencies, but Python 3.9 or newer is required.
 
 On Windows:
 
 ```sh
 py -m pip install escapyde
 ```
```

