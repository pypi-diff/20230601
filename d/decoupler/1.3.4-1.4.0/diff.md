# Comparing `tmp/decoupler-1.3.4.tar.gz` & `tmp/decoupler-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoupler-1.3.4.tar", last modified: Mon Feb 27 10:38:55 2023, max compression
+gzip compressed data, was "decoupler-1.4.0.tar", last modified: Thu Jun  1 14:36:07 2023, max compression
```

## Comparing `decoupler-1.3.4.tar` & `decoupler-1.4.0.tar`

### file list

```diff
@@ -1,97 +1,35 @@
-drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-02-27 10:38:55.488600 decoupler-1.3.4/
--rw-rw-r--   0 badi      (1000) badi      (1000)      193 2023-02-21 14:37:43.000000 decoupler-1.3.4/.bumpversion.cfg
--rw-rw-r--   0 badi      (1000) badi      (1000)      553 2022-11-25 14:21:47.000000 decoupler-1.3.4/.codecov.yml
-drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-02-27 10:38:55.468600 decoupler-1.3.4/.github/
-drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-02-27 10:38:55.472600 decoupler-1.3.4/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 badi      (1000) badi      (1000)      868 2022-08-02 11:57:51.000000 decoupler-1.3.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 badi      (1000) badi      (1000)      139 2022-08-02 11:57:51.000000 decoupler-1.3.4/.github/ISSUE_TEMPLATE/question.md
-drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-02-27 10:38:55.472600 decoupler-1.3.4/.github/workflows/
--rw-rw-r--   0 badi      (1000) badi      (1000)     2110 2023-02-27 10:03:02.000000 decoupler-1.3.4/.github/workflows/devel.yml
--rw-rw-r--   0 badi      (1000) badi      (1000)     2294 2023-02-27 10:02:39.000000 decoupler-1.3.4/.github/workflows/main.yml
--rw-rw-r--   0 badi      (1000) badi      (1000)     1830 2022-09-01 13:24:39.000000 decoupler-1.3.4/.gitignore
--rw-rw-r--   0 badi      (1000) badi      (1000)      188 2022-02-28 21:57:49.000000 decoupler-1.3.4/.readthedocs.yml
--rw-rw-r--   0 badi      (1000) badi      (1000)    35149 2022-02-28 21:57:49.000000 decoupler-1.3.4/LICENSE
--rw-rw-r--   0 badi      (1000) badi      (1000)     3068 2023-02-27 10:38:55.488600 decoupler-1.3.4/PKG-INFO
--rw-rw-r--   0 badi      (1000) badi      (1000)     2565 2022-07-16 11:16:01.000000 decoupler-1.3.4/README.md
-drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-02-27 10:38:55.476600 decoupler-1.3.4/decoupler/
--rw-rw-r--   0 badi      (1000) badi      (1000)     1782 2023-02-21 14:37:43.000000 decoupler-1.3.4/decoupler/__init__.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     9084 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/benchmark.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     2337 2022-08-30 11:32:20.000000 decoupler-1.3.4/decoupler/consensus.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     7418 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/decouple.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     5087 2022-11-28 10:18:37.000000 decoupler-1.3.4/decoupler/method_aucell.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     8303 2022-11-22 08:34:04.000000 decoupler-1.3.4/decoupler/method_gsea.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     7534 2022-11-22 08:36:01.000000 decoupler-1.3.4/decoupler/method_gsva.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     3848 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/method_mdt.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     4376 2022-11-22 08:44:04.000000 decoupler-1.3.4/decoupler/method_mlm.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     9876 2022-11-22 08:15:24.000000 decoupler-1.3.4/decoupler/method_ora.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     3649 2022-10-17 07:56:21.000000 decoupler-1.3.4/decoupler/method_udt.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     3742 2022-11-22 08:43:02.000000 decoupler-1.3.4/decoupler/method_ulm.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     9884 2022-11-22 08:40:49.000000 decoupler-1.3.4/decoupler/method_viper.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     6185 2022-11-22 08:39:12.000000 decoupler-1.3.4/decoupler/method_wmean.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     5961 2022-11-22 08:39:44.000000 decoupler-1.3.4/decoupler/method_wsum.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     6487 2022-11-22 08:46:48.000000 decoupler-1.3.4/decoupler/metrics.py
--rw-rw-r--   0 badi      (1000) badi      (1000)    13790 2023-02-14 08:42:05.000000 decoupler-1.3.4/decoupler/omnip.py
--rw-rw-r--   0 badi      (1000) badi      (1000)    21541 2023-02-21 14:34:20.000000 decoupler-1.3.4/decoupler/plotting.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     7376 2022-11-22 08:07:46.000000 decoupler-1.3.4/decoupler/pre.py
-drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-02-27 10:38:55.480600 decoupler-1.3.4/decoupler/tests/
--rw-rw-r--   0 badi      (1000) badi      (1000)        0 2022-07-14 11:35:36.000000 decoupler-1.3.4/decoupler/tests/__init__.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     1459 2022-11-22 08:32:47.000000 decoupler-1.3.4/decoupler/tests/test_aucell.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     3681 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/tests/test_benchmark.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     1307 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/tests/test_consensus.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     2001 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/tests/test_decouple.py
--rw-rw-r--   0 badi      (1000) badi      (1000)      930 2022-11-22 08:34:29.000000 decoupler-1.3.4/decoupler/tests/test_gsea.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     1064 2022-11-22 08:35:29.000000 decoupler-1.3.4/decoupler/tests/test_gsva.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     1056 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/tests/test_mdt.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     3230 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/tests/test_metrics.py
--rw-rw-r--   0 badi      (1000) badi      (1000)      862 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/tests/test_mlm.py
--rw-rw-r--   0 badi      (1000) badi      (1000)      985 2022-11-28 10:19:57.000000 decoupler-1.3.4/decoupler/tests/test_omnip.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     1556 2022-11-22 08:16:19.000000 decoupler-1.3.4/decoupler/tests/test_ora.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     6086 2023-01-17 08:43:16.000000 decoupler-1.3.4/decoupler/tests/test_plotting.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     2834 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/tests/test_pre.py
--rw-rw-r--   0 badi      (1000) badi      (1000)      986 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/tests/test_udt.py
--rw-rw-r--   0 badi      (1000) badi      (1000)      862 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/tests/test_ulm.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     5930 2023-01-16 14:42:48.000000 decoupler-1.3.4/decoupler/tests/test_utils.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     9345 2023-02-23 08:51:26.000000 decoupler-1.3.4/decoupler/tests/test_utilsanndata.py
--rw-rw-r--   0 badi      (1000) badi      (1000)    11125 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/tests/test_utilsbenchmark.py
--rw-rw-r--   0 badi      (1000) badi      (1000)     1633 2022-11-22 08:41:00.000000 decoupler-1.3.4/decoupler/tests/test_viper.py
--rw-rw-r--   0 badi      (1000) badi      (1000)      905 2022-11-22 08:38:07.000000 decoupler-1.3.4/decoupler/tests/test_wmean.py
--rw-rw-r--   0 badi      (1000) badi      (1000)      899 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/tests/test_wsum.py
--rw-rw-r--   0 badi      (1000) badi      (1000)    16380 2023-01-16 14:29:50.000000 decoupler-1.3.4/decoupler/utils.py
--rw-rw-r--   0 badi      (1000) badi      (1000)    19197 2023-02-27 09:57:35.000000 decoupler-1.3.4/decoupler/utils_anndata.py
--rw-rw-r--   0 badi      (1000) badi      (1000)    10906 2022-09-01 13:24:39.000000 decoupler-1.3.4/decoupler/utils_benchmark.py
-drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-02-27 10:38:55.476600 decoupler-1.3.4/decoupler.egg-info/
--rw-rw-r--   0 badi      (1000) badi      (1000)     3068 2023-02-27 10:38:55.000000 decoupler-1.3.4/decoupler.egg-info/PKG-INFO
--rw-rw-r--   0 badi      (1000) badi      (1000)     2259 2023-02-27 10:38:55.000000 decoupler-1.3.4/decoupler.egg-info/SOURCES.txt
--rw-rw-r--   0 badi      (1000) badi      (1000)        1 2023-02-27 10:38:55.000000 decoupler-1.3.4/decoupler.egg-info/dependency_links.txt
--rw-rw-r--   0 badi      (1000) badi      (1000)       37 2023-02-27 10:38:55.000000 decoupler-1.3.4/decoupler.egg-info/requires.txt
--rw-rw-r--   0 badi      (1000) badi      (1000)       10 2023-02-27 10:38:55.000000 decoupler-1.3.4/decoupler.egg-info/top_level.txt
-drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-02-27 10:38:55.480600 decoupler-1.3.4/docs/
--rw-rw-r--   0 badi      (1000) badi      (1000)      638 2022-02-28 21:57:49.000000 decoupler-1.3.4/docs/Makefile
--rw-rw-r--   0 badi      (1000) badi      (1000)      799 2022-02-28 21:57:49.000000 decoupler-1.3.4/docs/make.bat
-drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-02-27 10:38:55.480600 decoupler-1.3.4/docs/source/
-drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-02-27 10:38:55.468600 decoupler-1.3.4/docs/source/_static/
-drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-02-27 10:38:55.480600 decoupler-1.3.4/docs/source/_static/css/
--rw-rw-r--   0 badi      (1000) badi      (1000)      154 2022-02-28 21:57:49.000000 decoupler-1.3.4/docs/source/_static/css/custom.css
--rw-rw-r--   0 badi      (1000) badi      (1000)     1729 2023-01-16 14:34:00.000000 decoupler-1.3.4/docs/source/api.rst
--rw-rw-r--   0 badi      (1000) badi      (1000)     2094 2022-11-28 18:18:10.000000 decoupler-1.3.4/docs/source/conf.py
--rw-rw-r--   0 badi      (1000) badi      (1000)   343847 2022-02-28 21:57:49.000000 decoupler-1.3.4/docs/source/graphical_abstract.png
--rw-rw-r--   0 badi      (1000) badi      (1000)     3479 2022-11-25 15:37:04.000000 decoupler-1.3.4/docs/source/index.rst
--rw-rw-r--   0 badi      (1000) badi      (1000)      359 2022-03-01 08:26:19.000000 decoupler-1.3.4/docs/source/installation.rst
--rw-rw-r--   0 badi      (1000) badi      (1000)    21495 2022-02-28 21:57:49.000000 decoupler-1.3.4/docs/source/logo.png
--rw-rw-r--   0 badi      (1000) badi      (1000)    49386 2022-09-01 13:24:39.000000 decoupler-1.3.4/docs/source/net_plot.png
-drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-02-27 10:38:55.488600 decoupler-1.3.4/docs/source/notebooks/
--rw-rw-r--   0 badi      (1000) badi      (1000)   416220 2023-02-14 08:42:00.000000 decoupler-1.3.4/docs/source/notebooks/benchmark.ipynb
--rw-rw-r--   0 badi      (1000) badi      (1000)   752421 2023-02-14 08:42:28.000000 decoupler-1.3.4/docs/source/notebooks/bulk.ipynb
--rw-rw-r--   0 badi      (1000) badi      (1000)   243071 2022-09-01 13:24:39.000000 decoupler-1.3.4/docs/source/notebooks/cell_annotation.ipynb
--rw-rw-r--   0 badi      (1000) badi      (1000)   294705 2022-11-28 18:08:16.000000 decoupler-1.3.4/docs/source/notebooks/dorothea.ipynb
--rw-rw-r--   0 badi      (1000) badi      (1000)   214865 2022-11-25 09:04:08.000000 decoupler-1.3.4/docs/source/notebooks/msigdb.ipynb
--rw-rw-r--   0 badi      (1000) badi      (1000)   170552 2022-11-28 18:07:58.000000 decoupler-1.3.4/docs/source/notebooks/progeny.ipynb
--rw-rw-r--   0 badi      (1000) badi      (1000)   553708 2023-02-23 08:53:11.000000 decoupler-1.3.4/docs/source/notebooks/pseudobulk.ipynb
--rw-rw-r--   0 badi      (1000) badi      (1000)  2702647 2022-11-28 18:09:05.000000 decoupler-1.3.4/docs/source/notebooks/spatial.ipynb
--rw-rw-r--   0 badi      (1000) badi      (1000)    33581 2022-11-28 17:51:45.000000 decoupler-1.3.4/docs/source/notebooks/translate.ipynb
--rw-rw-r--   0 badi      (1000) badi      (1000)    82984 2022-09-01 13:24:39.000000 decoupler-1.3.4/docs/source/notebooks/usage.ipynb
--rw-rw-r--   0 badi      (1000) badi      (1000)      639 2022-03-29 07:17:22.000000 decoupler-1.3.4/docs/source/reference.rst
--rw-rw-r--   0 badi      (1000) badi      (1000)     4420 2023-02-27 10:21:11.000000 decoupler-1.3.4/docs/source/release_notes.rst
--rw-rw-r--   0 badi      (1000) badi      (1000)       48 2023-02-27 10:21:43.000000 decoupler-1.3.4/docs/source/requirements.txt
--rw-rw-r--   0 badi      (1000) badi      (1000)       38 2023-02-27 10:38:55.488600 decoupler-1.3.4/setup.cfg
--rw-rw-r--   0 badi      (1000) badi      (1000)      882 2023-02-21 14:37:43.000000 decoupler-1.3.4/setup.py
+drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-06-01 14:36:07.581088 decoupler-1.4.0/
+-rw-rw-r--   0 badi      (1000) badi      (1000)    35149 2022-02-28 21:57:49.000000 decoupler-1.4.0/LICENSE
+-rw-rw-r--   0 badi      (1000) badi      (1000)     3068 2023-06-01 14:36:07.581088 decoupler-1.4.0/PKG-INFO
+-rw-rw-r--   0 badi      (1000) badi      (1000)     2565 2022-07-16 11:16:01.000000 decoupler-1.4.0/README.md
+drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-06-01 14:36:07.577088 decoupler-1.4.0/decoupler/
+-rw-rw-r--   0 badi      (1000) badi      (1000)     2029 2023-04-26 15:05:28.000000 decoupler-1.4.0/decoupler/__init__.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     9084 2023-05-31 16:59:59.000000 decoupler-1.4.0/decoupler/benchmark.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     2337 2022-08-30 11:32:20.000000 decoupler-1.4.0/decoupler/consensus.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     7514 2023-04-26 12:17:59.000000 decoupler-1.4.0/decoupler/decouple.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     5087 2022-11-28 10:18:37.000000 decoupler-1.4.0/decoupler/method_aucell.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     8303 2023-06-01 12:57:39.000000 decoupler-1.4.0/decoupler/method_gsea.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     7534 2022-11-22 08:36:01.000000 decoupler-1.4.0/decoupler/method_gsva.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     3848 2022-09-01 13:24:39.000000 decoupler-1.4.0/decoupler/method_mdt.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     4376 2022-11-22 08:44:04.000000 decoupler-1.4.0/decoupler/method_mlm.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     9876 2023-04-26 18:31:23.000000 decoupler-1.4.0/decoupler/method_ora.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     3649 2022-10-17 07:56:21.000000 decoupler-1.4.0/decoupler/method_udt.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     3742 2022-11-22 08:43:02.000000 decoupler-1.4.0/decoupler/method_ulm.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     9884 2022-11-22 08:40:49.000000 decoupler-1.4.0/decoupler/method_viper.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     6393 2023-04-27 10:23:28.000000 decoupler-1.4.0/decoupler/method_wmean.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     6169 2023-04-27 10:23:40.000000 decoupler-1.4.0/decoupler/method_wsum.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     6487 2022-11-22 08:46:48.000000 decoupler-1.4.0/decoupler/metrics.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)    20127 2023-06-01 13:10:11.000000 decoupler-1.4.0/decoupler/omnip.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)    34993 2023-05-31 18:37:27.000000 decoupler-1.4.0/decoupler/plotting.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)     7376 2022-11-22 08:07:46.000000 decoupler-1.4.0/decoupler/pre.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)    16380 2023-01-16 14:29:50.000000 decoupler-1.4.0/decoupler/utils.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)    31439 2023-04-26 19:03:29.000000 decoupler-1.4.0/decoupler/utils_anndata.py
+-rw-rw-r--   0 badi      (1000) badi      (1000)    10906 2022-09-01 13:24:39.000000 decoupler-1.4.0/decoupler/utils_benchmark.py
+drwxrwxr-x   0 badi      (1000) badi      (1000)        0 2023-06-01 14:36:07.581088 decoupler-1.4.0/decoupler.egg-info/
+-rw-rw-r--   0 badi      (1000) badi      (1000)     3068 2023-06-01 14:36:07.000000 decoupler-1.4.0/decoupler.egg-info/PKG-INFO
+-rw-rw-r--   0 badi      (1000) badi      (1000)      708 2023-06-01 14:36:07.000000 decoupler-1.4.0/decoupler.egg-info/SOURCES.txt
+-rw-rw-r--   0 badi      (1000) badi      (1000)        1 2023-06-01 14:36:07.000000 decoupler-1.4.0/decoupler.egg-info/dependency_links.txt
+-rw-rw-r--   0 badi      (1000) badi      (1000)       37 2023-06-01 14:36:07.000000 decoupler-1.4.0/decoupler.egg-info/requires.txt
+-rw-rw-r--   0 badi      (1000) badi      (1000)       10 2023-06-01 14:36:07.000000 decoupler-1.4.0/decoupler.egg-info/top_level.txt
+-rw-rw-r--   0 badi      (1000) badi      (1000)       38 2023-06-01 14:36:07.581088 decoupler-1.4.0/setup.cfg
+-rw-rw-r--   0 badi      (1000) badi      (1000)      882 2023-03-21 12:10:03.000000 decoupler-1.4.0/setup.py
```

### Comparing `decoupler-1.3.4/LICENSE` & `decoupler-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/PKG-INFO` & `decoupler-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoupler
-Version: 1.3.4
+Version: 1.4.0
 Summary: Ensemble of methods to infer biological activities from omics data
 Home-page: https://github.com/saezlab/decoupler-py
 Author: Pau Badia i Mompel
 Author-email: pau.badia@uni-heidelberg.de
 Project-URL: Bug Tracker, https://github.com/saezlab/decoupler-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `decoupler-1.3.4/README.md` & `decoupler-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/__init__.py` & `decoupler-1.4.0/decoupler/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-__version__ = '1.3.4'  # noqa: F401
