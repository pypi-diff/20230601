# Comparing `tmp/pycarot-0.0.3.tar.gz` & `tmp/pycarot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycarot-0.0.3.tar", last modified: Mon Dec 19 15:43:10 2022, max compression
+gzip compressed data, was "pycarot-0.0.4.tar", last modified: Wed May 31 23:10:25 2023, max compression
```

## Comparing `pycarot-0.0.3.tar` & `pycarot-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-12-19 15:43:10.559762 pycarot-0.0.3/
--rw-rw-rw-   0        0        0     1091 2022-11-11 08:20:38.000000 pycarot-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      921 2022-12-19 15:43:10.559762 pycarot-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       11 2022-11-16 21:29:18.000000 pycarot-0.0.3/README.md
--rw-rw-rw-   0        0        0     1528 2022-12-19 15:42:06.000000 pycarot-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-19 15:43:10.559762 pycarot-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-11-11 07:35:02.000000 pycarot-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-19 15:43:10.436869 pycarot-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2022-12-19 15:43:10.500256 pycarot-0.0.3/src/pycarot/
--rw-rw-rw-   0        0        0       65 2022-12-19 15:40:02.000000 pycarot-0.0.3/src/pycarot/__init__.py
--rw-rw-rw-   0        0        0       73 2022-11-11 07:35:02.000000 pycarot-0.0.3/src/pycarot/__main__.py
--rw-rw-rw-   0        0        0     2142 2022-12-18 20:26:51.000000 pycarot-0.0.3/src/pycarot/event.py
-drwxrwxrwx   0        0        0        0 2022-12-19 15:43:10.557328 pycarot-0.0.3/src/pycarot/ioc/
--rw-rw-rw-   0        0        0      123 2022-11-11 08:01:57.000000 pycarot-0.0.3/src/pycarot/ioc/__init__.py
--rw-rw-rw-   0        0        0     2682 2022-11-11 08:16:05.000000 pycarot-0.0.3/src/pycarot/ioc/container.py
--rw-rw-rw-   0        0        0     1443 2022-11-22 16:58:00.000000 pycarot-0.0.3/src/pycarot/ioc/entries.py
--rw-rw-rw-   0        0        0      389 2022-11-11 07:35:02.000000 pycarot-0.0.3/src/pycarot/ioc/exceptions.py
--rw-rw-rw-   0        0        0      984 2022-11-11 08:23:23.000000 pycarot-0.0.3/src/pycarot/ioc/static.py
--rw-rw-rw-   0        0        0     2847 2022-12-19 15:40:02.000000 pycarot-0.0.3/src/pycarot/progress.py
-drwxrwxrwx   0        0        0        0 2022-12-19 15:43:10.541442 pycarot-0.0.3/src/pycarot.egg-info/
--rw-rw-rw-   0        0        0      921 2022-12-19 15:43:10.000000 pycarot-0.0.3/src/pycarot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2022-12-19 15:43:10.000000 pycarot-0.0.3/src/pycarot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-19 15:43:10.000000 pycarot-0.0.3/src/pycarot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2022-12-19 15:43:10.000000 pycarot-0.0.3/src/pycarot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2022-12-19 15:43:10.000000 pycarot-0.0.3/src/pycarot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-12-19 15:43:10.000000 pycarot-0.0.3/src/pycarot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 23:10:25.201216 pycarot-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-05-31 22:21:28.000000 pycarot-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      487 2023-05-31 23:10:25.200207 pycarot-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-05-31 22:21:28.000000 pycarot-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1200 2023-05-31 23:09:59.000000 pycarot-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 23:10:25.201216 pycarot-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-05-31 22:21:28.000000 pycarot-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 23:10:25.138268 pycarot-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 23:10:25.162049 pycarot-0.0.4/src/pycarot/
+-rw-rw-rw-   0        0        0       65 2023-05-31 23:07:54.000000 pycarot-0.0.4/src/pycarot/__init__.py
+-rw-rw-rw-   0        0        0       75 2023-05-31 23:07:54.000000 pycarot-0.0.4/src/pycarot/__main__.py
+-rw-rw-rw-   0        0        0     2141 2023-05-31 23:07:54.000000 pycarot-0.0.4/src/pycarot/event.py
+drwxrwxrwx   0        0        0        0 2023-05-31 23:10:25.197173 pycarot-0.0.4/src/pycarot/ioc/
+-rw-rw-rw-   0        0        0      123 2023-05-31 23:07:54.000000 pycarot-0.0.4/src/pycarot/ioc/__init__.py
+-rw-rw-rw-   0        0        0     2682 2023-05-31 22:21:28.000000 pycarot-0.0.4/src/pycarot/ioc/container.py
+-rw-rw-rw-   0        0        0     1494 2023-05-31 23:07:54.000000 pycarot-0.0.4/src/pycarot/ioc/entries.py
+-rw-rw-rw-   0        0        0      389 2023-05-31 22:21:28.000000 pycarot-0.0.4/src/pycarot/ioc/exceptions.py
+-rw-rw-rw-   0        0        0      984 2023-05-31 22:21:28.000000 pycarot-0.0.4/src/pycarot/ioc/static.py
+-rw-rw-rw-   0        0        0     2848 2023-05-31 23:07:54.000000 pycarot-0.0.4/src/pycarot/progress.py
+drwxrwxrwx   0        0        0        0 2023-05-31 23:10:25.179192 pycarot-0.0.4/src/pycarot.egg-info/
+-rw-rw-rw-   0        0        0      487 2023-05-31 23:10:25.000000 pycarot-0.0.4/src/pycarot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2023-05-31 23:10:25.000000 pycarot-0.0.4/src/pycarot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 23:10:25.000000 pycarot-0.0.4/src/pycarot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-31 23:10:25.000000 pycarot-0.0.4/src/pycarot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-05-31 23:10:25.000000 pycarot-0.0.4/src/pycarot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 23:10:25.000000 pycarot-0.0.4/src/pycarot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 23:10:25.199185 pycarot-0.0.4/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-31 23:07:54.000000 pycarot-0.0.4/src/tests/__init__.py
+-rw-rw-rw-   0        0        0      420 2023-05-31 23:07:54.000000 pycarot-0.0.4/src/tests/test_event.py
```

### Comparing `pycarot-0.0.3/LICENSE` & `pycarot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycarot-0.0.3/pyproject.toml` & `pycarot-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -3,54 +3,50 @@
     "setuptools>=42.0.0", 
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pycarot"
-version = "0.0.3"
+version = "0.0.4"
 description = "pycarot - python tools"
 readme = "README.md"
