# Comparing `tmp/faps-2.7.3.tar.gz` & `tmp/faps-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faps-2.7.3.tar", last modified: Thu Nov 10 08:31:54 2022, max compression
+gzip compressed data, was "faps-2.7.4.tar", last modified: Thu Jun  1 10:56:37 2023, max compression
```

## Comparing `faps-2.7.3.tar` & `faps-2.7.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        0 2022-11-10 08:31:54.937972 faps-2.7.3/
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1070 2021-05-26 22:02:12.000000 faps-2.7.3/LICENSE
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      316 2022-11-10 08:31:54.937972 faps-2.7.3/PKG-INFO
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     6120 2022-10-19 11:56:09.000000 faps-2.7.3/README.md
-drwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        0 2022-11-10 08:31:54.937972 faps-2.7.3/faps/
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1457 2021-10-06 06:36:33.000000 faps-2.7.3/faps/__init__.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     5300 2021-05-26 22:02:12.000000 faps-2.7.3/faps/accuracy_paternity.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      925 2021-05-26 22:02:12.000000 faps-2.7.3/faps/alogsumexp.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1368 2021-05-26 22:02:12.000000 faps-2.7.3/faps/calculate_SNP_calls.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2169 2021-05-26 22:02:12.000000 faps-2.7.3/faps/calculate_geno_probs.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2017 2021-05-26 22:02:12.000000 faps-2.7.3/faps/convert_genotypes.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     7338 2021-09-10 11:43:43.000000 faps-2.7.3/faps/do_clustering.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     5074 2021-09-23 09:21:14.000000 faps-2.7.3/faps/draw_fathers.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1712 2021-05-26 22:02:12.000000 faps-2.7.3/faps/effective_nloci.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)    10578 2021-05-26 22:02:12.000000 faps-2.7.3/faps/export_to_colony.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)    16554 2022-10-19 12:07:56.000000 faps-2.7.3/faps/genotypeArray.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1281 2021-05-26 22:02:12.000000 faps-2.7.3/faps/incompatibilities.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     4599 2021-05-26 22:02:12.000000 faps-2.7.3/faps/lik_partition.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     3496 2021-05-26 22:02:12.000000 faps-2.7.3/faps/lik_sampled_fathers.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     3108 2021-05-26 22:02:12.000000 faps-2.7.3/faps/lik_unsampled_fathers.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     8557 2021-09-10 12:02:01.000000 faps-2.7.3/faps/make_generation.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     3922 2021-05-26 22:02:12.000000 faps-2.7.3/faps/make_offspring.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1893 2021-05-26 22:02:12.000000 faps-2.7.3/faps/make_parents.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)    20879 2021-05-26 22:02:12.000000 faps-2.7.3/faps/make_power.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2328 2021-05-26 22:02:12.000000 faps-2.7.3/faps/make_sibships.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     8377 2021-05-26 22:02:12.000000 faps-2.7.3/faps/mating_events.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     4256 2021-05-26 22:02:12.000000 faps-2.7.3/faps/mating_summary.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     3835 2021-05-26 22:02:12.000000 faps-2.7.3/faps/pairwise_lik_fullsibs.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      671 2021-05-26 22:02:12.000000 faps-2.7.3/faps/parent_index.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1880 2021-05-26 22:02:12.000000 faps-2.7.3/faps/partition_accuracy.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)    17789 2021-09-10 11:43:43.000000 faps-2.7.3/faps/paternityArray.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)    12149 2021-09-10 11:44:11.000000 faps-2.7.3/faps/paternity_array.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1487 2021-05-26 22:02:12.000000 faps-2.7.3/faps/paternity_list.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     4641 2021-09-24 04:59:08.000000 faps-2.7.3/faps/posterior_mating.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2865 2021-05-26 22:02:12.000000 faps-2.7.3/faps/pr_transition.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2716 2021-05-26 22:02:12.000000 faps-2.7.3/faps/pr_unsampled.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     3455 2021-05-26 22:02:12.000000 faps-2.7.3/faps/read_genotypes.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     3193 2021-05-26 22:02:12.000000 faps-2.7.3/faps/read_paternity_array.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      938 2021-05-26 22:02:12.000000 faps-2.7.3/faps/relation_matrix.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)    28162 2022-10-23 18:26:18.000000 faps-2.7.3/faps/sibshipCluster.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     4993 2021-09-10 11:43:43.000000 faps-2.7.3/faps/sibship_clustering.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2999 2021-05-26 22:02:12.000000 faps-2.7.3/faps/sibship_partitions.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     5919 2019-10-07 10:41:27.000000 faps-2.7.3/faps/sibship_paternity.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     5698 2018-07-04 08:28:43.000000 faps-2.7.3/faps/sibship_transitions.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      908 2021-05-26 22:02:12.000000 faps-2.7.3/faps/squash_siblings.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2187 2022-03-10 07:24:53.000000 faps-2.7.3/faps/summarise_paternity.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2873 2022-03-10 07:24:48.000000 faps-2.7.3/faps/summarise_sires.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     7139 2021-06-02 07:57:18.000000 faps-2.7.3/faps/transition_probability.py
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      429 2021-05-26 22:02:12.000000 faps-2.7.3/faps/unique_rows.py
-drwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        0 2022-11-10 08:31:54.937972 faps-2.7.3/faps.egg-info/
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      316 2022-11-10 08:31:54.000000 faps-2.7.3/faps.egg-info/PKG-INFO
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1272 2022-11-10 08:31:54.000000 faps-2.7.3/faps.egg-info/SOURCES.txt
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)        1 2022-11-10 08:31:54.000000 faps-2.7.3/faps.egg-info/dependency_links.txt
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)        1 2018-03-23 17:02:35.000000 faps-2.7.3/faps.egg-info/not-zip-safe
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)       36 2022-11-10 08:31:54.000000 faps-2.7.3/faps.egg-info/requires.txt
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)        5 2022-11-10 08:31:54.000000 faps-2.7.3/faps.egg-info/top_level.txt
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)       79 2022-11-10 08:31:54.941972 faps-2.7.3/setup.cfg
--rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      486 2022-10-27 12:44:59.000000 faps-2.7.3/setup.py
+drwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        0 2023-06-01 10:56:37.525455 faps-2.7.4/
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1070 2021-05-26 22:02:12.000000 faps-2.7.4/LICENSE
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      316 2023-06-01 10:56:37.525455 faps-2.7.4/PKG-INFO
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     6120 2022-10-19 11:56:09.000000 faps-2.7.4/README.md
+drwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        0 2023-06-01 10:56:37.525455 faps-2.7.4/faps/
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1457 2021-10-06 06:36:33.000000 faps-2.7.4/faps/__init__.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     5300 2021-05-26 22:02:12.000000 faps-2.7.4/faps/accuracy_paternity.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      925 2021-05-26 22:02:12.000000 faps-2.7.4/faps/alogsumexp.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1368 2021-05-26 22:02:12.000000 faps-2.7.4/faps/calculate_SNP_calls.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2169 2021-05-26 22:02:12.000000 faps-2.7.4/faps/calculate_geno_probs.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2017 2021-05-26 22:02:12.000000 faps-2.7.4/faps/convert_genotypes.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     7338 2021-09-10 11:43:43.000000 faps-2.7.4/faps/do_clustering.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     5074 2021-09-23 09:21:14.000000 faps-2.7.4/faps/draw_fathers.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1712 2021-05-26 22:02:12.000000 faps-2.7.4/faps/effective_nloci.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)    10578 2021-05-26 22:02:12.000000 faps-2.7.4/faps/export_to_colony.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)    16554 2022-10-19 12:07:56.000000 faps-2.7.4/faps/genotypeArray.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1281 2021-05-26 22:02:12.000000 faps-2.7.4/faps/incompatibilities.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     4599 2021-05-26 22:02:12.000000 faps-2.7.4/faps/lik_partition.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     3496 2021-05-26 22:02:12.000000 faps-2.7.4/faps/lik_sampled_fathers.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     3108 2021-05-26 22:02:12.000000 faps-2.7.4/faps/lik_unsampled_fathers.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     8557 2021-09-10 12:02:01.000000 faps-2.7.4/faps/make_generation.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     3922 2021-05-26 22:02:12.000000 faps-2.7.4/faps/make_offspring.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1893 2021-05-26 22:02:12.000000 faps-2.7.4/faps/make_parents.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)    20879 2021-05-26 22:02:12.000000 faps-2.7.4/faps/make_power.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2328 2021-05-26 22:02:12.000000 faps-2.7.4/faps/make_sibships.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     8377 2021-05-26 22:02:12.000000 faps-2.7.4/faps/mating_events.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     4256 2021-05-26 22:02:12.000000 faps-2.7.4/faps/mating_summary.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     3835 2021-05-26 22:02:12.000000 faps-2.7.4/faps/pairwise_lik_fullsibs.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      671 2021-05-26 22:02:12.000000 faps-2.7.4/faps/parent_index.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1880 2021-05-26 22:02:12.000000 faps-2.7.4/faps/partition_accuracy.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)    17789 2021-09-10 11:43:43.000000 faps-2.7.4/faps/paternityArray.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)    12221 2023-05-30 06:38:41.000000 faps-2.7.4/faps/paternity_array.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1487 2021-05-26 22:02:12.000000 faps-2.7.4/faps/paternity_list.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     4641 2021-09-24 04:59:08.000000 faps-2.7.4/faps/posterior_mating.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2865 2021-05-26 22:02:12.000000 faps-2.7.4/faps/pr_transition.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2716 2021-05-26 22:02:12.000000 faps-2.7.4/faps/pr_unsampled.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     3455 2021-05-26 22:02:12.000000 faps-2.7.4/faps/read_genotypes.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     3193 2021-05-26 22:02:12.000000 faps-2.7.4/faps/read_paternity_array.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      938 2021-05-26 22:02:12.000000 faps-2.7.4/faps/relation_matrix.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)    28162 2022-10-23 18:26:18.000000 faps-2.7.4/faps/sibshipCluster.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     4993 2021-09-10 11:43:43.000000 faps-2.7.4/faps/sibship_clustering.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2999 2021-05-26 22:02:12.000000 faps-2.7.4/faps/sibship_partitions.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     5919 2019-10-07 10:41:27.000000 faps-2.7.4/faps/sibship_paternity.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     5698 2018-07-04 08:28:43.000000 faps-2.7.4/faps/sibship_transitions.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      908 2021-05-26 22:02:12.000000 faps-2.7.4/faps/squash_siblings.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2187 2022-03-10 07:24:53.000000 faps-2.7.4/faps/summarise_paternity.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     2873 2022-03-10 07:24:48.000000 faps-2.7.4/faps/summarise_sires.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     7143 2023-06-01 10:21:07.000000 faps-2.7.4/faps/transition_probability.py
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      429 2021-05-26 22:02:12.000000 faps-2.7.4/faps/unique_rows.py
+drwxr-xr-x   0 thomas.ellis  (1000) tellis    (1000)        0 2023-06-01 10:56:37.525455 faps-2.7.4/faps.egg-info/
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      316 2023-06-01 10:56:36.000000 faps-2.7.4/faps.egg-info/PKG-INFO
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)     1272 2023-06-01 10:56:37.000000 faps-2.7.4/faps.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)        1 2023-06-01 10:56:36.000000 faps-2.7.4/faps.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)        1 2018-03-23 17:02:35.000000 faps-2.7.4/faps.egg-info/not-zip-safe
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)       36 2023-06-01 10:56:37.000000 faps-2.7.4/faps.egg-info/requires.txt
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)        5 2023-06-01 10:56:37.000000 faps-2.7.4/faps.egg-info/top_level.txt
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)       79 2023-06-01 10:56:37.525455 faps-2.7.4/setup.cfg
+-rw-r--r--   0 thomas.ellis  (1000) tellis    (1000)      486 2023-06-01 10:48:26.000000 faps-2.7.4/setup.py
```

### Comparing `faps-2.7.3/LICENSE` & `faps-2.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/README.md` & `faps-2.7.4/README.md`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/__init__.py` & `faps-2.7.4/faps/__init__.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/accuracy_paternity.py` & `faps-2.7.4/faps/accuracy_paternity.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/alogsumexp.py` & `faps-2.7.4/faps/alogsumexp.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/calculate_SNP_calls.py` & `faps-2.7.4/faps/calculate_SNP_calls.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/calculate_geno_probs.py` & `faps-2.7.4/faps/calculate_geno_probs.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/convert_genotypes.py` & `faps-2.7.4/faps/convert_genotypes.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/do_clustering.py` & `faps-2.7.4/faps/do_clustering.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/draw_fathers.py` & `faps-2.7.4/faps/draw_fathers.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/effective_nloci.py` & `faps-2.7.4/faps/effective_nloci.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/export_to_colony.py` & `faps-2.7.4/faps/export_to_colony.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/genotypeArray.py` & `faps-2.7.4/faps/genotypeArray.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/incompatibilities.py` & `faps-2.7.4/faps/incompatibilities.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/lik_partition.py` & `faps-2.7.4/faps/lik_partition.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/lik_sampled_fathers.py` & `faps-2.7.4/faps/lik_sampled_fathers.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/lik_unsampled_fathers.py` & `faps-2.7.4/faps/lik_unsampled_fathers.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/make_generation.py` & `faps-2.7.4/faps/make_generation.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/make_offspring.py` & `faps-2.7.4/faps/make_offspring.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/make_parents.py` & `faps-2.7.4/faps/make_parents.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/make_power.py` & `faps-2.7.4/faps/make_power.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/make_sibships.py` & `faps-2.7.4/faps/make_sibships.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/mating_events.py` & `faps-2.7.4/faps/mating_events.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/mating_summary.py` & `faps-2.7.4/faps/mating_summary.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/pairwise_lik_fullsibs.py` & `faps-2.7.4/faps/pairwise_lik_fullsibs.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/parent_index.py` & `faps-2.7.4/faps/parent_index.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/partition_accuracy.py` & `faps-2.7.4/faps/partition_accuracy.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/paternityArray.py` & `faps-2.7.4/faps/paternityArray.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/paternity_array.py` & `faps-2.7.4/faps/paternity_array.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from faps.paternityArray import paternityArray
 from faps.genotypeArray import genotypeArray
 from faps.transition_probability import transition_probability
 from faps.incompatibilities import incompatibilities
 from warnings import warn
 
-def paternity_array(offspring, mothers, males, mu=1e-12, missing_parents = 0, purge=None, selfing_rate=None, max_clashes=None, covariate=None, integration="full"):
+def paternity_array(offspring, mothers, males, mu=1e-12, missing_parents = 0.5, purge=None, selfing_rate=None, max_clashes=None, covariate=None, integration="full"):
     """
     Construct a paternityArray object for the offspring given known mothers
     and a set of candidate fathers using genotype data. Currently only SNP
     data is supported.
 
     Additional information about paternity from non-genetic sources can be
     provided through the argument `covariate`. For example, this might be a
@@ -31,15 +31,16 @@
         Point estimate of the genotyping error rate. Clustering is unstable if
         mu_input is set to exactly zero. Any zero values will therefore be set
         to a very small number close to zero (1e-12). Defaults to 1e-12
     missing_parents : float between zero and one
         Input value for the proportion of adults who are missing from the sample.
         This is used to weight the probabilties of paternity for each father
         relative to the probability that a father was not sampled. Defaults to
-        zero, but you should definitely change this.
+        0.5, which effectively places no prior weight either way, and means
+        information comes from the likelihood.
     purge: vector of str, or float between zero and one, optional
         Individuals who can be removed from the paternity array a priori. If
         a float is given, that proportion of individuals is removed from the
         array at random. Alternatively a string or vector of strings containing
         names of specific candidate fathers can be supplied.
     selfing_rate: float between zero and one, optional
         Input value for the prior probability of self-fertilisation.
```

