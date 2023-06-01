# Comparing `tmp/sinker-0.1.0.tar.gz` & `tmp/sinker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinker-0.1.0.tar", max compression
+gzip compressed data, was "sinker-0.1.1.tar", max compression
```

## Comparing `sinker-0.1.0.tar` & `sinker-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    10847 2023-02-17 01:16:40.669539 sinker-0.1.0/LICENSE-APACHE
--rw-r--r--   0        0        0     1061 2023-02-17 01:16:41.003379 sinker-0.1.0/LICENSE-MIT
--rw-r--r--   0        0        0      568 2023-03-02 23:28:02.307526 sinker-0.1.0/README.md
--rw-r--r--   0        0        0      670 2023-03-02 21:32:15.445951 sinker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-17 01:16:41.011666 sinker-0.1.0/src/sinker/__init__.py
--rwxr-xr-x   0        0        0      126 2023-02-27 18:41:42.859822 sinker-0.1.0/src/sinker/__main__.py
--rw-r--r--   0        0        0     4112 2023-02-17 01:16:41.013411 sinker-0.1.0/src/sinker/bulk_action_generator.py
--rw-r--r--   0        0        0      674 2023-02-17 01:16:41.013609 sinker-0.1.0/src/sinker/es.py
--rw-r--r--   0        0        0     1203 2023-02-17 01:16:41.011545 sinker-0.1.0/src/sinker/query_templates.py
--rw-r--r--   0        0        0     5098 2023-02-17 01:16:41.011353 sinker-0.1.0/src/sinker/runner.py
--rw-r--r--   0        0        0     2779 2023-02-17 20:22:04.259803 sinker-0.1.0/src/sinker/settings.py
--rw-r--r--   0        0        0     5704 2023-02-17 01:16:41.014313 sinker-0.1.0/src/sinker/sinker.py
--rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 sinker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10847 2023-02-17 01:16:40.669539 sinker-0.1.1/LICENSE-APACHE
+-rw-r--r--   0        0        0     1067 2023-03-13 22:53:29.429831 sinker-0.1.1/LICENSE-MIT
+-rw-r--r--   0        0        0    11761 2023-03-13 22:51:39.412599 sinker-0.1.1/README.md
+-rw-r--r--   0        0        0      693 2023-06-01 18:08:55.070658 sinker-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-17 01:16:41.011666 sinker-0.1.1/src/sinker/__init__.py
+-rwxr-xr-x   0        0        0      126 2023-02-27 18:41:42.859822 sinker-0.1.1/src/sinker/__main__.py
+-rw-r--r--   0        0        0     4112 2023-03-03 18:15:41.612877 sinker-0.1.1/src/sinker/bulk_action_generator.py
+-rw-r--r--   0        0        0      674 2023-02-17 01:16:41.013609 sinker-0.1.1/src/sinker/es.py
+-rw-r--r--   0        0        0     1203 2023-02-17 01:16:41.011545 sinker-0.1.1/src/sinker/query_templates.py
+-rw-r--r--   0        0        0     5491 2023-06-01 05:14:38.877134 sinker-0.1.1/src/sinker/runner.py
+-rw-r--r--   0        0        0     2779 2023-02-17 20:22:04.259803 sinker-0.1.1/src/sinker/settings.py
+-rw-r--r--   0        0        0     5739 2023-06-01 18:00:19.949321 sinker-0.1.1/src/sinker/sinker.py
+-rw-r--r--   0        0        0      514 2023-06-01 18:05:17.736631 sinker-0.1.1/src/sinker/utils.py
+-rw-r--r--   0        0        0    12429 1970-01-01 00:00:00.000000 sinker-0.1.1/PKG-INFO
```

### Comparing `sinker-0.1.0/LICENSE-APACHE` & `sinker-0.1.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `sinker-0.1.0/LICENSE-MIT` & `sinker-0.1.1/LICENSE-MIT`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 Reth Contributors
+Copyright (c) 2023 Paradigm Operations LP.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sinker-0.1.0/pyproject.toml` & `sinker-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "sinker"
-version = "0.1.0"
+version = "0.1.1"
 description = "Synchronize Postgres to Elasticsearch"
 authors = ["Loren Siebert <loren@paradigm.xyz>"]
 license = "MIT/Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 sinker = "sinker.__main__:main"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
 elasticsearch = "^8.6.1"
 environs = "^9.5.0"
 psycopg = "^3.1.8"
