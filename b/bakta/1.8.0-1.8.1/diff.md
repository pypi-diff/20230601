# Comparing `tmp/bakta-1.8.0.tar.gz` & `tmp/bakta-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bakta-1.8.0.tar", last modified: Tue May 30 14:58:34 2023, max compression
+gzip compressed data, was "bakta-1.8.1.tar", last modified: Thu Jun  1 09:02:59 2023, max compression
```

## Comparing `bakta-1.8.0.tar` & `bakta-1.8.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:34.019009 bakta-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-30 14:58:23.000000 bakta-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    47858 2023-05-30 14:58:34.019009 bakta-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40267 2023-05-30 14:58:23.000000 bakta-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:34.015009 bakta-1.8.0/bakta/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:34.015009 bakta-1.8.0/bakta/expert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/expert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/expert/amrfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/expert/protein_sequences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:34.019009 bakta-1.8.0/bakta/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33942 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    43977 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/cds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/crispr.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/gaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/nc_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/nc_rna_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/orf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/ori.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/r_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/s_orf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/signal_peptides.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/t_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/tm_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:34.019009 bakta-1.8.0/bakta/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/io/fasta.py
--rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/io/gff.py
--rw-r--r--   0 runner    (1001) docker     (123)    19547 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/io/insdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/io/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/ips.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29754 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/proteins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/psc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/pscc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/so.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/ups.py
--rw-r--r--   0 runner    (1001) docker     (123)    27984 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:34.015009 bakta-1.8.0/bakta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47858 2023-05-30 14:58:33.000000 bakta-1.8.0/bakta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-30 14:58:33.000000 bakta-1.8.0/bakta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:58:33.000000 bakta-1.8.0/bakta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-30 14:58:33.000000 bakta-1.8.0/bakta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:58:33.000000 bakta-1.8.0/bakta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-30 14:58:33.000000 bakta-1.8.0/bakta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 14:58:33.000000 bakta-1.8.0/bakta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:58:34.019009 bakta-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-30 14:58:23.000000 bakta-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:34.019009 bakta-1.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    20648 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_bakta.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_bakta_proteins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_edge_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_nt_sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_pseudo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_sORF.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_sig_peps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_user_proteins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:02:59.229494 bakta-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-01 09:02:49.000000 bakta-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    47858 2023-06-01 09:02:59.229494 bakta-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40267 2023-06-01 09:02:49.000000 bakta-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:02:59.225494 bakta-1.8.1/bakta/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:02:59.225494 bakta-1.8.1/bakta/expert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/expert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/expert/amrfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/expert/protein_sequences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:02:59.229494 bakta-1.8.1/bakta/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33672 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/features/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43977 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/features/cds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/features/crispr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/features/gaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/features/nc_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/features/nc_rna_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/features/orf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/features/ori.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/features/r_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/features/s_orf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/features/signal_peptides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/features/t_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/features/tm_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:02:59.229494 bakta-1.8.1/bakta/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/io/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/io/gff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19547 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/io/insdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/io/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/ips.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29754 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/proteins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/psc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/pscc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/so.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/ups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27984 2023-06-01 09:02:49.000000 bakta-1.8.1/bakta/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:02:59.225494 bakta-1.8.1/bakta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47858 2023-06-01 09:02:59.000000 bakta-1.8.1/bakta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-01 09:02:59.000000 bakta-1.8.1/bakta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:02:59.000000 bakta-1.8.1/bakta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-01 09:02:59.000000 bakta-1.8.1/bakta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:02:59.000000 bakta-1.8.1/bakta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-01 09:02:59.000000 bakta-1.8.1/bakta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 09:02:59.000000 bakta-1.8.1/bakta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:02:59.229494 bakta-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-01 09:02:49.000000 bakta-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:02:59.229494 bakta-1.8.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    20648 2023-06-01 09:02:49.000000 bakta-1.8.1/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-01 09:02:49.000000 bakta-1.8.1/test/test_bakta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-01 09:02:49.000000 bakta-1.8.1/test/test_bakta_proteins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-01 09:02:49.000000 bakta-1.8.1/test/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-01 09:02:49.000000 bakta-1.8.1/test/test_edge_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-01 09:02:49.000000 bakta-1.8.1/test/test_nt_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-06-01 09:02:49.000000 bakta-1.8.1/test/test_pseudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-01 09:02:49.000000 bakta-1.8.1/test/test_sORF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-01 09:02:49.000000 bakta-1.8.1/test/test_sig_peps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-06-01 09:02:49.000000 bakta-1.8.1/test/test_user_proteins.py
```

### Comparing `bakta-1.8.0/LICENSE` & `bakta-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/PKG-INFO` & `bakta-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakta
-Version: 1.8.0
+Version: 1.8.1
 Summary: Bakta: rapid & standardized annotation of bacterial genomes, MAGs & plasmids
 Home-page: https://github.com/oschwengers/bakta
 Author: Oliver Schwengers
 Author-email: oliver.schwengers@computational.bio.uni-giessen.de
 License: GPLv3
 Project-URL: Documentation, https://bakta.readthedocs.io
 Project-URL: Source, https://github.com/oschwengers/bakta
