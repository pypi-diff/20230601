# Comparing `tmp/btyper3-3.3.4.tar.gz` & `tmp/btyper3-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btyper3-3.3.4.tar", last modified: Tue Dec 13 14:57:43 2022, max compression
+gzip compressed data, was "btyper3-3.4.0.tar", last modified: Thu Jun  1 14:33:22 2023, max compression
```

## Comparing `btyper3-3.3.4.tar` & `btyper3-3.4.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:43.015141 btyper3-3.3.4/
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2022-12-13 14:57:20.000000 btyper3-3.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2022-12-13 14:57:20.000000 btyper3-3.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2022-12-13 14:57:43.015141 btyper3-3.3.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     9922 2022-12-13 14:57:20.000000 btyper3-3.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:43.011141 btyper3-3.3.4/btyper3/
--rwxr-xr-x   0 runner    (1001) docker     (123)    18268 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4554 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/ani.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10033 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/blast.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1961 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/mlst.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6617 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/print_final_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:43.011141 btyper3-3.3.4/btyper3/seq_ani_db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_ani_db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:43.011141 btyper3-3.3.4/btyper3/seq_ani_db/geneflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_ani_db/geneflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_ani_db/geneflow/geneflow.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:43.011141 btyper3-3.3.4/btyper3/seq_ani_db/species/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_ani_db/species/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_ani_db/species/species.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:43.011141 btyper3-3.3.4/btyper3/seq_ani_db/subspecies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_ani_db/subspecies/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      401 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_ani_db/subspecies/subspecies.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:43.011141 btyper3-3.3.4/btyper3/seq_ani_db/typestrains/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_ani_db/typestrains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_ani_db/typestrains/typestrains.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:43.011141 btyper3-3.3.4/btyper3/seq_bt_db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_bt_db/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   976196 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_bt_db/btyper3_bt_sequences.faa
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:43.015141 btyper3-3.3.4/btyper3/seq_mlst_db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_mlst_db/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   156106 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_mlst_db/pubmlst.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:43.015141 btyper3-3.3.4/btyper3/seq_panC_db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_panC_db/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    64169 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_panC_db/panC.fna
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:43.015141 btyper3-3.3.4/btyper3/seq_virulence_db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_virulence_db/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21236 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_virulence_db/btyper3_virulence_sequences.faa
--rwxr-xr-x   0 runner    (1001) docker     (123)    61410 2022-12-13 14:57:20.000000 btyper3-3.3.4/btyper3/seq_virulence_db/btyper3_virulence_sequences.ffn
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:57:43.011141 btyper3-3.3.4/btyper3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2022-12-13 14:57:42.000000 btyper3-3.3.4/btyper3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2022-12-13 14:57:43.000000 btyper3-3.3.4/btyper3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 14:57:42.000000 btyper3-3.3.4/btyper3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-13 14:57:42.000000 btyper3-3.3.4/btyper3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 14:57:42.000000 btyper3-3.3.4/btyper3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-13 14:57:42.000000 btyper3-3.3.4/btyper3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-13 14:57:43.000000 btyper3-3.3.4/btyper3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2022-12-13 14:57:43.015141 btyper3-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2022-12-13 14:57:20.000000 btyper3-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:22.314838 btyper3-3.4.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-06-01 14:33:15.000000 btyper3-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-01 14:33:15.000000 btyper3-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-06-01 14:33:22.314838 btyper3-3.4.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10180 2023-06-01 14:33:15.000000 btyper3-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:22.306837 btyper3-3.4.0/btyper3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18266 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4554 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/ani.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10033 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/blast.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1961 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/mlst.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6617 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/print_final_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:22.310837 btyper3-3.4.0/btyper3/seq_ani_db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_ani_db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:22.310837 btyper3-3.4.0/btyper3/seq_ani_db/geneflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_ani_db/geneflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_ani_db/geneflow/geneflow.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:22.310837 btyper3-3.4.0/btyper3/seq_ani_db/species/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_ani_db/species/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_ani_db/species/species.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:22.310837 btyper3-3.4.0/btyper3/seq_ani_db/subspecies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_ani_db/subspecies/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      401 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_ani_db/subspecies/subspecies.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:22.310837 btyper3-3.4.0/btyper3/seq_ani_db/typestrains/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_ani_db/typestrains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_ani_db/typestrains/typestrains.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:22.310837 btyper3-3.4.0/btyper3/seq_bt_db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_bt_db/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   976196 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_bt_db/btyper3_bt_sequences.faa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:22.310837 btyper3-3.4.0/btyper3/seq_mlst_db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_mlst_db/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   156106 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_mlst_db/pubmlst.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:22.310837 btyper3-3.4.0/btyper3/seq_panC_db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_panC_db/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    64169 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_panC_db/panC.fna
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:22.314838 btyper3-3.4.0/btyper3/seq_virulence_db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_virulence_db/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21236 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_virulence_db/btyper3_virulence_sequences.faa
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61410 2023-06-01 14:33:15.000000 btyper3-3.4.0/btyper3/seq_virulence_db/btyper3_virulence_sequences.ffn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:33:22.310837 btyper3-3.4.0/btyper3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-06-01 14:33:22.000000 btyper3-3.4.0/btyper3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-01 14:33:22.000000 btyper3-3.4.0/btyper3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:33:22.000000 btyper3-3.4.0/btyper3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 14:33:22.000000 btyper3-3.4.0/btyper3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:33:22.000000 btyper3-3.4.0/btyper3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-01 14:33:22.000000 btyper3-3.4.0/btyper3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 14:33:22.000000 btyper3-3.4.0/btyper3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-01 14:33:22.314838 btyper3-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-01 14:33:15.000000 btyper3-3.4.0/setup.py
```

### Comparing `btyper3-3.3.4/LICENSE` & `btyper3-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `btyper3-3.3.4/PKG-INFO` & `btyper3-3.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btyper3
-Version: 3.3.4
+Version: 3.4.0
 Summary: In silico taxonomic classification of Bacillus cereus group isolates using assembled genomes
 Home-page: https://github.com/lmc297/btyper3
 Author: Laura M. Carroll
 Author-email: lmc297@cornell.edu
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/lmc297/btyper3/issues
 Project-URL: Publication, https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7536271/
@@ -84,30 +84,32 @@
 3. Install via `pip` (this will download required Python dependencies as well):
    ```console
    pip install btyper3  
    ```
 
 ------------------------------------------------------------------------
 
-## News: updates in BTyper3 v3.2.0 and v3.3.0 -- new species just dropped!
+## News: updates in BTyper3 v3.2.0, v3.3.0, and v3.4.0 -- new species just dropped!
 
 The primary function of BTyper3 is to allow users to taxonomically classify *B. cereus* group genomes using a standardized nomenclature (see <a href="https://journals.asm.org/doi/10.1128/mBio.00034-20">here</a> and <a href="https://www.frontiersin.org/articles/10.3389/fmicb.2020.580691/full">here</a> for details regarding how the standardized nomenclature was constructed, and how it compares to historical typing methods, respectively). However, we understand that some users may also want to compare their *B. cereus* group genomes to the type strain genomes of published *B. cereus* group species. Thus, in BTyper3 v3.2.0, we have added the `--ani_typestrains` option, which calculates ANI values between a query genome and the genomes of all published *B. cereus* group species type strains and reports the type strain that produces the highest ANI value.
 
-The type strain genomes used by BTyper3's `--ani_typestrains` option correspond to the species discussed in <a href="https://www.tandfonline.com/doi/full/10.1080/10408398.2021.1916735">Figure 2 of our taxonomy review</a>, plus five species published after the review was published</a> (i.e., *Bacillus sanguinis*, *Bacillus paramobilis*, and *Bacillus hominis*, added in v3.2.0, and "*B. arachidis*" and *B. rhizoplanae*, added in v3.3.0). Within the standardized taxonomy that BTyper3 uses for genomospecies assignment:
+The type strain genomes used by BTyper3's `--ani_typestrains` option correspond to the species discussed in <a href="https://www.tandfonline.com/doi/full/10.1080/10408398.2021.1916735">Figure 2 of our taxonomy review</a>, plus species published after the review was published</a> (i.e., *Bacillus sanguinis*, *Bacillus paramobilis*, and *Bacillus hominis*, added in v3.2.0; "*B. arachidis*" and *B. rhizoplanae*, added in v3.3.0; "*B. pretiosus*", added in v3.4.0). Within the standardized taxonomy that BTyper3 uses for genomospecies assignment:
 
 * All members of *Bacillus sanguinis* (type strain RefSeq Assembly Accession GCF_018332475.1) belong to *B. mosaicus* (i.e., *B. sanguinis* is not considered a novel species in the standardized taxonomy)
 
 * All members of *Bacillus paramobilis* (type strain RefSeq Assembly Accession GCF_018332495.1) belong to *B. mosaicus* (i.e., *B. paramobilis* is not considered a novel species in the standardized taxonomy)
 
 * All members of *Bacillus hominis* (type strain RefSeq Assembly Accession GCF_018332515.1) belong to *B. mycoides* (i.e., *B. hominis* is not considered a novel species in the standardized taxonomy)
 
 * "*Bacillus arachidis*" (type strain RefSeq Assembly Accession GCF_017498775.1) replaces the putative genomospecies previously referred to as "Unknown Species 17" in the standardized taxonomy
 
 * *Bacillus rhizoplanae* (type strain RefSeq Assembly Accession GCF_917563915.1) represents a novel genomospecies within the standardized taxonomy and has been added to the database
 
+* All members of "*Bacillus pretiosus*" (type strain RefSeq Assembly Accession GCF_025916425.1) belong to *B. mosaicus* (i.e., "*B. pretiosus*" is not considered a novel species in the standardized taxonomy)
+
 **Importantly, *B. cereus* group species are often proposed in the literature using unstandardized approaches** (e.g., varying genomospecies thresholds, which may produce overlapping genomospecies). We have added the type strain comparison method in BTyper3 v3.2.0, as users may still want to compare a query genome with the type strains of published *B. cereus* group species. However, interpret results with caution, as some *B. cereus* group genomes may belong to multiple species using type strain genomes.
 
 For more information, check out our:
 
 * <a href="https://www.tandfonline.com/doi/full/10.1080/10408398.2021.1916735">Review of *B. cereus* group taxonomy/nomenclature</a>
 
 * <a href="https://journals.asm.org/doi/full/10.1128/mBio.00034-20">Standardized nomenclature for the *B. cereus* group</a>
@@ -151,36 +153,36 @@
 
 #### Perform all default analyses, using an assembled genome (complete or draft) in (multi-)FASTA format as input (fastANI is not in the user's path):
 
 ```
 btyper3 -i /path/to/genome.fasta -o /path/to/desired/output_directory --fastani_path /path/to/FastANI_executable/fastANI
 ```
 
-#### Perform all default analyses, plus pseudo-gene flow unit assignment AND species type strain comparison, using an assembled genome (complete or draft) in (multi-)FASTA format as input (assumes fastANI is in the user's path):
+#### Perform all default analyses, plus pseudo-gene flow unit assignment, using an assembled genome (complete or draft) in (multi-)FASTA format as input (assumes fastANI is in the user's path):
 
 ```
