# Comparing `tmp/samba_metric-0.0.6.tar.gz` & `tmp/samba_metric-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samba_metric-0.0.6.tar", last modified: Thu Jun  1 19:05:27 2023, max compression
+gzip compressed data, was "samba_metric-0.0.7.tar", last modified: Thu Jun  1 19:08:31 2023, max compression
```

## Comparing `samba_metric-0.0.6.tar` & `samba_metric-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 19:05:27.280920 samba_metric-0.0.6/
--rw-rw-rw-   0        0        0     2193 2023-06-01 19:05:27.280920 samba_metric-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1869 2023-06-01 18:30:45.000000 samba_metric-0.0.6/README.md
--rw-rw-rw-   0        0        0      695 2023-06-01 19:05:11.000000 samba_metric-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 19:05:27.280920 samba_metric-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-01 19:05:27.216612 samba_metric-0.0.6/src/
--rw-rw-rw-   0        0        0       81 2023-06-01 19:01:13.000000 samba_metric-0.0.6/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 19:05:27.254796 samba_metric-0.0.6/src/samba/
--rw-rw-rw-   0        0        0     4882 2023-06-01 18:30:45.000000 samba_metric-0.0.6/src/samba/SAMBA_metric.py
--rw-rw-rw-   0        0        0      154 2023-06-01 19:04:51.000000 samba_metric-0.0.6/src/samba/__init__.py
--rw-rw-rw-   0        0        0     5522 2023-06-01 18:30:45.000000 samba_metric-0.0.6/src/samba/micro2matrix.py
--rw-rw-rw-   0        0        0     2068 2023-06-01 18:30:45.000000 samba_metric-0.0.6/src/samba/textreeCreate.py
-drwxrwxrwx   0        0        0        0 2023-06-01 19:05:27.278875 samba_metric-0.0.6/src/samba_metric.egg-info/
--rw-rw-rw-   0        0        0     2193 2023-06-01 19:05:27.000000 samba_metric-0.0.6/src/samba_metric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-06-01 19:05:27.000000 samba_metric-0.0.6/src/samba_metric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 19:05:27.000000 samba_metric-0.0.6/src/samba_metric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-06-01 19:05:27.000000 samba_metric-0.0.6/src/samba_metric.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-01 19:05:27.000000 samba_metric-0.0.6/src/samba_metric.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 19:08:31.014019 samba_metric-0.0.7/
+-rw-rw-rw-   0        0        0     2193 2023-06-01 19:08:31.014019 samba_metric-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1869 2023-06-01 18:30:45.000000 samba_metric-0.0.7/README.md
+-rw-rw-rw-   0        0        0      695 2023-06-01 19:08:06.000000 samba_metric-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 19:08:31.015043 samba_metric-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 19:08:30.958950 samba_metric-0.0.7/src/
+-rw-rw-rw-   0        0        0       81 2023-06-01 19:01:13.000000 samba_metric-0.0.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:08:30.997295 samba_metric-0.0.7/src/samba/
+-rw-rw-rw-   0        0        0     4882 2023-06-01 18:30:45.000000 samba_metric-0.0.7/src/samba/SAMBA_metric.py
+-rw-rw-rw-   0        0        0      159 2023-06-01 19:08:06.000000 samba_metric-0.0.7/src/samba/__init__.py
+-rw-rw-rw-   0        0        0     5522 2023-06-01 18:30:45.000000 samba_metric-0.0.7/src/samba/microbiome2matrix.py
+-rw-rw-rw-   0        0        0     2068 2023-06-01 18:30:45.000000 samba_metric-0.0.7/src/samba/textreeCreate.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:08:31.012128 samba_metric-0.0.7/src/samba_metric.egg-info/
+-rw-rw-rw-   0        0        0     2193 2023-06-01 19:08:30.000000 samba_metric-0.0.7/src/samba_metric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-06-01 19:08:30.000000 samba_metric-0.0.7/src/samba_metric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 19:08:30.000000 samba_metric-0.0.7/src/samba_metric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-06-01 19:08:30.000000 samba_metric-0.0.7/src/samba_metric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-01 19:08:30.000000 samba_metric-0.0.7/src/samba_metric.egg-info/top_level.txt
```

### Comparing `samba_metric-0.0.6/PKG-INFO` & `samba_metric-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samba_metric
-Version: 0.0.6
+Version: 0.0.7
 Author-email: Oshrit Shtossel <oshritvig@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `samba_metric-0.0.6/README.md` & `samba_metric-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `samba_metric-0.0.6/pyproject.toml` & `samba_metric-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "samba_metric"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 readme = "README.md"
 authors = [{ name = "Oshrit Shtossel", email = "oshritvig@gmail.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `samba_metric-0.0.6/src/samba/SAMBA_metric.py` & `samba_metric-0.0.7/src/samba/SAMBA_metric.py`

 * *Files identical despite different names*

### Comparing `samba_metric-0.0.6/src/samba/micro2matrix.py` & `samba_metric-0.0.7/src/samba/microbiome2matrix.py`

 * *Files identical despite different names*

### Comparing `samba_metric-0.0.6/src/samba/textreeCreate.py` & `samba_metric-0.0.7/src/samba/textreeCreate.py`

 * *Files identical despite different names*

### Comparing `samba_metric-0.0.6/src/samba_metric.egg-info/PKG-INFO` & `samba_metric-0.0.7/src/samba_metric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samba-metric
-Version: 0.0.6
+Version: 0.0.7
 Author-email: Oshrit Shtossel <oshritvig@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