+pytest-mock = "^3.10.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 black = "^23.1.0"
 mypy = "^1.0.0"
 psycopg-binary = "^3.1.8"
```

### Comparing `sinker-0.1.0/src/sinker/bulk_action_generator.py` & `sinker-0.1.1/src/sinker/bulk_action_generator.py`

 * *Files identical despite different names*

### Comparing `sinker-0.1.0/src/sinker/es.py` & `sinker-0.1.1/src/sinker/es.py`

 * *Files identical despite different names*

### Comparing `sinker-0.1.0/src/sinker/query_templates.py` & `sinker-0.1.1/src/sinker/query_templates.py`

 * *Files identical despite different names*

### Comparing `sinker-0.1.0/src/sinker/runner.py` & `sinker-0.1.1/src/sinker/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import concurrent
 import json
 import logging
 from concurrent.futures import ThreadPoolExecutor
 from time import sleep
 from typing import Any
 
 import psycopg
@@ -37,16 +38,20 @@
         psycopg.connect(autocommit=True).execute("; ".join(ddl_list))
         self.views_to_sinkers: dict[str, Sinker] = {
             view: Sinker(view, index) for (view, index) in views_to_indices.items()
         }
 
         # set up materialized views and Elasticsearch indices, and populate them with initial data
         with ThreadPoolExecutor(max_workers=len(self.views_to_sinkers)) as executor:
+            futures = []
             for sinker in self.views_to_sinkers.values():
-                executor.submit(sinker.setup)
+                futures.append(executor.submit(sinker.setup))
+            for future in concurrent.futures.as_completed(futures):
+                view: str = future.result()
+                logger.info(f"{view} sinker is set up")
 
         parent_tables_to_indices: dict[str, str] = {
             sinker.parent_table: sinker.index for sinker in self.views_to_sinkers.values()
         }
 
         # set up replication slot
         drop_slot: str = q.DROP_SLOT.format(SINKER_REPLICATION_SLOT)
@@ -80,19 +85,22 @@
         # occurred because the materialized view will already be up-to-date.
         # ---------------------------------------
         if not views:
             logger.debug("Nothing is something worth doing.")
             sleep(SINKER_POLL_INTERVAL)
             return
         with ThreadPoolExecutor(max_workers=len(views)) as executor:
+            futures = []
             for view_tuple in views:
                 view: str = view_tuple[0].split(SCHEMA_TABLE_DELIMITER)[1]
                 sinker: Sinker = self.views_to_sinkers[view]
-                executor.submit(sinker.refresh_view)
-                logger.debug(f"{view} view is refreshed")
+                futures.append(executor.submit(sinker.refresh_view))
+            for future in concurrent.futures.as_completed(futures):
+                view_result: str = future.result()
+                logger.info(f"{view_result} view is refreshed")
 
         # ---------------------------------------
         # a triggered update from here on will cause a new materialized view entry to be added to the "end"
         # of the table to be processed on the next loop iteration.
         # ---------------------------------------
 
         logger.info("Processing replication slot entries...")
```

### Comparing `sinker-0.1.0/src/sinker/settings.py` & `sinker-0.1.1/src/sinker/settings.py`

 * *Files identical despite different names*

### Comparing `sinker-0.1.0/src/sinker/sinker.py` & `sinker-0.1.1/src/sinker/sinker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import logging
 import os
-import re
 from typing import Iterable, Dict, Any
 
 import psycopg
 from elasticsearch.helpers import bulk
 
 import sinker.query_templates as q
 from .es import get_client
@@ -14,37 +13,38 @@
     DEFAULT_SCHEMA,
     SINKER_SCHEMA,
     SINKER_TODO_TABLE,
     ELASTICSEARCH_BULK_KWARGS,
     PGCHUNK_SIZE,
     SCHEMA_TABLE_DELIMITER,
 )
+from .utils import generate_schema_tables
 
 logger = logging.getLogger(__name__)
 
 BACKFILL_CURSOR_NAME = "backfill"
