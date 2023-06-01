# Comparing `tmp/phc-ingestion-0.3.28.tar.gz` & `tmp/phc-ingestion-0.3.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.28.tar", last modified: Wed May 31 10:55:06 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.29.tar", last modified: Thu Jun  1 09:40:27 2023, max compression
```

## Comparing `phc-ingestion-0.3.28.tar` & `phc-ingestion-0.3.29.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0       16 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/PYPI.md
--rw-r--r--   0        0        0        0 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1603 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4737 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      879 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/caris/util/gene_to_coords.py
--rw-r--r--   0        0        0      555 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4636 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21500 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     5010 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3127 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8876 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     3187 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     2743 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/nextgen/process.py
--rw-r--r--   0        0        0     1672 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/nextgen/util/coords_to_genes.py
--rw-r--r--   0        0        0      297 2023-05-31 10:54:38.062541 phc-ingestion-0.3.28/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2018 2023-05-31 10:54:38.066542 phc-ingestion-0.3.28/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     6525 2023-05-31 10:54:38.066542 phc-ingestion-0.3.28/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     3577 2023-05-31 10:54:38.066542 phc-ingestion-0.3.28/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     5430 2023-05-31 10:54:38.066542 phc-ingestion-0.3.28/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-05-31 10:54:38.066542 phc-ingestion-0.3.28/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     1923 2023-05-31 10:54:38.066542 phc-ingestion-0.3.28/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-05-31 10:54:38.066542 phc-ingestion-0.3.28/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-05-31 10:54:38.066542 phc-ingestion-0.3.28/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0     1029 2023-05-31 10:54:38.066542 phc-ingestion-0.3.28/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.28/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/PYPI.md
+-rw-r--r--   0        0        0        0 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1603 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4636 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21500 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     5010 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3127 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8876 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     3187 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     2802 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2111 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     6525 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     3576 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     5430 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     1923 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0     1029 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.29/PKG-INFO
```

### Comparing `phc-ingestion-0.3.28/ingestion/caris/process.py` & `phc-ingestion-0.3.29/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.29/ingestion/caris/util/cnv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from logging import Logger
-from ingestion.caris.util.gene_to_coords import gene_to_coords
+from ingestion.shared_util.gene_to_coords import gene_to_coords
 
 
 def extract_cnv(prefix, data, ingest_status, log: Logger):
     # Get all CNV calls into a csv
     caris_lo_keywords = {"intermediate": "gain", "amplified": "amplification", "deleted": "loss"}
     if ingest_status["cnv_performed"]:
         tests = []
```

### Comparing `phc-ingestion-0.3.28/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.29/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.29/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/caris/util/gene_to_coords.py` & `phc-ingestion-0.3.29/ingestion/shared_util/gene_to_coords.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def gene_to_coords(reference_genome, gene):
     BASE_PATH = os.path.abspath(os.path.dirname(__file__))
 
     # Create reference dict where gene is key, list of chr, pos1, pos2 as value
     ref_dict = {}
-    with gzip.open(f"{BASE_PATH}/../../resources/{reference_genome}_map.csv.gz", "rt") as f:
+    with gzip.open(f"{BASE_PATH}/../resources/{reference_genome}_map.csv.gz", "rt") as f:
         for line in f.readlines()[1:]:
             working_line = line.split(",")
             ref_dict.update(
                 {working_line[3].strip(): [working_line[0], working_line[1], working_line[2]]}
             )
     try:
         chromosome = ref_dict.get(gene)[0]
```

### Comparing `phc-ingestion-0.3.28/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.29/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/caris/util/json.py` & `phc-ingestion-0.3.29/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.29/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.29/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.29/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.29/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/foundation/process.py` & `phc-ingestion-0.3.29/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.29/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.29/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.29/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.29/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/nextgen/process.py` & `phc-ingestion-0.3.29/ingestion/nextgen/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         "archiveFileId": source_file_id,
         "caseId": prefix,
         "ingestion_id": ingestion_id,
     }
     with scoped_logger(__name__, log_context) as log:
         cnv_path_name = process_cnv(
             pdf_in_file=vendor_files["pdfFile"],
+            cnv_in_file=vendor_files["somaticCnvTxtFile"],
             root_path=local_output_dir,
             prefix=prefix,
             log=log,
         )
         manifest = process_manifest(
             pdf_in_file=vendor_files["pdfFile"],
             source_file_id=source_file_id,
```

### Comparing `phc-ingestion-0.3.28/ingestion/nextgen/util/coords_to_genes.py` & `phc-ingestion-0.3.29/ingestion/shared_util/coords_to_genes.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 def coords_to_genes(reference_genome, chromosome, coordinate, log):
     BASE_PATH = os.path.abspath(os.path.dirname(__file__))
 
     # Create reference dict where gene is key, list of chr, pos1, pos2 as value
     ref_dict = {}
-    with gzip.open(f"{BASE_PATH}/../../resources/{reference_genome}_map.csv.gz", "rt") as f:
+    with gzip.open(f"{BASE_PATH}/../resources/{reference_genome}_map.csv.gz", "rt") as f:
         for line in f.readlines()[1:]:
             working_line = line.split(",")
             ref_dict.update(
                 {working_line[3].strip(): [working_line[0], working_line[1], working_line[2]]}
             )
 
     # Dictionary comprehension by chromosome
```

### Comparing `phc-ingestion-0.3.28/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.29/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.29/ingestion/nextgen/util/process_structural.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 from logging import Logger
 
-from ingestion.nextgen.util.coords_to_genes import coords_to_genes
+from ingestion.shared_util.coords_to_genes import coords_to_genes
 from ingestion.nextgen.util.variant_table import extract_variant_table
 from ingestion.nextgen.util.interpretation import map_interpretation
 
 
 def process_structural(sv_in_file: str, pdf_in_file, root_path: str, prefix: str, log: Logger):
     structural_variant_table = extract_variant_table(pdf=pdf_in_file, variant_type="structural")
```

### Comparing `phc-ingestion-0.3.28/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.29/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.3.29/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.29/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.29/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.28/pyproject.toml` & `phc-ingestion-0.3.29/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.28"
+version = "0.3.29"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

