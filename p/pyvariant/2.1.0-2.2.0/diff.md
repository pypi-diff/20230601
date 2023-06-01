# Comparing `tmp/pyvariant-2.1.0.tar.gz` & `tmp/pyvariant-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvariant-2.1.0.tar", last modified: Fri May 26 20:34:34 2023, max compression
+gzip compressed data, was "pyvariant-2.2.0.tar", last modified: Thu Jun  1 21:03:59 2023, max compression
```

## Comparing `pyvariant-2.1.0.tar` & `pyvariant-2.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-26 20:34:34.200603 pyvariant-2.1.0/
--rw-r--r--   0 mdouglas  (2185) users      (100)     1072 2023-05-16 21:59:33.000000 pyvariant-2.1.0/LICENSE
--rw-r--r--   0 mdouglas  (2185) users      (100)     8087 2023-05-26 20:34:34.203496 pyvariant-2.1.0/PKG-INFO
--rw-r--r--   0 mdouglas  (2185) users      (100)     6903 2023-05-16 21:59:33.000000 pyvariant-2.1.0/README.md
--rw-r--r--   0 mdouglas  (2185) users      (100)      342 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyproject.toml
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-26 20:34:33.931073 pyvariant-2.1.0/pyvariant/
--rw-r--r--   0 mdouglas  (2185) users      (100)      197 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/__init__.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     1995 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/cli.py
--rw-r--r--   0 mdouglas  (2185) users      (100)      956 2023-05-26 20:27:04.000000 pyvariant-2.1.0/pyvariant/constants.py
--rw-r--r--   0 mdouglas  (2185) users      (100)   141512 2023-05-26 20:27:04.000000 pyvariant-2.1.0/pyvariant/core.py
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-26 20:34:34.102744 pyvariant-2.1.0/pyvariant/data/
--rw-r--r--   0 mdouglas  (2185) users      (100)        4 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/data/empty.fa
--rw-r--r--   0 mdouglas  (2185) users      (100)       10 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/data/empty.fa.fai
--rw-r--r--   0 mdouglas  (2185) users      (100)    25066 2023-05-26 20:27:04.000000 pyvariant-2.1.0/pyvariant/ensembl_cache.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     7150 2023-05-26 20:27:04.000000 pyvariant-2.1.0/pyvariant/ensembl_release.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     4877 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/files.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     4051 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/parser.py
--rw-r--r--   0 mdouglas  (2185) users      (100)    32268 2023-05-26 20:27:04.000000 pyvariant-2.1.0/pyvariant/positions.py
--rw-r--r--   0 mdouglas  (2185) users      (100)    13398 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/regex.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     8450 2023-05-26 20:27:04.000000 pyvariant-2.1.0/pyvariant/sequence.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     1623 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/tables.py
--rw-r--r--   0 mdouglas  (2185) users      (100)    14143 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/utils.py
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-26 20:34:34.083579 pyvariant-2.1.0/pyvariant.egg-info/
--rw-r--r--   0 mdouglas  (2185) users      (100)     8087 2023-05-26 20:34:33.000000 pyvariant-2.1.0/pyvariant.egg-info/PKG-INFO
--rw-r--r--   0 mdouglas  (2185) users      (100)      803 2023-05-26 20:34:33.000000 pyvariant-2.1.0/pyvariant.egg-info/SOURCES.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)        1 2023-05-26 20:34:33.000000 pyvariant-2.1.0/pyvariant.egg-info/dependency_links.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)       49 2023-05-26 20:34:33.000000 pyvariant-2.1.0/pyvariant.egg-info/entry_points.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)      166 2023-05-26 20:34:33.000000 pyvariant-2.1.0/pyvariant.egg-info/requires.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)       10 2023-05-26 20:34:33.000000 pyvariant-2.1.0/pyvariant.egg-info/top_level.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)        1 2023-05-26 20:34:33.000000 pyvariant-2.1.0/pyvariant.egg-info/zip-safe
--rw-r--r--   0 mdouglas  (2185) users      (100)     1624 2023-05-26 20:34:34.210161 pyvariant-2.1.0/setup.cfg
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-26 20:34:34.191862 pyvariant-2.1.0/tests/
--rw-r--r--   0 mdouglas  (2185) users      (100)    70716 2023-05-26 20:27:05.000000 pyvariant-2.1.0/tests/test_core.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     9802 2023-05-26 20:27:05.000000 pyvariant-2.1.0/tests/test_core_map.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     6158 2023-05-26 20:27:05.000000 pyvariant-2.1.0/tests/test_ensembl_cache.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     1487 2023-05-26 20:27:05.000000 pyvariant-2.1.0/tests/test_ensembl_release.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     2025 2023-05-26 20:27:05.000000 pyvariant-2.1.0/tests/test_files.py
--rw-r--r--   0 mdouglas  (2185) users      (100)       88 2023-05-16 21:59:34.000000 pyvariant-2.1.0/tests/test_init.py
--rw-r--r--   0 mdouglas  (2185) users      (100)    37583 2023-05-16 21:59:34.000000 pyvariant-2.1.0/tests/test_parser.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     3400 2023-05-26 20:27:05.000000 pyvariant-2.1.0/tests/test_sequence.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     7262 2023-05-16 21:59:34.000000 pyvariant-2.1.0/tests/test_utils.py
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-01 21:03:59.238783 pyvariant-2.2.0/
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1072 2023-05-16 21:59:33.000000 pyvariant-2.2.0/LICENSE
+-rw-r--r--   0 mdouglas  (2185) users      (100)     8087 2023-06-01 21:03:59.241349 pyvariant-2.2.0/PKG-INFO
+-rw-r--r--   0 mdouglas  (2185) users      (100)     6903 2023-05-16 21:59:33.000000 pyvariant-2.2.0/README.md
+-rw-r--r--   0 mdouglas  (2185) users      (100)      342 2023-05-16 21:59:33.000000 pyvariant-2.2.0/pyproject.toml
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-01 21:03:59.071277 pyvariant-2.2.0/pyvariant/
+-rw-r--r--   0 mdouglas  (2185) users      (100)      829 2023-06-01 20:06:52.000000 pyvariant-2.2.0/pyvariant/__init__.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1995 2023-05-16 21:59:33.000000 pyvariant-2.2.0/pyvariant/cli.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)      956 2023-05-26 20:27:04.000000 pyvariant-2.2.0/pyvariant/constants.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)   143931 2023-06-01 20:06:42.000000 pyvariant-2.2.0/pyvariant/core.py
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-01 21:03:59.148769 pyvariant-2.2.0/pyvariant/data/
+-rw-r--r--   0 mdouglas  (2185) users      (100)        4 2023-05-16 21:59:33.000000 pyvariant-2.2.0/pyvariant/data/empty.fa
+-rw-r--r--   0 mdouglas  (2185) users      (100)       10 2023-05-16 21:59:33.000000 pyvariant-2.2.0/pyvariant/data/empty.fa.fai
+-rw-r--r--   0 mdouglas  (2185) users      (100)    25066 2023-05-26 20:27:04.000000 pyvariant-2.2.0/pyvariant/ensembl_cache.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     7149 2023-05-30 19:30:43.000000 pyvariant-2.2.0/pyvariant/ensembl_release.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     4877 2023-05-16 21:59:33.000000 pyvariant-2.2.0/pyvariant/files.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     4728 2023-05-29 20:48:35.000000 pyvariant-2.2.0/pyvariant/parser.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)    14837 2023-05-29 20:48:35.000000 pyvariant-2.2.0/pyvariant/regex.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     8450 2023-05-26 20:27:04.000000 pyvariant-2.2.0/pyvariant/sequence.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1623 2023-05-16 21:59:33.000000 pyvariant-2.2.0/pyvariant/tables.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)    14143 2023-05-16 21:59:33.000000 pyvariant-2.2.0/pyvariant/utils.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)    45586 2023-05-30 18:49:03.000000 pyvariant-2.2.0/pyvariant/variants.py
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-01 21:03:59.130250 pyvariant-2.2.0/pyvariant.egg-info/
+-rw-r--r--   0 mdouglas  (2185) users      (100)     8087 2023-06-01 21:03:58.000000 pyvariant-2.2.0/pyvariant.egg-info/PKG-INFO
+-rw-r--r--   0 mdouglas  (2185) users      (100)      802 2023-06-01 21:03:58.000000 pyvariant-2.2.0/pyvariant.egg-info/SOURCES.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)        1 2023-06-01 21:03:58.000000 pyvariant-2.2.0/pyvariant.egg-info/dependency_links.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)       49 2023-06-01 21:03:58.000000 pyvariant-2.2.0/pyvariant.egg-info/entry_points.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)      166 2023-06-01 21:03:58.000000 pyvariant-2.2.0/pyvariant.egg-info/requires.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)       10 2023-06-01 21:03:58.000000 pyvariant-2.2.0/pyvariant.egg-info/top_level.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)        1 2023-06-01 21:03:58.000000 pyvariant-2.2.0/pyvariant.egg-info/zip-safe
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1624 2023-06-01 21:03:59.247901 pyvariant-2.2.0/setup.cfg
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-01 21:03:59.231228 pyvariant-2.2.0/tests/
+-rw-r--r--   0 mdouglas  (2185) users      (100)    72420 2023-06-01 20:06:40.000000 pyvariant-2.2.0/tests/test_core.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     9802 2023-05-26 20:27:05.000000 pyvariant-2.2.0/tests/test_core_map.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     6158 2023-05-26 20:27:05.000000 pyvariant-2.2.0/tests/test_ensembl_cache.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1487 2023-05-26 20:27:05.000000 pyvariant-2.2.0/tests/test_ensembl_release.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     2025 2023-05-26 20:27:05.000000 pyvariant-2.2.0/tests/test_files.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)       88 2023-05-16 21:59:34.000000 pyvariant-2.2.0/tests/test_init.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)    39897 2023-05-29 20:48:35.000000 pyvariant-2.2.0/tests/test_parser.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     3400 2023-05-26 20:27:05.000000 pyvariant-2.2.0/tests/test_sequence.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     7262 2023-05-16 21:59:34.000000 pyvariant-2.2.0/tests/test_utils.py
```

### Comparing `pyvariant-2.1.0/LICENSE` & `pyvariant-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvariant-2.1.0/PKG-INFO` & `pyvariant-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvariant
-Version: 2.1.0
+Version: 2.2.0
 Summary: Map biological sequence variants (mutations) to their equivalent chromosome, cDNA, gene, exon, protein, and RNA positions.
 Home-page: https://github.com/mattdoug604/pyvariant.git
 Author: Matthew Douglas
 Author-email: mattdoug604@gmail.com
 Maintainer: Matthew Douglas
 Maintainer-email: mattdoug604@gmail.com
 License: MIT
