# Comparing `tmp/config_yml-0.3.0.tar.gz` & `tmp/config_yml-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_yml-0.3.0.tar", last modified: Wed May 17 12:35:03 2023, max compression
+gzip compressed data, was "config_yml-0.3.1.tar", last modified: Thu Jun  1 11:58:26 2023, max compression
```

## Comparing `config_yml-0.3.0.tar` & `config_yml-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:35:03.539859 config_yml-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-17 12:35:03.539859 config_yml-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-17 12:34:53.000000 config_yml-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:35:03.535859 config_yml-0.3.0/config_yml/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 12:34:53.000000 config_yml-0.3.0/config_yml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-17 12:34:53.000000 config_yml-0.3.0/config_yml/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:35:03.539859 config_yml-0.3.0/config_yml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-17 12:35:03.000000 config_yml-0.3.0/config_yml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-17 12:35:03.000000 config_yml-0.3.0/config_yml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:35:03.000000 config_yml-0.3.0/config_yml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 12:35:03.000000 config_yml-0.3.0/config_yml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 12:35:03.000000 config_yml-0.3.0/config_yml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:35:03.539859 config_yml-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-17 12:34:53.000000 config_yml-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:35:03.539859 config_yml-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:34:53.000000 config_yml-0.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:35:03.539859 config_yml-0.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:34:53.000000 config_yml-0.3.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 12:34:53.000000 config_yml-0.3.0/tests/data/config_existing.yml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 12:34:53.000000 config_yml-0.3.0/tests/data/config_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-05-17 12:34:53.000000 config_yml-0.3.0/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:58:26.911657 config_yml-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-01 11:58:26.911657 config_yml-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-01 11:58:10.000000 config_yml-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:58:26.911657 config_yml-0.3.1/config_yml/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-01 11:58:10.000000 config_yml-0.3.1/config_yml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-06-01 11:58:10.000000 config_yml-0.3.1/config_yml/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:58:26.911657 config_yml-0.3.1/config_yml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-01 11:58:26.000000 config_yml-0.3.1/config_yml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-01 11:58:26.000000 config_yml-0.3.1/config_yml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:58:26.000000 config_yml-0.3.1/config_yml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 11:58:26.000000 config_yml-0.3.1/config_yml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 11:58:26.000000 config_yml-0.3.1/config_yml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:58:26.911657 config_yml-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-01 11:58:10.000000 config_yml-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:58:26.911657 config_yml-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 11:58:10.000000 config_yml-0.3.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:58:26.911657 config_yml-0.3.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 11:58:10.000000 config_yml-0.3.1/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 11:58:10.000000 config_yml-0.3.1/tests/data/config_existing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 11:58:10.000000 config_yml-0.3.1/tests/data/config_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-06-01 11:58:10.000000 config_yml-0.3.1/tests/test_config.py
```

### Comparing `config_yml-0.3.0/PKG-INFO` & `config_yml-0.3.1/config_yml.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: config_yml
-Version: 0.3.0
+Name: config-yml
+Version: 0.3.1
 Summary: Utility modules for Class management
 Home-page: https://github.com/Phornee/config_yml
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,10 +16,11 @@
 # Config management class
 Configuration management package
 - Yaml based
 - Can use a config template embeded in your application distribution, and a local config (in /home/var/{application})
   customized for your particular installation (that could be edited manually, or by your ansible recipe).
 - Local config will be merged with the template in your application overwritting its values, allowing you to upgrade 
   and distribute your application adding new fields with default values seamlessly.
+- When merging two lists, if the items inside are dicts it will identify them as equal if the field 'name' matches.
 - Provides functionality not only to read the configuration, but also to modify it in runtime
```

### Comparing `config_yml-0.3.0/README.md` & `config_yml-0.3.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Config management class
 Configuration management package
 - Yaml based
 - Can use a config template embeded in your application distribution, and a local config (in /home/var/{application})
   customized for your particular installation (that could be edited manually, or by your ansible recipe).
 - Local config will be merged with the template in your application overwritting its values, allowing you to upgrade 
   and distribute your application adding new fields with default values seamlessly.
+- When merging two lists, if the items inside are dicts it will identify them as equal if the field 'name' matches.
 - Provides functionality not only to read the configuration, but also to modify it in runtime
```

### Comparing `config_yml-0.3.0/config_yml/config.py` & `config_yml-0.3.1/config_yml/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -147,21 +147,37 @@
                 if key not in dest_config:
                     if isinstance(value, dict):
                         dest_config[key] = {}
                     elif isinstance(value, list):
                         dest_config[key] = []
                 if type(value) in [int, str, bool, float, tuple]:
                     dest_config[key] = value
-                Config._merge_config(source_config[key], dest_config[key])
+                else:
+                    Config._merge_config(source_config[key], dest_config[key])
         elif isinstance(dest_config, list):
             if not isinstance(source_config, list):
                 raise TypeError()
-            for elem in source_config:
-                if elem not in dest_config:
-                    dest_config.append(elem)
+            for src_elem in source_config:
+                if not isinstance(src_elem, dict):
+                    if src_elem not in dest_config:
+                        dest_config.append(src_elem)
+                else:
+                    if 'name' in src_elem:
+                        found_dest_elem = None
+                        for dest_elem in dest_config:
+                            dest_elem_name = dest_elem.get('name', None)
+                            if dest_elem_name == src_elem['name']:
+                                found_dest_elem = dest_elem
+                                break
+                        if found_dest_elem:
+                            Config._merge_config(src_elem, found_dest_elem)
+                        else:
+                            dest_config.append(src_elem)
+                    else:
+                        dest_config.append(src_elem)
         else:
             dest_config = source_config
 
     def update(self, config_update):
         """Update the config with new data
         Args:
             config_update (dict): Values to modify
```

### Comparing `config_yml-0.3.0/setup.py` & `config_yml-0.3.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="config_yml",
-    version="0.3.0",
+    version="0.3.1",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Utility modules for Class management",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/config_yml",
     packages=setuptools.find_packages(),
```

### Comparing `config_yml-0.3.0/tests/test_config.py` & `config_yml-0.3.1/tests/test_config.py`

 * *Files identical despite different names*

