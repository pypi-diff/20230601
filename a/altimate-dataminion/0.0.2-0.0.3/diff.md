# Comparing `tmp/altimate_dataminion-0.0.2.tar.gz` & `tmp/altimate_dataminion-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altimate_dataminion-0.0.2.tar", max compression
+gzip compressed data, was "altimate_dataminion-0.0.3.tar", max compression
```

## Comparing `altimate_dataminion-0.0.2.tar` & `altimate_dataminion-0.0.3.tar`

### file list

```diff
@@ -1,47 +1,67 @@
--rw-r--r--   0        0        0       67 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/README.md
--rw-r--r--   0        0        0      197 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/base/__init__.py
--rw-r--r--   0        0        0     6641 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/base/dialect.py
--rw-r--r--   0        0        0     2022 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/base/extractor.py
--rw-r--r--   0        0        0     4767 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/base/metadata_profiler.py
--rw-r--r--   0        0        0     4400 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/base/profiler.py
--rw-r--r--   0        0        0     1554 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/base/source.py
--rw-r--r--   0        0        0     1549 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/config_factory.py
--rw-r--r--   0        0        0        0 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/postgresql/__init__.py
--rw-r--r--   0        0        0     7331 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/postgresql/dialect.py
--rw-r--r--   0        0        0      515 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/postgresql/extractor.py
--rw-r--r--   0        0        0      940 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/postgresql/profiler.py
--rw-r--r--   0        0        0     6053 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/postgresql/source.py
--rw-r--r--   0        0        0        0 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/s3/__init__.py
--rw-r--r--   0        0        0     7685 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/s3/source.py
--rw-r--r--   0        0        0     1261 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/shared_models.py
--rw-r--r--   0        0        0        0 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/snowflake/__init__.py
--rw-r--r--   0        0        0    13760 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/snowflake/dialect.py
--rw-r--r--   0        0        0      770 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/snowflake/profiler.py
--rw-r--r--   0        0        0     7118 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_models/snowflake/source.py
--rw-r--r--   0        0        0      208 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/builders/__init__.py
--rw-r--r--   0        0        0      134 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/builders/base_builder.py
--rw-r--r--   0        0        0     4269 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/builders/column_metrics_query_builder.py
--rw-r--r--   0        0        0      548 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/builders/custom_query_builder.py
--rw-r--r--   0        0        0     1146 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/builders/metadata_query_builder.py
--rw-r--r--   0        0        0      912 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/builders/performance_query_builder.py
--rw-r--r--   0        0        0     2091 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/builders/schema_query_builder.py
--rw-r--r--   0        0        0     1381 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/builders/table_query_builder.py
--rw-r--r--   0        0        0      999 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/builders/utils.py
--rw-r--r--   0        0        0     1280 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/exceptions.py
--rw-r--r--   0        0        0     4246 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/factory.py
--rw-r--r--   0        0        0     2271 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/main.py
--rw-r--r--   0        0        0        0 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/metrics/__init__.py
--rw-r--r--   0        0        0     2101 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/metrics/column_metric_type.py
--rw-r--r--   0        0        0      385 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/metrics/metadata_metric_type.py
--rw-r--r--   0        0        0      390 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/metrics/performance_metric_type.py
--rw-r--r--   0        0        0      363 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/metrics/schema_metric_type.py
--rw-r--r--   0        0        0      256 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/metrics/table_metric_type.py
--rw-r--r--   0        0        0        0 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/transformer/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/transformer/base.py
--rw-r--r--   0        0        0     2295 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/transformer/metrics.py
--rw-r--r--   0        0        0     2129 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/transformer/schema.py
--rw-r--r--   0        0        0      394 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/altimate_profiler/utils.py
--rw-r--r--   0        0        0      690 2023-05-12 22:45:07.796947 altimate_dataminion-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 altimate_dataminion-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       67 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/README.md
+-rw-r--r--   0        0        0      197 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/base/__init__.py
+-rw-r--r--   0        0        0     6650 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/base/dialect.py
+-rw-r--r--   0        0        0     3365 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/base/extractor.py
+-rw-r--r--   0        0        0     4767 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/base/metadata_profiler.py
+-rw-r--r--   0        0        0     4400 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/base/profiler.py
+-rw-r--r--   0        0        0     3462 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/base/source.py
+-rw-r--r--   0        0        0     6491 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/base/ssh_source.py
+-rw-r--r--   0        0        0     2710 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/config_factory.py
+-rw-r--r--   0        0        0     1344 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/constants.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/duckdb/__init__.py
+-rw-r--r--   0        0        0     7220 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/duckdb/dialect.py
+-rw-r--r--   0        0        0     2694 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/duckdb/extractor.py
+-rw-r--r--   0        0        0     4793 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/duckdb/metadata_profiler.py
+-rw-r--r--   0        0        0     3119 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/duckdb/profiler.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/postgresql/__init__.py
+-rw-r--r--   0        0        0     7331 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/postgresql/dialect.py
+-rw-r--r--   0        0        0      331 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/postgresql/extractor.py
+-rw-r--r--   0        0        0     1190 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/postgresql/profiler.py
+-rw-r--r--   0        0        0     5988 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/postgresql/source.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/s3/__init__.py
+-rw-r--r--   0        0        0     2196 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/s3/csv_source_dialect.py
+-rw-r--r--   0        0        0      361 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/s3/extractor.py
+-rw-r--r--   0        0        0     2252 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/s3/json_source_dialect.py
+-rw-r--r--   0        0        0     1872 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/s3/parquet_source_dialect.py
+-rw-r--r--   0        0        0      939 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/s3/profiler.py
+-rw-r--r--   0        0        0     7685 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/s3/source.py
+-rw-r--r--   0        0        0      390 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/s3/utils.py
+-rw-r--r--   0        0        0     1289 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/shared_models.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/snowflake/__init__.py
+-rw-r--r--   0        0        0    13760 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/snowflake/dialect.py
+-rw-r--r--   0        0        0     1083 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/snowflake/profiler.py
+-rw-r--r--   0        0        0     7361 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_models/snowflake/source.py
+-rw-r--r--   0        0        0      260 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/builders/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/builders/base_builder.py
+-rw-r--r--   0        0        0     4269 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/builders/column_metrics_query_builder.py
+-rw-r--r--   0        0        0      548 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/builders/custom_query_builder.py
+-rw-r--r--   0        0        0     1146 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/builders/metadata_query_builder.py
+-rw-r--r--   0        0        0      912 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/builders/performance_query_builder.py
+-rw-r--r--   0        0        0     1637 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/builders/s3_column_metrics_query_builder.py
+-rw-r--r--   0        0        0     2127 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/builders/s3_schema_query_builder.py
+-rw-r--r--   0        0        0     1052 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/builders/s3_table_query_builder.py
+-rw-r--r--   0        0        0     2091 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/builders/schema_query_builder.py
+-rw-r--r--   0        0        0     1381 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/builders/table_query_builder.py
+-rw-r--r--   0        0        0      999 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/builders/utils.py
+-rw-r--r--   0        0        0     1440 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/exceptions.py
+-rw-r--r--   0        0        0     4239 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/factory.py
+-rw-r--r--   0        0        0     2308 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/main.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/metrics/__init__.py
+-rw-r--r--   0        0        0     2101 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/metrics/column_metric_type.py
+-rw-r--r--   0        0        0      385 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/metrics/metadata_metric_type.py
+-rw-r--r--   0        0        0      390 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/metrics/performance_metric_type.py
+-rw-r--r--   0        0        0      363 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/metrics/schema_metric_type.py
+-rw-r--r--   0        0        0      256 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/metrics/table_metric_type.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/transformer/__init__.py
+-rw-r--r--   0        0        0     1716 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/transformer/base.py
+-rw-r--r--   0        0        0     2061 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/transformer/duckdb_schema.py
+-rw-r--r--   0        0        0     2295 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/transformer/metrics.py
+-rw-r--r--   0        0        0     2129 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/transformer/schema.py
+-rw-r--r--   0        0        0      394 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/utils.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/validator/__init__.py
+-rw-r--r--   0        0        0     2207 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/validator/mappers.py
+-rw-r--r--   0        0        0     1998 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/altimate_profiler/validator/utils.py
+-rw-r--r--   0        0        0      764 2023-06-01 00:46:25.023987 altimate_dataminion-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 altimate_dataminion-0.0.3/PKG-INFO
```

### Comparing `altimate_dataminion-0.0.2/altimate_models/base/dialect.py` & `altimate_dataminion-0.0.3/altimate_models/base/dialect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import List, Text
 
 from altimate_models.shared_models import Policy, TableResource
