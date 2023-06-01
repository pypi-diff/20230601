# Comparing `tmp/tello_solectric_pl-0.0.2b0.tar.gz` & `tmp/tello_solectric_pl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tello_solectric_pl-0.0.2b0.tar", last modified: Thu Jun  1 12:05:27 2023, max compression
+gzip compressed data, was "tello_solectric_pl-0.0.3.tar", last modified: Thu Jun  1 12:33:50 2023, max compression
```

## Comparing `tello_solectric_pl-0.0.2b0.tar` & `tello_solectric_pl-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:05:27.401039 tello_solectric_pl-0.0.2b0/
--rw-rw-r--   0 adasiek   (1000) adasiek   (1000)     3178 2023-06-01 12:05:27.401039 tello_solectric_pl-0.0.2b0/PKG-INFO
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     2546 2023-04-08 09:49:02.000000 tello_solectric_pl-0.0.2b0/README.md
--rw-rw-r--   0 adasiek   (1000) adasiek   (1000)       38 2023-06-01 12:05:27.401039 tello_solectric_pl-0.0.2b0/setup.cfg
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      891 2023-06-01 12:05:16.000000 tello_solectric_pl-0.0.2b0/setup.py
-drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:05:27.401039 tello_solectric_pl-0.0.2b0/tello_solectric_pl/
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      288 2023-04-08 09:32:08.000000 tello_solectric_pl-0.0.2b0/tello_solectric_pl/__init__.py
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3044 2023-06-01 12:05:06.000000 tello_solectric_pl-0.0.2b0/tello_solectric_pl/tello_solectric_pl.py
-drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:05:27.401039 tello_solectric_pl-0.0.2b0/tello_solectric_pl.egg-info/
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3178 2023-06-01 12:05:27.000000 tello_solectric_pl-0.0.2b0/tello_solectric_pl.egg-info/PKG-INFO
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      299 2023-06-01 12:05:27.000000 tello_solectric_pl-0.0.2b0/tello_solectric_pl.egg-info/SOURCES.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)        1 2023-06-01 12:05:27.000000 tello_solectric_pl-0.0.2b0/tello_solectric_pl.egg-info/dependency_links.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)       11 2023-06-01 12:05:27.000000 tello_solectric_pl-0.0.2b0/tello_solectric_pl.egg-info/requires.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)       19 2023-06-01 12:05:27.000000 tello_solectric_pl-0.0.2b0/tello_solectric_pl.egg-info/top_level.txt
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:33:50.805644 tello_solectric_pl-0.0.3/
+-rw-rw-r--   0 adasiek   (1000) adasiek   (1000)     3176 2023-06-01 12:33:50.805644 tello_solectric_pl-0.0.3/PKG-INFO
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     2546 2023-04-08 09:49:02.000000 tello_solectric_pl-0.0.3/README.md
+-rw-rw-r--   0 adasiek   (1000) adasiek   (1000)       38 2023-06-01 12:33:50.805644 tello_solectric_pl-0.0.3/setup.cfg
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      890 2023-06-01 12:31:52.000000 tello_solectric_pl-0.0.3/setup.py
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:33:50.805644 tello_solectric_pl-0.0.3/tello_solectric_pl/
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      288 2023-04-08 09:32:08.000000 tello_solectric_pl-0.0.3/tello_solectric_pl/__init__.py
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3044 2023-06-01 12:05:06.000000 tello_solectric_pl-0.0.3/tello_solectric_pl/tello_solectric_pl.py
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:33:50.805644 tello_solectric_pl-0.0.3/tello_solectric_pl.egg-info/
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3176 2023-06-01 12:33:50.000000 tello_solectric_pl-0.0.3/tello_solectric_pl.egg-info/PKG-INFO
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      299 2023-06-01 12:33:50.000000 tello_solectric_pl-0.0.3/tello_solectric_pl.egg-info/SOURCES.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)        1 2023-06-01 12:33:50.000000 tello_solectric_pl-0.0.3/tello_solectric_pl.egg-info/dependency_links.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)       11 2023-06-01 12:33:50.000000 tello_solectric_pl-0.0.3/tello_solectric_pl.egg-info/requires.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)       19 2023-06-01 12:33:50.000000 tello_solectric_pl-0.0.3/tello_solectric_pl.egg-info/top_level.txt
```

### Comparing `tello_solectric_pl-0.0.2b0/PKG-INFO` & `tello_solectric_pl-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tello_solectric_pl
-Version: 0.0.2b0
+Version: 0.0.3
 Summary: Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)
 Home-page: https://solectric.pl
 Author: Adam Jurkiewicz
 Author-email: adam@jurkiewicz.tech
 License: UNKNOWN
 Keywords: Dron Tello TelloEDU Ryzen RyzenTT DJI
 Platform: UNKNOWN
```

### Comparing `tello_solectric_pl-0.0.2b0/README.md` & `tello_solectric_pl-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tello_solectric_pl-0.0.2b0/setup.py` & `tello_solectric_pl-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tello_solectric_pl",
-    version="0.0.2b",
+    version="0.0.3",
     author="Adam Jurkiewicz",
     python_requires='>=3.8',
     author_email="adam@jurkiewicz.tech",
     description="Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://solectric.pl",
```

### Comparing `tello_solectric_pl-0.0.2b0/tello_solectric_pl/tello_solectric_pl.py` & `tello_solectric_pl-0.0.3/tello_solectric_pl/tello_solectric_pl.py`

 * *Files identical despite different names*

### Comparing `tello_solectric_pl-0.0.2b0/tello_solectric_pl.egg-info/PKG-INFO` & `tello_solectric_pl-0.0.3/tello_solectric_pl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tello-solectric-pl
-Version: 0.0.2b0
+Version: 0.0.3
 Summary: Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)
 Home-page: https://solectric.pl
 Author: Adam Jurkiewicz
 Author-email: adam@jurkiewicz.tech
 License: UNKNOWN
 Keywords: Dron Tello TelloEDU Ryzen RyzenTT DJI
 Platform: UNKNOWN
```