-btyper3 -i /path/to/genome.fasta -o /path/to/desired/output_directory --ani_geneflow True --ani_typestrains True
+btyper3 -i /path/to/genome.fasta -o /path/to/desired/output_directory --ani_geneflow True
 ```
 
 #### Perform seven-gene MLST only, using user-supplied MLST gene sequences and the latest version of the PubMLST *B. cereus s.l.* database (sequences can be in multi-FASTA format, or concatenated into a single sequence in FASTA format):
 
 ```
-btyper3 -i /path/to/mlst.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --virulence False --bt False --panC False --download_mlst_latest True
+btyper3 -i /path/to/mlst.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --ani_typestrains False --virulence False --bt False --panC False --download_mlst_latest True
 ```
 
 #### Perform *panC* group assignment only, using a user-supplied *panC* gene sequence in FASTA format:
 
 ```
-btyper3 -i /path/to/panC.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --virulence False --bt False --mlst False
+btyper3 -i /path/to/panC.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --ani_typestrains False --virulence False --bt False --mlst False
 ```
 
 #### Perform virulence factor and Bt toxin-encoding gene detection in a plasmid sequence in FASTA format:
 
 ```
-btyper3 -i /path/to/plasmid.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --mlst False --panC False
+btyper3 -i /path/to/plasmid.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --ani_typestrains False --mlst False --panC False
 ```
 
 
 ------------------------------------------------------------------------
 
 
 Disclaimer: BTyper3 is pretty neat! However, no tool is perfect, and BTyper3 cannot definitively prove whether an isolate is pathogenic or not. As always, interpret your results with caution. We are not responsible for taxonomic misclassifications, misclassifications of an isolate's pathogenic potential or industrial utility, and/or misinterpretations (biological, statistical, or otherwise) of BTyper3 results.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: btyper3 Version: 3.3.4 Summary: In silico taxonomic
+Metadata-Version: 2.1 Name: btyper3 Version: 3.4.0 Summary: In silico taxonomic
 classification of Bacillus cereus group isolates using assembled genomes Home-
 page: https://github.com/lmc297/btyper3 Author: Laura M. Carroll Author-email:
 lmc297@cornell.edu License: GPLv3 Project-URL: Bug Tracker, https://github.com/
 lmc297/btyper3/issues Project-URL: Publication, https://www.ncbi.nlm.nih.gov/
 pmc/articles/PMC7536271/ Project-URL: Changelog, https://github.com/lmc297/
 btyper3/blob/master/archive/CHANGELOG.md Keywords: bacillus,taxonomy,genome,ANI
 Platform: any Classifier: Development Status :: 6 - Mature Classifier: Intended
@@ -38,60 +38,63 @@
 Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=Download) v2.9.0+ and up  2.
 [Add BLAST+ to your path](https://unix.stackexchange.com/questions/26047/how-
 to-correctly-add-a-path-to-path), if necessary (to check if BLAST+ is in your
 path, try running `makeblastdb -h` and `tblastn -h` from your command line; you
 should get a help message for each command, with no error messages) 3. Install
 via `pip` (this will download required Python dependencies as well): ```console
 pip install btyper3 ``` -------------------------------------------------------
------------------ ## News: updates in BTyper3 v3.2.0 and v3.3.0 -- new species
-just dropped! The primary function of BTyper3 is to allow users to
+----------------- ## News: updates in BTyper3 v3.2.0, v3.3.0, and v3.4.0 -- new
+species just dropped! The primary function of BTyper3 is to allow users to
 taxonomically classify *B. cereus* group genomes using a standardized
 nomenclature (see here and here for details regarding how the standardized
 nomenclature was constructed, and how it compares to historical typing methods,
 respectively). However, we understand that some users may also want to compare
 their *B. cereus* group genomes to the type strain genomes of published *B.
 cereus* group species. Thus, in BTyper3 v3.2.0, we have added the `--
 ani_typestrains` option, which calculates ANI values between a query genome and
 the genomes of all published *B. cereus* group species type strains and reports
 the type strain that produces the highest ANI value. The type strain genomes
 used by BTyper3's `--ani_typestrains` option correspond to the species
-discussed in Figure_2_of_our_taxonomy_review, plus five species published after
-the review was published
+discussed in Figure_2_of_our_taxonomy_review, plus species published after the
+review was published
  (i.e., *Bacillus sanguinis*, *Bacillus paramobilis*, and *Bacillus hominis*,
-added in v3.2.0, and "*B. arachidis*" and *B. rhizoplanae*, added in v3.3.0).
-Within the standardized taxonomy that BTyper3 uses for genomospecies
-assignment: * All members of *Bacillus sanguinis* (type strain RefSeq Assembly
-Accession GCF_018332475.1) belong to *B. mosaicus* (i.e., *B. sanguinis* is not
-considered a novel species in the standardized taxonomy) * All members of
-*Bacillus paramobilis* (type strain RefSeq Assembly Accession GCF_018332495.1)
-belong to *B. mosaicus* (i.e., *B. paramobilis* is not considered a novel
-species in the standardized taxonomy) * All members of *Bacillus hominis* (type
-strain RefSeq Assembly Accession GCF_018332515.1) belong to *B. mycoides*
-(i.e., *B. hominis* is not considered a novel species in the standardized
-taxonomy) * "*Bacillus arachidis*" (type strain RefSeq Assembly Accession
-GCF_017498775.1) replaces the putative genomospecies previously referred to as
-"Unknown Species 17" in the standardized taxonomy * *Bacillus rhizoplanae*
-(type strain RefSeq Assembly Accession GCF_917563915.1) represents a novel
-genomospecies within the standardized taxonomy and has been added to the
-database **Importantly, *B. cereus* group species are often proposed in the
-literature using unstandardized approaches** (e.g., varying genomospecies
-thresholds, which may produce overlapping genomospecies). We have added the
-type strain comparison method in BTyper3 v3.2.0, as users may still want to
-compare a query genome with the type strains of published *B. cereus* group
-species. However, interpret results with caution, as some *B. cereus* group
-genomes may belong to multiple species using type strain genomes. For more
-information, check out our: * Review_of_*B._cereus*_group_taxonomy/nomenclature
-* Standardized_nomenclature_for_the_*B._cereus*_group * Comparison_of_our
-standardized_nomenclature_to_other_*B._cereus*_group_typing_methods_(e.g.,
-MLST,_*panC*,_ANI-based_comparisons_to_species_type_strain_genomes) -----------
-------------------------------------------------------------- ## Citation ###
-If you found the BTyper3 tool, its source code, and/or any of its associated
-databases useful, please cite: Carroll, Laura M., Martin Wiedmann, Jasna Kovac.
-2020. "Proposal_of_a_Taxonomic_Nomenclature_for_the_*Bacillus_cereus*_Group
-Which_Reconciles_Genomic_Definitions_of_Bacterial_Species_with_Clinical_and
+added in v3.2.0; "*B. arachidis*" and *B. rhizoplanae*, added in v3.3.0; "*B.
+pretiosus*", added in v3.4.0). Within the standardized taxonomy that BTyper3
+uses for genomospecies assignment: * All members of *Bacillus sanguinis* (type
+strain RefSeq Assembly Accession GCF_018332475.1) belong to *B. mosaicus*
+(i.e., *B. sanguinis* is not considered a novel species in the standardized
+taxonomy) * All members of *Bacillus paramobilis* (type strain RefSeq Assembly
+Accession GCF_018332495.1) belong to *B. mosaicus* (i.e., *B. paramobilis* is
+not considered a novel species in the standardized taxonomy) * All members of
+*Bacillus hominis* (type strain RefSeq Assembly Accession GCF_018332515.1)
+belong to *B. mycoides* (i.e., *B. hominis* is not considered a novel species
+in the standardized taxonomy) * "*Bacillus arachidis*" (type strain RefSeq
+Assembly Accession GCF_017498775.1) replaces the putative genomospecies
+previously referred to as "Unknown Species 17" in the standardized taxonomy *
+*Bacillus rhizoplanae* (type strain RefSeq Assembly Accession GCF_917563915.1)
+represents a novel genomospecies within the standardized taxonomy and has been
+added to the database * All members of "*Bacillus pretiosus*" (type strain
+RefSeq Assembly Accession GCF_025916425.1) belong to *B. mosaicus* (i.e., "*B.
+pretiosus*" is not considered a novel species in the standardized taxonomy)
+**Importantly, *B. cereus* group species are often proposed in the literature
+using unstandardized approaches** (e.g., varying genomospecies thresholds,
+which may produce overlapping genomospecies). We have added the type strain
+comparison method in BTyper3 v3.2.0, as users may still want to compare a query
+genome with the type strains of published *B. cereus* group species. However,
+interpret results with caution, as some *B. cereus* group genomes may belong to
+multiple species using type strain genomes. For more information, check out
+our: * Review_of_*B._cereus*_group_taxonomy/nomenclature * Standardized
+nomenclature_for_the_*B._cereus*_group * Comparison_of_our_standardized
+nomenclature_to_other_*B._cereus*_group_typing_methods_(e.g.,_MLST,_*panC*,
+ANI-based_comparisons_to_species_type_strain_genomes) -------------------------
+----------------------------------------------- ## Citation ### If you found
+the BTyper3 tool, its source code, and/or any of its associated databases
+useful, please cite: Carroll, Laura M., Martin Wiedmann, Jasna Kovac. 2020.
+"Proposal_of_a_Taxonomic_Nomenclature_for_the_*Bacillus_cereus*_Group_Which
+Reconciles_Genomic_Definitions_of_Bacterial_Species_with_Clinical_and
 Industrial_Phenotypes." *mBio* 11(1): e00034-20; DOI: 10.1128/mBio.00034-20.
 Carroll, Laura M., Rachel A. Cheng, Jasna Kovac. 2020. "No_Assembly_Required:
 Using_BTyper3_to_Assess_the_Congruency_of_a_Proposed_Taxonomic_Framework_for
 the_*Bacillus_cereus*_group_with_Historical_Typing_Methods." *Frontiers in
 Microbiology* 11: 580691; DOI: 10.3389/fmicb.2020.580691. ---------------------
 --------------------------------------------------- ## Quick Start For detailed
 information, check out the BTyper3_wiki ### Command Structure ``` btyper3 -i
