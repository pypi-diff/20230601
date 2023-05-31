# Comparing `tmp/motion_python-0.1.44.tar.gz` & `tmp/motion_python-0.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.44.tar", max compression
+gzip compressed data, was "motion_python-0.1.45.tar", max compression
```

## Comparing `motion_python-0.1.44.tar` & `motion_python-0.1.45.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3319 2023-05-31 21:42:14.375259 motion_python-0.1.44/README.md
--rw-r--r--   0        0        0      202 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/__init__.py
--rw-r--r--   0        0        0     1817 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/cli.py
--rw-r--r--   0        0        0    23617 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/component.py
--rw-r--r--   0        0        0    12098 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/execute.py
--rw-r--r--   0        0        0     4392 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/fit_task.py
--rw-r--r--   0        0        0     7489 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      595 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/route.py
--rw-r--r--   0        0        0     6283 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/utils.py
--rw-r--r--   0        0        0     1775 2023-05-31 21:42:39.411378 motion_python-0.1.44/pyproject.toml
--rw-r--r--   0        0        0     4563 1970-01-01 00:00:00.000000 motion_python-0.1.44/PKG-INFO
+-rw-r--r--   0        0        0     3319 2023-05-31 23:35:00.799328 motion_python-0.1.45/README.md
+-rw-r--r--   0        0        0      202 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/__init__.py
+-rw-r--r--   0        0        0     1817 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/cli.py
+-rw-r--r--   0        0        0    23617 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/component.py
+-rw-r--r--   0        0        0    12098 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/execute.py
+-rw-r--r--   0        0        0     4392 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/fit_task.py
+-rw-r--r--   0        0        0     7489 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      595 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/route.py
+-rw-r--r--   0        0        0     6283 2023-05-31 23:35:00.799328 motion_python-0.1.45/motion/utils.py
+-rw-r--r--   0        0        0     1775 2023-05-31 23:35:20.415195 motion_python-0.1.45/pyproject.toml
+-rw-r--r--   0        0        0     4563 1970-01-01 00:00:00.000000 motion_python-0.1.45/PKG-INFO
```

### Comparing `motion_python-0.1.44/README.md` & `motion_python-0.1.45/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.44/motion/cli.py` & `motion_python-0.1.45/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.44/motion/component.py` & `motion_python-0.1.45/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.44/motion/execute.py` & `motion_python-0.1.45/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.44/motion/fit_task.py` & `motion_python-0.1.45/motion/fit_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.44/motion/instance.py` & `motion_python-0.1.45/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.44/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.45/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.44/motion/route.py` & `motion_python-0.1.45/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.44/motion/utils.py` & `motion_python-0.1.45/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.44/pyproject.toml` & `motion_python-0.1.45/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.44"
+version = "0.1.45"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.44/PKG-INFO` & `motion_python-0.1.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.44
+Version: 0.1.45
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

