# Comparing `tmp/bmsdna_lakeapi-0.5.2.tar.gz` & `tmp/bmsdna_lakeapi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.5.2.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.6.0.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.5.2.tar` & `bmsdna_lakeapi-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1081 2023-06-01 08:34:42.665014 bmsdna_lakeapi-0.5.2/LICENSE
--rw-r--r--   0        0        0     8929 2023-06-01 08:34:42.665014 bmsdna_lakeapi-0.5.2/README.md
--rw-r--r--   0        0        0      337 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1185 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      670 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     6355 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     9131 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6039 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11357 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    11904 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    18925 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6754 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1452 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6512 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4253 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3109 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2478 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1998 2023-06-01 08:34:42.669014 bmsdna_lakeapi-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/LICENSE
+-rw-r--r--   0        0        0     8929 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/README.md
+-rw-r--r--   0        0        0      337 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1185 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      670 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     6355 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     9131 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6039 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11565 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    11712 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    15480 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6754 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1452 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6512 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4293 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3579 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3109 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2478 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1998 2023-06-01 10:49:26.913496 bmsdna_lakeapi-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.6.0/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.5.2/LICENSE` & `bmsdna_lakeapi-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/README.md` & `bmsdna_lakeapi-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,45 +13,50 @@
     Literal,
     Optional,
     Sequence,
     Tuple,
     TypedDict,
     Union,
     cast,
+    TYPE_CHECKING,
 )
 from typing_extensions import TypedDict, NotRequired, Required
 from fastapi import APIRouter, Request
 
 import yaml
 from polars.type_aliases import JoinStrategy
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 
 from bmsdna.lakeapi.core.log import get_logger
 from bmsdna.lakeapi.core.partition_utils import _with_implicit_parameters
 from bmsdna.lakeapi.core.types import FileTypes, OperatorType, Param, PolaryTypeFunction, Engines, SearchConfig
 
+if TYPE_CHECKING:
+    from bmsdna.lakeapi.context.df_base import ExecutionContext
 logger = get_logger(__name__)
 
 
 @dataclass(frozen=True)
 class BasicConfig:
     enable_sql_endpoint: bool
     temp_folder_path: str
     data_path: str
     min_search_length: int
     default_engine: Engines
