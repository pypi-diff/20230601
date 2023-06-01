# Comparing `tmp/tigrisdb-1.0.0b3.tar.gz` & `tmp/tigrisdb-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigrisdb-1.0.0b3.tar", max compression
+gzip compressed data, was "tigrisdb-1.0.0b4.tar", max compression
```

## Comparing `tigrisdb-1.0.0b3.tar` & `tigrisdb-1.0.0b4.tar`

### file list

```diff
@@ -1,49 +1,51 @@
--rw-r--r--   0        0        0    11357 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/LICENSE
--rw-r--r--   0        0        0      935 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/README.md
--rw-r--r--   0        0        0     1583 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      313 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     1897 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/field_behavior_pb2.py
--rw-r--r--   0        0        0      685 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/field_behavior_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/field_behavior_pb2_grpc.py
--rw-r--r--   0        0        0     2125 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/http_pb2.py
--rw-r--r--   0        0        0     2272 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0     1507 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/httpbody_pb2.py
--rw-r--r--   0        0        0      882 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/httpbody_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/google/api/httpbody_pb2_grpc.py
--rw-r--r--   0        0        0    27129 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/openapiv3/OpenAPIv3_pb2.py
--rw-r--r--   0        0        0    49576 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/openapiv3/OpenAPIv3_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/openapiv3/OpenAPIv3_pb2_grpc.py
--rw-r--r--   0        0        0     2102 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/openapiv3/annotations_pb2.py
--rw-r--r--   0        0        0      555 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/openapiv3/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/openapiv3/annotations_pb2_grpc.py
--rw-r--r--   0        0        0    44365 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/api_pb2.py
--rw-r--r--   0        0        0    37886 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/api_pb2.pyi
--rw-r--r--   0        0        0    51527 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/api_pb2_grpc.py
--rw-r--r--   0        0        0     7946 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/auth_pb2.py
--rw-r--r--   0        0        0     6220 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/auth_pb2.pyi
--rw-r--r--   0        0        0    11198 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/auth_pb2_grpc.py
--rw-r--r--   0        0        0     9308 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/server/v1/observability_pb2.py
--rw-r--r--   0        0        0     8458 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/server/v1/observability_pb2.pyi
--rw-r--r--   0        0        0     7981 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/observability_pb2_grpc.py
--rw-r--r--   0        0        0    14625 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/search_pb2.py
--rw-r--r--   0        0        0    11907 2023-05-24 01:28:39.520574 tigrisdb-1.0.0b3/api/generated/server/v1/search_pb2.pyi
--rw-r--r--   0        0        0    23238 2023-05-24 01:28:39.524574 tigrisdb-1.0.0b3/api/generated/server/v1/search_pb2_grpc.py
--rw-r--r--   0        0        0     1147 2023-05-24 01:28:43.288538 tigrisdb-1.0.0b3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/__init__.py
--rw-r--r--   0        0        0     2799 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/auth.py
--rw-r--r--   0        0        0     2333 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/client.py
--rw-r--r--   0        0        0     1968 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/collection.py
--rw-r--r--   0        0        0     1986 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/database.py
--rw-r--r--   0        0        0      484 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/errors.py
--rw-r--r--   0        0        0     1860 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/search.py
--rw-r--r--   0        0        0     4587 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/search_index.py
--rw-r--r--   0        0        0      554 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/types/__init__.py
--rw-r--r--   0        0        0      267 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/types/filters/__init__.py
--rw-r--r--   0        0        0      704 2023-05-24 01:28:02.692903 tigrisdb-1.0.0b3/tigrisdb/types/filters/logical.py
--rw-r--r--   0        0        0     1132 2023-05-24 01:28:02.696903 tigrisdb-1.0.0b3/tigrisdb/types/filters/selector.py
--rw-r--r--   0        0        0     8903 2023-05-24 01:28:02.696903 tigrisdb-1.0.0b3/tigrisdb/types/search.py
--rw-r--r--   0        0        0      487 2023-05-24 01:28:02.696903 tigrisdb-1.0.0b3/tigrisdb/types/sort.py
--rw-r--r--   0        0        0     1092 2023-05-24 01:28:02.696903 tigrisdb-1.0.0b3/tigrisdb/utils.py
--rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 tigrisdb-1.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 01:24:06.221088 tigrisdb-1.0.0b4/LICENSE
+-rw-r--r--   0        0        0      935 2023-06-01 01:24:06.221088 tigrisdb-1.0.0b4/README.md
+-rw-r--r--   0        0        0     1583 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      313 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     1897 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/google/api/field_behavior_pb2.py
+-rw-r--r--   0        0        0      685 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/google/api/field_behavior_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/google/api/field_behavior_pb2_grpc.py
+-rw-r--r--   0        0        0     2125 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/google/api/http_pb2.py
+-rw-r--r--   0        0        0     2272 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0     1507 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/google/api/httpbody_pb2.py
+-rw-r--r--   0        0        0      882 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/google/api/httpbody_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/google/api/httpbody_pb2_grpc.py
+-rw-r--r--   0        0        0    27129 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/openapiv3/OpenAPIv3_pb2.py
+-rw-r--r--   0        0        0    49576 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/openapiv3/OpenAPIv3_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/openapiv3/OpenAPIv3_pb2_grpc.py
+-rw-r--r--   0        0        0     2102 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/openapiv3/annotations_pb2.py
+-rw-r--r--   0        0        0      555 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/openapiv3/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/openapiv3/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0    44365 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/server/v1/api_pb2.py
+-rw-r--r--   0        0        0    37886 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/server/v1/api_pb2.pyi
+-rw-r--r--   0        0        0    51527 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/server/v1/api_pb2_grpc.py
+-rw-r--r--   0        0        0     7946 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/server/v1/auth_pb2.py
+-rw-r--r--   0        0        0     6220 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/server/v1/auth_pb2.pyi
+-rw-r--r--   0        0        0    11198 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/server/v1/auth_pb2_grpc.py
+-rw-r--r--   0        0        0     9308 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/server/v1/observability_pb2.py
+-rw-r--r--   0        0        0     8458 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/server/v1/observability_pb2.pyi
+-rw-r--r--   0        0        0     7981 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/server/v1/observability_pb2_grpc.py
+-rw-r--r--   0        0        0    14625 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/server/v1/search_pb2.py
+-rw-r--r--   0        0        0    11907 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/server/v1/search_pb2.pyi
+-rw-r--r--   0        0        0    23238 2023-06-01 01:24:46.381455 tigrisdb-1.0.0b4/api/generated/server/v1/search_pb2_grpc.py
+-rw-r--r--   0        0        0     1147 2023-06-01 01:24:50.261477 tigrisdb-1.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/__init__.py
+-rw-r--r--   0        0        0     2799 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/auth.py
+-rw-r--r--   0        0        0     2785 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/client.py
+-rw-r--r--   0        0        0     1968 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/collection.py
+-rw-r--r--   0        0        0     1986 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/database.py
+-rw-r--r--   0        0        0      774 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/errors.py
+-rw-r--r--   0        0        0     1860 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/search.py
+-rw-r--r--   0        0        0     4587 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/search_index.py
+-rw-r--r--   0        0        0      559 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/types/__init__.py
+-rw-r--r--   0        0        0      267 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/types/filters/__init__.py
+-rw-r--r--   0        0        0      704 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/types/filters/logical.py
+-rw-r--r--   0        0        0     1132 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/types/filters/selector.py
+-rw-r--r--   0        0        0     8873 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/types/search.py
+-rw-r--r--   0        0        0      487 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/types/sort.py
+-rw-r--r--   0        0        0      606 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/types/vector.py
+-rw-r--r--   0        0        0     1092 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/utils.py
+-rw-r--r--   0        0        0     4539 2023-06-01 01:24:06.225088 tigrisdb-1.0.0b4/tigrisdb/vector_store.py
+-rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 tigrisdb-1.0.0b4/PKG-INFO
```

### Comparing `tigrisdb-1.0.0b3/LICENSE` & `tigrisdb-1.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/README.md` & `tigrisdb-1.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/google/api/annotations_pb2.py` & `tigrisdb-1.0.0b4/api/generated/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/google/api/field_behavior_pb2.py` & `tigrisdb-1.0.0b4/api/generated/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/google/api/field_behavior_pb2.pyi` & `tigrisdb-1.0.0b4/api/generated/google/api/field_behavior_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/google/api/http_pb2.py` & `tigrisdb-1.0.0b4/api/generated/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/google/api/http_pb2.pyi` & `tigrisdb-1.0.0b4/api/generated/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/google/api/httpbody_pb2.py` & `tigrisdb-1.0.0b4/api/generated/google/api/httpbody_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/google/api/httpbody_pb2.pyi` & `tigrisdb-1.0.0b4/api/generated/google/api/httpbody_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/openapiv3/OpenAPIv3_pb2.py` & `tigrisdb-1.0.0b4/api/generated/openapiv3/OpenAPIv3_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/openapiv3/OpenAPIv3_pb2.pyi` & `tigrisdb-1.0.0b4/api/generated/openapiv3/OpenAPIv3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/openapiv3/annotations_pb2.py` & `tigrisdb-1.0.0b4/api/generated/openapiv3/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/openapiv3/annotations_pb2.pyi` & `tigrisdb-1.0.0b4/api/generated/openapiv3/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/server/v1/api_pb2.py` & `tigrisdb-1.0.0b4/api/generated/server/v1/api_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/server/v1/api_pb2.pyi` & `tigrisdb-1.0.0b4/api/generated/server/v1/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/server/v1/api_pb2_grpc.py` & `tigrisdb-1.0.0b4/api/generated/server/v1/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/server/v1/auth_pb2.py` & `tigrisdb-1.0.0b4/api/generated/server/v1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/server/v1/auth_pb2.pyi` & `tigrisdb-1.0.0b4/api/generated/server/v1/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/server/v1/auth_pb2_grpc.py` & `tigrisdb-1.0.0b4/api/generated/server/v1/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/server/v1/observability_pb2.py` & `tigrisdb-1.0.0b4/api/generated/server/v1/observability_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/server/v1/observability_pb2.pyi` & `tigrisdb-1.0.0b4/api/generated/server/v1/observability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/server/v1/observability_pb2_grpc.py` & `tigrisdb-1.0.0b4/api/generated/server/v1/observability_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/server/v1/search_pb2.py` & `tigrisdb-1.0.0b4/api/generated/server/v1/search_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/server/v1/search_pb2.pyi` & `tigrisdb-1.0.0b4/api/generated/server/v1/search_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/api/generated/server/v1/search_pb2_grpc.py` & `tigrisdb-1.0.0b4/api/generated/server/v1/search_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/pyproject.toml` & `tigrisdb-1.0.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tigrisdb"
-version = "1.0.0-beta.3"
+version = "1.0.0-beta.4"
 description = "Python SDK for Tigris <http://www.tigrisdata.com>"
 authors = ["Tigris team <support@tigrisdata.com>"]
 repository = "https://www.github.com/tigrisdata/tigris-client-python"
 documentation = "https://www.tigrisdata.com/docs/"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `tigrisdb-1.0.0b3/tigrisdb/auth.py` & `tigrisdb-1.0.0b4/tigrisdb/auth.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/tigrisdb/client.py` & `tigrisdb-1.0.0b4/tigrisdb/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,22 +22,32 @@
     def __init__(self, config: Optional[ClientConfig]):
         os.environ["PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION"] = "python"
 
         if not config:
             config = ClientConfig()
         self.__config = config
         if not config.server_url:
-            config.server_url = TigrisClient.__LOCAL_SERVER
+            config.server_url = os.getenv("TIGRIS_URI", TigrisClient.__LOCAL_SERVER)
         if config.server_url.startswith("https://"):
             config.server_url = config.server_url.replace("https://", "")
         if config.server_url.startswith("http://"):
             config.server_url = config.server_url.replace("http://", "")
         if ":" not in config.server_url:
             config.server_url = f"{config.server_url}:443"
 
+        # initialize rest of config
+        if not config.project_name:
+            config.project_name = os.getenv("TIGRIS_PROJECT")
+        if not config.client_id:
+            config.client_id = os.getenv("TIGRIS_CLIENT_ID")
+        if not config.client_secret:
+            config.client_secret = os.getenv("TIGRIS_CLIENT_SECRET")
+        if not config.branch:
+            config.branch = os.getenv("TIGRIS_DB_BRANCH", "")
+
         is_local_dev = any(
             map(
                 lambda k: k in config.server_url,
                 ["localhost", "127.0.0.1", "tigrisdb-local-server:", "[::1]"],
             )
         )
```