@@ -100,31 +103,31 @@
 Commands #### Perform all default analyses, using an assembled genome (complete
 or draft) in (multi-)FASTA format as input (assumes fastANI is in the user's
 path): ``` btyper3 -i /path/to/genome.fasta -o /path/to/desired/
 output_directory ``` #### Perform all default analyses, using an assembled
 genome (complete or draft) in (multi-)FASTA format as input (fastANI is not in
 the user's path): ``` btyper3 -i /path/to/genome.fasta -o /path/to/desired/
 output_directory --fastani_path /path/to/FastANI_executable/fastANI ``` ####
-Perform all default analyses, plus pseudo-gene flow unit assignment AND species
-type strain comparison, using an assembled genome (complete or draft) in
-(multi-)FASTA format as input (assumes fastANI is in the user's path): ```
-btyper3 -i /path/to/genome.fasta -o /path/to/desired/output_directory --
-ani_geneflow True --ani_typestrains True ``` #### Perform seven-gene MLST only,
-using user-supplied MLST gene sequences and the latest version of the PubMLST
-*B. cereus s.l.* database (sequences can be in multi-FASTA format, or
-concatenated into a single sequence in FASTA format): ``` btyper3 -i /path/to/
-mlst.fasta -o /path/to/desired/output_directory --ani_species False --
-ani_subspecies False --virulence False --bt False --panC False --
-download_mlst_latest True ``` #### Perform *panC* group assignment only, using
-a user-supplied *panC* gene sequence in FASTA format: ``` btyper3 -i /path/to/
-panC.fasta -o /path/to/desired/output_directory --ani_species False --
-ani_subspecies False --virulence False --bt False --mlst False ``` #### Perform
-virulence factor and Bt toxin-encoding gene detection in a plasmid sequence in
-FASTA format: ``` btyper3 -i /path/to/plasmid.fasta -o /path/to/desired/
-output_directory --ani_species False --ani_subspecies False --mlst False --panC
-False ``` ---------------------------------------------------------------------
---- Disclaimer: BTyper3 is pretty neat! However, no tool is perfect, and
-BTyper3 cannot definitively prove whether an isolate is pathogenic or not. As
-always, interpret your results with caution. We are not responsible for
-taxonomic misclassifications, misclassifications of an isolate's pathogenic
-potential or industrial utility, and/or misinterpretations (biological,
-statistical, or otherwise) of BTyper3 results.
+Perform all default analyses, plus pseudo-gene flow unit assignment, using an
+assembled genome (complete or draft) in (multi-)FASTA format as input (assumes
+fastANI is in the user's path): ``` btyper3 -i /path/to/genome.fasta -o /path/
+to/desired/output_directory --ani_geneflow True ``` #### Perform seven-gene
+MLST only, using user-supplied MLST gene sequences and the latest version of
+the PubMLST *B. cereus s.l.* database (sequences can be in multi-FASTA format,
+or concatenated into a single sequence in FASTA format): ``` btyper3 -i /path/
+to/mlst.fasta -o /path/to/desired/output_directory --ani_species False --
+ani_subspecies False --ani_typestrains False --virulence False --bt False --
+panC False --download_mlst_latest True ``` #### Perform *panC* group assignment
+only, using a user-supplied *panC* gene sequence in FASTA format: ``` btyper3 -
+i /path/to/panC.fasta -o /path/to/desired/output_directory --ani_species False
+--ani_subspecies False --ani_typestrains False --virulence False --bt False --
+mlst False ``` #### Perform virulence factor and Bt toxin-encoding gene
+detection in a plasmid sequence in FASTA format: ``` btyper3 -i /path/to/
+plasmid.fasta -o /path/to/desired/output_directory --ani_species False --
+ani_subspecies False --ani_typestrains False --mlst False --panC False ``` ----
+-------------------------------------------------------------------
+- Disclaimer: BTyper3 is pretty neat! However, no tool is perfect, and BTyper3
+cannot definitively prove whether an isolate is pathogenic or not. As always,
+interpret your results with caution. We are not responsible for taxonomic
+misclassifications, misclassifications of an isolate's pathogenic potential or
+industrial utility, and/or misinterpretations (biological, statistical, or
+otherwise) of BTyper3 results.
```

### Comparing `btyper3-3.3.4/README.md` & `btyper3-3.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,30 +60,32 @@
 3. Install via `pip` (this will download required Python dependencies as well):
    ```console
    pip install btyper3  
    ```
 
 ------------------------------------------------------------------------
 
-## News: updates in BTyper3 v3.2.0 and v3.3.0 -- new species just dropped!
+## News: updates in BTyper3 v3.2.0, v3.3.0, and v3.4.0 -- new species just dropped!
 
 The primary function of BTyper3 is to allow users to taxonomically classify *B. cereus* group genomes using a standardized nomenclature (see <a href="https://journals.asm.org/doi/10.1128/mBio.00034-20">here</a> and <a href="https://www.frontiersin.org/articles/10.3389/fmicb.2020.580691/full">here</a> for details regarding how the standardized nomenclature was constructed, and how it compares to historical typing methods, respectively). However, we understand that some users may also want to compare their *B. cereus* group genomes to the type strain genomes of published *B. cereus* group species. Thus, in BTyper3 v3.2.0, we have added the `--ani_typestrains` option, which calculates ANI values between a query genome and the genomes of all published *B. cereus* group species type strains and reports the type strain that produces the highest ANI value.
 
-The type strain genomes used by BTyper3's `--ani_typestrains` option correspond to the species discussed in <a href="https://www.tandfonline.com/doi/full/10.1080/10408398.2021.1916735">Figure 2 of our taxonomy review</a>, plus five species published after the review was published</a> (i.e., *Bacillus sanguinis*, *Bacillus paramobilis*, and *Bacillus hominis*, added in v3.2.0, and "*B. arachidis*" and *B. rhizoplanae*, added in v3.3.0). Within the standardized taxonomy that BTyper3 uses for genomospecies assignment:
+The type strain genomes used by BTyper3's `--ani_typestrains` option correspond to the species discussed in <a href="https://www.tandfonline.com/doi/full/10.1080/10408398.2021.1916735">Figure 2 of our taxonomy review</a>, plus species published after the review was published</a> (i.e., *Bacillus sanguinis*, *Bacillus paramobilis*, and *Bacillus hominis*, added in v3.2.0; "*B. arachidis*" and *B. rhizoplanae*, added in v3.3.0; "*B. pretiosus*", added in v3.4.0). Within the standardized taxonomy that BTyper3 uses for genomospecies assignment:
 
 * All members of *Bacillus sanguinis* (type strain RefSeq Assembly Accession GCF_018332475.1) belong to *B. mosaicus* (i.e., *B. sanguinis* is not considered a novel species in the standardized taxonomy)
 
 * All members of *Bacillus paramobilis* (type strain RefSeq Assembly Accession GCF_018332495.1) belong to *B. mosaicus* (i.e., *B. paramobilis* is not considered a novel species in the standardized taxonomy)
 
 * All members of *Bacillus hominis* (type strain RefSeq Assembly Accession GCF_018332515.1) belong to *B. mycoides* (i.e., *B. hominis* is not considered a novel species in the standardized taxonomy)
 
 * "*Bacillus arachidis*" (type strain RefSeq Assembly Accession GCF_017498775.1) replaces the putative genomospecies previously referred to as "Unknown Species 17" in the standardized taxonomy
 
 * *Bacillus rhizoplanae* (type strain RefSeq Assembly Accession GCF_917563915.1) represents a novel genomospecies within the standardized taxonomy and has been added to the database
 
+* All members of "*Bacillus pretiosus*" (type strain RefSeq Assembly Accession GCF_025916425.1) belong to *B. mosaicus* (i.e., "*B. pretiosus*" is not considered a novel species in the standardized taxonomy)
+
 **Importantly, *B. cereus* group species are often proposed in the literature using unstandardized approaches** (e.g., varying genomospecies thresholds, which may produce overlapping genomospecies). We have added the type strain comparison method in BTyper3 v3.2.0, as users may still want to compare a query genome with the type strains of published *B. cereus* group species. However, interpret results with caution, as some *B. cereus* group genomes may belong to multiple species using type strain genomes.
 
 For more information, check out our:
 
 * <a href="https://www.tandfonline.com/doi/full/10.1080/10408398.2021.1916735">Review of *B. cereus* group taxonomy/nomenclature</a>
 
 * <a href="https://journals.asm.org/doi/full/10.1128/mBio.00034-20">Standardized nomenclature for the *B. cereus* group</a>
@@ -127,36 +129,36 @@
 
 #### Perform all default analyses, using an assembled genome (complete or draft) in (multi-)FASTA format as input (fastANI is not in the user's path):
 
 ```
 btyper3 -i /path/to/genome.fasta -o /path/to/desired/output_directory --fastani_path /path/to/FastANI_executable/fastANI
 ```
 
-#### Perform all default analyses, plus pseudo-gene flow unit assignment AND species type strain comparison, using an assembled genome (complete or draft) in (multi-)FASTA format as input (assumes fastANI is in the user's path):
+#### Perform all default analyses, plus pseudo-gene flow unit assignment, using an assembled genome (complete or draft) in (multi-)FASTA format as input (assumes fastANI is in the user's path):
 
 ```
-btyper3 -i /path/to/genome.fasta -o /path/to/desired/output_directory --ani_geneflow True --ani_typestrains True
+btyper3 -i /path/to/genome.fasta -o /path/to/desired/output_directory --ani_geneflow True
 ```
 
 #### Perform seven-gene MLST only, using user-supplied MLST gene sequences and the latest version of the PubMLST *B. cereus s.l.* database (sequences can be in multi-FASTA format, or concatenated into a single sequence in FASTA format):
 
 ```
-btyper3 -i /path/to/mlst.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --virulence False --bt False --panC False --download_mlst_latest True
+btyper3 -i /path/to/mlst.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --ani_typestrains False --virulence False --bt False --panC False --download_mlst_latest True
 ```
 
 #### Perform *panC* group assignment only, using a user-supplied *panC* gene sequence in FASTA format:
 
 ```
-btyper3 -i /path/to/panC.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --virulence False --bt False --mlst False
+btyper3 -i /path/to/panC.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --ani_typestrains False --virulence False --bt False --mlst False
 ```
 
 #### Perform virulence factor and Bt toxin-encoding gene detection in a plasmid sequence in FASTA format:
 
 ```
-btyper3 -i /path/to/plasmid.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --mlst False --panC False
+btyper3 -i /path/to/plasmid.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --ani_typestrains False --mlst False --panC False
 ```
 
 
 ------------------------------------------------------------------------
 
 
 Disclaimer: BTyper3 is pretty neat! However, no tool is perfect, and BTyper3 cannot definitively prove whether an isolate is pathogenic or not. As always, interpret your results with caution. We are not responsible for taxonomic misclassifications, misclassifications of an isolate's pathogenic potential or industrial utility, and/or misinterpretations (biological, statistical, or otherwise) of BTyper3 results.
```

#### html2text {}

```diff
@@ -25,60 +25,63 @@
 Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=Download) v2.9.0+ and up  2.
 [Add BLAST+ to your path](https://unix.stackexchange.com/questions/26047/how-
 to-correctly-add-a-path-to-path), if necessary (to check if BLAST+ is in your
 path, try running `makeblastdb -h` and `tblastn -h` from your command line; you
 should get a help message for each command, with no error messages) 3. Install
 via `pip` (this will download required Python dependencies as well): ```console
 pip install btyper3 ``` -------------------------------------------------------
