# Comparing `tmp/perfunctory-0.0.3.tar.gz` & `tmp/perfunctory-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perfunctory-0.0.3.tar", last modified: Thu Jun  1 17:56:00 2023, max compression
+gzip compressed data, was "perfunctory-0.0.4.tar", last modified: Thu Jun  1 18:03:14 2023, max compression
```

## Comparing `perfunctory-0.0.3.tar` & `perfunctory-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:56:00.544544 perfunctory-0.0.3/
--rw-r--r--   0 harpreetsingh   (501) staff       (20)        4 2023-06-01 17:31:35.000000 perfunctory-0.0.3/LICENSE.txt
--rw-r--r--   0 harpreetsingh   (501) staff       (20)      542 2023-06-01 17:56:00.544048 perfunctory-0.0.3/PKG-INFO
--rw-r--r--   0 harpreetsingh   (501) staff       (20)       75 2023-06-01 17:32:16.000000 perfunctory-0.0.3/README.md
-drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:56:00.539790 perfunctory-0.0.3/perfunctory/
--rw-r--r--   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:27:18.000000 perfunctory-0.0.3/perfunctory/__init__.py
--rw-r--r--   0 harpreetsingh   (501) staff       (20)     8204 2023-06-01 17:25:00.000000 perfunctory-0.0.3/perfunctory/rbaa.py
-drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:56:00.543170 perfunctory-0.0.3/perfunctory.egg-info/
--rw-r--r--   0 harpreetsingh   (501) staff       (20)      542 2023-06-01 17:56:00.000000 perfunctory-0.0.3/perfunctory.egg-info/PKG-INFO
--rw-r--r--   0 harpreetsingh   (501) staff       (20)      248 2023-06-01 17:56:00.000000 perfunctory-0.0.3/perfunctory.egg-info/SOURCES.txt
--rw-r--r--   0 harpreetsingh   (501) staff       (20)        1 2023-06-01 17:56:00.000000 perfunctory-0.0.3/perfunctory.egg-info/dependency_links.txt
--rw-r--r--   0 harpreetsingh   (501) staff       (20)      122 2023-06-01 17:56:00.000000 perfunctory-0.0.3/perfunctory.egg-info/requires.txt
--rw-r--r--   0 harpreetsingh   (501) staff       (20)       12 2023-06-01 17:56:00.000000 perfunctory-0.0.3/perfunctory.egg-info/top_level.txt
--rw-r--r--   0 harpreetsingh   (501) staff       (20)       38 2023-06-01 17:56:00.544791 perfunctory-0.0.3/setup.cfg
--rw-r--r--   0 harpreetsingh   (501) staff       (20)     1040 2023-06-01 17:55:36.000000 perfunctory-0.0.3/setup.py
+drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 18:03:14.118496 perfunctory-0.0.4/
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)        4 2023-06-01 17:31:35.000000 perfunctory-0.0.4/LICENSE.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)      542 2023-06-01 18:03:14.117951 perfunctory-0.0.4/PKG-INFO
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)       75 2023-06-01 17:32:16.000000 perfunctory-0.0.4/README.md
+drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 18:03:14.113756 perfunctory-0.0.4/perfunctory/
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)       30 2023-06-01 18:02:05.000000 perfunctory-0.0.4/perfunctory/__init__.py
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)     8204 2023-06-01 17:25:00.000000 perfunctory-0.0.4/perfunctory/rbaa.py
+drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 18:03:14.117000 perfunctory-0.0.4/perfunctory.egg-info/
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)      542 2023-06-01 18:03:13.000000 perfunctory-0.0.4/perfunctory.egg-info/PKG-INFO
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)      248 2023-06-01 18:03:13.000000 perfunctory-0.0.4/perfunctory.egg-info/SOURCES.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)        1 2023-06-01 18:03:13.000000 perfunctory-0.0.4/perfunctory.egg-info/dependency_links.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)      122 2023-06-01 18:03:13.000000 perfunctory-0.0.4/perfunctory.egg-info/requires.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)       12 2023-06-01 18:03:13.000000 perfunctory-0.0.4/perfunctory.egg-info/top_level.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)       38 2023-06-01 18:03:14.118711 perfunctory-0.0.4/setup.cfg
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)     1040 2023-06-01 18:02:12.000000 perfunctory-0.0.4/setup.py
```

### Comparing `perfunctory-0.0.3/PKG-INFO` & `perfunctory-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfunctory
-Version: 0.0.3
+Version: 0.0.4
 Summary: perfunctory
 Home-page: UNKNOWN
 Author: (Hank Singh)
 Author-email: <harpreetsingh1811@gmail.com>
 License: UNKNOWN
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `perfunctory-0.0.3/perfunctory/rbaa.py` & `perfunctory-0.0.4/perfunctory/rbaa.py`

 * *Files identical despite different names*

### Comparing `perfunctory-0.0.3/perfunctory.egg-info/PKG-INFO` & `perfunctory-0.0.4/perfunctory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfunctory
-Version: 0.0.3
+Version: 0.0.4
 Summary: perfunctory
 Home-page: UNKNOWN
 Author: (Hank Singh)
 Author-email: <harpreetsingh1811@gmail.com>
 License: UNKNOWN
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `perfunctory-0.0.3/setup.py` & `perfunctory-0.0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = "perfunctory"
 LONG_DESCRIPTION = """Nope.
                     """
 
 # Setting up
 setup(
     name="perfunctory",
```

