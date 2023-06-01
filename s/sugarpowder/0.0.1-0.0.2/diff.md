# Comparing `tmp/sugarpowder-0.0.1.tar.gz` & `tmp/sugarpowder-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sugarpowder-0.0.1.tar", last modified: Thu Jun  1 03:17:34 2023, max compression
+gzip compressed data, was "sugarpowder-0.0.2.tar", last modified: Thu Jun  1 07:53:47 2023, max compression
```

## Comparing `sugarpowder-0.0.1.tar` & `sugarpowder-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-06-01 03:17:34.748940 sugarpowder-0.0.1/
--rw-r--r--   0 docker    (1000) docker    (1000)     1083 2023-05-31 23:29:34.000000 sugarpowder-0.0.1/LICENSE
--rw-r--r--   0 docker    (1000) docker    (1000)     2395 2023-06-01 03:17:34.748940 sugarpowder-0.0.1/PKG-INFO
--rw-r--r--   0 docker    (1000) docker    (1000)      531 2023-06-01 00:41:58.000000 sugarpowder-0.0.1/README.md
--rw-r--r--   0 docker    (1000) docker    (1000)      681 2023-06-01 03:16:40.000000 sugarpowder-0.0.1/pyproject.toml
--rw-r--r--   0 docker    (1000) docker    (1000)       38 2023-06-01 03:17:34.748940 sugarpowder-0.0.1/setup.cfg
--rw-r--r--   0 docker    (1000) docker    (1000)      435 2023-06-01 03:05:45.000000 sugarpowder-0.0.1/setup.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-06-01 03:17:34.748940 sugarpowder-0.0.1/src/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-06-01 03:17:34.748940 sugarpowder-0.0.1/src/sugarpowder/
--rw-r--r--   0 docker    (1000) docker    (1000)      100 2023-05-31 23:41:04.000000 sugarpowder-0.0.1/src/sugarpowder/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5307 2023-06-01 00:38:24.000000 sugarpowder-0.0.1/src/sugarpowder/pipes.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1049 2023-05-31 23:49:44.000000 sugarpowder-0.0.1/src/sugarpowder/witherr.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-06-01 03:17:34.748940 sugarpowder-0.0.1/src/sugarpowder.egg-info/
--rw-r--r--   0 docker    (1000) docker    (1000)     2395 2023-06-01 03:17:34.000000 sugarpowder-0.0.1/src/sugarpowder.egg-info/PKG-INFO
--rw-r--r--   0 docker    (1000) docker    (1000)      329 2023-06-01 03:17:34.000000 sugarpowder-0.0.1/src/sugarpowder.egg-info/SOURCES.txt
--rw-r--r--   0 docker    (1000) docker    (1000)        1 2023-06-01 03:17:34.000000 sugarpowder-0.0.1/src/sugarpowder.egg-info/dependency_links.txt
--rw-r--r--   0 docker    (1000) docker    (1000)        1 2023-06-01 03:05:51.000000 sugarpowder-0.0.1/src/sugarpowder.egg-info/not-zip-safe
--rw-r--r--   0 docker    (1000) docker    (1000)       12 2023-06-01 03:17:34.000000 sugarpowder-0.0.1/src/sugarpowder.egg-info/top_level.txt
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-06-01 03:17:34.748940 sugarpowder-0.0.1/tests/
--rw-r--r--   0 docker    (1000) docker    (1000)      938 2023-06-01 00:42:04.000000 sugarpowder-0.0.1/tests/test.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-06-01 07:53:47.578352 sugarpowder-0.0.2/
+-rw-r--r--   0 docker    (1000) docker    (1000)     1083 2023-05-31 23:29:34.000000 sugarpowder-0.0.2/LICENSE
+-rw-r--r--   0 docker    (1000) docker    (1000)     2395 2023-06-01 07:53:47.578352 sugarpowder-0.0.2/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)      531 2023-06-01 00:41:58.000000 sugarpowder-0.0.2/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      681 2023-06-01 07:53:40.000000 sugarpowder-0.0.2/pyproject.toml
+-rw-r--r--   0 docker    (1000) docker    (1000)       38 2023-06-01 07:53:47.578352 sugarpowder-0.0.2/setup.cfg
+-rw-r--r--   0 docker    (1000) docker    (1000)      436 2023-06-01 07:53:34.000000 sugarpowder-0.0.2/setup.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-06-01 07:53:47.578352 sugarpowder-0.0.2/src/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-06-01 07:53:47.578352 sugarpowder-0.0.2/src/sugarpowder/
+-rw-r--r--   0 docker    (1000) docker    (1000)      100 2023-05-31 23:41:04.000000 sugarpowder-0.0.2/src/sugarpowder/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      225 2023-06-01 07:51:54.000000 sugarpowder-0.0.2/src/sugarpowder/mark_time.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5307 2023-06-01 00:38:24.000000 sugarpowder-0.0.2/src/sugarpowder/pipes.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1049 2023-05-31 23:49:44.000000 sugarpowder-0.0.2/src/sugarpowder/witherr.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-06-01 07:53:47.578352 sugarpowder-0.0.2/src/sugarpowder.egg-info/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2395 2023-06-01 07:53:47.000000 sugarpowder-0.0.2/src/sugarpowder.egg-info/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)      344 2023-06-01 07:53:47.000000 sugarpowder-0.0.2/src/sugarpowder.egg-info/SOURCES.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        1 2023-06-01 07:53:47.000000 sugarpowder-0.0.2/src/sugarpowder.egg-info/dependency_links.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        1 2023-06-01 03:05:51.000000 sugarpowder-0.0.2/src/sugarpowder.egg-info/not-zip-safe
+-rw-r--r--   0 docker    (1000) docker    (1000)       12 2023-06-01 07:53:47.000000 sugarpowder-0.0.2/src/sugarpowder.egg-info/top_level.txt
```

### Comparing `sugarpowder-0.0.1/LICENSE` & `sugarpowder-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sugarpowder-0.0.1/PKG-INFO` & `sugarpowder-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sugarpowder
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package of Python syntactic sugars inspired by Elixir, Go, Rust, Julia, and other languages
 Author: Geunseong Jung
 Author-email: Geunseong Jung <dreamwayjgs@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Geunseong Jung (정근성)
```

### Comparing `sugarpowder-0.0.1/README.md` & `sugarpowder-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sugarpowder-0.0.1/pyproject.toml` & `sugarpowder-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sugarpowder"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Geunseong Jung", email="dreamwayjgs@gmail.com" },
 ]
 description = "Package of Python syntactic sugars inspired by Elixir, Go, Rust, Julia, and other languages"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

### Comparing `sugarpowder-0.0.1/src/sugarpowder/pipes.py` & `sugarpowder-0.0.2/src/sugarpowder/pipes.py`

 * *Files identical despite different names*

### Comparing `sugarpowder-0.0.1/src/sugarpowder/witherr.py` & `sugarpowder-0.0.2/src/sugarpowder/witherr.py`

 * *Files identical despite different names*

### Comparing `sugarpowder-0.0.1/src/sugarpowder.egg-info/PKG-INFO` & `sugarpowder-0.0.2/src/sugarpowder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sugarpowder
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package of Python syntactic sugars inspired by Elixir, Go, Rust, Julia, and other languages
 Author: Geunseong Jung
 Author-email: Geunseong Jung <dreamwayjgs@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Geunseong Jung (정근성)
```

