# Comparing `tmp/kurve-0.4.tar.gz` & `tmp/kurve-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kurve-0.4.tar", last modified: Thu Jun  1 16:42:03 2023, max compression
+gzip compressed data, was "kurve-0.5.tar", last modified: Thu Jun  1 17:08:12 2023, max compression
```

## Comparing `kurve-0.4.tar` & `kurve-0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-01 16:42:03.789561 kurve-0.4/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     3991 2023-06-01 16:42:03.789418 kurve-0.4/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     2961 2023-05-30 15:59:48.000000 kurve-0.4/README.md
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-01 16:42:03.787085 kurve-0.4/kurve/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2023-05-30 15:52:46.000000 kurve-0.4/kurve/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      739 2023-05-30 15:55:46.000000 kurve-0.4/kurve/base_source.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      203 2023-05-30 15:55:44.000000 kurve-0.4/kurve/cardinality.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    16559 2023-05-30 16:25:27.000000 kurve-0.4/kurve/edge_builder.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     6095 2023-05-30 15:53:24.000000 kurve-0.4/kurve/entity.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      403 2023-05-30 15:50:48.000000 kurve-0.4/kurve/enums.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    18785 2023-05-30 15:54:23.000000 kurve-0.4/kurve/graph.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     1117 2023-05-30 15:54:28.000000 kurve-0.4/kurve/middleware.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-01 16:42:03.788108 kurve-0.4/kurve/models/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      374 2023-05-30 15:54:35.000000 kurve-0.4/kurve/models/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    40236 2023-05-30 15:55:35.000000 kurve-0.4/kurve/sources.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      182 2023-05-30 15:55:38.000000 kurve-0.4/kurve/util.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-01 16:42:03.787982 kurve-0.4/kurve.egg-info/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     3991 2023-06-01 16:42:03.000000 kurve-0.4/kurve.egg-info/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      501 2023-06-01 16:42:03.000000 kurve-0.4/kurve.egg-info/SOURCES.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-01 16:42:03.000000 kurve-0.4/kurve.egg-info/dependency_links.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-05-30 16:01:25.000000 kurve-0.4/kurve.egg-info/not-zip-safe
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     6656 2023-06-01 16:42:03.000000 kurve-0.4/kurve.egg-info/requires.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        6 2023-06-01 16:42:03.000000 kurve-0.4/kurve.egg-info/top_level.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-06-01 16:42:03.789595 kurve-0.4/setup.cfg
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     2162 2023-06-01 16:40:59.000000 kurve-0.4/setup.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-01 16:42:03.789115 kurve-0.4/tests/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      523 2023-05-30 15:51:34.000000 kurve-0.4/tests/test_bigquery_graph.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      764 2023-05-30 15:51:41.000000 kurve-0.4/tests/test_local_graph.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      878 2023-05-30 15:51:48.000000 kurve-0.4/tests/test_postgres_graph.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      786 2023-05-30 15:51:54.000000 kurve-0.4/tests/test_s3_graph.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-01 17:08:12.662309 kurve-0.5/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     3970 2023-06-01 17:08:12.662180 kurve-0.5/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     2961 2023-05-30 15:59:48.000000 kurve-0.5/README.md
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-01 17:08:12.660378 kurve-0.5/kurve/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2023-05-30 15:52:46.000000 kurve-0.5/kurve/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      739 2023-05-30 15:55:46.000000 kurve-0.5/kurve/base_source.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      203 2023-05-30 15:55:44.000000 kurve-0.5/kurve/cardinality.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    16559 2023-05-30 16:25:27.000000 kurve-0.5/kurve/edge_builder.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     6095 2023-05-30 15:53:24.000000 kurve-0.5/kurve/entity.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      403 2023-05-30 15:50:48.000000 kurve-0.5/kurve/enums.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    18785 2023-05-30 15:54:23.000000 kurve-0.5/kurve/graph.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     1117 2023-05-30 15:54:28.000000 kurve-0.5/kurve/middleware.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-01 17:08:12.661189 kurve-0.5/kurve/models/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      374 2023-05-30 15:54:35.000000 kurve-0.5/kurve/models/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    40236 2023-05-30 15:55:35.000000 kurve-0.5/kurve/sources.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      182 2023-05-30 15:55:38.000000 kurve-0.5/kurve/util.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-01 17:08:12.661090 kurve-0.5/kurve.egg-info/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     3970 2023-06-01 17:08:12.000000 kurve-0.5/kurve.egg-info/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      501 2023-06-01 17:08:12.000000 kurve-0.5/kurve.egg-info/SOURCES.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-01 17:08:12.000000 kurve-0.5/kurve.egg-info/dependency_links.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-05-30 16:01:25.000000 kurve-0.5/kurve.egg-info/not-zip-safe
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      361 2023-06-01 17:08:12.000000 kurve-0.5/kurve.egg-info/requires.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        6 2023-06-01 17:08:12.000000 kurve-0.5/kurve.egg-info/top_level.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-06-01 17:08:12.662341 kurve-0.5/setup.cfg
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     2285 2023-06-01 17:07:59.000000 kurve-0.5/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-01 17:08:12.661924 kurve-0.5/tests/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      523 2023-05-30 15:51:34.000000 kurve-0.5/tests/test_bigquery_graph.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      764 2023-05-30 15:51:41.000000 kurve-0.5/tests/test_local_graph.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      878 2023-05-30 15:51:48.000000 kurve-0.5/tests/test_postgres_graph.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      786 2023-05-30 15:51:54.000000 kurve-0.5/tests/test_s3_graph.py
```

### Comparing `kurve-0.4/PKG-INFO` & `kurve-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kurve
-Version: 0.4
+Version: 0.5
 Summary: An interface for dynamic entity linking with graphs as the backend for arbitrary data sources.
 Home-page: https://github.com/kurveai/kurve
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/kurveai/kurve
 Project-URL: Issue Tracker, https://github.com/kurveai/kurve/issues