------------------ ## News: updates in BTyper3 v3.2.0 and v3.3.0 -- new species
-just dropped! The primary function of BTyper3 is to allow users to
+----------------- ## News: updates in BTyper3 v3.2.0, v3.3.0, and v3.4.0 -- new
+species just dropped! The primary function of BTyper3 is to allow users to
 taxonomically classify *B. cereus* group genomes using a standardized
 nomenclature (see here and here for details regarding how the standardized
 nomenclature was constructed, and how it compares to historical typing methods,
 respectively). However, we understand that some users may also want to compare
 their *B. cereus* group genomes to the type strain genomes of published *B.
 cereus* group species. Thus, in BTyper3 v3.2.0, we have added the `--
 ani_typestrains` option, which calculates ANI values between a query genome and
 the genomes of all published *B. cereus* group species type strains and reports
 the type strain that produces the highest ANI value. The type strain genomes
 used by BTyper3's `--ani_typestrains` option correspond to the species
-discussed in Figure_2_of_our_taxonomy_review, plus five species published after
-the review was published
+discussed in Figure_2_of_our_taxonomy_review, plus species published after the
+review was published
  (i.e., *Bacillus sanguinis*, *Bacillus paramobilis*, and *Bacillus hominis*,
-added in v3.2.0, and "*B. arachidis*" and *B. rhizoplanae*, added in v3.3.0).
-Within the standardized taxonomy that BTyper3 uses for genomospecies
-assignment: * All members of *Bacillus sanguinis* (type strain RefSeq Assembly
-Accession GCF_018332475.1) belong to *B. mosaicus* (i.e., *B. sanguinis* is not
-considered a novel species in the standardized taxonomy) * All members of
-*Bacillus paramobilis* (type strain RefSeq Assembly Accession GCF_018332495.1)
-belong to *B. mosaicus* (i.e., *B. paramobilis* is not considered a novel
-species in the standardized taxonomy) * All members of *Bacillus hominis* (type
-strain RefSeq Assembly Accession GCF_018332515.1) belong to *B. mycoides*
-(i.e., *B. hominis* is not considered a novel species in the standardized
-taxonomy) * "*Bacillus arachidis*" (type strain RefSeq Assembly Accession
-GCF_017498775.1) replaces the putative genomospecies previously referred to as
-"Unknown Species 17" in the standardized taxonomy * *Bacillus rhizoplanae*
-(type strain RefSeq Assembly Accession GCF_917563915.1) represents a novel
-genomospecies within the standardized taxonomy and has been added to the
-database **Importantly, *B. cereus* group species are often proposed in the
-literature using unstandardized approaches** (e.g., varying genomospecies
-thresholds, which may produce overlapping genomospecies). We have added the
-type strain comparison method in BTyper3 v3.2.0, as users may still want to
-compare a query genome with the type strains of published *B. cereus* group
-species. However, interpret results with caution, as some *B. cereus* group
-genomes may belong to multiple species using type strain genomes. For more
-information, check out our: * Review_of_*B._cereus*_group_taxonomy/nomenclature
-* Standardized_nomenclature_for_the_*B._cereus*_group * Comparison_of_our
-standardized_nomenclature_to_other_*B._cereus*_group_typing_methods_(e.g.,
-MLST,_*panC*,_ANI-based_comparisons_to_species_type_strain_genomes) -----------
-------------------------------------------------------------- ## Citation ###
-If you found the BTyper3 tool, its source code, and/or any of its associated
-databases useful, please cite: Carroll, Laura M., Martin Wiedmann, Jasna Kovac.
-2020. "Proposal_of_a_Taxonomic_Nomenclature_for_the_*Bacillus_cereus*_Group
-Which_Reconciles_Genomic_Definitions_of_Bacterial_Species_with_Clinical_and
+added in v3.2.0; "*B. arachidis*" and *B. rhizoplanae*, added in v3.3.0; "*B.
+pretiosus*", added in v3.4.0). Within the standardized taxonomy that BTyper3
+uses for genomospecies assignment: * All members of *Bacillus sanguinis* (type
+strain RefSeq Assembly Accession GCF_018332475.1) belong to *B. mosaicus*
+(i.e., *B. sanguinis* is not considered a novel species in the standardized
+taxonomy) * All members of *Bacillus paramobilis* (type strain RefSeq Assembly
+Accession GCF_018332495.1) belong to *B. mosaicus* (i.e., *B. paramobilis* is
+not considered a novel species in the standardized taxonomy) * All members of
+*Bacillus hominis* (type strain RefSeq Assembly Accession GCF_018332515.1)
+belong to *B. mycoides* (i.e., *B. hominis* is not considered a novel species
+in the standardized taxonomy) * "*Bacillus arachidis*" (type strain RefSeq
+Assembly Accession GCF_017498775.1) replaces the putative genomospecies
+previously referred to as "Unknown Species 17" in the standardized taxonomy *
+*Bacillus rhizoplanae* (type strain RefSeq Assembly Accession GCF_917563915.1)
+represents a novel genomospecies within the standardized taxonomy and has been
+added to the database * All members of "*Bacillus pretiosus*" (type strain
+RefSeq Assembly Accession GCF_025916425.1) belong to *B. mosaicus* (i.e., "*B.
+pretiosus*" is not considered a novel species in the standardized taxonomy)
+**Importantly, *B. cereus* group species are often proposed in the literature
+using unstandardized approaches** (e.g., varying genomospecies thresholds,
+which may produce overlapping genomospecies). We have added the type strain
+comparison method in BTyper3 v3.2.0, as users may still want to compare a query
+genome with the type strains of published *B. cereus* group species. However,
+interpret results with caution, as some *B. cereus* group genomes may belong to
+multiple species using type strain genomes. For more information, check out
+our: * Review_of_*B._cereus*_group_taxonomy/nomenclature * Standardized
+nomenclature_for_the_*B._cereus*_group * Comparison_of_our_standardized
+nomenclature_to_other_*B._cereus*_group_typing_methods_(e.g.,_MLST,_*panC*,
+ANI-based_comparisons_to_species_type_strain_genomes) -------------------------
+----------------------------------------------- ## Citation ### If you found
+the BTyper3 tool, its source code, and/or any of its associated databases
+useful, please cite: Carroll, Laura M., Martin Wiedmann, Jasna Kovac. 2020.
+"Proposal_of_a_Taxonomic_Nomenclature_for_the_*Bacillus_cereus*_Group_Which
+Reconciles_Genomic_Definitions_of_Bacterial_Species_with_Clinical_and
 Industrial_Phenotypes." *mBio* 11(1): e00034-20; DOI: 10.1128/mBio.00034-20.
 Carroll, Laura M., Rachel A. Cheng, Jasna Kovac. 2020. "No_Assembly_Required:
 Using_BTyper3_to_Assess_the_Congruency_of_a_Proposed_Taxonomic_Framework_for
 the_*Bacillus_cereus*_group_with_Historical_Typing_Methods." *Frontiers in
 Microbiology* 11: 580691; DOI: 10.3389/fmicb.2020.580691. ---------------------
 --------------------------------------------------- ## Quick Start For detailed
 information, check out the BTyper3_wiki ### Command Structure ``` btyper3 -i
@@ -87,31 +90,31 @@
 Commands #### Perform all default analyses, using an assembled genome (complete
 or draft) in (multi-)FASTA format as input (assumes fastANI is in the user's
 path): ``` btyper3 -i /path/to/genome.fasta -o /path/to/desired/
 output_directory ``` #### Perform all default analyses, using an assembled
 genome (complete or draft) in (multi-)FASTA format as input (fastANI is not in
 the user's path): ``` btyper3 -i /path/to/genome.fasta -o /path/to/desired/
 output_directory --fastani_path /path/to/FastANI_executable/fastANI ``` ####
-Perform all default analyses, plus pseudo-gene flow unit assignment AND species
-type strain comparison, using an assembled genome (complete or draft) in
-(multi-)FASTA format as input (assumes fastANI is in the user's path): ```
-btyper3 -i /path/to/genome.fasta -o /path/to/desired/output_directory --
-ani_geneflow True --ani_typestrains True ``` #### Perform seven-gene MLST only,
-using user-supplied MLST gene sequences and the latest version of the PubMLST
-*B. cereus s.l.* database (sequences can be in multi-FASTA format, or
-concatenated into a single sequence in FASTA format): ``` btyper3 -i /path/to/
-mlst.fasta -o /path/to/desired/output_directory --ani_species False --
-ani_subspecies False --virulence False --bt False --panC False --
-download_mlst_latest True ``` #### Perform *panC* group assignment only, using
-a user-supplied *panC* gene sequence in FASTA format: ``` btyper3 -i /path/to/
-panC.fasta -o /path/to/desired/output_directory --ani_species False --
-ani_subspecies False --virulence False --bt False --mlst False ``` #### Perform
-virulence factor and Bt toxin-encoding gene detection in a plasmid sequence in
-FASTA format: ``` btyper3 -i /path/to/plasmid.fasta -o /path/to/desired/
-output_directory --ani_species False --ani_subspecies False --mlst False --panC
-False ``` ---------------------------------------------------------------------
---- Disclaimer: BTyper3 is pretty neat! However, no tool is perfect, and
-BTyper3 cannot definitively prove whether an isolate is pathogenic or not. As
-always, interpret your results with caution. We are not responsible for
-taxonomic misclassifications, misclassifications of an isolate's pathogenic
-potential or industrial utility, and/or misinterpretations (biological,
-statistical, or otherwise) of BTyper3 results.
+Perform all default analyses, plus pseudo-gene flow unit assignment, using an
+assembled genome (complete or draft) in (multi-)FASTA format as input (assumes
+fastANI is in the user's path): ``` btyper3 -i /path/to/genome.fasta -o /path/
+to/desired/output_directory --ani_geneflow True ``` #### Perform seven-gene
+MLST only, using user-supplied MLST gene sequences and the latest version of
+the PubMLST *B. cereus s.l.* database (sequences can be in multi-FASTA format,
+or concatenated into a single sequence in FASTA format): ``` btyper3 -i /path/
+to/mlst.fasta -o /path/to/desired/output_directory --ani_species False --
+ani_subspecies False --ani_typestrains False --virulence False --bt False --
+panC False --download_mlst_latest True ``` #### Perform *panC* group assignment
+only, using a user-supplied *panC* gene sequence in FASTA format: ``` btyper3 -
+i /path/to/panC.fasta -o /path/to/desired/output_directory --ani_species False
+--ani_subspecies False --ani_typestrains False --virulence False --bt False --
+mlst False ``` #### Perform virulence factor and Bt toxin-encoding gene
+detection in a plasmid sequence in FASTA format: ``` btyper3 -i /path/to/
+plasmid.fasta -o /path/to/desired/output_directory --ani_species False --
+ani_subspecies False --ani_typestrains False --mlst False --panC False ``` ----
+-------------------------------------------------------------------
+- Disclaimer: BTyper3 is pretty neat! However, no tool is perfect, and BTyper3
+cannot definitively prove whether an isolate is pathogenic or not. As always,
+interpret your results with caution. We are not responsible for taxonomic
+misclassifications, misclassifications of an isolate's pathogenic potential or
+industrial utility, and/or misinterpretations (biological, statistical, or
+otherwise) of BTyper3 results.
```

### Comparing `btyper3-3.3.4/btyper3/__init__.py` & `btyper3-3.4.0/btyper3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from .ani import Ani
 from .blast import Blast
 from .mlst import Mlst
 from .print_final_results import FinalResults
 
 __author__ = "Laura M. Carroll <lmc297@cornell.edu>"
-__version__ = "3.3.4"
+__version__ = "3.4.0"
 
 
 @contextlib.contextmanager
 def _forward_warnings():
 	_showwarning = warnings.showwarning
 	try:
 		warnings.showwarning = lambda message, category, filename, lineno, file=None, line=None: logging.warning(f"Warning: {message}")
@@ -413,15 +413,15 @@
 
 	parser.add_argument("--ani_species", help = "Optional argument; True or False; assign genome to a species using FastANI; default = True", nargs = "?", default = "True")
 
 	parser.add_argument("--ani_subspecies", help = "Optional argument; True or False; assign genome to a subspecies, if relevant, using FastANI; default = True", nargs = "?", default = "True")
 
 	parser.add_argument("--ani_geneflow", help = "Optional argument; True or False; assign genome to a pseudo-gene flow unit using the method described by Carroll, et al. using FastANI; default = False", nargs = "?", default = "False")
 
-	parser.add_argument("--ani_typestrains", help = "Optional argument; True or False; calculate ANI values between the query genome relative to all B. cereus s.l. species type strain genomes using FastANI, and report the closest species type strain/highest ANI value; default = False", nargs = "?", default = "False")
+	parser.add_argument("--ani_typestrains", help = "Optional argument; True or False; calculate ANI values between the query genome relative to all B. cereus s.l. species type strain genomes using FastANI, and report the closest species type strain/highest ANI value; default = True", nargs = "?", default = "True")
 
 	parser.add_argument("--virulence", help = "Optional argument; True or False; perform virulence gene detection (required if one wants to assign genomes to biovars Anthracis or Emeticus); default = True", nargs = "?", default = "True")
 
 	parser.add_argument("--bt", help = "Optional argument; True or False; perform Bt toxin gene detection for cry, cyt, and vip genes (required if one wants to assign genomes to biovar Thuringiensis); default = True", nargs = "?", default = "True")
 
 	parser.add_argument("--mlst", help = "Optional argument; True or False; assign genome to a sequence type (ST) using the seven-gene multi-locus sequence typing (MLST) scheme available in PubMLST; default = True", nargs = "?", default = "True")
```

### Comparing `btyper3-3.3.4/btyper3/ani.py` & `btyper3-3.4.0/btyper3/ani.py`

 * *Files identical despite different names*

### Comparing `btyper3-3.3.4/btyper3/blast.py` & `btyper3-3.4.0/btyper3/blast.py`

 * *Files identical despite different names*

### Comparing `btyper3-3.3.4/btyper3/mlst.py` & `btyper3-3.4.0/btyper3/mlst.py`

 * *Files identical despite different names*

### Comparing `btyper3-3.3.4/btyper3/print_final_results.py` & `btyper3-3.4.0/btyper3/print_final_results.py`

 * *Files identical despite different names*

### Comparing `btyper3-3.3.4/btyper3/seq_ani_db/geneflow/geneflow.tsv` & `btyper3-3.4.0/btyper3/seq_ani_db/geneflow/geneflow.tsv`

 * *Files identical despite different names*

### Comparing `btyper3-3.3.4/btyper3/seq_ani_db/species/species.tsv` & `btyper3-3.4.0/btyper3/seq_ani_db/species/species.tsv`

 * *Files identical despite different names*

### Comparing `btyper3-3.3.4/btyper3/seq_ani_db/typestrains/typestrains.tsv` & `btyper3-3.4.0/btyper3/seq_ani_db/typestrains/typestrains.tsv`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 B_mobilis_0711P9-1_GCF_001884045.fna.gz	mobilis	https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/001/884/045/GCF_001884045.1_ASM188404v1/GCF_001884045.1_ASM188404v1_genomic.fna.gz
 B_mycoides_DSM_2048_GCF_000003925.fna.gz	mycoides	https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/003/925/GCF_000003925.1_ASM392v1/GCF_000003925.1_ASM392v1_genomic.fna.gz
 B_nitratireducens_4049_GCF_001884135.fna.gz	nitratireducens	https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/001/884/135/GCF_001884135.1_ASM188413v1/GCF_001884135.1_ASM188413v1_genomic.fna.gz
 B_pacificus_EB422_GCF_001884025.fna.gz	pacificus	https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/001/884/025/GCF_001884025.1_ASM188402v1/GCF_001884025.1_ASM188402v1_genomic.fna.gz
 B_paramobilis_BML-BC017_GCF_018332495.fna.gz	paramobilis	https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/018/332/495/GCF_018332495.1_ASM1833249v1/GCF_018332495.1_ASM1833249v1_genomic.fna.gz
 B_paramycoides_NH24A2_GCF_001884235.fna.gz	paramycoides	https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/001/884/235/GCF_001884235.1_ASM188423v1/GCF_001884235.1_ASM188423v1_genomic.fna.gz
 B_paranthracis_Mn5_GCF_001883995.fna.gz	paranthracis	https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/001/883/995/GCF_001883995.1_ASM188399v1/GCF_001883995.1_ASM188399v1_genomic.fna.gz
+B_pretiosus_SAICEU11T_GCF_025916425.fna.gz	pretiosus	https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/025/916/425/GCF_025916425.1_ASM2591642v1/GCF_025916425.1_ASM2591642v1_genomic.fna.gz
 B_proteolyticus_TD42_GCF_001884065.fna.gz	proteolyticus	https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/001/884/065/GCF_001884065.1_ASM188406v1/GCF_001884065.1_ASM188406v1_genomic.fna.gz
 B_pseudomycoides_DSM_12442_GCF_000161455.fna.gz	pseudomycoides	https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/161/455/GCF_000161455.1_ASM16145v1/GCF_000161455.1_ASM16145v1_genomic.fna.gz
 B_rhizoplanae_CIP_111899_GCF_917563915.fna.gz	rhizoplanae	https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/917/563/915/GCF_917563915.1_JJ-63/GCF_917563915.1_JJ-63_genomic.fna.gz
 B_sanguinis_BML-BC004_GCF_018332475.fna.gz	sanguinis	https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/018/332/475/GCF_018332475.1_ASM1833247v1/GCF_018332475.1_ASM1833247v1_genomic.fna.gz
 B_thuringiensis_serovar_berliner_ATCC_10792_GCF_000161615.fna.gz	thuringiensis	https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/161/615/GCF_000161615.1_ASM16161v1/GCF_000161615.1_ASM16161v1_genomic.fna.gz
 B_toyonensis_BCT-7112_GCF_000496285.fna.gz	toyonensis	ftp://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/496/285/GCF_000496285.1_ASM49628v1/GCF_000496285.1_ASM49628v1_genomic.fna.gz
 B_tropicus_N24_GCF_001884035.fna.gz	tropicus	https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/001/884/035/GCF_001884035.1_ASM188403v1/GCF_001884035.1_ASM188403v1_genomic.fna.gz
```

### Comparing `btyper3-3.3.4/btyper3/seq_bt_db/btyper3_bt_sequences.faa` & `btyper3-3.4.0/btyper3/seq_bt_db/btyper3_bt_sequences.faa`

 * *Files identical despite different names*

### Comparing `btyper3-3.3.4/btyper3/seq_mlst_db/pubmlst.xml` & `btyper3-3.4.0/btyper3/seq_mlst_db/pubmlst.xml`

 * *Files identical despite different names*

### Comparing `btyper3-3.3.4/btyper3/seq_panC_db/panC.fna` & `btyper3-3.4.0/btyper3/seq_panC_db/panC.fna`

 * *Files identical despite different names*

### Comparing `btyper3-3.3.4/btyper3/seq_virulence_db/btyper3_virulence_sequences.faa` & `btyper3-3.4.0/btyper3/seq_virulence_db/btyper3_virulence_sequences.faa`

 * *Files identical despite different names*

### Comparing `btyper3-3.3.4/btyper3/seq_virulence_db/btyper3_virulence_sequences.ffn` & `btyper3-3.4.0/btyper3/seq_virulence_db/btyper3_virulence_sequences.ffn`

 * *Files identical despite different names*

### Comparing `btyper3-3.3.4/btyper3.egg-info/PKG-INFO` & `btyper3-3.4.0/btyper3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btyper3
-Version: 3.3.4
+Version: 3.4.0
 Summary: In silico taxonomic classification of Bacillus cereus group isolates using assembled genomes
 Home-page: https://github.com/lmc297/btyper3
 Author: Laura M. Carroll
 Author-email: lmc297@cornell.edu
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/lmc297/btyper3/issues
 Project-URL: Publication, https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7536271/
@@ -84,30 +84,32 @@
 3. Install via `pip` (this will download required Python dependencies as well):
    ```console
    pip install btyper3  
    ```
 
 ------------------------------------------------------------------------
 
-## News: updates in BTyper3 v3.2.0 and v3.3.0 -- new species just dropped!
+## News: updates in BTyper3 v3.2.0, v3.3.0, and v3.4.0 -- new species just dropped!
 
 The primary function of BTyper3 is to allow users to taxonomically classify *B. cereus* group genomes using a standardized nomenclature (see <a href="https://journals.asm.org/doi/10.1128/mBio.00034-20">here</a> and <a href="https://www.frontiersin.org/articles/10.3389/fmicb.2020.580691/full">here</a> for details regarding how the standardized nomenclature was constructed, and how it compares to historical typing methods, respectively). However, we understand that some users may also want to compare their *B. cereus* group genomes to the type strain genomes of published *B. cereus* group species. Thus, in BTyper3 v3.2.0, we have added the `--ani_typestrains` option, which calculates ANI values between a query genome and the genomes of all published *B. cereus* group species type strains and reports the type strain that produces the highest ANI value.
 
-The type strain genomes used by BTyper3's `--ani_typestrains` option correspond to the species discussed in <a href="https://www.tandfonline.com/doi/full/10.1080/10408398.2021.1916735">Figure 2 of our taxonomy review</a>, plus five species published after the review was published</a> (i.e., *Bacillus sanguinis*, *Bacillus paramobilis*, and *Bacillus hominis*, added in v3.2.0, and "*B. arachidis*" and *B. rhizoplanae*, added in v3.3.0). Within the standardized taxonomy that BTyper3 uses for genomospecies assignment:
+The type strain genomes used by BTyper3's `--ani_typestrains` option correspond to the species discussed in <a href="https://www.tandfonline.com/doi/full/10.1080/10408398.2021.1916735">Figure 2 of our taxonomy review</a>, plus species published after the review was published</a> (i.e., *Bacillus sanguinis*, *Bacillus paramobilis*, and *Bacillus hominis*, added in v3.2.0; "*B. arachidis*" and *B. rhizoplanae*, added in v3.3.0; "*B. pretiosus*", added in v3.4.0). Within the standardized taxonomy that BTyper3 uses for genomospecies assignment:
 
 * All members of *Bacillus sanguinis* (type strain RefSeq Assembly Accession GCF_018332475.1) belong to *B. mosaicus* (i.e., *B. sanguinis* is not considered a novel species in the standardized taxonomy)
 
 * All members of *Bacillus paramobilis* (type strain RefSeq Assembly Accession GCF_018332495.1) belong to *B. mosaicus* (i.e., *B. paramobilis* is not considered a novel species in the standardized taxonomy)
 
 * All members of *Bacillus hominis* (type strain RefSeq Assembly Accession GCF_018332515.1) belong to *B. mycoides* (i.e., *B. hominis* is not considered a novel species in the standardized taxonomy)
 
 * "*Bacillus arachidis*" (type strain RefSeq Assembly Accession GCF_017498775.1) replaces the putative genomospecies previously referred to as "Unknown Species 17" in the standardized taxonomy
 
 * *Bacillus rhizoplanae* (type strain RefSeq Assembly Accession GCF_917563915.1) represents a novel genomospecies within the standardized taxonomy and has been added to the database
 
+* All members of "*Bacillus pretiosus*" (type strain RefSeq Assembly Accession GCF_025916425.1) belong to *B. mosaicus* (i.e., "*B. pretiosus*" is not considered a novel species in the standardized taxonomy)
+
 **Importantly, *B. cereus* group species are often proposed in the literature using unstandardized approaches** (e.g., varying genomospecies thresholds, which may produce overlapping genomospecies). We have added the type strain comparison method in BTyper3 v3.2.0, as users may still want to compare a query genome with the type strains of published *B. cereus* group species. However, interpret results with caution, as some *B. cereus* group genomes may belong to multiple species using type strain genomes.
 
 For more information, check out our:
 
 * <a href="https://www.tandfonline.com/doi/full/10.1080/10408398.2021.1916735">Review of *B. cereus* group taxonomy/nomenclature</a>
 
 * <a href="https://journals.asm.org/doi/full/10.1128/mBio.00034-20">Standardized nomenclature for the *B. cereus* group</a>
@@ -151,36 +153,36 @@
 
 #### Perform all default analyses, using an assembled genome (complete or draft) in (multi-)FASTA format as input (fastANI is not in the user's path):
 
 ```
 btyper3 -i /path/to/genome.fasta -o /path/to/desired/output_directory --fastani_path /path/to/FastANI_executable/fastANI
 ```
 
-#### Perform all default analyses, plus pseudo-gene flow unit assignment AND species type strain comparison, using an assembled genome (complete or draft) in (multi-)FASTA format as input (assumes fastANI is in the user's path):
+#### Perform all default analyses, plus pseudo-gene flow unit assignment, using an assembled genome (complete or draft) in (multi-)FASTA format as input (assumes fastANI is in the user's path):
 
 ```
-btyper3 -i /path/to/genome.fasta -o /path/to/desired/output_directory --ani_geneflow True --ani_typestrains True
+btyper3 -i /path/to/genome.fasta -o /path/to/desired/output_directory --ani_geneflow True
 ```
 
 #### Perform seven-gene MLST only, using user-supplied MLST gene sequences and the latest version of the PubMLST *B. cereus s.l.* database (sequences can be in multi-FASTA format, or concatenated into a single sequence in FASTA format):
 
 ```
-btyper3 -i /path/to/mlst.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --virulence False --bt False --panC False --download_mlst_latest True
+btyper3 -i /path/to/mlst.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --ani_typestrains False --virulence False --bt False --panC False --download_mlst_latest True
 ```
 
 #### Perform *panC* group assignment only, using a user-supplied *panC* gene sequence in FASTA format:
 
 ```
-btyper3 -i /path/to/panC.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --virulence False --bt False --mlst False
+btyper3 -i /path/to/panC.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --ani_typestrains False --virulence False --bt False --mlst False
 ```
 
 #### Perform virulence factor and Bt toxin-encoding gene detection in a plasmid sequence in FASTA format:
 
 ```
-btyper3 -i /path/to/plasmid.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --mlst False --panC False
+btyper3 -i /path/to/plasmid.fasta -o /path/to/desired/output_directory --ani_species False --ani_subspecies False --ani_typestrains False --mlst False --panC False
 ```
 
 
 ------------------------------------------------------------------------
 
 
 Disclaimer: BTyper3 is pretty neat! However, no tool is perfect, and BTyper3 cannot definitively prove whether an isolate is pathogenic or not. As always, interpret your results with caution. We are not responsible for taxonomic misclassifications, misclassifications of an isolate's pathogenic potential or industrial utility, and/or misinterpretations (biological, statistical, or otherwise) of BTyper3 results.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: btyper3 Version: 3.3.4 Summary: In silico taxonomic
+Metadata-Version: 2.1 Name: btyper3 Version: 3.4.0 Summary: In silico taxonomic
 classification of Bacillus cereus group isolates using assembled genomes Home-
 page: https://github.com/lmc297/btyper3 Author: Laura M. Carroll Author-email:
 lmc297@cornell.edu License: GPLv3 Project-URL: Bug Tracker, https://github.com/
 lmc297/btyper3/issues Project-URL: Publication, https://www.ncbi.nlm.nih.gov/
 pmc/articles/PMC7536271/ Project-URL: Changelog, https://github.com/lmc297/
 btyper3/blob/master/archive/CHANGELOG.md Keywords: bacillus,taxonomy,genome,ANI
 Platform: any Classifier: Development Status :: 6 - Mature Classifier: Intended
@@ -38,60 +38,63 @@
 Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=Download) v2.9.0+ and up  2.
 [Add BLAST+ to your path](https://unix.stackexchange.com/questions/26047/how-
 to-correctly-add-a-path-to-path), if necessary (to check if BLAST+ is in your
 path, try running `makeblastdb -h` and `tblastn -h` from your command line; you
 should get a help message for each command, with no error messages) 3. Install
 via `pip` (this will download required Python dependencies as well): ```console
 pip install btyper3 ``` -------------------------------------------------------
