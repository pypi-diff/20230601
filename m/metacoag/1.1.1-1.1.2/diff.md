# Comparing `tmp/metacoag-1.1.1.tar.gz` & `tmp/metacoag-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metacoag-1.1.1.tar", last modified: Wed Feb 22 00:23:46 2023, max compression
+gzip compressed data, was "metacoag-1.1.2.tar", last modified: Thu Jun  1 01:32:41 2023, max compression
```

## Comparing `metacoag-1.1.1.tar` & `metacoag-1.1.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:23:46.882069 metacoag-1.1.1/
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     5232 2023-02-14 12:16:54.000000 metacoag-1.1.1/CODE_OF_CONDUCT.md
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)    35149 2023-02-14 12:16:54.000000 metacoag-1.1.1/LICENSE
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      343 2023-02-14 12:16:54.000000 metacoag-1.1.1/MANIFEST.in
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10026 2023-02-22 00:23:46.881418 metacoag-1.1.1/PKG-INFO
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     9308 2023-02-14 12:16:54.000000 metacoag-1.1.1/README.md
--rwxrwxr-x   0 vijinimallawaarachchi   (501) staff       (20)    34459 2023-02-14 12:16:54.000000 metacoag-1.1.1/metacoag
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:23:46.839783 metacoag-1.1.1/metacoag.egg-info/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10026 2023-02-22 00:23:46.000000 metacoag-1.1.1/metacoag.egg-info/PKG-INFO
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      618 2023-02-22 00:23:46.000000 metacoag-1.1.1/metacoag.egg-info/SOURCES.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2023-02-22 00:23:46.000000 metacoag-1.1.1/metacoag.egg-info/dependency_links.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       72 2023-02-22 00:23:46.000000 metacoag-1.1.1/metacoag.egg-info/entry_points.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       63 2023-02-22 00:23:46.000000 metacoag-1.1.1/metacoag.egg-info/requires.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       15 2023-02-22 00:23:46.000000 metacoag-1.1.1/metacoag.egg-info/top_level.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2023-02-22 00:23:46.000000 metacoag-1.1.1/metacoag.egg-info/zip-safe
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:23:46.842700 metacoag-1.1.1/metacoag_utils/
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-14 12:16:54.000000 metacoag-1.1.1/metacoag_utils/__init__.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:23:46.843353 metacoag-1.1.1/metacoag_utils/auxiliary/
--rwxrwxr-x   0 vijinimallawaarachchi   (501) staff       (20) 15929643 2023-02-14 12:16:54.000000 metacoag-1.1.1/metacoag_utils/auxiliary/marker.hmm
--rwxrwxr-x   0 vijinimallawaarachchi   (501) staff       (20)     1099 2023-02-14 12:16:54.000000 metacoag-1.1.1/metacoag_utils/bidirectionalmap.py
--rwxrwxr-x   0 vijinimallawaarachchi   (501) staff       (20)     6535 2023-02-14 12:16:54.000000 metacoag-1.1.1/metacoag_utils/feature_utils.py
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     8929 2023-02-14 12:16:54.000000 metacoag-1.1.1/metacoag_utils/file_utils.py
--rwxrwxr-x   0 vijinimallawaarachchi   (501) staff       (20)    10906 2023-02-14 12:16:54.000000 metacoag-1.1.1/metacoag_utils/graph_utils.py
--rwxrwxr-x   0 vijinimallawaarachchi   (501) staff       (20)    15011 2023-02-14 12:16:54.000000 metacoag-1.1.1/metacoag_utils/label_prop_utils.py
--rwxrwxr-x   0 vijinimallawaarachchi   (501) staff       (20)     8793 2023-02-14 12:16:54.000000 metacoag-1.1.1/metacoag_utils/marker_gene_utils.py
--rwxrwxr-x   0 vijinimallawaarachchi   (501) staff       (20)    15685 2023-02-14 12:16:54.000000 metacoag-1.1.1/metacoag_utils/matching_utils.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:23:46.880409 metacoag-1.1.1/metacoag_utils/support/
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     2043 2023-02-14 12:16:54.000000 metacoag-1.1.1/metacoag_utils/support/combine_cov.py
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       38 2023-02-22 00:23:46.882282 metacoag-1.1.1/setup.cfg
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     1558 2023-02-14 12:16:54.000000 metacoag-1.1.1/setup.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-01 01:32:41.141706 metacoag-1.1.2/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     5232 2022-08-05 12:06:27.000000 metacoag-1.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    35149 2022-08-05 12:06:27.000000 metacoag-1.1.2/LICENSE
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      343 2023-02-14 12:08:36.000000 metacoag-1.1.2/MANIFEST.in
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10606 2023-06-01 01:32:41.141408 metacoag-1.1.2/PKG-INFO
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     9888 2023-06-01 00:40:34.000000 metacoag-1.1.2/README.md
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    39264 2023-06-01 01:01:19.000000 metacoag-1.1.2/metacoag
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-01 01:32:41.026621 metacoag-1.1.2/metacoag.egg-info/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10606 2023-06-01 01:32:40.000000 metacoag-1.1.2/metacoag.egg-info/PKG-INFO
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      647 2023-06-01 01:32:40.000000 metacoag-1.1.2/metacoag.egg-info/SOURCES.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2023-06-01 01:32:40.000000 metacoag-1.1.2/metacoag.egg-info/dependency_links.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       72 2023-06-01 01:32:40.000000 metacoag-1.1.2/metacoag.egg-info/entry_points.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       69 2023-06-01 01:32:40.000000 metacoag-1.1.2/metacoag.egg-info/requires.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       15 2023-06-01 01:32:40.000000 metacoag-1.1.2/metacoag.egg-info/top_level.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2022-11-25 05:01:14.000000 metacoag-1.1.2/metacoag.egg-info/zip-safe
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-01 01:32:41.029813 metacoag-1.1.2/metacoag_utils/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-06-01 01:29:39.000000 metacoag-1.1.2/metacoag_utils/.DS_Store
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2022-08-05 12:06:27.000000 metacoag-1.1.2/metacoag_utils/__init__.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-01 01:32:41.030145 metacoag-1.1.2/metacoag_utils/auxiliary/
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20) 15929643 2022-08-05 12:06:27.000000 metacoag-1.1.2/metacoag_utils/auxiliary/marker.hmm
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     1099 2022-08-05 12:06:27.000000 metacoag-1.1.2/metacoag_utils/bidirectionalmap.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     6522 2023-05-15 05:51:21.000000 metacoag-1.1.2/metacoag_utils/feature_utils.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    12073 2023-05-15 05:51:35.000000 metacoag-1.1.2/metacoag_utils/graph_utils.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    15011 2023-05-15 04:06:48.000000 metacoag-1.1.2/metacoag_utils/label_prop_utils.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     8598 2023-06-01 00:52:02.000000 metacoag-1.1.2/metacoag_utils/marker_gene_utils.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    15606 2023-05-15 05:49:05.000000 metacoag-1.1.2/metacoag_utils/matching_utils.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-01 01:32:41.140939 metacoag-1.1.2/metacoag_utils/support/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-06-01 01:29:39.000000 metacoag-1.1.2/metacoag_utils/support/.DS_Store
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1745 2023-05-15 06:13:29.000000 metacoag-1.1.2/metacoag_utils/support/combine_cov.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       38 2023-06-01 01:32:41.141789 metacoag-1.1.2/setup.cfg
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1580 2023-05-15 05:58:22.000000 metacoag-1.1.2/setup.py
```

### Comparing `metacoag-1.1.1/CODE_OF_CONDUCT.md` & `metacoag-1.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.1/LICENSE` & `metacoag-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.1/PKG-INFO` & `metacoag-1.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,18 @@
-Metadata-Version: 2.1
-Name: metacoag
-Version: 1.1.1
-Summary: MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
-Home-page: https://github.com/metagentools/MetaCoAG
-Author: Vijini Mallawaarachchi and Yu Lin
-Author-email: viji.mallawaarachchi@gmail.com
-License: GPL-3.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <img src="https://raw.githubusercontent.com/metagentools/MetaCoAG/master/MetaCoAG_Logo.png" width="500" title="MetaCoAG logo" alt="MetaCoAG logo">
 </p>
 
 # MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
 
 [![DOI](https://img.shields.io/badge/DOI-10.1007/978--3--031--04749--7__5-informational)](https://doi.org/10.1007/978-3-031-04749-7_5)
 [![DOI](https://img.shields.io/badge/DOI-10.1089/cmb.2022.0262-green)](https://doi.org/10.1089/cmb.2022.0262)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/metacoag/badges/version.svg)](https://anaconda.org/bioconda/metacoag)
 [![PyPI version](https://badge.fury.io/py/metacoag.svg)](https://badge.fury.io/py/metacoag)
+[![Anaconda-Server Badge](https://anaconda.org/bioconda/metacoag/badges/downloads.svg)](https://anaconda.org/bioconda/metacoag)
 
 [![CI](https://github.com/metagentools/MetaCoAG/actions/workflows/testing.yml/badge.svg)](https://github.com/metagentools/MetaCoAG/actions/workflows/testing.yml)
 ![GitHub](https://img.shields.io/github/license/Vini2/MetaCoAG)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CodeQL](https://github.com/metagentools/MetaCoAG/actions/workflows/codeql.yml/badge.svg)](https://github.com/metagentools/MetaCoAG/actions/workflows/codeql.yml)
 [![Documentation Status](https://readthedocs.org/projects/metacoag/badge/?version=latest)](https://metacoag.readthedocs.io/en/latest/?badge=latest)
 
@@ -37,21 +20,23 @@
 
 For detailed instructions on installation, usage and visualisation, please refer to the [documentation hosted at Read the Docs](https://metacoag.readthedocs.io/).
 
 **NEW:** MetaCoAG is now available on bioconda at 
 [https://anaconda.org/bioconda/metacoag](https://anaconda.org/bioconda/metacoag) and on PyPI at [https://pypi.org/project/metacoag/](https://pypi.org/project/metacoag/).
 
 ## Dependencies
-MetaCoAG installation requires Python 3.7 or above (tested on Python 3.7.4). You will need the following python dependencies to run MetaCoAG and related support scripts. The tested versions of the dependencies are listed as well.
-* [python-igraph](https://igraph.org/python/) - version 0.9.6
-* [biopython](https://biopython.org/) - version 1.74
-* [networkx](https://networkx.github.io/) - version 2.4
-* [scipy](https://www.scipy.org/) - version 1.3.1
-* [numpy](https://numpy.org/) - version 1.17.2
-* [tqdm](https://github.com/tqdm/tqdm) - version 4.36.1
+MetaCoAG installation requires Python 3.7 or above. You will need the following python dependencies to run MetaCoAG and related support scripts. The latest tested versions of the dependencies are listed as well.
+* [python](https://www.python.org/) - version 3.11.0
+* [python-igraph](https://igraph.org/python/) - version 0.10.4
+* [biopython](https://biopython.org/) - version 1.80
+* [networkx](https://networkx.github.io/) - version 3.0
+* [scipy](https://www.scipy.org/) - version 1.10.0
+* [numpy](https://numpy.org/) - version 1.24.2
+* [tqdm](https://github.com/tqdm/tqdm) - version 4.64.1
+* [click](https://click.palletsprojects.com/) - version 8.1.3
 
 MetaCoAG uses the following tools to scan for single-copy marker genes. These tools have been tested on the following versions.
 * [FragGeneScan](https://sourceforge.net/projects/fraggenescan/) - version 1.31
 * [HMMER](http://hmmer.org/) - version 3.3.2
 
 
 ## Installing MetaCoAG using conda
@@ -163,7 +148,15 @@
 doi = {10.1089/cmb.2022.0262},
 note ={PMID: 36367700},
 URL = {https://doi.org/10.1089/cmb.2022.0262},
 eprint = {https://doi.org/10.1089/cmb.2022.0262},
 abstract = { Metagenomics enables the recovery of various genetic materials from different species, thus providing valuable insights into microbial communities. Metagenomic binning group sequences belong to different organisms, which is an important step in the early stages of metagenomic analysis pipelines. The classic pipeline followed in metagenomic binning is to assemble short reads into longer contigs and then bin these resulting contigs into groups representing different taxonomic groups in the metagenomic sample. Most of the currently available binning tools are designed to bin metagenomic contigs, but they do not make use of the assembly graphs that produce such assemblies. In this study, we propose MetaCoAG, a metagenomic binning tool that uses assembly graphs with the composition and coverage information of contigs. MetaCoAG estimates the number of initial bins using single-copy marker genes, assigns contigs into bins iteratively, and adjusts the number of bins dynamically throughout the binning process. We show that MetaCoAG significantly outperforms state-of-the-art binning tools by producing similar or more high-quality bins than the second-best binning tool on both simulated and real datasets. To the best of our knowledge, MetaCoAG is the first stand-alone contig-binning tool that directly makes use of the assembly graph information along with other features of the contigs. }
 }
 ```
+
+## Funding
+
+MetaCoAG is funded by an [Essential Open Source Software for Science Grant](https://chanzuckerberg.com/eoss/proposals/cogent3-python-apis-for-iq-tree-and-graphbin-via-a-plug-in-architecture/) from the Chan Zuckerberg Initiative.
+
+<p align="left">
+  <img src="https://chanzuckerberg.com/wp-content/themes/czi/img/logo.svg" width="300">
+</p>
```

### Comparing `metacoag-1.1.1/README.md` & `metacoag-1.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,36 @@
+Metadata-Version: 2.1
+Name: metacoag
+Version: 1.1.2
+Summary: MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
+Home-page: https://github.com/metagentools/MetaCoAG
+Author: Vijini Mallawaarachchi and Yu Lin
+Author-email: viji.mallawaarachchi@gmail.com
+License: GPL-3.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <img src="https://raw.githubusercontent.com/metagentools/MetaCoAG/master/MetaCoAG_Logo.png" width="500" title="MetaCoAG logo" alt="MetaCoAG logo">
 </p>
 
 # MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
 
 [![DOI](https://img.shields.io/badge/DOI-10.1007/978--3--031--04749--7__5-informational)](https://doi.org/10.1007/978-3-031-04749-7_5)
 [![DOI](https://img.shields.io/badge/DOI-10.1089/cmb.2022.0262-green)](https://doi.org/10.1089/cmb.2022.0262)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/metacoag/badges/version.svg)](https://anaconda.org/bioconda/metacoag)
 [![PyPI version](https://badge.fury.io/py/metacoag.svg)](https://badge.fury.io/py/metacoag)
+[![Anaconda-Server Badge](https://anaconda.org/bioconda/metacoag/badges/downloads.svg)](https://anaconda.org/bioconda/metacoag)
 
 [![CI](https://github.com/metagentools/MetaCoAG/actions/workflows/testing.yml/badge.svg)](https://github.com/metagentools/MetaCoAG/actions/workflows/testing.yml)
 ![GitHub](https://img.shields.io/github/license/Vini2/MetaCoAG)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CodeQL](https://github.com/metagentools/MetaCoAG/actions/workflows/codeql.yml/badge.svg)](https://github.com/metagentools/MetaCoAG/actions/workflows/codeql.yml)
 [![Documentation Status](https://readthedocs.org/projects/metacoag/badge/?version=latest)](https://metacoag.readthedocs.io/en/latest/?badge=latest)
 
@@ -19,21 +38,23 @@
 
 For detailed instructions on installation, usage and visualisation, please refer to the [documentation hosted at Read the Docs](https://metacoag.readthedocs.io/).
 
 **NEW:** MetaCoAG is now available on bioconda at 
 [https://anaconda.org/bioconda/metacoag](https://anaconda.org/bioconda/metacoag) and on PyPI at [https://pypi.org/project/metacoag/](https://pypi.org/project/metacoag/).
 
 ## Dependencies
-MetaCoAG installation requires Python 3.7 or above (tested on Python 3.7.4). You will need the following python dependencies to run MetaCoAG and related support scripts. The tested versions of the dependencies are listed as well.
-* [python-igraph](https://igraph.org/python/) - version 0.9.6
-* [biopython](https://biopython.org/) - version 1.74
-* [networkx](https://networkx.github.io/) - version 2.4
-* [scipy](https://www.scipy.org/) - version 1.3.1
-* [numpy](https://numpy.org/) - version 1.17.2
-* [tqdm](https://github.com/tqdm/tqdm) - version 4.36.1
+MetaCoAG installation requires Python 3.7 or above. You will need the following python dependencies to run MetaCoAG and related support scripts. The latest tested versions of the dependencies are listed as well.
+* [python](https://www.python.org/) - version 3.11.0
+* [python-igraph](https://igraph.org/python/) - version 0.10.4
+* [biopython](https://biopython.org/) - version 1.80
+* [networkx](https://networkx.github.io/) - version 3.0
+* [scipy](https://www.scipy.org/) - version 1.10.0
+* [numpy](https://numpy.org/) - version 1.24.2
+* [tqdm](https://github.com/tqdm/tqdm) - version 4.64.1
+* [click](https://click.palletsprojects.com/) - version 8.1.3
 
 MetaCoAG uses the following tools to scan for single-copy marker genes. These tools have been tested on the following versions.
 * [FragGeneScan](https://sourceforge.net/projects/fraggenescan/) - version 1.31
 * [HMMER](http://hmmer.org/) - version 3.3.2
 
 
 ## Installing MetaCoAG using conda
@@ -145,7 +166,15 @@
 doi = {10.1089/cmb.2022.0262},
 note ={PMID: 36367700},
 URL = {https://doi.org/10.1089/cmb.2022.0262},
 eprint = {https://doi.org/10.1089/cmb.2022.0262},
 abstract = { Metagenomics enables the recovery of various genetic materials from different species, thus providing valuable insights into microbial communities. Metagenomic binning group sequences belong to different organisms, which is an important step in the early stages of metagenomic analysis pipelines. The classic pipeline followed in metagenomic binning is to assemble short reads into longer contigs and then bin these resulting contigs into groups representing different taxonomic groups in the metagenomic sample. Most of the currently available binning tools are designed to bin metagenomic contigs, but they do not make use of the assembly graphs that produce such assemblies. In this study, we propose MetaCoAG, a metagenomic binning tool that uses assembly graphs with the composition and coverage information of contigs. MetaCoAG estimates the number of initial bins using single-copy marker genes, assigns contigs into bins iteratively, and adjusts the number of bins dynamically throughout the binning process. We show that MetaCoAG significantly outperforms state-of-the-art binning tools by producing similar or more high-quality bins than the second-best binning tool on both simulated and real datasets. To the best of our knowledge, MetaCoAG is the first stand-alone contig-binning tool that directly makes use of the assembly graph information along with other features of the contigs. }
 }
 ```
+
+## Funding
+
+MetaCoAG is funded by an [Essential Open Source Software for Science Grant](https://chanzuckerberg.com/eoss/proposals/cogent3-python-apis-for-iq-tree-and-graphbin-via-a-plug-in-architecture/) from the Chan Zuckerberg Initiative.
+
+<p align="left">
+  <img src="https://chanzuckerberg.com/wp-content/themes/czi/img/logo.svg" width="300">
+</p>
```

### Comparing `metacoag-1.1.1/metacoag` & `metacoag-1.1.2/metacoag`

 * *Files 6% similar despite different names*

```diff
@@ -3,120 +3,319 @@
 import concurrent.futures
 import csv
 import gc
 import logging
 import math
 import operator
 import os
+import pathlib
 import subprocess
 import sys
 import time
 
+import click
 from Bio import SeqIO
 from igraph import *
 from tqdm import tqdm
 
-from metacoag_utils import (feature_utils, file_utils, graph_utils,
-                            label_prop_utils, marker_gene_utils,
-                            matching_utils)
+from metacoag_utils import (feature_utils, graph_utils, label_prop_utils,
+                            marker_gene_utils, matching_utils)
 from metacoag_utils.bidirectionalmap import BidirectionalMap
 
 __author__ = "Vijini Mallawaarachchi and Yu Lin"
 __copyright__ = "Copyright 2020, MetaCoAG Project"
 __license__ = "GPL-3.0"
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 __maintainer__ = "Vijini Mallawaarachchi"
 __email__ = "vijini.mallawaarachchi@anu.edu.au"
 __status__ = "Stable Release"
 
-# Set paramters
+
+# Set global paramters
 # ---------------------------------------------------
 
 MAX_WEIGHT = sys.float_info.max
 M_MARKER_GENES = 108
 
 
-def main():
-    # Setup argument parser
-    # ---------------------------------------------------
-
-    args = file_utils.get_args(__version__)
-
-    # Validate arguments
-    validated_args = file_utils.validate(args)
-
-    # Parse arguments
-    assembler = validated_args["assembler"]
-    contigs_file = validated_args["contigs"]
-    assembly_graph_file = validated_args["graph"]
-    contig_paths_file = validated_args["paths"]
-    abundance_file = validated_args["abundance"]
-    output_path = validated_args["output"]
-    prefix = validated_args["prefix"]
-    min_length = validated_args["min_length"]
-    p_intra = validated_args["p_intra"]
-    p_inter = validated_args["p_inter"]
-    depth = validated_args["depth"]
-    mg_threshold = validated_args["mg_threshold"]
-    bin_mg_threshold = validated_args["bin_mg_threshold"]
-    min_bin_size = validated_args["min_bin_size"]
-    hmm = validated_args["hmm"]
-    d_limit = validated_args["d_limit"]
-    delimiter = validated_args["delimiter"]
-    nthreads = validated_args["nthreads"]
+# Setup argument parser
+# ---------------------------------------------------
+
+@click.command()
+@click.option(
+    "--assembler",
+    help="name of the assembler used. (Supports SPAdes, MEGAHIT and Flye)",
+    type=click.Choice(["spades", "megahit", "megahitc", "flye"], case_sensitive=False),
+    required=True,
+)
+@click.option(
+    "--graph",
+    help="path to the assembly graph file",
+    type=click.Path(exists=True),
+    required=True,
+)
+@click.option(
+    "--contigs",
+    help="path to the contigs file",
+    type=click.Path(exists=True),
+    required=True,
+)
+@click.option(
+    "--abundance",
+    help="path to the abundance file",
+    type=click.Path(exists=True),
+    required=True,
+)
+@click.option(
+    "--paths",
+    help="path to the contigs.paths (metaSPAdes) or assembly.info (metaFlye) file",
+    type=click.Path(exists=True),
+    required=False,
+)
+@click.option(
+    "--output",
+    help="path to the output folder",
+    type=click.Path(dir_okay=True, writable=True, readable=True),
+    required=True,
+)
+@click.option(
+    "--hmm",
+    help="path to marker.hmm file.",
+    default=os.path.join(pathlib.Path(__file__).absolute(), "auxiliary", "marker.hmm"),
+    show_default=True,
+    type=click.Path(),
+    required=False,
+)
+@click.option(
+    "--prefix",
+    help="prefix for the output file",
+    type=str,
+    required=False,
+)
+@click.option(
+    "--min_length",
+    help="minimum length of contigs to consider for binning.",
+    type=int,
+    default=1000,
+    show_default=True,
+    required=False,
+)
+@click.option(
+    "--p_intra",
+    help="minimum probability of an edge matching to assign to the same bin.",
+    type=click.FloatRange(0, 1),
+    default=0.1,
+    show_default=True,
+    required=False,
+)
+@click.option(
+    "--p_inter",
+    help="maximum probability of an edge matching to create a new bin.",
+    type=click.FloatRange(0, 1),
+    default=0.01,
+    show_default=True,
+    required=False,
+)
+@click.option(
+    "--d_limit",
+    help="distance limit for contig matching.",
+    type=int,
+    default=20,
+    show_default=True,
+    required=False,
+)
+@click.option(
+    "--depth",
+    help="depth to consider for label propagation.",
+    type=int,
+    default=10,
+    show_default=True,
+    required=False,
+)
+@click.option(
+    "--mg_threshold",
+    help="length threshold to consider marker genes.",
+    type=click.FloatRange(0, 1, clamp=True),
+    default=0.5,
+    show_default=True,
+    required=False,
+)
+@click.option(
+    "--bin_mg_threshold",
+    help="minimum fraction of marker genes that should be present in a bin.",
+    type=click.FloatRange(0, 1, clamp=True),
+    default=0.33333,
+    show_default=True,
+    required=False,
+)
+@click.option(
+    "--min_bin_size",
+    help="minimum size of a bin to output in base pairs (bp).",
+    type=int,
+    default=200000,
+    show_default=True,
+    required=False,
+)
+@click.option(
+    "--delimiter",
+    help="delimiter for output results. Supports a comma (,), a semicolon (;), a tab ($'\\t'), a space (\" \") and a pipe (|) .",
+    type=click.Choice([",", ";", "$'\\t'", "\" \""], case_sensitive=False),
+    default=",",
+    show_default=True,
+    required=False,
+)
+@click.option(
+    "--nthreads",
+    help="number of threads to use.",
+    type=int,
+    default=8,
+    show_default=True,
+    required=False,
+)
+@click.version_option(__version__, "-v", "--version", is_flag=True)
+def main(
+    assembler,
+    graph,
+    contigs,
+    abundance,
+    paths,
+    output,
+    hmm,
+    prefix,
+    min_length,
+    p_intra,
+    p_inter,
+    d_limit,
+    depth,
+    mg_threshold,
+    bin_mg_threshold,
+    min_bin_size,
+    delimiter,
+    nthreads
+):
+    """
+    MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
+    """
+
+    # Parse arguments for paths
+    # ------------------------------------------------------------------------
+
+    contigs_file = contigs
+    assembly_graph_file = graph
+    contig_paths_file = paths
+    abundance_file = abundance
+    output_path = output
 
     bin_threshold = -math.log(p_intra, 10)
     break_threshold = -math.log(p_inter, 10)
 
     n_bins = 0
 
+
     # Setup logger
-    # -----------------------
+    # ------------------------------------------------------------------------
 
-    logger = logging.getLogger("MetaCoaAG 1.1.1")
+    logger = logging.getLogger("MetaCoaAG 1.1.2")
     logger.setLevel(logging.DEBUG)
     logging.captureWarnings(True)
     formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
     consoleHeader = logging.StreamHandler()
     consoleHeader.setFormatter(formatter)
     consoleHeader.setLevel(logging.INFO)
     logger.addHandler(consoleHeader)
 
     # Setup output path for log file
-    fileHandler = logging.FileHandler(output_path + "/" + prefix + "metacoag.log")
+    fileHandler = logging.FileHandler(f"{output_path}/{prefix}metacoag.log")
     fileHandler.setLevel(logging.DEBUG)
     fileHandler.setFormatter(formatter)
     logger.addHandler(fileHandler)
 
+
+    # Validate files
+    # ------------------------------------------------------------------------
+
+    # Check if paths file is provided when the assembler type is SPAdes
+    if assembler.lower() == "spades" and contig_paths_file is None:
+        logger.error("Please make sure to provide the path to the contigs.paths file.")
+        logger.error("Exiting MetaCoAG... Bye...!")
+        sys.exit(1)
+
+    # Check if paths file is provided when the assembler type is Flye
+    if assembler.lower() == "flye" and contig_paths_file is None:
+        logger.error("Please make sure to provide the path to the assembly_info.txt file.")
+        logger.error("Exiting MetaCoAG... Bye...!")
+        sys.exit(1)
+
+    # Skip paths file when the assembler type is MEGAHIT
+    if assembler.lower() == "megahit":
+        contig_paths_file = "None"
+
+    # Validate prefix
+    if prefix != None:
+        if not prefix.endswith("_"):
+            prefix = f"{prefix}_"
+    else:
+        prefix = ""
+
+    # Validate min_bin_size
+    if min_bin_size <= 0:
+        logger.error("Please enter a valid number for min_bin_size")
+        logger.error("Exiting MetaCoAG... Bye...!")
+        sys.exit(1)
+    
+    # Validate depth
+    if depth <= 0:
+        logger.error("Please enter a valid number for depth")
+        logger.error("Exiting MetaCoAG... Bye...!")
+        sys.exit(1)
+
+    # Validate d_limit
+    if d_limit <= 0:
+        logger.error("Please enter a valid number for d_limit")
+        logger.error("Exiting MetaCoAG... Bye...!")
+        sys.exit(1)
+    
+    # Validate number of threads
+    if nthreads <= 0:
+        logger.error("Please enter a valid number for the number of threads")
+        logger.error("Exiting MetaCoAG... Bye...!")
+        sys.exit(1)
+
+
+    # Start MetaCoAG
+    # ------------------------------------------------------------------------
+
     logger.info(
         "Welcome to MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs."
     )
 
     logger.info("Input arguments: ")
-    logger.info("Assembler used: " + assembler)
-    logger.info("Contigs file: " + contigs_file)
-    logger.info("Assembly graph file: " + assembly_graph_file)
-    logger.info("Contig paths file: " + contig_paths_file)
-    logger.info("Abundance file: " + abundance_file)
-    logger.info("Final binning output file: " + output_path)
-    logger.info("Minimum length of contigs to consider: " + str(min_length))
-    logger.info("Depth to consider for label propagation: " + str(depth))
-    logger.info("p_intra: " + str(p_intra))
-    logger.info("p_inter: " + str(p_inter))
-    logger.debug("bin_threshold: " + str(bin_threshold))
-    logger.debug("break_threshold: " + str(break_threshold))
-    logger.info("mg_threshold: " + str(mg_threshold))
-    logger.info("bin_mg_threshold: " + str(bin_mg_threshold))
-    logger.info("min_bin_size: " + str(min_bin_size) + " base pairs")
-    logger.info("d_limit: " + str(d_limit))
-    logger.info("Number of threads: " + str(nthreads))
+    logger.info(f"Assembler used: {assembler}")
+    logger.info(f"Contigs file: {contigs_file}")
+    logger.info(f"Assembly graph file: {assembly_graph_file}")
+    logger.info(f"Contig paths file: {contig_paths_file}")
+    logger.info(f"Abundance file: {abundance_file}")
+    logger.info(f"Final binning output file: {output_path}")
+    logger.info(f"Marker gene file hmm: {hmm}")
+    logger.info(f"Minimum length of contigs to consider: {min_length}")
+    logger.info(f"Depth to consider for label propagation: {depth}")
+    logger.info(f"p_intra: {p_intra}")
+    logger.info(f"p_inter: {p_inter}")
+    logger.debug(f"bin_threshold: {bin_threshold}")
+    logger.debug(f"break_threshold: {break_threshold}")
+    logger.info(f"mg_threshold: {mg_threshold}")
+    logger.info(f"bin_mg_threshold: {bin_mg_threshold}")
+    logger.info(f"min_bin_size: {min_bin_size} base pairs")
+    logger.info(f"d_limit: {d_limit}")
+    logger.info(f"Number of threads: {nthreads}")
+    
     logger.info("MetaCoAG started")
-
     start_time = time.time()
 
+
     # Get links of the assembly graph
     # ------------------------------------------------------------------------
 
     try:
         if assembler == "spades":
             # Get paths, segments, links and contigs of the assembly graph
             (
@@ -167,14 +366,26 @@
                 node_count,
                 contigs_map,
             ) = graph_utils.get_links_flye(contig_paths_file, contig_names_rev)
 
             # Get reverse mapping of contig map
             contigs_map_rev = contigs_map.inverse
 
+        if assembler == "megahitc":
+
+            # Get links and contigs of the assembly graph
+            (
+                node_count,
+                links,
+                contig_names,
+            ) = graph_utils.get_links_megahit_custom(assembly_graph_file)
+
+            # Get reverse mapping of contig identifiers
+            contig_names_rev = contig_names.inverse
+
     except:
         logger.error(
             "Please make sure that the correct path to the contig paths file is provided."
         )
         logger.info("Exiting MetaCoAG... Bye...!")
         sys.exit(1)
 
@@ -185,15 +396,15 @@
 
     try:
         # Create graph
         assembly_graph = Graph()
 
         # Add vertices
         assembly_graph.add_vertices(node_count)
-        logger.info("Total number of contigs available: " + str(node_count))
+        logger.info(f"Total number of contigs available: {node_count}")
 
         # Name vertices with contig identifiers
         for i in range(node_count):
             assembly_graph.vs[i]["id"] = i
             assembly_graph.vs[i]["label"] = contig_names[i]
 
         # Get list of edges
@@ -211,29 +422,26 @@
                 assembly_graph_file=assembly_graph_file,
                 contigs_map=contigs_map,
                 contigs_map_rev=contigs_map_rev,
                 paths=paths,
                 segment_contigs=segment_contigs,
             )
 
-        if assembler == "megahit":
+        if assembler == "megahit" or assembler == "megahitc":
             edge_list = graph_utils.get_graph_edges_megahit(
                 links=links, contig_names_rev=contig_names_rev
             )
 
         # Add edges to the graph
         assembly_graph.add_edges(edge_list)
 
         # Simplify the graph
         assembly_graph.simplify(multiple=True, loops=False, combine_edges=None)
 
-        logger.info(
-            "Total number of edges in the assembly graph: "
-            + str(len(list(assembly_graph.es)))
-        )
+        logger.info(f"Total number of edges in the assembly graph: {len(list(assembly_graph.es))}")
 
     except:
         logger.error(
             "Please make sure that the correct path to the assembly graph file is provided."
         )
         logger.info("Exiting MetaCoAG... Bye...!")
         sys.exit(1)
@@ -247,15 +455,15 @@
                 graph_to_contig_map[n] = n2
 
         graph_to_contig_map_rev = graph_to_contig_map.inverse
 
     # Get isolated contigs with no neighbours
     isolated = graph_utils.get_isolated(node_count, assembly_graph)
 
-    logger.info("Total isolated contigs in the assembly graph: " + str(len(isolated)))
+    logger.info(f"Total isolated contigs in the assembly graph: {len(isolated)}")
 
     # Get the number of samples and the length and coverage of contigs
     # ------------------------------------------------------------------------
 
     logger.info("Obtaining lengths and coverage values of contigs")
 
     if assembler == "megahit":
@@ -288,27 +496,25 @@
         if contig_lengths[contig] >= min_length:
             my_long += 1
 
     for contig in isolated:
         if contig_lengths[contig] >= min_length:
             isolated_long.append(contig)
 
-    logger.info("Total long contigs: " + str(my_long))
-    logger.info(
-        "Total isolated long contigs in the assembly graph: " + str(len(isolated_long))
-    )
+    logger.info(f"Total long contigs: {my_long}")
+    logger.info(f"Total isolated long contigs in the assembly graph: {len(isolated_long)}")
 
     # Set intra weight and inter weight
     # ------------------------------------------------------------------------
 
     w_intra = bin_threshold * (n_samples + 1)
     w_inter = break_threshold * (n_samples + 1)
 
-    logger.debug("w_intra: " + str(w_intra))
-    logger.debug("w_inter: " + str(w_inter))
+    logger.debug(f"w_intra: {w_intra}")
+    logger.debug("w_inter: {w_inter}")
 
     # Get tetramer composition of contigs
     # ------------------------------------------------------------------------
 
     logger.info("Obtaining tetranucleotide frequencies of contigs")
 
     normalized_tetramer_profiles = feature_utils.get_tetramer_profiles(
@@ -324,15 +530,15 @@
     gc.collect()
 
     # Get contigs with marker genes
     # -----------------------------------------------------
 
     logger.info("Scanning for single-copy marker genes")
 
-    if not os.path.exists(contigs_file + ".hmmout"):
+    if not os.path.exists(f"{contigs_file}.hmmout"):
         # Check if FragGeneScan is installed
         try:
             p = subprocess.run(["which", "run_FragGeneScan.pl"], capture_output=True)
             if p.returncode != 0:
                 raise Exception("Command does not exist")
         except:
             logger.error(
@@ -391,18 +597,15 @@
 
         all_contig_markers = marker_gene_utils.get_all_contigs_with_marker_genes(
             contigs_file=contigs_file,
             contig_names_rev=contig_names_rev,
             mg_length_threshold=mg_threshold,
         )
 
-    logger.info(
-        "Number of contigs containing single-copy marker genes: "
-        + str(len(contig_markers))
-    )
+    logger.info(f"Number of contigs containing single-copy marker genes: {len(contig_markers)}")
 
     # Check if there are contigs with single-copy marker genes
     if len(contig_markers) == 0:
         logger.info(
             "Could not find contigs that contain single-copy marker genes. The dataset cannot be binned."
         )
         logger.info("Exiting MetaCoAG... Bye...!")
@@ -476,15 +679,15 @@
         contig_num = smg_iteration[0][i]
 
         bins[i] = [contig_num]
         bin_of_contig[contig_num] = i
 
         bin_markers[i] = contig_markers[contig_num]
 
-    logger.debug("Number of initial bins detected: " + str(len(smg_iteration[0])))
+    logger.debug(f"Number of initial bins detected: {len(smg_iteration[0])}")
     logger.debug("Initialised bins: ")
     logger.debug(bins)
 
     # Assign contigs with single-copy marker genes to bins
     # -----------------------------------------------------
 
     logger.info("Matching and assigning contigs with single-copy marker genes to bins")
@@ -510,25 +713,22 @@
         coverages=coverages,
         assembly_graph=assembly_graph,
         w_intra=w_intra,
         w_inter=w_inter,
         d_limit=d_limit,
     )
 
-    logger.debug("Number of bins after matching: " + str(len(bins)))
+    logger.debug(f"Number of bins after matching: {len(bins)}")
 
     logger.debug("Bins with contigs containing seed marker genes")
 
     for b in bins:
-        logger.debug(str(b) + ": " + str(bins[b]))
+        logger.debug(f"{b}: {bins[b]}")
 
-    logger.debug(
-        "Number of binned contigs with single-copy marker genes: "
-        + str(len(bin_of_contig))
-    )
+    logger.debug(f"Number of binned contigs with single-copy marker genes: {len(bin_of_contig)}")
 
     del smg_iteration
     del my_gene_counts
     del unique_my_gene_counts
     del marker_contigs
     del marker_contig_counts
     del total_contig_mgs
@@ -550,18 +750,15 @@
         unbinned_mg_contig_lengths[contig] = contig_lengths[contigid]
 
     # Sort the unmatched in the the descending order of their contig lengths
     unbinned_mg_contig_lengths_sorted = sorted(
         unbinned_mg_contig_lengths.items(), key=operator.itemgetter(1), reverse=True
     )
 
-    logger.debug(
-        "Number of unbinned contigs with single-copy marker genes: "
-        + str(len(unbinned_mg_contigs))
-    )
+    logger.debug(f"Number of unbinned contigs with single-copy marker genes: {len(unbinned_mg_contigs)}")
 
     logger.info("Further assigning contigs with single-copy marker genes")
 
     # Further assigning unmatched contigs to bins
     (
         bins,
         bin_of_contig,
@@ -583,21 +780,16 @@
     )
 
     # Get remaining contigs with single-copy marker genes which are not assigned to bins
     unbinned_mg_contigs = list(
         set(contig_markers.keys()) - set(binned_contigs_with_markers)
     )
 
-    logger.debug(
-        "Remaining number of unbinned MG seed contigs: " + str(len(unbinned_mg_contigs))
-    )
-    logger.debug(
-        "Number of binned contigs with single-copy marker genes: "
-        + str(len(bin_of_contig))
-    )
+    logger.debug(f"Remaining number of unbinned MG seed contigs: {len(unbinned_mg_contigs)}")
+    logger.debug(f"Number of binned contigs with single-copy marker genes: {len(bin_of_contig)}")
 
     del unbinned_mg_contigs
     del unbinned_mg_contig_lengths
     del unbinned_mg_contig_lengths_sorted
     gc.collect()
 
     # Get seed bin counts and profiles
@@ -623,32 +815,30 @@
     # Get binned and unbinned contigs
     # -----------------------------------------------------
 
     binned_contigs = list(bin_of_contig.keys())
 
     unbinned_contigs = list(set([x for x in range(node_count)]) - set(binned_contigs))
 
-    logger.debug("Number of binned contigs: " + str(len(binned_contigs)))
-    logger.debug("Number of unbinned contigs: " + str(len(unbinned_contigs)))
-    logger.debug(
-        "Number of binned contigs with markers: "
-        + str(len(binned_contigs_with_markers))
-    )
+    logger.debug(f"Number of binned contigs: {len(binned_contigs)}")
+    logger.debug(f"Number of unbinned contigs: {len(unbinned_contigs)}")
+    logger.debug(f"Number of binned contigs with markers: {len(binned_contigs_with_markers)}")
 
     # Get components without labels
     # -----------------------------------------------------
 
     # Get connected contigs within the labelled components
     non_isolated = graph_utils.get_non_isolated(
         node_count=node_count,
         assembly_graph=assembly_graph,
         binned_contigs=binned_contigs,
+        nthreads=nthreads
     )
 
-    logger.debug("Number of non-isolated contigs: " + str(len(non_isolated)))
+    logger.debug(f"Number of non-isolated contigs: {len(non_isolated)}")
 
     # Propagate labels to vertices of unlabelled long contigs
     # -----------------------------------------------------
 
     logger.info("Propagating labels to connected vertices of unlabelled long contigs")
 
     # Label propagation on connected vertices of unlabelled long contigs
@@ -670,15 +860,15 @@
         assembly_graph=assembly_graph,
         normalized_tetramer_profiles=normalized_tetramer_profiles,
         coverages=coverages,
         depth=1,
         weight=w_intra,
     )
 
-    logger.debug("Total number of binned contigs: " + str(len(bin_of_contig)))
+    logger.debug(f"Total number of binned contigs: {len(bin_of_contig)}")
 
     # Further propagate labels to vertices of unlabelled long contigs
     # --------------------------------------------------------------------------------
 
     # Further label propagation on connected vertices of unlabelled long contigs
     (
         bins,
@@ -698,25 +888,25 @@
         assembly_graph=assembly_graph,
         normalized_tetramer_profiles=normalized_tetramer_profiles,
         coverages=coverages,
         depth=depth,
         weight=w_inter,
     )
 
-    logger.debug("Total number of binned contigs: " + str(len(bin_of_contig)))
+    logger.debug(f"Total number of binned contigs: {len(bin_of_contig)}")
 
     # Get binned and unbinned contigs
     # -----------------------------------------------------
 
     binned_contigs = list(bin_of_contig.keys())
 
     unbinned_contigs = list(set([x for x in range(node_count)]) - set(binned_contigs))
 
-    logger.debug("Number of binned contigs: " + str(len(binned_contigs)))
-    logger.debug("Number of unbinned contigs: " + str(len(unbinned_contigs)))
+    logger.debug(f"Number of binned contigs: {len(binned_contigs)}")
+    logger.debug(f"Number of unbinned contigs: {len(unbinned_contigs)}")
 
     # Propagate labels to vertices of unlabelled long contigs in isolated components
     # -----------------------------------------------------------------------------------------------
 
     logger.info("Further propagating labels to vertices of unlabelled long contigs")
 
     # Get long unbinned contigs
@@ -793,15 +983,15 @@
             bin_of_contig=bin_of_contig,
             bin_markers=bin_markers,
             binned_contigs_with_markers=binned_contigs_with_markers,
             contig_markers=contig_markers,
             contig_lengths=contig_lengths,
         )
 
-    logger.debug("Total number of binned contigs: " + str(len(bin_of_contig)))
+    logger.debug(f"Total number of binned contigs: {len(bin_of_contig)}")
 
     #  Further propagate labels to vertices of unlabelled long contigs
     # --------------------------------------------------------------------------------
 
     logger.info(
         "Further propagating labels to connected vertices of unlabelled long contigs"
     )
@@ -824,24 +1014,24 @@
         assembly_graph=assembly_graph,
         normalized_tetramer_profiles=normalized_tetramer_profiles,
         coverages=coverages,
         depth=depth,
         weight=MAX_WEIGHT,
     )
 
-    logger.debug("Total number of binned contigs: " + str(len(bin_of_contig)))
+    logger.debug(f"Total number of binned contigs: {len(bin_of_contig)}")
 
     # Get elapsed time
     # -----------------------------------
 
     # Determine elapsed time
     elapsed_time = time.time() - start_time
 
     # Print elapsed time for the process
-    logger.info("Elapsed time: " + str(elapsed_time) + " seconds")
+    logger.info(f"Elapsed time: {elapsed_time} seconds")
 
     # Get bin sizes
     # -----------------------------------
 
     bin_size = {}
 
     for b in bins:
@@ -867,22 +1057,15 @@
 
     for b in bins:
         possible_bins = []
 
         no_possible_bins = True
 
         logger.debug(
-            "Bin "
-            + str(b)
-            + ": # contigs: "
-            + str(len(bins[b]))
-            + ", bin size: "
-            + str(bin_size[b])
-            + "bp, # markers: "
-            + str(len(bin_markers[b]))
+            f"Bin {b}: # contigs: {len(bins[b])}, bin size: {bin_size[b]}bp, # markers: {len(bin_markers[b])}"
         )
 
         min_pb = -1
         min_pb_weight = MAX_WEIGHT
 
         for pb in bin_markers:
             common_mgs = list(set(bin_markers[pb]).intersection(set(bin_markers[b])))
@@ -944,29 +1127,29 @@
         for b in bin_clique:
             bin_clique_size[bin_name] += bin_size[b]
 
     # Get final list of bins and write result to output file
     # ----------------------------------------------------------
 
     # Get output path
-    output_bins_path = output_path + prefix + "bins/"
-    lq_output_bins_path = output_path + prefix + "low_quality_bins/"
+    output_bins_path = f"{output_path}/{prefix}bins"
+    lq_output_bins_path = f"{output_path}/{prefix}low_quality_bins"
 
     # Create output directory for bin files
     if not os.path.isdir(output_bins_path):
-        subprocess.run("mkdir -p " + output_bins_path, shell=True)
+        subprocess.run(f"mkdir -p {output_bins_path}", shell=True)
     if not os.path.isdir(lq_output_bins_path):
-        subprocess.run("mkdir -p " + lq_output_bins_path, shell=True)
+        subprocess.run(f"mkdir -p {lq_output_bins_path}", shell=True)
 
     final_bins = {}
     lowq_bins = {}
 
     final_bin_count = 0
 
-    with open(output_path + prefix + "contig_to_bin.tsv", mode="w") as out_file:
+    with open(f"{output_path}/{prefix}contig_to_bin.tsv", mode="w") as out_file:
         output_writer = csv.writer(
             out_file, delimiter=delimiter, quotechar='"', quoting=csv.QUOTE_MINIMAL
         )
 
         for bin_clique in bin_cliques:
             bin_name = "_".join(str(x) for x in list(bin_clique))
 
@@ -1003,20 +1186,20 @@
 
     logger.info("Writing the Final Binning result to file")
 
     bin_files = {}
 
     for bin_name in set(final_bins.values()):
         bin_files[bin_name] = open(
-            output_bins_path + prefix + "bin_" + bin_name + ".fasta", "w+"
+            f"{output_bins_path}/{prefix}bin_{bin_name}.fasta", "w+"
         )
 
     for bin_name in set(lowq_bins.values()):
         bin_files[bin_name] = open(
-            lq_output_bins_path + prefix + "bin_" + bin_name + "_seqs.fasta", "w+"
+            f"{lq_output_bins_path}/{prefix}bin_{bin_name}_seqs.fasta", "w+"
         )
 
     for n, record in tqdm(
         enumerate(SeqIO.parse(contigs_file, "fasta")),
         desc="Splitting contigs into bins",
     ):
         if assembler == "megahit":
@@ -1037,16 +1220,16 @@
     # Close output files
     for c in set(final_bins.values()):
         bin_files[c].close()
 
     for c in set(lowq_bins.values()):
         bin_files[c].close()
 
-    logger.info("Producing " + str(final_bin_count) + " bins...")
-    logger.info("Final binning results can be found in " + str(output_bins_path))
+    logger.info(f"Producing {final_bin_count} bins...")
+    logger.info(f"Final binning results can be found in {output_bins_path}")
 
     # Exit program
     # -----------------------------------
 
     logger.info("Thank you for using MetaCoAG!")
```

### Comparing `metacoag-1.1.1/metacoag.egg-info/PKG-INFO` & `metacoag-1.1.2/metacoag.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metacoag
-Version: 1.1.1
+Version: 1.1.2
 Summary: MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
 Home-page: https://github.com/metagentools/MetaCoAG
 Author: Vijini Mallawaarachchi and Yu Lin
 Author-email: viji.mallawaarachchi@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,15 @@
 
 # MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
 
 [![DOI](https://img.shields.io/badge/DOI-10.1007/978--3--031--04749--7__5-informational)](https://doi.org/10.1007/978-3-031-04749-7_5)
 [![DOI](https://img.shields.io/badge/DOI-10.1089/cmb.2022.0262-green)](https://doi.org/10.1089/cmb.2022.0262)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/metacoag/badges/version.svg)](https://anaconda.org/bioconda/metacoag)
 [![PyPI version](https://badge.fury.io/py/metacoag.svg)](https://badge.fury.io/py/metacoag)
+[![Anaconda-Server Badge](https://anaconda.org/bioconda/metacoag/badges/downloads.svg)](https://anaconda.org/bioconda/metacoag)
 
 [![CI](https://github.com/metagentools/MetaCoAG/actions/workflows/testing.yml/badge.svg)](https://github.com/metagentools/MetaCoAG/actions/workflows/testing.yml)
 ![GitHub](https://img.shields.io/github/license/Vini2/MetaCoAG)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CodeQL](https://github.com/metagentools/MetaCoAG/actions/workflows/codeql.yml/badge.svg)](https://github.com/metagentools/MetaCoAG/actions/workflows/codeql.yml)
 [![Documentation Status](https://readthedocs.org/projects/metacoag/badge/?version=latest)](https://metacoag.readthedocs.io/en/latest/?badge=latest)
 
@@ -37,21 +38,23 @@
 
 For detailed instructions on installation, usage and visualisation, please refer to the [documentation hosted at Read the Docs](https://metacoag.readthedocs.io/).
 
 **NEW:** MetaCoAG is now available on bioconda at 
 [https://anaconda.org/bioconda/metacoag](https://anaconda.org/bioconda/metacoag) and on PyPI at [https://pypi.org/project/metacoag/](https://pypi.org/project/metacoag/).
 
 ## Dependencies
-MetaCoAG installation requires Python 3.7 or above (tested on Python 3.7.4). You will need the following python dependencies to run MetaCoAG and related support scripts. The tested versions of the dependencies are listed as well.
-* [python-igraph](https://igraph.org/python/) - version 0.9.6
-* [biopython](https://biopython.org/) - version 1.74
-* [networkx](https://networkx.github.io/) - version 2.4
-* [scipy](https://www.scipy.org/) - version 1.3.1
-* [numpy](https://numpy.org/) - version 1.17.2
-* [tqdm](https://github.com/tqdm/tqdm) - version 4.36.1
+MetaCoAG installation requires Python 3.7 or above. You will need the following python dependencies to run MetaCoAG and related support scripts. The latest tested versions of the dependencies are listed as well.
+* [python](https://www.python.org/) - version 3.11.0
+* [python-igraph](https://igraph.org/python/) - version 0.10.4
+* [biopython](https://biopython.org/) - version 1.80
+* [networkx](https://networkx.github.io/) - version 3.0
+* [scipy](https://www.scipy.org/) - version 1.10.0
+* [numpy](https://numpy.org/) - version 1.24.2
+* [tqdm](https://github.com/tqdm/tqdm) - version 4.64.1
+* [click](https://click.palletsprojects.com/) - version 8.1.3
 
 MetaCoAG uses the following tools to scan for single-copy marker genes. These tools have been tested on the following versions.
 * [FragGeneScan](https://sourceforge.net/projects/fraggenescan/) - version 1.31
 * [HMMER](http://hmmer.org/) - version 3.3.2
 
 
 ## Installing MetaCoAG using conda
@@ -163,7 +166,15 @@
 doi = {10.1089/cmb.2022.0262},
 note ={PMID: 36367700},
 URL = {https://doi.org/10.1089/cmb.2022.0262},
 eprint = {https://doi.org/10.1089/cmb.2022.0262},
 abstract = { Metagenomics enables the recovery of various genetic materials from different species, thus providing valuable insights into microbial communities. Metagenomic binning group sequences belong to different organisms, which is an important step in the early stages of metagenomic analysis pipelines. The classic pipeline followed in metagenomic binning is to assemble short reads into longer contigs and then bin these resulting contigs into groups representing different taxonomic groups in the metagenomic sample. Most of the currently available binning tools are designed to bin metagenomic contigs, but they do not make use of the assembly graphs that produce such assemblies. In this study, we propose MetaCoAG, a metagenomic binning tool that uses assembly graphs with the composition and coverage information of contigs. MetaCoAG estimates the number of initial bins using single-copy marker genes, assigns contigs into bins iteratively, and adjusts the number of bins dynamically throughout the binning process. We show that MetaCoAG significantly outperforms state-of-the-art binning tools by producing similar or more high-quality bins than the second-best binning tool on both simulated and real datasets. To the best of our knowledge, MetaCoAG is the first stand-alone contig-binning tool that directly makes use of the assembly graph information along with other features of the contigs. }
 }
 ```
+
+## Funding
+
+MetaCoAG is funded by an [Essential Open Source Software for Science Grant](https://chanzuckerberg.com/eoss/proposals/cogent3-python-apis-for-iq-tree-and-graphbin-via-a-plug-in-architecture/) from the Chan Zuckerberg Initiative.
+
+<p align="left">
+  <img src="https://chanzuckerberg.com/wp-content/themes/czi/img/logo.svg" width="300">
+</p>
```

### Comparing `metacoag-1.1.1/metacoag.egg-info/SOURCES.txt` & `metacoag-1.1.2/metacoag.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 metacoag.egg-info/PKG-INFO
 metacoag.egg-info/SOURCES.txt
 metacoag.egg-info/dependency_links.txt
 metacoag.egg-info/entry_points.txt
 metacoag.egg-info/requires.txt
 metacoag.egg-info/top_level.txt
 metacoag.egg-info/zip-safe
+metacoag_utils/.DS_Store
 metacoag_utils/__init__.py
 metacoag_utils/bidirectionalmap.py
 metacoag_utils/feature_utils.py
-metacoag_utils/file_utils.py
 metacoag_utils/graph_utils.py
 metacoag_utils/label_prop_utils.py
 metacoag_utils/marker_gene_utils.py
 metacoag_utils/matching_utils.py
 metacoag_utils/auxiliary/marker.hmm
+metacoag_utils/support/.DS_Store
 metacoag_utils/support/combine_cov.py
```

### Comparing `metacoag-1.1.1/metacoag_utils/auxiliary/marker.hmm` & `metacoag-1.1.2/metacoag_utils/auxiliary/marker.hmm`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.1/metacoag_utils/bidirectionalmap.py` & `metacoag-1.1.2/metacoag_utils/bidirectionalmap.py`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.1/metacoag_utils/feature_utils.py` & `metacoag-1.1.2/metacoag_utils/feature_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 from multiprocessing import Pool
 
 import numpy as np
 from Bio import SeqIO
 
 # Create logger
-logger = logging.getLogger("MetaCoaAG 1.1.1")
+logger = logging.getLogger("MetaCoaAG 1.1.2")
 
 # Set complements of each nucleotide
 complements = {"A": "T", "C": "G", "G": "C", "T": "A"}
 
 # Set bits for each nucleotide
 nt_bits = {"A": 0, "C": 1, "G": 2, "T": 3}
 
@@ -74,18 +74,18 @@
 ):
     tetramer_profiles = {}
     normalized_tetramer_profiles = {}
 
     contigs_file = contigs_file.split("/")[-1]
 
     if os.path.isfile(
-        output_path + contigs_file + ".normalized_contig_tetramers.pickle"
+        f"{output_path}{contigs_file}.normalized_contig_tetramers.pickle"
     ):
         with open(
-            output_path + contigs_file + ".normalized_contig_tetramers.pickle", "rb"
+            f"{output_path}{contigs_file}.normalized_contig_tetramers.pickle", "rb"
         ) as handle:
             normalized_tetramer_profiles = pickle.load(handle)
 
     else:
         kmer_inds_4, kmer_count_len_4 = compute_kmer_inds(4)
 
         pool = Pool(nthreads)
@@ -99,15 +99,15 @@
         i = 0
 
         for l in range(len(normalized)):
             normalized_tetramer_profiles[i] = normalized[l]
             i += 1
 
         with open(
-            output_path + contigs_file + ".normalized_contig_tetramers.pickle", "wb"
+            f"{output_path}{contigs_file}.normalized_contig_tetramers.pickle", "wb"
         ) as handle:
             pickle.dump(
                 normalized_tetramer_profiles, handle, protocol=pickle.HIGHEST_PROTOCOL
             )
 
     tetramer_profiles = {}
 
@@ -153,21 +153,20 @@
 
                     if contig_num not in coverages:
                         coverages[contig_num] = [contig_coverage]
                     else:
                         coverages[contig_num].append(contig_coverage)
 
     if len(coverages) == 0:
-        logger.error(
-            "Could not find any contigs longer than " + str(min_length) + "bp."
-        )
+        logger.error(f"Could not find any contigs longer than {min_length}bp.")
         logger.info("Exiting MetaCoAG... Bye...!")
         sys.exit(1)
 
-    n_samples = len(coverages[0])
+    sample_vals = list(coverages.keys())
+    n_samples = len(coverages[sample_vals[0]])
 
     return sequences, coverages, contig_lengths, n_samples
 
 
 def get_cov_len_megahit(
     contigs_file, contig_names_rev, graph_to_contig_map_rev, min_length, abundance_file
 ):
@@ -201,17 +200,15 @@
 
                     if contig_num not in coverages:
                         coverages[contig_num] = [contig_coverage]
                     else:
                         coverages[contig_num].append(contig_coverage)
 
     if len(coverages) == 0:
-        logger.error(
-            "Could not find any contigs longer than " + str(min_length) + "bp."
-        )
+        logger.error(f"Could not find any contigs longer than {min_length}bp.")
         logger.info("Exiting MetaCoAG... Bye...!")
         sys.exit(1)
 
     n_samples = len(coverages[list(coverages.keys())[0]])
 
     return sequences, coverages, contig_lengths, n_samples
```

### Comparing `metacoag-1.1.1/metacoag_utils/label_prop_utils.py` & `metacoag-1.1.2/metacoag_utils/label_prop_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 
 from metacoag_utils import matching_utils
 
 MAX_WEIGHT = sys.float_info.max
 
 # create logger
-logger = logging.getLogger("MetaCoaAG 1.1.1")
+logger = logging.getLogger("MetaCoaAG 1.1.2")
 
 
 class DataWrap:
     def __init__(self, data):
         self.data = data
 
     def __lt__(self, other):
```

### Comparing `metacoag-1.1.1/metacoag_utils/marker_gene_utils.py` & `metacoag-1.1.2/metacoag_utils/marker_gene_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 #!/usr/bin/env python3
 
 import logging
 import os
 import pathlib
 
 # create logger
-logger = logging.getLogger("MetaCoaAG 1.1.1")
+logger = logging.getLogger("MetaCoaAG 1.1.2")
 
 
 # Modified from SolidBin
 def scan_for_marker_genes(contigs_file, nthreads, markerURL, hard=0):
-    software_path = pathlib.Path(__file__).parent.absolute()
-
-    if markerURL == "":
-        markerURL = os.path.join(software_path, "auxiliary", "marker.hmm")
 
     fragScanURL = "run_FragGeneScan.pl"
     hmmExeURL = "hmmsearch"
 
-    logger.info("Marker file: " + markerURL)
+    logger.info("Using marker file: " + markerURL)
 
-    fragResultURL = contigs_file + ".frag.faa"
-    hmmResultURL = contigs_file + ".hmmout"
+    fragResultURL = f"{contigs_file}.frag.faa"
+    hmmResultURL = f"{contigs_file}.hmmout"
     if not (os.path.exists(fragResultURL)):
         fragCmd = (
             fragScanURL
             + " -genome="
             + contigs_file
             + " -out="
             + contigs_file
@@ -33,15 +29,15 @@
             + str(nthreads)
             + " 1>"
             + contigs_file
             + ".frag.out 2>"
             + contigs_file
             + ".frag.err"
         )
-        logger.debug("exec cmd: " + fragCmd)
+        logger.debug(f"exec cmd: {fragCmd}")
         os.system(fragCmd)
 
     if os.path.exists(fragResultURL):
         if not (os.path.exists(hmmResultURL)):
             hmmCmd = (
                 hmmExeURL
                 + " --domtblout "
@@ -54,32 +50,30 @@
                 + fragResultURL
                 + " 1>"
                 + hmmResultURL
                 + ".out 2>"
                 + hmmResultURL
                 + ".err"
             )
-            logger.debug("exec cmd: " + hmmCmd)
+            logger.debug(f"exec cmd: {hmmCmd}")
             os.system(hmmCmd)
 
         else:
-            logger.debug(
-                "HMMER search failed! Path: " + hmmResultURL + " does not exist."
-            )
+            logger.debug(f"HMMER search failed! Path: {hmmResultURL} does not exist.")
     else:
-        logger.debug("FragGeneScan failed! Path: " + fragResultURL + " does not exist.")
+        logger.debug(f"FragGeneScan failed! Path: {fragResultURL} does not exist.")
 
 
 # Get contigs containing marker genes
 def get_all_contigs_with_marker_genes(
     contigs_file, contig_names_rev, mg_length_threshold
 ):
     contig_markers = {}
 
-    with open(contigs_file + ".hmmout", "r") as myfile:
+    with open(f"{contigs_file}.hmmout", "r") as myfile:
         for line in myfile.readlines():
             if not line.startswith("#"):
                 strings = line.strip().split()
 
                 contig = strings[0]
 
                 # Marker gene name
@@ -114,15 +108,15 @@
 def get_contigs_with_marker_genes(
     contigs_file, contig_names_rev, mg_length_threshold, contig_lengths, min_length
 ):
     marker_contigs = {}
     marker_contig_counts = {}
     contig_markers = {}
 
-    with open(contigs_file + ".hmmout", "r") as myfile:
+    with open(f"{contigs_file}.hmmout", "r") as myfile:
         for line in myfile.readlines():
             if not line.startswith("#"):
                 strings = line.strip().split()
 
                 contig = strings[0]
 
                 # Marker gene name
@@ -184,15 +178,15 @@
     contig_lengths,
     min_length,
 ):
     marker_contigs = {}
     marker_contig_counts = {}
     contig_markers = {}
 
-    with open(contigs_file + ".hmmout", "r") as myfile:
+    with open(f"{contigs_file}.hmmout", "r") as myfile:
         for line in myfile.readlines():
             if not line.startswith("#"):
                 strings = line.strip().split()
 
                 contig = strings[0]
 
                 # Marker gene name
```

### Comparing `metacoag-1.1.1/metacoag_utils/matching_utils.py` & `metacoag-1.1.2/metacoag_utils/matching_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Constants set from MaxBin 2.0
 MU_INTRA, SIGMA_INTRA = 0, 0.01037897 / 2
 MU_INTER, SIGMA_INTER = 0.0676654, 0.03419337
 VERY_SMALL_DOUBLE = 1e-10
 MAX_WEIGHT = sys.float_info.max
 
 # create logger
-logger = logging.getLogger("MetaCoaAG 1.1.1")
+logger = logging.getLogger("MetaCoaAG 1.1.2")
 
 
 def normpdf(x, mean, sd):
     var = float(sd) ** 2
     denom = sd * (2 * math.pi) ** 0.5
     num = math.exp(-((float(x) - float(mean)) ** 2) / (2 * var))
     return num / denom
@@ -85,29 +85,25 @@
 ):
     edge_weights_per_iteration = {}
 
     smg_iterations = len(smg_iteration)
 
     for i in range(smg_iterations):
         logger.debug(
-            "Iteration "
-            + str(i)
-            + ": "
-            + str(len(smg_iteration[i]))
-            + " contig(s) with seed marker genes"
+            f"Iteration {i}: {len(smg_iteration[i])} contig(s) with seed marker genes"
         )
 
         if i > 0:
             B = nx.Graph()
 
             common = set(binned_contigs_with_markers).intersection(
                 set(smg_iteration[i])
             )
             to_bin = list(set(smg_iteration[i]) - common)
-            logger.debug(str(len(to_bin)) + " contig(s) to bin in the iteration")
+            logger.debug(f"{len(to_bin)} contig(s) to bin in the iteration")
             n_bins = len(bins)
             bottom_nodes = []
 
             for n in range(n_bins):
                 contigid = bins[n][0]
                 if contigid not in bottom_nodes:
                     bottom_nodes.append(contigid)
@@ -319,15 +315,15 @@
                             bin_of_contig[longest_nb_contig] = n_bins
                             binned_count += 1
 
                             bin_markers[n_bins] = contig_markers[longest_nb_contig]
                             n_bins += 1
                             binned_contigs_with_markers.append(longest_nb_contig)
 
-            logger.debug(str(binned_count) + " contig(s) binned in the iteration")
+            logger.debug(f"{binned_count} contig(s) binned in the iteration")
 
     if len(smg_iteration) > 0:
         del edge_weights_per_iteration
         del B
         del my_matching
         del not_binned
         del edge_weights
```

### Comparing `metacoag-1.1.1/setup.py` & `metacoag-1.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python3
 
 import setuptools
 
-
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 packages = setuptools.find_packages()
 package_data = {"metacoag_utils": ["metacoag_utils/*", "metacoag_utils/auxiliary/*"]}
 
 data_files = [(".", ["LICENSE", "README.md"])]
 
 setuptools.setup(
     name="metacoag",
-    version="1.1.1",
+    version="1.1.2",
     zip_safe=True,
     author="Vijini Mallawaarachchi and Yu Lin",
     author_email="viji.mallawaarachchi@gmail.com",
     description="MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/metagentools/MetaCoAG",
@@ -43,12 +42,13 @@
     install_requires=[
         "biopython",
         "python-igraph",
         "networkx",
         "scipy",
         "numpy",
         "tqdm",
-	"pandas",
+        "pandas",
         "hmmer",
+        "click"
     ],
     python_requires=">=3.7",
 )
```

