# Comparing `tmp/taxOrder-0.1.2.tar.gz` & `tmp/taxOrder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/felixl/PycharmProjects/taxOrder/dist/.tmp-ch2guca8/taxOrder-0.1.2.tar", last modified: Thu Dec  1 15:34:50 2022, max compression
+gzip compressed data, was "taxOrder-0.2.0.tar", last modified: Thu Jun  1 09:16:17 2023, max compression
```

## Comparing `taxOrder-0.1.2.tar` & `taxOrder-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2022-12-01 15:34:50.380270 taxOrder-0.1.2/
--rw-r--r--   0 felixl   (10024) users      (501)    35148 2022-12-01 14:14:30.000000 taxOrder-0.1.2/LICENSE
--rw-r--r--   0 felixl   (10024) users      (501)     1325 2022-12-01 15:34:50.378269 taxOrder-0.1.2/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)      789 2022-12-01 14:19:52.000000 taxOrder-0.1.2/README.md
--rw-r--r--   0 felixl   (10024) users      (501)       38 2022-12-01 15:34:50.381271 taxOrder-0.1.2/setup.cfg
--rw-r--r--   0 felixl   (10024) users      (501)      986 2022-12-01 15:34:36.000000 taxOrder-0.1.2/setup.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2022-12-01 15:34:49.973296 taxOrder-0.1.2/taxOrder/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2022-12-01 13:23:00.000000 taxOrder-0.1.2/taxOrder/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)       14 2022-12-01 13:28:58.000000 taxOrder-0.1.2/taxOrder/requirements.txt
--rw-r--r--   0 felixl   (10024) users      (501)     2943 2022-12-01 14:05:50.000000 taxOrder-0.1.2/taxOrder/taxOrder.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2022-12-01 15:34:50.062286 taxOrder-0.1.2/taxOrder.egg-info/
--rw-r--r--   0 felixl   (10024) users      (501)     1325 2022-12-01 15:34:49.000000 taxOrder-0.1.2/taxOrder.egg-info/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)      288 2022-12-01 15:34:49.000000 taxOrder-0.1.2/taxOrder.egg-info/SOURCES.txt
--rw-r--r--   0 felixl   (10024) users      (501)        1 2022-12-01 15:34:49.000000 taxOrder-0.1.2/taxOrder.egg-info/dependency_links.txt
--rw-r--r--   0 felixl   (10024) users      (501)       52 2022-12-01 15:34:49.000000 taxOrder-0.1.2/taxOrder.egg-info/entry_points.txt
--rw-r--r--   0 felixl   (10024) users      (501)       15 2022-12-01 15:34:49.000000 taxOrder-0.1.2/taxOrder.egg-info/requires.txt
--rw-r--r--   0 felixl   (10024) users      (501)        9 2022-12-01 15:34:49.000000 taxOrder-0.1.2/taxOrder.egg-info/top_level.txt
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:16:17.304694 taxOrder-0.2.0/
+-rw-r--r--   0 felixl   (10024) users      (501)    35148 2022-12-01 14:14:30.000000 taxOrder-0.2.0/LICENSE
+-rw-r--r--   0 felixl   (10024) users      (501)     1325 2023-06-01 09:16:17.302703 taxOrder-0.2.0/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)      789 2022-12-01 14:19:52.000000 taxOrder-0.2.0/README.md
+-rw-r--r--   0 felixl   (10024) users      (501)       38 2023-06-01 09:16:17.305695 taxOrder-0.2.0/setup.cfg
+-rw-r--r--   0 felixl   (10024) users      (501)      986 2023-06-01 09:15:31.000000 taxOrder-0.2.0/setup.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:16:17.270702 taxOrder-0.2.0/taxOrder/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2022-12-01 13:23:00.000000 taxOrder-0.2.0/taxOrder/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)       14 2022-12-01 13:28:58.000000 taxOrder-0.2.0/taxOrder/requirements.txt
+-rw-r--r--   0 felixl   (10024) users      (501)     3001 2023-06-01 09:12:18.000000 taxOrder-0.2.0/taxOrder/taxOrder.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:16:17.297698 taxOrder-0.2.0/taxOrder.egg-info/
+-rw-r--r--   0 felixl   (10024) users      (501)     1325 2023-06-01 09:16:17.000000 taxOrder-0.2.0/taxOrder.egg-info/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)      288 2023-06-01 09:16:17.000000 taxOrder-0.2.0/taxOrder.egg-info/SOURCES.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        1 2023-06-01 09:16:17.000000 taxOrder-0.2.0/taxOrder.egg-info/dependency_links.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       52 2023-06-01 09:16:17.000000 taxOrder-0.2.0/taxOrder.egg-info/entry_points.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       15 2023-06-01 09:16:17.000000 taxOrder-0.2.0/taxOrder.egg-info/requires.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        9 2023-06-01 09:16:17.000000 taxOrder-0.2.0/taxOrder.egg-info/top_level.txt
```

### Comparing `taxOrder-0.1.2/LICENSE` & `taxOrder-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taxOrder-0.1.2/PKG-INFO` & `taxOrder-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxOrder
-Version: 0.1.2
+Version: 0.2.0
 Summary: Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `taxOrder-0.1.2/README.md` & `taxOrder-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `taxOrder-0.1.2/setup.py` & `taxOrder-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="taxOrder",