```

### Comparing `pyvariant-2.1.0/README.md` & `pyvariant-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyvariant-2.1.0/pyvariant/cli.py` & `pyvariant-2.2.0/pyvariant/cli.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.1.0/pyvariant/constants.py` & `pyvariant-2.2.0/pyvariant/constants.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.1.0/pyvariant/core.py` & `pyvariant-2.2.0/pyvariant/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,29 @@
     STOP_CODON,
     SUBSTITUTION,
     TRANSCRIPT_ID,
     TRANSCRIPT_NAME,
 )
 from .files import tsv_to_dict, txt_to_list
 from .parser import parse
-from .positions import (
+from .sequence import PyfaidxFasta, get_sequence, mutate_sequence
+from .tables import AMINO_ACID_TABLE
+from .utils import (
+    calc_cdna_to_protein,
+    classify_seq_change,
+    collapse_seq_change,
+    expand_nt,
+    expand_pep,
+    is_insertion,
+    reverse_complement,
+    reverse_translate,
+    split_by_codon,
+    strip_version,
+)
+from .variants import (
     CdnaDeletion,
     CdnaDelins,
     CdnaDuplication,
     CdnaFusion,
     CdnaInsertion,
     CdnaPosition,
     CdnaSubstitution,
@@ -48,14 +62,15 @@
     DnaDuplication,
     DnaFusion,
     DnaInsertion,
     DnaPosition,
     DnaSubstitution,
     ExonFusion,
     ExonPosition,
+    ExonSmallVariant,
     ProteinDeletion,
     ProteinDelins,
     ProteinDuplication,
     ProteinFrameshift,
     ProteinFusion,
     ProteinInsertion,
     ProteinPosition,
@@ -72,28 +87,14 @@
     _ExonSmallVariant,
     _Fusion,
     _Position,
     _ProteinSmallVariant,
     _RnaSmallVariant,
     _SmallVariant,
 )
-from .sequence import PyfaidxFasta, get_sequence, mutate_sequence
-from .tables import AMINO_ACID_TABLE
-from .utils import (
-    calc_cdna_to_protein,
-    classify_seq_change,
-    collapse_seq_change,
-    expand_nt,
-    expand_pep,
-    is_insertion,
-    reverse_complement,
-    reverse_translate,
-    split_by_codon,
-    strip_version,
-)
 
 
 class Core:
     """Core class that handles converting between position types and retrieving information on
     biological features.
     """
 
@@ -1003,14 +1004,15 @@
     def _position_to_cdna(self, position, canonical: bool):
         return self._position_to(
             position,
             fusionf=self._position_to_cdna,
             fusiont=CdnaFusion,
             cdnavf=self._cdna_to_cdna_variant,
             dnavf=self._dna_to_cdna_variant,
+            exonvf=self._exon_to_cdna_variant,
             proteinvf=self._protein_to_cdna_variant,
             rnavf=self._rna_to_cdna_variant,
             cdnaf=self._cdna_to_cdna,
             dnaf=self._dna_to_cdna,
             exonf=self._exon_to_cdna,
             proteinf=self._protein_to_cdna,
             rnaf=self._rna_to_cdna,
@@ -1020,14 +1022,15 @@
     def _position_to_dna(self, position, canonical: bool):
         return self._position_to(
             position,
             fusionf=self._position_to_dna,
             fusiont=DnaFusion,
             cdnavf=self._cdna_to_dna_variant,
             dnavf=self._dna_to_dna_variant,
+            exonvf=self._exon_to_dna_variant,
             proteinvf=self._protein_to_dna_variant,
             rnavf=self._rna_to_dna_variant,
             cdnaf=self._cdna_to_dna,
             dnaf=self._dna_to_dna,
             exonf=self._exon_to_dna,
             proteinf=self._protein_to_dna,
             rnaf=self._rna_to_dna,
@@ -1037,14 +1040,15 @@
     def _position_to_exon(self, position, canonical: bool):
         return self._position_to(
             position,
             fusionf=self._position_to_exon,
             fusiont=ExonFusion,
             cdnavf=self._cdna_to_exon_variant,
             dnavf=self._dna_to_exon_variant,
+            exonvf=self._exon_to_exon_variant,
             proteinvf=self._protein_to_exon_variant,
             rnavf=self._rna_to_exon_variant,
             cdnaf=self._cdna_to_exon,
             dnaf=self._dna_to_exon,
             exonf=self._exon_to_exon,
             proteinf=self._protein_to_exon,
             rnaf=self._rna_to_exon,
@@ -1054,14 +1058,15 @@
     def _position_to_protein(self, position, canonical: bool):
         return self._position_to(
             position,
             fusionf=self._position_to_protein,
             fusiont=ProteinFusion,
             cdnavf=self._cdna_to_protein_variant,
             dnavf=self._dna_to_protein_variant,
+            exonvf=self._exon_to_protein_variant,
             proteinvf=self._protein_to_protein_variant,
             rnavf=self._rna_to_protein_variant,
             cdnaf=self._cdna_to_protein,
             dnaf=self._dna_to_protein,
             exonf=self._exon_to_protein,
             proteinf=self._protein_to_protein,
             rnaf=self._rna_to_protein,
@@ -1070,14 +1075,15 @@
 
     def _position_to_rna(self, position, canonical: bool):
         return self._position_to(
             position,
             fusionf=self._position_to_rna,
             fusiont=RnaFusion,
             cdnavf=self._cdna_to_rna_variant,
+            exonvf=self._exon_to_rna_variant,
             dnavf=self._dna_to_rna_variant,
             proteinvf=self._protein_to_rna_variant,
             rnavf=self._rna_to_rna_variant,
             cdnaf=self._cdna_to_rna,
             dnaf=self._dna_to_rna,
             exonf=self._exon_to_rna,
             proteinf=self._protein_to_rna,
@@ -1088,14 +1094,15 @@
     def _position_to(
         self,
         position,
         fusionf: Callable,
         fusiont: Type,
         cdnavf: Callable,
         dnavf: Callable,
+        exonvf: Callable,
         proteinvf: Callable,
         rnavf: Callable,
         cdnaf: Callable,
         dnaf: Callable,
         exonf: Callable,
         proteinf: Callable,
         rnaf: Callable,
@@ -1129,14 +1136,27 @@
                     position.end,
                     position.end_offset,
                     [position.strand],
                     position.refseq,
                     position.altseq,
                     canonical,
                 )
+            elif position.is_exon:
+                position = cast(_ExonSmallVariant, position)
+                return exonvf(
+                    [position.transcript_id],
+                    position.start,
+                    position.start_offset,
+                    position.end,
+                    position.end_offset,
+                    [position.strand],
+                    position.refseq,
+                    position.altseq,
+                    canonical,
+                )
             elif position.is_protein:
                 position = cast(_ProteinSmallVariant, position)
                 return proteinvf(
                     [position.transcript_id],
                     position.start,
                     position.start_offset,
                     position.end,
@@ -2099,14 +2119,28 @@
         result_start = convert(start, start_offset)
         if (start, start_offset) == (end, end_offset):
             return sorted(result_start)
         else:
             result_end = convert(end, end_offset)
             return join_positions(result_start, result_end, TRANSCRIPT_ID)
 
+    def _exon_to_cdna_variant(
+        self,
+        transcript_id: List[str],
+        start: int,
+        start_offset: int,
+        end: int,
+        end_offset: int,
+        strand: List[str],
+        refseq: str,
+        altseq: str,
+        canonical: bool = False,
+    ) -> List[_ExonSmallVariant]:
+        return []
+
     def _exon_to_dna(
         self,
         transcript_id: List[str],
         start: int,
         start_offset: int,
         end: int,
         end_offset: int,
@@ -2147,14 +2181,28 @@
         result_start = convert(start, start_offset)
         if (start, start_offset) == (end, end_offset):
             return sorted(result_start)
         else:
             result_end = convert(end, end_offset)
             return join_positions(result_start, result_end, CONTIG_ID)
 
+    def _exon_to_dna_variant(
+        self,
+        transcript_id: List[str],
+        start: int,
+        start_offset: int,
+        end: int,
+        end_offset: int,
+        strand: List[str],
+        refseq: str,
+        altseq: str,
+        canonical: bool = False,
+    ) -> List[_ExonSmallVariant]:
+        return []
+
     def _exon_to_exon(
         self,
         transcript_id: List[str],
         start: int,
         start_offset: int,
         end: int,
         end_offset: int,
@@ -2200,14 +2248,28 @@
         result_start = convert(start, start_offset)
         if (start, start_offset) == (end, end_offset):
             return sorted(result_start)
         else:
             result_end = convert(end, end_offset)
             return join_positions(result_start, result_end, TRANSCRIPT_ID)
 
+    def _exon_to_exon_variant(
+        self,
+        transcript_id: List[str],
+        start: int,
+        start_offset: int,
+        end: int,
+        end_offset: int,
+        strand: List[str],
+        refseq: str,
+        altseq: str,
+        canonical: bool = False,
+    ) -> List[_ExonSmallVariant]:
+        return []
+
     def _exon_to_protein(
         self,
         transcript_id: List[str],
         start: int,
         start_offset: int,
         end: int,
         end_offset: int,
@@ -2236,14 +2298,28 @@
                     [cdna.strand],
                     canonical=canonical,
                 )
             )
 
         return result
 
+    def _exon_to_protein_variant(
+        self,
+        transcript_id: List[str],
+        start: int,
+        start_offset: int,
+        end: int,
+        end_offset: int,
+        strand: List[str],
+        refseq: str,
+        altseq: str,
+        canonical: bool = False,
+    ) -> List[_ExonSmallVariant]:
+        return []
+
     def _exon_to_rna(
         self,
         transcript_id: List[str],
         start: int,
         start_offset: int,
         end: int,
         end_offset: int,
@@ -2288,14 +2364,28 @@
         result_start = convert(start, start_offset)
         if (start, start_offset) == (end, end_offset):
             return sorted(result_start)
         else:
             result_end = convert(end, end_offset)
             return join_positions(result_start, result_end, TRANSCRIPT_ID)
 
+    def _exon_to_rna_variant(
+        self,
+        transcript_id: List[str],
+        start: int,
+        start_offset: int,
+        end: int,
+        end_offset: int,
+        strand: List[str],
+        refseq: str,
+        altseq: str,
+        canonical: bool = False,
+    ) -> List[_ExonSmallVariant]:
+        return []
+
     def _protein_to_cdna(
         self,
         transcript_id: List[str],
         start: int,
         start_offset: int,
         end: int,
         end_offset: int,
@@ -3068,14 +3158,19 @@
             (CDNA, INSERTION): CdnaInsertion,
             (CDNA, SUBSTITUTION): CdnaSubstitution,
             (DNA, DELETION): DnaDeletion,
             (DNA, DELINS): DnaDelins,
             (DNA, DUPLICATION): DnaDuplication,
             (DNA, INSERTION): DnaInsertion,
             (DNA, SUBSTITUTION): DnaSubstitution,
+            (EXON, DELETION): ExonSmallVariant,
+            (EXON, DELINS): ExonSmallVariant,
+            (EXON, DUPLICATION): ExonSmallVariant,
+            (EXON, INSERTION): ExonSmallVariant,
+            (EXON, SUBSTITUTION): ExonSmallVariant,
             (PROTEIN, DELETION): ProteinDeletion,
             (PROTEIN, DELINS): ProteinDelins,
             (PROTEIN, DUPLICATION): ProteinDuplication,
             (PROTEIN, FRAMESHIFT): ProteinFrameshift,
             (PROTEIN, INSERTION): ProteinInsertion,
             (PROTEIN, SUBSTITUTION): ProteinSubstitution,
             (RNA, DELETION): RnaDeletion,
@@ -3168,17 +3263,14 @@
                     start_offset=start_offset,
                     end=end,
                     end_offset=end_offset,
                     refseq=new_ref,
                     altseq=new_alt,
                 )
                 variant_list.append(variant)
-            elif position.is_exon:
-                # TODO: Is there a way to map a small variant to an exon?
-                pass
             else:
                 raise ValueError(
                     f"Unrecognized variant type for {position.position_type}/{variant_type} ({new_ref}/{new_alt})"
                 )
 
         return variant_list
 
@@ -3558,15 +3650,14 @@
 
     def _uniquify_series(self, series: pd.Series) -> List:
         return sorted(series.dropna().unique().tolist())
 
     # ---------------------------------------------------------------------------------------------
     # Functions for getting feature aliases
     # ---------------------------------------------------------------------------------------------
-    @lru_cache
     def contig_alias(self, contig_id: str) -> List[str]:
         """List all aliases of the given contig ID.
 
         Args:
             contig_id (str): contig ID
 
         Returns:
@@ -3583,51 +3674,47 @@
         if not contig_id.startswith("chr"):
             contig_id_alt = "chr" + contig_id
             if contig_id_alt not in alias:
                 alias.append(contig_id_alt)
 
         return alias
 
-    @lru_cache
     def exon_alias(self, exon_id: str) -> List[str]:
         """List all aliases of the given exon ID.
 
         Args:
             exon_id (str): exon ID
 
         Returns:
             List[str]: All aliases of the given exon ID
         """
         return self._alias(exon_id, self._exon_alias)
 
-    @lru_cache
     def gene_alias(self, gene_id: str) -> List[str]:
         """List all aliases of the given gene ID.
 
         Args:
             gene_id (str): gene ID
 
         Returns:
             List[str]: All aliases of the given gene ID
         """
         return self._alias(gene_id, self._gene_alias)
 
-    @lru_cache
     def protein_alias(self, protein_id: str) -> List[str]:
         """List all aliases of the given protein ID.
 
         Args:
             protein_id (str): protein ID
 
         Returns:
             List[str]: All aliases of the given protein ID
         """
         return self._alias(protein_id, self._protein_alias)
 
-    @lru_cache
     def transcript_alias(self, transcript_id: str) -> List[str]:
         """List all aliases of the given transcript ID.
 
         Args:
             transcript_id (str): transcript ID
 
         Returns:
@@ -3807,15 +3894,14 @@
             bool: True if is an transcript else False
         """
         return any((i[1] in (TRANSCRIPT_ID, TRANSCRIPT_NAME) for i in self.normalize_id(feature)))
 
     # ---------------------------------------------------------------------------------------------
     # Functions for checking if a transcript is a canonical transcript
     # ---------------------------------------------------------------------------------------------
-    @lru_cache
     def is_canonical_transcript(self, transcript_id: str) -> bool:
         """Check if the given transcript ID is the canonical transcript for its gene.
 
         Args:
             transcript_id (str): transcript ID
 
         Returns:
```

### Comparing `pyvariant-2.1.0/pyvariant/ensembl_cache.py` & `pyvariant-2.2.0/pyvariant/ensembl_cache.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.1.0/pyvariant/ensembl_release.py` & `pyvariant-2.2.0/pyvariant/ensembl_release.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from __future__ import annotations
 
 from typing import Dict, List, Optional, Union, cast
 
 from .core import Core
 from .ensembl_cache import EnsemblCache
 from .files import tsv_to_dict, txt_to_list
-from .positions import CdnaPosition
 from .sequence import PyfaidxFasta
 from .utils import reverse_complement
+from .variants import CdnaPosition
 
 
 class EnsemblRelease(Core):
     """Handles converting between position types and retrieving information on biological features
     based on an Ensembl release.
     """
```

### Comparing `pyvariant-2.1.0/pyvariant/files.py` & `pyvariant-2.2.0/pyvariant/files.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.1.0/pyvariant/parser.py` & `pyvariant-2.2.0/pyvariant/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,14 +55,25 @@
         parsed["breakpoint1"]["variant_type"] = translate_suffix(parsed["breakpoint1"]["suffix"])
         parsed["breakpoint2"]["variant_type"] = MISSING
 
     # Normalize values in each breakpoint
     for breakpoint in parsed.values():
         breakpoint["position_type"] = translate_prefix(breakpoint["prefix"])
 
+        # TODO: Treats variants in the intron of a promoter as a single offset, e.g.
+        # 'NM_000546:c.-28-112G>A' -28 + -112 = -140. This allows the genomic position to be
+        # calculated correctly but the displayed string will be wrong (e.g. NM_000546:c.-140G>A)
+        if breakpoint["start_offset2"]:
+            breakpoint["start_offset"] = (breakpoint["start_offset"] or 0) + breakpoint[
+                "start_offset2"
+            ]
+
+        if breakpoint["end_offset2"]:
+            breakpoint["end_offset"] = (breakpoint["end_offset"] or 0) + breakpoint["end_offset2"]
+
         if breakpoint["start"] is None and breakpoint["start_offset"]:
             breakpoint["start"] = 1
 
         if breakpoint["end"] is None:
             breakpoint["end"] = breakpoint["start"]
             if breakpoint["end_offset"] is None:
                 breakpoint["end_offset"] = breakpoint["start_offset"]
@@ -80,16 +91,18 @@
 
         else:
             # Convert sequences to uppercase
             for key in ["refseq", "altseq"]:
                 if breakpoint[key]:
                     breakpoint[key] = breakpoint[key].upper()
 
-        # Drop 'refseq_end'
+        # Drop 'extra' values
+        breakpoint.pop("end_offset2", "")
         breakpoint.pop("refseq_end", "")
+        breakpoint.pop("start_offset2", "")
 
     return parsed
 
 
 def protein_letters_3to1(sequence: str) -> str:
     """Convert a sequence of 3-letter amino acids into 1-letter amino acids.
```

### Comparing `pyvariant-2.1.0/pyvariant/regex.py` & `pyvariant-2.2.0/pyvariant/regex.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 # -------------------------------------------------------------------------------------------------
 MISSING = None  # Default value for missing attributes
 MATCH_TYPES = {
     "feature": str,
     "prefix": str,
     "start": int,
     "start_offset": int,
+    "start_offset2": int,
     "start_seq": str,
     "end": int,
     "end_offset": int,
+    "end_offset2": int,
     "end_seq": str,
     "strand": str,
     "refseq": str,
     "altseq": str,
     "suffix": str,
     "suffix2": str,
 }
@@ -55,32 +57,35 @@
         rf"(?P<breakpoint1_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_start_seq>{SEQ})?"
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
         r"(?P<breakpoint1_suffix>delins)"
         rf"(?P<breakpoint1_altseq>{SEQ})"
     ),
     # Delins, multiple bases. Examples:
     # ENST00000078429:c.625_627delinsACC
     # BRCA2:p.K1025_K1026delinsN*
     re.compile(
         rf"(?P<breakpoint1_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_start_seq>{SEQ})?"
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
         r"_"
         rf"(?P<breakpoint1_end_seq>{SEQ})?"
         rf"(?P<breakpoint1_end>{POSITION})?"
         rf"(?P<breakpoint1_end_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_end_offset2>{OFFSET})?"
         r"(?P<breakpoint1_suffix>delins)"
         rf"(?P<breakpoint1_altseq>{SEQ})"
     ),
     # Deletion, single base. Examples:
     # ENST00000297679:c.45del
     # ENST00000297679:c.45del (not HGVS)
     # BRCA2:p.A1847del
@@ -88,14 +93,15 @@
         rf"(?P<breakpoint1_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_start_seq>{SEQ})?"
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
         r"(?P<breakpoint1_suffix>del)"
         rf"(?P<breakpoint1_refseq>{SEQ})?"
     ),
     # Deletion, multiple bases. Examples:
     # ENST00000297679:c.45_46del
     # ENST00000297679:c.45_46delAG (not HGVS)
     # BRCA1:e.7_8del
@@ -104,49 +110,54 @@
         rf"(?P<breakpoint1_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_start_seq>{SEQ})?"
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
         r"_"
         rf"(?P<breakpoint1_end_seq>{SEQ})?"
         rf"(?P<breakpoint1_end>{POSITION})?"
         rf"(?P<breakpoint1_end_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_end_offset2>{OFFSET})?"
         r"(?P<breakpoint1_suffix>del)"
         rf"(?P<breakpoint1_refseq>{SEQ})?"
     ),
     # Duplication, single base. Examples:
     # ENST00000217260:c.98dup
     re.compile(
         rf"(?P<breakpoint1_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_start_seq>{SEQ})?"
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
         r"(?P<breakpoint1_suffix>dup)"
         rf"(?P<breakpoint1_refseq>{SEQ})?"
     ),
     # Duplication, multiple bases. Examples:
     # ENST00000217260:c.98_99dup
     # EGFR:p.N771_H773dup
     re.compile(
         rf"(?P<breakpoint1_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_start_seq>{SEQ})?"
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
         r"_"
         rf"(?P<breakpoint1_end_seq>{SEQ})?"
         rf"(?P<breakpoint1_end>{POSITION})?"
         rf"(?P<breakpoint1_end_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_end_offset2>{OFFSET})?"
         r"(?P<breakpoint1_suffix>dup)"
         rf"(?P<breakpoint1_refseq>{SEQ})?"
     ),
     # Frameshift, single base. Examples:
     # BRCA1:p.E1013Nfs*4
     # BRCA1:p.E1013Nfs (not HGVS, missing new termination position)
     # NP_003997.2:p.Arg97fs (not HGVS, missing altseq)
@@ -154,14 +165,15 @@
         rf"(?P<breakpoint1_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_start_seq>{SEQ})?"
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
         rf"(?P<breakpoint1_altseq>{SEQ})?"
         r"(?P<breakpoint1_suffix>fs)"
         r"\*?"
         rf"({POSITION})?"  # TODO: Do something with new termination position?
     ),
     # Insertion. Examples:
     # chr13:g.32913032_32913033insTT
@@ -170,107 +182,120 @@
         rf"(?P<breakpoint1_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_start_seq>{SEQ})?"
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
         r"_"
         rf"(?P<breakpoint1_end_seq>{SEQ})?"
         rf"(?P<breakpoint1_end>{POSITION})?"
         rf"(?P<breakpoint1_end_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_end_offset2>{OFFSET})?"
         r"(?P<breakpoint1_suffix>ins)"
         rf"(?P<breakpoint1_altseq>{SEQ})?"
     ),
     # Nucleotide substitution. Examples:
     # ENST00000078429:r.916A>G
     # CEP72:c.1-2384C>T
     # TERT:c.-124C>T
+    # NM_000546:c.-28-112G>A
     re.compile(
         rf"(?P<breakpoint1_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
         rf"(?P<breakpoint1_refseq>{SEQ})"
         r"(?P<breakpoint1_suffix>>)"
         rf"(?P<breakpoint1_altseq>{SEQ})"
     ),
     # Protein substitution. Examples:
     # BRAF:p.R4621I
     re.compile(
         rf"(?P<breakpoint1_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_refseq>{SEQ})"
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
         rf"(?P<breakpoint1_altseq>{SEQ})"
     ),
     # Fusion. Examples:
     # NM_152263.2:r.-115_775::NM_002609.3:r.1580_*1924
     re.compile(
         rf"(?P<breakpoint1_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
         r"_?"
         rf"(?P<breakpoint1_end>{POSITION})?"
         rf"(?P<breakpoint1_end_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_end_offset2>{OFFSET})?"
         r"::"
         rf"(?P<breakpoint2_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint2_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint2_start>{POSITION})?"
         rf"(?P<breakpoint2_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint2_start_offset2>{OFFSET})?"
         r"_?"
         rf"(?P<breakpoint2_end>{POSITION})?"
         rf"(?P<breakpoint2_end_offset>{OFFSET})?"
+        rf"(?P<breakpoint2_end_offset2>{OFFSET})?"
     ),
     # Non-variant position, multiple bases. Examples:
     # 5:g.1282623_1282626
     re.compile(
         rf"(?P<breakpoint1_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
         r"_"
         rf"(?P<breakpoint1_end>{POSITION})?"
         rf"(?P<breakpoint1_end_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_end_offset2>{OFFSET})?"
     ),
     # Non-variant position, single base. Examples:
     # ENST00000078429:c.625
     re.compile(
         rf"(?P<breakpoint1_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
     ),
     # -------------------------------------------------------------------------------------------------
     # Non-HGVS string matching
     # -------------------------------------------------------------------------------------------------
     # Delins, single base. Examples:
     # BRAF:p.V600delVinsYM (not HGVS)
     re.compile(
         rf"(?P<breakpoint1_feature>{REFERENCE})"
         r":"
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_start_seq>{SEQ})?"
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
         r"(?P<breakpoint1_suffix>del)"
         rf"(?P<breakpoint1_refseq>{SEQ})"
         r"(?P<breakpoint1_suffix2>ins)"
         rf"(?P<breakpoint1_altseq>{SEQ})"
     ),
     # Fusion. Examples:
     # (chr8,chr8):fusion(g.128070272,g.127289817)
@@ -280,25 +305,29 @@
         r","
         rf"(?P<breakpoint2_feature>{REFERENCE})"
         r"\):fusion\("
         rf"(?P<breakpoint1_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint1_start>{POSITION})?"
         rf"(?P<breakpoint1_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_start_offset2>{OFFSET})?"
         r"_?"
         rf"(?P<breakpoint1_end>{POSITION})?"
         rf"(?P<breakpoint1_end_offset>{OFFSET})?"
+        rf"(?P<breakpoint1_end_offset2>{OFFSET})?"
         r","
         rf"(?P<breakpoint2_prefix>{PREFIX})"
         r"."
         rf"(?P<breakpoint2_start>{POSITION})?"
         rf"(?P<breakpoint2_start_offset>{OFFSET})?"
+        rf"(?P<breakpoint2_start_offset2>{OFFSET})?"
         r"_?"
         rf"(?P<breakpoint2_end>{POSITION})?"
         rf"(?P<breakpoint2_end_offset>{OFFSET})?"
+        rf"(?P<breakpoint2_end_offset2>{OFFSET})?"
         r"\)"
     ),
 ]
 
 
 # -------------------------------------------------------------------------------------------------
 # Regex matching logic
```

### Comparing `pyvariant-2.1.0/pyvariant/sequence.py` & `pyvariant-2.2.0/pyvariant/sequence.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.1.0/pyvariant/tables.py` & `pyvariant-2.2.0/pyvariant/tables.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.1.0/pyvariant/utils.py` & `pyvariant-2.2.0/pyvariant/utils.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.1.0/pyvariant.egg-info/PKG-INFO` & `pyvariant-2.2.0/pyvariant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvariant
-Version: 2.1.0
+Version: 2.2.0
 Summary: Map biological sequence variants (mutations) to their equivalent chromosome, cDNA, gene, exon, protein, and RNA positions.
 Home-page: https://github.com/mattdoug604/pyvariant.git
 Author: Matthew Douglas
 Author-email: mattdoug604@gmail.com
 Maintainer: Matthew Douglas
 Maintainer-email: mattdoug604@gmail.com
 License: MIT
```

### Comparing `pyvariant-2.1.0/pyvariant.egg-info/SOURCES.txt` & `pyvariant-2.2.0/pyvariant.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 pyvariant/cli.py
 pyvariant/constants.py
 pyvariant/core.py
 pyvariant/ensembl_cache.py
 pyvariant/ensembl_release.py
 pyvariant/files.py
 pyvariant/parser.py
-pyvariant/positions.py
 pyvariant/regex.py
 pyvariant/sequence.py
 pyvariant/tables.py
 pyvariant/utils.py
+pyvariant/variants.py
 pyvariant.egg-info/PKG-INFO
 pyvariant.egg-info/SOURCES.txt
 pyvariant.egg-info/dependency_links.txt
 pyvariant.egg-info/entry_points.txt
 pyvariant.egg-info/requires.txt
 pyvariant.egg-info/top_level.txt
 pyvariant.egg-info/zip-safe
```

### Comparing `pyvariant-2.1.0/setup.cfg` & `pyvariant-2.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyvariant
-version = 2.1.0
+version = 2.2.0
 description = Map biological sequence variants (mutations) to their equivalent chromosome, cDNA, gene, exon, protein, and RNA positions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mattdoug604/pyvariant.git
 author = Matthew Douglas
 author_email = mattdoug604@gmail.com
 maintainer = Matthew Douglas
@@ -32,15 +32,15 @@
 packages = find:
 python_requires = >=3.8
 include_package_data = True
 zip_safe = True
 install_requires = 
 	appdirs
 	BioPython>=1.73,<1.80
-	gtfparse==2.0.1
+	gtfparse<=2.0.1
 	packaging
 	pandas
 	polars<0.17.0
 	pyarrow
 	pyfaidx
 
 [options.package_data]
```

### Comparing `pyvariant-2.1.0/tests/test_core.py` & `pyvariant-2.2.0/tests/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,34 +20,35 @@
     GENE_ID,
     GENE_NAME,
     PROTEIN_ID,
     TRANSCRIPT_ID,
     TRANSCRIPT_NAME,
 )
 from pyvariant.core import Core
-from pyvariant.positions import (
+from pyvariant.sequence import PyfaidxFasta
+from pyvariant.variants import (
     CdnaDeletion,
     CdnaDelins,
     CdnaDuplication,
     CdnaPosition,
     CdnaSubstitution,
     DnaDelins,
     DnaInsertion,
     DnaPosition,
     DnaSubstitution,
     ExonFusion,
     ExonPosition,
+    ExonSmallVariant,
     ProteinFrameshift,
     ProteinPosition,
     ProteinSubstitution,
     RnaDelins,
     RnaPosition,
     RnaSubstitution,
 )
-from pyvariant.sequence import PyfaidxFasta
 
 
 # -------------------------------------------------------------------------------------------------
 # init
 # -------------------------------------------------------------------------------------------------
 def test_init():
     obj = Core(
@@ -1942,15 +1943,32 @@
                 start=54695570,
                 start_offset=0,
                 end=54695572,
                 end_offset=0,
                 strand="+",
             )
         ],
-        "exon": [],
+        "exon": [
+            ExonSmallVariant(
+                refseq="AAA",
+                altseq="GT",
+                _core=ensembl100,
+                contig_id="4",
+                start=2,
+                start_offset=0,
+                end=2,
+                end_offset=0,
+                strand="+",
+                gene_id="ENSG00000157404",
+                gene_name="KIT",
+                transcript_id="ENST00000288135",
+                transcript_name="KIT-201",
+                exon_id="ENSE00001032350",
+            )
+        ],
         "protein": [
             ProteinFrameshift(
                 refseq="K",
                 altseq="",
                 _core=ensembl100,
                 contig_id="4",
                 start=43,
@@ -2185,15 +2203,35 @@
                     end=114713909,
                     end_offset=0,
                     strand="-",
                 )
             ],
             [],
         ),
-        "exon": ([], []),
+        "exon": (
+            [
+                ExonSmallVariant(
+                    refseq="CAA",
+                    altseq="AAG",
+                    _core=ensembl100,
+                    contig_id="1",
+                    start=3,
+                    start_offset=0,
+                    end=3,
+                    end_offset=0,
+                    strand="-",
+                    gene_id="ENSG00000213281",
+                    gene_name="NRAS",
+                    transcript_id="ENST00000369535",
+                    transcript_name="NRAS-201",
+                    exon_id="ENSE00001751295",
+                )
+            ],
+            [],
+        ),
         "protein": ([], []),
         "rna": (
             [
                 RnaDelins(
                     refseq="CAA",
                     altseq="AAG",
                     _core=ensembl100,
@@ -2243,15 +2281,32 @@
                 start=114713909,
                 start_offset=0,
                 end=114713909,
                 end_offset=0,
                 strand="-",
             )
         ],
-        "exon": [],
+        "exon": [
+            ExonSmallVariant(
+                refseq="C",
+                altseq="A",
+                _core=ensembl100,
+                contig_id="1",
+                start=3,
+                start_offset=0,
+                end=3,
+                end_offset=0,
+                strand="-",
+                gene_id="ENSG00000213281",
+                gene_name="NRAS",
+                transcript_id="ENST00000369535",
+                transcript_name="NRAS-201",
+                exon_id="ENSE00001751295",
+            )
+        ],
         "protein": [
             ProteinSubstitution(
                 refseq="Q",
                 altseq="K",
                 _core=ensembl100,
                 contig_id="1",
                 start=61,
```

### Comparing `pyvariant-2.1.0/tests/test_core_map.py` & `pyvariant-2.2.0/tests/test_core_map.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.1.0/tests/test_ensembl_cache.py` & `pyvariant-2.2.0/tests/test_ensembl_cache.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.1.0/tests/test_ensembl_release.py` & `pyvariant-2.2.0/tests/test_ensembl_release.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.1.0/tests/test_files.py` & `pyvariant-2.2.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.1.0/tests/test_parser.py` & `pyvariant-2.2.0/tests/test_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,52 @@
                 "prefix": None,
                 "position_type": None,
                 "suffix": None,
                 "variant_type": None,
             },
         },
     ),
+    # cDNA/RNA deletion (multiple bases, promoter)
+    (
+        "NM_02412.1:r.-20_-18del",
+        {
+            "breakpoint1": {
+                "feature": "NM_02412.1",
+                "start": 1,
+                "start_offset": -20,
+                "start_seq": None,
+                "end": 1,
+                "end_offset": -18,
+                "end_seq": None,
+                "strand": None,
+                "refseq": None,
+                "altseq": None,
+                "prefix": "r",
+                "position_type": "rna",
+                "suffix": "del",
+                "variant_type": "deletion",
+            },
+            "breakpoint2": {
+                "feature": None,
+                "start": None,
+                "start_offset": None,
+                "start_seq": None,
+                "end": None,
+                "end_offset": None,
+                "end_seq": None,
+                "strand": None,
+                "refseq": None,
+                "altseq": None,
+                "prefix": None,
+                "position_type": None,
+                "suffix": None,
+                "variant_type": None,
+            },
+        },
+    ),
     # cDNA/RNA deletion-insertion
     (
         "LRG_2t1:c.775delinsga",
         {
             "breakpoint1": {
                 "feature": "LRG_2t1",
                 "start": 775,
@@ -327,14 +365,52 @@
                 "suffix": ">",
                 "variant_type": "substitution",
             },
             "breakpoint2": {
                 "feature": None,
                 "start": None,
                 "start_offset": None,
+                "start_seq": None,
+                "end": None,
+                "end_offset": None,
+                "end_seq": None,
+                "strand": None,
+                "refseq": None,
+                "altseq": None,
+                "prefix": None,
+                "position_type": None,
+                "suffix": None,
+                "variant_type": None,
+            },
+        },
+    ),
+    # cDNA/RNA substitution (promoter intron)
+    (
+        "NM_000546:c.-28-112G>A",
+        {
+            "breakpoint1": {
+                "feature": "NM_000546",
+                "start": 1,
+                "start_offset": -140,
+                "start_seq": None,
+                "end": 1,
+                "end_offset": -140,
+                "end_seq": None,
+                "strand": None,
+                "refseq": "G",
+                "altseq": "A",
+                "prefix": "c",
+                "position_type": "cdna",
+                "suffix": ">",
+                "variant_type": "substitution",
+            },
+            "breakpoint2": {
+                "feature": None,
+                "start": None,
+                "start_offset": None,
                 "start_seq": None,
                 "end": None,
                 "end_offset": None,
                 "end_seq": None,
                 "strand": None,
                 "refseq": None,
                 "altseq": None,
```

### Comparing `pyvariant-2.1.0/tests/test_sequence.py` & `pyvariant-2.2.0/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.1.0/tests/test_utils.py` & `pyvariant-2.2.0/tests/test_utils.py`

 * *Files identical despite different names*

