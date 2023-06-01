# Comparing `tmp/packaging-demo-eric-0.0.3.tar.gz` & `tmp/packaging-demo-eric-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaging-demo-eric-0.0.3.tar", last modified: Tue May 30 22:39:40 2023, max compression
+gzip compressed data, was "packaging-demo-eric-0.0.5.tar", last modified: Thu Jun  1 07:10:20 2023, max compression
```

## Comparing `packaging-demo-eric-0.0.3.tar` & `packaging-demo-eric-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-05-30 22:39:40.254357 packaging-demo-eric-0.0.3/
--rw-r--r--   0 eric      (1000) eric      (1000)      458 2023-05-30 22:39:40.254357 packaging-demo-eric-0.0.3/PKG-INFO
--rw-r--r--   0 eric      (1000) eric      (1000)       74 2023-05-09 21:25:38.000000 packaging-demo-eric-0.0.3/README.md
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-05-30 22:39:40.254357 packaging-demo-eric-0.0.3/packaging_demo/
--rw-r--r--   0 eric      (1000) eric      (1000)       18 2023-05-10 03:25:38.000000 packaging-demo-eric-0.0.3/packaging_demo/__init__.py
--rw-r--r--   0 eric      (1000) eric      (1000)      109 2023-05-30 21:29:39.000000 packaging-demo-eric-0.0.3/packaging_demo/colorized_demo.py
--rw-r--r--   0 eric      (1000) eric      (1000)      195 2023-05-10 03:26:10.000000 packaging-demo-eric-0.0.3/packaging_demo/my_file.py
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-05-30 22:39:40.254357 packaging-demo-eric-0.0.3/packaging_demo/my_folder/
--rw-r--r--   0 eric      (1000) eric      (1000)        6 2023-05-10 03:25:38.000000 packaging-demo-eric-0.0.3/packaging_demo/my_folder/__init__.py
--rw-r--r--   0 eric      (1000) eric      (1000)      101 2023-05-30 21:56:08.000000 packaging-demo-eric-0.0.3/packaging_demo/my_folder/my_nested_file.py
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-05-30 22:39:40.254357 packaging-demo-eric-0.0.3/packaging_demo/my_folder/sub_package/
--rw-r--r--   0 eric      (1000) eric      (1000)        0 2023-05-10 03:22:22.000000 packaging-demo-eric-0.0.3/packaging_demo/my_folder/sub_package/__init__.py
--rw-r--r--   0 eric      (1000) eric      (1000)        0 2023-05-03 10:03:22.000000 packaging-demo-eric-0.0.3/packaging_demo/my_folder/sub_package/some_deeply_nested_file.py
--rw-r--r--   0 eric      (1000) eric      (1000)       25 2023-05-10 03:25:38.000000 packaging-demo-eric-0.0.3/packaging_demo/my_other_file.py
--rw-r--r--   0 eric      (1000) eric      (1000)      678 2023-05-30 21:29:41.000000 packaging-demo-eric-0.0.3/packaging_demo/states_info.py
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-05-30 22:39:40.254357 packaging-demo-eric-0.0.3/packaging_demo_eric.egg-info/
--rw-r--r--   0 eric      (1000) eric      (1000)      458 2023-05-30 22:39:40.000000 packaging-demo-eric-0.0.3/packaging_demo_eric.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) eric      (1000)      579 2023-05-30 22:39:40.000000 packaging-demo-eric-0.0.3/packaging_demo_eric.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) eric      (1000)        1 2023-05-30 22:39:40.000000 packaging-demo-eric-0.0.3/packaging_demo_eric.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) eric      (1000)      181 2023-05-30 22:39:40.000000 packaging-demo-eric-0.0.3/packaging_demo_eric.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) eric      (1000)       15 2023-05-30 22:39:40.000000 packaging-demo-eric-0.0.3/packaging_demo_eric.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) eric      (1000)     1983 2023-05-30 22:39:33.000000 packaging-demo-eric-0.0.3/pyproject.toml
--rw-r--r--   0 eric      (1000) eric      (1000)       38 2023-05-30 22:39:40.254357 packaging-demo-eric-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:20.168200 packaging-demo-eric-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 07:10:20.168200 packaging-demo-eric-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:20.168200 packaging-demo-eric-0.0.5/packaging_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/colorized_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/my_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:20.168200 packaging-demo-eric-0.0.5/packaging_demo/my_folder/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/my_folder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/my_folder/my_nested_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:20.168200 packaging-demo-eric-0.0.5/packaging_demo/my_folder/sub_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/my_folder/sub_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/my_folder/sub_package/some_deeply_nested_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/my_other_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/packaging_demo/states_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:20.168200 packaging-demo-eric-0.0.5/packaging_demo_eric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 07:10:20.000000 packaging-demo-eric-0.0.5/packaging_demo_eric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-01 07:10:20.000000 packaging-demo-eric-0.0.5/packaging_demo_eric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:10:20.000000 packaging-demo-eric-0.0.5/packaging_demo_eric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 07:10:20.000000 packaging-demo-eric-0.0.5/packaging_demo_eric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 07:10:20.000000 packaging-demo-eric-0.0.5/packaging_demo_eric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 07:10:20.168200 packaging-demo-eric-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 07:09:38.000000 packaging-demo-eric-0.0.5/version.txt
```

### Comparing `packaging-demo-eric-0.0.3/packaging_demo/states_info.py` & `packaging-demo-eric-0.0.5/packaging_demo/states_info.py`

 * *Files identical despite different names*

### Comparing `packaging-demo-eric-0.0.3/packaging_demo_eric.egg-info/SOURCES.txt` & `packaging-demo-eric-0.0.5/packaging_demo_eric.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 README.md
 pyproject.toml
+version.txt
 packaging_demo/__init__.py
 packaging_demo/colorized_demo.py
 packaging_demo/my_file.py
 packaging_demo/my_other_file.py
 packaging_demo/states_info.py
 packaging_demo/my_folder/__init__.py
 packaging_demo/my_folder/my_nested_file.py
```

### Comparing `packaging-demo-eric-0.0.3/pyproject.toml` & `packaging-demo-eric-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.package-data]
 package_demo = ["*.json"]
 
 [project]
 name = "packaging-demo-eric"
-version = "0.0.3"
 authors = [
     {name = "Eric Riddoch", email = "some-email@gmail.com"},
 ]
 description = "My package description"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["one", "two"]
@@ -20,23 +19,25 @@
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "numpy",
     'importlib-metadata; python_version<"3.8"',
 ]
-
-# dynamic = ["version"]
+dynamic = ["version"]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov"]
 release = ["build", "twine"]
 static-code-qa = ["pre-commit"]
-dev = ["packaging-demo[test,release,static-code-qa]"]
+dev = ["packaging-demo-eric[test,release,static-code-qa]"]
+
 
+[tool.setuptools.dynamic]
+version = {file = "version.txt"}
 
 [tool.black]
 line-length = 119
 exclude = [
     "venv"
 ]
```

