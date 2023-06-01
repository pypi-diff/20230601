# Comparing `tmp/cassio-0.0.1.tar.gz` & `tmp/cassio-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cassio-0.0.1.tar", last modified: Tue May 30 20:51:07 2023, max compression
+gzip compressed data, was "cassio-0.0.2.tar", last modified: Thu Jun  1 08:38:58 2023, max compression
```

## Comparing `cassio-0.0.1.tar` & `cassio-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-05-30 20:51:07.956904 cassio-0.0.1/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2779 2023-05-30 20:51:07.956904 cassio-0.0.1/PKG-INFO
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1327 2023-05-30 20:43:53.000000 cassio-0.0.1/README.md
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       78 2023-05-30 20:51:07.956904 cassio-0.0.1/setup.cfg
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1846 2023-05-30 20:51:05.000000 cassio-0.0.1/setup.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-05-30 20:51:07.952904 cassio-0.0.1/src/
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-05-30 20:51:07.956904 cassio-0.0.1/src/cassio/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       35 2023-05-23 20:27:53.000000 cassio-0.0.1/src/cassio/__init__.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-05-30 20:51:07.956904 cassio-0.0.1/src/cassio/db_extractor/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       71 2023-05-19 16:24:14.000000 cassio-0.0.1/src/cassio/db_extractor/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2825 2023-05-23 21:38:32.000000 cassio-0.0.1/src/cassio/db_extractor/cassandra_extractor.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-05-30 20:51:07.956904 cassio-0.0.1/src/cassio/globals/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       43 2023-05-23 20:27:43.000000 cassio-0.0.1/src/cassio/globals/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      349 2023-05-23 20:28:43.000000 cassio-0.0.1/src/cassio/globals/globals.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-05-30 20:51:07.956904 cassio-0.0.1/src/cassio/history/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       64 2023-05-23 00:11:06.000000 cassio-0.0.1/src/cassio/history/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2386 2023-05-23 21:39:10.000000 cassio-0.0.1/src/cassio/history/history_management.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-05-30 20:51:07.956904 cassio-0.0.1/src/cassio/inspection/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       73 2023-05-19 16:24:06.000000 cassio-0.0.1/src/cassio/inspection/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      323 2023-05-19 16:24:34.000000 cassio-0.0.1/src/cassio/inspection/schema.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-05-30 20:51:07.956904 cassio-0.0.1/src/cassio/keyvalue/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       45 2023-05-23 14:40:40.000000 cassio-0.0.1/src/cassio/keyvalue/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     3326 2023-05-25 15:21:39.000000 cassio-0.0.1/src/cassio/keyvalue/kv_cache.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-05-30 20:51:07.956904 cassio-0.0.1/src/cassio/utils/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       50 2023-05-23 21:35:34.000000 cassio-0.0.1/src/cassio/utils/__init__.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-05-30 20:51:07.956904 cassio-0.0.1/src/cassio/utils/vector/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       67 2023-05-23 21:35:29.000000 cassio-0.0.1/src/cassio/utils/vector/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2531 2023-05-24 14:14:55.000000 cassio-0.0.1/src/cassio/utils/vector/distance_metrics.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-05-30 20:51:07.956904 cassio-0.0.1/src/cassio/vector/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       57 2023-05-23 20:58:39.000000 cassio-0.0.1/src/cassio/vector/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     8926 2023-05-25 22:43:01.000000 cassio-0.0.1/src/cassio/vector/vector_db_driver.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-05-30 20:51:07.956904 cassio-0.0.1/src/cassio.egg-info/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2779 2023-05-30 20:51:07.000000 cassio-0.0.1/src/cassio.egg-info/PKG-INFO
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      743 2023-05-30 20:51:07.000000 cassio-0.0.1/src/cassio.egg-info/SOURCES.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        1 2023-05-30 20:51:07.000000 cassio-0.0.1/src/cassio.egg-info/dependency_links.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       36 2023-05-30 20:51:07.000000 cassio-0.0.1/src/cassio.egg-info/requires.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        7 2023-05-30 20:51:07.000000 cassio-0.0.1/src/cassio.egg-info/top_level.txt
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2808 2023-06-01 08:38:58.969094 cassio-0.0.2/PKG-INFO
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1356 2023-05-30 20:52:15.000000 cassio-0.0.2/README.md
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       78 2023-06-01 08:38:58.969094 cassio-0.0.2/setup.cfg
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1846 2023-06-01 08:38:26.000000 cassio-0.0.2/setup.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       35 2023-05-23 20:27:53.000000 cassio-0.0.2/src/cassio/__init__.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/db_extractor/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       71 2023-05-30 22:40:16.000000 cassio-0.0.2/src/cassio/db_extractor/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2825 2023-05-23 21:38:32.000000 cassio-0.0.2/src/cassio/db_extractor/cassandra_extractor.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/globals/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       43 2023-05-23 20:27:43.000000 cassio-0.0.2/src/cassio/globals/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)      349 2023-05-23 20:28:43.000000 cassio-0.0.2/src/cassio/globals/globals.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/history/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       64 2023-05-23 00:11:06.000000 cassio-0.0.2/src/cassio/history/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2386 2023-05-23 21:39:10.000000 cassio-0.0.2/src/cassio/history/history_management.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/inspection/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       73 2023-05-19 16:24:06.000000 cassio-0.0.2/src/cassio/inspection/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)      323 2023-05-30 22:40:16.000000 cassio-0.0.2/src/cassio/inspection/schema.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/keyvalue/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       45 2023-05-23 14:40:40.000000 cassio-0.0.2/src/cassio/keyvalue/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     3326 2023-05-25 15:21:39.000000 cassio-0.0.2/src/cassio/keyvalue/kv_cache.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/utils/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       50 2023-05-23 21:35:34.000000 cassio-0.0.2/src/cassio/utils/__init__.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/utils/vector/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       67 2023-05-23 21:35:29.000000 cassio-0.0.2/src/cassio/utils/vector/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2531 2023-05-24 14:14:55.000000 cassio-0.0.2/src/cassio/utils/vector/distance_metrics.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio/vector/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       57 2023-05-23 20:58:39.000000 cassio-0.0.2/src/cassio/vector/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     9216 2023-05-31 20:59:33.000000 cassio-0.0.2/src/cassio/vector/vector_db_driver.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-01 08:38:58.965094 cassio-0.0.2/src/cassio.egg-info/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2808 2023-06-01 08:38:58.000000 cassio-0.0.2/src/cassio.egg-info/PKG-INFO
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)      743 2023-06-01 08:38:58.000000 cassio-0.0.2/src/cassio.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)        1 2023-06-01 08:38:58.000000 cassio-0.0.2/src/cassio.egg-info/dependency_links.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       36 2023-06-01 08:38:58.000000 cassio-0.0.2/src/cassio.egg-info/requires.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)        7 2023-06-01 08:38:58.000000 cassio-0.0.2/src/cassio.egg-info/top_level.txt
```

### Comparing `cassio-0.0.1/PKG-INFO` & `cassio-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cassio
-Version: 0.0.1
+Version: 0.0.2
 Summary: A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.
 Home-page: https://github.com/hemidactylus/cassio
 Author: Stefano Lottini
 Author-email: stefano.lottini@datastax.com
 License: LICENSE.txt
 Description: # cassIO
         