------------------ ## News: updates in BTyper3 v3.2.0 and v3.3.0 -- new species
-just dropped! The primary function of BTyper3 is to allow users to
+----------------- ## News: updates in BTyper3 v3.2.0, v3.3.0, and v3.4.0 -- new
+species just dropped! The primary function of BTyper3 is to allow users to
 taxonomically classify *B. cereus* group genomes using a standardized
 nomenclature (see here and here for details regarding how the standardized
 nomenclature was constructed, and how it compares to historical typing methods,
 respectively). However, we understand that some users may also want to compare
 their *B. cereus* group genomes to the type strain genomes of published *B.
 cereus* group species. Thus, in BTyper3 v3.2.0, we have added the `--
 ani_typestrains` option, which calculates ANI values between a query genome and
 the genomes of all published *B. cereus* group species type strains and reports
 the type strain that produces the highest ANI value. The type strain genomes
 used by BTyper3's `--ani_typestrains` option correspond to the species
-discussed in Figure_2_of_our_taxonomy_review, plus five species published after
-the review was published
+discussed in Figure_2_of_our_taxonomy_review, plus species published after the
+review was published
  (i.e., *Bacillus sanguinis*, *Bacillus paramobilis*, and *Bacillus hominis*,
-added in v3.2.0, and "*B. arachidis*" and *B. rhizoplanae*, added in v3.3.0).
-Within the standardized taxonomy that BTyper3 uses for genomospecies
-assignment: * All members of *Bacillus sanguinis* (type strain RefSeq Assembly
-Accession GCF_018332475.1) belong to *B. mosaicus* (i.e., *B. sanguinis* is not
-considered a novel species in the standardized taxonomy) * All members of
-*Bacillus paramobilis* (type strain RefSeq Assembly Accession GCF_018332495.1)
-belong to *B. mosaicus* (i.e., *B. paramobilis* is not considered a novel
-species in the standardized taxonomy) * All members of *Bacillus hominis* (type
-strain RefSeq Assembly Accession GCF_018332515.1) belong to *B. mycoides*
-(i.e., *B. hominis* is not considered a novel species in the standardized
-taxonomy) * "*Bacillus arachidis*" (type strain RefSeq Assembly Accession
-GCF_017498775.1) replaces the putative genomospecies previously referred to as
-"Unknown Species 17" in the standardized taxonomy * *Bacillus rhizoplanae*
-(type strain RefSeq Assembly Accession GCF_917563915.1) represents a novel
-genomospecies within the standardized taxonomy and has been added to the
-database **Importantly, *B. cereus* group species are often proposed in the
-literature using unstandardized approaches** (e.g., varying genomospecies
-thresholds, which may produce overlapping genomospecies). We have added the
-type strain comparison method in BTyper3 v3.2.0, as users may still want to
-compare a query genome with the type strains of published *B. cereus* group
-species. However, interpret results with caution, as some *B. cereus* group
-genomes may belong to multiple species using type strain genomes. For more
-information, check out our: * Review_of_*B._cereus*_group_taxonomy/nomenclature
-* Standardized_nomenclature_for_the_*B._cereus*_group * Comparison_of_our
-standardized_nomenclature_to_other_*B._cereus*_group_typing_methods_(e.g.,
-MLST,_*panC*,_ANI-based_comparisons_to_species_type_strain_genomes) -----------
-------------------------------------------------------------- ## Citation ###
-If you found the BTyper3 tool, its source code, and/or any of its associated
-databases useful, please cite: Carroll, Laura M., Martin Wiedmann, Jasna Kovac.
-2020. "Proposal_of_a_Taxonomic_Nomenclature_for_the_*Bacillus_cereus*_Group
-Which_Reconciles_Genomic_Definitions_of_Bacterial_Species_with_Clinical_and
+added in v3.2.0; "*B. arachidis*" and *B. rhizoplanae*, added in v3.3.0; "*B.
+pretiosus*", added in v3.4.0). Within the standardized taxonomy that BTyper3
+uses for genomospecies assignment: * All members of *Bacillus sanguinis* (type
+strain RefSeq Assembly Accession GCF_018332475.1) belong to *B. mosaicus*
+(i.e., *B. sanguinis* is not considered a novel species in the standardized
+taxonomy) * All members of *Bacillus paramobilis* (type strain RefSeq Assembly
+Accession GCF_018332495.1) belong to *B. mosaicus* (i.e., *B. paramobilis* is
+not considered a novel species in the standardized taxonomy) * All members of
+*Bacillus hominis* (type strain RefSeq Assembly Accession GCF_018332515.1)
+belong to *B. mycoides* (i.e., *B. hominis* is not considered a novel species
+in the standardized taxonomy) * "*Bacillus arachidis*" (type strain RefSeq
+Assembly Accession GCF_017498775.1) replaces the putative genomospecies
+previously referred to as "Unknown Species 17" in the standardized taxonomy *
+*Bacillus rhizoplanae* (type strain RefSeq Assembly Accession GCF_917563915.1)
+represents a novel genomospecies within the standardized taxonomy and has been
+added to the database * All members of "*Bacillus pretiosus*" (type strain
+RefSeq Assembly Accession GCF_025916425.1) belong to *B. mosaicus* (i.e., "*B.
+pretiosus*" is not considered a novel species in the standardized taxonomy)
+**Importantly, *B. cereus* group species are often proposed in the literature
+using unstandardized approaches** (e.g., varying genomospecies thresholds,
+which may produce overlapping genomospecies). We have added the type strain
+comparison method in BTyper3 v3.2.0, as users may still want to compare a query
+genome with the type strains of published *B. cereus* group species. However,
+interpret results with caution, as some *B. cereus* group genomes may belong to
+multiple species using type strain genomes. For more information, check out
+our: * Review_of_*B._cereus*_group_taxonomy/nomenclature * Standardized
+nomenclature_for_the_*B._cereus*_group * Comparison_of_our_standardized
+nomenclature_to_other_*B._cereus*_group_typing_methods_(e.g.,_MLST,_*panC*,
+ANI-based_comparisons_to_species_type_strain_genomes) -------------------------
+----------------------------------------------- ## Citation ### If you found
+the BTyper3 tool, its source code, and/or any of its associated databases
+useful, please cite: Carroll, Laura M., Martin Wiedmann, Jasna Kovac. 2020.
+"Proposal_of_a_Taxonomic_Nomenclature_for_the_*Bacillus_cereus*_Group_Which
+Reconciles_Genomic_Definitions_of_Bacterial_Species_with_Clinical_and
 Industrial_Phenotypes." *mBio* 11(1): e00034-20; DOI: 10.1128/mBio.00034-20.
 Carroll, Laura M., Rachel A. Cheng, Jasna Kovac. 2020. "No_Assembly_Required:
 Using_BTyper3_to_Assess_the_Congruency_of_a_Proposed_Taxonomic_Framework_for
 the_*Bacillus_cereus*_group_with_Historical_Typing_Methods." *Frontiers in
 Microbiology* 11: 580691; DOI: 10.3389/fmicb.2020.580691. ---------------------
 --------------------------------------------------- ## Quick Start For detailed
 information, check out the BTyper3_wiki ### Command Structure ``` btyper3 -i
@@ -100,31 +103,31 @@
 Commands #### Perform all default analyses, using an assembled genome (complete
 or draft) in (multi-)FASTA format as input (assumes fastANI is in the user's
 path): ``` btyper3 -i /path/to/genome.fasta -o /path/to/desired/
 output_directory ``` #### Perform all default analyses, using an assembled
 genome (complete or draft) in (multi-)FASTA format as input (fastANI is not in
 the user's path): ``` btyper3 -i /path/to/genome.fasta -o /path/to/desired/
 output_directory --fastani_path /path/to/FastANI_executable/fastANI ``` ####
-Perform all default analyses, plus pseudo-gene flow unit assignment AND species
-type strain comparison, using an assembled genome (complete or draft) in
-(multi-)FASTA format as input (assumes fastANI is in the user's path): ```
-btyper3 -i /path/to/genome.fasta -o /path/to/desired/output_directory --
-ani_geneflow True --ani_typestrains True ``` #### Perform seven-gene MLST only,
-using user-supplied MLST gene sequences and the latest version of the PubMLST
-*B. cereus s.l.* database (sequences can be in multi-FASTA format, or
-concatenated into a single sequence in FASTA format): ``` btyper3 -i /path/to/
-mlst.fasta -o /path/to/desired/output_directory --ani_species False --
-ani_subspecies False --virulence False --bt False --panC False --
-download_mlst_latest True ``` #### Perform *panC* group assignment only, using
-a user-supplied *panC* gene sequence in FASTA format: ``` btyper3 -i /path/to/
-panC.fasta -o /path/to/desired/output_directory --ani_species False --
-ani_subspecies False --virulence False --bt False --mlst False ``` #### Perform
-virulence factor and Bt toxin-encoding gene detection in a plasmid sequence in
-FASTA format: ``` btyper3 -i /path/to/plasmid.fasta -o /path/to/desired/
-output_directory --ani_species False --ani_subspecies False --mlst False --panC
-False ``` ---------------------------------------------------------------------
---- Disclaimer: BTyper3 is pretty neat! However, no tool is perfect, and
-BTyper3 cannot definitively prove whether an isolate is pathogenic or not. As
-always, interpret your results with caution. We are not responsible for
-taxonomic misclassifications, misclassifications of an isolate's pathogenic
-potential or industrial utility, and/or misinterpretations (biological,
-statistical, or otherwise) of BTyper3 results.
+Perform all default analyses, plus pseudo-gene flow unit assignment, using an
+assembled genome (complete or draft) in (multi-)FASTA format as input (assumes
+fastANI is in the user's path): ``` btyper3 -i /path/to/genome.fasta -o /path/
+to/desired/output_directory --ani_geneflow True ``` #### Perform seven-gene
+MLST only, using user-supplied MLST gene sequences and the latest version of
+the PubMLST *B. cereus s.l.* database (sequences can be in multi-FASTA format,
+or concatenated into a single sequence in FASTA format): ``` btyper3 -i /path/
+to/mlst.fasta -o /path/to/desired/output_directory --ani_species False --
+ani_subspecies False --ani_typestrains False --virulence False --bt False --
+panC False --download_mlst_latest True ``` #### Perform *panC* group assignment
+only, using a user-supplied *panC* gene sequence in FASTA format: ``` btyper3 -
+i /path/to/panC.fasta -o /path/to/desired/output_directory --ani_species False
+--ani_subspecies False --ani_typestrains False --virulence False --bt False --
+mlst False ``` #### Perform virulence factor and Bt toxin-encoding gene
+detection in a plasmid sequence in FASTA format: ``` btyper3 -i /path/to/
+plasmid.fasta -o /path/to/desired/output_directory --ani_species False --
+ani_subspecies False --ani_typestrains False --mlst False --panC False ``` ----
+-------------------------------------------------------------------
+- Disclaimer: BTyper3 is pretty neat! However, no tool is perfect, and BTyper3
+cannot definitively prove whether an isolate is pathogenic or not. As always,
+interpret your results with caution. We are not responsible for taxonomic
+misclassifications, misclassifications of an isolate's pathogenic potential or
+industrial utility, and/or misinterpretations (biological, statistical, or
+otherwise) of BTyper3 results.
```

### Comparing `btyper3-3.3.4/btyper3.egg-info/SOURCES.txt` & `btyper3-3.4.0/btyper3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `btyper3-3.3.4/setup.cfg` & `btyper3-3.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `btyper3-3.3.4/setup.py` & `btyper3-3.4.0/setup.py`

 * *Files identical despite different names*

