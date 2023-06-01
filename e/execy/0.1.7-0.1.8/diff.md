# Comparing `tmp/execy-0.1.7.tar.gz` & `tmp/execy-0.1.8.tar.gz`

## Comparing `execy-0.1.7.tar` & `execy-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,15 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 execy-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 execy-0.1.7/.python-version
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 execy-0.1.7/requirements-dev.lock
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 execy-0.1.7/requirements.lock
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 execy-0.1.7/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 execy-0.1.7/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 execy-0.1.7/.pytest_cache/README.md
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 execy-0.1.7/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 execy-0.1.7/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 execy-0.1.7/.vscode/settings.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 execy-0.1.7/src/execy/__init__.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 execy-0.1.7/src/execy/exec.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 execy-0.1.7/tests/test_exec.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 execy-0.1.7/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 execy-0.1.7/LICENSE
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 execy-0.1.7/README.md
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 execy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 execy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 execy-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 execy-0.1.8/.python-version
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 execy-0.1.8/requirements-dev.lock
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 execy-0.1.8/requirements.lock
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 execy-0.1.8/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 execy-0.1.8/.github/workflows/python-publishing.yml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 execy-0.1.8/.vscode/settings.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 execy-0.1.8/src/execy/__init__.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 execy-0.1.8/src/execy/exec.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 execy-0.1.8/tests/test_exec.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 execy-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 execy-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 execy-0.1.8/README.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 execy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 execy-0.1.8/PKG-INFO
```

### Comparing `execy-0.1.7/src/execy/exec.py` & `execy-0.1.8/src/execy/exec.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import time
 import asyncio
+import time
 from functools import wraps
 
 
 def exec_time(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         if asyncio.iscoroutinefunction(func):
```

### Comparing `execy-0.1.7/tests/test_exec.py` & `execy-0.1.8/tests/test_exec.py`

 * *Files identical despite different names*

### Comparing `execy-0.1.7/README.md` & `execy-0.1.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Execy
+[![Upload Python Package](https://github.com/hglong16/execy/actions/workflows/python-publish.yml/badge.svg?branch=master)](https://github.com/hglong16/execy/actions/workflows/python-publish.yml)
 
-The ececy exec_time decorator is a utility that measures the execution time of a function. It can be used to easily track and log the time taken by a function to execute, both for synchronous and asynchronous functions.
+The execy `@exec_time` decorator is a utility that measures the execution time of a function. It can be used to easily track and log the time taken by a function to execute, both for synchronous and asynchronous functions.
 
 ## Table of Contents
 
 - [Execy](#execy)
   - [Table of Contents](#table-of-contents)
   - [Installation](#installation)
   - [Usage](#usage)
```

### Comparing `execy-0.1.7/PKG-INFO` & `execy-0.1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: execy
-Version: 0.1.7
+Version: 0.1.8
 Summary: The ececy exec_time decorator is a utility that measures the execution time of a function. It can be used to easily track and log the time taken by a function to execute, both for synchronous and asynchronous functions.
 Author-email: hglong16 <intihad.vuong@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Execy
+[![Upload Python Package](https://github.com/hglong16/execy/actions/workflows/python-publish.yml/badge.svg?branch=master)](https://github.com/hglong16/execy/actions/workflows/python-publish.yml)
 
-The ececy exec_time decorator is a utility that measures the execution time of a function. It can be used to easily track and log the time taken by a function to execute, both for synchronous and asynchronous functions.
+The execy `@exec_time` decorator is a utility that measures the execution time of a function. It can be used to easily track and log the time taken by a function to execute, both for synchronous and asynchronous functions.
 
 ## Table of Contents
 
 - [Execy](#execy)
   - [Table of Contents](#table-of-contents)
   - [Installation](#installation)
   - [Usage](#usage)
```