-from altimate_profiler.builders.column_metrics_query_builder import ColumnMetricsQueryBuilder
+from altimate_profiler.builders.column_metrics_query_builder import (
+    ColumnMetricsQueryBuilder,
+)
 from altimate_profiler.builders.table_query_builder import TableQueryBuilder
 
 
 class SQLAlchemySourceDialect:
     @classmethod
     def _row_count(cls, table, params):
         return "select COALESCE(COUNT(*), 0)  from {table}".format(table=table)
```

### Comparing `altimate_dataminion-0.0.2/altimate_models/base/extractor.py` & `altimate_dataminion-0.0.3/altimate_models/base/extractor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 import logging
-from typing import Text
+from typing import Optional, Text
 
 from sqlalchemy import create_engine, inspect
 
+from altimate_models.base.source import DataSource
+from altimate_models.constants import TEST_SQL_QUERY
+
 
 class SQLAlchemyExtractor:
-    def __init__(self, connection_str: Text):
+    # TODO: currently allowing connection_str as well as datasource.
+    # should get rid of raw strings passed around at some point: AL-639
+    def __init__(
+        self,
+        connection_str: Optional[Text] = None,
+        data_source: Optional[DataSource] = None,
+    ):
         self.connection_str = connection_str
+        self.data_source: DataSource = data_source
         self.engine = None
         self.connection = None
 
     def _initialize(self):
         if self.engine and self.connection:
             return
 
