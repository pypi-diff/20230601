# Comparing `tmp/taxOrder-0.2.1.tar.gz` & `tmp/taxOrder-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/felixl/PycharmProjects/taxOrder/dist/tmp7tfdaqd2/taxOrder-0.2.1.tar", last modified: Thu Jun  1 09:25:05 2023, max compression
+gzip compressed data, was "/home/felixl/PycharmProjects/taxOrder/dist/tmp5e2_pqs_/taxOrder-0.2.2.tar", last modified: Thu Jun  1 09:32:15 2023, max compression
```

## Comparing `taxOrder-0.2.1.tar` & `taxOrder-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:25:05.000000 taxOrder-0.2.1/
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2022-12-01 13:23:00.000000 taxOrder-0.2.1/taxOrder/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)       14 2022-12-01 13:28:58.000000 taxOrder-0.2.1/taxOrder/requirements.txt
--rw-r--r--   0 felixl   (10024) users      (501)     3003 2023-06-01 09:23:43.000000 taxOrder-0.2.1/taxOrder/taxOrder.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder.egg-info/
--rw-r--r--   0 felixl   (10024) users      (501)     1516 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder.egg-info/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)      288 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder.egg-info/SOURCES.txt
--rw-r--r--   0 felixl   (10024) users      (501)        1 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder.egg-info/dependency_links.txt
--rw-r--r--   0 felixl   (10024) users      (501)       53 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder.egg-info/entry_points.txt
--rw-r--r--   0 felixl   (10024) users      (501)       15 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder.egg-info/requires.txt
--rw-r--r--   0 felixl   (10024) users      (501)        9 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder.egg-info/top_level.txt
--rw-r--r--   0 felixl   (10024) users      (501)    35148 2022-12-01 14:14:30.000000 taxOrder-0.2.1/LICENSE
--rw-r--r--   0 felixl   (10024) users      (501)      941 2023-06-01 09:24:02.000000 taxOrder-0.2.1/README.md
--rw-r--r--   0 felixl   (10024) users      (501)      986 2023-06-01 09:23:42.000000 taxOrder-0.2.1/setup.py
--rw-r--r--   0 felixl   (10024) users      (501)     1516 2023-06-01 09:25:05.000000 taxOrder-0.2.1/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)       38 2023-06-01 09:25:05.000000 taxOrder-0.2.1/setup.cfg
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:32:15.000000 taxOrder-0.2.2/
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:32:15.000000 taxOrder-0.2.2/taxOrder/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2022-12-01 13:23:00.000000 taxOrder-0.2.2/taxOrder/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)       14 2022-12-01 13:28:58.000000 taxOrder-0.2.2/taxOrder/requirements.txt
+-rw-r--r--   0 felixl   (10024) users      (501)     3003 2023-06-01 09:23:43.000000 taxOrder-0.2.2/taxOrder/taxOrder.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:32:15.000000 taxOrder-0.2.2/taxOrder.egg-info/
+-rw-r--r--   0 felixl   (10024) users      (501)     1514 2023-06-01 09:32:15.000000 taxOrder-0.2.2/taxOrder.egg-info/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)      288 2023-06-01 09:32:15.000000 taxOrder-0.2.2/taxOrder.egg-info/SOURCES.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        1 2023-06-01 09:32:15.000000 taxOrder-0.2.2/taxOrder.egg-info/dependency_links.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       53 2023-06-01 09:32:15.000000 taxOrder-0.2.2/taxOrder.egg-info/entry_points.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       15 2023-06-01 09:32:15.000000 taxOrder-0.2.2/taxOrder.egg-info/requires.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        9 2023-06-01 09:32:15.000000 taxOrder-0.2.2/taxOrder.egg-info/top_level.txt
+-rw-r--r--   0 felixl   (10024) users      (501)    35148 2022-12-01 14:14:30.000000 taxOrder-0.2.2/LICENSE
+-rw-r--r--   0 felixl   (10024) users      (501)      939 2023-06-01 09:27:11.000000 taxOrder-0.2.2/README.md
+-rw-r--r--   0 felixl   (10024) users      (501)     1020 2023-06-01 09:31:58.000000 taxOrder-0.2.2/setup.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1514 2023-06-01 09:32:15.000000 taxOrder-0.2.2/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)       38 2023-06-01 09:32:15.000000 taxOrder-0.2.2/setup.cfg
```

### Comparing `taxOrder-0.2.1/taxOrder/taxOrder.py` & `taxOrder-0.2.2/taxOrder/taxOrder.py`

 * *Files identical despite different names*

### Comparing `taxOrder-0.2.1/taxOrder.egg-info/PKG-INFO` & `taxOrder-0.2.2/taxOrder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxOrder
-Version: 0.2.1
+Version: 0.2.2
 Summary: Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
 Home-page: UNKNOWN
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -14,15 +14,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Package:
 ```
 from taxOrder import order_taxa
 
-taxorder = order_taxa(tree, 'Homo_sapiens', format=1, --idmap='')
+taxorder = order_taxa(tree, 'Homo_sapiens', format=1, idmap='')
 ```
 
 
 Command line implementation:
 ```
 usage: taxOrder [-h] -t <path> -r str [--outfile [str]] [--format [str]] [--idmap [<path>]]
```

### Comparing `taxOrder-0.2.1/LICENSE` & `taxOrder-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taxOrder-0.2.1/README.md` & `taxOrder-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Package:
 ```
 from taxOrder import order_taxa
 
-taxorder = order_taxa(tree, 'Homo_sapiens', format=1, --idmap='')
+taxorder = order_taxa(tree, 'Homo_sapiens', format=1, idmap='')
 ```
 
 
 Command line implementation:
 ```
 usage: taxOrder [-h] -t <path> -r str [--outfile [str]] [--format [str]] [--idmap [<path>]]
```

### Comparing `taxOrder-0.2.1/setup.py` & `taxOrder-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="taxOrder",
-    version="0.2.1",
+    version="0.2.2",
     #python_requires='>=3.7.0',
     description="Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species",
     author="Felix Langschied",
     author_email="langschied@bio.uni-frankfurt.de",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=find_packages(),
+    packages=find_packages(include=['taxOrder', 'taxOrder.*']),
     package_data={'': ['*']},
     install_requires=[
         'ete3',
         'six',
         'numpy'
     ],
     license="GPL-3.0",
```

### Comparing `taxOrder-0.2.1/PKG-INFO` & `taxOrder-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxOrder
-Version: 0.2.1
+Version: 0.2.2
 Summary: Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
 Home-page: UNKNOWN
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -14,15 +14,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Package:
 ```
 from taxOrder import order_taxa
 
-taxorder = order_taxa(tree, 'Homo_sapiens', format=1, --idmap='')
+taxorder = order_taxa(tree, 'Homo_sapiens', format=1, idmap='')
 ```
 
 
 Command line implementation:
 ```
 usage: taxOrder [-h] -t <path> -r str [--outfile [str]] [--format [str]] [--idmap [<path>]]
```

