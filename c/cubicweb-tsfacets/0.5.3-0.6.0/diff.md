# Comparing `tmp/cubicweb-tsfacets-0.5.3.tar.gz` & `tmp/cubicweb-tsfacets-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-tsfacets-0.5.3.tar", last modified: Mon Dec 12 11:39:07 2022, max compression
+gzip compressed data, was "cubicweb-tsfacets-0.6.0.tar", last modified: Thu Jun  1 14:24:00 2023, max compression
```

## Comparing `cubicweb-tsfacets-0.5.3.tar` & `cubicweb-tsfacets-0.6.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 11:39:07.186296 cubicweb-tsfacets-0.5.3/
--rw-rw-rw-   0 root         (0) root         (0)      372 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3453 2022-12-12 11:39:07.186296 cubicweb-tsfacets-0.5.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2931 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 11:39:07.182296 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/
--rw-rw-rw-   0 root         (0) root         (0)     1882 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/ccplugin.py
--rw-rw-rw-   0 root         (0) root         (0)      854 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      867 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 11:39:07.182296 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      248 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/i18n/fr.po
--rw-rw-rw-   0 root         (0) root         (0)     4990 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 11:39:07.182296 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1089 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)    12593 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 11:39:07.182296 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3453 2022-12-12 11:39:06.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      773 2022-12-12 11:39:07.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-12 11:39:06.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2022-12-12 11:39:06.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-12 11:39:06.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       35 2022-12-12 11:39:06.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-12-12 11:39:07.000000 cubicweb-tsfacets-0.5.3/cubicweb_tsfacets.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-12 11:39:07.186296 cubicweb-tsfacets-0.5.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2676 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 11:39:07.186296 cubicweb-tsfacets-0.5.3/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 11:39:07.186296 cubicweb-tsfacets-0.5.3/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     1703 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/test/test_tsfacets.py
--rw-rw-rw-   0 root         (0) root         (0)     1342 2022-12-12 11:38:53.000000 cubicweb-tsfacets-0.5.3/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:24:00.224832 cubicweb-tsfacets-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3433 2023-06-01 14:24:00.224832 cubicweb-tsfacets-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:24:00.224832 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/
+-rw-rw-rw-   0 root         (0) root         (0)     3658 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/ccplugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      854 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:24:00.224832 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)     5115 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:24:00.224832 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)    12771 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:24:00.224832 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3433 2023-06-01 14:24:00.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      773 2023-06-01 14:24:00.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 14:24:00.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-01 14:24:00.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 14:24:00.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-01 14:24:00.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-01 14:24:00.000000 cubicweb-tsfacets-0.6.0/cubicweb_tsfacets.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 14:24:00.224832 cubicweb-tsfacets-0.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2676 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:24:00.224832 cubicweb-tsfacets-0.6.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:24:00.224832 cubicweb-tsfacets-0.6.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     1703 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/test/test_tsfacets.py
+-rw-rw-rw-   0 root         (0) root         (0)     1342 2023-06-01 14:23:52.000000 cubicweb-tsfacets-0.6.0/tox.ini
```

### Comparing `cubicweb-tsfacets-0.5.3/PKG-INFO` & `cubicweb-tsfacets-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-tsfacets
-Version: 0.5.3
+Version: 0.6.0
 Summary: This cube implements facets using postgresql text search vectors.
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/tsfacets
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: JavaScript
 Description-Content-Type: text/markdown
 
 Summary
@@ -83,9 +82,7 @@
     }
 
     target_etypes = {"Performance"}
 ```
 
 Thus, `CubicWeb-TSFacets` will provide the methods we will need to
 build our interface.
-
-
```

