# Comparing `tmp/lakeshack-0.2.1.tar.gz` & `tmp/lakeshack-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakeshack-0.2.1.tar", last modified: Tue Apr  4 23:39:40 2023, max compression
+gzip compressed data, was "lakeshack-0.2.2.tar", last modified: Thu Jun  1 02:53:54 2023, max compression
```

## Comparing `lakeshack-0.2.1.tar` & `lakeshack-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-04 23:39:40.157609 lakeshack-0.2.1/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    35149 2023-03-24 02:44:47.000000 lakeshack-0.2.1/LICENSE
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      536 2023-04-04 23:39:40.157609 lakeshack-0.2.1/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1306 2023-03-25 21:55:10.000000 lakeshack-0.2.1/README.rst
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-04 23:39:40.157609 lakeshack-0.2.1/lakeshack/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      107 2023-04-04 23:37:39.000000 lakeshack-0.2.1/lakeshack/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    21109 2023-03-26 03:39:07.000000 lakeshack-0.2.1/lakeshack/lakeshack.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    21874 2023-04-04 23:30:22.000000 lakeshack-0.2.1/lakeshack/metastore.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-04 23:39:40.157609 lakeshack-0.2.1/lakeshack.egg-info/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      536 2023-04-04 23:39:40.000000 lakeshack-0.2.1/lakeshack.egg-info/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      365 2023-04-04 23:39:40.000000 lakeshack-0.2.1/lakeshack.egg-info/SOURCES.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-04-04 23:39:40.000000 lakeshack-0.2.1/lakeshack.egg-info/dependency_links.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       39 2023-04-04 23:39:40.000000 lakeshack-0.2.1/lakeshack.egg-info/requires.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       16 2023-04-04 23:39:40.000000 lakeshack-0.2.1/lakeshack.egg-info/top_level.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       89 2023-03-24 02:44:47.000000 lakeshack-0.2.1/pyproject.toml
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      782 2023-04-04 23:39:40.157609 lakeshack-0.2.1/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       67 2023-03-24 02:44:47.000000 lakeshack-0.2.1/setup.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-04 23:39:40.157609 lakeshack-0.2.1/tests/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        0 2023-03-24 02:44:47.000000 lakeshack-0.2.1/tests/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    11035 2023-03-24 03:06:07.000000 lakeshack-0.2.1/tests/test_lakeshack.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    14346 2023-04-04 23:31:53.000000 lakeshack-0.2.1/tests/test_metastore.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     4071 2023-03-24 03:08:42.000000 lakeshack-0.2.1/tests/utils.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-01 02:53:54.281934 lakeshack-0.2.2/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    35149 2023-03-24 02:44:47.000000 lakeshack-0.2.2/LICENSE
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1843 2023-06-01 02:53:54.281934 lakeshack-0.2.2/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1306 2023-03-25 21:55:10.000000 lakeshack-0.2.2/README.rst
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-01 02:53:54.281934 lakeshack-0.2.2/lakeshack/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      107 2023-06-01 02:39:09.000000 lakeshack-0.2.2/lakeshack/__init__.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    21109 2023-03-26 03:39:07.000000 lakeshack-0.2.2/lakeshack/lakeshack.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    21954 2023-06-01 02:33:22.000000 lakeshack-0.2.2/lakeshack/metastore.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-01 02:53:54.281934 lakeshack-0.2.2/lakeshack.egg-info/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1843 2023-06-01 02:53:54.000000 lakeshack-0.2.2/lakeshack.egg-info/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      365 2023-06-01 02:53:54.000000 lakeshack-0.2.2/lakeshack.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-06-01 02:53:54.000000 lakeshack-0.2.2/lakeshack.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       39 2023-06-01 02:53:54.000000 lakeshack-0.2.2/lakeshack.egg-info/requires.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       16 2023-06-01 02:53:54.000000 lakeshack-0.2.2/lakeshack.egg-info/top_level.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       89 2023-03-24 02:44:47.000000 lakeshack-0.2.2/pyproject.toml
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      788 2023-06-01 02:53:54.281934 lakeshack-0.2.2/setup.cfg
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       67 2023-03-24 02:44:47.000000 lakeshack-0.2.2/setup.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-01 02:53:54.281934 lakeshack-0.2.2/tests/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        0 2023-03-24 02:44:47.000000 lakeshack-0.2.2/tests/__init__.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    11840 2023-06-01 02:13:42.000000 lakeshack-0.2.2/tests/test_lakeshack.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    14346 2023-04-04 23:31:53.000000 lakeshack-0.2.2/tests/test_metastore.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     4071 2023-03-24 03:08:42.000000 lakeshack-0.2.2/tests/utils.py
```

### Comparing `lakeshack-0.2.1/LICENSE` & `lakeshack-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeshack-0.2.1/README.rst` & `lakeshack-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `lakeshack-0.2.1/lakeshack/lakeshack.py` & `lakeshack-0.2.2/lakeshack/lakeshack.py`

 * *Files identical despite different names*

