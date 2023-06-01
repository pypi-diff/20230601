# Comparing `tmp/educelab-cmdparse-0.1.0.tar.gz` & `tmp/educelab-cmdparse-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "educelab-cmdparse-0.1.0.tar", last modified: Wed May 31 20:09:09 2023, max compression
+gzip compressed data, was "educelab-cmdparse-0.2.0.tar", last modified: Thu Jun  1 17:25:18 2023, max compression
```

## Comparing `educelab-cmdparse-0.1.0.tar` & `educelab-cmdparse-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-31 20:09:09.876963 educelab-cmdparse-0.1.0/
--rw-r--r--   0 seth       (501) staff       (20)    34450 2023-05-31 19:36:53.000000 educelab-cmdparse-0.1.0/LICENSE
--rw-r--r--   0 seth       (501) staff       (20)     1025 2023-05-31 20:09:09.877013 educelab-cmdparse-0.1.0/PKG-INFO
--rw-r--r--   0 seth       (501) staff       (20)      318 2023-05-31 20:06:38.000000 educelab-cmdparse-0.1.0/README.md
--rw-r--r--   0 seth       (501) staff       (20)      103 2023-05-31 20:06:38.000000 educelab-cmdparse-0.1.0/pyproject.toml
--rw-r--r--   0 seth       (501) staff       (20)        0 2023-05-31 20:06:38.000000 educelab-cmdparse-0.1.0/requirements.txt
--rw-r--r--   0 seth       (501) staff       (20)      921 2023-05-31 20:09:09.877272 educelab-cmdparse-0.1.0/setup.cfg
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-31 20:09:09.875401 educelab-cmdparse-0.1.0/src/
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-31 20:09:09.875329 educelab-cmdparse-0.1.0/src/educelab/
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-31 20:09:09.876170 educelab-cmdparse-0.1.0/src/educelab/cmdparse/
--rw-r--r--   0 seth       (501) staff       (20)       49 2023-05-31 20:06:38.000000 educelab-cmdparse-0.1.0/src/educelab/cmdparse/__init__.py
--rw-r--r--   0 seth       (501) staff       (20)     1718 2023-05-31 20:06:38.000000 educelab-cmdparse-0.1.0/src/educelab/cmdparse/cmdparse.py
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-31 20:09:09.876844 educelab-cmdparse-0.1.0/src/educelab_cmdparse.egg-info/
--rw-r--r--   0 seth       (501) staff       (20)     1025 2023-05-31 20:09:09.000000 educelab-cmdparse-0.1.0/src/educelab_cmdparse.egg-info/PKG-INFO
--rw-r--r--   0 seth       (501) staff       (20)      351 2023-05-31 20:09:09.000000 educelab-cmdparse-0.1.0/src/educelab_cmdparse.egg-info/SOURCES.txt
--rw-r--r--   0 seth       (501) staff       (20)        1 2023-05-31 20:09:09.000000 educelab-cmdparse-0.1.0/src/educelab_cmdparse.egg-info/dependency_links.txt
--rw-r--r--   0 seth       (501) staff       (20)       32 2023-05-31 20:09:09.000000 educelab-cmdparse-0.1.0/src/educelab_cmdparse.egg-info/requires.txt
--rw-r--r--   0 seth       (501) staff       (20)        9 2023-05-31 20:09:09.000000 educelab-cmdparse-0.1.0/src/educelab_cmdparse.egg-info/top_level.txt
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-06-01 17:25:18.808443 educelab-cmdparse-0.2.0/
+-rw-r--r--   0 seth       (501) staff       (20)    34450 2023-05-31 19:36:53.000000 educelab-cmdparse-0.2.0/LICENSE
+-rw-r--r--   0 seth       (501) staff       (20)     1046 2023-06-01 17:25:18.808497 educelab-cmdparse-0.2.0/PKG-INFO
+-rw-r--r--   0 seth       (501) staff       (20)      318 2023-05-31 20:06:38.000000 educelab-cmdparse-0.2.0/README.md
+-rw-r--r--   0 seth       (501) staff       (20)      103 2023-05-31 20:06:38.000000 educelab-cmdparse-0.2.0/pyproject.toml
+-rw-r--r--   0 seth       (501) staff       (20)        0 2023-05-31 20:06:38.000000 educelab-cmdparse-0.2.0/requirements.txt
+-rw-r--r--   0 seth       (501) staff       (20)      942 2023-06-01 17:25:18.808729 educelab-cmdparse-0.2.0/setup.cfg
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-06-01 17:25:18.806717 educelab-cmdparse-0.2.0/src/
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-06-01 17:25:18.806651 educelab-cmdparse-0.2.0/src/educelab/
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-06-01 17:25:18.807762 educelab-cmdparse-0.2.0/src/educelab/cmdparse/
+-rw-r--r--   0 seth       (501) staff       (20)       50 2023-06-01 17:24:53.000000 educelab-cmdparse-0.2.0/src/educelab/cmdparse/__init__.py
+-rw-r--r--   0 seth       (501) staff       (20)     1760 2023-06-01 17:24:53.000000 educelab-cmdparse-0.2.0/src/educelab/cmdparse/cmdparse.py
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-06-01 17:25:18.808323 educelab-cmdparse-0.2.0/src/educelab_cmdparse.egg-info/
+-rw-r--r--   0 seth       (501) staff       (20)     1046 2023-06-01 17:25:18.000000 educelab-cmdparse-0.2.0/src/educelab_cmdparse.egg-info/PKG-INFO
+-rw-r--r--   0 seth       (501) staff       (20)      351 2023-06-01 17:25:18.000000 educelab-cmdparse-0.2.0/src/educelab_cmdparse.egg-info/SOURCES.txt
+-rw-r--r--   0 seth       (501) staff       (20)        1 2023-06-01 17:25:18.000000 educelab-cmdparse-0.2.0/src/educelab_cmdparse.egg-info/dependency_links.txt
+-rw-r--r--   0 seth       (501) staff       (20)       32 2023-06-01 17:25:18.000000 educelab-cmdparse-0.2.0/src/educelab_cmdparse.egg-info/requires.txt
+-rw-r--r--   0 seth       (501) staff       (20)        9 2023-06-01 17:25:18.000000 educelab-cmdparse-0.2.0/src/educelab_cmdparse.egg-info/top_level.txt
```

### Comparing `educelab-cmdparse-0.1.0/LICENSE` & `educelab-cmdparse-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `educelab-cmdparse-0.1.0/PKG-INFO` & `educelab-cmdparse-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: educelab-cmdparse
-Version: 0.1.0
-Summary: EduceLab image processing module
+Version: 0.2.0
+Summary: Python module for parsing arbitrary pipeline commands
 Home-page: https://gitlab.com/educelab/educelab-cmdparse
 Download-URL: https://gitlab.com/educelab/educelab-cmdparse
 Author: Seth Parker
 Author-email: c.seth.parker@uky.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `educelab-cmdparse-0.1.0/setup.cfg` & `educelab-cmdparse-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = educelab-cmdparse