### Comparing `cubicweb-tsfacets-0.5.3/README.md` & `cubicweb-tsfacets-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/ccplugin.py` & `cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/ccplugin.py`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/entities.py` & `cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/hooks.py` & `cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/importer.py` & `cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/importer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cubicweb_tsfacets import convert_sql_to_rql
+from cubicweb_tsfacets import convert_rql_to_sql
 from cubicweb_tsfacets.views import build_mapping_table_name
 
 
 def build_facet_table(cnx, facet_cls):
     table_name = facet_cls.table_name
     ts_config = cnx.vreg.config["text-search-config"]
     target_etype_sql_part = ",".join(
@@ -18,15 +18,15 @@
     from_parts = []
     vector_parts = []
     args = {}
     for (
         facet_key,
         request_facet_def,
     ) in facet_cls.key_names_to_rql_definition.items():
-        sql, _args = convert_sql_to_rql(cnx, request_facet_def.rql_request)
+        sql, _args = convert_rql_to_sql(cnx, request_facet_def.rql_request)
         for key, value in _args.items():
             # here we want to be sure we don't have the same keys on all
             # generated SQL
             new_k = str(hash((facet_key, sql, key)))
             sql = sql.replace(f"%({key})s", f"%({new_k})s")
             args[new_k] = value
         if request_facet_def.needs_mapping:
@@ -40,19 +40,20 @@
             cnx.system_sql(f"DROP TABLE IF EXISTS {mapping_table_name}")
             cnx.system_sql(
                 f"""
                 CREATE TABLE
                     {mapping_table_name} (id serial PRIMARY KEY, value varchar)
                 """
             )
-            insert = f"""
-            INSERT INTO {mapping_table_name} (value)
-            values {",".join(["(%s)"]*len(all_values))}
-            """
-            cnx.system_sql(insert, list(all_values))
+            if all_values:
+                insert = f"""
+                INSERT INTO {mapping_table_name} (value)
+                values {",".join(["(%s)"]*len(all_values))}
+                """
+                cnx.system_sql(insert, list(all_values))
             cnx.system_sql(f"CREATE INDEX ON {mapping_table_name}(value)")
             from_parts.append(
                 f"""
                 LEFT OUTER JOIN (
                     SELECT
                         _f{facet_key}_to_be_mapped.target_eid,
                         {mapping_table_name}.id
@@ -77,15 +78,15 @@
             ARRAY_AGG(
                 DISTINCT CASE WHEN _f{facet_key}.value is NULL
                 THEN ''  ELSE '{facet_key}.' || _f{facet_key}.value END
             )
             """
         )
     if facet_cls.text_search_indexation:
-        sql, _args = convert_sql_to_rql(cnx, facet_cls.text_search_indexation)
+        sql, _args = convert_rql_to_sql(cnx, facet_cls.text_search_indexation)
         for key, value in _args.items():
             # here we want to be sure we don't have the same keys on all
             # generated SQL
             new_k = str(hash((facet_key, sql, key)))
             sql = sql.replace(f"%({key})s", f"%({new_k})s")
             args[new_k] = value
         fti_vector_from = f"""
@@ -120,14 +121,15 @@
                     {fti_vector_from}
                 GROUP BY entities.eid
                 {", _tstable.text" if fti_vector_from else ""}
             )
         """,
         args,
     )
+    cnx.system_sql(f"CREATE INDEX {table_name}_eid_idx ON {table_name}(eid)")
     if fti_vector_from:
         cnx.system_sql(
             f"CREATE INDEX {table_name}_ginidx ON {table_name} USING GIN(textsearchvector)"
         )
     cnx.system_sql(
         f"CREATE INDEX {table_name}_fti_ginidx ON {table_name} USING GIN(facetvector)"
     )
```

### Comparing `cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/migration/postcreate.py` & `cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/schema.py` & `cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.5.3/cubicweb_tsfacets/views.py` & `cubicweb-tsfacets-0.6.0/cubicweb_tsfacets/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 from typing import Dict, List, Set, Tuple, Optional, Union
 from typing_extensions import TypedDict
-import re
 
 from cubicweb.appobject import AppObject
 from cubicweb.rset import ResultSet
 from cubicweb_tsfacets import (
-    convert_sql_to_rql,
+    convert_rql_to_sql,
     build_rset_descr,
     convert_to_tsquery,
+    TSFacetsSQLGenerator,
 )
 
 
 class FacetItemType(TypedDict):
     value: str
     count: str
 
@@ -88,19 +88,18 @@
 
     def _build_sql_parts(
         self,
         rql: str = None,
         rql_args: Dict = None,
         selected_facets: Dict[str, List[str]] = None,
         text_search: str = None,
-        quote_to_use_in_sql="'",
         with_row_nb: bool = False,
     ) -> Tuple[str, str, Dict[str, str]]:
         if rql:
-            converted_sql, sql_args = convert_sql_to_rql(self._cw.cnx, rql, rql_args)
+            converted_sql, sql_args = convert_rql_to_sql(self._cw.cnx, rql, rql_args)
             if with_row_nb:
                 converted_sql = f"""
                 SELECT _TABLE_TO_COUNT.*, ROW_NUMBER() OVER () AS row_nb
                 FROM ({converted_sql}) as _TABLE_TO_COUNT
                 """
             sql_restriction_part = f"""
             JOIN ({converted_sql}) as _TABLE_FROM_RQL(target_eid)
@@ -115,35 +114,35 @@
         ts_vector_parts = self._build_tsvector_parts(selected_facets or {})
         where_parts = []
         if ts_vector_parts:
             # here we use double ' because we will be inside a function.
             where_parts.append(
                 f"""
                 TSFT.facetvector @@ to_tsquery(
-                    {quote_to_use_in_sql}{'&'.join(ts_vector_parts)}{quote_to_use_in_sql}
+                    '{'&'.join(ts_vector_parts)}'
                 )
             """
             )
 
         if text_search:
             ts_config = self._cw.vreg.config["text-search-config"]
             query = convert_to_tsquery(text_search)
             if ts_config:
                 where_parts.append(
                     f"""
                     to_tsquery(
-                        {quote_to_use_in_sql}{ts_config}{quote_to_use_in_sql},
-                        {quote_to_use_in_sql}{query}{quote_to_use_in_sql}
+                        '{ts_config}',
+                        '{query}'
                     ) @@ TSFT.textsearchvector
                 """
                 )
             else:
                 where_parts.append(
                     f"""