@@ -45,35 +55,55 @@
 
         if self.engine is not None:
             self.engine.dispose()
             self.engine = None
 
     def test(self):
         try:
-            self._initialize()
-            result = self._execute("SELECT 1")
-            self._terminate()
+            if self.data_source:
+                with self.data_source.get_engine() as engine:
+                    with engine.connect() as connection:
+                        self.connection = connection
+                        result = self._execute(TEST_SQL_QUERY)
+                        rows = result["rows"]
+                        columns = result["columns"]
+
+                        return_result = (
+                            len(rows) == 1 and rows[0][columns[0]] == 1
+                        )  # TODO: Fix Indexing
+
+                return return_result
+
+            else:
+                # Keeping this to support older connection_str method
+                self._initialize()
+                result = self._execute(TEST_SQL_QUERY)
+                self._terminate()
 
-            rows = result["rows"]
-            columns = result["columns"]
+                rows = result["rows"]
+                columns = result["columns"]
 
-            return len(rows) == 1 and rows[0][columns[0]] == 1  # TODO: Fix Indexing
+                return len(rows) == 1 and rows[0][columns[0]] == 1  # TODO: Fix Indexing
         except Exception as e:
             logging.error(e)
             return False
 
     def foreign_keys(self, table_name: Text):
         self._initialize()
 
         inspector = inspect(self.engine)
         foreign_keys = inspector.get_foreign_keys(table_name)
 
         return foreign_keys
 
     def run(self, sql: Text):
-        self._initialize()
-
-        results = self._execute(sql)
-
-        self._terminate()
+        if self.data_source:
+            with self.data_source.get_engine() as engine:
+                with engine.connect() as connection:
+                    self.connection = connection
+                    results = self._execute(sql)
+        else:
+            self._initialize()
+            results = self._execute(sql)
+            self._terminate()
 
         return results
```

### Comparing `altimate_dataminion-0.0.2/altimate_models/base/metadata_profiler.py` & `altimate_dataminion-0.0.3/altimate_models/base/metadata_profiler.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_models/base/profiler.py` & `altimate_dataminion-0.0.3/altimate_models/base/profiler.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_models/postgresql/dialect.py` & `altimate_dataminion-0.0.3/altimate_models/postgresql/dialect.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_models/postgresql/profiler.py` & `altimate_dataminion-0.0.3/altimate_models/postgresql/profiler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+from typing import TYPE_CHECKING
+
 from altimate_models.base.profiler import SQLAlchemyProfiler
-from altimate_models.base.source import DataSource
 from altimate_models.postgresql.dialect import PostgreSQLSourceDialect
 from altimate_models.postgresql.extractor import PostgreSQLExtractor
 from altimate_models.shared_models import Policy, ResourceType
 
