# Comparing `tmp/un_yaml-0.1.1.tar.gz` & `tmp/un_yaml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "un_yaml-0.1.1.tar", max compression
+gzip compressed data, was "un_yaml-0.1.2.tar", max compression
```

## Comparing `un_yaml-0.1.1.tar` & `un_yaml-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-31 12:54:36.386488 un_yaml-0.1.1/LICENSE
--rw-r--r--   0        0        0      100 2023-05-31 12:54:36.387406 un_yaml-0.1.1/README.md
--rw-r--r--   0        0        0      652 2023-05-31 13:33:07.339502 un_yaml-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      119 2023-05-31 13:33:07.341430 un_yaml-0.1.1/un_yaml/__init__.py
--rw-r--r--   0        0        0     3728 2023-05-31 12:54:36.393070 un_yaml-0.1.1/un_yaml/un_cli.py
--rw-r--r--   0        0        0     1420 2023-05-31 12:54:36.393499 un_yaml-0.1.1/un_yaml/un_uri.py
--rw-r--r--   0        0        0     2180 2023-05-31 12:54:36.393871 un_yaml-0.1.1/un_yaml/un_yaml.py
--rw-r--r--   0        0        0       24 2023-05-31 13:33:07.342331 un_yaml-0.1.1/un_yaml/wrapper.py
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 un_yaml-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 12:54:36.386488 un_yaml-0.1.2/LICENSE
+-rw-r--r--   0        0        0      100 2023-05-31 12:54:36.387406 un_yaml-0.1.2/README.md
+-rw-r--r--   0        0        0      652 2023-05-31 23:54:18.885846 un_yaml-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-05-31 13:33:07.341430 un_yaml-0.1.2/un_yaml/__init__.py
+-rw-r--r--   0        0        0     3755 2023-05-31 23:54:18.886677 un_yaml-0.1.2/un_yaml/un_cli.py
+-rw-r--r--   0        0        0     1420 2023-05-31 12:54:36.393499 un_yaml-0.1.2/un_yaml/un_uri.py
+-rw-r--r--   0        0        0     2180 2023-05-31 12:54:36.393871 un_yaml-0.1.2/un_yaml/un_yaml.py
+-rw-r--r--   0        0        0       24 2023-05-31 13:33:07.342331 un_yaml-0.1.2/un_yaml/wrapper.py
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 un_yaml-0.1.2/PKG-INFO
```

### Comparing `un_yaml-0.1.1/LICENSE` & `un_yaml-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `un_yaml-0.1.1/pyproject.toml` & `un_yaml-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "un_yaml"
-version = "0.1.1"
+version = "0.1.2"
 description = "Universal YAML: replace repetitive code with your own Domain-Specific un-Language (DSuL)"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 anyio = "^3.7.0"
```

### Comparing `un_yaml-0.1.1/un_yaml/un_cli.py` & `un_yaml-0.1.2/un_yaml/un_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,20 +35,21 @@
         super().__init__(yaml_data)
         if UnCli.CMD not in self.cfg:
             raise ValueError(f"'{UnCli.CMD}' not in file '{file}':\n{self.cfg}")
         self.cmds = self.get(UnCli.CMD)
         self.doc = self.get_handler("doc")()
 
     def parse_version(self, parser: ArgumentParser) -> None:
-        __version__ = version("un_yaml")
+        doc_name = self.info("doc")
+        __version__ = version(doc_name)
         parser.add_argument(
             "-v",
             "--version",
             action="store_const",
-            const=f"{self.info('doc')} {__version__}",
+            const=f"{doc_name} {__version__}",
             help="Show version and exit.",
         )
 
     def make_parser(self) -> ArgumentParser:
         parser = ArgumentParser(self.get("doc"))
         self.parse_version(parser)
         subparsers = parser.add_subparsers(dest="command")
```

### Comparing `un_yaml-0.1.1/un_yaml/un_uri.py` & `un_yaml-0.1.2/un_yaml/un_uri.py`

 * *Files identical despite different names*

### Comparing `un_yaml-0.1.1/un_yaml/un_yaml.py` & `un_yaml-0.1.2/un_yaml/un_yaml.py`

 * *Files identical despite different names*

### Comparing `un_yaml-0.1.1/PKG-INFO` & `un_yaml-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: un-yaml
-Version: 0.1.1
+Version: 0.1.2
 Summary: Universal YAML: replace repetitive code with your own Domain-Specific un-Language (DSuL)
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