+__version__ = '1.4.0'  # noqa: F401
 __version_info__ = tuple([int(num) for num in __version__.split('.')])  # noqa: F401
 
 from .pre import extract, match, rename_net, get_net_mat, filt_min_n, mask_features  # noqa: F401
 from .utils import melt, show_methods, check_corr, get_toy_data, summarize_acts, assign_groups  # noqa: F401
 from .utils import dense_run, p_adjust_fdr, shuffle_net, read_gmt  # noqa: F401
-from .utils_anndata import get_acts, swap_layer, get_pseudobulk, get_contrast  # noqa: F401
-from .utils_anndata import get_top_targets, format_contrast_results  # noqa: F401
+from .utils_anndata import get_acts, swap_layer, get_pseudobulk, get_contrast, rank_sources_groups  # noqa: F401
+from .utils_anndata import get_top_targets, format_contrast_results, filter_by_expr, filter_by_prop  # noqa: F401
 from .method_wmean import run_wmean  # noqa: F401
 from .method_wsum import run_wsum  # noqa: F401
 from .method_ulm import run_ulm  # noqa: F401
 from .method_mdt import run_mdt  # noqa: F401
 from .method_mlm import run_mlm  # noqa: F401
 from .method_udt import run_udt  # noqa: F401
 from .method_ora import run_ora, test1r, get_ora_df  # noqa: F401
 from .method_gsva import run_gsva  # noqa: F401
 from .method_gsea import run_gsea  # noqa: F401
 from .method_viper import run_viper  # noqa: F401
 from .method_aucell import run_aucell  # noqa: F401
 from .decouple import decouple, run_consensus  # noqa: F401
 from .consensus import cons  # noqa: F401
