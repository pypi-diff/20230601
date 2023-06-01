# Comparing `tmp/mhcgnomes-1.8.4.tar.gz` & `tmp/mhcgnomes-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mhcgnomes-1.8.4.tar", last modified: Thu Jun  2 18:09:26 2022, max compression
+gzip compressed data, was "mhcgnomes-1.8.6.tar", last modified: Thu Jun  1 20:17:21 2023, max compression
```

## Comparing `mhcgnomes-1.8.4.tar` & `mhcgnomes-1.8.6.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2022-06-02 18:09:26.736012 mhcgnomes-1.8.4/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)       26 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/MANIFEST.in
--rw-r--r--   0 iskander   (501) staff       (20)     8142 2022-06-02 18:09:26.735865 mhcgnomes-1.8.4/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     7430 2022-04-26 17:58:23.000000 mhcgnomes-1.8.4/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2022-06-02 18:09:26.720912 mhcgnomes-1.8.4/mhcgnomes/
--rw-r--r--   0 iskander   (501) staff       (20)     1527 2022-04-21 04:07:52.000000 mhcgnomes-1.8.4/mhcgnomes/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     9166 2022-04-21 04:12:12.000000 mhcgnomes-1.8.4/mhcgnomes/allele.py
--rw-r--r--   0 iskander   (501) staff       (20)     3411 2022-04-11 22:05:54.000000 mhcgnomes-1.8.4/mhcgnomes/allele_annotations.py
--rw-r--r--   0 iskander   (501) staff       (20)     2134 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/allele_without_gene.py
--rw-r--r--   0 iskander   (501) staff       (20)     3655 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/class2_locus.py
--rw-r--r--   0 iskander   (501) staff       (20)     2965 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/common.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2022-06-02 18:09:26.722324 mhcgnomes-1.8.4/mhcgnomes/data/
--rw-r--r--   0 iskander   (501) staff       (20)    91628 2022-04-13 03:59:42.000000 mhcgnomes-1.8.4/mhcgnomes/data/allele_aliases.yaml
--rw-r--r--   0 iskander   (501) staff       (20)        0 2022-04-20 18:44:13.000000 mhcgnomes-1.8.4/mhcgnomes/data/common_genes.yaml
--rw-r--r--   0 iskander   (501) staff       (20)    12979 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/data/curated_allele_aliases.yaml
--rw-r--r--   0 iskander   (501) staff       (20)       12 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/data/default_alleles.yaml
--rw-r--r--   0 iskander   (501) staff       (20)     1315 2022-05-03 21:09:58.000000 mhcgnomes-1.8.4/mhcgnomes/data/gene_aliases.yaml
--rw-r--r--   0 iskander   (501) staff       (20)     5582 2022-04-21 04:02:13.000000 mhcgnomes-1.8.4/mhcgnomes/data/haplotypes.yaml
--rw-r--r--   0 iskander   (501) staff       (20)      480 2022-05-04 03:22:54.000000 mhcgnomes-1.8.4/mhcgnomes/data/known_alleles.yaml
--rw-r--r--   0 iskander   (501) staff       (20)    10648 2022-04-21 03:48:54.000000 mhcgnomes-1.8.4/mhcgnomes/data/serotypes.yaml
--rw-r--r--   0 iskander   (501) staff       (20)    31104 2022-04-21 03:59:53.000000 mhcgnomes-1.8.4/mhcgnomes/data/species.yaml
--rw-r--r--   0 iskander   (501) staff       (20)     2469 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/data.py
--rw-r--r--   0 iskander   (501) staff       (20)      995 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/dataframe.py
--rw-r--r--   0 iskander   (501) staff       (20)      761 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/errors.py
--rw-r--r--   0 iskander   (501) staff       (20)     4128 2022-05-04 21:48:00.000000 mhcgnomes-1.8.4/mhcgnomes/function_api.py
--rw-r--r--   0 iskander   (501) staff       (20)     4792 2022-04-21 04:12:12.000000 mhcgnomes-1.8.4/mhcgnomes/gene.py
--rw-r--r--   0 iskander   (501) staff       (20)     6156 2022-04-21 04:10:50.000000 mhcgnomes-1.8.4/mhcgnomes/haplotype.py
--rw-r--r--   0 iskander   (501) staff       (20)     3049 2022-04-20 20:23:15.000000 mhcgnomes-1.8.4/mhcgnomes/mhc_class.py
--rw-r--r--   0 iskander   (501) staff       (20)     2659 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/mhc_class_helpers.py
--rw-r--r--   0 iskander   (501) staff       (20)     1943 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/mutation.py
--rw-r--r--   0 iskander   (501) staff       (20)     7567 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/normalizing_dictionary.py
--rw-r--r--   0 iskander   (501) staff       (20)     1932 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/normalizing_set.py
--rw-r--r--   0 iskander   (501) staff       (20)     6840 2022-04-22 21:13:26.000000 mhcgnomes-1.8.4/mhcgnomes/pair.py
--rw-r--r--   0 iskander   (501) staff       (20)    63897 2022-05-09 22:19:26.000000 mhcgnomes-1.8.4/mhcgnomes/parser.py
--rw-r--r--   0 iskander   (501) staff       (20)     4716 2022-04-11 17:49:00.000000 mhcgnomes-1.8.4/mhcgnomes/parsing_helpers.py
--rw-r--r--   0 iskander   (501) staff       (20)     7482 2022-04-21 04:12:12.000000 mhcgnomes-1.8.4/mhcgnomes/result.py
--rw-r--r--   0 iskander   (501) staff       (20)     5282 2022-04-21 04:07:52.000000 mhcgnomes-1.8.4/mhcgnomes/result_sorting.py
--rw-r--r--   0 iskander   (501) staff       (20)     1521 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/result_with_gene.py
--rw-r--r--   0 iskander   (501) staff       (20)     1258 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/result_with_mhc_class.py
--rw-r--r--   0 iskander   (501) staff       (20)     5355 2022-04-21 04:12:12.000000 mhcgnomes-1.8.4/mhcgnomes/result_with_multiple_alleles.py
--rw-r--r--   0 iskander   (501) staff       (20)     1910 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/result_with_species.py
--rw-r--r--   0 iskander   (501) staff       (20)     1944 2022-04-21 04:09:33.000000 mhcgnomes-1.8.4/mhcgnomes/serotype.py
--rw-r--r--   0 iskander   (501) staff       (20)    25633 2022-04-21 03:58:32.000000 mhcgnomes-1.8.4/mhcgnomes/species.py
--rw-r--r--   0 iskander   (501) staff       (20)     3300 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/standard_format.py
--rw-r--r--   0 iskander   (501) staff       (20)     2671 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/token.py
--rw-r--r--   0 iskander   (501) staff       (20)      695 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/mhcgnomes/token_canonical_sequences.py
--rw-r--r--   0 iskander   (501) staff       (20)     4019 2022-04-18 18:57:25.000000 mhcgnomes-1.8.4/mhcgnomes/token_substitution.py
--rw-r--r--   0 iskander   (501) staff       (20)     3799 2022-05-09 21:06:51.000000 mhcgnomes-1.8.4/mhcgnomes/tokenize.py
--rw-r--r--   0 iskander   (501) staff       (20)       22 2022-05-04 21:49:52.000000 mhcgnomes-1.8.4/mhcgnomes/version.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2022-06-02 18:09:26.721398 mhcgnomes-1.8.4/mhcgnomes.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     8142 2022-06-02 18:09:26.000000 mhcgnomes-1.8.4/mhcgnomes.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     2272 2022-06-02 18:09:26.000000 mhcgnomes-1.8.4/mhcgnomes.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2022-06-02 18:09:26.000000 mhcgnomes-1.8.4/mhcgnomes.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2022-06-02 18:09:26.000000 mhcgnomes-1.8.4/mhcgnomes.egg-info/requires.txt
--rw-r--r--   0 iskander   (501) staff       (20)       10 2022-06-02 18:09:26.000000 mhcgnomes-1.8.4/mhcgnomes.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2022-06-02 18:09:26.736065 mhcgnomes-1.8.4/setup.cfg
--rw-r--r--   0 iskander   (501) staff       (20)     2193 2022-04-05 23:02:22.000000 mhcgnomes-1.8.4/setup.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2022-06-02 18:09:26.735682 mhcgnomes-1.8.4/test/
--rw-r--r--   0 iskander   (501) staff       (20)      476 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_Bofr.py
--rw-r--r--   0 iskander   (501) staff       (20)     4776 2022-04-21 04:12:12.000000 mhcgnomes-1.8.4/test/test_allele.py
--rw-r--r--   0 iskander   (501) staff       (20)      342 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_allele_aliases.py
--rw-r--r--   0 iskander   (501) staff       (20)     1923 2022-04-11 22:10:02.000000 mhcgnomes-1.8.4/test/test_annotations.py
--rw-r--r--   0 iskander   (501) staff       (20)      940 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_bad_inputs.py
--rw-r--r--   0 iskander   (501) staff       (20)      155 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_cat.py
--rw-r--r--   0 iskander   (501) staff       (20)      307 2022-04-22 21:17:58.000000 mhcgnomes-1.8.4/test/test_cd1.py
--rw-r--r--   0 iskander   (501) staff       (20)     1572 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_chicken.py
--rw-r--r--   0 iskander   (501) staff       (20)      276 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_class2_locus.py
--rw-r--r--   0 iskander   (501) staff       (20)      801 2022-04-21 04:12:12.000000 mhcgnomes-1.8.4/test/test_class2_pair.py
--rw-r--r--   0 iskander   (501) staff       (20)      967 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_cow.py
--rw-r--r--   0 iskander   (501) staff       (20)     1912 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_dog.py
--rw-r--r--   0 iskander   (501) staff       (20)     1716 2022-04-22 21:07:22.000000 mhcgnomes-1.8.4/test/test_fish.py
--rw-r--r--   0 iskander   (501) staff       (20)      781 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_haplotype.py
--rw-r--r--   0 iskander   (501) staff       (20)      473 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_horse.py
--rw-r--r--   0 iskander   (501) staff       (20)     9235 2022-05-09 20:44:51.000000 mhcgnomes-1.8.4/test/test_human.py
--rw-r--r--   0 iskander   (501) staff       (20)    74875 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_iedb_names.py
--rw-r--r--   0 iskander   (501) staff       (20) 10782843 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_imgt_hla_names.py
--rw-r--r--   0 iskander   (501) staff       (20)  3999643 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_ipd_mhc_names.py
--rw-r--r--   0 iskander   (501) staff       (20)     1321 2022-04-18 22:00:42.000000 mhcgnomes-1.8.4/test/test_mhc_class_parsing.py
--rw-r--r--   0 iskander   (501) staff       (20)     1809 2022-05-03 21:28:15.000000 mhcgnomes-1.8.4/test/test_mouse.py
--rw-r--r--   0 iskander   (501) staff       (20)  1334613 2022-05-06 22:43:06.000000 mhcgnomes-1.8.4/test/test_netmhciipan_3_1_alleles.py
--rw-r--r--   0 iskander   (501) staff       (20)   738334 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_netmhcpan_3_0_alleles.py
--rw-r--r--   0 iskander   (501) staff       (20)   340541 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_netmhcpan_4_0_alleles.py
--rw-r--r--   0 iskander   (501) staff       (20)     1579 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_nhp.py
--rw-r--r--   0 iskander   (501) staff       (20)      531 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_normalizing_dictionary.py
--rw-r--r--   0 iskander   (501) staff       (20)      585 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_normalizing_set.py
--rw-r--r--   0 iskander   (501) staff       (20)     9521 2022-04-19 18:32:52.000000 mhcgnomes-1.8.4/test/test_parser.py
--rw-r--r--   0 iskander   (501) staff       (20)     1869 2022-05-09 21:07:10.000000 mhcgnomes-1.8.4/test/test_rat.py
--rw-r--r--   0 iskander   (501) staff       (20)      381 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_serotype.py
--rw-r--r--   0 iskander   (501) staff       (20)      956 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_sheep.py
--rw-r--r--   0 iskander   (501) staff       (20)      869 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_species.py
--rw-r--r--   0 iskander   (501) staff       (20)     1222 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_standard_format.py
--rw-r--r--   0 iskander   (501) staff       (20)     2933 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_swine.py
--rw-r--r--   0 iskander   (501) staff       (20)     2399 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_tokenize.py
--rw-r--r--   0 iskander   (501) staff       (20)     1038 2021-12-21 21:57:22.000000 mhcgnomes-1.8.4/test/test_uniprot_descriptions.py
--rw-r--r--   0 iskander   (501) staff       (20)      203 2022-04-11 20:26:32.000000 mhcgnomes-1.8.4/test/test_workshop_alleles.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-06-01 20:17:21.292626 mhcgnomes-1.8.6/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)       26 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/MANIFEST.in
+-rw-r--r--   0 iskander   (501) staff       (20)     8110 2023-06-01 20:17:21.292479 mhcgnomes-1.8.6/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     7418 2022-08-09 16:32:19.000000 mhcgnomes-1.8.6/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-06-01 20:17:21.276569 mhcgnomes-1.8.6/mhcgnomes/
+-rw-r--r--   0 iskander   (501) staff       (20)     1527 2022-04-21 04:07:52.000000 mhcgnomes-1.8.6/mhcgnomes/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     9166 2022-04-21 04:12:12.000000 mhcgnomes-1.8.6/mhcgnomes/allele.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3411 2022-04-11 22:05:54.000000 mhcgnomes-1.8.6/mhcgnomes/allele_annotations.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2134 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/allele_without_gene.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3655 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/class2_locus.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2965 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/common.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-06-01 20:17:21.278100 mhcgnomes-1.8.6/mhcgnomes/data/
+-rw-r--r--   0 iskander   (501) staff       (20)    91628 2022-04-13 03:59:42.000000 mhcgnomes-1.8.6/mhcgnomes/data/allele_aliases.yaml
+-rw-r--r--   0 iskander   (501) staff       (20)        0 2022-04-20 18:44:13.000000 mhcgnomes-1.8.6/mhcgnomes/data/common_genes.yaml
+-rw-r--r--   0 iskander   (501) staff       (20)    12979 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/data/curated_allele_aliases.yaml
+-rw-r--r--   0 iskander   (501) staff       (20)       12 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/data/default_alleles.yaml
+-rw-r--r--   0 iskander   (501) staff       (20)     1315 2022-05-03 21:09:58.000000 mhcgnomes-1.8.6/mhcgnomes/data/gene_aliases.yaml
+-rw-r--r--   0 iskander   (501) staff       (20)     5582 2022-04-21 04:02:13.000000 mhcgnomes-1.8.6/mhcgnomes/data/haplotypes.yaml
+-rw-r--r--   0 iskander   (501) staff       (20)      480 2022-05-04 03:22:54.000000 mhcgnomes-1.8.6/mhcgnomes/data/known_alleles.yaml
+-rw-r--r--   0 iskander   (501) staff       (20)    10648 2022-04-21 03:48:54.000000 mhcgnomes-1.8.6/mhcgnomes/data/serotypes.yaml
+-rw-r--r--   0 iskander   (501) staff       (20)    31104 2022-04-21 03:59:53.000000 mhcgnomes-1.8.6/mhcgnomes/data/species.yaml
+-rw-r--r--   0 iskander   (501) staff       (20)     2469 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/data.py
+-rw-r--r--   0 iskander   (501) staff       (20)      995 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/dataframe.py
+-rw-r--r--   0 iskander   (501) staff       (20)      761 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/errors.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4128 2022-05-04 21:48:00.000000 mhcgnomes-1.8.6/mhcgnomes/function_api.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4792 2022-04-21 04:12:12.000000 mhcgnomes-1.8.6/mhcgnomes/gene.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6156 2022-04-21 04:10:50.000000 mhcgnomes-1.8.6/mhcgnomes/haplotype.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3049 2022-04-20 20:23:15.000000 mhcgnomes-1.8.6/mhcgnomes/mhc_class.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2659 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/mhc_class_helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1943 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/mutation.py
+-rw-r--r--   0 iskander   (501) staff       (20)     7567 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/normalizing_dictionary.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1932 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/normalizing_set.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6840 2022-04-22 21:13:26.000000 mhcgnomes-1.8.6/mhcgnomes/pair.py
+-rw-r--r--   0 iskander   (501) staff       (20)    63898 2022-08-09 16:32:19.000000 mhcgnomes-1.8.6/mhcgnomes/parser.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4716 2022-04-11 17:49:00.000000 mhcgnomes-1.8.6/mhcgnomes/parsing_helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)     7482 2022-04-21 04:12:12.000000 mhcgnomes-1.8.6/mhcgnomes/result.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5282 2022-04-21 04:07:52.000000 mhcgnomes-1.8.6/mhcgnomes/result_sorting.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1521 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/result_with_gene.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1258 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/result_with_mhc_class.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5355 2022-04-21 04:12:12.000000 mhcgnomes-1.8.6/mhcgnomes/result_with_multiple_alleles.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1910 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/result_with_species.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1944 2022-04-21 04:09:33.000000 mhcgnomes-1.8.6/mhcgnomes/serotype.py
+-rw-r--r--   0 iskander   (501) staff       (20)    25633 2022-04-21 03:58:32.000000 mhcgnomes-1.8.6/mhcgnomes/species.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3300 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/standard_format.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2671 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/token.py
+-rw-r--r--   0 iskander   (501) staff       (20)      695 2021-12-21 21:57:22.000000 mhcgnomes-1.8.6/mhcgnomes/token_canonical_sequences.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4019 2022-04-18 18:57:25.000000 mhcgnomes-1.8.6/mhcgnomes/token_substitution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3799 2022-05-09 21:06:51.000000 mhcgnomes-1.8.6/mhcgnomes/tokenize.py
+-rw-r--r--   0 iskander   (501) staff       (20)       23 2023-06-01 20:17:01.000000 mhcgnomes-1.8.6/mhcgnomes/version.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-06-01 20:17:21.277102 mhcgnomes-1.8.6/mhcgnomes.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     8110 2023-06-01 20:17:21.000000 mhcgnomes-1.8.6/mhcgnomes.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     2299 2023-06-01 20:17:21.000000 mhcgnomes-1.8.6/mhcgnomes.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-06-01 20:17:21.000000 mhcgnomes-1.8.6/mhcgnomes.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-06-01 20:17:21.000000 mhcgnomes-1.8.6/mhcgnomes.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       10 2023-06-01 20:17:21.000000 mhcgnomes-1.8.6/mhcgnomes.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-06-01 20:17:21.292661 mhcgnomes-1.8.6/setup.cfg
+-rw-r--r--   0 iskander   (501) staff       (20)     2201 2023-06-01 20:16:51.000000 mhcgnomes-1.8.6/setup.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-06-01 20:17:21.292302 mhcgnomes-1.8.6/test/
+-rw-r--r--   0 iskander   (501) staff       (20)      476 2023-03-08 17:04:20.000000 mhcgnomes-1.8.6/test/test_Bofr.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4776 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_allele.py
+-rw-r--r--   0 iskander   (501) staff       (20)      342 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_allele_aliases.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1923 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_annotations.py
+-rw-r--r--   0 iskander   (501) staff       (20)      940 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_bad_inputs.py
+-rw-r--r--   0 iskander   (501) staff       (20)      155 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_cat.py
+-rw-r--r--   0 iskander   (501) staff       (20)      307 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_cd1.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1572 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_chicken.py
+-rw-r--r--   0 iskander   (501) staff       (20)      276 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_class2_locus.py
+-rw-r--r--   0 iskander   (501) staff       (20)      801 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_class2_pair.py
+-rw-r--r--   0 iskander   (501) staff       (20)      967 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_cow.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1912 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_dog.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1716 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_fish.py
+-rw-r--r--   0 iskander   (501) staff       (20)      142 2023-03-08 19:48:55.000000 mhcgnomes-1.8.6/test/test_github_issues.py
+-rw-r--r--   0 iskander   (501) staff       (20)      781 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_haplotype.py
+-rw-r--r--   0 iskander   (501) staff       (20)      473 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_horse.py
+-rw-r--r--   0 iskander   (501) staff       (20)     9235 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_human.py
+-rw-r--r--   0 iskander   (501) staff       (20)    74875 2023-03-08 19:49:18.000000 mhcgnomes-1.8.6/test/test_iedb_names.py
+-rw-r--r--   0 iskander   (501) staff       (20) 10782843 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_imgt_hla_names.py
+-rw-r--r--   0 iskander   (501) staff       (20)  3999643 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_ipd_mhc_names.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1321 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_mhc_class_parsing.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1809 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_mouse.py
+-rw-r--r--   0 iskander   (501) staff       (20)  1334613 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_netmhciipan_3_1_alleles.py
+-rw-r--r--   0 iskander   (501) staff       (20)   738334 2023-03-08 19:50:47.000000 mhcgnomes-1.8.6/test/test_netmhcpan_3_0_alleles.py
+-rw-r--r--   0 iskander   (501) staff       (20)   340541 2023-03-08 19:50:49.000000 mhcgnomes-1.8.6/test/test_netmhcpan_4_0_alleles.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1579 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_nhp.py
+-rw-r--r--   0 iskander   (501) staff       (20)      531 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_normalizing_dictionary.py
+-rw-r--r--   0 iskander   (501) staff       (20)      585 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_normalizing_set.py
+-rw-r--r--   0 iskander   (501) staff       (20)     9521 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_parser.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1869 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_rat.py
+-rw-r--r--   0 iskander   (501) staff       (20)      381 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_serotype.py
+-rw-r--r--   0 iskander   (501) staff       (20)      956 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_sheep.py
+-rw-r--r--   0 iskander   (501) staff       (20)      869 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_species.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1222 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_standard_format.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2933 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_swine.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2399 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_tokenize.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1038 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_uniprot_descriptions.py
+-rw-r--r--   0 iskander   (501) staff       (20)      203 2023-06-01 20:16:50.000000 mhcgnomes-1.8.6/test/test_workshop_alleles.py
```

### Comparing `mhcgnomes-1.8.4/LICENSE` & `mhcgnomes-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/PKG-INFO` & `mhcgnomes-1.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: mhcgnomes
-Version: 1.8.4
+Version: 1.8.6
 Summary: Python library for parsing MHC nomenclature in the wild
 Home-page: https://github.com/til-unc/mhcgnomes
 Author: Alex Rubinsteyn
 Author-email: alex.rubinsteyn@unc.edu
 License: http://www.apache.org/licenses/LICENSE-2.0.html
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<a href="https://travis-ci.com/pirl-unc/mhcgnomes">
+<a href="https://app.travis-ci.com/github/pirl-unc/mhcgnomes">
     <img src="https://travis-ci.com/pirl-unc/mhcgnomes.svg?branch=main" alt="Build Status" />
