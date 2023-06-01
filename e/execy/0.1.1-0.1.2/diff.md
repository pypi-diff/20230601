# Comparing `tmp/execy-0.1.1.tar.gz` & `tmp/execy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "execy-0.1.1.tar", last modified: Thu Jun  1 03:15:36 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `execy-0.1.1.tar` & `execy-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 long      (1000) long      (1000)        0 2023-06-01 03:15:36.114116 execy-0.1.1/
--rw-rw-r--   0 long      (1000) long      (1000)     1067 2023-06-01 03:11:19.000000 execy-0.1.1/LICENSE
--rw-rw-r--   0 long      (1000) long      (1000)     1314 2023-06-01 03:15:36.114116 execy-0.1.1/PKG-INFO
--rw-rw-r--   0 long      (1000) long      (1000)     1062 2023-06-01 03:12:04.000000 execy-0.1.1/README.md
--rw-rw-r--   0 long      (1000) long      (1000)      629 2023-06-01 03:15:19.000000 execy-0.1.1/pyproject.toml
--rw-rw-r--   0 long      (1000) long      (1000)       38 2023-06-01 03:15:36.114116 execy-0.1.1/setup.cfg
--rw-rw-r--   0 long      (1000) long      (1000)      342 2023-06-01 03:14:13.000000 execy-0.1.1/setup.py
-drwxrwxr-x   0 long      (1000) long      (1000)        0 2023-06-01 03:15:36.110116 execy-0.1.1/src/
-drwxrwxr-x   0 long      (1000) long      (1000)        0 2023-06-01 03:15:36.110116 execy-0.1.1/src/exectime/
--rw-rw-r--   0 long      (1000) long      (1000)        0 2023-06-01 02:10:01.000000 execy-0.1.1/src/exectime/__init__.py
--rw-rw-r--   0 long      (1000) long      (1000)     1123 2023-06-01 02:21:40.000000 execy-0.1.1/src/exectime/exec.py
-drwxrwxr-x   0 long      (1000) long      (1000)        0 2023-06-01 03:15:36.114116 execy-0.1.1/src/execy.egg-info/
--rw-rw-r--   0 long      (1000) long      (1000)     1314 2023-06-01 03:15:36.000000 execy-0.1.1/src/execy.egg-info/PKG-INFO
--rw-rw-r--   0 long      (1000) long      (1000)      270 2023-06-01 03:15:36.000000 execy-0.1.1/src/execy.egg-info/SOURCES.txt
--rw-rw-r--   0 long      (1000) long      (1000)        1 2023-06-01 03:15:36.000000 execy-0.1.1/src/execy.egg-info/dependency_links.txt
--rw-rw-r--   0 long      (1000) long      (1000)       69 2023-06-01 03:15:36.000000 execy-0.1.1/src/execy.egg-info/requires.txt
--rw-rw-r--   0 long      (1000) long      (1000)        9 2023-06-01 03:15:36.000000 execy-0.1.1/src/execy.egg-info/top_level.txt
-drwxrwxr-x   0 long      (1000) long      (1000)        0 2023-06-01 03:15:36.114116 execy-0.1.1/tests/
--rw-r--r--   0 long      (1000) long      (1000)      879 2023-06-01 02:25:55.000000 execy-0.1.1/tests/test_exec.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 execy-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 execy-0.1.2/.python-version
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 execy-0.1.2/requirements-dev.lock
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 execy-0.1.2/requirements.lock
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 execy-0.1.2/setup.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 execy-0.1.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 execy-0.1.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 execy-0.1.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 execy-0.1.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 execy-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 execy-0.1.2/src/exectime/__init__.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 execy-0.1.2/src/exectime/exec.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 execy-0.1.2/tests/test_exec.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 execy-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 execy-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 execy-0.1.2/README.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 execy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 execy-0.1.2/PKG-INFO
```

### Comparing `execy-0.1.1/LICENSE` & `execy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `execy-0.1.1/PKG-INFO` & `execy-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: execy
-Version: 0.1.1
-Summary: Add a short description here
-Author: hglong16
+Version: 0.1.2
+Summary: The ececy exec_time decorator is a utility that measures the execution time of a function. It can be used to easily track and log the time taken by a function to execute, both for synchronous and asynchronous functions.
 Author-email: hglong16 <intihad.vuong@gmail.com>
-License: MIT
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Python: >=3.8
+Requires-Dist: pytest-asyncio~=0.21.0
+Requires-Dist: setuptools~=67.8.0
+Requires-Dist: twine~=4.0.2
+Requires-Dist: wheel~=0.40.0
+Description-Content-Type: text/markdown
 
 # Execy
 
 The ececy exec_time decorator is a utility that measures the execution time of a function. It can be used to easily track and log the time taken by a function to execute, both for synchronous and asynchronous functions.
 
 ## Table of Contents
```

### Comparing `execy-0.1.1/README.md` & `execy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `execy-0.1.1/pyproject.toml` & `execy-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "execy"
-version = "0.1.1"
-description = "Add a short description here"
+version = "0.1.2"
+description = "The ececy exec_time decorator is a utility that measures the execution time of a function. It can be used to easily track and log the time taken by a function to execute, both for synchronous and asynchronous functions."
 authors = [
     { name = "hglong16", email = "intihad.vuong@gmail.com" }
 ]
 dependencies = ["pytest-asyncio~=0.21.0", "setuptools~=67.8.0", "wheel~=0.40.0", "twine~=4.0.2"]
 readme = "README.md"
 requires-python = ">= 3.8"
```

### Comparing `execy-0.1.1/src/exectime/exec.py` & `execy-0.1.2/src/exectime/exec.py`

 * *Files identical despite different names*

### Comparing `execy-0.1.1/tests/test_exec.py` & `execy-0.1.2/tests/test_exec.py`

 * *Files identical despite different names*