-from .omnip import show_resources, get_resource, get_progeny, get_dorothea, translate_net  # noqa: F401
-from .plotting import plot_volcano, plot_violins, plot_barplot  # noqa: F401
-from .plotting import plot_metrics_scatter, plot_metrics_boxplot, plot_metrics_scatter_cols  # noqa: F401
+from .omnip import show_resources, get_resource, get_progeny, get_dorothea, translate_net, get_collectri  # noqa: F401
+from .omnip import get_ksn_omnipath  # noqa: F401
+from .plotting import plot_volcano, plot_violins, plot_barplot, plot_metrics_scatter, plot_metrics_boxplot  # noqa: F401
+from .plotting import plot_metrics_scatter_cols, plot_psbulk_samples, plot_filter_by_expr, plot_filter_by_prop  # noqa: F401
+from .plotting import plot_volcano_df, plot_targets  # noqa: F401
 from .benchmark import benchmark, format_benchmark_inputs, get_performances  # noqa: F401
 from .utils_benchmark import get_toy_benchmark_data, show_metrics  # noqa: F401
 from .metrics import metric_auroc, metric_auprc, metric_mcauroc, metric_mcauprc  # noqa: F401
```

### Comparing `decoupler-1.3.4/decoupler/benchmark.py` & `decoupler-1.4.0/decoupler/benchmark.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/consensus.py` & `decoupler-1.4.0/decoupler/consensus.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/decouple.py` & `decoupler-1.4.0/decoupler/decouple.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         # Store obtained dfs
         for r in results:
             mat.obsm[r] = results[r]
     else:
         return results
 
 
