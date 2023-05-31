# Comparing `tmp/poetry_plugin_pypi_mirror-0.3.1.tar.gz` & `tmp/poetry_plugin_pypi_mirror-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_pypi_mirror-0.3.1.tar", max compression
+gzip compressed data, was "poetry_plugin_pypi_mirror-0.3.2.tar", max compression
```

## Comparing `poetry_plugin_pypi_mirror-0.3.1.tar` & `poetry_plugin_pypi_mirror-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1457 2022-10-23 17:58:22.833789 poetry_plugin_pypi_mirror-0.3.1/LICENSE
--rw-r--r--   0        0        0     3180 2023-04-30 21:13:13.233149 poetry_plugin_pypi_mirror-0.3.1/README.md
--rw-r--r--   0        0        0     1133 2023-04-30 21:13:36.699871 poetry_plugin_pypi_mirror-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-23 17:58:22.833789 poetry_plugin_pypi_mirror-0.3.1/src/poetry_plugin_pypi_mirror/__init__.py
--rw-r--r--   0        0        0     4559 2023-04-30 20:53:03.808326 poetry_plugin_pypi_mirror-0.3.1/src/poetry_plugin_pypi_mirror/plugins.py
--rw-r--r--   0        0        0       48 2022-10-23 17:58:22.833789 poetry_plugin_pypi_mirror-0.3.1/src/poetry_plugin_pypi_mirror/py.typed
--rw-r--r--   0        0        0     4042 1970-01-01 00:00:00.000000 poetry_plugin_pypi_mirror-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1457 2023-05-31 23:05:55.198380 poetry_plugin_pypi_mirror-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3180 2023-05-31 23:06:36.234804 poetry_plugin_pypi_mirror-0.3.2/README.md
+-rw-r--r--   0        0        0     1133 2023-05-31 23:23:23.924080 poetry_plugin_pypi_mirror-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-31 23:05:55.201713 poetry_plugin_pypi_mirror-0.3.2/src/poetry_plugin_pypi_mirror/__init__.py
+-rw-r--r--   0        0        0     4559 2023-05-31 23:05:55.201713 poetry_plugin_pypi_mirror-0.3.2/src/poetry_plugin_pypi_mirror/plugins.py
+-rw-r--r--   0        0        0       48 2023-05-31 23:05:55.201713 poetry_plugin_pypi_mirror-0.3.2/src/poetry_plugin_pypi_mirror/py.typed
+-rw-r--r--   0        0        0     4042 1970-01-01 00:00:00.000000 poetry_plugin_pypi_mirror-0.3.2/PKG-INFO
```

### Comparing `poetry_plugin_pypi_mirror-0.3.1/LICENSE` & `poetry_plugin_pypi_mirror-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_mirror-0.3.1/README.md` & `poetry_plugin_pypi_mirror-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -66,13 +66,13 @@
 
 *poetry-plugin-pypi-mirror* depends on poetry internals which can change between
 poetry releases. It's important to ensure compatibility between the poetry
 version in use and the plugin version in use.
 
 | Poetry version(s) | Compatible plugin version(s) |
 |-------------------|------------------------------|
-| >= 1.3, < 1.5     | ^0.3.1                       |
+| >= 1.3, < 1.6     | ^0.3.1                       |
 | ~1.2.1            | < 0.3.0                      |
 
 ## See also
 
 * [python-poetry/poetry#1632](https://github.com/python-poetry/poetry/issues/1632) - poetry feature request to add support for global repository URL replacement
```

### Comparing `poetry_plugin_pypi_mirror-0.3.1/pyproject.toml` & `poetry_plugin_pypi_mirror-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "poetry-plugin-pypi-mirror"
-version = "0.3.1"
+version = "0.3.2"
 description = "Poetry plugin that adds support for pypi.org mirrors and pull-through caches"
 authors = ["Jacob Henner <code@ventricle.us>"]
 license = "BSD-3-Clause"
 keywords = ["packaging", "poetry", "pypi"]
 readme = "README.md"
 homepage = "https://github.com/arcesium/poetry-plugin-pypi-mirror"
 repository = "https://github.com/arcesium/poetry-plugin-pypi-mirror"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-poetry = ">= 1.3, < 1.5"
+poetry = ">= 1.3, < 1.6"
 
 [tool.poetry.plugins."poetry.plugin"]
 demo = "poetry_plugin_pypi_mirror.plugins:PyPIMirrorPlugin"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 mypy = "^0.991"
```

### Comparing `poetry_plugin_pypi_mirror-0.3.1/src/poetry_plugin_pypi_mirror/plugins.py` & `poetry_plugin_pypi_mirror-0.3.2/src/poetry_plugin_pypi_mirror/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_mirror-0.3.1/PKG-INFO` & `poetry_plugin_pypi_mirror-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-pypi-mirror
-Version: 0.3.1
+Version: 0.3.2
 Summary: Poetry plugin that adds support for pypi.org mirrors and pull-through caches
 Home-page: https://github.com/arcesium/poetry-plugin-pypi-mirror
 License: BSD-3-Clause
 Keywords: packaging,poetry,pypi
 Author: Jacob Henner
 Author-email: code@ventricle.us
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: poetry (>=1.3,<1.5)
+Requires-Dist: poetry (>=1.3,<1.6)
 Project-URL: Repository, https://github.com/arcesium/poetry-plugin-pypi-mirror
 Description-Content-Type: text/markdown
 
 # poetry-plugin-pypi-mirror
 
 ## Description
 
@@ -87,14 +87,14 @@
 
 *poetry-plugin-pypi-mirror* depends on poetry internals which can change between
 poetry releases. It's important to ensure compatibility between the poetry
 version in use and the plugin version in use.
 
 | Poetry version(s) | Compatible plugin version(s) |
 |-------------------|------------------------------|
-| >= 1.3, < 1.5     | ^0.3.1                       |
+| >= 1.3, < 1.6     | ^0.3.1                       |
 | ~1.2.1            | < 0.3.0                      |
 
 ## See also
 
 * [python-poetry/poetry#1632](https://github.com/python-poetry/poetry/issues/1632) - poetry feature request to add support for global repository URL replacement
```

