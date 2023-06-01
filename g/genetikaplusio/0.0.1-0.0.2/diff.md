# Comparing `tmp/genetikaplusio-0.0.1.tar.gz` & `tmp/genetikaplusio-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genetikaplusio-0.0.1.tar", last modified: Thu Jun  1 14:27:19 2023, max compression
+gzip compressed data, was "genetikaplusio-0.0.2.tar", last modified: Thu Jun  1 14:39:50 2023, max compression
```

## Comparing `genetikaplusio-0.0.1.tar` & `genetikaplusio-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-01 14:27:19.533169 genetikaplusio-0.0.1/
--rw-r--r--   0 alonbentzion   (501) staff       (20)     1035 2023-06-01 14:13:50.000000 genetikaplusio-0.0.1/LICENSE.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)     4431 2023-06-01 14:27:19.532904 genetikaplusio-0.0.1/PKG-INFO
--rw-r--r--   0 alonbentzion   (501) staff       (20)     2931 2023-06-01 12:05:45.000000 genetikaplusio-0.0.1/README.md
--rw-r--r--   0 alonbentzion   (501) staff       (20)       38 2023-06-01 14:27:19.533236 genetikaplusio-0.0.1/setup.cfg
--rw-r--r--   0 alonbentzion   (501) staff       (20)     1167 2023-06-01 14:27:15.000000 genetikaplusio-0.0.1/setup.py
-drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-01 14:27:19.531813 genetikaplusio-0.0.1/src/
-drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-01 14:27:19.532646 genetikaplusio-0.0.1/src/genetikaplusio.egg-info/
--rw-r--r--   0 alonbentzion   (501) staff       (20)     4431 2023-06-01 14:27:19.000000 genetikaplusio-0.0.1/src/genetikaplusio.egg-info/PKG-INFO
--rw-r--r--   0 alonbentzion   (501) staff       (20)      300 2023-06-01 14:27:19.000000 genetikaplusio-0.0.1/src/genetikaplusio.egg-info/SOURCES.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)        1 2023-06-01 14:27:19.000000 genetikaplusio-0.0.1/src/genetikaplusio.egg-info/dependency_links.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)      407 2023-06-01 14:27:19.000000 genetikaplusio-0.0.1/src/genetikaplusio.egg-info/requires.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)       40 2023-06-01 14:27:19.000000 genetikaplusio-0.0.1/src/genetikaplusio.egg-info/top_level.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)     6995 2023-06-01 14:12:34.000000 genetikaplusio-0.0.1/src/gp_db_io.py
--rw-r--r--   0 alonbentzion   (501) staff       (20)     1971 2023-06-01 14:12:36.000000 genetikaplusio-0.0.1/src/gp_sqlconnection.py
--rw-r--r--   0 alonbentzion   (501) staff       (20)     3034 2023-06-01 14:12:39.000000 genetikaplusio-0.0.1/src/gp_storage_io.py
+drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-01 14:39:50.234517 genetikaplusio-0.0.2/
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     1035 2023-06-01 14:13:50.000000 genetikaplusio-0.0.2/LICENSE.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     4431 2023-06-01 14:39:50.234344 genetikaplusio-0.0.2/PKG-INFO
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     2931 2023-06-01 12:05:45.000000 genetikaplusio-0.0.2/README.md
+-rw-r--r--   0 alonbentzion   (501) staff       (20)       38 2023-06-01 14:39:50.234564 genetikaplusio-0.0.2/setup.cfg
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     1167 2023-06-01 14:39:45.000000 genetikaplusio-0.0.2/setup.py
+drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-01 14:39:50.233129 genetikaplusio-0.0.2/src/
+drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-01 14:39:50.234111 genetikaplusio-0.0.2/src/genetikaplusio.egg-info/
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     4431 2023-06-01 14:39:50.000000 genetikaplusio-0.0.2/src/genetikaplusio.egg-info/PKG-INFO
+-rw-r--r--   0 alonbentzion   (501) staff       (20)      300 2023-06-01 14:39:50.000000 genetikaplusio-0.0.2/src/genetikaplusio.egg-info/SOURCES.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)        1 2023-06-01 14:39:50.000000 genetikaplusio-0.0.2/src/genetikaplusio.egg-info/dependency_links.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)      318 2023-06-01 14:39:50.000000 genetikaplusio-0.0.2/src/genetikaplusio.egg-info/requires.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)       40 2023-06-01 14:39:50.000000 genetikaplusio-0.0.2/src/genetikaplusio.egg-info/top_level.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     6995 2023-06-01 14:12:34.000000 genetikaplusio-0.0.2/src/gp_db_io.py
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     1971 2023-06-01 14:12:36.000000 genetikaplusio-0.0.2/src/gp_sqlconnection.py
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     3034 2023-06-01 14:12:39.000000 genetikaplusio-0.0.2/src/gp_storage_io.py
```

### Comparing `genetikaplusio-0.0.1/LICENSE.txt` & `genetikaplusio-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genetikaplusio-0.0.1/PKG-INFO` & `genetikaplusio-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetikaplusio
-Version: 0.0.1
+Version: 0.0.2
 Summary: IO for database
 Author: Alon Ben Zion
 Author-email: alon@genetikaplus.com
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

### Comparing `genetikaplusio-0.0.1/README.md` & `genetikaplusio-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `genetikaplusio-0.0.1/setup.py` & `genetikaplusio-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     requirements = r.read().splitlines()
 
 with open("LICENSE.txt", 'r') as l:
     license = l.read()
 
 setup(
     name="genetikaplusio",
-    version="0.0.1",
+    version="0.0.2",
     author="Alon Ben Zion",
     author_email="alon@genetikaplus.com",
     license=license,
     description="IO for database",
     py_modules=["gp_db_io", "gp_storage_io", "gp_sqlconnection"],
     package_dir={"": "src"},
     classifiers=[
```

### Comparing `genetikaplusio-0.0.1/src/genetikaplusio.egg-info/PKG-INFO` & `genetikaplusio-0.0.2/src/genetikaplusio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetikaplusio
-Version: 0.0.1
+Version: 0.0.2
 Summary: IO for database
 Author: Alon Ben Zion
 Author-email: alon@genetikaplus.com
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

### Comparing `genetikaplusio-0.0.1/src/gp_db_io.py` & `genetikaplusio-0.0.2/src/gp_db_io.py`

 * *Files identical despite different names*

### Comparing `genetikaplusio-0.0.1/src/gp_sqlconnection.py` & `genetikaplusio-0.0.2/src/gp_sqlconnection.py`

 * *Files identical despite different names*

### Comparing `genetikaplusio-0.0.1/src/gp_storage_io.py` & `genetikaplusio-0.0.2/src/gp_storage_io.py`

 * *Files identical despite different names*

