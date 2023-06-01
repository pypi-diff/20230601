# Comparing `tmp/yetl-framework-1.3.9.tar.gz` & `tmp/yetl-framework-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.3.9.tar", last modified: Sun May 28 18:37:11 2023, max compression
+gzip compressed data, was "yetl-framework-1.4.1.tar", last modified: Thu Jun  1 16:10:51 2023, max compression
```

## Comparing `yetl-framework-1.3.9.tar` & `yetl-framework-1.4.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-28 18:37:11.350350 yetl-framework-1.3.9/
--rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-05-28 18:37:11.350350 yetl-framework-1.3.9/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-28 18:37:11.350350 yetl-framework-1.3.9/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-28 18:37:11.346350 yetl-framework-1.3.9/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      895 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-28 18:37:11.346350 yetl-framework-1.3.9/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-28 18:37:11.346350 yetl-framework-1.3.9/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3345 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8759 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-28 18:37:11.350350 yetl-framework-1.3.9/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3990 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6533 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3713 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-28 18:37:11.350350 yetl-framework-1.3.9/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-28 18:36:18.000000 yetl-framework-1.3.9/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-28 18:37:11.350350 yetl-framework-1.3.9/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-05-28 18:37:11.000000 yetl-framework-1.3.9/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      902 2023-05-28 18:37:11.000000 yetl-framework-1.3.9/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-28 18:37:11.000000 yetl-framework-1.3.9/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-28 18:37:11.000000 yetl-framework-1.3.9/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       29 2023-05-28 18:37:11.000000 yetl-framework-1.3.9/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-28 18:37:11.000000 yetl-framework-1.3.9/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 16:10:51.810496 yetl-framework-1.4.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-01 16:10:51.806496 yetl-framework-1.4.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-01 16:10:51.810496 yetl-framework-1.4.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 16:10:51.806496 yetl-framework-1.4.1/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 16:10:51.806496 yetl-framework-1.4.1/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 16:10:51.806496 yetl-framework-1.4.1/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3023 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8764 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 16:10:51.806496 yetl-framework-1.4.1/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3790 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4049 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 16:10:51.806496 yetl-framework-1.4.1/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-01 16:10:01.000000 yetl-framework-1.4.1/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-01 16:10:51.806496 yetl-framework-1.4.1/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-01 16:10:51.000000 yetl-framework-1.4.1/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      902 2023-06-01 16:10:51.000000 yetl-framework-1.4.1/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-01 16:10:51.000000 yetl-framework-1.4.1/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-01 16:10:51.000000 yetl-framework-1.4.1/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       29 2023-06-01 16:10:51.000000 yetl-framework-1.4.1/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-06-01 16:10:51.000000 yetl-framework-1.4.1/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.3.9/PKG-INFO` & `yetl-framework-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.3.9
+Version: 1.4.1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.3.9/README.md` & `yetl-framework-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.9/setup.py` & `yetl-framework-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.3.9",
+    version="1.4.1",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.3.9/yetl/cli/_init.py` & `yetl-framework-1.4.1/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.9/yetl/config/_config.py` & `yetl-framework-1.4.1/yetl/config/_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         return tables
 
     def get_table_mapping(
         self,
         stage: StageType,
         table: str = _INDEX_WILDCARD,
         database: str = _INDEX_WILDCARD,
-        create_table: bool = True
+        create_table: bool = True,
     ):
         table_mapping = self.tables.get_table_mapping(
             stage=stage, table=table, database=database, create_table=create_table
         )
 
         return table_mapping
 
@@ -77,15 +77,10 @@
         destination: Table,
         checkpoint_name: str = None,
     ):
         if not checkpoint_name:
             checkpoint_name = f"{source.database}.{source.table}-{destination.database}.{destination.table}"
 
         source.checkpoint = checkpoint_name
