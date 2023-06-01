# Comparing `tmp/foundationdb-7.3.1.tar.gz` & `tmp/foundationdb-7.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/foundationdb-7.3.1.tar", last modified: Thu May 25 01:53:31 2023, max compression
+gzip compressed data, was "dist/foundationdb-7.3.2.tar", last modified: Thu Jun  1 15:07:22 2023, max compression
```

## Comparing `foundationdb-7.3.1.tar` & `foundationdb-7.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)        0 2023-05-25 01:53:31.000000 foundationdb-7.3.1/
-drwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)        0 2023-05-25 01:53:31.000000 foundationdb-7.3.1/fdb/
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1913 2023-05-24 23:32:08.000000 foundationdb-7.3.1/fdb/subspace_impl.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    30888 2023-05-24 23:32:08.000000 foundationdb-7.3.1/fdb/six.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)       25 2023-05-24 23:07:00.000000 foundationdb-7.3.1/fdb/apiversion.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    21791 2023-05-24 23:32:08.000000 foundationdb-7.3.1/fdb/tuple.py
--rwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    26547 2023-05-24 23:32:08.000000 foundationdb-7.3.1/fdb/directory_impl.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     4811 2023-05-24 23:32:08.000000 foundationdb-7.3.1/fdb/__init__.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     5842 2023-05-24 23:32:08.000000 foundationdb-7.3.1/fdb/tenant_management.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     2814 2023-05-24 23:32:08.000000 foundationdb-7.3.1/fdb/locality.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    38989 2023-05-24 23:32:08.000000 foundationdb-7.3.1/fdb/fdboptions.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    66069 2023-05-24 23:32:08.000000 foundationdb-7.3.1/fdb/impl.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)      245 2023-05-24 23:32:08.000000 foundationdb-7.3.1/README.rst
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1427 2023-05-25 01:53:31.000000 foundationdb-7.3.1/PKG-INFO
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1416 2023-05-24 23:07:00.000000 foundationdb-7.3.1/setup.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    11665 2023-05-24 23:07:00.000000 foundationdb-7.3.1/LICENSE
+drwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)        0 2023-06-01 15:07:22.000000 foundationdb-7.3.2/
+drwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)        0 2023-06-01 15:07:22.000000 foundationdb-7.3.2/fdb/
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1913 2023-06-01 05:15:08.000000 foundationdb-7.3.2/fdb/subspace_impl.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    30888 2023-06-01 05:15:08.000000 foundationdb-7.3.2/fdb/six.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)       25 2023-06-01 04:58:38.000000 foundationdb-7.3.2/fdb/apiversion.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    21791 2023-06-01 05:15:08.000000 foundationdb-7.3.2/fdb/tuple.py
+-rwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    26547 2023-06-01 05:15:08.000000 foundationdb-7.3.2/fdb/directory_impl.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     4811 2023-06-01 05:15:08.000000 foundationdb-7.3.2/fdb/__init__.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     5842 2023-06-01 05:15:08.000000 foundationdb-7.3.2/fdb/tenant_management.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     2814 2023-06-01 05:15:08.000000 foundationdb-7.3.2/fdb/locality.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    38989 2023-06-01 05:15:08.000000 foundationdb-7.3.2/fdb/fdboptions.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    66069 2023-06-01 05:15:08.000000 foundationdb-7.3.2/fdb/impl.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)      252 2023-06-01 05:15:08.000000 foundationdb-7.3.2/README.rst
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1434 2023-06-01 15:07:22.000000 foundationdb-7.3.2/PKG-INFO
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1416 2023-06-01 04:58:38.000000 foundationdb-7.3.2/setup.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    11665 2023-06-01 04:58:38.000000 foundationdb-7.3.2/LICENSE
```

### Comparing `foundationdb-7.3.1/fdb/subspace_impl.py` & `foundationdb-7.3.2/fdb/subspace_impl.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.1/fdb/six.py` & `foundationdb-7.3.2/fdb/six.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.1/fdb/tuple.py` & `foundationdb-7.3.2/fdb/tuple.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.1/fdb/directory_impl.py` & `foundationdb-7.3.2/fdb/directory_impl.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.1/fdb/__init__.py` & `foundationdb-7.3.2/fdb/__init__.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.1/fdb/tenant_management.py` & `foundationdb-7.3.2/fdb/tenant_management.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.1/fdb/locality.py` & `foundationdb-7.3.2/fdb/locality.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.1/fdb/fdboptions.py` & `foundationdb-7.3.2/fdb/fdboptions.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.1/fdb/impl.py` & `foundationdb-7.3.2/fdb/impl.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.1/PKG-INFO` & `foundationdb-7.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 1.1
 Name: foundationdb
-Version: 7.3.1
+Version: 7.3.2
 Summary: Python bindings for the FoundationDB database
 Home-page: https://www.foundationdb.org
 Author: FoundationDB
 Author-email: fdb-dist@apple.com
 License: UNKNOWN
 Description: Complete documentation of the FoundationDB Python API can be found at https://apple.github.io/foundationdb/api-python.html.
         
-        These bindings require the FoundationDB client. The client can be obtained from https://www.foundationdb.org/download/.
+        These bindings require the FoundationDB client. The client can be obtained from https://github.com/apple/foundationdb/releases
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `foundationdb-7.3.1/setup.py` & `foundationdb-7.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     with open("README.rst") as f:
         long_desc = f.read()
 except:
     long_desc = ""
 
 setup(name="foundationdb",
-      version="7.3.1",
+      version="7.3.2",
       author="FoundationDB",
       author_email="fdb-dist@apple.com",
       description="Python bindings for the FoundationDB database",
       url="https://www.foundationdb.org",
       packages=['fdb'],
       package_data={'fdb': ["fdb/*.py"]},
       long_description=long_desc,
```

### Comparing `foundationdb-7.3.1/LICENSE` & `foundationdb-7.3.2/LICENSE`

 * *Files identical despite different names*