### Comparing `faps-2.7.3/faps/paternity_list.py` & `faps-2.7.4/faps/paternity_list.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/posterior_mating.py` & `faps-2.7.4/faps/posterior_mating.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/pr_transition.py` & `faps-2.7.4/faps/pr_transition.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/pr_unsampled.py` & `faps-2.7.4/faps/pr_unsampled.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/read_genotypes.py` & `faps-2.7.4/faps/read_genotypes.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/read_paternity_array.py` & `faps-2.7.4/faps/read_paternity_array.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/relation_matrix.py` & `faps-2.7.4/faps/relation_matrix.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/sibshipCluster.py` & `faps-2.7.4/faps/sibshipCluster.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/sibship_clustering.py` & `faps-2.7.4/faps/sibship_clustering.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/sibship_partitions.py` & `faps-2.7.4/faps/sibship_partitions.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/sibship_paternity.py` & `faps-2.7.4/faps/sibship_paternity.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/sibship_transitions.py` & `faps-2.7.4/faps/sibship_transitions.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/squash_siblings.py` & `faps-2.7.4/faps/squash_siblings.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/summarise_paternity.py` & `faps-2.7.4/faps/summarise_paternity.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/summarise_sires.py` & `faps-2.7.4/faps/summarise_sires.py`

 * *Files identical despite different names*

### Comparing `faps-2.7.3/faps/transition_probability.py` & `faps-2.7.4/faps/transition_probability.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     # Implementation integrating over all possible genotypes.
     # Added June 2020 from version 2.5 onwards
     if integration == "full":
         # Array of probabilities of drawing paternal allele if the dad is 0,1,2
         allele_freqs = males.allele_freqs()
         af = np.array([
             (1-allele_freqs)**2,
-            allele_freqs * (1-allele_freqs),
+            2 * allele_freqs * (1-allele_freqs),
             allele_freqs ** 2
         ])
 
         # Empty arrays to store probabilities of paternity, and of missing dads
         lik_array = np.zeros([offspring.size, males.size, offspring.nloci])
         lik_absent = np.zeros([offspring.size, offspring.nloci])
```

### Comparing `faps-2.7.3/faps.egg-info/SOURCES.txt` & `faps-2.7.4/faps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