+if TYPE_CHECKING:
+    from altimate_models.postgresql.source import PostgresSource
+
 
 class PostgreSQLProfiler(SQLAlchemyProfiler):
-    def __init__(self, data_source: DataSource, policy: Policy):
+    def __init__(self, data_source: "PostgresSource", policy: Policy):
         if policy.resource0.resource_type != ResourceType.TABLE:
             raise Exception("PostgreSQLProfiler only supports table resources")
 
+        # FIXME - There should be a check here to ensure that
+        # database in source and in policy both match
         super().__init__(
             extractor=PostgreSQLExtractor(
-                data_source.get_connection_string(
-                    database=policy.resource0.resource.database,
-                    schema=policy.resource0.resource.db_schema,
-                )
+                connection_str=data_source.get_connection_string(
+                    # database=policy.resource0.resource.database,
+                    # schema=policy.resource0.resource.db_schema,
+                ),
+                data_source=data_source,
             ),
             policy=policy,
             dialect=PostgreSQLSourceDialect(),
         )
```

### Comparing `altimate_dataminion-0.0.2/altimate_models/postgresql/source.py` & `altimate_dataminion-0.0.3/altimate_models/postgresql/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,22 @@
     host: Optional[Text]
     port: Optional[Text]
     user: Optional[Text]
     password: Optional[Text]
     database: Optional[Text]
     sync_credentials: bool = False
 
