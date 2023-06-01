# Comparing `tmp/bmsdna_lakeapi-0.5.1.tar.gz` & `tmp/bmsdna_lakeapi-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.5.1.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.5.2.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.5.1.tar` & `bmsdna_lakeapi-0.5.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1081 2023-05-31 08:32:18.764371 bmsdna_lakeapi-0.5.1/LICENSE
--rw-r--r--   0        0        0     8929 2023-05-31 08:32:18.764371 bmsdna_lakeapi-0.5.1/README.md
--rw-r--r--   0        0        0      337 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      670 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     6355 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     9131 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6039 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11357 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    11904 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    18925 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6754 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1177 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6512 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4253 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3109 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2478 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-05-31 08:32:18.776371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-05-31 08:32:18.780371 bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1998 2023-05-31 08:32:18.780371 bmsdna_lakeapi-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-01 08:34:42.665014 bmsdna_lakeapi-0.5.2/LICENSE
+-rw-r--r--   0        0        0     8929 2023-06-01 08:34:42.665014 bmsdna_lakeapi-0.5.2/README.md
+-rw-r--r--   0        0        0      337 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1185 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      670 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     6355 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     9131 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6039 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11357 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    11904 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    18925 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6754 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1452 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6512 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4253 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3109 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2478 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1998 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.5.2/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.5.1/LICENSE` & `bmsdna_lakeapi-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/README.md` & `bmsdna_lakeapi-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/partition_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,20 +12,26 @@
 
 def _with_implicit_parameters(paramslist: "List[Param]", file_type: str, basic_config: "BasicConfig", uri: str):
     if file_type == "delta":
         delta_uri = os.path.join(
             basic_config.data_path,
             uri,
         )
-        from deltalake import DeltaTable
+        if not os.path.exists(os.path.join(delta_uri, "_delta_log")):
+            return paramslist
+        from deltalake import DeltaTable, PyDeltaTableError
 
-        part_cols = DeltaTable(delta_uri).metadata().partition_columns
-        if part_cols and len(part_cols) > 0:
-            all_names = [(p.colname or p.name).lower() for p in paramslist]
-            new_params = list(paramslist)
-            for pc in part_cols:
-                if pc.lower() not in all_names and not should_hide_colname(pc):
-                    from bmsdna.lakeapi.core.types import Param
+        try:
+            part_cols = DeltaTable(delta_uri).metadata().partition_columns
+            if part_cols and len(part_cols) > 0:
+                all_names = [(p.colname or p.name).lower() for p in paramslist]
+                new_params = list(paramslist)
+                for pc in part_cols:
+                    if pc.lower() not in all_names and not should_hide_colname(pc):
+                        from bmsdna.lakeapi.core.types import Param
+
+                        new_params.append(Param(pc, operators=["="], colname=pc))
+                return new_params
+        except PyDeltaTableError as err:
+            return paramslist  # this is not critical here
 
-                    new_params.append(Param(pc, operators=["="], colname=pc))
-            return new_params
     return paramslist
```

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.1/pyproject.toml` & `bmsdna_lakeapi-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.5.1/PKG-INFO` & `bmsdna_lakeapi-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