### Comparing `tigrisdb-1.0.0b3/tigrisdb/collection.py` & `tigrisdb-1.0.0b4/tigrisdb/collection.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/tigrisdb/database.py` & `tigrisdb-1.0.0b4/tigrisdb/database.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/tigrisdb/search.py` & `tigrisdb-1.0.0b4/tigrisdb/search.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/tigrisdb/search_index.py` & `tigrisdb-1.0.0b4/tigrisdb/search_index.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/tigrisdb/types/__init__.py` & `tigrisdb-1.0.0b4/tigrisdb/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict, Optional, Type
 
 Document: Type[dict] = Dict
 
 
 @dataclass
 class ClientConfig:
-    project_name: str
+    project_name: str = ""
     client_id: Optional[str] = None
     client_secret: Optional[str] = None
     branch: str = ""
     server_url: str = "localhost:8081"
 
 
 class Serializable(abc.ABC):
```

### Comparing `tigrisdb-1.0.0b3/tigrisdb/types/filters/logical.py` & `tigrisdb-1.0.0b4/tigrisdb/types/filters/logical.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/tigrisdb/types/filters/selector.py` & `tigrisdb-1.0.0b4/tigrisdb/types/filters/selector.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/tigrisdb/types/search.py` & `tigrisdb-1.0.0b4/tigrisdb/types/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     field: str
     vector: List[float]
 
     def query(self):
         return {self.field: self.vector}
 
 
-# TODO: add filter, collation
 @dataclass
 class Query:
     q: str = ""
     search_fields: List[str] = field(default_factory=list)
     vector_query: VectorField = None
     filter_by: Optional[Filter] = None
     facet_by: Union[str, List[FacetField]] = field(default_factory=list)
```

### Comparing `tigrisdb-1.0.0b3/tigrisdb/utils.py` & `tigrisdb-1.0.0b4/tigrisdb/utils.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b3/PKG-INFO` & `tigrisdb-1.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigrisdb
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Python SDK for Tigris <http://www.tigrisdata.com>
 Home-page: https://www.github.com/tigrisdata/tigris-client-python
 License: Apache-2.0
 Keywords: database,nosql,vector,search
 Author: Tigris team
 Author-email: support@tigrisdata.com
 Requires-Python: >=3.8,<4.0
```

