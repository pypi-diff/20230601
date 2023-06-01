# Comparing `tmp/resource-schema-guard-rail-0.0.5.tar.gz` & `tmp/resource-schema-guard-rail-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resource-schema-guard-rail-0.0.5.tar", last modified: Wed May 31 20:23:04 2023, max compression
+gzip compressed data, was "resource-schema-guard-rail-0.0.6.tar", last modified: Thu Jun  1 21:05:53 2023, max compression
```

## Comparing `resource-schema-guard-rail-0.0.5.tar` & `resource-schema-guard-rail-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,52 @@
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-05-31 20:23:04.559340 resource-schema-guard-rail-0.0.5/
--rw-r--r--   0 sgathili   (504) staff       (20)    10142 2023-05-31 20:20:49.000000 resource-schema-guard-rail-0.0.5/LICENSE
--rw-r--r--   0 sgathili   (504) staff       (20)     4023 2023-05-31 20:23:04.559415 resource-schema-guard-rail-0.0.5/PKG-INFO
--rw-r--r--   0 sgathili   (504) staff       (20)     3349 2023-05-31 20:20:49.000000 resource-schema-guard-rail-0.0.5/README.md
--rw-r--r--   0 sgathili   (504) staff       (20)      593 2023-05-31 20:23:04.559740 resource-schema-guard-rail-0.0.5/setup.cfg
--rw-r--r--   0 sgathili   (504) staff       (20)     1937 2023-05-31 20:20:49.000000 resource-schema-guard-rail-0.0.5/setup.py
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-05-31 20:23:04.557440 resource-schema-guard-rail-0.0.5/src/
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-05-31 20:23:04.558951 resource-schema-guard-rail-0.0.5/src/resource_schema_guard_rail.egg-info/
--rw-r--r--   0 sgathili   (504) staff       (20)     4023 2023-05-31 20:23:04.000000 resource-schema-guard-rail-0.0.5/src/resource_schema_guard_rail.egg-info/PKG-INFO
--rw-r--r--   0 sgathili   (504) staff       (20)      394 2023-05-31 20:23:04.000000 resource-schema-guard-rail-0.0.5/src/resource_schema_guard_rail.egg-info/SOURCES.txt
--rw-r--r--   0 sgathili   (504) staff       (20)        1 2023-05-31 20:23:04.000000 resource-schema-guard-rail-0.0.5/src/resource_schema_guard_rail.egg-info/dependency_links.txt
--rw-r--r--   0 sgathili   (504) staff       (20)       67 2023-05-31 20:23:04.000000 resource-schema-guard-rail-0.0.5/src/resource_schema_guard_rail.egg-info/entry_points.txt
--rw-r--r--   0 sgathili   (504) staff       (20)      258 2023-05-31 20:23:04.000000 resource-schema-guard-rail-0.0.5/src/resource_schema_guard_rail.egg-info/requires.txt
--rw-r--r--   0 sgathili   (504) staff       (20)        5 2023-05-31 20:23:04.000000 resource-schema-guard-rail-0.0.5/src/resource_schema_guard_rail.egg-info/top_level.txt
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-05-31 20:23:04.557497 resource-schema-guard-rail-0.0.5/src/rpdk/
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-05-31 20:23:04.559191 resource-schema-guard-rail-0.0.5/src/rpdk/guard_rail/
--rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-05-31 20:20:49.000000 resource-schema-guard-rail-0.0.5/src/rpdk/guard_rail/__init__.py
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.640442 resource-schema-guard-rail-0.0.6/
+-rw-r--r--   0 sgathili   (504) staff       (20)    10142 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/LICENSE
+-rw-r--r--   0 sgathili   (504) staff       (20)       63 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/MANIFEST.in
+-rw-r--r--   0 sgathili   (504) staff       (20)     4023 2023-06-01 21:05:53.640549 resource-schema-guard-rail-0.0.6/PKG-INFO
+-rw-r--r--   0 sgathili   (504) staff       (20)     3349 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/README.md
+-rw-r--r--   0 sgathili   (504) staff       (20)      593 2023-06-01 21:05:53.641114 resource-schema-guard-rail-0.0.6/setup.cfg
+-rw-r--r--   0 sgathili   (504) staff       (20)     2010 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/setup.py
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.634453 resource-schema-guard-rail-0.0.6/src/
+-rw-r--r--   0 sgathili   (504) staff       (20)     2538 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/cli.py
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.635517 resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/
+-rw-r--r--   0 sgathili   (504) staff       (20)     4023 2023-06-01 21:05:53.000000 resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/PKG-INFO
+-rw-r--r--   0 sgathili   (504) staff       (20)     1661 2023-06-01 21:05:53.000000 resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/SOURCES.txt
+-rw-r--r--   0 sgathili   (504) staff       (20)        1 2023-06-01 21:05:53.000000 resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/dependency_links.txt
+-rw-r--r--   0 sgathili   (504) staff       (20)       67 2023-06-01 21:05:53.000000 resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/entry_points.txt
+-rw-r--r--   0 sgathili   (504) staff       (20)      258 2023-06-01 21:05:53.000000 resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/requires.txt
+-rw-r--r--   0 sgathili   (504) staff       (20)        9 2023-06-01 21:05:53.000000 resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/top_level.txt
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.635673 resource-schema-guard-rail-0.0.6/src/rpdk/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/__init__.py
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.635813 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/__init__.py
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.636465 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/__init__.py
+-rw-r--r--   0 sgathili   (504) staff       (20)     3870 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/data_types.py
+-rw-r--r--   0 sgathili   (504) staff       (20)     6239 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/runner.py
+-rw-r--r--   0 sgathili   (504) staff       (20)    11087 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/stateful.py
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.636669 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/templates/
+-rw-r--r--   0 sgathili   (504) staff       (20)      590 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/templates/guard-result-pojo.output
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.636858 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/__init__.py
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.637138 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/combiners/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/combiners/__init__.py
+-rw-r--r--   0 sgathili   (504) staff       (20)     1579 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/combiners/schema-linter-combiner-rules.guard
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.637751 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/core/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/core/__init__.py
+-rw-r--r--   0 sgathili   (504) staff       (20)      555 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/core/schema-linter-core-arn-rules.guard
+-rw-r--r--   0 sgathili   (504) staff       (20)     2855 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/core/schema-linter-core-rules.guard
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.638190 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/permissions/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/permissions/__init__.py
+-rw-r--r--   0 sgathili   (504) staff       (20)     2699 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/permissions/schema-linter-core-permission-rules.guard
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.638589 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/stateful/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/stateful/__init__.py
+-rw-r--r--   0 sgathili   (504) staff       (20)    12380 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/stateful/schema-stateful-cfn-enforced-checks.guard
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.638942 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/tags/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/tags/__init__.py
+-rw-r--r--   0 sgathili   (504) staff       (20)     2711 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/tags/schema-linter-core-tagging-rules.guard
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.640147 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/__init__.py
+-rw-r--r--   0 sgathili   (504) staff       (20)     4997 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/arg_handler.py
+-rw-r--r--   0 sgathili   (504) staff       (20)      858 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/common.py
+-rw-r--r--   0 sgathili   (504) staff       (20)      928 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/logger.py
+-rw-r--r--   0 sgathili   (504) staff       (20)      893 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/miscellaneous.py
+-rw-r--r--   0 sgathili   (504) staff       (20)     2510 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/schema_utils.py
```

### Comparing `resource-schema-guard-rail-0.0.5/LICENSE` & `resource-schema-guard-rail-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.5/PKG-INFO` & `resource-schema-guard-rail-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resource-schema-guard-rail
-Version: 0.0.5
+Version: 0.0.6
 Summary: Schema Guard Rail
 Home-page: UNKNOWN
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `resource-schema-guard-rail-0.0.5/README.md` & `resource-schema-guard-rail-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.5/setup.cfg` & `resource-schema-guard-rail-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.5/setup.py` & `resource-schema-guard-rail-0.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,23 +32,25 @@
         else:
             requirements.append(line)
     return requirements
 
 
 setuptools.setup(
     name="resource-schema-guard-rail",
-    version="0.0.5",
+    version="0.0.6",
     description="Schema Guard Rail",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Amazon Web Services",
     author_email="aws-cloudformation-developers@amazon.com",
-    packages=["rpdk.guard_rail"],
+    packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
+    py_modules=["cli"],
     install_requires=read_requirements("requirements_dev.txt"),
+    include_package_data=True,
     python_requires=">=3.7",
     entry_points={
         "console_scripts": [
             "guard-rail-cli = cli:main",
             "guard-rail = cli:main",
         ]
     },
```

### Comparing `resource-schema-guard-rail-0.0.5/src/resource_schema_guard_rail.egg-info/PKG-INFO` & `resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resource-schema-guard-rail
-Version: 0.0.5
+Version: 0.0.6
 Summary: Schema Guard Rail
 Home-page: UNKNOWN
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

