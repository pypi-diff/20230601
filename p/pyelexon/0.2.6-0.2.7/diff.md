# Comparing `tmp/pyelexon-0.2.6.tar.gz` & `tmp/pyelexon-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyelexon-0.2.6.tar", max compression
+gzip compressed data, was "pyelexon-0.2.7.tar", max compression
```

## Comparing `pyelexon-0.2.6.tar` & `pyelexon-0.2.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1076 2022-11-30 16:17:24.849929 pyelexon-0.2.6/LICENSE.txt
--rw-r--r--   0        0        0     1260 2022-11-30 16:17:24.850012 pyelexon-0.2.6/README.md
--rw-r--r--   0        0        0       52 2023-03-09 13:18:46.883583 pyelexon-0.2.6/pyelexon/__init__.py
--rwxr-xr-x   0        0        0      500 2022-11-30 16:17:24.850579 pyelexon-0.2.6/pyelexon/configure_logging.py
--rw-r--r--   0        0        0       90 2022-11-30 16:17:24.850637 pyelexon-0.2.6/pyelexon/exceptions.py
--rw-r--r--   0        0        0      348 2023-01-30 10:06:49.144322 pyelexon-0.2.6/pyelexon/kwargs_mapping.py
--rw-r--r--   0        0        0     7591 2023-03-09 12:19:03.027260 pyelexon-0.2.6/pyelexon/pyelexon.py
--rw-r--r--   0        0        0     1366 2023-03-09 13:18:48.607684 pyelexon-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 pyelexon-0.2.6/setup.py
--rw-r--r--   0        0        0     2155 1970-01-01 00:00:00.000000 pyelexon-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-01 09:05:03.864717 pyelexon-0.2.7/LICENSE.txt
+-rw-r--r--   0        0        0     1260 2023-06-01 09:05:03.864805 pyelexon-0.2.7/README.md
+-rw-r--r--   0        0        0       52 2023-06-01 11:03:54.443033 pyelexon-0.2.7/pyelexon/__init__.py
+-rwxr-xr-x   0        0        0      500 2023-06-01 09:05:03.865401 pyelexon-0.2.7/pyelexon/configure_logging.py
+-rw-r--r--   0        0        0       90 2023-06-01 09:05:03.865480 pyelexon-0.2.7/pyelexon/exceptions.py
+-rw-r--r--   0        0        0      348 2023-06-01 09:05:03.865565 pyelexon-0.2.7/pyelexon/kwargs_mapping.py
+-rw-r--r--   0        0        0     7591 2023-06-01 09:05:03.865680 pyelexon-0.2.7/pyelexon/pyelexon.py
+-rw-r--r--   0        0        0     1367 2023-06-01 11:03:54.443239 pyelexon-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1952 1970-01-01 00:00:00.000000 pyelexon-0.2.7/setup.py
+-rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 pyelexon-0.2.7/PKG-INFO
```

### Comparing `pyelexon-0.2.6/LICENSE.txt` & `pyelexon-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyelexon-0.2.6/README.md` & `pyelexon-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pyelexon-0.2.6/pyelexon/pyelexon.py` & `pyelexon-0.2.7/pyelexon/pyelexon.py`

 * *Files identical despite different names*

### Comparing `pyelexon-0.2.6/pyproject.toml` & `pyelexon-0.2.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyelexon"
-version = "0.2.6"
+version = "0.2.7"
 description = ""
 authors = ["atsangarides <andreas_tsangarides@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/atsangarides/pyelexon"
 repository = "https://github.com/atsangarides/pyelexon"
 keywords = ["api", "energy"]
@@ -16,15 +16,15 @@
 ]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "2.26.0"
+requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 black = "^21.9b0"
 pre-commit = "^2.15.0"
 python-dotenv = "^0.19.1"
 pytest-recording = "^0.12.0"
```

### Comparing `pyelexon-0.2.6/setup.py` & `pyelexon-0.2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['pyelexon']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['requests==2.26.0']
+['requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'pyelexon',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': '',
     'long_description': '# pyelexon\n\nSimple python wrapper for the Elexon BMRS API.\n\n[![](https://img.shields.io/badge/python-3.8-blue.svg)](https://github.com/pyenv/pyenv)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n\n## Getting started\n\n* Register on the Elexon BMRS [data portal](https://www.elexonportal.co.uk/news/latest?cachebust=q3pzb5uiac)\nand retrieve your `api_key`\n\n* Example usage\n```python\nfrom datetime import date\nfrom pyelexon import Elexon\n\napi_key = "123456"\nreport = "DETSYSPRICES"\nparams = {\n    "settlement_date": "2021-01-01",\n    "settlement_period": 1\n}\n\nelexon = Elexon(api_key)\n# returns content of response\nr: bytes = elexon.fetch_data(report, params)\n```\nExample with report specific method\n```python\nfrom datetime import date\nfrom pyelexon import Elexon\n\napi_key = "123456"\nreport = "DETSYSPRICES"\n\n\nelexon = Elexon(api_key)\n# returns content of response\nr: bytes = elexon.get_detsysprices(\n    report,\n    settlement_date=date(2021, 1, 1),\n    settlement_period=1\n)\n```\n\n## Tested reports\n\n* `DETSYSPRICES`\n* `DYNBMDATA`\n* `PHYBMDATA`\n',
     'author': 'atsangarides',
     'author_email': 'andreas_tsangarides@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/atsangarides/pyelexon',
```

### Comparing `pyelexon-0.2.6/PKG-INFO` & `pyelexon-0.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyelexon
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Home-page: https://github.com/atsangarides/pyelexon
 License: MIT
 Keywords: api,energy
 Author: atsangarides
 Author-email: andreas_tsangarides@hotmail.com
 Requires-Python: >=3.8,<4.0
@@ -14,15 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: requests (==2.26.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/atsangarides/pyelexon
 Description-Content-Type: text/markdown
 
 # pyelexon
 
 Simple python wrapper for the Elexon BMRS API.
```

