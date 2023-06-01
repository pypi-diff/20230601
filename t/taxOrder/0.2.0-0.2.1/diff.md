# Comparing `tmp/taxOrder-0.2.0.tar.gz` & `tmp/taxOrder-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taxOrder-0.2.0.tar", last modified: Thu Jun  1 09:16:17 2023, max compression
+gzip compressed data, was "/home/felixl/PycharmProjects/taxOrder/dist/tmp7tfdaqd2/taxOrder-0.2.1.tar", last modified: Thu Jun  1 09:25:05 2023, max compression
```

## Comparing `taxOrder-0.2.0.tar` & `taxOrder-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:16:17.304694 taxOrder-0.2.0/
--rw-r--r--   0 felixl   (10024) users      (501)    35148 2022-12-01 14:14:30.000000 taxOrder-0.2.0/LICENSE
--rw-r--r--   0 felixl   (10024) users      (501)     1325 2023-06-01 09:16:17.302703 taxOrder-0.2.0/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)      789 2022-12-01 14:19:52.000000 taxOrder-0.2.0/README.md
--rw-r--r--   0 felixl   (10024) users      (501)       38 2023-06-01 09:16:17.305695 taxOrder-0.2.0/setup.cfg
--rw-r--r--   0 felixl   (10024) users      (501)      986 2023-06-01 09:15:31.000000 taxOrder-0.2.0/setup.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:16:17.270702 taxOrder-0.2.0/taxOrder/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2022-12-01 13:23:00.000000 taxOrder-0.2.0/taxOrder/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)       14 2022-12-01 13:28:58.000000 taxOrder-0.2.0/taxOrder/requirements.txt
--rw-r--r--   0 felixl   (10024) users      (501)     3001 2023-06-01 09:12:18.000000 taxOrder-0.2.0/taxOrder/taxOrder.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:16:17.297698 taxOrder-0.2.0/taxOrder.egg-info/
--rw-r--r--   0 felixl   (10024) users      (501)     1325 2023-06-01 09:16:17.000000 taxOrder-0.2.0/taxOrder.egg-info/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)      288 2023-06-01 09:16:17.000000 taxOrder-0.2.0/taxOrder.egg-info/SOURCES.txt
--rw-r--r--   0 felixl   (10024) users      (501)        1 2023-06-01 09:16:17.000000 taxOrder-0.2.0/taxOrder.egg-info/dependency_links.txt
--rw-r--r--   0 felixl   (10024) users      (501)       52 2023-06-01 09:16:17.000000 taxOrder-0.2.0/taxOrder.egg-info/entry_points.txt
--rw-r--r--   0 felixl   (10024) users      (501)       15 2023-06-01 09:16:17.000000 taxOrder-0.2.0/taxOrder.egg-info/requires.txt
--rw-r--r--   0 felixl   (10024) users      (501)        9 2023-06-01 09:16:17.000000 taxOrder-0.2.0/taxOrder.egg-info/top_level.txt
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:25:05.000000 taxOrder-0.2.1/
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2022-12-01 13:23:00.000000 taxOrder-0.2.1/taxOrder/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)       14 2022-12-01 13:28:58.000000 taxOrder-0.2.1/taxOrder/requirements.txt
+-rw-r--r--   0 felixl   (10024) users      (501)     3003 2023-06-01 09:23:43.000000 taxOrder-0.2.1/taxOrder/taxOrder.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder.egg-info/
+-rw-r--r--   0 felixl   (10024) users      (501)     1516 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder.egg-info/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)      288 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder.egg-info/SOURCES.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        1 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder.egg-info/dependency_links.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       53 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder.egg-info/entry_points.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       15 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder.egg-info/requires.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        9 2023-06-01 09:25:05.000000 taxOrder-0.2.1/taxOrder.egg-info/top_level.txt
+-rw-r--r--   0 felixl   (10024) users      (501)    35148 2022-12-01 14:14:30.000000 taxOrder-0.2.1/LICENSE
+-rw-r--r--   0 felixl   (10024) users      (501)      941 2023-06-01 09:24:02.000000 taxOrder-0.2.1/README.md
+-rw-r--r--   0 felixl   (10024) users      (501)      986 2023-06-01 09:23:42.000000 taxOrder-0.2.1/setup.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1516 2023-06-01 09:25:05.000000 taxOrder-0.2.1/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)       38 2023-06-01 09:25:05.000000 taxOrder-0.2.1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `taxOrder-0.2.0/LICENSE` & `taxOrder-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taxOrder-0.2.0/PKG-INFO` & `taxOrder-0.2.1/taxOrder.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 Metadata-Version: 2.1
 Name: taxOrder
-Version: 0.2.0
+Version: 0.2.1
 Summary: Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
+Home-page: UNKNOWN
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
+Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-usage: taxOrder.py [-h] -t <path> -r str [--outfile [str]] [--format [str]] [--idmap [<path>]]
+Package:
+```
+from taxOrder import order_taxa
+
+taxorder = order_taxa(tree, 'Homo_sapiens', format=1, --idmap='')
+```
+
+
+Command line implementation:
+```
+usage: taxOrder [-h] -t <path> -r str [--outfile [str]] [--format [str]] [--idmap [<path>]]
 
 Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
 
 
   -h, --help            show this help message and exit
 
   -t <path>, --tree <path>