@@ -36,18 +36,18 @@
         - `pip install -e .` in the LangChain `cassio` branch of [this fork](https://github.com/hemidactylus/langchain/tree/cassio);
         - plus any additional requirement files specific to the examples
         you're running (such as Jupyter).
         
         ### Publishing
         
         ```
+        # (bump version & commit ...)
         python setup.py sdist bdist_wheel
         twine upload dist/*
         # (login to PyPI ...)
-        
         ```
         
         ### Unit testing
         
         In a virtualenv with the `requirements-dev.txt` installed, run:
         
         ```
```

### Comparing `cassio-0.0.1/README.md` & `cassio-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 - `pip install -e .` in the LangChain `cassio` branch of [this fork](https://github.com/hemidactylus/langchain/tree/cassio);
 - plus any additional requirement files specific to the examples
 you're running (such as Jupyter).
 
 ### Publishing
 
 ```
+# (bump version & commit ...)
 python setup.py sdist bdist_wheel
 twine upload dist/*
 # (login to PyPI ...)
-
 ```
 
 ### Unit testing
 
 In a virtualenv with the `requirements-dev.txt` installed, run:
 
 ```
```

### Comparing `cassio-0.0.1/setup.py` & `cassio-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 setup(
     name='cassio',
-    version='0.0.1',
+    version='0.0.2',
     author='Stefano Lottini',
     author_email='stefano.lottini@datastax.com',
     package_dir={"": "src"},
     packages=find_packages(where='src'),
     # entry_points={
     #     "console_scripts": [
     #         "clothesline=clothesline:main",
```

### Comparing `cassio-0.0.1/src/cassio/db_extractor/cassandra_extractor.py` & `cassio-0.0.2/src/cassio/db_extractor/cassandra_extractor.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.1/src/cassio/history/history_management.py` & `cassio-0.0.2/src/cassio/history/history_management.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.1/src/cassio/keyvalue/kv_cache.py` & `cassio-0.0.2/src/cassio/keyvalue/kv_cache.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.1/src/cassio/utils/vector/distance_metrics.py` & `cassio-0.0.2/src/cassio/utils/vector/distance_metrics.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.1/src/cassio/vector/vector_db_driver.py` & `cassio-0.0.2/src/cassio/vector/vector_db_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 """
 
 from operator import itemgetter
 import json
 
 from cassandra.cluster import Session
 from cassandra.query import SimpleStatement
-from cassandra import ReadFailure
+from cassandra.protocol import SyntaxException
 
 from cassio.globals.globals import globals
 from cassio.utils.vector.distance_metrics import distanceMetricsMap
 
 EXPERIMENTAL_VECTOR_SEARCH_ERROR = (
     "Vector search is an experimental feature and should "
     "be first enabled with 'cassio.globals.enableExperimentalVectorSearch()`"
 )
 
 _createVectorDBTableCQLTemplate = """
 CREATE TABLE IF NOT EXISTS {keyspace}.{tableName} (
     document_id {idType} PRIMARY KEY,
-    embedding_vector FLOAT VECTOR[{embeddingDimension}],
+    embedding_vector VECTOR<FLOAT, {embeddingDimension}>,
     document TEXT,
     metadata_blob TEXT
 );
 """
 _createVectorDBTableIndexCQLTemplate = """
 CREATE CUSTOM INDEX IF NOT EXISTS {indexName} ON {keyspace}.{tableName} (embedding_vector)
 USING 'org.apache.cassandra.index.sai.StorageAttachedIndex' ;
@@ -44,21 +44,34 @@
 """
 _getVectorDBTableItemCQLTemplate = """
 SELECT
     document_id, embedding_vector, document, metadata_blob
 FROM {keyspace}.{tableName}
     WHERE document_id=%s;
 """
-_searchVectorDBTableItemCQLTemplate = """
+
+# For some time, this is still the one for Astra DB
+_searchVectorDBTableItemCQLTemplateLegacy = """
 SELECT
     document_id, embedding_vector, document, metadata_blob
 FROM {keyspace}.{tableName}
     WHERE embedding_vector ANN OF %s
     LIMIT %s
+    ALLOW FILTERING;
 """
+# ... while this is the final syntax:
+_searchVectorDBTableItemCQLTemplate = """
+SELECT
+    document_id, embedding_vector, document, metadata_blob
+FROM {keyspace}.{tableName}
+    ORDER BY embedding_vector ANN OF %s
+    LIMIT %s
+    ALLOW FILTERING;
+"""
+
 _truncateVectorDBTableCQLTemplate = """
 TRUNCATE TABLE {keyspace}.{tableName};
 """
 _deleteVectorDBTableItemCQLTemplate = """
 DELETE FROM {keyspace}.{tableName}
 WHERE document_id = %s;
 """
@@ -86,25 +99,21 @@
         """
         try:
             searchVectorDBTableItemCQL = SimpleStatement(_searchVectorDBTableItemCQLTemplate.format(
                 keyspace=self.keyspace,
                 tableName=self.tableName
             ))
             return self._executeCQL(searchVectorDBTableItemCQL, (embedding_vector, numRows))
-        except ReadFailure:
-            # likely a count issue. Let's count the rows (it's a small number)
-            rowCount = self._countRows()
-            if rowCount < numRows:
-                if rowCount:
-                    return self.ANNSearch(embedding_vector, min(numRows, rowCount))
-                else:
-                    return []
-            else:
-                # a repeated error, likely another reason. Reraise
-                raise
+        except SyntaxException as e:
+            # we try the legacy syntax (transitional workaround)
+            searchVectorDBTableItemCQL = SimpleStatement(_searchVectorDBTableItemCQLTemplateLegacy.format(
+                keyspace=self.keyspace,
+                tableName=self.tableName
+            ))
+            return self._executeCQL(searchVectorDBTableItemCQL, (embedding_vector, numRows))
 
     def _countRows(self):
         countRowsCQL = SimpleStatement(_countRowsCQLTemplate.format(
             keyspace=self.keyspace,
             tableName=self.tableName
         ))
         return self._executeCQL(countRowsCQL, tuple()).one().count
```

### Comparing `cassio-0.0.1/src/cassio.egg-info/PKG-INFO` & `cassio-0.0.2/src/cassio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cassio
-Version: 0.0.1
+Version: 0.0.2
 Summary: A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.
 Home-page: https://github.com/hemidactylus/cassio
 Author: Stefano Lottini
 Author-email: stefano.lottini@datastax.com
 License: LICENSE.txt
 Description: # cassIO
         
@@ -36,18 +36,18 @@
         - `pip install -e .` in the LangChain `cassio` branch of [this fork](https://github.com/hemidactylus/langchain/tree/cassio);
         - plus any additional requirement files specific to the examples
         you're running (such as Jupyter).
         
         ### Publishing
         
         ```
+        # (bump version & commit ...)
         python setup.py sdist bdist_wheel
         twine upload dist/*
         # (login to PyPI ...)
-        
         ```
         
         ### Unit testing
         
         In a virtualenv with the `requirements-dev.txt` installed, run:
         
         ```
```

### Comparing `cassio-0.0.1/src/cassio.egg-info/SOURCES.txt` & `cassio-0.0.2/src/cassio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