-        source._render()
-        if destination.checkpoint_location is not None:
-            destination.checkpoint = checkpoint_name
-            destination.options["checkpointLocation"] = destination.checkpoint_location
-            destination._render()
-            self._logger.info(f"checkpointLocation: {destination.checkpoint_location}")
-        else:
-            self._logger.info("No checkpoint configuration found")
+        source.render()
+        destination.checkpoint = checkpoint_name
+        destination.render()
```

### Comparing `yetl-framework-1.3.9/yetl/config/_decorators.py` & `yetl-framework-1.4.1/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.9/yetl/config/_logging_config.py` & `yetl-framework-1.4.1/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.9/yetl/config/_project.py` & `yetl-framework-1.4.1/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.9/yetl/config/_spark_context.py` & `yetl-framework-1.4.1/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.9/yetl/config/_tables.py` & `yetl-framework-1.4.1/yetl/config/_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,23 +131,23 @@
 
     def create_table(
         self,
         stage: Union[StageType, str] = _INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
         table=_INDEX_WILDCARD,
         first_match: bool = True,
-        **kwargs
+        **kwargs,
     ):
         return self.lookup_table(
             stage=stage,
             database=database,
             table=table,
             first_match=first_match,
             create_table=True,
-            **kwargs
+            **kwargs,
         )
 
     def lookup_table(
         self,
         stage: Union[StageType, str] = _INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
         table=_INDEX_WILDCARD,
@@ -204,35 +204,35 @@
             return tables
 
     def get_table_mapping(
         self,
         stage: StageType,
         table=_INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
-        create_table: bool = True
+        create_table: bool = True,
     ):
         destination = self.lookup_table(
             stage=stage,
             database=database,
             table=table,
             first_match=True,
-            create_table=create_table
+            create_table=create_table,
         )
         source = {}
 
         tables = []
         try:
             for index in destination.depends_on:
                 do_stage, do_database, do_table = Tables.parse_index(index)
                 tables = tables + self.lookup_table(
                     stage=do_stage,
                     table=do_table,
                     database=do_database,
                     first_match=False,
-                    create_table=create_table
+                    create_table=create_table,
                 )
         except Exception as e:
             raise Exception(f"Error looking up dependencies for table {table}") from e
 
         for tbl in tables:
             source[tbl.table] = tbl
```

### Comparing `yetl-framework-1.3.9/yetl/config/_timeslice.py` & `yetl-framework-1.4.1/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.9/yetl/config/_utils.py` & `yetl-framework-1.4.1/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.9/yetl/config/deltalake.py` & `yetl-framework-1.4.1/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.9/yetl/config/table/_deltalake.py` & `yetl-framework-1.4.1/yetl/config/table/_deltalake.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,22 +28,23 @@
 
     _logger: Any = PrivateAttr(default=None)
     _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
     _spark: DeltaLakeFn = PrivateAttr(default=None)
     depends_on: List[str] = Field(default=[])
     delta_properties: Dict[str, str] = Field(default=None)
     delta_constraints: Dict[str, str] = Field(default=None)
-    partition_by: List[str] = Field(default=None)
-    z_order_by: List[str] = Field(default=None)
+    partition_by: Union[List[str], str] = Field(default=None)
+    z_order_by: Union[List[str], str] = Field(default=None)
+    vacuum: int = Field(default=31)
     options: Union[dict, None] = Field(default=None)
     timeslice: Timeslice = Field(...)
     location: str = Field(default=None)
-    checkpoint_location: str = Field(default=None)
     stage: StageType = Field(...)
     managed: bool = Field(default=False)
+
     sql: str = Field(default=None)
 
     def _load_sql(self, path: str):
         path = abs_config_path(self.config_path, path)
         sql = load_text(path)
         return sql
 
@@ -63,34 +64,28 @@
             self.path = render_jinja(self.path, self._replacements)
             self.location = os.path.join(self.location, self.path)
             if not is_databricks():
                 self.location = f"{self.config_path}/../data{self.location}"
                 self.location = os.path.abspath(self.location)
             self._replacements[JinjaVariables.LOCATION] = self.location
 
-            if self.options:
-                for option, value in self.options.items():
-                    self.options[option] = render_jinja(value, self._replacements)
-
             if self.sql:
                 # render the path
                 self.sql = render_jinja(self.sql, self._replacements)
                 # load the file
                 self.sql = self._load_sql(self.sql)
                 # render the SQL
                 self.sql = render_jinja(self.sql, self._replacements)
 
-            self._rendered = True
+            if self.options:
+                for option, value in self.options.items():
+                    if isinstance(value, str):
+                        self.options[option] = render_jinja(value, self._replacements)
 
-        if self._rendered and self.options:
-            value = self.options.get("checkpointLocation")
-            if value:
-                self.options["checkpointLocation"] = render_jinja(
-                    value, self._replacements
-                )
+        self._rendered = True
 
     # TODO: Create or alter table
     def create_table(self):
         self._spark.create_database(self.database)
 
         if self.managed:
             self._spark.create_table(
```

### Comparing `yetl-framework-1.3.9/yetl/config/table/_factory.py` & `yetl-framework-1.4.1/yetl/config/table/_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,10 +28,10 @@
 
         return table_class(
             **config,
         )
 
 
 factory = TableFactory()
-factory.register_table_type(TableType.Read, Read)
-factory.register_table_type(TableType.DeltaLake, DeltaLake)
-factory.register_table_type(TableType.Write, Write)
+factory.register_table_type(TableType.read, Read)
+factory.register_table_type(TableType.delta_lake, DeltaLake)
+factory.register_table_type(TableType.write, Write)
```

### Comparing `yetl-framework-1.3.9/yetl/config/table/_read.py` & `yetl-framework-1.4.1/yetl/config/table/_read.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,31 +99,31 @@
                 path = self.spark_schema
                 path = render_jinja(self.spark_schema, self._replacements)
                 path = abs_config_path(self.config_path, path)
                 if os.path.exists(path):
                     self._load_schema(path)
                 else:
                     self.spark_schema = path
-                    self._logger.warning(f"Schema path doesn't exist, schema has not been loaded and remains to be path {path}.")
+                    self._logger.warning(
+                        f"Schema path doesn't exist, schema has not been loaded and remains to be path {path}."
+                    )
 
             corrupt_record_name = self.options.get(
                 self._OPTION_CORRUPT_RECORD_NAME, None
             )
             if isinstance(self.spark_schema, StructType) and corrupt_record_name:
                 if corrupt_record_name not in self.spark_schema.names:
                     self.spark_schema.add(field=corrupt_record_name, data_type="string")
 
-            self._rendered = True
+            if self.options:
+                for option, value in self.options.items():
+                    if isinstance(value, str):
+                        self.options[option] = render_jinja(value, self._replacements)
 
-        if self._rendered and self.options:
-            value = self.options.get("checkpointLocation")
-            if value:
-                self.options["checkpointLocation"] = render_jinja(
-                    value, self._replacements
-                )
+        self._rendered = True
 
     def _config_schema_hints(self):
         path = self.options.get(self._OPTION_CF_SCHEMA_HINTS, None)
         if path and "/" in path:
             self._load_schema(path)
 
             if self.options.get("header"):
```

### Comparing `yetl-framework-1.3.9/yetl/config/table/_table.py` & `yetl-framework-1.4.1/yetl/config/table/_table.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .._utils import JinjaVariables
 from typing import Any, Dict, Union, List
 from .._timeslice import Timeslice
 from .._stage_type import StageType
 from ._table_type import TableType
 from .._project import Project
 from enum import Enum
+from .._utils import render_jinja
 
 
 class ValidationThresholdType(Enum):
     exception = ("exception",)
     warning = "warning"
 
 
@@ -91,14 +92,22 @@
             JinjaVariables.TABLE: self.table,
             JinjaVariables.DATABASE: self.database,
             JinjaVariables.CONTAINER: self.container,
             JinjaVariables.CHECKPOINT: self.checkpoint,
             JinjaVariables.PROJECT: self.project.name,
         }
 
+    def render(self):
+        self._replacements[JinjaVariables.CHECKPOINT] = self.checkpoint
+
+        if self.options:
+            for option, value in self.options.items():
+                if isinstance(value, str):
+                    self.options[option] = render_jinja(value, self._replacements)
+
     def thresholds_select_sql(self, threshold_type: ValidationThresholdType):
         if threshold_type == ValidationThresholdType.exception:
             if self.exception_thresholds:
                 return self.exception_thresholds.select_sql()
             else:
                 return ValidationThreshold.default_select_sql()
```

### Comparing `yetl-framework-1.3.9/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.4.1/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.9/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.4.1/yetl_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.3.9
+Version: 1.4.1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.3.9/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.4.1/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

