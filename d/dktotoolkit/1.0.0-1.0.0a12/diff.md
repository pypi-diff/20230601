# Comparing `tmp/dktotoolkit-1.0.0.tar.gz` & `tmp/dktotoolkit-1.0.0a12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dktotoolkit-1.0.0.tar", last modified: Thu Jun  1 13:03:26 2023, max compression
+gzip compressed data, was "dktotoolkit-1.0.0a12.tar", last modified: Thu Jun  1 12:58:17 2023, max compression
```

## Comparing `dktotoolkit-1.0.0.tar` & `dktotoolkit-1.0.0a12.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:03:26.185353 dktotoolkit-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 13:03:11.000000 dktotoolkit-1.0.0/LICENCE.txt
--rw-r--r--   0 root         (0) root         (0)     6666 2023-06-01 13:03:26.185353 dktotoolkit-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6239 2023-06-01 13:03:11.000000 dktotoolkit-1.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-06-01 13:03:26.189353 dktotoolkit-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-06-01 13:03:11.000000 dktotoolkit-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:03:26.185353 dktotoolkit-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:03:26.185353 dktotoolkit-1.0.0/src/dktotoolkit/
--rw-rw-rw-   0 root         (0) root         (0)     1602 2023-06-01 13:03:11.000000 dktotoolkit-1.0.0/src/dktotoolkit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3162 2023-06-01 13:03:11.000000 dktotoolkit-1.0.0/src/dktotoolkit/_loadenv.py
--rw-rw-rw-   0 root         (0) root         (0)      971 2023-06-01 13:03:11.000000 dktotoolkit-1.0.0/src/dktotoolkit/_replace_with_mask.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-01 13:03:11.000000 dktotoolkit-1.0.0/src/dktotoolkit/dict2obj.py
--rw-rw-rw-   0 root         (0) root         (0)     2035 2023-06-01 13:03:11.000000 dktotoolkit-1.0.0/src/dktotoolkit/dotenv2clock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:03:26.185353 dktotoolkit-1.0.0/src/dktotoolkit/function/
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-06-01 13:03:11.000000 dktotoolkit-1.0.0/src/dktotoolkit/function/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-06-01 13:03:11.000000 dktotoolkit-1.0.0/src/dktotoolkit/function/_compatMode.py
--rw-rw-rw-   0 root         (0) root         (0)     2889 2023-06-01 13:03:11.000000 dktotoolkit-1.0.0/src/dktotoolkit/loadenv.py
--rw-rw-rw-   0 root         (0) root         (0)     4752 2023-06-01 13:03:11.000000 dktotoolkit-1.0.0/src/dktotoolkit/parse_dates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:03:26.185353 dktotoolkit-1.0.0/src/dktotoolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6666 2023-06-01 13:03:26.000000 dktotoolkit-1.0.0/src/dktotoolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      523 2023-06-01 13:03:26.000000 dktotoolkit-1.0.0/src/dktotoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 13:03:26.000000 dktotoolkit-1.0.0/src/dktotoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-01 13:03:26.000000 dktotoolkit-1.0.0/src/dktotoolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-01 13:03:26.000000 dktotoolkit-1.0.0/src/dktotoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 12:58:04.000000 dktotoolkit-1.0.0a12/LICENCE.txt
+-rw-r--r--   0 root         (0) root         (0)     6669 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6239 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.268872 dktotoolkit-1.0.0a12/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.268872 dktotoolkit-1.0.0a12/src/dktotoolkit/
+-rw-rw-rw-   0 root         (0) root         (0)     1602 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3162 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/_loadenv.py
+-rw-rw-rw-   0 root         (0) root         (0)      971 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/_replace_with_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/dict2obj.py
+-rw-rw-rw-   0 root         (0) root         (0)     2035 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/dotenv2clock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/src/dktotoolkit/function/
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/function/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/function/_compatMode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2889 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/loadenv.py
+-rw-rw-rw-   0 root         (0) root         (0)     4752 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/parse_dates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6669 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      523 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/top_level.txt
```

### Comparing `dktotoolkit-1.0.0/PKG-INFO` & `dktotoolkit-1.0.0a12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dktotoolkit
-Version: 1.0.0
+Version: 1.0.0a12
 Summary: A little toolkit with fancy functions
 Home-page: https://discord-catho.frama.io/module_toolkit
 Author: Pierre
 Project-URL: Source Code, https://framagit.org/discord-catho/module_toolkit
 Keywords: dotenv,.env,toolkit,parse dates
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dktotoolkit-1.0.0/README.md` & `dktotoolkit-1.0.0a12/README.md`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.0/setup.cfg` & `dktotoolkit-1.0.0a12/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dktotoolkit
-version = 1.0.0
+version = 1.0.0a12
 author = Pierre
 description = A little toolkit with fancy functions
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://discord-catho.frama.io/module_toolkit
 project_urls = 
 	Source Code = https://framagit.org/discord-catho/module_toolkit
```

### Comparing `dktotoolkit-1.0.0/src/dktotoolkit/__init__.py` & `dktotoolkit-1.0.0a12/src/dktotoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.0/src/dktotoolkit/_loadenv.py` & `dktotoolkit-1.0.0a12/src/dktotoolkit/_loadenv.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.0/src/dktotoolkit/_replace_with_mask.py` & `dktotoolkit-1.0.0a12/src/dktotoolkit/_replace_with_mask.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.0/src/dktotoolkit/dict2obj.py` & `dktotoolkit-1.0.0a12/src/dktotoolkit/dict2obj.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.0/src/dktotoolkit/dotenv2clock.py` & `dktotoolkit-1.0.0a12/src/dktotoolkit/dotenv2clock.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.0/src/dktotoolkit/function/_compatMode.py` & `dktotoolkit-1.0.0a12/src/dktotoolkit/function/_compatMode.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.0/src/dktotoolkit/loadenv.py` & `dktotoolkit-1.0.0a12/src/dktotoolkit/loadenv.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.0/src/dktotoolkit/parse_dates.py` & `dktotoolkit-1.0.0a12/src/dktotoolkit/parse_dates.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.0/src/dktotoolkit.egg-info/PKG-INFO` & `dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dktotoolkit
-Version: 1.0.0
+Version: 1.0.0a12
 Summary: A little toolkit with fancy functions
 Home-page: https://discord-catho.frama.io/module_toolkit
 Author: Pierre
 Project-URL: Source Code, https://framagit.org/discord-catho/module_toolkit
 Keywords: dotenv,.env,toolkit,parse dates
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dktotoolkit-1.0.0/src/dktotoolkit.egg-info/SOURCES.txt` & `dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