-def run_consensus(mat, net, source='source', target='target', weight='weight', min_n=5, verbose=False, use_raw=True):
+def run_consensus(mat, net, source='source', target='target', weight='weight', min_n=5, verbose=False, use_raw=True, args={}):
     """
     Consensus score from top methods.
 
     This consensus score is calculated from the three top performer methods: `ulm`, `mlm` and `wsum_norm`.
     For each of these methods, the obtained activities are transformed into z-scores, first for positive
     values and then for negative ones. These two sets of z-score transformed activities are computed by
     subsetting the values bigger or lower than 0, then by mirroring the selected values into their
@@ -188,14 +188,16 @@
         Column name in net with weights.
     min_n : int
         Minimum of targets per source. If less, sources are removed.
     verbose : bool
         Whether to show progress.
     use_raw : bool
         Use raw attribute of mat if present.
+    args : dict
+        Parameters for the ``decoupler.decouple`` function.
 
     Returns
     -------
     estimate : DataFrame
         Consensus scores. Stored in `.obsm['consensus_estimate']` if `mat` is AnnData.
     pvals : DataFrame
         Obtained p-values. Stored in `.obsm['consensus_pvals']` if `mat` is AnnData.
@@ -205,15 +207,15 @@
     m, r, c = extract(mat, use_raw=use_raw, verbose=verbose)
 
     if verbose:
         print('Running consensus.')
 
     # Run top methods
     res = decouple(mat=[m, r, c], net=net, source=source, target=target, weight=weight,
-                   min_n=min_n, verbose=verbose, use_raw=use_raw)
+                   min_n=min_n, verbose=verbose, use_raw=use_raw, args=args)
 
     # Exctract
     estimate, pvals = res['consensus_estimate'], res['consensus_pvals']
 
     # AnnData support
     if isinstance(mat, AnnData):
         # Update obsm AnnData object
```

### Comparing `decoupler-1.3.4/decoupler/method_aucell.py` & `decoupler-1.4.0/decoupler/method_aucell.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/method_gsea.py` & `decoupler-1.4.0/decoupler/method_gsea.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/method_gsva.py` & `decoupler-1.4.0/decoupler/method_gsva.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/method_mdt.py` & `decoupler-1.4.0/decoupler/method_mdt.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/method_mlm.py` & `decoupler-1.4.0/decoupler/method_mlm.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/method_ora.py` & `decoupler-1.4.0/decoupler/method_ora.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/method_udt.py` & `decoupler-1.4.0/decoupler/method_udt.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/method_ulm.py` & `decoupler-1.4.0/decoupler/method_ulm.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/method_viper.py` & `decoupler-1.4.0/decoupler/method_viper.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/method_wmean.py` & `decoupler-1.4.0/decoupler/method_wmean.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,24 @@
     pvals = np.where(pvals >= 0.5, 1-(pvals), pvals)
     pvals = pvals * 2
 
     # Compute z-score
     norm = np.zeros((mat.shape[0], net.shape[1]), dtype=nb.f4)
     for i in nb.prange(mat.shape[0]):
         for j in range(net.shape[1]):
-            norm[i, j] = (estimate[i, j] - np.mean(null_dst[i, j, :])) / std(null_dst[i, j, :], 1)
+            e = estimate[i, j]
+            d = std(null_dst[i, j, :], 1)
+            if d != 0.:
+                n = (e - np.mean(null_dst[i, j, :])) / d
+            else:
+                if e != 0.:
+                    n = np.inf
+                else:
+                    n = 0.
+            norm[i, j] = n
 
     # Compute corr score
     corr = (estimate * -np.log10(pvals)).astype(nb.f4)
 
     return norm, corr, pvals
```

### Comparing `decoupler-1.3.4/decoupler/method_wsum.py` & `decoupler-1.4.0/decoupler/method_wsum.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,24 @@
     pvals = np.where(pvals >= 0.5, 1-(pvals), pvals)
     pvals = pvals * 2
 
     # Compute z-score
     norm = np.zeros((mat.shape[0], net.shape[1]), dtype=nb.f4)
     for i in nb.prange(mat.shape[0]):
         for j in range(net.shape[1]):
-            norm[i, j] = (estimate[i, j] - np.mean(null_dst[i, j, :])) / std(null_dst[i, j, :], 1)
+            e = estimate[i, j]
+            d = std(null_dst[i, j, :], 1)
+            if d != 0.:
+                n = (e - np.mean(null_dst[i, j, :])) / d
+            else:
+                if e != 0.:
+                    n = np.inf
+                else:
+                    n = 0.
+            norm[i, j] = n
 
     # Compute corr score
     corr = (estimate * -np.log10(pvals)).astype(nb.f4)
 
     return norm, corr, pvals
```

### Comparing `decoupler-1.3.4/decoupler/metrics.py` & `decoupler-1.4.0/decoupler/metrics.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/omnip.py` & `decoupler-1.4.0/decoupler/omnip.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 ]
 
 import os
 import builtins
 from types import ModuleType
 from typing import Iterable
 from typing_extensions import Literal
+import warnings
+from datetime import datetime
 import numpy as np
 import pandas as pd
 
 builtins.PYPATH_LOG = os.devnull
 PYPATH_MIN_VERSION = '0.14.28'
 ORGANISMS = {
     'human': (
@@ -49,16 +51,16 @@
     try:
 
         import omnipath as op
 
     except Exception:
 
         raise ImportError(
-            'omnipath is not installed. Please install it with: '
-            'pip install omnipath'
+            'omnipath is not installed. Please install it by: '
+            '`pip install omnipath`.'
         )
 
     return op
 
 
 def _is_organism(
         name: str | int,
@@ -91,15 +93,19 @@
     """
     Does the organism name or ID mean human?
     """
 
     return _is_organism(name, 'rat')
 
 
-def get_progeny(organism: str | int = 'human', top: int = 100) -> pd.DataFrame:
+def get_progeny(
+        organism: str | int = 'human',
+        top: int = 100,
+        **kwargs
+        ) -> pd.DataFrame:
     """
     Pathway RespOnsive GENes for activity inference (PROGENy).
 
     Wrapper to access PROGENy model gene weights. Each pathway is defined with
     a collection of target genes, each interaction has an associated p-value
     and weight. The top significant interactions per pathway are returned.
 
@@ -107,25 +113,27 @@
     ----------
     organism : str
         The organism of interest: either NCBI Taxonomy ID, common name,
         latin name or Ensembl name. Organisms other than human will be
         translated from human data by orthology.
     top : int
         Number of genes per pathway to return.
