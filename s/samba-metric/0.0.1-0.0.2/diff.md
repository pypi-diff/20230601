# Comparing `tmp/samba_metric-0.0.1.tar.gz` & `tmp/samba_metric-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samba_metric-0.0.1.tar", last modified: Thu Jun  1 18:31:34 2023, max compression
+gzip compressed data, was "samba_metric-0.0.2.tar", last modified: Thu Jun  1 18:41:33 2023, max compression
```

## Comparing `samba_metric-0.0.1.tar` & `samba_metric-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 18:31:34.445746 samba_metric-0.0.1/
--rw-rw-rw-   0        0        0     2193 2023-06-01 18:31:34.444844 samba_metric-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1869 2023-06-01 18:30:45.000000 samba_metric-0.0.1/README.md
--rw-rw-rw-   0        0        0      695 2023-06-01 18:30:45.000000 samba_metric-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 18:31:34.446776 samba_metric-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-01 18:31:34.419943 samba_metric-0.0.1/src/
--rw-rw-rw-   0        0        0     4882 2023-06-01 18:30:45.000000 samba_metric-0.0.1/src/SAMBA_metric.py
--rw-rw-rw-   0        0        0      137 2023-06-01 18:30:45.000000 samba_metric-0.0.1/src/__init__.py
--rw-rw-rw-   0        0        0     5522 2023-06-01 18:30:45.000000 samba_metric-0.0.1/src/micro2matrix.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:31:34.443712 samba_metric-0.0.1/src/samba_metric.egg-info/
--rw-rw-rw-   0        0        0     2193 2023-06-01 18:31:34.000000 samba_metric-0.0.1/src/samba_metric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-06-01 18:31:34.000000 samba_metric-0.0.1/src/samba_metric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 18:31:34.000000 samba_metric-0.0.1/src/samba_metric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-06-01 18:31:34.000000 samba_metric-0.0.1/src/samba_metric.egg-info/requires.txt
--rw-rw-rw-   0        0        0       49 2023-06-01 18:31:34.000000 samba_metric-0.0.1/src/samba_metric.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2068 2023-06-01 18:30:45.000000 samba_metric-0.0.1/src/textreeCreate.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:41:33.347745 samba_metric-0.0.2/
+-rw-rw-rw-   0        0        0     2193 2023-06-01 18:41:33.347246 samba_metric-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1869 2023-06-01 18:30:45.000000 samba_metric-0.0.2/README.md
+-rw-rw-rw-   0        0        0      695 2023-06-01 18:40:32.000000 samba_metric-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 18:41:33.348750 samba_metric-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 18:41:33.320499 samba_metric-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-01 18:41:33.327488 samba_metric-0.0.2/src/samba/
+-rw-rw-rw-   0        0        0     4882 2023-06-01 18:30:45.000000 samba_metric-0.0.2/src/samba/SAMBA_metric.py
+-rw-rw-rw-   0        0        0      164 2023-06-01 18:39:58.000000 samba_metric-0.0.2/src/samba/__init__.py
+-rw-rw-rw-   0        0        0     5522 2023-06-01 18:30:45.000000 samba_metric-0.0.2/src/samba/micro2matrix.py
+-rw-rw-rw-   0        0        0     2068 2023-06-01 18:30:45.000000 samba_metric-0.0.2/src/samba/textreeCreate.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:41:33.345498 samba_metric-0.0.2/src/samba_metric.egg-info/
+-rw-rw-rw-   0        0        0     2193 2023-06-01 18:41:33.000000 samba_metric-0.0.2/src/samba_metric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-06-01 18:41:33.000000 samba_metric-0.0.2/src/samba_metric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 18:41:33.000000 samba_metric-0.0.2/src/samba_metric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-06-01 18:41:33.000000 samba_metric-0.0.2/src/samba_metric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-01 18:41:33.000000 samba_metric-0.0.2/src/samba_metric.egg-info/top_level.txt
```

### Comparing `samba_metric-0.0.1/PKG-INFO` & `samba_metric-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samba_metric
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Oshrit Shtossel <oshritvig@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `samba_metric-0.0.1/README.md` & `samba_metric-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `samba_metric-0.0.1/pyproject.toml` & `samba_metric-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "samba_metric"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 readme = "README.md"
 authors = [{ name = "Oshrit Shtossel", email = "oshritvig@gmail.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `samba_metric-0.0.1/src/SAMBA_metric.py` & `samba_metric-0.0.2/src/samba/SAMBA_metric.py`

 * *Files identical despite different names*

### Comparing `samba_metric-0.0.1/src/micro2matrix.py` & `samba_metric-0.0.2/src/samba/micro2matrix.py`

 * *Files identical despite different names*

### Comparing `samba_metric-0.0.1/src/samba_metric.egg-info/PKG-INFO` & `samba_metric-0.0.2/src/samba_metric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samba-metric
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Oshrit Shtossel <oshritvig@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `samba_metric-0.0.1/src/textreeCreate.py` & `samba_metric-0.0.2/src/samba/textreeCreate.py`

 * *Files identical despite different names*