-</a>
-<a href="https://coveralls.io/github/pirl-unc/mhcgnomes?branch=main">
-    <img src="https://coveralls.io/repos/pirl-unc/mhcgnomes/badge.svg?branch=main&service=github" alt="Coverage Status" />
+</a> 
+<a href="https://coveralls.io/github/til-unc/mhcgnomes">
+    <img src="https://coveralls.io/repos/github/til-unc/mhcgnomes/badge.svg?branch=main" alt="Coverage Status">
 </a>
 <a href="https://pypi.python.org/pypi/mhcgnomes/">
     <img src="https://img.shields.io/pypi/v/mhcgnomes.svg?maxAge=1000" alt="PyPI" />
 </a>
 
 
 ![](https://raw.githubusercontent.com/til-unc/mhcgnomes/main/gnome-red-text.png) 
@@ -175,9 +174,7 @@
 
 * [IPD-MHC: nomenclature requirements for the non-human major histocompatibility complex in the next-generation sequencing era](https://link.springer.com/article/10.1007%2Fs00251-018-1072-4)
 * [Comparative MHC nomenclature: report from the ISAG/IUIS-VIC committee 2018]()
 * [ISAG/IUIS-VIC Comparative MHC Nomenclature
 Committee report, 2005](https://link.springer.com/content/pdf/10.1007%2Fs00251-005-0071-4.pdf)
 * [Marsupial MHC Class II β Genes Are Not Orthologous to the Eutherian β Gene Families]()
 * [Nomenclature for factors of the SLA system, update 2008](https://www.ncbi.nlm.nih.gov/pubmed/19317739)
-
-
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: mhcgnomes Version: 1.8.4 Summary: Python library
+Metadata-Version: 2.1 Name: mhcgnomes Version: 1.8.6 Summary: Python library
 for parsing MHC nomenclature in the wild Home-page: https://github.com/til-unc/
 mhcgnomes Author: Alex Rubinsteyn Author-email: alex.rubinsteyn@unc.edu
-License: http://www.apache.org/licenses/LICENSE-2.0.html Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
-Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
-Science/Research Classifier: License :: OSI Approved :: Apache Software License
+License: http://www.apache.org/licenses/LICENSE-2.0.html Classifier:
+Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
+Operating System :: OS Independent Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python Classifier: Topic :: Scientific/
 Engineering :: Bio-Informatics Description-Content-Type: text/markdown License-
 File: LICENSE [Build_Status] [Coverage_Status] [PyPI] ![](https://
 raw.githubusercontent.com/til-unc/mhcgnomes/main/gnome-red-text.png) #
 mhcgnomes: Parsing MHC nomenclature in the wild MHCgnomes is a parsing library
 for multi-species MHC nomenclature which aims to correctly parse every name in
 [IEDB](http://www.iedb.org/), [IMGT/HLA](https://www.ebi.ac.uk/ipd/imgt/hla/),
```

### Comparing `mhcgnomes-1.8.4/README.md` & `mhcgnomes-1.8.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-<a href="https://travis-ci.com/pirl-unc/mhcgnomes">
+<a href="https://app.travis-ci.com/github/pirl-unc/mhcgnomes">
     <img src="https://travis-ci.com/pirl-unc/mhcgnomes.svg?branch=main" alt="Build Status" />
-</a>
-<a href="https://coveralls.io/github/pirl-unc/mhcgnomes?branch=main">
-    <img src="https://coveralls.io/repos/pirl-unc/mhcgnomes/badge.svg?branch=main&service=github" alt="Coverage Status" />
+</a> 
+<a href="https://coveralls.io/github/til-unc/mhcgnomes">
+    <img src="https://coveralls.io/repos/github/til-unc/mhcgnomes/badge.svg?branch=main" alt="Coverage Status">
 </a>
 <a href="https://pypi.python.org/pypi/mhcgnomes/">
     <img src="https://img.shields.io/pypi/v/mhcgnomes.svg?maxAge=1000" alt="PyPI" />
 </a>
 
 
 ![](https://raw.githubusercontent.com/til-unc/mhcgnomes/main/gnome-red-text.png)
```

### Comparing `mhcgnomes-1.8.4/mhcgnomes/__init__.py` & `mhcgnomes-1.8.6/mhcgnomes/__init__.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/allele.py` & `mhcgnomes-1.8.6/mhcgnomes/allele.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/allele_annotations.py` & `mhcgnomes-1.8.6/mhcgnomes/allele_annotations.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/allele_without_gene.py` & `mhcgnomes-1.8.6/mhcgnomes/allele_without_gene.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/class2_locus.py` & `mhcgnomes-1.8.6/mhcgnomes/class2_locus.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/common.py` & `mhcgnomes-1.8.6/mhcgnomes/common.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/data/allele_aliases.yaml` & `mhcgnomes-1.8.6/mhcgnomes/data/allele_aliases.yaml`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/data/curated_allele_aliases.yaml` & `mhcgnomes-1.8.6/mhcgnomes/data/curated_allele_aliases.yaml`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/data/gene_aliases.yaml` & `mhcgnomes-1.8.6/mhcgnomes/data/gene_aliases.yaml`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/data/haplotypes.yaml` & `mhcgnomes-1.8.6/mhcgnomes/data/haplotypes.yaml`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/data/serotypes.yaml` & `mhcgnomes-1.8.6/mhcgnomes/data/serotypes.yaml`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/data/species.yaml` & `mhcgnomes-1.8.6/mhcgnomes/data/species.yaml`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/data.py` & `mhcgnomes-1.8.6/mhcgnomes/data.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/dataframe.py` & `mhcgnomes-1.8.6/mhcgnomes/dataframe.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/errors.py` & `mhcgnomes-1.8.6/mhcgnomes/errors.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/function_api.py` & `mhcgnomes-1.8.6/mhcgnomes/function_api.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/gene.py` & `mhcgnomes-1.8.6/mhcgnomes/gene.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/haplotype.py` & `mhcgnomes-1.8.6/mhcgnomes/haplotype.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/mhc_class.py` & `mhcgnomes-1.8.6/mhcgnomes/mhc_class.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/mhc_class_helpers.py` & `mhcgnomes-1.8.6/mhcgnomes/mhc_class_helpers.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/mutation.py` & `mhcgnomes-1.8.6/mhcgnomes/mutation.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/normalizing_dictionary.py` & `mhcgnomes-1.8.6/mhcgnomes/normalizing_dictionary.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/normalizing_set.py` & `mhcgnomes-1.8.6/mhcgnomes/normalizing_set.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/pair.py` & `mhcgnomes-1.8.6/mhcgnomes/pair.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/parser.py` & `mhcgnomes-1.8.6/mhcgnomes/parser.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1631,8 +1631,8 @@
 
         if result.raw_string != name:
             result = result.copy(raw_string=name)
 
         if max_allele_fields:
             result = result.restrict_allele_fields(max_allele_fields)
 
-        return result
+        return result
```

### Comparing `mhcgnomes-1.8.4/mhcgnomes/parsing_helpers.py` & `mhcgnomes-1.8.6/mhcgnomes/parsing_helpers.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/result.py` & `mhcgnomes-1.8.6/mhcgnomes/result.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/result_sorting.py` & `mhcgnomes-1.8.6/mhcgnomes/result_sorting.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/result_with_gene.py` & `mhcgnomes-1.8.6/mhcgnomes/result_with_gene.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/result_with_mhc_class.py` & `mhcgnomes-1.8.6/mhcgnomes/result_with_mhc_class.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/result_with_multiple_alleles.py` & `mhcgnomes-1.8.6/mhcgnomes/result_with_multiple_alleles.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/result_with_species.py` & `mhcgnomes-1.8.6/mhcgnomes/result_with_species.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/serotype.py` & `mhcgnomes-1.8.6/mhcgnomes/serotype.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/species.py` & `mhcgnomes-1.8.6/mhcgnomes/species.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/standard_format.py` & `mhcgnomes-1.8.6/mhcgnomes/standard_format.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/token.py` & `mhcgnomes-1.8.6/mhcgnomes/token.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/token_canonical_sequences.py` & `mhcgnomes-1.8.6/mhcgnomes/token_canonical_sequences.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/token_substitution.py` & `mhcgnomes-1.8.6/mhcgnomes/token_substitution.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes/tokenize.py` & `mhcgnomes-1.8.6/mhcgnomes/tokenize.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/mhcgnomes.egg-info/PKG-INFO` & `mhcgnomes-1.8.6/mhcgnomes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: mhcgnomes
-Version: 1.8.4
+Version: 1.8.6
 Summary: Python library for parsing MHC nomenclature in the wild
 Home-page: https://github.com/til-unc/mhcgnomes
 Author: Alex Rubinsteyn
 Author-email: alex.rubinsteyn@unc.edu
 License: http://www.apache.org/licenses/LICENSE-2.0.html
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<a href="https://travis-ci.com/pirl-unc/mhcgnomes">
+<a href="https://app.travis-ci.com/github/pirl-unc/mhcgnomes">
     <img src="https://travis-ci.com/pirl-unc/mhcgnomes.svg?branch=main" alt="Build Status" />
-</a>
-<a href="https://coveralls.io/github/pirl-unc/mhcgnomes?branch=main">
-    <img src="https://coveralls.io/repos/pirl-unc/mhcgnomes/badge.svg?branch=main&service=github" alt="Coverage Status" />
+</a> 
+<a href="https://coveralls.io/github/til-unc/mhcgnomes">
+    <img src="https://coveralls.io/repos/github/til-unc/mhcgnomes/badge.svg?branch=main" alt="Coverage Status">
 </a>
 <a href="https://pypi.python.org/pypi/mhcgnomes/">
     <img src="https://img.shields.io/pypi/v/mhcgnomes.svg?maxAge=1000" alt="PyPI" />
 </a>
 
 
 ![](https://raw.githubusercontent.com/til-unc/mhcgnomes/main/gnome-red-text.png) 
@@ -175,9 +174,7 @@
 
 * [IPD-MHC: nomenclature requirements for the non-human major histocompatibility complex in the next-generation sequencing era](https://link.springer.com/article/10.1007%2Fs00251-018-1072-4)
 * [Comparative MHC nomenclature: report from the ISAG/IUIS-VIC committee 2018]()
 * [ISAG/IUIS-VIC Comparative MHC Nomenclature
 Committee report, 2005](https://link.springer.com/content/pdf/10.1007%2Fs00251-005-0071-4.pdf)
 * [Marsupial MHC Class II β Genes Are Not Orthologous to the Eutherian β Gene Families]()
 * [Nomenclature for factors of the SLA system, update 2008](https://www.ncbi.nlm.nih.gov/pubmed/19317739)
-
-
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: mhcgnomes Version: 1.8.4 Summary: Python library
+Metadata-Version: 2.1 Name: mhcgnomes Version: 1.8.6 Summary: Python library
 for parsing MHC nomenclature in the wild Home-page: https://github.com/til-unc/
 mhcgnomes Author: Alex Rubinsteyn Author-email: alex.rubinsteyn@unc.edu
-License: http://www.apache.org/licenses/LICENSE-2.0.html Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
-Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
-Science/Research Classifier: License :: OSI Approved :: Apache Software License
+License: http://www.apache.org/licenses/LICENSE-2.0.html Classifier:
+Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
+Operating System :: OS Independent Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python Classifier: Topic :: Scientific/
 Engineering :: Bio-Informatics Description-Content-Type: text/markdown License-
 File: LICENSE [Build_Status] [Coverage_Status] [PyPI] ![](https://
 raw.githubusercontent.com/til-unc/mhcgnomes/main/gnome-red-text.png) #
 mhcgnomes: Parsing MHC nomenclature in the wild MHCgnomes is a parsing library
 for multi-species MHC nomenclature which aims to correctly parse every name in
 [IEDB](http://www.iedb.org/), [IMGT/HLA](https://www.ebi.ac.uk/ipd/imgt/hla/),
```

### Comparing `mhcgnomes-1.8.4/mhcgnomes.egg-info/SOURCES.txt` & `mhcgnomes-1.8.6/mhcgnomes.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 test/test_cd1.py
 test/test_chicken.py
 test/test_class2_locus.py
 test/test_class2_pair.py
 test/test_cow.py
 test/test_dog.py
 test/test_fish.py
+test/test_github_issues.py
 test/test_haplotype.py
 test/test_horse.py
 test/test_human.py
 test/test_iedb_names.py
 test/test_imgt_hla_names.py
 test/test_ipd_mhc_names.py
 test/test_mhc_class_parsing.py
```

### Comparing `mhcgnomes-1.8.4/setup.py` & `mhcgnomes-1.8.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,16 +51,16 @@
             'Intended Audience :: Science/Research',
             'License :: OSI Approved :: Apache Software License',
             'Programming Language :: Python',
             'Topic :: Scientific/Engineering :: Bio-Informatics',
         ],
         install_requires=[
             "serializable",
-	    "PyYAML==5.4",
+	        "PyYAML>=5.4",
             "pandas",
-	    "numpy",
+	        "numpy",
         ],
         long_description_content_type='text/markdown',
         long_description=readme_markdown,
         packages=['mhcgnomes'],
         package_data={'mhcgnomes': ["data/*.yaml"]},
     )
```

### Comparing `mhcgnomes-1.8.4/test/test_allele.py` & `mhcgnomes-1.8.6/test/test_allele.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_annotations.py` & `mhcgnomes-1.8.6/test/test_annotations.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_bad_inputs.py` & `mhcgnomes-1.8.6/test/test_bad_inputs.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_chicken.py` & `mhcgnomes-1.8.6/test/test_chicken.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_class2_pair.py` & `mhcgnomes-1.8.6/test/test_class2_pair.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_cow.py` & `mhcgnomes-1.8.6/test/test_cow.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_dog.py` & `mhcgnomes-1.8.6/test/test_dog.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_fish.py` & `mhcgnomes-1.8.6/test/test_fish.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_haplotype.py` & `mhcgnomes-1.8.6/test/test_haplotype.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_human.py` & `mhcgnomes-1.8.6/test/test_human.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_iedb_names.py` & `mhcgnomes-1.8.6/test/test_iedb_names.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_imgt_hla_names.py` & `mhcgnomes-1.8.6/test/test_imgt_hla_names.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_ipd_mhc_names.py` & `mhcgnomes-1.8.6/test/test_ipd_mhc_names.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_mhc_class_parsing.py` & `mhcgnomes-1.8.6/test/test_mhc_class_parsing.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_mouse.py` & `mhcgnomes-1.8.6/test/test_mouse.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_netmhciipan_3_1_alleles.py` & `mhcgnomes-1.8.6/test/test_netmhciipan_3_1_alleles.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_netmhcpan_3_0_alleles.py` & `mhcgnomes-1.8.6/test/test_netmhcpan_3_0_alleles.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_netmhcpan_4_0_alleles.py` & `mhcgnomes-1.8.6/test/test_netmhcpan_4_0_alleles.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_nhp.py` & `mhcgnomes-1.8.6/test/test_nhp.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_normalizing_dictionary.py` & `mhcgnomes-1.8.6/test/test_normalizing_dictionary.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_normalizing_set.py` & `mhcgnomes-1.8.6/test/test_normalizing_set.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_parser.py` & `mhcgnomes-1.8.6/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_rat.py` & `mhcgnomes-1.8.6/test/test_rat.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_sheep.py` & `mhcgnomes-1.8.6/test/test_sheep.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_species.py` & `mhcgnomes-1.8.6/test/test_species.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_standard_format.py` & `mhcgnomes-1.8.6/test/test_standard_format.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_swine.py` & `mhcgnomes-1.8.6/test/test_swine.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_tokenize.py` & `mhcgnomes-1.8.6/test/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `mhcgnomes-1.8.4/test/test_uniprot_descriptions.py` & `mhcgnomes-1.8.6/test/test_uniprot_descriptions.py`

 * *Files identical despite different names*