-TABLE_RE = re.compile(r"from\s\"?(\S+)\b", re.I)
 
 
 class Sinker:
     def __init__(self, view, index):
         """
         :param view: Postgres materialized view name
         :param index: Elasticsearch index name
         """
         self.view: str = view
         self.index: str = index
         self.parent_table: str = ""  # defined during setup process
 
-    def setup(self):
+    def setup(self) -> str:
         """
         Creates materialized views with supporting functions and triggers, and creates Elasticsearch indices
         """
         self.setup_pg()
         self.setup_es()
+        return self.view
 
     def setup_es(self) -> None:
         logger.info(f"Setting up the {self.index} Elasticsearch index")
         self.recreate_index()
         self.backfill_index()
 
         # optionally enable ES replicas here
@@ -101,33 +101,33 @@
         ddl_list.append(create_view)
         create_index: str = q.CREATE_VIEW_INDEX.format(self.view, schema_view_name)
         ddl_list.append(create_index)
         # Get constituent tables from SQL query and create function and triggers for them
         plpgsql: str = f"{schema_view_name}_fn"
         create_function: str = q.CREATE_FUNCTION.format(plpgsql, SINKER_SCHEMA, SINKER_TODO_TABLE, schema_view_name)
         ddl_list.append(create_function)
-        schema_tables: list[Any] = TABLE_RE.findall(view_select_query)
-        for schema_table in schema_tables:
+        for schema_table in generate_schema_tables(view_select_query):
             schema, _, table = schema_table.rpartition(SCHEMA_TABLE_DELIMITER)
             schema = schema or DEFAULT_SCHEMA
             trigger_name: str = f"{SINKER_SCHEMA}_{self.view}_{schema}_{table}"
             create_trigger: str = q.CREATE_TRIGGER.format(trigger_name, schema, table, plpgsql)
             ddl_list.append(create_trigger)
+            # The last table is the top-level table that gets DELETE events with an ID in the replication slot.
+            # The materialized views do not contain the ID of the doc being deleted,
+            # so we'll use this table's delete events as a proxy.
+            # lsn,xid,data
+            # 0/24EDA4D8,17393,BEGIN 17393
+            # 0/24EDA4D8,17393,"table public.""Foo"": DELETE: id[text]:'91754ea9-2983-4cf7-bdf9-fc23d2386d90'"
+            # 0/24EDC1B0,17393,COMMIT 17393
+            # 0/24EDC228,17394,BEGIN 17394
+            # 0/24EF0D60,17394,table sinker.foo_mv: DELETE: (no-tuple-data)
+            # 0/24EF4718,17394,COMMIT 17394
+            self.parent_table = schema_table
         create_todo_entry: str = q.CREATE_TODO_ENTRY.format(SINKER_SCHEMA, SINKER_TODO_TABLE, schema_view_name)
         ddl_list.append(create_todo_entry)
         psycopg.connect(autocommit=True).execute("; ".join(ddl_list))
-        # The last table is the top-level table that gets DELETE events with an ID in the replication slot.
-        # The materialized views do not contain the ID of the doc being deleted,
-        # so we'll use this table's delete events as a proxy.
-        # lsn,xid,data
-        # 0/24EDA4D8,17393,BEGIN 17393
-        # 0/24EDA4D8,17393,"table public.""Foo"": DELETE: id[text]:'91754ea9-2983-4cf7-bdf9-fc23d2386d90'"
-        # 0/24EDC1B0,17393,COMMIT 17393
-        # 0/24EDC228,17394,BEGIN 17394
-        # 0/24EF0D60,17394,table sinker.foo_mv: DELETE: (no-tuple-data)
-        # 0/24EF4718,17394,COMMIT 17394
-        self.parent_table = schema_tables[-1]
 
-    def refresh_view(self) -> None:
+    def refresh_view(self) -> str:
         logger.info(f"Refreshing the {self.view} materialized view")
         refresh_view_query: str = q.REFRESH_VIEW.format(SINKER_SCHEMA, self.view)
         psycopg.connect(autocommit=True).execute(refresh_view_query)
+        return self.view
```