-    version="0.1.2",
+    version="0.2.0",
     #python_requires='>=3.7.0',
     description="Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species",
     author="Felix Langschied",
     author_email="langschied@bio.uni-frankfurt.de",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `taxOrder-0.1.2/taxOrder/taxOrder.py` & `taxOrder-0.2.0/taxOrder/taxOrder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,57 @@
 import ete3 as ete
 import argparse
 import os
 
 
+def initial_list(t):
+    copylist = []
+    node = t.search_nodes(name=args.reference)[0]
+    while node:
+        for subnode in node:
+            copylist.append(subnode.name)
+        node = node.up
+    return copylist
+
+def order_species(ilist):
+    specorder = []
+    for name in ilist:
+        if name not in specorder:
+            specorder.append(name)
+    return specorder
+
+def parse_mappingfile(path):
+    n2t = {}
+    with open(path) as sh:
+        for line in sh:
+            taxid, name = line.strip().split()
+            n2t[name] = f'ncbi{taxid}'
+            if len(name.split('_')) > 2:
+                shortname = '_'.join(name.split('_')[:2])
+                n2t[shortname] = f'ncbi{taxid}'
+    return n2t
+
+def check_file(f):
+    if not os.path.isfile(f):
+        raise ValueError(f'File not found at: {f}')
+
+
+def taxOrder(tree, reference, format=1, idmap=''):
+    tree = ete.Tree(args.tree, format=args.format)
+    initial = initial_list(tree)
+    specorder = order_species(initial)
+    # mapping
+    if args.idmap:
+        name2taxid = parse_mappingfile(args.idmap)
+        outnames = [name2taxid[name] for name in specorder]
+    else:
+        outnames = specorder
+    return outnames
+     
+
 def main():
     parser = argparse.ArgumentParser(
         description='Returns list of species in a phylogenetic tree ordered '
                     'by increasing taxonomic distance to a reference species'
     )
     parser.add_argument(
         '-t', '--tree', metavar='<path>', type=str, required=True,
@@ -35,60 +80,23 @@
         help=(
             'TaxOrder can map species names to taxids accepted by '
             'PhyloProfile if supplied with a tab-seperated file like:\n'
             'taxid\tname'
         )
     )
 
-    def initial_list(t):
-        copylist = []
-        node = t.search_nodes(name=args.reference)[0]
-        while node:
-            for subnode in node:
-                copylist.append(subnode.name)
-            node = node.up
-        return copylist
-
-    def order_species(ilist):
-        specorder = []
-        for name in ilist:
-            if name not in specorder:
-                specorder.append(name)
-        return specorder
-
-    def parse_mappingfile(path):
-        n2t = {}
-        with open(path) as sh:
-            for line in sh:
-                taxid, name = line.strip().split()
-                n2t[name] = f'ncbi{taxid}'
-                if len(name.split('_')) > 2:
-                    shortname = '_'.join(name.split('_')[:2])
-                    n2t[shortname] = f'ncbi{taxid}'
-        return n2t
-
-    def check_file(f):
-        if not os.path.isfile(f):
-            raise ValueError(f'File not found at: {f}')
 
     args = parser.parse_args()
     for file in [args.tree, args.idmap, args.outfile]:
         if file:
             check_file(file)
+            
+    # work    
+    outnames = taxOrder(tree, reference, format=format, idmap=idmap)
 
-    # work
-    tree = ete.Tree(args.tree, format=args.format)
-    initial = initial_list(tree)
-    specorder = order_species(initial)
-    # mapping
-    if args.idmap:
-        name2taxid = parse_mappingfile(args.idmap)
-        outnames = [name2taxid[name] for name in specorder]
-    else:
-        outnames = specorder
     # output
     if args.outfile:
         with open(args.outfile, 'w') as of:
             for name in outnames:
                 of.write(f'{name}\n')
     for name in outnames:
         print(name)
```

### Comparing `taxOrder-0.1.2/taxOrder.egg-info/PKG-INFO` & `taxOrder-0.2.0/taxOrder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxOrder
-Version: 0.1.2
+Version: 0.2.0
 Summary: Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

