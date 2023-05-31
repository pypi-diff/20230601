# Comparing `tmp/motion_python-0.1.45.tar.gz` & `tmp/motion_python-0.1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.45.tar", max compression
+gzip compressed data, was "motion_python-0.1.46.tar", max compression
```

## Comparing `motion_python-0.1.45.tar` & `motion_python-0.1.46.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3319 2023-05-31 23:35:00.799328 motion_python-0.1.45/README.md
--rw-r--r--   0        0        0      202 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/__init__.py
--rw-r--r--   0        0        0     1817 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/cli.py
--rw-r--r--   0        0        0    23617 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/component.py
--rw-r--r--   0        0        0    12098 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/execute.py
--rw-r--r--   0        0        0     4392 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/fit_task.py
--rw-r--r--   0        0        0     7489 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      595 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/route.py
--rw-r--r--   0        0        0     6283 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/utils.py
--rw-r--r--   0        0        0     1775 2023-05-31 23:35:20.415195 motion_python-0.1.45/pyproject.toml
--rw-r--r--   0        0        0     4563 1970-01-01 00:00:00.000000 motion_python-0.1.45/PKG-INFO
+-rw-r--r--   0        0        0     3319 2023-05-31 23:50:19.038567 motion_python-0.1.46/README.md
+-rw-r--r--   0        0        0      202 2023-05-31 23:50:19.038567 motion_python-0.1.46/motion/__init__.py
+-rw-r--r--   0        0        0     1817 2023-05-31 23:50:19.038567 motion_python-0.1.46/motion/cli.py
+-rw-r--r--   0        0        0    23617 2023-05-31 23:50:19.038567 motion_python-0.1.46/motion/component.py
+-rw-r--r--   0        0        0    12098 2023-05-31 23:50:19.038567 motion_python-0.1.46/motion/execute.py
+-rw-r--r--   0        0        0     4392 2023-05-31 23:50:19.038567 motion_python-0.1.46/motion/fit_task.py
+-rw-r--r--   0        0        0     7489 2023-05-31 23:50:19.038567 motion_python-0.1.46/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-05-31 23:50:19.042567 motion_python-0.1.46/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      595 2023-05-31 23:50:19.042567 motion_python-0.1.46/motion/route.py
+-rw-r--r--   0        0        0     6283 2023-05-31 23:50:19.042567 motion_python-0.1.46/motion/utils.py
+-rw-r--r--   0        0        0     1773 2023-05-31 23:50:37.678846 motion_python-0.1.46/pyproject.toml
+-rw-r--r--   0        0        0     4559 1970-01-01 00:00:00.000000 motion_python-0.1.46/PKG-INFO
```

### Comparing `motion_python-0.1.45/README.md` & `motion_python-0.1.46/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.45/motion/cli.py` & `motion_python-0.1.46/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.45/motion/component.py` & `motion_python-0.1.46/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.45/motion/execute.py` & `motion_python-0.1.46/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.45/motion/fit_task.py` & `motion_python-0.1.46/motion/fit_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.45/motion/instance.py` & `motion_python-0.1.46/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.45/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.46/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.45/motion/route.py` & `motion_python-0.1.46/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.45/motion/utils.py` & `motion_python-0.1.46/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.45/pyproject.toml` & `motion_python-0.1.46/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.45"
+version = "0.1.46"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -20,15 +20,15 @@
 uvicorn = "^0.21.1"
 httpx = "^0.23.3"
 python-multipart = "^0.0.6"
 pydantic = "^1.10.7"
 urllib3 = "^1.26.15"
 flask = "^2.2.3"
 rich = "^13.3.4"
-cloudpickle = "^2.2.1"
+cloudpickle = "^2.1"
 redis = "^4.5.5"
 psutil = "^5.9.5"
 
 [tool.poetry.group.dev.dependencies]
 poetry-types = "^0.3.5"
 pytest = "^7.2.2"
 mypy = "^1.1.1"
```

### Comparing `motion_python-0.1.45/PKG-INFO` & `motion_python-0.1.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.45
+Version: 0.1.46
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
+Requires-Dist: cloudpickle (>=2.1,<3.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: croniter (>=1.3.8,<2.0.0)
 Requires-Dist: duckdb (>=0.7.1,<0.8.0)
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: flask (>=2.2.3,<3.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
```