### Comparing `lakeshack-0.2.1/lakeshack/metastore.py` & `lakeshack-0.2.2/lakeshack/metastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,15 +446,17 @@
         for cluster_column_value in cluster_column_values:
             stmt = sa.select(self.table.c.filepath).where(
                 sa.and_(
                     col_cluster_min <= cluster_column_value,
                     cluster_column_value <= col_cluster_max,
                 )
             )
-            for (col, op, value) in optional_where_clauses:
+            for col, op, value in optional_where_clauses:
+                if col not in self.optional_columns:
+                    continue
                 col_min = self.table.columns[f"{col}_min"]
                 col_max = self.table.columns[f"{col}_max"]
                 if op == ">=":
                     stmt = stmt.where(value <= col_max)
                 elif op == ">":
                     stmt = stmt.where(value < col_max)
                 elif op == "=" or op == "==":
```

### Comparing `lakeshack-0.2.1/setup.cfg` & `lakeshack-0.2.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 	Documentation = https://mhendrey.github.io/lakeshack
 author = Matthew Hendrey
 author_email = matthew.hendrey@gmail.com
 classifiers = 
 	Programming Language :: Python :: 3
 license = GNU GPLv3
 description = Query parquet files using pyarrow or S3 Select by first gathering file metadata into a database
-description-file = README.rst
+long_description = file: README.rst
 keywords = pyarrow, s3, parquet
 
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.8
 install_requires =
```

### Comparing `lakeshack-0.2.1/tests/test_lakeshack.py` & `lakeshack-0.2.2/tests/test_lakeshack.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,14 +258,36 @@
     pa_schema = dataset.schema
 
     metastore = Metastore(f"sqlite:///{dbname}", "test", pa_schema)
     lakeshack = Lakeshack(metastore, fs.LocalFileSystem())
     query_check(lakeshack, "ts")
 
 
+def test_query_ts_optional_where_clause(pq_dir_ts):
+    """
+    Test querying the metastore that has just the 'id' column listed,
+    but provide an optional 'timestamp' clause in the lakeshack.query().
+    This should pull back all the records and then filter according to the
+    timestamp filter
+
+    Parameters
+    ----------
+    pq_dir_ts : Path
+        Session-scoped fixture that is a path (dir) to the test parquet files
+    """
+    data_dir = str(pq_dir_ts)
+    dataset = ds.dataset(data_dir, format="parquet", filesystem=fs.LocalFileSystem())
+    pa_schema = dataset.schema
+
+    metastore = Metastore("sqlite:///:memory:", "test", pa_schema, "id")
+    metastore.update(data_dir, fs.LocalFileSystem())
+    lakeshack = Lakeshack(metastore, fs.LocalFileSystem())
+    query_check(lakeshack, "ts")
+
+
 def test_query_tz(metastore_db_tz, pq_dir_tz):
     """
     Test querying the metastore when timestamp column is tz aware datetime
 
     Parameters
     ----------
     metastore_db_tz : Path
```

### Comparing `lakeshack-0.2.1/tests/test_metastore.py` & `lakeshack-0.2.2/tests/test_metastore.py`

 * *Files identical despite different names*

### Comparing `lakeshack-0.2.1/tests/utils.py` & `lakeshack-0.2.2/tests/utils.py`

 * *Files identical despite different names*