-    def get_connection_string(
-        self, database: Text = None, schema: Text = None, *args, **kwargs
-    ) -> Text:
+    def get_connection_string(self, *args, **kwargs) -> Text:
+        host = kwargs.get("host", self.host)
+        port = kwargs.get("port", self.port)
         return "postgresql://{user}:{password}@{host}:{port}/{database}".format(
             user=self.user,
             password=self.password,
-            host=self.host,
-            port=self.port,
+            host=host,
+            port=port,
             database=self.database,
         )
 
     @classmethod
     def get_connection_information(cls, data_store_config: Dict):
         data_store_config[
             "connection_info"
@@ -77,19 +77,18 @@
         self.connection_hash = conn_info["connection_hash"]
 
     def test_connection(self):
         if not "sqlalchemy" in sys.modules:
             raise ImportError(
                 "sqlalchemy is not installed. Please install sqlalchemy to test connections"
             )
-        connection_string = self.get_connection_string(database=self.database)
         try:
-            engine = create_engine(connection_string)
-            engine.connect()
-            print(green_bold_string("Successfully connected to Postgres!"))
+            with self.get_engine() as engine:
+                engine.connect()
+                print(green_bold_string("Successfully connected to Postgres!"))
 
         except Exception as e:
             print(red("Connection to Postgres failed."))
             print("Check your credentials and try again.")
             raise AltimateDataStoreConnectionException(
                 f"Connection to {self.name} failed." f" Please check the credentials"
             )
@@ -150,10 +149,10 @@
         host, port = url.split(":")
         return {"host": host, "port": port, "database": database}
 
     def update_credentials(self, credentials: str):
         _user, _pass = credentials.split(":")
         self.user = _user
         self.password = _pass
-        
+
     def override_schema(self, schema):
         return schema
```

### Comparing `altimate_dataminion-0.0.2/altimate_models/s3/source.py` & `altimate_dataminion-0.0.3/altimate_models/s3/source.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_models/shared_models.py` & `altimate_dataminion-0.0.3/altimate_models/shared_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 class ResourceType(Enum):
     FILE = "file"
     TABLE = "table"
 
 
 class TableResource(BaseModel):
     database: Text
-    db_schema: Optional[Text] = Field(alias="schema")
-    table: Optional[Text]
+    db_schema: Optional[Text] = Field(alias="schema", default=None)
+    table: Optional[Text] = None
 
 
 class S3Resource(BaseModel):
     bucket: Text
     path: Text
     format: Text
     options: Optional[Dict[Text, Any]]
 
 
 class Resource(BaseModel):
     resource_type: ResourceType
     resource: Union[TableResource, S3Resource]
-    filters: Optional[Text]
+    filters: Optional[Text] = None
 
 
 class Policy(BaseModel):
     policy_index: int
     policy_type: Text
     resources: List[Resource]
     filters: Optional[Text]
```

### Comparing `altimate_dataminion-0.0.2/altimate_models/snowflake/dialect.py` & `altimate_dataminion-0.0.3/altimate_models/snowflake/dialect.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_models/snowflake/profiler.py` & `altimate_dataminion-0.0.3/altimate_models/snowflake/profiler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,27 @@
+from typing import TYPE_CHECKING
+
 from altimate_models.base.extractor import SQLAlchemyExtractor
 from altimate_models.base.profiler import SQLAlchemyProfiler
-from altimate_models.base.source import DataSource
 from altimate_models.shared_models import Policy
 from altimate_models.snowflake.dialect import SnowflakeSourceDialect
 
+if TYPE_CHECKING:
+    from altimate_models.snowflake.source import SnowflakeSource
+
 
 class SnowflakeProfiler(SQLAlchemyProfiler):
-    def __init__(self, data_source: DataSource, policy: Policy):
+    def __init__(self, data_source: "SnowflakeSource", policy: Policy):
+        # FIXME - raise exception if the database in datasource
+        # and that in policy is not the same.
+        # data_source.database = policy.resource0.resource.database
         super().__init__(
             extractor=SQLAlchemyExtractor(
-                data_source.get_connection_string(
-                    database=policy.resource0.resource.database,
-                    schema=policy.resource0.resource.db_schema,
-                )
+                connection_str=data_source.get_connection_string(
+                    # database=policy.resource0.resource.database,
+                    # schema=policy.resource0.resource.db_schema,
+                ),
+                data_source=data_source,
             ),
             policy=policy,
             dialect=SnowflakeSourceDialect(),
         )
```

### Comparing `altimate_dataminion-0.0.2/altimate_models/snowflake/source.py` & `altimate_dataminion-0.0.3/altimate_models/snowflake/source.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,28 +19,29 @@
     role: Optional[Text]
     warehouse: Optional[Text]
     user: Optional[Text]
     password: Optional[Text]
     database: Optional[Text]
     sync_credentials: bool = False
 
-    def get_connection_string(
-        self, database: Text = None, schema: Text = None, *args, **kwargs
-    ) -> Text:
+    def get_connection_string(self, *args, **kwargs) -> Text:
         connection_string = "{NAME}://{user}:{password}@{account}/{database}".format(
             NAME=self.NAME,
             user=self.user,
             password=self.password,
             account=self.account,
             database=self.database,
             warehouse=self.warehouse,
             role=self.role,
         )
-        if schema:
-            connection_string += "/{schema}".format(schema=schema)
+        # uncomment this when we add support for changing schema
+        # CAUTION: schema is used internally by pydantic.
+        # when we do add this, use a different name
+        # if schema:
+        #     connection_string += "/{schema}".format(schema=schema)
         connection_string += "?warehouse={warehouse}&role={role}".format(
             warehouse=self.warehouse,
             role=self.role,
         )
         return connection_string
 
     @classmethod
@@ -90,19 +91,18 @@
         self.connection_hash = conn_info["connection_hash"]
 
     def test_connection(self):
         if not "sqlalchemy" in sys.modules:
             raise ImportError(
                 "sqlalchemy is not installed. Please install sqlalchemy to test connections"
             )
-        connection_string = self.get_connection_string(database=self.database)
         try:
-            engine = create_engine(connection_string)
-            engine.connect()
-            print(green_bold_string("Successfully connected to Snowflake!"))
+            with self.get_engine() as engine:
+                engine.connect()
+                print(green_bold_string("Successfully connected to Snowflake!"))
 
         except Exception as e:
             print(red("Connection to Snowflake failed."))
             print("Check your credentials and try again.")
             raise AltimateDataStoreConnectionException(
                 f"Connection to {self.name} failed." f" Please check the credentials"
             )
@@ -112,14 +112,16 @@
         password = config_dict.pop("password")
         username = config_dict.pop("user")
         if self.sync_credentials:
             config_dict["key"] = f"altimate:{username}:{password}"
         return config_dict
 
     def get_resource(self):
+        if self.database is None:
+            raise ValueError("database must be set to get resource")
         return Resource(
             resource_type=ResourceType.TABLE,
             resource=TableResource(
                 database=self.database,
             ),
         )
 
@@ -134,14 +136,16 @@
         fqn = f"database={self.database}/schema={schema}/table={table}"
         return identifier, fqn
 
     @classmethod
     def get_resource_config(cls, resource_config: Dict):
         filters = resource_config.get("filters")
         identifier = resource_config.get("identifier")
+        if identifier is None:
+            raise ValueError("identifier must be set to get resource")
         data_store_type, path = identifier.split("://")
         database, schema, table = path.split(".")
         resource = TableResource(database=database, schema=schema, table=table)
         return Resource(
             resource_type=ResourceType.TABLE, resource=resource, filters=filters
         )
 
@@ -172,15 +176,15 @@
         url, params = connection_info.split("?")
         account, database = url.split("/")
         config = {"account": account, "database": database}
         for param in params.split("&"):
             key, value = param.split("=")
             config[key] = value
         return config
-    
+
     def update_credentials(self, credentials: str):
         _user, _pass = credentials.split(":")
         self.user = _user
         self.password = _pass
 
     def override_schema(self, schema):
         return schema
```

### Comparing `altimate_dataminion-0.0.2/altimate_profiler/builders/column_metrics_query_builder.py` & `altimate_dataminion-0.0.3/altimate_profiler/builders/column_metrics_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_profiler/builders/custom_query_builder.py` & `altimate_dataminion-0.0.3/altimate_profiler/builders/custom_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_profiler/builders/metadata_query_builder.py` & `altimate_dataminion-0.0.3/altimate_profiler/builders/metadata_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_profiler/builders/performance_query_builder.py` & `altimate_dataminion-0.0.3/altimate_profiler/builders/performance_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_profiler/builders/schema_query_builder.py` & `altimate_dataminion-0.0.3/altimate_profiler/builders/schema_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_profiler/builders/table_query_builder.py` & `altimate_dataminion-0.0.3/altimate_profiler/builders/table_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_profiler/builders/utils.py` & `altimate_dataminion-0.0.3/altimate_profiler/builders/utils.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_profiler/exceptions.py` & `altimate_dataminion-0.0.3/altimate_profiler/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,7 +68,14 @@
 
 class AltimateRegistryNotFoundError(Exception):
     pass
 
 
 class AltimateJSONFileNotLoadingError(Exception):
     pass
+
+
+INVALID_UNICODE_IN_CSV = "Invalid unicode (byte sequence mismatch) detected in CSV file"
+
+
+class AltimateInvalidCharactersInCSVException(Exception):
+    pass
```

### Comparing `altimate_dataminion-0.0.2/altimate_profiler/factory.py` & `altimate_dataminion-0.0.3/altimate_profiler/factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from typing import Text
 
 from altimate_models.base.extractor import SQLAlchemyExtractor
 from altimate_models.base.metadata_profiler import SqlAlchemyMetadataProfiler
 from altimate_models.base.source import DataSource
 from altimate_models.postgresql.dialect import PostgreSQLSourceDialect
+from altimate_models.postgresql.extractor import PostgreSQLExtractor
 from altimate_models.postgresql.profiler import PostgreSQLProfiler
+from altimate_models.s3.source import S3Source
 
-# from altimate_profiler.duckdb_profiler.dialect import DuckDBSourceDialect
-# from altimate_profiler.duckdb_profiler.extractor import DuckDBExtractor
-# from altimate_profiler.duckdb_profiler.files.csv.dialect import CsvSourceDialect
-# from altimate_profiler.duckdb_profiler.files.json.dialect import JsonSourceDialect
-# from altimate_profiler.duckdb_profiler.files.parquet.dialect import ParquetSourceDialect
-# from altimate_profiler.duckdb_profiler.metadata.profiler import DuckDBMetadataProfiler
-# from altimate_profiler.duckdb_profiler.source.s3.models import S3Profiler
-# from altimate_profiler.duckdb_profiler.transformer.schema_transformer import DuckDBSchemaTransformer
+from altimate_models.duckdb.extractor import DuckDBExtractor
+from altimate_models.s3.csv_source_dialect import CsvSourceDialect
+from altimate_models.s3.json_source_dialect import JsonSourceDialect
+from altimate_models.s3.parquet_source_dialect import ParquetSourceDialect
+from altimate_models.duckdb.metadata_profiler import DuckDBMetadataProfiler
+from altimate_models.s3.profiler import S3Profiler
+from altimate_profiler.transformer.duckdb_schema import DuckDBSchemaTransformer
 from altimate_models.shared_models import Policy
 from altimate_models.snowflake.dialect import SnowflakeSourceDialect
 from altimate_models.snowflake.profiler import SnowflakeProfiler
+
 from altimate_profiler.exceptions import AltimateDataStoreNotSupported
 from altimate_profiler.transformer.base import Transformer
 from altimate_profiler.transformer.schema import SchemaTransformer
 
 
 class SchemaTransformerFactory:
     SOURCE_MAP = {
         "snowflake": SchemaTransformer,
         "postgres": SchemaTransformer,
-        # "s3": DuckDBSchemaTransformer,
+        "s3": DuckDBSchemaTransformer,
     }
     TABLE_SOURCES = ["snowflake", "postgres"]
     FILE_SOURCES = ["s3"]
 
     @classmethod
     def create(cls, data_source_type: Text) -> Transformer:
         transformer = cls.SOURCE_MAP.get(data_source_type)
@@ -39,15 +41,15 @@
         return transformer
 
 
 class MetadataFactory:
     DATA_SOURCE_TO_PROFILER = {
         "snowflake": SqlAlchemyMetadataProfiler,
         "postgres": SqlAlchemyMetadataProfiler,
-        # "s3": DuckDBMetadataProfiler,
+        "s3": DuckDBMetadataProfiler,
     }
 
     @classmethod
     def create(
         cls,
         data_source: DataSource,
         policy: Policy,
@@ -61,15 +63,15 @@
         return profiler(data_source, dialect, policy, resource_name)
 
 
 class ProfilerFactory:
     DATA_SOURCE_TO_PROFILER = {
         "snowflake": SnowflakeProfiler,
         "postgres": PostgreSQLProfiler,
-        # "s3": S3Profiler,
+        "s3": S3Profiler,
     }
 
     @classmethod
     def create(cls, data_source: DataSource, policy: Policy):
         profiler = cls.DATA_SOURCE_TO_PROFILER.get(data_source.type)
         if not profiler:
             raise AltimateDataStoreNotSupported("Data source is not supported!")
@@ -77,40 +79,42 @@
         return profiler(data_source, policy)
 
 
 class DialectFactory:
     DATA_SOURCE_TO_DIALECT = {
         "snowflake": SnowflakeSourceDialect,
         "postgres": PostgreSQLSourceDialect,
-        # "s3": {
-        #     "csv": CsvSourceDialect,
-        #     "parquet": ParquetSourceDialect,
-        #     "json": JsonSourceDialect,
-        # }
+        "s3": {
+            "csv": CsvSourceDialect,
+            "parquet": ParquetSourceDialect,
+            "json": JsonSourceDialect,
+        }
     }
 
     @classmethod
     def create(cls, data_source: DataSource):
-        if data_source.type == "s3":
-            dialect = cls.DATA_SOURCE_TO_DIALECT.get(data_source.type).get(
+        if isinstance(
+            data_source, S3Source
+        ):  # use stronger match than string comparison `data_source.type == "s3":`
+            dialect = cls.DATA_SOURCE_TO_DIALECT.get('s3').get(
                 data_source.file_format
             )
         else:
             dialect = cls.DATA_SOURCE_TO_DIALECT.get(data_source.type)
 
         if not dialect:
             raise AltimateDataStoreNotSupported("Data source is not supported!")
         return dialect
 
 
 class ExtractorFactory:
     DATA_SOURCE_TO_Extractor = {
         "snowflake": SQLAlchemyExtractor,
-        "postgres": SQLAlchemyExtractor,
-        # "s3": DuckDBExtractor,
+        "postgres": PostgreSQLExtractor,
+        "s3": DuckDBExtractor,
     }
 
     @classmethod
     def create(cls, data_source: DataSource):
         extractor = cls.DATA_SOURCE_TO_Extractor.get(data_source.type)
         if not extractor:
             raise AltimateDataStoreNotSupported("Data source is not supported!")
```

### Comparing `altimate_dataminion-0.0.2/altimate_profiler/main.py` & `altimate_dataminion-0.0.3/altimate_profiler/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,54 @@
-from typing import List
+from typing import TYPE_CHECKING, List
+
+if TYPE_CHECKING:
+    from altimate_models.base.source import DataSource
 
-from altimate_models.base.source import DataSource
 from altimate_models.shared_models import Policy, ProfileConfig, Resource, ResourceType
 from altimate_profiler.factory import (
     DialectFactory,
-    ExtractorFactory,
     MetadataFactory,
     ProfilerFactory,
     SchemaTransformerFactory,
 )
 from altimate_profiler.transformer.metrics import MetricTransformer
 
 
-def get_schema_profile(data_source: DataSource, profile_config: ProfileConfig) -> List:
+def get_schema_profile(
+    data_source: "DataSource", profile_config: ProfileConfig
+) -> List:
     schemas = []
     for policy in profile_config.policies:
         profiler = ProfilerFactory.create(data_source, policy)
         discovered_data = profiler.get_discovery_data()
         transformer = SchemaTransformerFactory.create(data_source.type)
         schema = transformer.transform(discovered_data)
         schemas.append(schema)
+
     return schemas
 
 
-def get_metrics_profile(data_source: DataSource, profile_config: ProfileConfig) -> List:
+def get_metrics_profile(
+    data_source: "DataSource", profile_config: ProfileConfig
+) -> List:
     metrics = []
     for policy in profile_config.policies:
         profiler = ProfilerFactory.create(data_source, policy)
 
         raw_metrics = profiler.get_metrics_data()
         transformer = MetricTransformer()
 
         transformed_metrics = transformer.transform(raw_metrics)
 
         metrics.append(transformed_metrics)
 
     return metrics
 
 
-def get_metadata(data_source: DataSource, resource: Resource) -> List:
+def get_metadata(data_source: "DataSource", resource: Resource) -> List:
     dialect = DialectFactory.create(data_source)
     if resource.resource_type == ResourceType.FILE:
         resource.resource.options = dialect.get_options(resource.resource.options)
         resource_name = dialect.create_table_path(resource.resource, dialect.DATA_QUERY)
     else:
         resource_name = dialect.create_table_path(resource.resource)
 
@@ -52,11 +58,11 @@
     policy = Policy(
         policy_index=0, resources=[resource], terms=[], policy_type="metadata"
     )
     profiler = MetadataFactory.create(data_source, policy, resource_name)
     return profiler.get_metadata()
 
 
-def get_debug_data(data_source: DataSource, debug_sql: str) -> List:
+def get_debug_data(data_source: "DataSource", debug_sql: str) -> List:
     policy = Policy(policy_index=0, resources=[], terms=[], policy_type="metadata")
     profiler = MetadataFactory.create(data_source, policy, "")
     return profiler.get_debugdata(debug_sql)
```

### Comparing `altimate_dataminion-0.0.2/altimate_profiler/metrics/column_metric_type.py` & `altimate_dataminion-0.0.3/altimate_profiler/metrics/column_metric_type.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_profiler/transformer/base.py` & `altimate_dataminion-0.0.3/altimate_profiler/transformer/base.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_profiler/transformer/metrics.py` & `altimate_dataminion-0.0.3/altimate_profiler/transformer/metrics.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/altimate_profiler/transformer/schema.py` & `altimate_dataminion-0.0.3/altimate_profiler/transformer/schema.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.2/pyproject.toml` & `altimate_dataminion-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "altimate-dataminion"
-version = "0.0.2"
+version = "0.0.3"
 description = "Internal package. Use this at your own risk, support not guaranteed"
 authors = ["Shardul Sardesai <shardul@altimate.ai>"]
 readme = "README.md"
 packages = [{include = "altimate_profiler"}, {include = "altimate_models"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
@@ -14,12 +14,16 @@
 mypy = "^1.2.0"
 isort = "^5.12.0"
 jsonschema = "^4.17.3"
 snowflake-connector-python = "^3.0.3"
 snowflake-sqlalchemy = "^1.4.7"
 sqlalchemy = {version = "<2.0.0", extras = ["mypy"]}
 psycopg2-binary = "2.9.5"
+sshtunnel = "^0.4.0"
+numpy = "^1.24.3"
+pandas = "^2.0.1"
+duckdb = "0.7.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