-version = 0.1.0
+version = 0.2.0
 author = Seth Parker
 author_email = c.seth.parker@uky.edu
-description = EduceLab image processing module
+description = Python module for parsing arbitrary pipeline commands
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/educelab/educelab-cmdparse
 download_url = https://gitlab.com/educelab/educelab-cmdparse
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
```

### Comparing `educelab-cmdparse-0.1.0/src/educelab/cmdparse/cmdparse.py` & `educelab-cmdparse-0.2.0/src/educelab/cmdparse/cmdparse.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 from typing import List
 
 
 def parse(cmd_list: List[str], namespace):
     commands = []
     for cmd_str in cmd_list:
         key, sep, val = cmd_str.lstrip('-').partition("=")
+        attr_key = key.replace('-', '_')
         try:
-            kwargs = getattr(namespace, key)(sep, val)
+            kwargs = getattr(namespace, attr_key)(sep, val)
         except AttributeError as e:
             raise ValueError(f'No parser for command: \'{cmd_str}\'') from e
         commands.append((key, kwargs))
     return commands
 
 
 def parse_parameter_list(param_str, keys: List[str], types, sep=',',
                          num_required=None, mode='*'):
     if num_required is None and mode == '+':
         raise ValueError(
-            'Specified nargs_mode \'+\' but nargs_required not provided')
+            'Specified nargs_mode \'+\' but num_required not provided')
 
     if num_required is not None and num_required > len(keys):
         raise ValueError(
-            'nargs_required is larger than number of parseable parameters')
+            'num_required is larger than number of parseable parameters')
 
     # container for parsed params
     params = {}
     if len(param_str) == 0:
         if mode == '+':
             raise ValueError(
                 f'Too few arguments: expected {num_required}, got 0')
```

### Comparing `educelab-cmdparse-0.1.0/src/educelab_cmdparse.egg-info/PKG-INFO` & `educelab-cmdparse-0.2.0/src/educelab_cmdparse.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: educelab-cmdparse
-Version: 0.1.0
-Summary: EduceLab image processing module
+Version: 0.2.0
+Summary: Python module for parsing arbitrary pipeline commands
 Home-page: https://gitlab.com/educelab/educelab-cmdparse
 Download-URL: https://gitlab.com/educelab/educelab-cmdparse
 Author: Seth Parker
 Author-email: c.seth.parker@uky.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

