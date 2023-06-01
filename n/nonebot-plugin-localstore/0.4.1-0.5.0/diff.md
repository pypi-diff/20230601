# Comparing `tmp/nonebot_plugin_localstore-0.4.1.tar.gz` & `tmp/nonebot_plugin_localstore-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_localstore-0.4.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_localstore-0.5.0.tar", max compression
```

## Comparing `nonebot_plugin_localstore-0.4.1.tar` & `nonebot_plugin_localstore-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-02-14 03:38:29.581949 nonebot_plugin_localstore-0.4.1/LICENSE
--rw-r--r--   0        0        0     2391 2023-02-14 03:38:29.581949 nonebot_plugin_localstore-0.4.1/README.md
--rw-r--r--   0        0        0     1622 2023-02-14 03:38:29.581949 nonebot_plugin_localstore-0.4.1/nonebot_plugin_localstore/__init__.py
--rw-r--r--   0        0        0     6020 2023-02-14 03:38:29.581949 nonebot_plugin_localstore-0.4.1/nonebot_plugin_localstore/data_source.py
--rw-r--r--   0        0        0     1871 2023-02-14 03:38:29.581949 nonebot_plugin_localstore-0.4.1/nonebot_plugin_localstore/script.py
--rw-r--r--   0        0        0      622 2023-02-14 03:38:29.581949 nonebot_plugin_localstore-0.4.1/nonebot_plugin_localstore/utils.py
--rw-r--r--   0        0        0     1180 2023-02-14 03:38:29.581949 nonebot_plugin_localstore-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 nonebot_plugin_localstore-0.4.1/setup.py
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 nonebot_plugin_localstore-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-01 14:28:53.099265 nonebot_plugin_localstore-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2391 2023-06-01 14:28:53.099265 nonebot_plugin_localstore-0.5.0/README.md
+-rw-r--r--   0        0        0     2453 2023-06-01 14:28:53.099265 nonebot_plugin_localstore-0.5.0/nonebot_plugin_localstore/__init__.py
+-rw-r--r--   0        0        0     6020 2023-06-01 14:28:53.099265 nonebot_plugin_localstore-0.5.0/nonebot_plugin_localstore/data_source.py
+-rw-r--r--   0        0        0     1871 2023-06-01 14:28:53.099265 nonebot_plugin_localstore-0.5.0/nonebot_plugin_localstore/script.py
+-rw-r--r--   0        0        0      622 2023-06-01 14:28:53.099265 nonebot_plugin_localstore-0.5.0/nonebot_plugin_localstore/utils.py
+-rw-r--r--   0        0        0     1229 2023-06-01 14:28:53.103266 nonebot_plugin_localstore-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3255 1970-01-01 00:00:00.000000 nonebot_plugin_localstore-0.5.0/PKG-INFO
```

### Comparing `nonebot_plugin_localstore-0.4.1/LICENSE` & `nonebot_plugin_localstore-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_localstore-0.4.1/README.md` & `nonebot_plugin_localstore-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_localstore-0.4.1/nonebot_plugin_localstore/data_source.py` & `nonebot_plugin_localstore-0.5.0/nonebot_plugin_localstore/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_localstore-0.4.1/nonebot_plugin_localstore/script.py` & `nonebot_plugin_localstore-0.5.0/nonebot_plugin_localstore/script.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_localstore-0.4.1/nonebot_plugin_localstore/utils.py` & `nonebot_plugin_localstore-0.5.0/nonebot_plugin_localstore/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_localstore-0.4.1/pyproject.toml` & `nonebot_plugin_localstore-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tool.poetry]
 name = "nonebot-plugin-localstore"
-version = "0.4.1"
+version = "0.5.0"
 description = "Local Storage Support for NoneBot2"
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/nonebot/plugin-localstore"
 repository = "https://github.com/nonebot/plugin-localstore"
 documentation = "https://github.com/nonebot/plugin-localstore#readme"
 keywords = ["nonebot2", "qq", "plugin"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = "^2.0.0-rc.1"
+nonebot2 = "^2.0.0"
 typing-extensions = ">=4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.1"
-black = "^22.6.0"
+black = "^23.1.0"
 nonemoji = "^0.1.2"
 pre-commit = "^2.20.0"
+pycln = "^2.1.4"
 
 [tool.poetry.plugins.nb_scripts]
 localstore = "nonebot_plugin_localstore.script:main"
 
 [tool.black]
 line-length = 88
 target-version = ["py38", "py39", "py310", "py311"]
@@ -35,14 +36,18 @@
 profile = "black"
 line_length = 88
 length_sort = true
 skip_gitignore = true
 force_sort_within_sections = true
 extra_standard_library = ["typing_extensions"]
 
+[tool.pycln]
+path = "."
+all = false
+
 [tool.pyright]
 pythonVersion = "3.8"
 pythonPlatform = "All"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_localstore-0.4.1/PKG-INFO` & `nonebot_plugin_localstore-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-localstore
-Version: 0.4.1
+Version: 0.5.0
 Summary: Local Storage Support for NoneBot2
 Home-page: https://github.com/nonebot/plugin-localstore
 License: MIT
 Keywords: nonebot2,qq,plugin
 Author: yanyongyu
 Author-email: yyy@nonebot.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot2 (>=2.0.0-rc.1,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.0.0)
 Project-URL: Documentation, https://github.com/nonebot/plugin-localstore#readme
 Project-URL: Repository, https://github.com/nonebot/plugin-localstore
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD041 -->
 <p align="center">
```