-                    to_tsquery({quote_to_use_in_sql}{query}{quote_to_use_in_sql})
+                    to_tsquery('{query}')
                     @@ TSFT.textsearchvector
                 """
                 )
 
         if where_parts:
             where = f"WHERE {' AND '.join(where_parts)}"
         else:
@@ -260,52 +259,65 @@
         :param rql_args: arguments for base_rql.
         :param text_search: a string to filter results.
         :return: a CubicWeb ResultSet.
         """
         if not (text_search or selected_facets):
             return self._cw.execute(base_rql, rql_args)
         rql_args = rql_args or {}
-        sql_restriction_part, where_sql_part, sql_args = self._build_sql_parts(
-            base_rql, rql_args, selected_facets, text_search, with_row_nb=True
-        )
-        limit_match = re.search(r"LIMIT \d+", sql_restriction_part)
-        if limit_match:
-            limit_part = limit_match.group(0)
-            sql_restriction_part = sql_restriction_part.replace(limit_part, "")
-        else:
-            limit_part = ""
-        offset_match = re.search(r"OFFSET \d+", sql_restriction_part)
-        if offset_match:
-            offset_part = offset_match.group(0)
-            sql_restriction_part = sql_restriction_part.replace(offset_part, "")
+        ts_vector_parts = self._build_tsvector_parts(selected_facets or {})
+        where_parts = []
+        if ts_vector_parts:
+            where_parts.append(
+                f"""
+                            TSFT.facetvector @@ to_tsquery(
+                                '{'&'.join(ts_vector_parts)}'
+                            )
+                        """
+            )
+        if text_search:
+            ts_config = self._cw.vreg.config["text-search-config"]
+            query = convert_to_tsquery(text_search)
+            if ts_config:
+                where_parts.append(
+                    f"""
+                    to_tsquery(
+                        '{ts_config}',
+                        '{query}'
+                    ) @@ TSFT.textsearchvector
+                """
+                )
+            else:
+                where_parts.append(
+                    f"""
+                    to_tsquery('{query}')
+                    @@ TSFT.textsearchvector
+                """
+                )
+        if where_parts:
+            tsft_where = " AND ".join(where_parts)
         else:
-            offset_part = ""
+            tsft_where = ""
+        sql_generator = TSFacetsSQLGenerator(
+            self._cw.cnx.vreg.schema,
+            self._cw.cnx.repo.system_source.dbhelper,
+            tsft_table=self.table_name,
+            tsft_where=tsft_where,
+        )
+        sql, sql_args = convert_rql_to_sql(
+            self._cw.cnx, base_rql, rql_args, sql_generator=sql_generator
+        )
 
         crs = self._cw.cnx.system_sql(
-            f"""
-            SELECT
-                _TABLE_FROM_RQL.*
-            FROM
-                {self.table_name} as TSFT
-                {sql_restriction_part}
-            {where_sql_part}
-            ORDER BY _TABLE_FROM_RQL.row_nb
-            {limit_part}
-            {offset_part}
-            """,
+            sql,
             {
                 **sql_args,
                 **rql_args,
             },
         )
-        raw_results = crs.fetchall()
-        results = []
-        for row in raw_results:
-            # we remove row_nb
-            results.append(row[:-1])
+        results = crs.fetchall()
         description = build_rset_descr(self._cw, base_rql, rql_args, results)
         rset = ResultSet(results, base_rql, rql_args, description)
         rset.req = self._cw
         return rset
 
     def get_id_to_value_mapping(self, facet_key: str) -> Union[Dict[str, str], None]:
         """
```

### Comparing `cubicweb-tsfacets-0.5.3/cubicweb_tsfacets.egg-info/PKG-INFO` & `cubicweb-tsfacets-0.6.0/cubicweb_tsfacets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-tsfacets
-Version: 0.5.3
+Version: 0.6.0
 Summary: This cube implements facets using postgresql text search vectors.
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/tsfacets
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: JavaScript
 Description-Content-Type: text/markdown
 
 Summary
@@ -83,9 +82,7 @@
     }
 
     target_etypes = {"Performance"}
 ```
 
 Thus, `CubicWeb-TSFacets` will provide the methods we will need to
 build our interface.
-
-
```

### Comparing `cubicweb-tsfacets-0.5.3/cubicweb_tsfacets.egg-info/SOURCES.txt` & `cubicweb-tsfacets-0.6.0/cubicweb_tsfacets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.5.3/setup.py` & `cubicweb-tsfacets-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.5.3/test/test_tsfacets.py` & `cubicweb-tsfacets-0.6.0/test/test_tsfacets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-tsfacets-0.5.3/tox.ini` & `cubicweb-tsfacets-0.6.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 deps =
   black >= 19.10b0
 commands = black .
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
```