-authors = [{ name="BaySiyah",email="siyah@ksknsy.de" }]
-license = { text="MIT License" }
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Intended Audience :: Developers",
-    "Operating System :: Microsoft :: Windows",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Typing :: Typed",
-]
+requires-python = ">=3.8"
+license = {file = "LICENSE.txt"}
 keywords = [
     "dependency", 
     "injection", 
     "event", 
     "IoC", 
     "container", 
     "progress", 
     "progressbar",
 ]
+authors = [
+    {name = "canoKes", email = "siyah@keskinsoy.com"},
+]
+maintainers = [
+    {name = "canoKes", email = "siyah@keskinsoy.com"},
+]
+classifiers = [
+    "Programming Language :: Python",
+    "Typing :: Typed",
+]
 dependencies = [
     "colorama == 0.4.6",
 ]
-requires-python = ">=3.8"
 
 [project.urls]
-Homepage = "https://github.com/BaySiyah/pycarot"
+homepage = "https://github.com/canoKes/pycarot"
 
 [project.scripts]
 pycarot = "pycarot.__main__:main"
 
 [tool.bumpver]
-current_version = "0.0.3"
+current_version = "0.0.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `pycarot-0.0.3/src/pycarot/event.py` & `pycarot-0.0.4/src/pycarot/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def name(self) -> str:
         return type(self).__name__
 
     def __str__(self) -> str:
         attributes = vars(self).items()
         out = self.name
         if attributes:
-            out +=  f" {', '.join([f'{k}({v})' for k, v in attributes])}"
+            out += f" {', '.join([f'{k}({v})' for k, v in attributes])}"
         return out
 
     def __repr__(self) -> str:
         return str(self)
 
 
 class EventManager:
```

### Comparing `pycarot-0.0.3/src/pycarot/ioc/container.py` & `pycarot-0.0.4/src/pycarot/ioc/container.py`

 * *Files identical despite different names*

### Comparing `pycarot-0.0.3/src/pycarot/ioc/entries.py` & `pycarot-0.0.4/src/pycarot/ioc/entries.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,21 +18,26 @@
         if not isinstance(service, type):
             raise ValueError("service has to be a type")
 
         self.implementation = implementation
         self.service = service
 
 
-
 class InstanceEntry(Entry):
     """Returns a preconstructed instance."""
 
     __slots__ = ("arguments", "keywords")
 
-    def __init__(self, implementation: type, service: type = None, arguments: tuple[Any] = None, keywords: dict[str, Any] = None) -> None:
+    def __init__(
+        self,
+        implementation: type,
+        service: type = None,
+        arguments: tuple[Any] = None,
+        keywords: dict[str, Any] = None,
+    ) -> None:
         super().__init__(implementation, service)
         self.arguments = arguments if arguments is not None else ()
         self.keywords = keywords if keywords is not None else {}
 
 
 class SingletonEntry(Entry):
     """A singlton entry. Returns always the same instance of an object."""
```

### Comparing `pycarot-0.0.3/src/pycarot/ioc/static.py` & `pycarot-0.0.4/src/pycarot/ioc/static.py`

 * *Files identical despite different names*

### Comparing `pycarot-0.0.3/src/pycarot/progress.py` & `pycarot-0.0.4/src/pycarot/progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 from typing import Any, Callable
 
 from colorama import Fore, Style
 
 
 class ProgressBar:
-    __slots__ = ("value", "total", "elements","title", "digits", "percentage")
+    __slots__ = ("value", "total", "elements", "title", "digits", "percentage")
 
     MAX_SIZE = 50
 
     def __init__(
         self,
         elements: int,
         title: str = None,
```

