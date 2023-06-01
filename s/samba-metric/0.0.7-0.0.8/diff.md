# Comparing `tmp/samba_metric-0.0.7.tar.gz` & `tmp/samba_metric-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samba_metric-0.0.7.tar", last modified: Thu Jun  1 19:08:31 2023, max compression
+gzip compressed data, was "samba_metric-0.0.8.tar", last modified: Thu Jun  1 19:12:05 2023, max compression
```

## Comparing `samba_metric-0.0.7.tar` & `samba_metric-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 19:08:31.014019 samba_metric-0.0.7/
--rw-rw-rw-   0        0        0     2193 2023-06-01 19:08:31.014019 samba_metric-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1869 2023-06-01 18:30:45.000000 samba_metric-0.0.7/README.md
--rw-rw-rw-   0        0        0      695 2023-06-01 19:08:06.000000 samba_metric-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 19:08:31.015043 samba_metric-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-01 19:08:30.958950 samba_metric-0.0.7/src/
--rw-rw-rw-   0        0        0       81 2023-06-01 19:01:13.000000 samba_metric-0.0.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 19:08:30.997295 samba_metric-0.0.7/src/samba/
--rw-rw-rw-   0        0        0     4882 2023-06-01 18:30:45.000000 samba_metric-0.0.7/src/samba/SAMBA_metric.py
--rw-rw-rw-   0        0        0      159 2023-06-01 19:08:06.000000 samba_metric-0.0.7/src/samba/__init__.py
--rw-rw-rw-   0        0        0     5522 2023-06-01 18:30:45.000000 samba_metric-0.0.7/src/samba/microbiome2matrix.py
--rw-rw-rw-   0        0        0     2068 2023-06-01 18:30:45.000000 samba_metric-0.0.7/src/samba/textreeCreate.py
-drwxrwxrwx   0        0        0        0 2023-06-01 19:08:31.012128 samba_metric-0.0.7/src/samba_metric.egg-info/
--rw-rw-rw-   0        0        0     2193 2023-06-01 19:08:30.000000 samba_metric-0.0.7/src/samba_metric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-06-01 19:08:30.000000 samba_metric-0.0.7/src/samba_metric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 19:08:30.000000 samba_metric-0.0.7/src/samba_metric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-06-01 19:08:30.000000 samba_metric-0.0.7/src/samba_metric.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-01 19:08:30.000000 samba_metric-0.0.7/src/samba_metric.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 19:12:05.559664 samba_metric-0.0.8/
+-rw-rw-rw-   0        0        0     2193 2023-06-01 19:12:05.559664 samba_metric-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1869 2023-06-01 18:30:45.000000 samba_metric-0.0.8/README.md
+-rw-rw-rw-   0        0        0      695 2023-06-01 19:11:03.000000 samba_metric-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 19:12:05.559664 samba_metric-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 19:12:05.526946 samba_metric-0.0.8/src/
+-rw-rw-rw-   0        0        0       81 2023-06-01 19:01:13.000000 samba_metric-0.0.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:12:05.541166 samba_metric-0.0.8/src/samba/
+-rw-rw-rw-   0        0        0     4882 2023-06-01 18:30:45.000000 samba_metric-0.0.8/src/samba/SAMBA_metric.py
+-rw-rw-rw-   0        0        0      161 2023-06-01 19:11:42.000000 samba_metric-0.0.8/src/samba/__init__.py
+-rw-rw-rw-   0        0        0     5533 2023-06-01 19:11:48.000000 samba_metric-0.0.8/src/samba/microbiome2matrix.py
+-rw-rw-rw-   0        0        0     2068 2023-06-01 18:30:45.000000 samba_metric-0.0.8/src/samba/textreeCreate.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:12:05.558666 samba_metric-0.0.8/src/samba_metric.egg-info/
+-rw-rw-rw-   0        0        0     2193 2023-06-01 19:12:05.000000 samba_metric-0.0.8/src/samba_metric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-06-01 19:12:05.000000 samba_metric-0.0.8/src/samba_metric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 19:12:05.000000 samba_metric-0.0.8/src/samba_metric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-06-01 19:12:05.000000 samba_metric-0.0.8/src/samba_metric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-01 19:12:05.000000 samba_metric-0.0.8/src/samba_metric.egg-info/top_level.txt
```

### Comparing `samba_metric-0.0.7/PKG-INFO` & `samba_metric-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samba_metric
-Version: 0.0.7
+Version: 0.0.8
 Author-email: Oshrit Shtossel <oshritvig@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `samba_metric-0.0.7/README.md` & `samba_metric-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `samba_metric-0.0.7/pyproject.toml` & `samba_metric-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "samba_metric"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 readme = "README.md"
 authors = [{ name = "Oshrit Shtossel", email = "oshritvig@gmail.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `samba_metric-0.0.7/src/samba/SAMBA_metric.py` & `samba_metric-0.0.8/src/samba/SAMBA_metric.py`

 * *Files identical despite different names*

### Comparing `samba_metric-0.0.7/src/samba/microbiome2matrix.py` & `samba_metric-0.0.8/src/samba/microbiome2matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from concurrent.futures.thread import ThreadPoolExecutor
 
 import numpy as np
 from scipy.cluster.hierarchy import linkage, dendrogram
 import tqdm
 import igraph
 
-from src import create_tax_tree
+from .textreeCreate import create_tax_tree
 
 
 def save_2d(otu, name, path):
     otu.dump(f"{path}/{name}.npy")
 
 
 def find_root(G, child):
```

### Comparing `samba_metric-0.0.7/src/samba/textreeCreate.py` & `samba_metric-0.0.8/src/samba/textreeCreate.py`

 * *Files identical despite different names*

### Comparing `samba_metric-0.0.7/src/samba_metric.egg-info/PKG-INFO` & `samba_metric-0.0.8/src/samba_metric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samba-metric
-Version: 0.0.7
+Version: 0.0.8
 Author-email: Oshrit Shtossel <oshritvig@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

