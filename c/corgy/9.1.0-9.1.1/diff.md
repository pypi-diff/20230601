# Comparing `tmp/corgy-9.1.0.tar.gz` & `tmp/corgy-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corgy-9.1.0.tar", max compression
+gzip compressed data, was "corgy-9.1.1.tar", max compression
```

## Comparing `corgy-9.1.0.tar` & `corgy-9.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    31893 2023-05-24 21:57:06.521003 corgy-9.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2023-05-24 21:57:06.521003 corgy-9.1.0/LICENSE
--rw-r--r--   0        0        0     4196 2023-05-24 21:57:06.521003 corgy-9.1.0/README.md
--rw-r--r--   0        0        0      468 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/__init__.py
--rw-r--r--   0        0        0     2329 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/_actions.py
--rw-r--r--   0        0        0      505 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/_annotations.py
--rw-r--r--   0        0        0    53646 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/_corgy.py
--rw-r--r--   0        0        0     3202 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/_corgychecker.py
--rw-r--r--   0        0        0     6237 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/_corgyparser.py
--rw-r--r--   0        0        0    36993 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/_helpfmt.py
--rw-r--r--   0        0        0    19746 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/_meta.py
--rw-r--r--   0        0        0       64 2023-05-24 21:57:45.793051 corgy-9.1.0/corgy/_version.py
--rw-r--r--   0        0        0        0 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/py.typed
--rw-r--r--   0        0        0     1598 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/types/__init__.py
--rw-r--r--   0        0        0     2382 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/types/_expand.py
--rw-r--r--   0        0        0     3750 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/types/_initargs.py
--rw-r--r--   0        0        0     2777 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/types/_inputfile.py
--rw-r--r--   0        0        0     5464 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/types/_keyvaluepairs.py
--rw-r--r--   0        0        0     5271 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/types/_outputfile.py
--rw-r--r--   0        0        0     9846 2023-05-24 21:57:06.521003 corgy-9.1.0/corgy/types/_subclass.py
--rw-r--r--   0        0        0    36201 2023-05-24 21:57:06.521003 corgy-9.1.0/docs/corgy.md
--rw-r--r--   0        0        0    11884 2023-05-24 21:57:06.521003 corgy-9.1.0/docs/corgy.types.md
--rw-r--r--   0        0        0      132 2023-05-24 21:57:06.521003 corgy-9.1.0/docs/index.md
--rw-r--r--   0        0        0     2697 2023-05-24 21:57:45.793051 corgy-9.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 21:57:06.521003 corgy-9.1.0/tests/__init__.py
--rw-r--r--   0        0        0    94529 2023-05-24 21:57:06.521003 corgy-9.1.0/tests/test_corgy.py
--rw-r--r--   0        0        0     4753 2023-05-24 21:57:06.521003 corgy-9.1.0/tests/test_corgychecker.py
--rw-r--r--   0        0        0    20305 2023-05-24 21:57:06.521003 corgy-9.1.0/tests/test_corgyparser.py
--rw-r--r--   0        0        0      800 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/test_doctests.py
--rw-r--r--   0        0        0    47095 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/test_helpfmt.py
--rw-r--r--   0        0        0        0 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/__init__.py
--rw-r--r--   0        0        0      328 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/_pklclasses.py
--rw-r--r--   0        0        0     2002 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/_specialtmps.py
--rw-r--r--   0        0        0     3356 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/_test_file.py
--rw-r--r--   0        0        0     2678 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/test_initargs.py
--rw-r--r--   0        0        0     2496 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/test_inputfiles.py
--rw-r--r--   0        0        0     5443 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/test_keyvaluepairs.py
--rw-r--r--   0        0        0     5122 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/test_outputfiles.py
--rw-r--r--   0        0        0     7082 2023-05-24 21:57:06.525003 corgy-9.1.0/tests/types/test_subclass.py
--rw-r--r--   0        0        0     5497 1970-01-01 00:00:00.000000 corgy-9.1.0/PKG-INFO
+-rw-r--r--   0        0        0    32171 2023-06-01 13:42:06.222186 corgy-9.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2023-06-01 13:42:06.222186 corgy-9.1.1/LICENSE
+-rw-r--r--   0        0        0     4196 2023-06-01 13:42:06.222186 corgy-9.1.1/README.md
+-rw-r--r--   0        0        0      468 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/__init__.py
+-rw-r--r--   0        0        0     2329 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/_actions.py
+-rw-r--r--   0        0        0      505 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/_annotations.py
+-rw-r--r--   0        0        0    53646 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/_corgy.py
+-rw-r--r--   0        0        0     3202 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/_corgychecker.py
+-rw-r--r--   0        0        0     6237 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/_corgyparser.py
+-rw-r--r--   0        0        0    37670 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/_helpfmt.py
+-rw-r--r--   0        0        0    19746 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/_meta.py
+-rw-r--r--   0        0        0       64 2023-06-01 13:42:46.770316 corgy-9.1.1/corgy/_version.py
+-rw-r--r--   0        0        0        0 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/py.typed
+-rw-r--r--   0        0        0     1598 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/types/__init__.py
+-rw-r--r--   0        0        0     2382 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/types/_expand.py
+-rw-r--r--   0        0        0     3750 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/types/_initargs.py
+-rw-r--r--   0        0        0     2777 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/types/_inputfile.py
+-rw-r--r--   0        0        0     5464 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/types/_keyvaluepairs.py
+-rw-r--r--   0        0        0     5271 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/types/_outputfile.py
+-rw-r--r--   0        0        0     9846 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/types/_subclass.py
+-rw-r--r--   0        0        0    36201 2023-06-01 13:42:06.226186 corgy-9.1.1/docs/corgy.md
+-rw-r--r--   0        0        0    11884 2023-06-01 13:42:06.226186 corgy-9.1.1/docs/corgy.types.md
+-rw-r--r--   0        0        0      132 2023-06-01 13:42:06.226186 corgy-9.1.1/docs/index.md
+-rw-r--r--   0        0        0     2697 2023-06-01 13:42:46.770316 corgy-9.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    94529 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/test_corgy.py
+-rw-r--r--   0        0        0     4753 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/test_corgychecker.py
+-rw-r--r--   0        0        0    20305 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/test_corgyparser.py
+-rw-r--r--   0        0        0      800 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/test_doctests.py
+-rw-r--r--   0        0        0    49021 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/test_helpfmt.py
+-rw-r--r--   0        0        0        0 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/__init__.py
+-rw-r--r--   0        0        0      328 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/_pklclasses.py
+-rw-r--r--   0        0        0     2002 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/_specialtmps.py
+-rw-r--r--   0        0        0     3356 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/_test_file.py
+-rw-r--r--   0        0        0     2678 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/test_initargs.py
+-rw-r--r--   0        0        0     2496 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/test_inputfiles.py
+-rw-r--r--   0        0        0     5443 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/test_keyvaluepairs.py
+-rw-r--r--   0        0        0     5122 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/test_outputfiles.py
+-rw-r--r--   0        0        0     7082 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/test_subclass.py
+-rw-r--r--   0        0        0     5497 1970-01-01 00:00:00.000000 corgy-9.1.1/PKG-INFO
```

### Comparing `corgy-9.1.0/CHANGELOG.md` & `corgy-9.1.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+### [9.1.1](https://github.com/jayanthkoushik/corgy/compare/v9.1.0...v9.1.1) (2023-06-01)
+
+
+### Bug Fixes
+
+* fallback to base formatting for subparsers in `CorgyHelpFormatter` ([87dede1](https://github.com/jayanthkoushik/corgy/commit/87dede132403735a584e2ed83de85b739877f86a))
+
 ## [9.1.0](https://github.com/jayanthkoushik/corgy/compare/v9.0.0...v9.1.0) (2023-05-24)
 
 
 ### Features
 
 * add support for `Self` type annotations ([b33ec24](https://github.com/jayanthkoushik/corgy/commit/b33ec24ad762c1dd0655ad4a5af847eb16f15b55))
```

### Comparing `corgy-9.1.0/LICENSE` & `corgy-9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/README.md` & `corgy-9.1.1/README.md`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/corgy/_actions.py` & `corgy-9.1.1/corgy/_actions.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/corgy/_corgy.py` & `corgy-9.1.1/corgy/_corgy.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/corgy/_corgychecker.py` & `corgy-9.1.1/corgy/_corgychecker.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/corgy/_corgyparser.py` & `corgy-9.1.1/corgy/_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/corgy/_helpfmt.py` & `corgy-9.1.1/corgy/_helpfmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import argparse
 import inspect
 import re
 import sys
 import textwrap
-from argparse import Action, ArgumentParser, HelpFormatter
+from argparse import _SubParsersAction, Action, ArgumentParser, HelpFormatter
 from collections.abc import Sequence as AbstractSequence
 from functools import lru_cache, partial
 from importlib import import_module
 from itertools import cycle, zip_longest
 from shutil import get_terminal_size
 from types import ModuleType
 from typing import Optional, Sequence, Tuple, Union
@@ -435,14 +435,17 @@
         return ""
 
     def _get_default_metavar_for_optional(self, action: Action) -> str:
         return self._get_default_metavar_for_type(action.type, self.using_colors)
 
     def _format_action_invocation(self, action: Action) -> str:
         """Format the invocation part of an argument, e.g. `-x, --x int`."""
+        if isinstance(action, _SubParsersAction):
+            return super()._format_action_invocation(action)
+
         if action.option_strings:
             option_strings = action.option_strings
         else:
             # If no option strings are present, (positional arguments), use
             # `action.dest`. However, this can be `argparse.SUPPRESS` for sub-actions,
             # in which case use the word `CMD`.
             option_strings = [
@@ -466,17 +469,16 @@
             "option_strings",
             [self.marker_choices_sep.join(placeholder_option_strings)],
         ):
             return super()._format_action_invocation(action).rstrip()
 
     def _format_args(self, action: Action, default_metavar: Optional[str]) -> str:
         """Format the metavars."""
-        if action.nargs == argparse.PARSER:
-            # No metavars for a sub-command.
-            return ""
+        if isinstance(action, _SubParsersAction):
+            return super()._format_args(action, default_metavar or "")
 
         metavar = action.metavar or default_metavar or ""
 
         if self.using_colors:
             # Create a placeholder for the metavar, and store it in the action.
             placeholder_metavar: Union[str, Tuple[str, ...]]
 
@@ -542,16 +544,23 @@
         is added to indicate if the argument is required, or optional. The argument type
         is used as the metavar, and colors are used for semantic highlighting.
         """
         # First, generate base format without help text. This is the invocation part,
         # e.g., `--x str`, but with the correct amount of spacing appended, for proper
         # alignment with the other arguments. The help is replaced with a dummy `\0`,
         # since with an empty help, there would be no extra spacing added.
+        if isinstance(action, _SubParsersAction):
+            return super()._format_action(action)
+
         with patch.object(action, "help", "\0"):
-            base_fmt = super()._format_action(action)
+            if isinstance(action, _SubParsersAction._ChoicesPseudoAction):
+                with patch.object(action, "metavar", ""):
+                    base_fmt = super()._format_action(action)
+            else:
+                base_fmt = super()._format_action(action)
         base_fmt = base_fmt[:-2]  # remove trailing `\0\n`
 
         # Create formatted choice list.
         if action.choices and self.show_full_help:
             if self.using_colors:
                 marker_choices_begin = _PLACEHOLDER_CHOICES_BEGIN
                 marker_choices_end = _PLACEHOLDER_CHOICES_END
@@ -795,23 +804,26 @@
             current_frame = current_frame.f_back
 
     def _format_usage(self, usage: Optional[str], *args, **kwargs) -> str:
         with patch.object(self._color_helper, "crayons", None):
             # Disable colors for usage string.
             fmt = super()._format_usage(usage, *args, **kwargs)
 
+        # Count the number of trailing newlines in the usage string.
+        trail_nls_match = re.search(r"\n*$", fmt)
+        n_trail_nls = len(trail_nls_match.group()) if trail_nls_match else 0
         output_width = self.output_width or get_terminal_size().columns
         # Wrap usage to output width.
         fmt = textwrap.fill(
             fmt,
             width=output_width,
             subsequent_indent=" " * self._indent_increment,
             break_on_hyphens=False,
         )
-        return fmt + "\n"
+        return fmt + "\n" * max(1, n_trail_nls)
 
     def __init__(self, prog: str):
         # noqa: D107
         self._color_helper = ColorHelper(self.use_colors)
         # Wrapping is managed by this class, so pass `sys.maxsize` to the superclass.
         super().__init__(prog, max_help_position=sys.maxsize, width=sys.maxsize)
```

### Comparing `corgy-9.1.0/corgy/_meta.py` & `corgy-9.1.1/corgy/_meta.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/corgy/types/__init__.py` & `corgy-9.1.1/corgy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/corgy/types/_expand.py` & `corgy-9.1.1/corgy/types/_expand.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/corgy/types/_initargs.py` & `corgy-9.1.1/corgy/types/_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/corgy/types/_inputfile.py` & `corgy-9.1.1/corgy/types/_inputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/corgy/types/_keyvaluepairs.py` & `corgy-9.1.1/corgy/types/_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/corgy/types/_outputfile.py` & `corgy-9.1.1/corgy/types/_outputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/corgy/types/_subclass.py` & `corgy-9.1.1/corgy/types/_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/docs/corgy.md` & `corgy-9.1.1/docs/corgy.md`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/docs/corgy.types.md` & `corgy-9.1.1/docs/corgy.types.md`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/pyproject.toml` & `corgy-9.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corgy"
-version = "9.1.0"  # managed by `poetry-dynamic-versioning`
+version = "9.1.1"  # managed by `poetry-dynamic-versioning`
 description = "Elegant data classes"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jayanthkoushik/corgy"
 packages = [
   { include = "corgy" },
```

### Comparing `corgy-9.1.0/tests/test_corgy.py` & `corgy-9.1.1/tests/test_corgy.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/tests/test_corgychecker.py` & `corgy-9.1.1/tests/test_corgychecker.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/tests/test_corgyparser.py` & `corgy-9.1.1/tests/test_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/tests/test_doctests.py` & `corgy-9.1.1/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/tests/test_helpfmt.py` & `corgy-9.1.1/tests/test_helpfmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -851,28 +851,56 @@
             f"  group 2 description\n"
             f"\n"
             f"  {_O('--w')} {_M('str')}    ({_K('optional')})\n",
         )
 
     def test_corgy_help_formatter_handles_sub_parsers(self):
         self.parser.add_argument("--arg", type=str)
-        subparsers = self.parser.add_subparsers(help="sub commands")
-        subparsers.add_parser("x", formatter_class=CorgyHelpFormatter)
-        subparsers.add_parser("y", formatter_class=CorgyHelpFormatter)
+        subparsers = self.parser.add_subparsers(help="sub commands", required=True)
 
         self.assertEqual(
             self.parser.format_help(),
             # positional arguments:
-            #   CMD        sub commands ([x/y])
+            #   {x,y}    sub commands
             #
             # options:
             #   -h/--help  show this help message and exit
             #   --arg str  (default: None)
             f"positional arguments:\n"
-            f"  {_O('CMD')}        sub commands ([{_C('x')}/{_C('y')}])\n"
+            "  {}         sub commands\n"
+            f"\n"
+            f"options:\n"
+            f"  {_O('-h')}/{_O('--help')}  show this help message and exit\n"
+            f"  {_O('--arg')} {_M('str')}  ({_DNone()})\n",
+        )
+
+        subparser_x = subparsers.add_parser(
+            "x", formatter_class=CorgyHelpFormatter, help="x help"
+        )
+        subparser_y = subparsers.add_parser(
+            "y", formatter_class=CorgyHelpFormatter, help="y help"
+        )
+
+        subparser_x.add_argument("--xa", type=int, help="x arg help")
+        subparser_y.add_argument("--ya", type=int, help="y arg help")
+
+        self.assertEqual(
+            self.parser.format_help(),
+            # positional arguments:
+            #     {x,y}    sub commands
+            #     x        x help
+            #     y        y help
+            #
+            # options:
+            #   -h/--help  show this help message and exit
+            #   --arg str  (default: None)
+            f"positional arguments:\n"
+            "  {x,y}      sub commands\n"
+            f"    {_O('x')}        x help\n"
+            f"    {_O('y')}        y help\n"
             f"\n"
             f"options:\n"
             f"  {_O('-h')}/{_O('--help')}  show this help message and exit\n"
             f"  {_O('--arg')} {_M('str')}  ({_DNone()})\n",
         )
 
 
@@ -1222,14 +1250,40 @@
             self.assertEqual(
                 self.parser.format_help(),
                 # options:
                 #   --arg str  (default: None)
                 f"options:\n" f"  {_O('--arg')} {_M('str')}  ({_DNone()})\n",
             )
 
+    def test_corgy_help_formatter_usage_handles_sub_parsers(self):
+        subparsers = self.parser.add_subparsers()
+        subparser1 = subparsers.add_parser("sub1", help="command 1")
+        subparser2 = subparsers.add_parser("sub2", help="command 2")
+        subparser1.add_argument("--x")
+        subparser2.add_argument("--y")
+
+        self.assertEqual(
+            self.parser.format_usage(),
+            # usage: {sub1,sub2} ...
+            "usage: {sub1,sub2} ...\n",
+        )
+
+    def test_corgy_help_formatter_usage_handles_sub_parsers_with_metavar(self):
+        subparsers = self.parser.add_subparsers(metavar="COMMAND")
+        subparser1 = subparsers.add_parser("sub1", help="command 1")
+        subparser2 = subparsers.add_parser("sub2", help="command 2")
+        subparser1.add_argument("--x")
+        subparser2.add_argument("--y")
+
+        self.assertEqual(
+            self.parser.format_usage(),
+            # usage: COMMAND ...
+            "usage: COMMAND ...\n",
+        )
+
 
 class _NoColorTestMeta(type):
     """Metaclass to create versions of test classes that don't use colors."""
 
     def __new__(cls, name, bases, namespace, **kwds):  # pylint: disable=duplicate-code
         for _item in dir(bases[0]):
             if not _item.startswith("test_"):
```

### Comparing `corgy-9.1.0/tests/types/_specialtmps.py` & `corgy-9.1.1/tests/types/_specialtmps.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/tests/types/_test_file.py` & `corgy-9.1.1/tests/types/_test_file.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/tests/types/test_initargs.py` & `corgy-9.1.1/tests/types/test_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/tests/types/test_inputfiles.py` & `corgy-9.1.1/tests/types/test_inputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/tests/types/test_keyvaluepairs.py` & `corgy-9.1.1/tests/types/test_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/tests/types/test_outputfiles.py` & `corgy-9.1.1/tests/types/test_outputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/tests/types/test_subclass.py` & `corgy-9.1.1/tests/types/test_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.0/PKG-INFO` & `corgy-9.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corgy
-Version: 9.1.0
+Version: 9.1.1
 Summary: Elegant data classes
 Home-page: https://github.com/jayanthkoushik/corgy
 License: MIT
 Keywords: data classes,argparse,argument parsing,command line parsing,cli
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.7,<4.0
```

