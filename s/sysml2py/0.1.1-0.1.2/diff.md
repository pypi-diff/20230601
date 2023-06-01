# Comparing `tmp/sysml2py-0.1.1.tar.gz` & `tmp/sysml2py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysml2py-0.1.1.tar", last modified: Thu Jun  1 12:18:22 2023, max compression
+gzip compressed data, was "sysml2py-0.1.2.tar", last modified: Thu Jun  1 12:44:34 2023, max compression
```

## Comparing `sysml2py-0.1.1.tar` & `sysml2py-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:18:22.236061 sysml2py-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 12:18:02.000000 sysml2py-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-01 12:18:22.236061 sysml2py-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-01 12:18:02.000000 sysml2py-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-01 12:18:02.000000 sysml2py-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:18:22.236061 sysml2py-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:18:22.236061 sysml2py-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:18:22.236061 sysml2py-0.1.1/src/sysml2py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:18:22.236061 sysml2py-0.1.1/src/sysml2py/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)    22327 2023-06-01 12:18:02.000000 sysml2py-0.1.1/src/sysml2py/grammar/KerML.tx
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-06-01 12:18:02.000000 sysml2py-0.1.1/src/sysml2py/grammar/KerMLExpressions.tx
--rw-r--r--   0 runner    (1001) docker     (123)    46559 2023-06-01 12:18:02.000000 sysml2py-0.1.1/src/sysml2py/grammar/SysML.tx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:18:22.236061 sysml2py-0.1.1/src/sysml2py/sysml2py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-01 12:18:22.000000 sysml2py-0.1.1/src/sysml2py/sysml2py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-01 12:18:22.000000 sysml2py-0.1.1/src/sysml2py/sysml2py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:18:22.000000 sysml2py-0.1.1/src/sysml2py/sysml2py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 12:18:22.000000 sysml2py-0.1.1/src/sysml2py/sysml2py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:18:22.236061 sysml2py-0.1.1/src/sysml2py/textx/
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-01 12:18:02.000000 sysml2py-0.1.1/src/sysml2py/textx/xtext_to_textx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:44:34.429178 sysml2py-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 12:44:14.000000 sysml2py-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-01 12:44:34.429178 sysml2py-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-01 12:44:14.000000 sysml2py-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-01 12:44:14.000000 sysml2py-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:44:34.429178 sysml2py-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:44:34.425178 sysml2py-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:44:34.429178 sysml2py-0.1.2/src/sysml2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-01 12:44:14.000000 sysml2py-0.1.2/src/sysml2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-01 12:44:14.000000 sysml2py-0.1.2/src/sysml2py/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:44:34.429178 sysml2py-0.1.2/src/sysml2py/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)    22327 2023-06-01 12:44:14.000000 sysml2py-0.1.2/src/sysml2py/grammar/KerML.tx
+-rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-06-01 12:44:14.000000 sysml2py-0.1.2/src/sysml2py/grammar/KerMLExpressions.tx
+-rw-r--r--   0 runner    (1001) docker     (123)    46559 2023-06-01 12:44:14.000000 sysml2py-0.1.2/src/sysml2py/grammar/SysML.tx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:44:34.429178 sysml2py-0.1.2/src/sysml2py/textx/
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-01 12:44:14.000000 sysml2py-0.1.2/src/sysml2py/textx/xtext_to_textx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-01 12:44:14.000000 sysml2py-0.1.2/src/sysml2py/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:44:34.429178 sysml2py-0.1.2/sysml2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-01 12:44:34.000000 sysml2py-0.1.2/sysml2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-01 12:44:34.000000 sysml2py-0.1.2/sysml2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:44:34.000000 sysml2py-0.1.2/sysml2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 12:44:34.000000 sysml2py-0.1.2/sysml2py.egg-info/top_level.txt
```

### Comparing `sysml2py-0.1.1/LICENSE` & `sysml2py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sysml2py-0.1.1/PKG-INFO` & `sysml2py-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysml2py
-Version: 0.1.1
+Version: 0.1.2
 Summary: SysML v2.0 Parser
 Author-email: Christopher Cox <chris.cox@westfall.io>
 Project-URL: Homepage, https://github.com/Westfall-io/sysml2py
 Project-URL: Bug Tracker, https://github.com/Westfall-io/sysml2py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sysml2py-0.1.1/README.md` & `sysml2py-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sysml2py-0.1.1/pyproject.toml` & `sysml2py-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysml2py"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Christopher Cox", email="chris.cox@westfall.io" },
 ]
 description = "SysML v2.0 Parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -20,15 +20,15 @@
 [tool.setuptools]
 # ...
 # By default, include-package-data is true in pyproject.toml, so you do
 # NOT have to specify this line.
 include-package-data = true
 
 [tool.setuptools.packages.find]
-where = ["src/sysml2py"]
+where = ["src/sysml2py", "src"]
 
 [tool.setuptools.package-data]
 grammar = ["*.tx"]
 
 [project.urls]
 "Homepage" = "https://github.com/Westfall-io/sysml2py"
 "Bug Tracker" = "https://github.com/Westfall-io/sysml2py/issues"
```

### Comparing `sysml2py-0.1.1/src/sysml2py/grammar/KerML.tx` & `sysml2py-0.1.2/src/sysml2py/grammar/KerML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.1.1/src/sysml2py/grammar/KerMLExpressions.tx` & `sysml2py-0.1.2/src/sysml2py/grammar/KerMLExpressions.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.1.1/src/sysml2py/grammar/SysML.tx` & `sysml2py-0.1.2/src/sysml2py/grammar/SysML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.1.1/src/sysml2py/sysml2py.egg-info/PKG-INFO` & `sysml2py-0.1.2/sysml2py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysml2py
-Version: 0.1.1
+Version: 0.1.2
 Summary: SysML v2.0 Parser
 Author-email: Christopher Cox <chris.cox@westfall.io>
 Project-URL: Homepage, https://github.com/Westfall-io/sysml2py
 Project-URL: Bug Tracker, https://github.com/Westfall-io/sysml2py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sysml2py-0.1.1/src/sysml2py/textx/xtext_to_textx.py` & `sysml2py-0.1.2/src/sysml2py/textx/xtext_to_textx.py`

 * *Files identical despite different names*

