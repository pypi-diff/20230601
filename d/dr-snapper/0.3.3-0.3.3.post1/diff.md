# Comparing `tmp/dr_snapper-0.3.3.tar.gz` & `tmp/dr_snapper-0.3.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dr_snapper-0.3.3.tar", max compression
+gzip compressed data, was "dr_snapper-0.3.3.post1.tar", max compression
```

## Comparing `dr_snapper-0.3.3.tar` & `dr_snapper-0.3.3.post1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-05-08 05:46:15.213407 dr_snapper-0.3.3/LICENSE
--rw-r--r--   0        0        0      978 2023-06-01 05:05:18.205434 dr_snapper-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 05:46:15.214674 dr_snapper-0.3.3/snapper/__init__.py
--rw-r--r--   0        0        0     8957 2023-05-08 05:46:15.214800 dr_snapper-0.3.3/snapper/cli.py
--rw-r--r--   0        0        0     1482 2023-05-08 05:46:15.214900 dr_snapper-0.3.3/snapper/utils.py
--rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 dr_snapper-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-08 05:46:15.213407 dr_snapper-0.3.3.post1/LICENSE
+-rw-r--r--   0        0        0     4635 2023-05-08 05:46:15.213511 dr_snapper-0.3.3.post1/README.md
+-rw-r--r--   0        0        0     1309 2023-06-01 05:16:15.444722 dr_snapper-0.3.3.post1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 05:46:15.214674 dr_snapper-0.3.3.post1/snapper/__init__.py
+-rw-r--r--   0        0        0     8957 2023-05-08 05:46:15.214800 dr_snapper-0.3.3.post1/snapper/cli.py
+-rw-r--r--   0        0        0     1482 2023-05-08 05:46:15.214900 dr_snapper-0.3.3.post1/snapper/utils.py
+-rw-r--r--   0        0        0     5600 1970-01-01 00:00:00.000000 dr_snapper-0.3.3.post1/PKG-INFO
```

### Comparing `dr_snapper-0.3.3/LICENSE` & `dr_snapper-0.3.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `dr_snapper-0.3.3/pyproject.toml` & `dr_snapper-0.3.3.post1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 [tool.poetry]
 name = "dr-snapper"
-version = "0.3.3"
+version = "0.3.3.post1"
 description = "Create a new timeline 'snapshot' to revert to when trying out risky ideas in DaVinci Resolve"
 authors = ["Caleb Trevatt <in03@users.noreply.github.com>"]
+readme = "README.md"
+homepage = "https://github.com/in03/snapper"
+repository = "https://github.com/in03/snapper"
+keywords = ["DaVinci Resolve", "Scripting", "Backups", "CLI"]
 license = "MIT"
 
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+]
+
 packages = [
 
     {include = "snapper"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10.0, <3.12.0"
```

### Comparing `dr_snapper-0.3.3/snapper/cli.py` & `dr_snapper-0.3.3.post1/snapper/cli.py`

 * *Files identical despite different names*

### Comparing `dr_snapper-0.3.3/snapper/utils.py` & `dr_snapper-0.3.3.post1/snapper/utils.py`

 * *Files identical despite different names*

