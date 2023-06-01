# Comparing `tmp/execy-0.1.6.tar.gz` & `tmp/execy-0.1.7.tar.gz`

## Comparing `execy-0.1.6.tar` & `execy-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 execy-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 execy-0.1.6/.python-version
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 execy-0.1.6/requirements-dev.lock
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 execy-0.1.6/requirements.lock
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 execy-0.1.6/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 execy-0.1.6/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 execy-0.1.6/.pytest_cache/README.md
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 execy-0.1.6/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 execy-0.1.6/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 execy-0.1.6/.vscode/settings.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 execy-0.1.6/src/execy/__init__.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 execy-0.1.6/src/execy/exec.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 execy-0.1.6/tests/test_exec.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 execy-0.1.6/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 execy-0.1.6/LICENSE
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 execy-0.1.6/README.md
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 execy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 execy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 execy-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 execy-0.1.7/.python-version
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 execy-0.1.7/requirements-dev.lock
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 execy-0.1.7/requirements.lock
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 execy-0.1.7/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 execy-0.1.7/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 execy-0.1.7/.pytest_cache/README.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 execy-0.1.7/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 execy-0.1.7/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 execy-0.1.7/.vscode/settings.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 execy-0.1.7/src/execy/__init__.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 execy-0.1.7/src/execy/exec.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 execy-0.1.7/tests/test_exec.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 execy-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 execy-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 execy-0.1.7/README.md
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 execy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 execy-0.1.7/PKG-INFO
```

### Comparing `execy-0.1.6/src/execy/exec.py` & `execy-0.1.7/src/execy/exec.py`

 * *Files identical despite different names*

### Comparing `execy-0.1.6/tests/test_exec.py` & `execy-0.1.7/tests/test_exec.py`

 * *Files identical despite different names*

### Comparing `execy-0.1.6/LICENSE` & `execy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `execy-0.1.6/README.md` & `execy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `execy-0.1.6/pyproject.toml` & `execy-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "execy"
-version = "0.1.6"
+version = "0.1.7"
 description = "The ececy exec_time decorator is a utility that measures the execution time of a function. It can be used to easily track and log the time taken by a function to execute, both for synchronous and asynchronous functions."
 authors = [
     { name = "hglong16", email = "intihad.vuong@gmail.com" }
 ]
 dependencies = []
 readme = "README.md"
 requires-python = ">= 3.8"
```

### Comparing `execy-0.1.6/PKG-INFO` & `execy-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: execy
-Version: 0.1.6
+Version: 0.1.7
 Summary: The ececy exec_time decorator is a utility that measures the execution time of a function. It can be used to easily track and log the time taken by a function to execute, both for synchronous and asynchronous functions.
 Author-email: hglong16 <intihad.vuong@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Execy
```