@@ -28,7 +40,10 @@
 optional arguments:
 
   --outfile [str]       Save output to file
 
   --format [str]        Tree format as specified at: https://etetoolkit.org/docs/latest/tutorial/tutorial_trees.html#reading-and-writing-newick-trees (Default: 1)
 
   --idmap [<path>]      TaxOrder can map species names to taxids accepted by PhyloProfile if supplied with a tab-seperated file like: taxid name
+```
+
+
```

### Comparing `taxOrder-0.2.0/README.md` & `taxOrder-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,18 @@
-usage: taxOrder.py [-h] -t <path> -r str [--outfile [str]] [--format [str]] [--idmap [<path>]]
+Package:
+```
+from taxOrder import order_taxa
+
+taxorder = order_taxa(tree, 'Homo_sapiens', format=1, --idmap='')
+```
+
+
+Command line implementation:
+```
+usage: taxOrder [-h] -t <path> -r str [--outfile [str]] [--format [str]] [--idmap [<path>]]
 
 Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
 
 
   -h, --help            show this help message and exit
 
   -t <path>, --tree <path>
@@ -14,7 +24,8 @@
 optional arguments:
 
   --outfile [str]       Save output to file
 
   --format [str]        Tree format as specified at: https://etetoolkit.org/docs/latest/tutorial/tutorial_trees.html#reading-and-writing-newick-trees (Default: 1)
 
   --idmap [<path>]      TaxOrder can map species names to taxids accepted by PhyloProfile if supplied with a tab-seperated file like: taxid name
+```
```

### Comparing `taxOrder-0.2.0/setup.py` & `taxOrder-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="taxOrder",
-    version="0.2.0",
+    version="0.2.1",
     #python_requires='>=3.7.0',
     description="Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species",
     author="Felix Langschied",
     author_email="langschied@bio.uni-frankfurt.de",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `taxOrder-0.2.0/taxOrder/taxOrder.py` & `taxOrder-0.2.1/taxOrder/taxOrder.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     return n2t
 
 def check_file(f):
     if not os.path.isfile(f):
         raise ValueError(f'File not found at: {f}')
 
 
-def taxOrder(tree, reference, format=1, idmap=''):
+def order_taxa(tree, reference, format=1, idmap=''):
     tree = ete.Tree(args.tree, format=args.format)
     initial = initial_list(tree)
     specorder = order_species(initial)
     # mapping
     if args.idmap:
         name2taxid = parse_mappingfile(args.idmap)
         outnames = [name2taxid[name] for name in specorder]
```

### Comparing `taxOrder-0.2.0/taxOrder.egg-info/PKG-INFO` & `taxOrder-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 Metadata-Version: 2.1
 Name: taxOrder
-Version: 0.2.0
+Version: 0.2.1
 Summary: Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
+Home-page: UNKNOWN
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
+Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-usage: taxOrder.py [-h] -t <path> -r str [--outfile [str]] [--format [str]] [--idmap [<path>]]
+Package:
+```
+from taxOrder import order_taxa
+
+taxorder = order_taxa(tree, 'Homo_sapiens', format=1, --idmap='')
+```
+
+
+Command line implementation:
+```
+usage: taxOrder [-h] -t <path> -r str [--outfile [str]] [--format [str]] [--idmap [<path>]]
 
 Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
 
 
   -h, --help            show this help message and exit
 
   -t <path>, --tree <path>
@@ -28,7 +40,10 @@
 optional arguments:
 
   --outfile [str]       Save output to file
 
   --format [str]        Tree format as specified at: https://etetoolkit.org/docs/latest/tutorial/tutorial_trees.html#reading-and-writing-newick-trees (Default: 1)
 
   --idmap [<path>]      TaxOrder can map species names to taxids accepted by PhyloProfile if supplied with a tab-seperated file like: taxid name
+```
+
+
```

