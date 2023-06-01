# Comparing `tmp/execy-0.1.3.tar.gz` & `tmp/execy-0.1.4.tar.gz`

## Comparing `execy-0.1.3.tar` & `execy-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 execy-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 execy-0.1.3/.python-version
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 execy-0.1.3/requirements-dev.lock
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 execy-0.1.3/requirements.lock
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 execy-0.1.3/setup.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 execy-0.1.3/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 execy-0.1.3/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 execy-0.1.3/.pytest_cache/README.md
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 execy-0.1.3/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 execy-0.1.3/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 execy-0.1.3/.vscode/settings.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 execy-0.1.3/src/exectime/__init__.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 execy-0.1.3/src/exectime/exec.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 execy-0.1.3/tests/test_exec.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 execy-0.1.3/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 execy-0.1.3/LICENSE
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 execy-0.1.3/README.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 execy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 execy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 execy-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 execy-0.1.4/.python-version
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 execy-0.1.4/requirements-dev.lock
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 execy-0.1.4/requirements.lock
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 execy-0.1.4/setup.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 execy-0.1.4/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 execy-0.1.4/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 execy-0.1.4/.pytest_cache/README.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 execy-0.1.4/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 execy-0.1.4/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 execy-0.1.4/.vscode/settings.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 execy-0.1.4/src/exectime/__init__.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 execy-0.1.4/src/exectime/exec.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 execy-0.1.4/tests/test_exec.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 execy-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 execy-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 execy-0.1.4/README.md
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 execy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 execy-0.1.4/PKG-INFO
```

### Comparing `execy-0.1.3/src/exectime/exec.py` & `execy-0.1.4/src/exectime/exec.py`

 * *Files identical despite different names*

### Comparing `execy-0.1.3/tests/test_exec.py` & `execy-0.1.4/tests/test_exec.py`

 * *Files identical despite different names*

### Comparing `execy-0.1.3/LICENSE` & `execy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `execy-0.1.3/README.md` & `execy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `execy-0.1.3/pyproject.toml` & `execy-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [project]
 name = "execy"
-version = "0.1.3"
+version = "0.1.4"
 description = "The ececy exec_time decorator is a utility that measures the execution time of a function. It can be used to easily track and log the time taken by a function to execute, both for synchronous and asynchronous functions."
 authors = [
     { name = "hglong16", email = "intihad.vuong@gmail.com" }
 ]
-dependencies = ["pytest-asyncio~=0.21.0", "setuptools~=67.8.0", "wheel~=0.40.0", "twine~=4.0.2"]
+dependencies = []
 readme = "README.md"
 requires-python = ">= 3.8"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye.scripts]
-build = "python setup.py sdist bdist_wheel"
-upload = "twine upload dist/*"
 
 [tool.rye]
 managed = true
 dev-dependencies = ["pytest~=7.3.1", "black~=23.3.0", "isort~=5.12.0"]
 [tool.hatch.metadata]
 allow-direct-references = true
```

### Comparing `execy-0.1.3/PKG-INFO` & `execy-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 Metadata-Version: 2.1
 Name: execy
-Version: 0.1.3
+Version: 0.1.4
 Summary: The ececy exec_time decorator is a utility that measures the execution time of a function. It can be used to easily track and log the time taken by a function to execute, both for synchronous and asynchronous functions.
 Author-email: hglong16 <intihad.vuong@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.8
-Requires-Dist: pytest-asyncio~=0.21.0
-Requires-Dist: setuptools~=67.8.0
-Requires-Dist: twine~=4.0.2
-Requires-Dist: wheel~=0.40.0
 Description-Content-Type: text/markdown
 
 # Execy
 
 The ececy exec_time decorator is a utility that measures the execution time of a function. It can be used to easily track and log the time taken by a function to execute, both for synchronous and asynchronous functions.
 
 ## Table of Contents
```

