# Comparing `tmp/hoppr_cop-1.1.6.tar.gz` & `tmp/hoppr_cop-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_cop-1.1.6.tar", max compression
+gzip compressed data, was "hoppr_cop-1.1.7.tar", max compression
```

## Comparing `hoppr_cop-1.1.6.tar` & `hoppr_cop-1.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1084 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/LICENSE.md
--rw-r--r--   0        0        0       55 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/combined/__init__.py
--rw-r--r--   0        0        0     3336 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/combined/cli.py
--rw-r--r--   0        0        0     4488 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/combined/combined_scanner.py
--rw-r--r--   0        0        0        0 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/gemnasium/__init__.py
--rw-r--r--   0        0        0     9223 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/gemnasium/gemnasium_scanner.py
--rw-r--r--   0        0        0     1134 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/gemnasium/models.py
--rwxr-xr-x   0        0        0      113 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/gemnasium/semver
--rw-r--r--   0        0        0        0 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/grype/__init__.py
--rw-r--r--   0        0        0     5953 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/grype/grype_scanner.py
--rw-r--r--   0        0        0     5289 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/grype/models.py
--rw-r--r--   0        0        0     9731 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/hoppr_plugin/hopprcop_plugin.py
--rw-r--r--   0        0        0      478 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/README.md
--rw-r--r--   0        0        0        0 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/__init__.py
--rw-r--r--   0        0        0      832 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/api/__init__.py
--rw-r--r--   0        0        0     1029 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/api/exception.py
--rw-r--r--   0        0        0     9487 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/api/model.py
--rw-r--r--   0        0        0    11624 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/api/ossindex.py
--rw-r--r--   0        0        0      153 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/api/py.typed
--rw-r--r--   0        0        0     3147 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/api/serializer.py
--rw-r--r--   0        0        0     4924 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/oss_index_scanner.py
--rw-r--r--   0        0        0        0 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/trivy/__init__.py
--rw-r--r--   0        0        0     5558 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/trivy/trivy_scanner.py
--rw-r--r--   0        0        0      853 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 hoppr_cop-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/LICENSE.md
+-rw-r--r--   0        0        0       55 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/combined/__init__.py
+-rw-r--r--   0        0        0     3336 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/combined/cli.py
+-rw-r--r--   0        0        0     4488 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/combined/combined_scanner.py
+-rw-r--r--   0        0        0        0 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/gemnasium/__init__.py
+-rw-r--r--   0        0        0     9223 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/gemnasium/gemnasium_scanner.py
+-rw-r--r--   0        0        0     1134 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/gemnasium/models.py
+-rwxr-xr-x   0        0        0      113 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/gemnasium/semver
+-rw-r--r--   0        0        0        0 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/grype/__init__.py
+-rw-r--r--   0        0        0     5953 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/grype/grype_scanner.py
+-rw-r--r--   0        0        0     5289 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/grype/models.py
+-rw-r--r--   0        0        0     9731 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/hoppr_plugin/hopprcop_plugin.py
+-rw-r--r--   0        0        0      478 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/README.md
+-rw-r--r--   0        0        0        0 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/api/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/api/exception.py
+-rw-r--r--   0        0        0     9487 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/api/model.py
+-rw-r--r--   0        0        0    11624 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/api/ossindex.py
+-rw-r--r--   0        0        0      153 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/api/py.typed
+-rw-r--r--   0        0        0     3147 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/api/serializer.py
+-rw-r--r--   0        0        0     4924 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/oss_index_scanner.py
+-rw-r--r--   0        0        0        0 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/trivy/__init__.py
+-rw-r--r--   0        0        0     5591 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/trivy/trivy_scanner.py
+-rw-r--r--   0        0        0      853 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 hoppr_cop-1.1.7/PKG-INFO
```

### Comparing `hoppr_cop-1.1.6/LICENSE.md` & `hoppr_cop-1.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.6/hopprcop/combined/cli.py` & `hoppr_cop-1.1.7/hopprcop/combined/cli.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.6/hopprcop/combined/combined_scanner.py` & `hoppr_cop-1.1.7/hopprcop/combined/combined_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.6/hopprcop/gemnasium/gemnasium_scanner.py` & `hoppr_cop-1.1.7/hopprcop/gemnasium/gemnasium_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.6/hopprcop/gemnasium/models.py` & `hoppr_cop-1.1.7/hopprcop/gemnasium/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.6/hopprcop/grype/grype_scanner.py` & `hoppr_cop-1.1.7/hopprcop/grype/grype_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.6/hopprcop/grype/models.py` & `hoppr_cop-1.1.7/hopprcop/grype/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.6/hopprcop/hoppr_plugin/hopprcop_plugin.py` & `hoppr_cop-1.1.7/hopprcop/hoppr_plugin/hopprcop_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.6/hopprcop/ossindex/api/__init__.py` & `hoppr_cop-1.1.7/hopprcop/ossindex/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.6/hopprcop/ossindex/api/exception.py` & `hoppr_cop-1.1.7/hopprcop/ossindex/api/exception.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.6/hopprcop/ossindex/api/model.py` & `hoppr_cop-1.1.7/hopprcop/ossindex/api/model.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.6/hopprcop/ossindex/api/ossindex.py` & `hoppr_cop-1.1.7/hopprcop/ossindex/api/ossindex.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.6/hopprcop/ossindex/api/serializer.py` & `hoppr_cop-1.1.7/hopprcop/ossindex/api/serializer.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.6/hopprcop/ossindex/oss_index_scanner.py` & `hoppr_cop-1.1.7/hopprcop/ossindex/oss_index_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.6/hopprcop/trivy/trivy_scanner.py` & `hoppr_cop-1.1.7/hopprcop/trivy/trivy_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         purls = list(filter(lambda x: x.type in self.supported_types, purls))
         if len(purls) > 0:
             bom = build_bom_dict_from_purls(purls)
             self.__add_operating_system_component(bom)
 
             with tempfile.NamedTemporaryFile(mode="w") as bom_file:
                 bom_file.write(json.dumps(bom))
+                bom_file.flush()
                 args = ["trivy", "sbom", "--format", "cyclonedx", str(bom_file.name)]
                 cache = os.getenv("CACHE_DIR")
                 if cache is not None:
                     args = args + ["--cache-dir", cache]
                 with Popen(
                     args,
                     stdout=PIPE,
```

### Comparing `hoppr_cop-1.1.6/pyproject.toml` & `hoppr_cop-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr-cop"
-version = "1.1.6"
+version = "1.1.7"
 description = ""
 authors = ["kganger <keith.e.ganger@lmco.com>"]
 license = "MIT"
 
 [[tool.poetry.packages]]
 include = "hopprcop"
```

### Comparing `hoppr_cop-1.1.6/PKG-INFO` & `hoppr_cop-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr-cop
-Version: 1.1.6
+Version: 1.1.7
 Summary: 
 License: MIT
 Author: kganger
 Author-email: keith.e.ganger@lmco.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

