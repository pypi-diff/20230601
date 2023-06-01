# Comparing `tmp/taxOrder-0.2.3.tar.gz` & `tmp/taxOrder-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/felixl/PycharmProjects/taxOrder/dist/tmpofb4z5jh/taxOrder-0.2.3.tar", last modified: Thu Jun  1 09:51:26 2023, max compression
+gzip compressed data, was "/home/felixl/PycharmProjects/taxOrder/dist/tmpwr9jxhcq/taxOrder-0.2.4.tar", last modified: Thu Jun  1 10:06:36 2023, max compression
```

## Comparing `taxOrder-0.2.3.tar` & `taxOrder-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:51:26.000000 taxOrder-0.2.3/
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:51:26.000000 taxOrder-0.2.3/taxOrder/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2022-12-01 13:23:00.000000 taxOrder-0.2.3/taxOrder/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     1121 2023-06-01 09:48:54.000000 taxOrder-0.2.3/taxOrder/ordering.py
--rw-r--r--   0 felixl   (10024) users      (501)       14 2022-12-01 13:28:58.000000 taxOrder-0.2.3/taxOrder/requirements.txt
--rw-r--r--   0 felixl   (10024) users      (501)     2631 2023-06-01 09:48:55.000000 taxOrder-0.2.3/taxOrder/taxOrder.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:51:26.000000 taxOrder-0.2.3/taxOrder.egg-info/
--rw-r--r--   0 felixl   (10024) users      (501)     1523 2023-06-01 09:51:26.000000 taxOrder-0.2.3/taxOrder.egg-info/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)      309 2023-06-01 09:51:26.000000 taxOrder-0.2.3/taxOrder.egg-info/SOURCES.txt
--rw-r--r--   0 felixl   (10024) users      (501)        1 2023-06-01 09:51:26.000000 taxOrder-0.2.3/taxOrder.egg-info/dependency_links.txt
--rw-r--r--   0 felixl   (10024) users      (501)       53 2023-06-01 09:51:26.000000 taxOrder-0.2.3/taxOrder.egg-info/entry_points.txt
--rw-r--r--   0 felixl   (10024) users      (501)       15 2023-06-01 09:51:26.000000 taxOrder-0.2.3/taxOrder.egg-info/requires.txt
--rw-r--r--   0 felixl   (10024) users      (501)        9 2023-06-01 09:51:26.000000 taxOrder-0.2.3/taxOrder.egg-info/top_level.txt
--rw-r--r--   0 felixl   (10024) users      (501)    35148 2022-12-01 14:14:30.000000 taxOrder-0.2.3/LICENSE
--rw-r--r--   0 felixl   (10024) users      (501)      948 2023-06-01 09:50:08.000000 taxOrder-0.2.3/README.md
--rw-r--r--   0 felixl   (10024) users      (501)     1020 2023-06-01 09:51:15.000000 taxOrder-0.2.3/setup.py
--rw-r--r--   0 felixl   (10024) users      (501)     1523 2023-06-01 09:51:26.000000 taxOrder-0.2.3/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)       38 2023-06-01 09:51:26.000000 taxOrder-0.2.3/setup.cfg
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 10:06:36.000000 taxOrder-0.2.4/
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2022-12-01 13:23:00.000000 taxOrder-0.2.4/taxOrder/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1121 2023-06-01 09:48:54.000000 taxOrder-0.2.4/taxOrder/ordering.py
+-rw-r--r--   0 felixl   (10024) users      (501)       14 2022-12-01 13:28:58.000000 taxOrder-0.2.4/taxOrder/requirements.txt
+-rw-r--r--   0 felixl   (10024) users      (501)     1932 2023-06-01 10:05:46.000000 taxOrder-0.2.4/taxOrder/taxOrder.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder.egg-info/
+-rw-r--r--   0 felixl   (10024) users      (501)     1523 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder.egg-info/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)      309 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder.egg-info/SOURCES.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        1 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder.egg-info/dependency_links.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       53 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder.egg-info/entry_points.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       15 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder.egg-info/requires.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        9 2023-06-01 10:06:36.000000 taxOrder-0.2.4/taxOrder.egg-info/top_level.txt
+-rw-r--r--   0 felixl   (10024) users      (501)    35148 2022-12-01 14:14:30.000000 taxOrder-0.2.4/LICENSE
+-rw-r--r--   0 felixl   (10024) users      (501)      948 2023-06-01 09:50:08.000000 taxOrder-0.2.4/README.md
+-rw-r--r--   0 felixl   (10024) users      (501)     1020 2023-06-01 10:06:16.000000 taxOrder-0.2.4/setup.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1523 2023-06-01 10:06:36.000000 taxOrder-0.2.4/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)       38 2023-06-01 10:06:36.000000 taxOrder-0.2.4/setup.cfg
```

### Comparing `taxOrder-0.2.3/taxOrder/ordering.py` & `taxOrder-0.2.4/taxOrder/ordering.py`

 * *Files identical despite different names*

### Comparing `taxOrder-0.2.3/taxOrder/taxOrder.py` & `taxOrder-0.2.4/taxOrder/taxOrder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,18 @@
-import ete3 as ete
 import argparse
 import os
