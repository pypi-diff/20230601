# Comparing `tmp/AlleleFinder-0.1.1.tar.gz` & `tmp/AlleleFinder-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adamkoziol/PycharmProjects/AlleleFinder/dist/tmpw68yl5cr/AlleleFinder-0.1.1.tar", last modified: Tue Apr  4 18:10:36 2023, max compression
+gzip compressed data, was "/home/adamkoziol/PycharmProjects/AlleleFinder/dist/tmpljkxth4p/AlleleFinder-0.1.2.tar", last modified: Thu Jun  1 18:10:45 2023, max compression
```

## Comparing `AlleleFinder-0.1.1.tar` & `AlleleFinder-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-04-04 18:10:36.000000 AlleleFinder-0.1.1/
--rwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)     1113 2023-02-24 20:49:53.000000 AlleleFinder-0.1.1/setup.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     1077 2023-03-10 15:09:59.000000 AlleleFinder-0.1.1/LICENSE
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      265 2023-04-04 18:10:36.000000 AlleleFinder-0.1.1/PKG-INFO
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-04-04 18:10:36.000000 AlleleFinder-0.1.1/AlleleFinder.egg-info/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      702 2023-04-04 18:10:36.000000 AlleleFinder-0.1.1/AlleleFinder.egg-info/SOURCES.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       19 2023-04-04 18:10:36.000000 AlleleFinder-0.1.1/AlleleFinder.egg-info/top_level.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      265 2023-04-04 18:10:36.000000 AlleleFinder-0.1.1/AlleleFinder.egg-info/PKG-INFO
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        1 2023-04-04 18:10:36.000000 AlleleFinder-0.1.1/AlleleFinder.egg-info/dependency_links.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     8402 2023-03-14 14:53:10.000000 AlleleFinder-0.1.1/README.md
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-04-04 18:10:36.000000 AlleleFinder-0.1.1/allele_tools/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    24429 2023-03-24 14:27:36.000000 AlleleFinder-0.1.1/allele_tools/allele_profiler.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    30190 2023-03-13 20:00:42.000000 AlleleFinder-0.1.1/allele_tools/stec.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2020-06-22 16:34:50.000000 AlleleFinder-0.1.1/allele_tools/__init__.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     6368 2023-03-13 14:59:24.000000 AlleleFinder-0.1.1/allele_tools/profile_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    85988 2023-03-24 18:37:56.000000 AlleleFinder-0.1.1/allele_tools/methods.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       51 2023-04-04 18:09:57.000000 AlleleFinder-0.1.1/allele_tools/version.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    28340 2023-03-24 18:52:09.000000 AlleleFinder-0.1.1/allele_tools/allele_updater.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    35343 2023-03-24 19:36:21.000000 AlleleFinder-0.1.1/allele_tools/allele_translate_reduce.py
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-04-04 18:10:36.000000 AlleleFinder-0.1.1/tests/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4599 2023-03-24 19:31:09.000000 AlleleFinder-0.1.1/tests/test_5_stec_allele_find.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     6584 2023-03-13 18:40:37.000000 AlleleFinder-0.1.1/tests/test_1_allele_translate_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4628 2023-03-13 20:02:00.000000 AlleleFinder-0.1.1/tests/test_3_stec_profile_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     1866 2023-03-24 19:31:09.000000 AlleleFinder-0.1.1/tests/test_6_stec_aa_allele_find.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2022-03-21 20:37:30.000000 AlleleFinder-0.1.1/tests/__init__.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     2829 2023-02-28 19:59:56.000000 AlleleFinder-0.1.1/tests/test_0_profile_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3245 2023-03-24 19:29:12.000000 AlleleFinder-0.1.1/tests/test_7_stec_allele_split.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     7795 2023-03-24 19:16:28.000000 AlleleFinder-0.1.1/tests/test_2_allele_updater.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3042 2023-03-13 19:11:01.000000 AlleleFinder-0.1.1/tests/test_4_stec_allele_translate_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       38 2023-04-04 18:10:36.000000 AlleleFinder-0.1.1/setup.cfg
+drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/
+-rwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)     1113 2023-02-24 20:49:53.000000 AlleleFinder-0.1.2/setup.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     1077 2023-03-10 15:09:59.000000 AlleleFinder-0.1.2/LICENSE
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      265 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/PKG-INFO
+drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/AlleleFinder.egg-info/
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      702 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/AlleleFinder.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       19 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/AlleleFinder.egg-info/top_level.txt
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      265 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/AlleleFinder.egg-info/PKG-INFO
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        1 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/AlleleFinder.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     8402 2023-06-01 18:07:22.000000 AlleleFinder-0.1.2/README.md
+drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/allele_tools/
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    24429 2023-03-24 14:27:36.000000 AlleleFinder-0.1.2/allele_tools/allele_profiler.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    30190 2023-06-01 15:06:39.000000 AlleleFinder-0.1.2/allele_tools/stec.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2020-06-22 16:34:50.000000 AlleleFinder-0.1.2/allele_tools/__init__.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     6368 2023-03-13 14:59:24.000000 AlleleFinder-0.1.2/allele_tools/profile_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    85988 2023-06-01 15:06:40.000000 AlleleFinder-0.1.2/allele_tools/methods.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       51 2023-06-01 18:07:22.000000 AlleleFinder-0.1.2/allele_tools/version.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    28340 2023-03-24 18:52:09.000000 AlleleFinder-0.1.2/allele_tools/allele_updater.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    35343 2023-03-24 19:36:21.000000 AlleleFinder-0.1.2/allele_tools/allele_translate_reduce.py
+drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/tests/
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4599 2023-06-01 15:06:40.000000 AlleleFinder-0.1.2/tests/test_5_stec_allele_find.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     6584 2023-06-01 15:06:40.000000 AlleleFinder-0.1.2/tests/test_1_allele_translate_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4628 2023-03-13 20:02:00.000000 AlleleFinder-0.1.2/tests/test_3_stec_profile_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     1866 2023-03-24 19:31:09.000000 AlleleFinder-0.1.2/tests/test_6_stec_aa_allele_find.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2022-03-21 20:37:30.000000 AlleleFinder-0.1.2/tests/__init__.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     2829 2023-02-28 19:59:56.000000 AlleleFinder-0.1.2/tests/test_0_profile_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3245 2023-03-24 19:29:12.000000 AlleleFinder-0.1.2/tests/test_7_stec_allele_split.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     7795 2023-06-01 15:06:39.000000 AlleleFinder-0.1.2/tests/test_2_allele_updater.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3042 2023-03-13 19:11:01.000000 AlleleFinder-0.1.2/tests/test_4_stec_allele_translate_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       38 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/setup.cfg
```

### Comparing `AlleleFinder-0.1.1/setup.py` & `AlleleFinder-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.1/LICENSE` & `AlleleFinder-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.1/AlleleFinder.egg-info/SOURCES.txt` & `AlleleFinder-0.1.2/AlleleFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.1/README.md` & `AlleleFinder-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 [`Conda`](https://docs.conda.io/en/latest/) is required to install AlleleFinder. See the [documentation](http://bioconda.github.io/) or [AlleleFinder installation](https://olc-bioinformatics.github.io/AlleleFinder/install/) for instructions of getting conda installed on your system
 
 
 Create a new conda environment:
 
 ```
-conda create -n allele_finder -c olcbioinformatics allelefinder=0.1.0=py_0
+conda create -n allele_finder -c olcbioinformatics allelefinder=0.1.2=py_0
 ```
 
 Additional documentation is available [here](https://olc-bioinformatics.github.io/AlleleFinder/installation)
 
 
 ## Reduce profiles
```

### Comparing `AlleleFinder-0.1.1/allele_tools/allele_profiler.py` & `AlleleFinder-0.1.2/allele_tools/allele_profiler.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.1/allele_tools/stec.py` & `AlleleFinder-0.1.2/allele_tools/stec.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
     if args.profile_file:
         log_str += f'. Parsing {args.profile_file} nucleotide profile to create corresponding,'\
                     ' reduced amino acid profile'
     logging.info(log_str)
     length_dict = {
         'ECs2973': 90,
         'ECs2974': 316,
-        'ECs1205': 320,
+        'ECs1205': 316,
         'ECs1206': 88
     }
     allele_translate_reduce = Translate(
         path=args.allele_path,
         profile=args.profile_file,
         report_path=args.report_path,
         translated_path=args.translated_path,
```

### Comparing `AlleleFinder-0.1.1/allele_tools/profile_reduce.py` & `AlleleFinder-0.1.2/allele_tools/profile_reduce.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.1/allele_tools/methods.py` & `AlleleFinder-0.1.2/allele_tools/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -568,15 +568,15 @@
     :return filtered: Boolean of whether the amino acid sequence passes length thresholds
     :return notes: Populated notes
     """
     # Dictionary of minimum acceptable lengths for each of the STEC genes
     length_dict = {
         'ECs2973': 90,
         'ECs2974': 316,
-        'ECs1205': 320,
+        'ECs1205': 316,
         'ECs1206': 88
     }
     filtered = False
     if not aa_seq.endswith('*'):
         notes.append(f'{gene} trimmed sequence did not end with a stop codon')
         if aa:
             filtered = True
```

### Comparing `AlleleFinder-0.1.1/allele_tools/allele_updater.py` & `AlleleFinder-0.1.2/allele_tools/allele_updater.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.1/allele_tools/allele_translate_reduce.py` & `AlleleFinder-0.1.2/allele_tools/allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.1/tests/test_5_stec_allele_find.py` & `AlleleFinder-0.1.2/tests/test_5_stec_allele_find.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             self.aa_report_file = os.path.join(self.aa_reports_path, 'aa_profiles.tsv')
             self.query_path = os.path.join(self.file_path, 'query')
             self.report_path = os.path.join(self.file_path, 'reports')
             self.report_file = os.path.join(self.report_path, 'profiles.tsv')
             self.length_dict = {
                 'ECs2973': 90,
                 'ECs2974': 316,
-                'ECs1205': 320,
+                'ECs1205': 316,
                 'ECs1206': 88
             }
             self.fake_path = os.path.join('~', 'completely_fake_path')
 
     return Variables()
```

### Comparing `AlleleFinder-0.1.1/tests/test_1_allele_translate_reduce.py` & `AlleleFinder-0.1.2/tests/test_1_allele_translate_reduce.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             self.nt_allele_path = os.path.join(self.file_path, 'nt_alleles')
             self.aa_allele_path = os.path.join(self.file_path, 'aa_alleles')
             self.aa_profile_path = os.path.join(self.file_path, 'aa_profile')
             self.aa_profile_file = os.path.join(self.aa_profile_path, 'profile.txt')
             self.length_dict = {
                 'ECs2973': 90,
                 'ECs2974': 316,
-                'ECs1205': 320,
+                'ECs1205': 316,
                 'ECs1206': 88
             }
             self.fake_path = os.path.join('~', 'completely_fake_path')
 
     return Variables()
```

### Comparing `AlleleFinder-0.1.1/tests/test_3_stec_profile_reduce.py` & `AlleleFinder-0.1.2/tests/test_3_stec_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.1/tests/test_6_stec_aa_allele_find.py` & `AlleleFinder-0.1.2/tests/test_6_stec_aa_allele_find.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.1/tests/test_0_profile_reduce.py` & `AlleleFinder-0.1.2/tests/test_0_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.1/tests/test_7_stec_allele_split.py` & `AlleleFinder-0.1.2/tests/test_7_stec_allele_split.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.1/tests/test_2_allele_updater.py` & `AlleleFinder-0.1.2/tests/test_2_allele_updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             self.report_path = os.path.join(self.file_path, 'reports')
             self.aa_report_file = os.path.join(self.report_path, 'aa_profiles.tsv')
 
             self.report_file = os.path.join(self.report_path, 'nt_profiles.tsv')
             self.length_dict = {
                 'ECs2973': 90,
                 'ECs2974': 316,
-                'ECs1205': 320,
+                'ECs1205': 316,
                 'ECs1206': 88
             }
             self.fake_path = os.path.join('~', 'completely_fake_path')
 
     return Variables()
```

### Comparing `AlleleFinder-0.1.1/tests/test_4_stec_allele_translate_reduce.py` & `AlleleFinder-0.1.2/tests/test_4_stec_allele_translate_reduce.py`

 * *Files identical despite different names*

