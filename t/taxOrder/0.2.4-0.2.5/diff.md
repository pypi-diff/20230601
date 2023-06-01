# Comparing `tmp/taxOrder-0.2.4.tar.gz` & `tmp/taxOrder-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/felixl/PycharmProjects/taxOrder/dist/tmpwr9jxhcq/taxOrder-0.2.4.tar", last modified: Thu Jun  1 10:06:36 2023, max compression
+gzip compressed data, was "/home/felixl/PycharmProjects/taxOrder/dist/tmpa_poq_li/taxOrder-0.2.5.tar", last modified: Thu Jun  1 11:03:55 2023, max compression
```

## Comparing `taxOrder-0.2.4.tar` & `taxOrder-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 10:06:36.000000 taxOrder-0.2.4/
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2022-12-01 13:23:00.000000 taxOrder-0.2.4/taxOrder/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     1121 2023-06-01 09:48:54.000000 taxOrder-0.2.4/taxOrder/ordering.py
--rw-r--r--   0 felixl   (10024) users      (501)       14 2022-12-01 13:28:58.000000 taxOrder-0.2.4/taxOrder/requirements.txt
--rw-r--r--   0 felixl   (10024) users      (501)     1932 2023-06-01 10:05:46.000000 taxOrder-0.2.4/taxOrder/taxOrder.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder.egg-info/
--rw-r--r--   0 felixl   (10024) users      (501)     1523 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder.egg-info/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)      309 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder.egg-info/SOURCES.txt
--rw-r--r--   0 felixl   (10024) users      (501)        1 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder.egg-info/dependency_links.txt
--rw-r--r--   0 felixl   (10024) users      (501)       53 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder.egg-info/entry_points.txt
--rw-r--r--   0 felixl   (10024) users      (501)       15 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder.egg-info/requires.txt
--rw-r--r--   0 felixl   (10024) users      (501)        9 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder.egg-info/top_level.txt
--rw-r--r--   0 felixl   (10024) users      (501)    35148 2022-12-01 14:14:30.000000 taxOrder-0.2.4/LICENSE
--rw-r--r--   0 felixl   (10024) users      (501)      948 2023-06-01 09:50:08.000000 taxOrder-0.2.4/README.md
--rw-r--r--   0 felixl   (10024) users      (501)     1020 2023-06-01 10:06:16.000000 taxOrder-0.2.4/setup.py
--rw-r--r--   0 felixl   (10024) users      (501)     1523 2023-06-01 10:06:36.000000 taxOrder-0.2.4/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)       38 2023-06-01 10:06:36.000000 taxOrder-0.2.4/setup.cfg
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 11:03:55.000000 taxOrder-0.2.5/
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 11:03:55.000000 taxOrder-0.2.5/taxOrder/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2022-12-01 13:23:00.000000 taxOrder-0.2.5/taxOrder/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1932 2023-06-01 10:05:46.000000 taxOrder-0.2.5/taxOrder/cmdline_taxOrder.py
+-rw-r--r--   0 felixl   (10024) users      (501)       14 2022-12-01 13:28:58.000000 taxOrder-0.2.5/taxOrder/requirements.txt
+-rw-r--r--   0 felixl   (10024) users      (501)     1121 2023-06-01 11:03:23.000000 taxOrder-0.2.5/taxOrder/taxOrder.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 11:03:55.000000 taxOrder-0.2.5/taxOrder.egg-info/
+-rw-r--r--   0 felixl   (10024) users      (501)     1523 2023-06-01 11:03:55.000000 taxOrder-0.2.5/taxOrder.egg-info/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)      317 2023-06-01 11:03:55.000000 taxOrder-0.2.5/taxOrder.egg-info/SOURCES.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        1 2023-06-01 11:03:55.000000 taxOrder-0.2.5/taxOrder.egg-info/dependency_links.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       61 2023-06-01 11:03:55.000000 taxOrder-0.2.5/taxOrder.egg-info/entry_points.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       15 2023-06-01 11:03:55.000000 taxOrder-0.2.5/taxOrder.egg-info/requires.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        9 2023-06-01 11:03:55.000000 taxOrder-0.2.5/taxOrder.egg-info/top_level.txt
+-rw-r--r--   0 felixl   (10024) users      (501)    35148 2022-12-01 14:14:30.000000 taxOrder-0.2.5/LICENSE
+-rw-r--r--   0 felixl   (10024) users      (501)      948 2023-06-01 11:02:50.000000 taxOrder-0.2.5/README.md
+-rw-r--r--   0 felixl   (10024) users      (501)     1028 2023-06-01 11:02:34.000000 taxOrder-0.2.5/setup.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1523 2023-06-01 11:03:55.000000 taxOrder-0.2.5/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)       38 2023-06-01 11:03:55.000000 taxOrder-0.2.5/setup.cfg
```

### Comparing `taxOrder-0.2.4/taxOrder/ordering.py` & `taxOrder-0.2.5/taxOrder/taxOrder.py`

 * *Files identical despite different names*

### Comparing `taxOrder-0.2.4/taxOrder/taxOrder.py` & `taxOrder-0.2.5/taxOrder/cmdline_taxOrder.py`

 * *Files identical despite different names*

### Comparing `taxOrder-0.2.4/taxOrder.egg-info/PKG-INFO` & `taxOrder-0.2.5/taxOrder.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxOrder
-Version: 0.2.4
+Version: 0.2.5
 Summary: Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
 Home-page: UNKNOWN
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Package:
 ```
-from taxOrder.ordering import order_taxa
+from taxOrder.taxOrder import order_taxa
 
 taxorder = order_taxa(tree, 'Homo_sapiens', format=1, idmap='')
 ```
 
 
 Command line implementation:
 ```
```

### Comparing `taxOrder-0.2.4/LICENSE` & `taxOrder-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `taxOrder-0.2.4/README.md` & `taxOrder-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Package:
 ```
-from taxOrder.ordering import order_taxa
+from taxOrder.taxOrder import order_taxa
 
 taxorder = order_taxa(tree, 'Homo_sapiens', format=1, idmap='')
 ```
 
 
 Command line implementation:
 ```
```

### Comparing `taxOrder-0.2.4/setup.py` & `taxOrder-0.2.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="taxOrder",
-    version="0.2.4",
+    version="0.2.5",
     #python_requires='>=3.7.0',
     description="Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species",
     author="Felix Langschied",
     author_email="langschied@bio.uni-frankfurt.de",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(include=['taxOrder', 'taxOrder.*']),
@@ -17,15 +17,15 @@
     install_requires=[
         'ete3',
         'six',
         'numpy'
     ],
     license="GPL-3.0",
     entry_points={
-        'console_scripts': ["taxOrder = taxOrder.taxOrder:main"],
+        'console_scripts': ["taxOrder = taxOrder.cmdline_taxOrder:main"],
     },
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Natural Language :: English",
     ],
```

### Comparing `taxOrder-0.2.4/PKG-INFO` & `taxOrder-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxOrder
-Version: 0.2.4
+Version: 0.2.5
 Summary: Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
 Home-page: UNKNOWN
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Package:
 ```
-from taxOrder.ordering import order_taxa
+from taxOrder.taxOrder import order_taxa
 
 taxorder = order_taxa(tree, 'Homo_sapiens', format=1, idmap='')
 ```
 
 
 Command line implementation:
 ```
```