+from ordering import order_taxa
 
 
-def initial_list(t, reference):
-    copylist = []
-    node = t.search_nodes(name=reference)[0]
-    while node:
-        for subnode in node:
-            copylist.append(subnode.name)
-        node = node.up
-    return copylist
-
-def order_species(ilist):
-    specorder = []
-    for name in ilist:
-        if name not in specorder:
-            specorder.append(name)
-    return specorder
-
-def parse_mappingfile(path):
-    n2t = {}
-    with open(path) as sh:
-        for line in sh:
-            taxid, name = line.strip().split()
-            n2t[name] = f'ncbi{taxid}'
-            if len(name.split('_')) > 2:
-                shortname = '_'.join(name.split('_')[:2])
-                n2t[shortname] = f'ncbi{taxid}'
-    return n2t
 
 def check_file(f):
     if not os.path.isfile(f):
         raise ValueError(f'File not found at: {f}')
 
 
-
-     
-
 def main():
     parser = argparse.ArgumentParser(
         description='Returns list of species in a phylogenetic tree ordered '
                     'by increasing taxonomic distance to a reference species'
     )
     parser.add_argument(
         '-t', '--tree', metavar='<path>', type=str, required=True,
@@ -77,15 +48,15 @@
 
     args = parser.parse_args()
     for file in [args.tree, args.idmap, args.outfile]:
         if file:
             check_file(file)
             
     # work    
-    outnames = taxOrder(tree, reference, format=format, idmap=idmap)
+    outnames = order_taxa(args.tree, args.reference, format=args.format, idmap=args.idmap)
 
     # output
     if args.outfile:
         with open(args.outfile, 'w') as of:
             for name in outnames:
                 of.write(f'{name}\n')
     for name in outnames:
```

### Comparing `taxOrder-0.2.3/taxOrder.egg-info/PKG-INFO` & `taxOrder-0.2.4/taxOrder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxOrder
-Version: 0.2.3
+Version: 0.2.4
 Summary: Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
 Home-page: UNKNOWN
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `taxOrder-0.2.3/LICENSE` & `taxOrder-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `taxOrder-0.2.3/README.md` & `taxOrder-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `taxOrder-0.2.3/setup.py` & `taxOrder-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="taxOrder",
-    version="0.2.3",
+    version="0.2.4",
     #python_requires='>=3.7.0',
     description="Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species",
     author="Felix Langschied",
     author_email="langschied@bio.uni-frankfurt.de",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(include=['taxOrder', 'taxOrder.*']),
```

### Comparing `taxOrder-0.2.3/PKG-INFO` & `taxOrder-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxOrder
-Version: 0.2.3
+Version: 0.2.4
 Summary: Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
 Home-page: UNKNOWN
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

