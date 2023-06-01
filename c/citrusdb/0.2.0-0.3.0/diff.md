# Comparing `tmp/citrusdb-0.2.0.tar.gz` & `tmp/citrusdb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citrusdb-0.2.0.tar", last modified: Fri May  5 19:00:03 2023, max compression
+gzip compressed data, was "citrusdb-0.3.0.tar", last modified: Thu Jun  1 13:26:10 2023, max compression
```

## Comparing `citrusdb-0.2.0.tar` & `citrusdb-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-05-05 19:00:03.677889 citrusdb-0.2.0/
--rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.2.0/LICENSE
--rw-r--r--   0 debabrata   (501) staff       (20)      690 2023-05-05 19:00:03.677761 citrusdb-0.2.0/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)      181 2023-04-21 09:07:38.000000 citrusdb-0.2.0/README.md
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-05-05 19:00:03.676127 citrusdb-0.2.0/citrusdb/
--rw-r--r--   0 debabrata   (501) staff       (20)       81 2023-04-21 10:45:02.000000 citrusdb-0.2.0/citrusdb/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-05-05 19:00:03.677096 citrusdb-0.2.0/citrusdb/api/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-15 19:33:43.000000 citrusdb-0.2.0/citrusdb/api/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     4620 2023-05-05 18:46:52.000000 citrusdb-0.2.0/citrusdb/api/local.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-05-05 19:00:03.675249 citrusdb-0.2.0/citrusdb/db/
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-05-05 19:00:03.677353 citrusdb-0.2.0/citrusdb/db/index/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-15 19:03:22.000000 citrusdb-0.2.0/citrusdb/db/index/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1478 2023-05-05 18:46:52.000000 citrusdb-0.2.0/citrusdb/db/index/hnswlib.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-05-05 19:00:03.677589 citrusdb-0.2.0/citrusdb/embedding/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-17 05:54:34.000000 citrusdb-0.2.0/citrusdb/embedding/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-05 18:46:52.000000 citrusdb-0.2.0/citrusdb/embedding/openai.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-05-05 19:00:03.676832 citrusdb-0.2.0/citrusdb.egg-info/
--rw-r--r--   0 debabrata   (501) staff       (20)      690 2023-05-05 19:00:03.000000 citrusdb-0.2.0/citrusdb.egg-info/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)      387 2023-05-05 19:00:03.000000 citrusdb-0.2.0/citrusdb.egg-info/SOURCES.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-05-05 19:00:03.000000 citrusdb-0.2.0/citrusdb.egg-info/dependency_links.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       40 2023-05-05 19:00:03.000000 citrusdb-0.2.0/citrusdb.egg-info/requires.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        9 2023-05-05 19:00:03.000000 citrusdb-0.2.0/citrusdb.egg-info/top_level.txt
--rw-r--r--   0 debabrata   (501) staff       (20)      598 2023-05-05 18:55:40.000000 citrusdb-0.2.0/pyproject.toml
--rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-05-05 19:00:03.677924 citrusdb-0.2.0/setup.cfg
--rw-r--r--   0 debabrata   (501) staff       (20)      771 2023-05-05 18:55:26.000000 citrusdb-0.2.0/setup.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.128952 citrusdb-0.3.0/
+-rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.3.0/LICENSE
+-rw-r--r--   0 debabrata   (501) staff       (20)     2175 2023-06-01 13:26:10.128769 citrusdb-0.3.0/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)     1666 2023-06-01 13:10:08.000000 citrusdb-0.3.0/README.md
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.125799 citrusdb-0.3.0/citrusdb/
+-rw-r--r--   0 debabrata   (501) staff       (20)      166 2023-06-01 13:09:38.000000 citrusdb-0.3.0/citrusdb/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.127263 citrusdb-0.3.0/citrusdb/api/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.0/citrusdb/api/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     3969 2023-06-01 13:09:38.000000 citrusdb-0.3.0/citrusdb/api/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     5708 2023-06-01 13:09:38.000000 citrusdb-0.3.0/citrusdb/api/local.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.124397 citrusdb-0.3.0/citrusdb/db/
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.127632 citrusdb-0.3.0/citrusdb/db/index/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.0/citrusdb/db/index/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-01 13:09:38.000000 citrusdb-0.3.0/citrusdb/db/index/hnswlib.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.127985 citrusdb-0.3.0/citrusdb/embedding/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.0/citrusdb/embedding/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.3.0/citrusdb/embedding/openai.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.128544 citrusdb-0.3.0/citrusdb/utils/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 13:09:38.000000 citrusdb-0.3.0/citrusdb/utils/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      205 2023-06-01 13:09:38.000000 citrusdb-0.3.0/citrusdb/utils/types.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      663 2023-06-01 13:09:38.000000 citrusdb-0.3.0/citrusdb/utils/utils.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-01 13:26:10.126756 citrusdb-0.3.0/citrusdb.egg-info/
+-rw-r--r--   0 debabrata   (501) staff       (20)     2175 2023-06-01 13:26:10.000000 citrusdb-0.3.0/citrusdb.egg-info/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)      484 2023-06-01 13:26:10.000000 citrusdb-0.3.0/citrusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-06-01 13:26:10.000000 citrusdb-0.3.0/citrusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       40 2023-06-01 13:26:10.000000 citrusdb-0.3.0/citrusdb.egg-info/requires.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        9 2023-06-01 13:26:10.000000 citrusdb-0.3.0/citrusdb.egg-info/top_level.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)      598 2023-06-01 13:22:53.000000 citrusdb-0.3.0/pyproject.toml
+-rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-06-01 13:26:10.129004 citrusdb-0.3.0/setup.cfg
+-rw-r--r--   0 debabrata   (501) staff       (20)      771 2023-06-01 13:23:08.000000 citrusdb-0.3.0/setup.py
```

### Comparing `citrusdb-0.2.0/LICENSE` & `citrusdb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `citrusdb-0.2.0/citrusdb/db/index/hnswlib.py` & `citrusdb-0.3.0/citrusdb/db/index/hnswlib.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,27 +21,30 @@
         # Increase index size
         if curr_elements + len(data) > max_elements:
             new_size = max(curr_elements + len(data), 2 * max_elements)
             self._index.resize_index(new_size)
 
         self._index.add_items(data, ids, replace_deleted)
 
-    def knn_query(self, query_embeddings, k=1):
-        labels, distances = self._index.knn_query(query_embeddings, k)
+    def knn_query(self, query_embeddings, k=1, filter_function=None):
+        labels, distances = self._index.knn_query(query_embeddings, k, filter=filter_function)
         return labels, distances
 
     def set_ef(self, ef: int):
         self._index.set_ef(ef)
 
     def get_dimension(self):
         return self._index.dim
 
     def load_index(self, path: str, allow_replace_deleted=False):
         self._index.load_index(path, allow_replace_deleted=allow_replace_deleted)
 
+    def mark_deleted(self, label: int):
+        self._index.mark_deleted(label)
+
     def save_index(self, path: str):
         self._index.save_index(path)
 
     def get_status(self):
         print("Max elements", self._index.max_elements)
         print("Current elements", self._index.element_count)
```

### Comparing `citrusdb-0.2.0/pyproject.toml` & `citrusdb-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "citrusdb"
-version = "0.2.0"
+version = "0.3.0"
 
 authors = [
   { name="Debabrata Mondal", email="debabrata.js@protonmail.com" },
 ]
 description = "citrus."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `citrusdb-0.2.0/setup.py` & `citrusdb-0.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="citrusdb",
-    version="0.2.0",
+    version="0.3.0",
     author="Debabrata Mondal",
     author_email="debabrata.js@protonmail.com",
     description="(distributed) vector database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/0xDebabrata/citrus",
     packages=find_packages(exclude=["demo"]),
```

