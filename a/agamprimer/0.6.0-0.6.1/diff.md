# Comparing `tmp/agamprimer-0.6.0.tar.gz` & `tmp/agamprimer-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agamprimer-0.6.0.tar", max compression
+gzip compressed data, was "agamprimer-0.6.1.tar", max compression
```

## Comparing `agamprimer-0.6.0.tar` & `agamprimer-0.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35049 2023-05-30 16:51:46.998781 agamprimer-0.6.0/AgamPrimer/AgamPrimer.py
--rw-r--r--   0        0        0       66 2022-12-19 20:36:15.048061 agamprimer-0.6.0/AgamPrimer/__init__.py
--rw-r--r--   0        0        0      761 2023-05-30 16:51:46.998781 agamprimer-0.6.0/AgamPrimer/agamPrimer.egg-info/PKG-INFO
--rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.0/AgamPrimer/agamPrimer.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.0/AgamPrimer/agamPrimer.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       11 2023-05-30 16:51:46.998781 agamprimer-0.6.0/AgamPrimer/agamPrimer.egg-info/top_level.txt
--rw-r--r--   0        0        0     1079 2022-10-08 11:18:21.612054 agamprimer-0.6.0/LICENSE
--rw-r--r--   0        0        0      726 2023-05-30 17:24:09.942962 agamprimer-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 agamprimer-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35048 2023-06-01 12:44:13.709658 agamprimer-0.6.1/AgamPrimer/AgamPrimer.py
+-rw-r--r--   0        0        0       66 2022-12-19 20:36:15.048061 agamprimer-0.6.1/AgamPrimer/__init__.py
+-rw-r--r--   0        0        0      761 2023-05-30 16:51:46.998781 agamprimer-0.6.1/AgamPrimer/agamPrimer.egg-info/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.1/AgamPrimer/agamPrimer.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.1/AgamPrimer/agamPrimer.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       11 2023-05-30 16:51:46.998781 agamprimer-0.6.1/AgamPrimer/agamPrimer.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1079 2022-10-08 11:18:21.612054 agamprimer-0.6.1/LICENSE
+-rw-r--r--   0        0        0      730 2023-06-01 12:44:13.713658 agamprimer-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 agamprimer-0.6.1/PKG-INFO
```

### Comparing `agamprimer-0.6.0/AgamPrimer/AgamPrimer.py` & `agamprimer-0.6.1/AgamPrimer/AgamPrimer.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,14 @@
 def primer_params(
     assay_type,
     primer_parameters=None,
     n_primer_pairs=None,
     amplicon_size_range=None,
     generate_defaults=False,
 ):
-
     """
     adds necessary parameters depending on assay_type, or can
     generate the default parameters
     """
 
     if generate_defaults:
         primer_parameters = {
@@ -642,15 +641,14 @@
     # check primers for specificity against the genome and write to file
     blat_df = gget_blat_genome(primer_df, assay_type, assembly="anoGam3")
     blat_df.to_csv(f"{out_dir}/{assay_name}.{assay_type}.blat.tsv", sep="\t")
     return (primer_df, blat_df)
 
 
 def _get_primer_arrays(contig, gdna_pos, sample_sets, assay_type, sample_query=None):
-
     if any(item in assay_type for item in ["gDNA", "probe"]):
         span_str = f"{contig}:{gdna_pos.min()}-{gdna_pos.max()}"
         snps = ag3.snp_calls(
             region=span_str, sample_sets=sample_sets, sample_query=sample_query
         )  # get genotypes
         ref_alt_arr = snps["variant_allele"].compute().values
         geno = snps["call_genotype"]
@@ -740,15 +738,14 @@
     res_dict,
     name,
     assay_type,
     sample_sets,
     target,
     out_dir=None,
 ):
-
     oligos, _ = _return_oligo_list(assay_type)
     if len(oligos) == 2:
         plt_title = ["Forward primer", "Reverse primer"]
     elif len(oligos) == 3:
         plt_title = ["Forward primer", "Reverse primer", "Probe"]
     elif len(oligos) == 1:
         plt_title = ["Probe"]
@@ -929,21 +926,21 @@
     )
     return (locgff, min_, max_, genegff)
 
 
 def _return_oligo_list(assay_type):
     if assay_type == "probe":
         oligos = ["probe"]
-        row_start = 5
+        row_start = 9
     elif any(item == assay_type for item in ["gDNA primers", "cDNA primers"]):
         oligos = ["forward", "reverse"]
-        row_start = 7
+        row_start = 11
     elif assay_type == "gDNA primers + probe":
         oligos = ["forward", "reverse", "probe"]
-        row_start = 8
+        row_start = 12
     return (oligos, row_start)
 
 
 def _convert_results_dict_naming(primer_dict):
     k = {}
     for key in primer_dict.keys():
         if "LEFT" in key:
```

### Comparing `agamprimer-0.6.0/AgamPrimer/agamPrimer.egg-info/PKG-INFO` & `agamprimer-0.6.1/AgamPrimer/agamPrimer.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `agamprimer-0.6.0/LICENSE` & `agamprimer-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agamprimer-0.6.0/pyproject.toml` & `agamprimer-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "AgamPrimer"
-version = "0.6.0"
+version = "0.6.1"
 description = "A package to design primers in Anopheles gambiae whilst considering genetic variation with malariagen_data"
 authors = [
     "Sanjay Nagi <sanjay.nagi@lstmed.ac.uk>",
     ]
 packages = [
     { include = "AgamPrimer" }
 ]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-primer3-py = "*"
+primer3-py = "2.0.0"
 malariagen_data = "*"
 openpyxl = "*"
 gget = "*"
 seaborn = "*"
 kaleido = "0.2.1"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `agamprimer-0.6.0/PKG-INFO` & `agamprimer-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agamprimer
-Version: 0.6.0
+Version: 0.6.1
 Summary: A package to design primers in Anopheles gambiae whilst considering genetic variation with malariagen_data
 License: MIT
 Author: Sanjay Nagi
 Author-email: sanjay.nagi@lstmed.ac.uk
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,9 +12,9 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gget
 Requires-Dist: kaleido (==0.2.1)
 Requires-Dist: malariagen_data
 Requires-Dist: openpyxl
-Requires-Dist: primer3-py
+Requires-Dist: primer3-py (==2.0.0)
 Requires-Dist: seaborn
```