@@ -15,15 +15,14 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
-Provides-Extra: base
 
 # kurve
 
 ## Functionality
 
 A library for turning data entities into a graph.  The entities
 can be files or RDBMS, depending on which connectors we're supporting
```

### Comparing `kurve-0.4/README.md` & `kurve-0.5/README.md`

 * *Files identical despite different names*

### Comparing `kurve-0.4/kurve/base_source.py` & `kurve-0.5/kurve/base_source.py`

 * *Files identical despite different names*

### Comparing `kurve-0.4/kurve/edge_builder.py` & `kurve-0.5/kurve/edge_builder.py`

 * *Files identical despite different names*

### Comparing `kurve-0.4/kurve/entity.py` & `kurve-0.5/kurve/entity.py`

 * *Files identical despite different names*

### Comparing `kurve-0.4/kurve/graph.py` & `kurve-0.5/kurve/graph.py`

 * *Files identical despite different names*

### Comparing `kurve-0.4/kurve/middleware.py` & `kurve-0.5/kurve/middleware.py`

 * *Files identical despite different names*

### Comparing `kurve-0.4/kurve/sources.py` & `kurve-0.5/kurve/sources.py`

 * *Files identical despite different names*

### Comparing `kurve-0.4/kurve.egg-info/PKG-INFO` & `kurve-0.5/kurve.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kurve
-Version: 0.4
+Version: 0.5
 Summary: An interface for dynamic entity linking with graphs as the backend for arbitrary data sources.
 Home-page: https://github.com/kurveai/kurve
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/kurveai/kurve
 Project-URL: Issue Tracker, https://github.com/kurveai/kurve/issues
@@ -15,15 +15,14 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
-Provides-Extra: base
 
 # kurve
 
 ## Functionality
 
 A library for turning data entities into a graph.  The entities
 can be files or RDBMS, depending on which connectors we're supporting
```

### Comparing `kurve-0.4/tests/test_bigquery_graph.py` & `kurve-0.5/tests/test_bigquery_graph.py`

 * *Files identical despite different names*

### Comparing `kurve-0.4/tests/test_local_graph.py` & `kurve-0.5/tests/test_local_graph.py`

 * *Files identical despite different names*

### Comparing `kurve-0.4/tests/test_postgres_graph.py` & `kurve-0.5/tests/test_postgres_graph.py`

 * *Files identical despite different names*

### Comparing `kurve-0.4/tests/test_s3_graph.py` & `kurve-0.5/tests/test_s3_graph.py`

 * *Files identical despite different names*

