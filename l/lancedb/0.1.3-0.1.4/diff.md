# Comparing `tmp/lancedb-0.1.3.tar.gz` & `tmp/lancedb-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lancedb-0.1.3.tar", last modified: Thu May 25 23:58:40 2023, max compression
+gzip compressed data, was "lancedb-0.1.4.tar", last modified: Thu Jun  1 03:20:34 2023, max compression
```

## Comparing `lancedb-0.1.3.tar` & `lancedb-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-05-25 23:58:40.888496 lancedb-0.1.3/
--rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-05-25 23:58:40.888410 lancedb-0.1.3/PKG-INFO
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-05-25 23:58:40.887747 lancedb-0.1.3/lancedb/
--rw-r--r--   0 changshe   (501) staff       (20)      922 2023-05-05 18:26:36.000000 lancedb-0.1.3/lancedb/__init__.py
--rw-r--r--   0 changshe   (501) staff       (20)      889 2023-05-05 18:26:36.000000 lancedb-0.1.3/lancedb/common.py
--rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-05-05 01:55:15.000000 lancedb-0.1.3/lancedb/context.py
--rw-r--r--   0 changshe   (501) staff       (20)     3377 2023-05-05 18:26:36.000000 lancedb-0.1.3/lancedb/db.py
--rw-r--r--   0 changshe   (501) staff       (20)     3758 2023-05-05 18:26:42.000000 lancedb-0.1.3/lancedb/embeddings.py
--rw-r--r--   0 changshe   (501) staff       (20)     3836 2023-05-25 23:57:48.000000 lancedb-0.1.3/lancedb/fts.py
--rw-r--r--   0 changshe   (501) staff       (20)     4872 2023-05-25 23:57:48.000000 lancedb-0.1.3/lancedb/query.py
--rw-r--r--   0 changshe   (501) staff       (20)     8833 2023-05-25 04:41:19.000000 lancedb-0.1.3/lancedb/table.py
--rw-r--r--   0 changshe   (501) staff       (20)     1376 2023-05-05 01:55:15.000000 lancedb-0.1.3/lancedb/util.py
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-05-25 23:58:40.888248 lancedb-0.1.3/lancedb.egg-info/
--rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-05-25 23:58:40.000000 lancedb-0.1.3/lancedb.egg-info/PKG-INFO
--rw-r--r--   0 changshe   (501) staff       (20)      335 2023-05-25 23:58:40.000000 lancedb-0.1.3/lancedb.egg-info/SOURCES.txt
--rw-r--r--   0 changshe   (501) staff       (20)        1 2023-05-25 23:58:40.000000 lancedb-0.1.3/lancedb.egg-info/dependency_links.txt
--rw-r--r--   0 changshe   (501) staff       (20)      151 2023-05-25 23:58:40.000000 lancedb-0.1.3/lancedb.egg-info/requires.txt
--rw-r--r--   0 changshe   (501) staff       (20)        8 2023-05-25 23:58:40.000000 lancedb-0.1.3/lancedb.egg-info/top_level.txt
--rw-r--r--   0 changshe   (501) staff       (20)     1333 2023-05-25 23:57:48.000000 lancedb-0.1.3/pyproject.toml
--rw-r--r--   0 changshe   (501) staff       (20)       38 2023-05-25 23:58:40.888527 lancedb-0.1.3/setup.cfg
--rw-r--r--   0 changshe   (501) staff       (20)      660 2023-05-05 01:55:15.000000 lancedb-0.1.3/setup.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-01 03:20:34.444041 lancedb-0.1.4/
+-rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-06-01 03:20:34.443940 lancedb-0.1.4/PKG-INFO
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-01 03:20:34.443133 lancedb-0.1.4/lancedb/
+-rw-r--r--   0 changshe   (501) staff       (20)      922 2023-05-05 18:26:36.000000 lancedb-0.1.4/lancedb/__init__.py
+-rw-r--r--   0 changshe   (501) staff       (20)      889 2023-05-05 18:26:36.000000 lancedb-0.1.4/lancedb/common.py
+-rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-05-05 01:55:15.000000 lancedb-0.1.4/lancedb/context.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3377 2023-05-05 18:26:36.000000 lancedb-0.1.4/lancedb/db.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3758 2023-05-05 18:26:42.000000 lancedb-0.1.4/lancedb/embeddings.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3836 2023-05-25 23:57:48.000000 lancedb-0.1.4/lancedb/fts.py
+-rw-r--r--   0 changshe   (501) staff       (20)     4872 2023-05-25 23:57:48.000000 lancedb-0.1.4/lancedb/query.py
+-rw-r--r--   0 changshe   (501) staff       (20)     8833 2023-05-25 04:41:19.000000 lancedb-0.1.4/lancedb/table.py
+-rw-r--r--   0 changshe   (501) staff       (20)     1376 2023-05-05 01:55:15.000000 lancedb-0.1.4/lancedb/util.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-01 03:20:34.443781 lancedb-0.1.4/lancedb.egg-info/
+-rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-06-01 03:20:34.000000 lancedb-0.1.4/lancedb.egg-info/PKG-INFO
+-rw-r--r--   0 changshe   (501) staff       (20)      335 2023-06-01 03:20:34.000000 lancedb-0.1.4/lancedb.egg-info/SOURCES.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        1 2023-06-01 03:20:34.000000 lancedb-0.1.4/lancedb.egg-info/dependency_links.txt
+-rw-r--r--   0 changshe   (501) staff       (20)      151 2023-06-01 03:20:34.000000 lancedb-0.1.4/lancedb.egg-info/requires.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        8 2023-06-01 03:20:34.000000 lancedb-0.1.4/lancedb.egg-info/top_level.txt
+-rw-r--r--   0 changshe   (501) staff       (20)     1333 2023-06-01 03:10:24.000000 lancedb-0.1.4/pyproject.toml
+-rw-r--r--   0 changshe   (501) staff       (20)       38 2023-06-01 03:20:34.444085 lancedb-0.1.4/setup.cfg
+-rw-r--r--   0 changshe   (501) staff       (20)      660 2023-05-05 01:55:15.000000 lancedb-0.1.4/setup.py
```

### Comparing `lancedb-0.1.3/PKG-INFO` & `lancedb-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1.3
+Version: 0.1.4
 Summary: lancedb
 Author-email: LanceDB Devs <dev@lancedb.com>
 Project-URL: repository, https://github.com/eto-ai/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.1.3/lancedb/__init__.py` & `lancedb-0.1.4/lancedb/__init__.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.3/lancedb/common.py` & `lancedb-0.1.4/lancedb/common.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.3/lancedb/context.py` & `lancedb-0.1.4/lancedb/context.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.3/lancedb/db.py` & `lancedb-0.1.4/lancedb/db.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.3/lancedb/embeddings.py` & `lancedb-0.1.4/lancedb/embeddings.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.3/lancedb/fts.py` & `lancedb-0.1.4/lancedb/fts.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.3/lancedb/query.py` & `lancedb-0.1.4/lancedb/query.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.3/lancedb/table.py` & `lancedb-0.1.4/lancedb/table.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.3/lancedb/util.py` & `lancedb-0.1.4/lancedb/util.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.3/lancedb.egg-info/PKG-INFO` & `lancedb-0.1.4/lancedb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1.3
+Version: 0.1.4
 Summary: lancedb
 Author-email: LanceDB Devs <dev@lancedb.com>
 Project-URL: repository, https://github.com/eto-ai/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.1.3/pyproject.toml` & `lancedb-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "lancedb"
-version = "0.1.3"
-dependencies = ["pylance>=0.4.15", "ratelimiter", "retry", "tqdm"]
+version = "0.1.4"
+dependencies = ["pylance>=0.4.17", "ratelimiter", "retry", "tqdm"]
 description = "lancedb"
 authors = [
     { name = "LanceDB Devs", email = "dev@lancedb.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `lancedb-0.1.3/setup.py` & `lancedb-0.1.4/setup.py`

 * *Files identical despite different names*

