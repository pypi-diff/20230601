# Comparing `tmp/oneoneoneexample-0.7.tar.gz` & `tmp/oneoneoneexample-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneoneoneexample-0.7.tar", last modified: Thu Jun  1 19:39:49 2023, max compression
+gzip compressed data, was "oneoneoneexample-0.8.tar", last modified: Thu Jun  1 19:44:22 2023, max compression
```

## Comparing `oneoneoneexample-0.7.tar` & `oneoneoneexample-0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 19:39:49.500258 oneoneoneexample-0.7/
--rw-rw-rw-   0        0        0       61 2023-06-01 19:39:49.499178 oneoneoneexample-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2168 2023-06-01 19:37:58.000000 oneoneoneexample-0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 19:39:49.476494 oneoneoneexample-0.7/oneoneoneexample.egg-info/
--rw-rw-rw-   0        0        0       61 2023-06-01 19:39:49.000000 oneoneoneexample-0.7/oneoneoneexample.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-06-01 19:39:49.000000 oneoneoneexample-0.7/oneoneoneexample.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 19:39:49.000000 oneoneoneexample-0.7/oneoneoneexample.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-01 19:39:49.000000 oneoneoneexample-0.7/oneoneoneexample.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-01 19:39:49.000000 oneoneoneexample-0.7/oneoneoneexample.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 19:39:49.487291 oneoneoneexample-0.7/pdf_generator/
--rw-rw-rw-   0        0        0     5640 2023-06-01 19:32:12.000000 oneoneoneexample-0.7/pdf_generator/convert.py
--rw-rw-rw-   0        0        0      239 2023-06-01 19:38:41.000000 oneoneoneexample-0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 19:39:49.500258 oneoneoneexample-0.7/setup.cfg
--rw-rw-rw-   0        0        0      237 2023-05-31 21:36:29.000000 oneoneoneexample-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:44:22.038294 oneoneoneexample-0.8/
+-rw-rw-rw-   0        0        0     2274 2023-06-01 19:44:22.036955 oneoneoneexample-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2168 2023-06-01 19:37:58.000000 oneoneoneexample-0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 19:44:22.022114 oneoneoneexample-0.8/oneoneoneexample.egg-info/
+-rw-rw-rw-   0        0        0     2274 2023-06-01 19:44:21.000000 oneoneoneexample-0.8/oneoneoneexample.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-01 19:44:21.000000 oneoneoneexample-0.8/oneoneoneexample.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 19:44:21.000000 oneoneoneexample-0.8/oneoneoneexample.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-01 19:44:21.000000 oneoneoneexample-0.8/oneoneoneexample.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-01 19:44:21.000000 oneoneoneexample-0.8/oneoneoneexample.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 19:44:22.024284 oneoneoneexample-0.8/pdf_generator/
+-rw-rw-rw-   0        0        0     5640 2023-06-01 19:32:12.000000 oneoneoneexample-0.8/pdf_generator/convert.py
+-rw-rw-rw-   0        0        0      239 2023-06-01 19:43:04.000000 oneoneoneexample-0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 19:44:22.039301 oneoneoneexample-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      423 2023-06-01 19:42:49.000000 oneoneoneexample-0.8/setup.py
```

### Comparing `oneoneoneexample-0.7/README.md` & `oneoneoneexample-0.8/README.md`

 * *Files identical despite different names*

### Comparing `oneoneoneexample-0.7/pdf_generator/convert.py` & `oneoneoneexample-0.8/pdf_generator/convert.py`

 * *Files identical despite different names*