+    prepare_sql_db_hook: "Callable[[ExecutionContext], Any] | None"
 
 
 def get_default_config():
     return BasicConfig(
         enable_sql_endpoint=os.getenv("ENABLE_SQL_ENDPOINT", "0") == "1",
         temp_folder_path=os.getenv("TEMP", "/tmp"),
         data_path=os.environ.get("DATA_PATH", "data"),
         min_search_length=3,
         default_engine="duckdb",
+        prepare_sql_db_hook=None,
     )
 
 
 @dataclass
 class Filter:
     key: str
     operator: Literal[
```

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,22 +36,14 @@
 
 endpoints = Literal["query", "meta", "request", "sql"]
 
 
 cache = cached(ttl=CACHE_EXPIRATION_TIME_SECONDS, cache=Cache.MEMORY, serializer=PickleSerializer())
 
 
-def get_table_name_from_uri(uri: str):
-    parts = uri.split("/")
-    try:
-        return parts[-2].replace(".", "_") + "_" + parts[-1].replace(".", "_")
-    except IndexError:
-        return uri
-
-
 class Dataframe:
     def __init__(
         self,
         version: str,
         tag: str,
         name: str,
         config: DatasourceConfig,
@@ -90,29 +82,31 @@
             ]
             df = df.select(*select)
         else:
             from pypika.terms import Star
 
             df = df.select(
                 Star(
-                    table=pypika.Table(get_table_name_from_uri(self.config.uri)),
+                    table=pypika.Table(self.tablename),
                 )
             )
         return df
 
     def _prep_df(self, df: QueryBuilder, endpoint: endpoints) -> QueryBuilder:
         if endpoint == "query":
             pass
         else:
             df = self.select_df(df)
         return df
 
     @property
     def tablename(self):
-        return self.version + "_" + self.tag + "_" + self.name + "_" + get_table_name_from_uri(self.config.uri)
+        if self.version  in ["1", "v1"]:
+            return self.tag + "_" + self.name
+        return self.tag + "_" + self.name + "_" + self.version
 
     def get_df(
         self,
         partitions: Optional[List[Tuple[str, str, Any]]],
         endpoint: endpoints = "request",
     ) -> ResultData:
         if self.df is None:
```

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/endpoint.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 from pathlib import Path
-from typing import Any, List, Literal, Optional, Type, Union, cast
+from typing import Any, Callable, List, Literal, Optional, Type, Union, cast
 from typing_extensions import TypedDict, NotRequired, Required
 import duckdb
 import polars as pl
 import pyarrow as pa
 import pypika
 import pypika.queries as fn
 from aiocache import Cache, cached
@@ -44,29 +44,14 @@
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 
 cache = cached(ttl=CACHE_EXPIRATION_TIME_SECONDS, cache=Cache.MEMORY, serializer=PickleSerializer())
 
 logger = get_logger(__name__)
 
 
-def get_delta_folders(rootdir) -> dict[str, Path]:
-    paths = [p.parent for p in Path(rootdir).rglob("*/_delta_log/")]
-    return {p.parent.name + "_" + p.name: p for p in paths}
-
-
-def register_duckdb_views(con: duckdb.DuckDBPyConnection, paths: dict[str, Path]):
-    for name, path in paths.items():
-        try:
-            dt = DeltaTable(path.absolute())
-            con.register(name, dt.to_pyarrow_dataset())
-        except PyDeltaTableError as e:
-            logger.warning(f"Could not register view for {name}. Error: {e}")
-            pass
-
-
 async def get_partitions(dataframe: Dataframe, params: BaseModel, config: Config) -> Optional[list]:
     parts = (
         await filter_partitions_based_on_params(
             DeltaTable(dataframe.uri).metadata(),
             params.dict(exclude_unset=True) if params else {},
             config.params or [],
         )
@@ -383,90 +368,7 @@
             try:
                 return await create_response(
                     request.url, format or request.headers["Accept"], df2, context, basic_config=basic_config
                 )
             except Exception as err:
                 logger.error("Error in creating response", exc_info=err)
                 raise HTTPException(status_code=500)
-
-
-duckcon: Optional[duckdb.DuckDBPyConnection] = None
-
-
-def create_sql_endpoint(router: APIRouter, basic_config: BasicConfig, configs: Configs):
-    paths = get_delta_folders(basic_config.data_path)
-
-    @router.on_event("shutdown")
-    async def shutdown_event():
-        global duckcon
-        if duckcon is not None:
-            duckcon.close()
-
-    @router.get("/api/sql/tables", tags=["sql"], operation_id="get_sql_tables")
-    async def get_sql_tables(
-        request: Request,
-        background_tasks: BackgroundTasks,
-        Accept: Union[str, None] = Header(default=None),
-        format: Optional[OutputFileType] = "json",
-    ):
-        try:
-            return [table for table in paths]
-        except Exception as err:
-            raise HTTPException(status_code=500, detail=str(err))
-
-    @router.post(
-        "/api/sql",
-        tags=["sql"],
-        operation_id="post_sql_endpoint",
-    )
-    async def get_sql_post(
-        request: Request,
-        background_tasks: BackgroundTasks,
-        Accept: Union[str, None] = Header(default=None),
-        format: Optional[OutputFileType] = "json",
-    ):
-        try:
-            body = await request.body()
-            from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContextBase
-
-            global duckcon
-            if duckcon is None:
-                duckcon = duckdb.connect()
-                register_duckdb_views(duckcon, paths)
-            context = DuckDbExecutionContextBase(duckcon)
-            df = context.execute_sql(body.decode("utf-8"))
-
-            return await create_response(
-                request.url, format or request.headers["Accept"], df, context, basic_config=basic_config
-            )
-        except Exception as err:
-            logger.error(err)
-            raise HTTPException(status_code=500, detail=str(err))
-
-    @router.get(
-        "/api/sql",
-        tags=["sql"],
-        operation_id="get_sql_endpoint",
-    )
-    async def get_sql_get(
-        request: Request,
-        background_tasks: BackgroundTasks,
-        sql: str,
-        Accept: Union[str, None] = Header(default=None),
-        format: Optional[OutputFileType] = "json",
-    ):
-        try:
-            from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContextBase
-
-            global duckcon
-            if duckcon is None:
-                duckcon = duckdb.connect()
-                register_duckdb_views(duckcon, paths)
-            context = DuckDbExecutionContextBase(duckcon)
-
-            df = context.execute_sql(sql)
-            return await create_response(
-                request.url, format or request.headers["Accept"], df, context, basic_config=basic_config
-            )
-        except Exception as err:
-            logger.error(err)
-            raise HTTPException(status_code=500, detail=str(err))
```

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/partition_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/route.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 def init_routes(configs: Configs, basic_config: BasicConfig):
     from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
 
     from bmsdna.lakeapi.core.endpoint import (
         get_response_model,
         create_detailed_meta_endpoint,
         create_config_endpoint,
-        create_sql_endpoint,
     )
+    from bmsdna.lakeapi.core.sql_endpoint import create_sql_endpoint
 
     all_lake_api_routers.append((basic_config, configs))
     router = APIRouter()
     metadata = []
 
     with DuckDbExecutionContext() as context:
         for config in configs:
```

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.5.2/pyproject.toml` & `bmsdna_lakeapi-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.5.2"
+version = "0.6.0"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.5.2/PKG-INFO` & `bmsdna_lakeapi-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.5.2
+Version: 0.6.0
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