```

### Comparing `bakta-1.8.0/README.md` & `bakta-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/config.py` & `bakta-1.8.1/bakta/config.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/constants.py` & `bakta-1.8.1/bakta/constants.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/db.py` & `bakta-1.8.1/bakta/db.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/expert/amrfinder.py` & `bakta-1.8.1/bakta/expert/amrfinder.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,37 +52,38 @@
         for line in fh:
             if(line[:7] != 'Protein'):
                 (
                     aa_identifier, gene, product, scope, element_type, element_subtype, clazz, subclass, method, target_length, reference_sequence_length,
                     cov_ref_seq, ident_ref_seq, alignment_length, accession_closest_seq, name_closest_seq, hmm_id, hmm_description
                 ) = line.split('\t')
                 cds = cds_by_hexdigest[aa_identifier]
-                expert_hit = {
+                hit = {
+                    'type': 'amrfinder',
                     'rank': 95,
                     'gene': gene if gene != '' else None,
                     'product': product,
                     'method': method
                 }
                 if(method.lower() != 'hmm'):
-                    expert_hit['query_cov'] = int(alignment_length) / len(cds['aa'])
+                    hit['query_cov'] = int(alignment_length) / len(cds['aa'])
                     model_cov = float(cov_ref_seq) / 100
-                    expert_hit['model_cov'] = model_cov
+                    hit['model_cov'] = model_cov
                     identity = float(ident_ref_seq) / 100
-                    expert_hit['identity'] = identity
-                    expert_hit['id'] = accession_closest_seq
-                    expert_hit['db_xrefs'] = [f'{bc.DB_XREF_NCBI_PROTEIN}:{accession_closest_seq}']
+                    hit['identity'] = identity
+                    hit['id'] = accession_closest_seq
+                    hit['db_xrefs'] = [f'{bc.DB_XREF_NCBI_PROTEIN}:{accession_closest_seq}']
                 else:
                     model_cov = 0
                     identity = 0
-                    expert_hit['id'] = hmm_id
-                    expert_hit['db_xrefs'] = [f'{bc.DB_XREF_NCBI_FAMILIES}:{hmm_id}']
+                    hit['id'] = hmm_id
+                    hit['db_xrefs'] = [f'{bc.DB_XREF_NCBI_FAMILIES}:{hmm_id}']
 
                 if('expert' not in cds):
-                    cds['expert'] = {}
-                cds['expert']['amrfinder'] = expert_hit
+                    cds['expert'] = []
+                cds['expert'].append(hit)
                 log.debug(
                     'hit: gene=%s, product=%s, method=%s, target-cov=%0.3f, identity=%0.3f, contig=%s, start=%i, stop=%i, strand=%s',
                     gene, product, method, model_cov, identity, cds['contig'], cds['start'], cds['stop'], cds['strand']
                 )
                 cds_found.add(aa_identifier)
 
     log.info('found=%i', len(cds_found))
```

### Comparing `bakta-1.8.0/bakta/expert/protein_sequences.py` & `bakta-1.8.1/bakta/expert/protein_sequences.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,35 +60,36 @@
             bitscore = float(bitscore)
             (source, rank, min_identity, min_query_cov, min_model_cov, gene, product, dbxrefs) = model_title.split(' ', 1)[1].split('~~~')
             rank = int(rank)
             min_identity = float(min_identity) / 100
             min_query_cov = float(min_query_cov) / 100
             min_model_cov = float(min_model_cov) / 100
             if(query_cov >= min_query_cov and model_cov >= min_model_cov and identity >= min_identity):
-                expert_hit = {
+                hit = {
+                    'type': expert_system,
                     'source': source,
                     'rank': rank,
                     'id': model_id,
                     'gene': gene if gene != '' else None,
                     'product': product,
                     'query_cov': query_cov,
                     'model_cov': model_cov,
                     'identity': identity,
                     'evalue': evalue,
                     'bitscore': bitscore,
                     'db_xrefs': [] if dbxrefs == '' else dbxrefs.split(',')
                 }
                 if(expert_system == 'user_proteins'):
-                    expert_hit['db_xrefs'].append(f'UserProtein:{model_id}')
+                    hit['db_xrefs'].append(f'UserProtein:{model_id}')
                 if('expert' not in cds):
-                    cds['expert'] = {}
-                cds['expert'][expert_system] = expert_hit
+                    cds['expert'] = []
+                cds['expert'].append(hit)
                 log.debug(
-                    'hit: contig=%s, start=%i, stop=%i, strand=%s, source=%s, rank=%i, query-cov=%0.3f, model-cov=%0.3f, identity=%0.3f, gene=%s, product=%s, evalue=%1.1e, bitscore=%f',
-                    cds['contig'], cds['start'], cds['stop'], cds['strand'], source, rank, query_cov, model_cov, identity, gene, product, evalue, bitscore
+                    'hit: source=%s, rank=%i, contig=%s, start=%i, stop=%i, strand=%s, query-cov=%0.3f, model-cov=%0.3f, identity=%0.3f, gene=%s, product=%s, evalue=%1.1e, bitscore=%f',
+                    source, rank, cds['contig'], cds['start'], cds['stop'], cds['strand'], query_cov, model_cov, identity, gene, product, evalue, bitscore
                 )
                 cds_found.add(aa_identifier)
 
     log.info('found=%i', len(cds_found))
     return cds_found
```

### Comparing `bakta-1.8.0/bakta/features/annotation.py` & `bakta-1.8.1/bakta/features/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     if(bc.PSEUDOGENE in feature):
         pseudogene_psc = feature[bc.PSEUDOGENE].get('psc', None)
         pseudogene_pscc = feature[bc.PSEUDOGENE].get('pscc', None)
     ups = feature.get('ups', None)
     ips = feature.get('ips', None)
     psc = feature.get('psc', None)
     pscc = feature.get('pscc', None)
-    expert = feature.get('expert', None)
+    expert_hits = feature.get('expert', [])
 
     gene = None
     genes = set()
     product = None
     db_xrefs = set()
     if(pseudogene_pscc):
         pseudogene_pscc_genes = pseudogene_pscc.get('gene', None)
@@ -97,30 +97,26 @@
             genes.update(ips_genes)
             gene = ips_genes[0]
         ips_product = ips.get('product', None)
         if(ips_product):
             product = ips_product
         for db_xref in ips['db_xrefs']:
             db_xrefs.add(db_xref)
-    if(expert):
-        rank = 0
-        for expert_system, expert_hit in expert.items():
-            expert_rank = expert_hit['rank']
-            if(expert_rank > rank):
-                expert_genes = expert_hit.get('gene', None)
-                if(expert_genes):
-                    expert_genes = expert_genes.replace('/', ',').split(',')
-                    genes.update(expert_genes)
-                    gene = expert_genes[0]
-                product = expert_hit.get('product', None)
-                expert_db_xrefs = expert_hit.get('db_xrefs', None)
-                if(expert_db_xrefs):
-                    for expert_db_xref in expert_db_xrefs:
-                        db_xrefs.add(expert_db_xref)
-                rank = expert_rank
+    rank = 0
+    for hit in expert_hits:
+        db_xrefs.update(hit.get('db_xrefs', []))
+        expert_rank = hit['rank']
+        if(expert_rank > rank):
+            expert_genes = hit.get('gene', None)
+            if(expert_genes):
+                expert_genes = expert_genes.replace('/', ',').split(',')
+                genes.update(expert_genes)
+                gene = expert_genes[0]
+            product = hit.get('product', None)
+            rank = expert_rank
 
     if(product):
         product = revise_cds_product(product)
         if(product):
             if(cfg.compliant):
                 product = insdc.revise_product_insdc(product)
             feature['product'] = product
```

### Comparing `bakta-1.8.0/bakta/features/cds.py` & `bakta-1.8.1/bakta/features/cds.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/features/crispr.py` & `bakta-1.8.1/bakta/features/crispr.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/features/gaps.py` & `bakta-1.8.1/bakta/features/gaps.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/features/nc_rna.py` & `bakta-1.8.1/bakta/features/nc_rna.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/features/nc_rna_region.py` & `bakta-1.8.1/bakta/features/nc_rna_region.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/features/orf.py` & `bakta-1.8.1/bakta/features/orf.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/features/ori.py` & `bakta-1.8.1/bakta/features/ori.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/features/r_rna.py` & `bakta-1.8.1/bakta/features/r_rna.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/features/s_orf.py` & `bakta-1.8.1/bakta/features/s_orf.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/features/signal_peptides.py` & `bakta-1.8.1/bakta/features/signal_peptides.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/features/t_rna.py` & `bakta-1.8.1/bakta/features/t_rna.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/features/tm_rna.py` & `bakta-1.8.1/bakta/features/tm_rna.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/io/fasta.py` & `bakta-1.8.1/bakta/io/fasta.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/io/gff.py` & `bakta-1.8.1/bakta/io/gff.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/io/insdc.py` & `bakta-1.8.1/bakta/io/insdc.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/io/json.py` & `bakta-1.8.1/bakta/io/json.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/io/tsv.py` & `bakta-1.8.1/bakta/io/tsv.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/ips.py` & `bakta-1.8.1/bakta/ips.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/main.py` & `bakta-1.8.1/bakta/main.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/plot.py` & `bakta-1.8.1/bakta/plot.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/proteins.py` & `bakta-1.8.1/bakta/proteins.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/psc.py` & `bakta-1.8.1/bakta/psc.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/pscc.py` & `bakta-1.8.1/bakta/pscc.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/so.py` & `bakta-1.8.1/bakta/so.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/ups.py` & `bakta-1.8.1/bakta/ups.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta/utils.py` & `bakta-1.8.1/bakta/utils.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/bakta.egg-info/PKG-INFO` & `bakta-1.8.1/bakta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakta
-Version: 1.8.0
+Version: 1.8.1
 Summary: Bakta: rapid & standardized annotation of bacterial genomes, MAGs & plasmids
 Home-page: https://github.com/oschwengers/bakta
 Author: Oliver Schwengers
 Author-email: oliver.schwengers@computational.bio.uni-giessen.de
 License: GPLv3
 Project-URL: Documentation, https://bakta.readthedocs.io
 Project-URL: Source, https://github.com/oschwengers/bakta
```

### Comparing `bakta-1.8.0/bakta.egg-info/SOURCES.txt` & `bakta-1.8.1/bakta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/setup.py` & `bakta-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/test/test_args.py` & `bakta-1.8.1/test/test_args.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/test/test_bakta.py` & `bakta-1.8.1/test/test_bakta.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/test/test_bakta_proteins.py` & `bakta-1.8.1/test/test_bakta_proteins.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/test/test_dependencies.py` & `bakta-1.8.1/test/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/test/test_edge_features.py` & `bakta-1.8.1/test/test_edge_features.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/test/test_nt_sequences.py` & `bakta-1.8.1/test/test_nt_sequences.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/test/test_pseudo.py` & `bakta-1.8.1/test/test_pseudo.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/test/test_sORF.py` & `bakta-1.8.1/test/test_sORF.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/test/test_sig_peps.py` & `bakta-1.8.1/test/test_sig_peps.py`

 * *Files identical despite different names*

### Comparing `bakta-1.8.0/test/test_user_proteins.py` & `bakta-1.8.1/test/test_user_proteins.py`

 * *Files 5% similar despite different names*

```diff
@@ -162,14 +162,13 @@
     with results_path.open() as fh:
         results = json.load(fh)
     assert results is not None
     
     ec_annotated = 0
     user_prot_feats = []
     for feat in results['features']:
-        if('expert' in feat and 'user_proteins' in feat['expert']):
-            user_prot_feats.append(feat)
-        for db_xref in feat['db_xrefs']:
-            if('EC' in db_xref):
-                ec_annotated += 1
+        for expert in feat.get('expert', []):
+            if(expert['type'] == 'user_proteins'):
+                user_prot_feats.append(feat)
+                ec_annotated += len([x for x in feat['db_xrefs'] if 'EC' in x])
     assert ec_annotated == 1
     assert len(user_prot_feats) == 1
```