+    kwargs
+        Passed to `omnipath.requests.Annotations.get`.
 
     Returns
     -------
     p : DataFrame
         Dataframe in long format containing target genes for each pathway with
         their associated weights and p-values.
     """
 
     op = _check_if_omnipath()
 
-    p = op.requests.Annotations.get(resources='PROGENy')
+    p = op.requests.Annotations.get(resources='PROGENy', **kwargs)
     p = p.set_index([
         'record_id', 'uniprot', 'genesymbol',
         'entity_type', 'source', 'label',
     ])
     p = p.unstack('label').droplevel(axis=1, level=0)
     p.columns = np.array(p.columns)
     p = p.reset_index()
@@ -152,18 +160,22 @@
         p = translate_net(
             p,
             columns='target',
             source_organism=9606,
             target_organism=organism,
         )
 
-    return p
+    return p.reset_index(drop=True)
 
 
-def get_resource(name: str, organism: str | int = 'human') -> pd.DataFrame:
+def get_resource(
+        name: str,
+        organism: str | int = 'human',
+        **kwargs
+        ) -> pd.DataFrame:
     """
     Wrapper to access resources inside Omnipath.
 
     This wrapper allows to easly query different prior knowledge resources. To
     check available resources run ``decoupler.show_resources()``. For more
     information visit the official website for
     [Omnipath](https://omnipathdb.org/).
@@ -172,14 +184,16 @@
     ----------
     name : str
         Name of the resource to query.
     organism : int | str
         The organism of interest: either NCBI Taxonomy ID, common name,
         latin name or Ensembl name. Organisms other than human will be
         translated from human data by orthology.
+    kwargs
+        Passed to `omnipath.requests.Annotations.get`.
 
     Returns
     -------
     df : DataFrame
         Dataframe in long format relating genes to biological entities.
     """
 
@@ -188,15 +202,19 @@
         f'{name} is not a valid resource. Please, run '
         'decoupler.show_resources to see the list of available resources.'
     )
     assert name in resources, msg
 
     op = _check_if_omnipath()
 
-    df = op.requests.Annotations.get(resources=name, entity_type='protein')
+    df = op.requests.Annotations.get(
+        resources=name,
+        entity_type='protein',
+        **kwargs
+    )
     df = df.set_index([
         'record_id', 'uniprot',
         'genesymbol', 'entity_type',
         'source', 'label',
     ])
     df = df.unstack('label').droplevel(axis=1, level=0)
     df = df.drop(
@@ -211,15 +229,15 @@
         df = translate_net(
             df,
             target_organism=organism,
             columns='genesymbol',
             unique_by=None,
         )
 
-    return df
+    return df.reset_index(drop=True)
 
 
 def show_resources() -> list:
     """
     Shows available resources in Omnipath. For more information visit the
     official website for [Omnipath](https://omnipathdb.org/).
 
@@ -234,14 +252,15 @@
     return list(op.requests.Annotations.resources())
 
 
 def get_dorothea(
         organism: str | int = 'human',
         levels: DOROTHEA_LEVELS | Iterable[DOROTHEA_LEVELS] = ('A', 'B', 'C'),
         weight_dict: dict[str, int] | None = None,
+        **kwargs
         ) -> pd.DataFrame:
     """
     DoRothEA gene regulatory network.
 
     Wrapper to access DoRothEA gene regulatory network. DoRothEA is a
     comprehensive resource containing a curated collection of transcription
     factors (TFs) and their target genes. Each interaction is weighted by its
@@ -257,14 +276,16 @@
     levels : list
         List of confidence levels to return. Goes from A to D, A being the
         most confident and D being the less.
     weight_dict : dict
         Dictionary of values to divide the mode of regulation (-1 or 1),
         one for each confidence level. Bigger values will generate weights
         close to zero.
+    kwargs
+        Passed to `omnipath.interactions.Dorothea.get`.
 
     Returns
     -------
     do : DataFrame
         Dataframe in long format containing target genes for each TF with
         their associated weights and confidence level.
     """
@@ -275,14 +296,15 @@
 
     _organism = (
         'mouse' if _is_mouse(organism) else
         'rat' if _is_rat(organism) else
         'human'
     )
 
+    _omnipath_check_version()
     op = _check_if_omnipath()
 
     # Load Dorothea
     do = op.interactions.Dorothea.get(
         fields=['dorothea_level', 'extra_attrs'],
         dorothea_levels=['A', 'B', 'C', 'D'],
         genesymbols=True,
@@ -352,15 +374,113 @@
             net=do,
             target_organism=organism,
             columns=('source', 'target'),
             unique_by=('source', 'target'),
             id_type='genesymbol',
         )
 
-    return do
+    return do.reset_index(drop=True)
+
+
+def get_collectri(
+        organism: str | int = 'human',
+        split_complexes=False,
+        **kwargs
+        ) -> pd.DataFrame:
+    """
+    CollecTRI gene regulatory network.
+
+    Wrapper to access CollecTRI gene regulatory network. CollecTRI is a
+    comprehensive resource containing a curated collection of transcription
+    factors (TFs) and their target genes. It is an expansion of DoRothEA.
+    Each interaction is weighted by its mode of regulation (either positive or negative).
+
+    Parameters
+    ----------
+    organism : str
+        The organism of interest: either NCBI Taxonomy ID, common name,
+        latin name or Ensembl name. Organisms other than human will be
+        translated from human data by orthology.
+    split_complexes : bool
+        Whether to split complexes into subunits. By default complexes are kept as they are.
+    kwargs
+        Passed to `omnipath.interactions.CollecTRI.get`.
+
+    Returns
+    -------
+    ct : DataFrame
+        Dataframe in long format containing target genes for each TF with
+        their associated weights.
+    """
+
+    _organism = (
+        'mouse' if _is_mouse(organism) else
+        'rat' if _is_rat(organism) else
+        'human'
+    )
+
+    _omnipath_check_version()
+    op = _check_if_omnipath()
+
+    # Load collectri
+    ct = op.interactions.CollecTRI.get(genesymbols=True, organism=_organism, loops=True, **kwargs)
+    if _organism == 'human':
+        mirna = op.interactions.TFmiRNA.get(genesymbols=True, databases=['CollecTRI'], strict_evidences=True)
+        ct = pd.concat([ct, mirna], ignore_index=True)
+
+    # Separate gene_pairs from normal interactions
+    msk = np.array([s.startswith('COMPLEX') for s in ct['source']])
+    cols = ['source_genesymbol', 'target_genesymbol', 'is_stimulation', 'is_inhibition']
+    ct_inter = ct.loc[~msk, cols]
+    ct_cmplx = ct.loc[msk, cols].copy()
+
+    # Merge gene_pairs into complexes
+    if not split_complexes:
+        cmpl_gsym = []
+        for s in ct_cmplx['source_genesymbol']:
+            if s.startswith('JUN') or s.startswith('FOS'):
+                cmpl_gsym.append('AP1')
+            elif s.startswith('REL') or s.startswith('NFKB'):
+                cmpl_gsym.append('NFKB')
+            else:
+                cmpl_gsym.append(s)
+        ct_cmplx.loc[:, 'source_genesymbol'] = cmpl_gsym
+
+    # Merge
+    ct = pd.concat([ct_inter, ct_cmplx])
+
+    # Drop duplicates
+    ct = ct.drop_duplicates(['source_genesymbol', 'target_genesymbol'])
+
+    # Add weight
+    weights = []
+    for is_stimulation, is_inhibition in zip(ct['is_stimulation'], ct['is_inhibition']):
+        if is_stimulation:
+            weights.append(1)
+        elif is_inhibition:
+            weights.append(-1)
+        else:
+            weights.append(1)
+    ct['weight'] = weights
+
+    # Select and rename columns
+    ct = ct.rename(columns={'source_genesymbol': 'source', 'target_genesymbol': 'target'})
+    ct = ct[['source', 'target', 'weight']]
+
+    if _organism not in ('mouse', 'rat') and not _is_human(organism):
+
+        ct = translate_net(
+            net=ct,
+            target_organism=organism,
+            columns=('source', 'target'),
+            unique_by=('source', 'target'),
+            id_type='genesymbol',
+        )
+
+    return ct.reset_index(drop=True)
 
 
 def translate_net(
         net: pd.DataFrame,
         columns: str | Iterable[str] = ('source', 'target', 'genesymbol'),
         source_organism: str | int = 'human',
         target_organism: str | int = 'mouse',
@@ -474,7 +594,83 @@
 
     if unique_by and all(c in hom_net.columns for c in unique_by):
 
         # Remove duplicated based on source and target
         hom_net = hom_net[~hom_net.duplicated(unique_by)]
 
     return hom_net
+
+
+def get_ksn_omnipath(
+        ) -> pd.DataFrame:
+    """
+    OmniPath kinase-substrate network
+
+    Wrapper to access the OmniPath kinase-substrate network. It contains a collection of
+    kinases and their target phosphosites. Each interaction is is weighted by its mode of
+    regulation (either positive for phosphorylation or negative for dephosphorylation).
+
+    Returns
+    -------
+    ksn : DataFrame
+        Dataframe in long format containing target phosphosites for each kinase with
+        their associated weights.
+    """
+
+    op = _check_if_omnipath()
+
+    # Load Kinase-Substrate Network
+    ksn = op.requests.Enzsub.get(genesymbols=True)
+
+    # Filter by phosphorilation
+    cols = ['enzyme_genesymbol', 'substrate_genesymbol', 'residue_type',
+            'residue_offset', 'modification', 'references', 'n_references']
+    msk = np.isin(ksn['modification'], ['phosphorylation', 'dephosphorylation'])
+    ksn = ksn.loc[msk, cols]
+
+    # Remove inters that are only Protmap, keep nans
+    msk = []
+    for r, l in zip(ksn['references'], ksn['n_references']):
+        if type(r) is str:
+            n = r.count('ProtMapper')
+            b = n < l
+        else:
+            b = True
+        msk.append(b)
+    msk = np.array(msk)
+    ksn = ksn.loc[msk, :]
+
+    # Build target gene substrate column
+    ksn['target'] = ['{0}_{1}{2}'.format(sub, res, off) for sub, res, off in
+                     zip(ksn['substrate_genesymbol'], ksn['residue_type'], ksn['residue_offset'])]
+
+    # Assigns mode of regulation
+    ksn['weight'] = [+1 if mod == 'phosphorylation' else -1 for mod in ksn['modification']]
+
+    # Remove duplicates
+    ksn = ksn.rename(columns={'enzyme_genesymbol': 'source'})[['source', 'target', 'weight']]
+    ksn = ksn.drop_duplicates(['source', 'target', 'weight'])
+
+    # If duplicates remain, keep dephosphorylation
+    ksn = ksn.groupby(['source', 'target']).min().reset_index()
+
+    return ksn
+
+
+def _omnipath_check_version() -> None:
+
+    import omnipath
+
+    version = tuple(map(int, omnipath.__version__.split('.')))
+
+    if version < (1, 0, 7):
+
+        op_updated = datetime.fromtimestamp(os.stat(omnipath.__file__).st_mtime)
+
+        if op_updated < datetime(2023, 5, 30):
+
+            warnings.warn(
+                'The installed version of `omnipath` is older than 1.0.7 or '
+                '2023-05-30. To make sure CollecTRI and DoRothEA data is '
+                'processed correctly, please update to the latest version by '
+                '`pip install git+https://github.com/saezlab/omnipath.git`.'
+            )
```

### Comparing `decoupler-1.3.4/decoupler/plotting.py` & `decoupler-1.4.0/decoupler/plotting.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import numpy as np
 import pandas as pd
+from anndata import AnnData
 
 from .pre import extract, rename_net
+from .utils_anndata import get_filterbyexpr_inputs, get_min_sample_size, get_cpm_cutoff, get_cpm
 
 
 def check_if_matplotlib(return_mpl=False):
     if not return_mpl:
         try:
             import matplotlib.pyplot as plt
         except Exception:
@@ -34,17 +36,20 @@
         raise ImportError('adjustText is not installed. Please install it with: pip install adjustText')
     return at
 
 
 def save_plot(fig, ax, save):
     if save is not None:
         if ax is not None:
-            fig.savefig(save, bbox_inches='tight')
+            if fig is not None:
+                fig.savefig(save, bbox_inches='tight')
+            else:
+                raise ValueError("fig is None, cannot save figure.")
         else:
-            raise ValueError("ax is not None, cannot save figure.")
+            raise ValueError("ax is None, cannot save figure.")
 
 
 def filter_limits(df, sign_limit=None, lFCs_limit=None):
 
     # Define limits if not defined
     if sign_limit is None:
         sign_limit = np.inf
@@ -179,15 +184,192 @@
     for x, y, s in zip(signs['logFCs'], signs['pvals'], signs.index):
         texts.append(ax.text(x, y, s))
     if len(texts) > 0:
         at.adjust_text(texts, arrowprops=dict(arrowstyle='-', color='black'), ax=ax)
 
     save_plot(fig, ax, save)
 
-    if return_fig and ax is None:
+    if return_fig:
+        return fig
+
+
+def plot_volcano_df(data, x, y, top=5, sign_thr=0.05, lFCs_thr=0.5, sign_limit=None, lFCs_limit=None,
+                    figsize=(7, 5), dpi=100, ax=None, return_fig=False, save=None):
+    """
+    Plot logFC and p-values from a long formated data-frame.
+
+    Parameters
+    ----------
+    data : pd.DataFrame
+        Results of DEA in long format.
+    x : str
+        Column name of data storing the logFCs.
+    y : str
+        Columns name of data storing the p-values.
+    top : int
+        Number of top differentially expressed features to show.
+    sign_thr : float
+        Significance threshold for p-values.
+    lFCs_thr : float
+        Significance threshold for logFCs.
+    sign_limit : float
+        Limit of p-values to plot in -log10.
+    lFCs_limit : float
+        Limit of logFCs to plot in absolute value.
+    figsize : tuple
+        Figure size.
+    dpi : int
+        DPI resolution of figure.
+    ax : Axes, None
+        A matplotlib axes object. If None returns new figure.
+    return_fig : bool
+        Whether to return a Figure object or not.
+    save : str, None
+        Path to where to save the plot. Infer the filetype if ending on {`.pdf`, `.png`, `.svg`}.
+
+    Returns
+    -------
+    fig : Figure, None
+        If return_fig, returns Figure object.
+    """
+
+    # Load plotting packages
+    plt = check_if_matplotlib()
+    at = check_if_adjustText()
+
+    # Transform sign_thr
+    sign_thr = -np.log10(sign_thr)
+
+    # Extract df
+    df = data.copy()
+    df['logFCs'] = df[x]
+    df['pvals'] = -np.log10(df[y])
+
+    # Filter by limits
+    df = filter_limits(df, sign_limit=sign_limit, lFCs_limit=lFCs_limit)
+
+    # Define color by up or down regulation and significance
+    df['weight'] = 'gray'
+    up_msk = (df['logFCs'] >= lFCs_thr) & (df['pvals'] >= sign_thr)
+    dw_msk = (df['logFCs'] <= -lFCs_thr) & (df['pvals'] >= sign_thr)
+    df.loc[up_msk, 'weight'] = '#D62728'
+    df.loc[dw_msk, 'weight'] = '#1F77B4'
+
+    # Plot
+    fig = None
+    if ax is None:
+        fig, ax = plt.subplots(1, 1, figsize=figsize, dpi=dpi)
+    df.plot.scatter(x='logFCs', y='pvals', c='weight', sharex=False, ax=ax)
+
+    # Draw sign lines
+    ax.axhline(y=sign_thr, linestyle='--', color="black")
+    ax.axvline(x=lFCs_thr, linestyle='--', color="black")
+    ax.axvline(x=-lFCs_thr, linestyle='--', color="black")
+
+    # Plot top sign features
+    signs = df[up_msk | dw_msk].sort_values('pvals', ascending=False)
+    signs = signs.iloc[:top]
+
+    # Add labels
+    ax.set_ylabel('-log10(pvals)')
+    texts = []
+    for x, y, s in zip(signs['logFCs'], signs['pvals'], signs.index):
+        texts.append(ax.text(x, y, s))
+    if len(texts) > 0:
+        at.adjust_text(texts, arrowprops=dict(arrowstyle='-', color='black'), ax=ax)
+
+    save_plot(fig, ax, save)
+
+    if return_fig:
+        return fig
+
+
+def plot_targets(data, stat, source_name, net, source='source', target='target', weight='weight', top=10, figsize=(5, 5),
+                 dpi=100, ax=None, return_fig=False, save=None):
+    """
+    Plot the weight and statistic of the target genes of a given source.
+
+    Parameters
+    ----------
+    data : pd.DataFrame
+        Results of DEA in long format.
+    stat : str
+        Column name of data storing feature statistics.
+    source_name : str
+        Name of source to plot.
+    net : DataFrame
+        Network dataframe..
+    source : str
+        Column name in net with source nodes.
+    target : str
+        Column name in net with target nodes.
+    weight : str, None
+        Column name in net with weights.
+    top : int
+        Number of features to show labels.
+    figsize : tuple
+        Figure size.
+    dpi : int
+        DPI resolution of figure.
+    ax : Axes, None
+        A matplotlib axes object. If None returns new figure.
+    return_fig : bool
+        Whether to return a Figure object or not.
+    save : str, None
+        Path to where to save the plot. Infer the filetype if ending on {`.pdf`, `.png`, `.svg`}.
+
+    Returns
+    -------
+    fig : Figure, None
+        If return_fig, returns Figure object.
+    """
+
+    # Load plotting packages
+    plt = check_if_matplotlib()
+    at = check_if_adjustText()
+
+    # Extract data
+    data = data[stat].copy()
+    net = net.copy()
+
+    # Extract weights of given source from net
+    w = net[net[source] == source_name].set_index(target)[[weight]]
+
+    # Join
+    data = pd.concat([data, w], axis=1, join='inner')
+
+    # Define activation/inhibition color
+    pos = ((data[weight] >= 0) & (data[stat] >= 0)) | ((data[weight] < 0) & (data[stat] < 0))
+    data['color'] = '#1F77B4'
+    data.loc[pos, 'color'] = '#D62728'
+
+    # Plot
+    fig = None
+    if ax is None:
+        fig, ax = plt.subplots(1, 1, figsize=figsize, dpi=dpi)
+    data.plot.scatter(x=weight, y=stat, c='color', ax=ax)
+    ax.grid()
+
+    # Draw sign lines
+    ax.axhline(y=0, linestyle='--', color="black")
+    ax.axvline(x=0, linestyle='--', color="black")
+    ax.set_title(source_name)
+
+    # Add labels for top features
+    top_names = np.abs((data[weight] * data[stat])).sort_values().tail(top).index
+    data = data.loc[top_names, :]
+    texts = []
+    for x, y, s in zip(data[weight], data[stat], data.index):
+        texts.append(ax.text(x, y, s))
+    if len(texts) > 0:
+        at.adjust_text(texts, arrowprops=dict(arrowstyle='-', color='black'), ax=ax)
+
+    save_plot(fig, ax, save)
+
+    if return_fig:
         return fig
 
 
 def plot_violins(mat, thr=None, log=False, use_raw=False, figsize=(7, 5), dpi=100, ax=None, title=None, ylabel=None,
                  color='#1F77B4', return_fig=False, save=None):
     """
     Plot distribution of features' values per sample.
@@ -254,15 +436,15 @@
     if title is not None:
         ax.set_title(title)
     if ylabel is not None:
         ax.set_ylabel(ylabel)
 
     save_plot(fig, ax, save)
 
-    if return_fig and ax is None:
+    if return_fig:
         return fig
 
 
 def set_limits(vmin, vcenter, vmax, values):
 
     if vmin is None:
         vmin = values.min()
@@ -379,15 +561,15 @@
     # Add legend
     sm = plt.cm.ScalarMappable(cmap=cmap, norm=divnorm)
     sm.set_array([])
     fig.colorbar(sm, ax=ax)
 
     save_plot(fig, ax, save)
 
-    if return_fig and ax is None:
+    if return_fig:
         return fig
 
 
 def build_msks(df, groupby):
 
     # Process groupby
     if type(groupby) is str:
@@ -515,15 +697,15 @@
         at.adjust_text(texts, arrowprops=dict(arrowstyle='-', color='gray'), ax=ax)
 
     # Write labels
     write_labels(ax, title, xlabel, ylabel, x, y)
 
     save_plot(fig, ax, save)
 
-    if return_fig and ax is None:
+    if return_fig:
         return fig
 
 
 def plot_metrics_scatter_cols(df, col, x='auroc', y='auprc', groupby=None, n_cols=4, figsize=(10, 12), dpi=100,
                               return_fig=False, save=None):
     """
     Extension of the function plot_metrics_scatter to group metrics by two categories at the same time.
@@ -596,15 +778,15 @@
 
     # Format legend
     handles, labels = axes[len(cats) - 1].get_legend_handles_labels()
     fig.legend(handles, labels, loc='center left', bbox_to_anchor=(1, 0.5), frameon=False)
 
     save_plot(fig, ax, save)
 
-    if return_fig and ax is None:
+    if return_fig:
         return fig
 
 
 def plot_metrics_boxplot(df, metric, groupby=None, figsize=(5, 5), dpi=100, ax=None, title=None,
                          xlabel=None, ylabel=None, return_fig=False, save=None, **kwargs):
     """
     Plot boxplots showing the distribution of scores between methods for a metric.
@@ -703,9 +885,233 @@
     ax.set_xlabel(xlabel)
     if ylabel is None:
         ylabel = metric.upper()
     ax.set_ylabel(ylabel)
 
     save_plot(fig, ax, save)
 
-    if return_fig and ax is None:
+    if return_fig:
+        return fig
+
+
+def plot_psbulk_samples(adata, groupby, figsize=(5, 5), dpi=100, ax=None, return_fig=False, save=None, **kwargs):
+    """
+    Quality Control plot to assess the quality of the obtained pseudobulk samples.
+
+    Parameters
+    ----------
+    adata : AnnData
+        AnnData obtained after running ``decoupler.get_pseudobulk``.
+    groupby : str, list
+        Name of the ``.obs`` column to group by. Can also be a list of columns.
+    figsize : tuple
+        Figure size.
+    dpi : int
+        DPI resolution of figure.
+    ax : Axes, None
+        A matplotlib axes object. If None returns new figure.
+    return_fig : bool
+        Whether to return a Figure object or not.
+    save : str, None
+        Path to where to save the plot. Infer the filetype if ending on {`.pdf`, `.png`, `.svg`}.
+    kwargs : dict
+        Other keyword arguments are passed through to seaborn.scatterplot().
+
+    Returns
+    -------
+    fig : Figure, None
+        If return_fig, returns Figure object.
+    """
+    # Load plotting packages
+    sns = check_if_seaborn()
+    plt = check_if_matplotlib()
+
+    # Extract obs
+    df = adata.obs.copy()
+
+    # Transform to log10
+    df['psbulk_n_cells'] = np.log10(df['psbulk_n_cells'])
+    df['psbulk_counts'] = np.log10(df['psbulk_counts'])
+
+    if type(groupby) is list and ax is not None:
+        raise ValueError("""If a grupby is a list of columns ax must be None.""")
+    elif type(groupby) is list:
+        fig, axes = plt.subplots(1, len(groupby), figsize=figsize, dpi=dpi, tight_layout=True)
+        axes = axes.ravel()
+        for ax, grp in zip(axes, groupby):
+            ax.grid(zorder=0)
+            sns.scatterplot(x='psbulk_n_cells', y='psbulk_counts', hue=grp, ax=ax, data=df, zorder=1, **kwargs)
+            ax.legend(loc='center left', bbox_to_anchor=(1, 0.5), frameon=False, title=grp)
+            ax.set_xlabel('Log10 number of cells')
+            ax.set_ylabel('Log10 total sum of counts')
+    else:
+        # Plot
+        fig = None
+        if ax is None:
+            fig, ax = plt.subplots(1, 1, figsize=figsize, dpi=dpi)
+        ax.grid(zorder=0)
+        sns.scatterplot(x='psbulk_n_cells', y='psbulk_counts', hue=groupby, ax=ax, data=df, zorder=1, **kwargs)
+        ax.legend(loc='center left', bbox_to_anchor=(1, 0.5), frameon=False, title=groupby)
+        ax.set_xlabel('Log10 number of cells')
+        ax.set_ylabel('Log10 total sum of counts')
+
+    save_plot(fig, ax, save)
+
+    if return_fig:
+        return fig
+
+
+def plot_filter_by_expr(adata, obs=None, group=None, lib_size=None, min_count=10, min_total_count=15, large_n=10,
+                        min_prop=0.7, cmap='viridis', figsize=(5, 4), dpi=100, ax=None, return_fig=False, save=None, **kwargs):
+    """
+    Plot to help determining the thresholds of the ``decoupler.filter_by_expr`` function.
+
+    Parameters
+    ----------
+    adata : AnnData
+        AnnData obtained after running ``decoupler.get_pseudobulk``.
+    obs : DataFrame, None
+        If provided, metadata dataframe, only needed if ``adata`` is not an ``AnnData``.
+    group : str, None
+        Name of the ``.obs`` column to group by. If None, it assumes that all samples belong to one group.
+    lib_size : int, float, None
+        Library size. If None, default to the sum of reads per sample.
+    min_count : int
+        Minimum count requiered per gene for at least some samples.
+    min_total_count : int
+        Minimum total count required per gene across all samples.
+    large_n : int
+        Number of samples per group that is considered to be "large".
+    min_prop : float
+        Minimum proportion of samples in the smallest group that express the gene.
+    cmap : str
+        Colormap to use.
+    figsize : tuple
+        Figure size.
+    dpi : int
+        DPI resolution of figure.
+    ax : Axes, None
+        A matplotlib axes object. If None returns new figure.
+    return_fig : bool
+        Whether to return a Figure object or not.
+    save : str, None
+        Path to where to save the plot. Infer the filetype if ending on {`.pdf`, `.png`, `.svg`}.
+    kwargs : dict
+        Other keyword arguments are passed through to ``sns.histplot``.
+
+    Returns
+    -------
+    fig : Figure, None
+        If return_fig, returns Figure object.
+    """
+    # Load plotting packages
+    sns = check_if_seaborn()
+    plt = check_if_matplotlib()
+
+    # Extract inputs
+    y, obs, var_names = get_filterbyexpr_inputs(adata, obs)
+
+    # Compute lib_size if needed
+    if lib_size is None:
+        lib_size = np.sum(y, axis=1)
+
+    # Minimum sample size cutoff
+    min_sample_size = get_min_sample_size(group, obs, large_n, min_prop)
+    min_sample_size -= 1e-14
+
+    # Total count cutoff
+    min_total_count -= 1e-14
+
+    # CPM cutoff
+    cpm_cutoff = get_cpm_cutoff(lib_size, min_count)
+
+    # CPM thr
+    cpm = get_cpm(y, lib_size)
+    sample_size = np.sum(cpm >= cpm_cutoff, axis=0)
+
+    # Total counts
+    total_counts = np.sum(y, axis=0)
+    total_counts[total_counts < 1.] = np.nan  # Handle 0s
+
+    # Plot
+    fig = None
+    if ax is None:
+        fig, ax = plt.subplots(1, 1, figsize=figsize, dpi=dpi)
+    sns.histplot(x=np.log10(total_counts), y=sample_size, cmap=cmap, cbar=True,
+                 cbar_kws=dict(shrink=.75, label='Number of features'),
+                 discrete=(False, True), ax=ax, **kwargs)
+    ax.axhline(y=min_sample_size - 0.5, c='gray', ls='--')
+    ax.axvline(x=np.log10(min_total_count), c='gray', ls='--')
+    ax.set_xlabel('Log10 total sum of counts')
+    ax.set_ylabel('Number of samples')
+
+    save_plot(fig, ax, save)
+
+    if return_fig:
         return fig
+
+
+def plot_filter_by_prop(adata, min_prop=0.2, min_smpls=2, cmap='viridis', figsize=(5, 4),
+                        dpi=100, ax=None, return_fig=False, save=None, **kwargs):
+    """
+    Plot to help determining the thresholds of the ``decoupler.filter_by_expr`` function.
+
+    Parameters
+    ----------
+    adata : AnnData
+        AnnData obtained after running ``decoupler.get_pseudobulk``. It requieres ``.layer['psbulk_props']``.
+    min_prop : float
+        Minimum proportion of cells that express a gene in a sample.
+    min_smpls : int
+        Minimum number of samples with bigger or equal proportion of cells with expression than ``min_prop``.
+    cmap : str
+        Colormap to use.
+    figsize : tuple
+        Figure size.
+    dpi : int
+        DPI resolution of figure.
+    ax : Axes, None
+        A matplotlib axes object. If None returns new figure.
+    return_fig : bool
+        Whether to return a Figure object or not.
+    save : str, None
+        Path to where to save the plot. Infer the filetype if ending on {`.pdf`, `.png`, `.svg`}.
+    kwargs : dict
+        Other keyword arguments are passed through to ``matplotlib.pyplot.hist``.
+
+    Returns
+    -------
+    fig : Figure, None
+        If return_fig, returns Figure object.
+    """
+    # Load plotting packages
+    plt = check_if_matplotlib()
+    msg = """adata must be an AnnData object that contains the layer 'psbulk_props'. Please check the
+            function decoupler.get_pseudobulk."""
+
+    if isinstance(adata, AnnData):
+        layer_keys = adata.layers.keys()
+        if 'psbulk_props' in list(layer_keys):
+            props = adata.layers['psbulk_props']
+            if isinstance(props, pd.DataFrame):
+                props = props.values
+        else:
+            raise ValueError(msg)
+
+        # Compute nsamples by minprop
+        nsmpls = np.sum(props >= min_prop, axis=0)
+
+        # Plot
+        fig = None
+        if ax is None:
+            fig, ax = plt.subplots(1, 1, figsize=figsize, dpi=dpi)
+        _ = ax.hist(nsmpls, log=True, color='gray', **kwargs)
+        ax.axvline(x=min_smpls, c='black', ls='--')
+        ax.set_xlabel('Number of samples where >= min_prop')
+        ax.set_ylabel('Number of genes')
+
+        save_plot(fig, ax, save)
+
+        if return_fig:
+            return fig
+    else:
+        raise ValueError(msg)
```

### Comparing `decoupler-1.3.4/decoupler/pre.py` & `decoupler-1.4.0/decoupler/pre.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/utils.py` & `decoupler-1.4.0/decoupler/utils.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler/utils_benchmark.py` & `decoupler-1.4.0/decoupler/utils_benchmark.py`

 * *Files identical despite different names*

### Comparing `decoupler-1.3.4/decoupler.egg-info/PKG-INFO` & `decoupler-1.4.0/decoupler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoupler
-Version: 1.3.4
+Version: 1.4.0
 Summary: Ensemble of methods to infer biological activities from omics data
 Home-page: https://github.com/saezlab/decoupler-py
 Author: Pau Badia i Mompel
 Author-email: pau.badia@uni-heidelberg.de
 Project-URL: Bug Tracker, https://github.com/saezlab/decoupler-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `decoupler-1.3.4/setup.py` & `decoupler-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="decoupler",
-    version="1.3.4",
+    version="1.4.0",
     author="Pau Badia i Mompel",
     author_email="pau.badia@uni-heidelberg.de",
     description="Ensemble of methods to infer biological activities from omics data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/saezlab/decoupler-py",
     project_urls={
```

