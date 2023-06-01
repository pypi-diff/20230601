# Comparing `tmp/pami-2023.3.1.tar.gz` & `tmp/pami-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2023.3.1.tar", last modified: Mon Apr  3 12:14:38 2023, max compression
+gzip compressed data, was "pami-2023.4.1.tar", last modified: Thu Jun  1 12:58:36 2023, max compression
```

## Comparing `pami-2023.3.1.tar` & `pami-2023.4.1.tar`

### file list

```diff
@@ -1,398 +1,401 @@
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.452167 pami-2023.3.1/
--rw-r--r--   0 likhitha   (505) staff       (20)    35149 2022-05-26 01:58:44.000000 pami-2023.3.1/LICENSE
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.138535 pami-2023.3.1/PAMI/
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.138728 pami-2023.3.1/PAMI/AssociationRules/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/AssociationRules/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.139369 pami-2023.3.1/PAMI/AssociationRules/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    12384 2022-10-26 03:59:07.000000 pami-2023.3.1/PAMI/AssociationRules/basic/RuleMiner.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-20 06:22:26.000000 pami-2023.3.1/PAMI/AssociationRules/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6588 2022-09-20 06:22:27.000000 pami-2023.3.1/PAMI/AssociationRules/basic/abstract.py
--rw-r--r--   0 likhitha   (505) staff       (20)      139 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.144380 pami-2023.3.1/PAMI/correlatedPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/correlatedPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.146188 pami-2023.3.1/PAMI/correlatedPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    25349 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/correlatedPattern/basic/CPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)    26794 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/correlatedPattern/basic/CPGrowthPlus.py
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/correlatedPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6055 2022-09-13 03:26:07.000000 pami-2023.3.1/PAMI/correlatedPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.146441 pami-2023.3.1/PAMI/coveragePatterns/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-06-30 05:11:02.000000 pami-2023.3.1/PAMI/coveragePatterns/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.147854 pami-2023.3.1/PAMI/coveragePatterns/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    13144 2022-09-20 06:22:26.000000 pami-2023.3.1/PAMI/coveragePatterns/basic/CMine.py
--rw-r--r--   0 likhitha   (505) staff       (20)    16908 2022-09-20 06:22:26.000000 pami-2023.3.1/PAMI/coveragePatterns/basic/CPPG.py
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-09-12 09:34:32.000000 pami-2023.3.1/PAMI/coveragePatterns/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6938 2022-09-13 03:26:08.000000 pami-2023.3.1/PAMI/coveragePatterns/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.164190 pami-2023.3.1/PAMI/extras/
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.166688 pami-2023.3.1/PAMI/extras/DF2DB/
--rw-r--r--   0 likhitha   (505) staff       (20)     2517 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/extras/DF2DB/DF2DB.py
--rw-r--r--   0 likhitha   (505) staff       (20)     2418 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/extras/DF2DB/DF2DBPlus.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/extras/DF2DB/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     1629 2022-09-13 03:26:08.000000 pami-2023.3.1/PAMI/extras/DF2DB/createTDB.py
--rw-r--r--   0 likhitha   (505) staff       (20)    10138 2023-01-08 10:45:15.000000 pami-2023.3.1/PAMI/extras/DF2DB/denseDF2DB.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5354 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
--rw-r--r--   0 likhitha   (505) staff       (20)     3822 2023-01-08 10:45:15.000000 pami-2023.3.1/PAMI/extras/DF2DB/sparseDF2DB.py
--rw-r--r--   0 likhitha   (505) staff       (20)     3503 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/extras/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.171175 pami-2023.3.1/PAMI/extras/calculateMISValues/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-07-01 00:24:16.000000 pami-2023.3.1/PAMI/extras/calculateMISValues/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     3741 2022-09-13 03:26:07.000000 pami-2023.3.1/PAMI/extras/calculateMISValues/usingBeta.py
--rw-r--r--   0 likhitha   (505) staff       (20)     3794 2022-09-13 03:26:07.000000 pami-2023.3.1/PAMI/extras/calculateMISValues/usingSD.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.174155 pami-2023.3.1/PAMI/extras/dbStats/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/extras/dbStats/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)    13000 2022-09-10 01:57:05.000000 pami-2023.3.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py
--rw-r--r--   0 likhitha   (505) staff       (20)    14610 2022-09-10 01:57:05.000000 pami-2023.3.1/PAMI/extras/dbStats/temporalDatabaseStats.py
--rw-r--r--   0 likhitha   (505) staff       (20)    10399 2022-09-10 01:57:05.000000 pami-2023.3.1/PAMI/extras/dbStats/transactionalDatabaseStats.py
--rw-r--r--   0 likhitha   (505) staff       (20)    13209 2023-01-08 10:45:15.000000 pami-2023.3.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
--rw-r--r--   0 likhitha   (505) staff       (20)     9982 2022-10-03 04:23:08.000000 pami-2023.3.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
--rw-r--r--   0 likhitha   (505) staff       (20)    12903 2022-09-10 01:57:05.000000 pami-2023.3.1/PAMI/extras/dbStats/utilityDatabaseStats.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.183209 pami-2023.3.1/PAMI/extras/fuzzyTransformation/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-03-01 01:58:12.000000 pami-2023.3.1/PAMI/extras/fuzzyTransformation/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5195 2023-03-01 01:58:42.000000 pami-2023.3.1/PAMI/extras/fuzzyTransformation/abstract.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5925 2023-03-01 02:03:56.000000 pami-2023.3.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5919 2023-03-21 05:53:43.000000 pami-2023.3.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5803 2023-03-21 05:53:43.000000 pami-2023.3.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.184188 pami-2023.3.1/PAMI/extras/generateDatabase/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/extras/generateDatabase/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     2877 2022-06-10 00:52:41.000000 pami-2023.3.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
--rw-r--r--   0 likhitha   (505) staff       (20)     7069 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
--rw-r--r--   0 likhitha   (505) staff       (20)     3399 2022-05-30 08:10:33.000000 pami-2023.3.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
--rw-r--r--   0 likhitha   (505) staff       (20)     3593 2022-06-20 05:11:46.000000 pami-2023.3.1/PAMI/extras/generateLatexGraphFile.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.185651 pami-2023.3.1/PAMI/extras/graph/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/extras/graph/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     1656 2022-06-24 01:22:27.000000 pami-2023.3.1/PAMI/extras/graph/dataFrameInToFigures.py
--rw-r--r--   0 likhitha   (505) staff       (20)     2954 2022-06-30 05:09:24.000000 pami-2023.3.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py
--rw-r--r--   0 likhitha   (505) staff       (20)     1167 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
--rw-r--r--   0 likhitha   (505) staff       (20)     1753 2022-06-20 05:11:45.000000 pami-2023.3.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
--rw-r--r--   0 likhitha   (505) staff       (20)     2203 2022-11-27 01:07:51.000000 pami-2023.3.1/PAMI/extras/graph/visualizePatterns.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.185970 pami-2023.3.1/PAMI/extras/image2Database/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-10 01:57:05.000000 pami-2023.3.1/PAMI/extras/image2Database/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.186260 pami-2023.3.1/PAMI/extras/imageProcessing/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-09-10 01:57:05.000000 pami-2023.3.1/PAMI/extras/imageProcessing/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     4582 2022-09-10 01:57:05.000000 pami-2023.3.1/PAMI/extras/imageProcessing/imagery2Databases.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.186565 pami-2023.3.1/PAMI/extras/neighbours/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/extras/neighbours/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     2834 2022-09-10 01:57:05.000000 pami-2023.3.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
--rw-r--r--   0 likhitha   (505) staff       (20)     3031 2022-07-28 04:00:44.000000 pami-2023.3.1/PAMI/extras/plotPointOnMap.py
--rw-r--r--   0 likhitha   (505) staff       (20)     3214 2022-07-28 04:00:44.000000 pami-2023.3.1/PAMI/extras/plotPointOnMap_dump.py
--rw-r--r--   0 likhitha   (505) staff       (20)     2178 2022-05-30 08:10:33.000000 pami-2023.3.1/PAMI/extras/scatterPlotSpatialPoints.py
--rw-r--r--   0 likhitha   (505) staff       (20)     1827 2022-09-13 03:26:07.000000 pami-2023.3.1/PAMI/extras/topKPatterns.py
--rw-r--r--   0 likhitha   (505) staff       (20)      473 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/extras/uncertaindb_convert.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.186735 pami-2023.3.1/PAMI/faultTolerantFrequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/faultTolerantFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.188778 pami-2023.3.1/PAMI/faultTolerantFrequentPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    15077 2023-03-21 06:08:32.000000 pami-2023.3.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
--rw-r--r--   0 likhitha   (505) staff       (20)    20676 2023-03-21 05:53:43.000000 pami-2023.3.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)    15543 2023-03-21 06:09:18.000000 pami-2023.3.1/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-09-10 01:57:05.000000 pami-2023.3.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6691 2022-09-16 08:22:43.000000 pami-2023.3.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.189491 pami-2023.3.1/PAMI/faultTolerantFrequentPattern/maximal/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-16 09:02:29.000000 pami-2023.3.1/PAMI/faultTolerantFrequentPattern/maximal/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6645 2022-09-22 03:52:49.000000 pami-2023.3.1/PAMI/faultTolerantFrequentPattern/maximal/abstract.py
--rw-r--r--   0 likhitha   (505) staff       (20)    11948 2022-09-22 04:41:50.000000 pami-2023.3.1/PAMI/faultTolerantFrequentPattern/maximal/maxFTP.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.189842 pami-2023.3.1/PAMI/frequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/frequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.193364 pami-2023.3.1/PAMI/frequentPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    13475 2022-09-13 07:44:04.000000 pami-2023.3.1/PAMI/frequentPattern/basic/Apriori.py
--rw-r--r--   0 likhitha   (505) staff       (20)    13441 2022-09-13 07:44:04.000000 pami-2023.3.1/PAMI/frequentPattern/basic/ECLAT.py
--rw-r--r--   0 likhitha   (505) staff       (20)    13207 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/frequentPattern/basic/ECLATDiffset.py
--rw-r--r--   0 likhitha   (505) staff       (20)    12389 2022-09-13 07:44:04.000000 pami-2023.3.1/PAMI/frequentPattern/basic/ECLATbitset.py
--rw-r--r--   0 likhitha   (505) staff       (20)    20353 2022-09-22 03:48:55.000000 pami-2023.3.1/PAMI/frequentPattern/basic/FPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/frequentPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     7733 2022-09-13 03:26:07.000000 pami-2023.3.1/PAMI/frequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.194306 pami-2023.3.1/PAMI/frequentPattern/closed/
--rw-r--r--   0 likhitha   (505) staff       (20)    20234 2022-09-13 07:44:04.000000 pami-2023.3.1/PAMI/frequentPattern/closed/CHARM.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/frequentPattern/closed/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6445 2022-09-13 03:26:07.000000 pami-2023.3.1/PAMI/frequentPattern/closed/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.195212 pami-2023.3.1/PAMI/frequentPattern/cuda/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/frequentPattern/cuda/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5003 2022-09-12 05:08:17.000000 pami-2023.3.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
--rw-r--r--   0 likhitha   (505) staff       (20)     7921 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
--rw-r--r--   0 likhitha   (505) staff       (20)     4839 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.197973 pami-2023.3.1/PAMI/frequentPattern/maximal/
--rw-r--r--   0 likhitha   (505) staff       (20)    25382 2023-02-07 05:06:18.000000 pami-2023.3.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/frequentPattern/maximal/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6436 2022-10-26 03:59:07.000000 pami-2023.3.1/PAMI/frequentPattern/maximal/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.199390 pami-2023.3.1/PAMI/frequentPattern/pyspark/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/frequentPattern/pyspark/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5603 2022-09-13 03:26:08.000000 pami-2023.3.1/PAMI/frequentPattern/pyspark/abstract.py
--rw-r--r--   0 likhitha   (505) staff       (20)    12024 2022-09-13 07:46:37.000000 pami-2023.3.1/PAMI/frequentPattern/pyspark/parallelApriori.py
--rw-r--r--   0 likhitha   (505) staff       (20)    10490 2022-09-13 07:50:03.000000 pami-2023.3.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
--rw-r--r--   0 likhitha   (505) staff       (20)    15608 2022-09-13 07:50:03.000000 pami-2023.3.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.200172 pami-2023.3.1/PAMI/frequentPattern/topk/
--rw-r--r--   0 likhitha   (505) staff       (20)    15148 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/frequentPattern/topk/FAE.py
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/frequentPattern/topk/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     4575 2022-09-12 06:50:04.000000 pami-2023.3.1/PAMI/frequentPattern/topk/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.200463 pami-2023.3.1/PAMI/frequentSpatialPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/frequentSpatialPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.203390 pami-2023.3.1/PAMI/frequentSpatialPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    18316 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/frequentSpatialPattern/basic/FSPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)    17714 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/frequentSpatialPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6680 2022-09-13 03:26:08.000000 pami-2023.3.1/PAMI/frequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.203828 pami-2023.3.1/PAMI/fuzzyCorrelatedPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/fuzzyCorrelatedPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.206626 pami-2023.3.1/PAMI/fuzzyCorrelatedPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    26118 2022-09-20 06:22:26.000000 pami-2023.3.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6635 2022-09-13 08:04:20.000000 pami-2023.3.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.206992 pami-2023.3.1/PAMI/fuzzyFrequentPatterns/
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/fuzzyFrequentPatterns/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.210043 pami-2023.3.1/PAMI/fuzzyFrequentPatterns/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    20926 2023-03-02 03:15:52.000000 pami-2023.3.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py
--rw-r--r--   0 likhitha   (505) staff       (20)    26037 2023-03-01 01:53:49.000000 pami-2023.3.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/fuzzyFrequentPatterns/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6450 2023-03-01 02:51:05.000000 pami-2023.3.1/PAMI/fuzzyFrequentPatterns/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.210378 pami-2023.3.1/PAMI/fuzzyFrequentSpatialPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/fuzzyFrequentSpatialPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.212055 pami-2023.3.1/PAMI/fuzzyFrequentSpatialPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    24222 2023-03-02 04:09:41.000000 pami-2023.3.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
--rw-r--r--   0 likhitha   (505) staff       (20)    26791 2023-03-01 01:58:20.000000 pami-2023.3.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6580 2022-09-13 03:26:08.000000 pami-2023.3.1/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.212369 pami-2023.3.1/PAMI/fuzzyPeriodicFrequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.214015 pami-2023.3.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    22613 2023-03-21 05:53:43.000000 pami-2023.3.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
--rw-r--r--   0 likhitha   (505) staff       (20)    25345 2023-03-01 01:58:20.000000 pami-2023.3.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6668 2022-09-13 03:26:08.000000 pami-2023.3.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.214315 pami-2023.3.1/PAMI/fuzzySpatialPeriodicFrequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.215486 pami-2023.3.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    27112 2023-03-21 05:53:43.000000 pami-2023.3.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
--rw-r--r--   0 likhitha   (505) staff       (20)    32216 2023-03-01 01:58:20.000000 pami-2023.3.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-16 08:22:43.000000 pami-2023.3.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6618 2023-03-21 05:53:43.000000 pami-2023.3.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.221641 pami-2023.3.1/PAMI/geoReferencedFrequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)    27548 2023-04-03 08:12:11.000000 pami-2023.3.1/PAMI/geoReferencedFrequentPattern/GFPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-04-03 08:12:11.000000 pami-2023.3.1/PAMI/geoReferencedFrequentPattern/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5007 2023-04-03 08:12:11.000000 pami-2023.3.1/PAMI/geoReferencedFrequentPattern/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.222006 pami-2023.3.1/PAMI/geoReferencedPeriodicFrequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-09-10 01:57:05.000000 pami-2023.3.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.222911 pami-2023.3.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    18686 2023-01-08 10:45:15.000000 pami-2023.3.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-12 13:22:01.000000 pami-2023.3.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6774 2022-09-13 03:26:08.000000 pami-2023.3.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.223230 pami-2023.3.1/PAMI/highUtilityFrequentPatterns/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/highUtilityFrequentPatterns/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.224902 pami-2023.3.1/PAMI/highUtilityFrequentPatterns/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    35252 2023-02-07 03:37:24.000000 pami-2023.3.1/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/highUtilityFrequentPatterns/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6081 2022-09-13 03:26:08.000000 pami-2023.3.1/PAMI/highUtilityFrequentPatterns/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.226127 pami-2023.3.1/PAMI/highUtilityFrequentSpatialPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/highUtilityFrequentSpatialPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.227949 pami-2023.3.1/PAMI/highUtilityFrequentSpatialPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    38373 2022-09-15 06:00:15.000000 pami-2023.3.1/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6181 2022-09-13 03:26:07.000000 pami-2023.3.1/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.228334 pami-2023.3.1/PAMI/highUtilityPatterns/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/highUtilityPatterns/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.230437 pami-2023.3.1/PAMI/highUtilityPatterns/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    31875 2023-02-07 03:55:11.000000 pami-2023.3.1/PAMI/highUtilityPatterns/basic/EFIM.py
--rw-r--r--   0 likhitha   (505) staff       (20)    23450 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/highUtilityPatterns/basic/HMiner.py
--rw-r--r--   0 likhitha   (505) staff       (20)    25807 2023-02-07 03:54:20.000000 pami-2023.3.1/PAMI/highUtilityPatterns/basic/UPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/highUtilityPatterns/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5053 2022-09-13 03:26:07.000000 pami-2023.3.1/PAMI/highUtilityPatterns/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.231020 pami-2023.3.1/PAMI/highUtilitySpatialPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/highUtilitySpatialPattern/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6718 2022-09-13 03:26:07.000000 pami-2023.3.1/PAMI/highUtilitySpatialPattern/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.232726 pami-2023.3.1/PAMI/highUtilitySpatialPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    25729 2023-02-07 04:08:34.000000 pami-2023.3.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
--rw-r--r--   0 likhitha   (505) staff       (20)    32747 2023-02-04 06:23:46.000000 pami-2023.3.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5955 2022-09-13 03:26:06.000000 pami-2023.3.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.233782 pami-2023.3.1/PAMI/highUtilitySpatialPattern/topk/
--rw-r--r--   0 likhitha   (505) staff       (20)    33511 2023-02-07 04:26:57.000000 pami-2023.3.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6625 2023-02-07 04:28:07.000000 pami-2023.3.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.234127 pami-2023.3.1/PAMI/localPeriodicPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/localPeriodicPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.235667 pami-2023.3.1/PAMI/localPeriodicPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    30377 2022-09-15 07:36:55.000000 pami-2023.3.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)    19626 2022-09-15 07:36:55.000000 pami-2023.3.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
--rw-r--r--   0 likhitha   (505) staff       (20)    18711 2022-09-15 07:36:55.000000 pami-2023.3.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/localPeriodicPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     8378 2022-09-15 07:26:35.000000 pami-2023.3.1/PAMI/localPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.235975 pami-2023.3.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-06-21 09:08:43.000000 pami-2023.3.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.239382 pami-2023.3.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    22172 2023-03-21 05:53:43.000000 pami-2023.3.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)    21275 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-12 07:16:58.000000 pami-2023.3.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5913 2022-09-13 03:26:08.000000 pami-2023.3.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.240152 pami-2023.3.1/PAMI/partialPeriodicFrequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/partialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.241547 pami-2023.3.1/PAMI/partialPeriodicFrequentPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    25450 2022-10-12 03:45:33.000000 pami-2023.3.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)    19431 2022-10-12 03:52:53.000000 pami-2023.3.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5392 2022-09-13 07:44:04.000000 pami-2023.3.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.242223 pami-2023.3.1/PAMI/partialPeriodicPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.244898 pami-2023.3.1/PAMI/partialPeriodicPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    49814 2023-03-02 08:48:22.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)     4195 2022-09-13 03:26:07.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
--rw-r--r--   0 likhitha   (505) staff       (20)    23287 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)    16900 2023-03-31 03:36:16.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5572 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.246153 pami-2023.3.1/PAMI/partialPeriodicPattern/closed/
--rw-r--r--   0 likhitha   (505) staff       (20)    19695 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/closed/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5595 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/closed/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.248905 pami-2023.3.1/PAMI/partialPeriodicPattern/maximal/
--rw-r--r--   0 likhitha   (505) staff       (20)    27900 2022-10-12 03:35:13.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/maximal/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     4261 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/maximal/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.250646 pami-2023.3.1/PAMI/partialPeriodicPattern/timeSeries/
--rw-r--r--   0 likhitha   (505) staff       (20)    25314 2022-09-13 07:44:04.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-08-02 07:47:39.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/timeSeries/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     5550 2022-09-13 07:44:04.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/timeSeries/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.251826 pami-2023.3.1/PAMI/partialPeriodicPattern/topk/
--rw-r--r--   0 likhitha   (505) staff       (20)    16925 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/topk/Topk_PPPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/topk/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     7837 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/partialPeriodicPattern/topk/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.252102 pami-2023.3.1/PAMI/partialPeriodicSpatialPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-06-28 05:26:47.000000 pami-2023.3.1/PAMI/partialPeriodicSpatialPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.253006 pami-2023.3.1/PAMI/partialPeriodicSpatialPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    18201 2022-09-16 08:22:43.000000 pami-2023.3.1/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-16 08:22:43.000000 pami-2023.3.1/PAMI/partialPeriodicSpatialPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6165 2022-09-16 08:22:40.000000 pami-2023.3.1/PAMI/partialPeriodicSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.253215 pami-2023.3.1/PAMI/periodicCorrelatedPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/periodicCorrelatedPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.254260 pami-2023.3.1/PAMI/periodicCorrelatedPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    26674 2022-09-16 08:22:43.000000 pami-2023.3.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-16 08:22:43.000000 pami-2023.3.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6652 2022-09-16 08:22:40.000000 pami-2023.3.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.254419 pami-2023.3.1/PAMI/periodicFrequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.256979 pami-2023.3.1/PAMI/periodicFrequentPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    14837 2022-09-13 07:43:58.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
--rw-r--r--   0 likhitha   (505) staff       (20)    24398 2022-09-13 07:43:58.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)    24123 2022-09-13 07:43:58.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
--rw-r--r--   0 likhitha   (505) staff       (20)    15529 2022-09-13 07:43:58.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
--rw-r--r--   0 likhitha   (505) staff       (20)    32465 2022-09-13 07:43:58.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)      726 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6525 2022-09-15 07:15:16.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.257804 pami-2023.3.1/PAMI/periodicFrequentPattern/closed/
--rw-r--r--   0 likhitha   (505) staff       (20)    19782 2022-09-13 07:43:58.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/closed/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6538 2022-09-13 03:26:08.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/closed/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.258370 pami-2023.3.1/PAMI/periodicFrequentPattern/cuda/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-02-11 00:26:28.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/cuda/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)    16537 2023-02-11 00:26:28.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.260046 pami-2023.3.1/PAMI/periodicFrequentPattern/maximal/
--rw-r--r--   0 likhitha   (505) staff       (20)    27844 2023-02-07 05:06:18.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/maximal/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     7873 2022-09-13 03:26:08.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/maximal/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.260303 pami-2023.3.1/PAMI/periodicFrequentPattern/topk/
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.261250 pami-2023.3.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
--rw-r--r--   0 likhitha   (505) staff       (20)    17228 2023-02-07 01:47:35.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-02-07 01:47:35.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6898 2023-02-07 01:47:35.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/topk/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.261942 pami-2023.3.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-02-07 01:52:08.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     4583 2023-02-07 01:49:30.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
--rw-r--r--   0 likhitha   (505) staff       (20)    16401 2023-02-07 01:56:38.000000 pami-2023.3.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.262360 pami-2023.3.1/PAMI/recurringPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/recurringPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.263258 pami-2023.3.1/PAMI/recurringPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    25551 2023-02-11 00:45:20.000000 pami-2023.3.1/PAMI/recurringPattern/basic/RPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/recurringPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6632 2022-09-13 07:44:04.000000 pami-2023.3.1/PAMI/recurringPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.263557 pami-2023.3.1/PAMI/relativeFrequentPatterns/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/relativeFrequentPatterns/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.265009 pami-2023.3.1/PAMI/relativeFrequentPatterns/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    25500 2022-09-20 08:51:48.000000 pami-2023.3.1/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/relativeFrequentPatterns/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     4261 2022-09-20 08:51:48.000000 pami-2023.3.1/PAMI/relativeFrequentPatterns/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.265272 pami-2023.3.1/PAMI/relativeHighUtilityPatterns/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/relativeHighUtilityPatterns/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.266480 pami-2023.3.1/PAMI/relativeHighUtilityPatterns/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    32789 2023-02-09 04:36:40.000000 pami-2023.3.1/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/relativeHighUtilityPatterns/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     7391 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/relativeHighUtilityPatterns/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.266757 pami-2023.3.1/PAMI/sequentialPatternMining/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/sequentialPatternMining/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.268416 pami-2023.3.1/PAMI/sequentialPatternMining/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    40559 2023-02-28 05:51:58.000000 pami-2023.3.1/PAMI/sequentialPatternMining/basic/SPADE.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-21 04:49:06.000000 pami-2023.3.1/PAMI/sequentialPatternMining/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6554 2023-01-08 10:45:15.000000 pami-2023.3.1/PAMI/sequentialPatternMining/basic/abstract.py
--rw-r--r--   0 likhitha   (505) staff       (20)    22030 2023-02-11 00:26:28.000000 pami-2023.3.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.269283 pami-2023.3.1/PAMI/sequentialPatternMining/closed/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-21 04:50:02.000000 pami-2023.3.1/PAMI/sequentialPatternMining/closed/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6279 2022-09-13 03:26:07.000000 pami-2023.3.1/PAMI/sequentialPatternMining/closed/abstract.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-21 04:50:31.000000 pami-2023.3.1/PAMI/sequentialPatternMining/closed/bide.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.269399 pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.275216 pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    15193 2022-11-21 07:50:04.000000 pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
--rw-r--r--   0 likhitha   (505) staff       (20)    24038 2022-11-21 07:17:33.000000 pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)    17918 2022-09-13 03:26:06.000000 pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-06-30 05:09:24.000000 pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     7258 2022-09-13 03:26:06.000000 pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.276431 pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/topK/
--rw-r--r--   0 likhitha   (505) staff       (20)    25615 2023-02-10 03:23:27.000000 pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     7177 2022-09-13 03:26:07.000000 pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.276695 pami-2023.3.1/PAMI/uncertainFrequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/uncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.438119 pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    24906 2022-09-13 07:44:04.000000 pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
--rw-r--r--   0 likhitha   (505) staff       (20)    25115 2023-02-28 09:14:04.000000 pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)    17825 2022-09-13 03:26:05.000000 pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
--rw-r--r--   0 likhitha   (505) staff       (20)    26168 2023-03-31 03:36:16.000000 pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
--rw-r--r--   0 likhitha   (505) staff       (20)    26931 2023-03-31 03:36:16.000000 pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
--rw-r--r--   0 likhitha   (505) staff       (20)    24582 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)    18153 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     4962 2022-09-13 07:44:04.000000 pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.438474 pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.442214 pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    30266 2023-02-07 01:21:17.000000 pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)    30696 2023-02-07 01:21:54.000000 pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6551 2022-09-13 07:44:04.000000 pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
--rw-r--r--   0 likhitha   (505) staff       (20)    30905 2022-10-03 07:07:51.000000 pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/basic/upfp.py
--rw-r--r--   0 likhitha   (505) staff       (20)    33359 2022-10-06 01:25:48.000000 pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/basic/upfpplus.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.443056 pami-2023.3.1/PAMI/uncertainProbablisticFrequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-27 07:43:30.000000 pami-2023.3.1/PAMI/uncertainProbablisticFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.443271 pami-2023.3.1/PAMI/uncertainProbablisticFrequentPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-27 07:43:44.000000 pami-2023.3.1/PAMI/uncertainProbablisticFrequentPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     4962 2022-09-27 07:44:21.000000 pami-2023.3.1/PAMI/uncertainProbablisticFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.443590 pami-2023.3.1/PAMI/weightedFrequentNeighbourhoodPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-06-28 05:36:22.000000 pami-2023.3.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.445999 pami-2023.3.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    26149 2023-02-06 08:15:48.000000 pami-2023.3.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6693 2023-02-06 08:50:12.000000 pami-2023.3.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.446439 pami-2023.3.1/PAMI/weightedFrequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/weightedFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.447923 pami-2023.3.1/PAMI/weightedFrequentPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    23009 2022-09-20 06:22:27.000000 pami-2023.3.1/PAMI/weightedFrequentPattern/basic/WFIM.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/weightedFrequentPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     6737 2022-09-13 07:44:04.000000 pami-2023.3.1/PAMI/weightedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.448517 pami-2023.3.1/PAMI/weightedFrequentRegularPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/weightedFrequentRegularPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.449487 pami-2023.3.1/PAMI/weightedFrequentRegularPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    26702 2023-02-10 03:46:01.000000 pami-2023.3.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     7555 2022-09-13 07:44:04.000000 pami-2023.3.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.449832 pami-2023.3.1/PAMI/weightedUncertainFrequentPattern/
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.3.1/PAMI/weightedUncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.450823 pami-2023.3.1/PAMI/weightedUncertainFrequentPattern/basic/
--rw-r--r--   0 likhitha   (505) staff       (20)    28437 2023-02-28 09:14:04.000000 pami-2023.3.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
--rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-13 07:44:03.000000 pami-2023.3.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 likhitha   (505) staff       (20)     4782 2023-02-10 23:22:45.000000 pami-2023.3.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
--rw-r--r--   0 likhitha   (505) staff       (20)    34388 2023-04-03 12:14:38.451961 pami-2023.3.1/PKG-INFO
--rw-r--r--   0 likhitha   (505) staff       (20)    33804 2023-03-31 03:36:16.000000 pami-2023.3.1/README.md
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-04-03 12:14:38.451678 pami-2023.3.1/pami.egg-info/
--rw-r--r--   0 likhitha   (505) staff       (20)    34388 2023-04-03 12:14:38.000000 pami-2023.3.1/pami.egg-info/PKG-INFO
--rw-r--r--   0 likhitha   (505) staff       (20)    13590 2023-04-03 12:14:38.000000 pami-2023.3.1/pami.egg-info/SOURCES.txt
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-04-03 12:14:38.000000 pami-2023.3.1/pami.egg-info/dependency_links.txt
--rw-r--r--   0 likhitha   (505) staff       (20)       75 2023-04-03 12:14:38.000000 pami-2023.3.1/pami.egg-info/requires.txt
--rw-r--r--   0 likhitha   (505) staff       (20)        5 2023-04-03 12:14:38.000000 pami-2023.3.1/pami.egg-info/top_level.txt
--rw-r--r--   0 likhitha   (505) staff       (20)       38 2023-04-03 12:14:38.452222 pami-2023.3.1/setup.cfg
--rw-r--r--   0 likhitha   (505) staff       (20)     1205 2023-04-03 08:12:11.000000 pami-2023.3.1/setup.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.389941 pami-2023.4.1/
+-rw-r--r--   0 likhitha   (505) staff       (20)    35149 2022-05-26 01:58:44.000000 pami-2023.4.1/LICENSE
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.260545 pami-2023.4.1/PAMI/
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.261036 pami-2023.4.1/PAMI/AssociationRules/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.263624 pami-2023.4.1/PAMI/AssociationRules/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)     7975 2023-05-24 23:17:26.000000 pami-2023.4.1/PAMI/AssociationRules/basic/ARWithConfidence.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     8038 2023-04-05 02:08:01.000000 pami-2023.4.1/PAMI/AssociationRules/basic/ARWithLeverage.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     8085 2023-04-05 02:08:01.000000 pami-2023.4.1/PAMI/AssociationRules/basic/ARWithLift.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    12384 2022-10-26 03:59:07.000000 pami-2023.4.1/PAMI/AssociationRules/basic/RuleMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-20 06:22:26.000000 pami-2023.4.1/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6547 2023-04-05 02:08:01.000000 pami-2023.4.1/PAMI/AssociationRules/basic/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)      139 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.263957 pami-2023.4.1/PAMI/correlatedPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.266733 pami-2023.4.1/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    25349 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/correlatedPattern/basic/CPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    26794 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/correlatedPattern/basic/CPGrowthPlus.py
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6055 2022-09-13 03:26:07.000000 pami-2023.4.1/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.267035 pami-2023.4.1/PAMI/coveragePatterns/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-06-30 05:11:02.000000 pami-2023.4.1/PAMI/coveragePatterns/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.268983 pami-2023.4.1/PAMI/coveragePatterns/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    13144 2022-09-20 06:22:26.000000 pami-2023.4.1/PAMI/coveragePatterns/basic/CMine.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    16908 2022-09-20 06:22:26.000000 pami-2023.4.1/PAMI/coveragePatterns/basic/CPPG.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-09-12 09:34:32.000000 pami-2023.4.1/PAMI/coveragePatterns/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6938 2022-09-13 03:26:08.000000 pami-2023.4.1/PAMI/coveragePatterns/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.271385 pami-2023.4.1/PAMI/extras/
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.273986 pami-2023.4.1/PAMI/extras/DF2DB/
+-rw-r--r--   0 likhitha   (505) staff       (20)     2517 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/extras/DF2DB/DF2DB.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     2418 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/extras/DF2DB/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     1629 2022-09-13 03:26:08.000000 pami-2023.4.1/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    10145 2023-06-01 12:40:35.000000 pami-2023.4.1/PAMI/extras/DF2DB/denseDF2DB.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5354 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     3822 2023-01-08 10:45:15.000000 pami-2023.4.1/PAMI/extras/DF2DB/sparseDF2DB.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     3503 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/extras/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.274692 pami-2023.4.1/PAMI/extras/calculateMISValues/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-07-01 00:24:16.000000 pami-2023.4.1/PAMI/extras/calculateMISValues/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     3741 2022-09-13 03:26:07.000000 pami-2023.4.1/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     3794 2022-09-13 03:26:07.000000 pami-2023.4.1/PAMI/extras/calculateMISValues/usingSD.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.284331 pami-2023.4.1/PAMI/extras/dbStats/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/extras/dbStats/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    13000 2022-09-10 01:57:05.000000 pami-2023.4.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    14610 2022-09-10 01:57:05.000000 pami-2023.4.1/PAMI/extras/dbStats/temporalDatabaseStats.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    10399 2022-09-10 01:57:05.000000 pami-2023.4.1/PAMI/extras/dbStats/transactionalDatabaseStats.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    13209 2023-01-08 10:45:15.000000 pami-2023.4.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     9982 2022-10-03 04:23:08.000000 pami-2023.4.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    12903 2022-09-10 01:57:05.000000 pami-2023.4.1/PAMI/extras/dbStats/utilityDatabaseStats.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.285616 pami-2023.4.1/PAMI/extras/fuzzyTransformation/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2023-03-01 01:58:12.000000 pami-2023.4.1/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5195 2023-03-01 01:58:42.000000 pami-2023.4.1/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5925 2023-03-01 02:03:56.000000 pami-2023.4.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5919 2023-03-21 05:53:43.000000 pami-2023.4.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5803 2023-03-21 05:53:43.000000 pami-2023.4.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.286693 pami-2023.4.1/PAMI/extras/generateDatabase/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/extras/generateDatabase/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     2877 2022-06-10 00:52:41.000000 pami-2023.4.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     7069 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     3399 2022-05-30 08:10:33.000000 pami-2023.4.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     3593 2022-06-20 05:11:46.000000 pami-2023.4.1/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.288578 pami-2023.4.1/PAMI/extras/graph/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     1656 2022-06-24 01:22:27.000000 pami-2023.4.1/PAMI/extras/graph/dataFrameInToFigures.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     2954 2022-06-30 05:09:24.000000 pami-2023.4.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     1167 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     1753 2022-06-20 05:11:45.000000 pami-2023.4.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     2203 2022-11-27 01:07:51.000000 pami-2023.4.1/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.288934 pami-2023.4.1/PAMI/extras/image2Database/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-10 01:57:05.000000 pami-2023.4.1/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.289221 pami-2023.4.1/PAMI/extras/imageProcessing/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-09-10 01:57:05.000000 pami-2023.4.1/PAMI/extras/imageProcessing/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     4582 2022-09-10 01:57:05.000000 pami-2023.4.1/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.289634 pami-2023.4.1/PAMI/extras/neighbours/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/extras/neighbours/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     2834 2022-09-10 01:57:05.000000 pami-2023.4.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     3031 2022-07-28 04:00:44.000000 pami-2023.4.1/PAMI/extras/plotPointOnMap.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     3214 2022-07-28 04:00:44.000000 pami-2023.4.1/PAMI/extras/plotPointOnMap_dump.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     2178 2022-05-30 08:10:33.000000 pami-2023.4.1/PAMI/extras/scatterPlotSpatialPoints.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     1827 2022-09-13 03:26:07.000000 pami-2023.4.1/PAMI/extras/topKPatterns.py
+-rw-r--r--   0 likhitha   (505) staff       (20)      473 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.289816 pami-2023.4.1/PAMI/faultTolerantFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.291501 pami-2023.4.1/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    15077 2023-04-05 02:08:01.000000 pami-2023.4.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    20676 2023-03-21 05:53:43.000000 pami-2023.4.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    15543 2023-04-05 02:08:01.000000 pami-2023.4.1/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-09-10 01:57:05.000000 pami-2023.4.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6691 2022-09-16 08:22:43.000000 pami-2023.4.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.292431 pami-2023.4.1/PAMI/faultTolerantFrequentPattern/maximal/
+-rw-r--r--   0 likhitha   (505) staff       (20)     1173 2023-06-01 12:40:35.000000 pami-2023.4.1/PAMI/faultTolerantFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6645 2022-09-22 03:52:49.000000 pami-2023.4.1/PAMI/faultTolerantFrequentPattern/maximal/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    11948 2022-09-22 04:41:50.000000 pami-2023.4.1/PAMI/faultTolerantFrequentPattern/maximal/maxFTP.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.292706 pami-2023.4.1/PAMI/frequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.295626 pami-2023.4.1/PAMI/frequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    13475 2022-09-13 07:44:04.000000 pami-2023.4.1/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    13441 2022-09-13 07:44:04.000000 pami-2023.4.1/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    13555 2023-05-26 00:41:32.000000 pami-2023.4.1/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    12389 2022-09-13 07:44:04.000000 pami-2023.4.1/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    20353 2022-09-22 03:48:55.000000 pami-2023.4.1/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/frequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     7733 2022-09-13 03:26:07.000000 pami-2023.4.1/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.296616 pami-2023.4.1/PAMI/frequentPattern/closed/
+-rw-r--r--   0 likhitha   (505) staff       (20)    20234 2022-09-13 07:44:04.000000 pami-2023.4.1/PAMI/frequentPattern/closed/CHARM.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/frequentPattern/closed/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6445 2022-09-13 03:26:07.000000 pami-2023.4.1/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.297581 pami-2023.4.1/PAMI/frequentPattern/cuda/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5003 2022-09-12 05:08:17.000000 pami-2023.4.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     7921 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     4839 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.298489 pami-2023.4.1/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 likhitha   (505) staff       (20)    25382 2023-02-07 05:06:18.000000 pami-2023.4.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/frequentPattern/maximal/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6436 2022-10-26 03:59:07.000000 pami-2023.4.1/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.299962 pami-2023.4.1/PAMI/frequentPattern/pyspark/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5603 2022-09-13 03:26:08.000000 pami-2023.4.1/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    12024 2022-09-13 07:46:37.000000 pami-2023.4.1/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    10490 2022-09-13 07:50:03.000000 pami-2023.4.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    15608 2022-09-13 07:50:03.000000 pami-2023.4.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.300902 pami-2023.4.1/PAMI/frequentPattern/topk/
+-rw-r--r--   0 likhitha   (505) staff       (20)    15148 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/frequentPattern/topk/FAE.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/frequentPattern/topk/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     4575 2022-09-12 06:50:04.000000 pami-2023.4.1/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.301215 pami-2023.4.1/PAMI/frequentSpatialPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/frequentSpatialPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.303363 pami-2023.4.1/PAMI/frequentSpatialPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    18316 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/frequentSpatialPattern/basic/FSPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    17714 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/frequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6680 2022-09-13 03:26:08.000000 pami-2023.4.1/PAMI/frequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.303821 pami-2023.4.1/PAMI/fuzzyCorrelatedPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.304595 pami-2023.4.1/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    26118 2022-09-20 06:22:26.000000 pami-2023.4.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6635 2022-09-13 08:04:20.000000 pami-2023.4.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.304922 pami-2023.4.1/PAMI/fuzzyFrequentPatterns/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/fuzzyFrequentPatterns/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.307146 pami-2023.4.1/PAMI/fuzzyFrequentPatterns/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    20926 2023-03-02 03:15:52.000000 pami-2023.4.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    26037 2023-03-01 01:53:49.000000 pami-2023.4.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/fuzzyFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6450 2023-03-01 02:51:05.000000 pami-2023.4.1/PAMI/fuzzyFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.307613 pami-2023.4.1/PAMI/fuzzyFrequentSpatialPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/fuzzyFrequentSpatialPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.310931 pami-2023.4.1/PAMI/fuzzyFrequentSpatialPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    24222 2023-03-02 04:09:41.000000 pami-2023.4.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    26791 2023-03-01 01:58:20.000000 pami-2023.4.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6580 2022-09-13 03:26:08.000000 pami-2023.4.1/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.311239 pami-2023.4.1/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.315636 pami-2023.4.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    22613 2023-03-21 05:53:43.000000 pami-2023.4.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    25345 2023-03-01 01:58:20.000000 pami-2023.4.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6668 2022-09-13 03:26:08.000000 pami-2023.4.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.319127 pami-2023.4.1/PAMI/fuzzySpatialPeriodicFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.320342 pami-2023.4.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    27112 2023-03-21 05:53:43.000000 pami-2023.4.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    32216 2023-03-01 01:58:20.000000 pami-2023.4.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-16 08:22:43.000000 pami-2023.4.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6618 2023-03-21 05:53:43.000000 pami-2023.4.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.321514 pami-2023.4.1/PAMI/geoReferencedFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)    27553 2023-06-01 12:40:35.000000 pami-2023.4.1/PAMI/geoReferencedFrequentPattern/GFPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-04-03 08:12:11.000000 pami-2023.4.1/PAMI/geoReferencedFrequentPattern/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5006 2023-06-01 12:40:35.000000 pami-2023.4.1/PAMI/geoReferencedFrequentPattern/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.321732 pami-2023.4.1/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-09-10 01:57:05.000000 pami-2023.4.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.322662 pami-2023.4.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    18686 2023-05-26 00:41:32.000000 pami-2023.4.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-12 13:22:01.000000 pami-2023.4.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6774 2022-09-13 03:26:08.000000 pami-2023.4.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.323425 pami-2023.4.1/PAMI/highUtilityFrequentPatterns/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/highUtilityFrequentPatterns/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.324624 pami-2023.4.1/PAMI/highUtilityFrequentPatterns/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    35252 2023-02-07 03:37:24.000000 pami-2023.4.1/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/highUtilityFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6081 2022-09-13 03:26:08.000000 pami-2023.4.1/PAMI/highUtilityFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.324948 pami-2023.4.1/PAMI/highUtilityFrequentSpatialPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/highUtilityFrequentSpatialPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.327036 pami-2023.4.1/PAMI/highUtilityFrequentSpatialPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    38373 2022-09-15 06:00:15.000000 pami-2023.4.1/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6181 2022-09-13 03:26:07.000000 pami-2023.4.1/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.327408 pami-2023.4.1/PAMI/highUtilityPatterns/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/highUtilityPatterns/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.329445 pami-2023.4.1/PAMI/highUtilityPatterns/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    31875 2023-02-07 03:55:11.000000 pami-2023.4.1/PAMI/highUtilityPatterns/basic/EFIM.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    23450 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/highUtilityPatterns/basic/HMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    25807 2023-02-07 03:54:20.000000 pami-2023.4.1/PAMI/highUtilityPatterns/basic/UPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/highUtilityPatterns/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5053 2022-09-13 03:26:07.000000 pami-2023.4.1/PAMI/highUtilityPatterns/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.337014 pami-2023.4.1/PAMI/highUtilitySpatialPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6718 2022-09-13 03:26:07.000000 pami-2023.4.1/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.338319 pami-2023.4.1/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    25729 2023-02-07 04:08:34.000000 pami-2023.4.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    32747 2023-02-04 06:23:46.000000 pami-2023.4.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5955 2022-09-13 03:26:06.000000 pami-2023.4.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.339227 pami-2023.4.1/PAMI/highUtilitySpatialPattern/topk/
+-rw-r--r--   0 likhitha   (505) staff       (20)    33511 2023-02-07 04:26:57.000000 pami-2023.4.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6625 2023-02-07 04:28:07.000000 pami-2023.4.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.339524 pami-2023.4.1/PAMI/localPeriodicPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.340771 pami-2023.4.1/PAMI/localPeriodicPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    30377 2022-09-15 07:36:55.000000 pami-2023.4.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    19626 2022-09-15 07:36:55.000000 pami-2023.4.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    18711 2022-09-15 07:36:55.000000 pami-2023.4.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     8378 2022-09-15 07:26:35.000000 pami-2023.4.1/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.341055 pami-2023.4.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-06-21 09:08:43.000000 pami-2023.4.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.342475 pami-2023.4.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    22172 2023-03-21 05:53:43.000000 pami-2023.4.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    21275 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-12 07:16:58.000000 pami-2023.4.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5913 2022-09-13 03:26:08.000000 pami-2023.4.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.342745 pami-2023.4.1/PAMI/partialPeriodicFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.343989 pami-2023.4.1/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    25450 2022-10-12 03:45:33.000000 pami-2023.4.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    19431 2022-10-12 03:52:53.000000 pami-2023.4.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5392 2022-09-13 07:44:04.000000 pami-2023.4.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.344426 pami-2023.4.1/PAMI/partialPeriodicPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.347156 pami-2023.4.1/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    49814 2023-03-02 08:48:22.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     4195 2022-09-13 03:26:07.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    23287 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    16901 2023-05-26 00:41:32.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5572 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.348181 pami-2023.4.1/PAMI/partialPeriodicPattern/closed/
+-rw-r--r--   0 likhitha   (505) staff       (20)    19695 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5595 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.349263 pami-2023.4.1/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 likhitha   (505) staff       (20)    27900 2022-10-12 03:35:13.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     4261 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.350288 pami-2023.4.1/PAMI/partialPeriodicPattern/timeSeries/
+-rw-r--r--   0 likhitha   (505) staff       (20)    25314 2022-09-13 07:44:04.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-08-02 07:47:39.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/timeSeries/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     5550 2022-09-13 07:44:04.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/timeSeries/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.351329 pami-2023.4.1/PAMI/partialPeriodicPattern/topk/
+-rw-r--r--   0 likhitha   (505) staff       (20)    16925 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/topk/Topk_PPPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     7837 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/partialPeriodicPattern/topk/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.351644 pami-2023.4.1/PAMI/partialPeriodicSpatialPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-06-28 05:26:47.000000 pami-2023.4.1/PAMI/partialPeriodicSpatialPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.352555 pami-2023.4.1/PAMI/partialPeriodicSpatialPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    18201 2022-09-16 08:22:43.000000 pami-2023.4.1/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-16 08:22:43.000000 pami-2023.4.1/PAMI/partialPeriodicSpatialPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6165 2022-09-16 08:22:40.000000 pami-2023.4.1/PAMI/partialPeriodicSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.352871 pami-2023.4.1/PAMI/periodicCorrelatedPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.353844 pami-2023.4.1/PAMI/periodicCorrelatedPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    26674 2022-09-16 08:22:43.000000 pami-2023.4.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-16 08:22:43.000000 pami-2023.4.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6652 2022-09-16 08:22:40.000000 pami-2023.4.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.354118 pami-2023.4.1/PAMI/periodicFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.356172 pami-2023.4.1/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    14838 2023-05-26 00:41:32.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    24398 2022-09-13 07:43:58.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    24123 2022-09-13 07:43:58.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    15529 2022-09-13 07:43:58.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    32465 2022-09-13 07:43:58.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)      726 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6525 2022-09-15 07:15:16.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.357204 pami-2023.4.1/PAMI/periodicFrequentPattern/closed/
+-rw-r--r--   0 likhitha   (505) staff       (20)    19782 2022-09-13 07:43:58.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6538 2022-09-13 03:26:08.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.357928 pami-2023.4.1/PAMI/periodicFrequentPattern/cuda/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-02-11 00:26:28.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    16537 2023-02-11 00:26:28.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.359064 pami-2023.4.1/PAMI/periodicFrequentPattern/maximal/
+-rw-r--r--   0 likhitha   (505) staff       (20)    27844 2023-02-07 05:06:18.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     7873 2022-09-13 03:26:08.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.359338 pami-2023.4.1/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.360259 pami-2023.4.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-r--r--   0 likhitha   (505) staff       (20)    17228 2023-02-07 01:47:35.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-02-07 01:47:35.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6898 2023-02-07 01:47:35.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.361335 pami-2023.4.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-02-07 01:52:08.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     4583 2023-02-07 01:49:30.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    16401 2023-02-07 01:56:38.000000 pami-2023.4.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.361736 pami-2023.4.1/PAMI/recurringPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.362916 pami-2023.4.1/PAMI/recurringPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    25551 2023-02-11 00:45:20.000000 pami-2023.4.1/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/recurringPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6632 2022-09-13 07:44:04.000000 pami-2023.4.1/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.363432 pami-2023.4.1/PAMI/relativeFrequentPatterns/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/relativeFrequentPatterns/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.365410 pami-2023.4.1/PAMI/relativeFrequentPatterns/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    25500 2022-09-20 08:51:48.000000 pami-2023.4.1/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/relativeFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     4261 2022-09-20 08:51:48.000000 pami-2023.4.1/PAMI/relativeFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.365869 pami-2023.4.1/PAMI/relativeHighUtilityPatterns/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/relativeHighUtilityPatterns/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.366849 pami-2023.4.1/PAMI/relativeHighUtilityPatterns/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    32789 2023-02-09 04:36:40.000000 pami-2023.4.1/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/relativeHighUtilityPatterns/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     7391 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/relativeHighUtilityPatterns/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.367252 pami-2023.4.1/PAMI/sequentialPatternMining/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.368744 pami-2023.4.1/PAMI/sequentialPatternMining/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    40559 2023-02-28 05:51:58.000000 pami-2023.4.1/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-21 04:49:06.000000 pami-2023.4.1/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6554 2023-01-08 10:45:15.000000 pami-2023.4.1/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    22030 2023-02-11 00:26:28.000000 pami-2023.4.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.369520 pami-2023.4.1/PAMI/sequentialPatternMining/closed/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-21 04:50:02.000000 pami-2023.4.1/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6279 2022-09-13 03:26:07.000000 pami-2023.4.1/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-21 04:50:31.000000 pami-2023.4.1/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.369621 pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.373000 pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    15381 2023-05-26 00:41:32.000000 pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    24073 2023-05-26 00:41:32.000000 pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    17918 2022-09-13 03:26:06.000000 pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-06-30 05:09:24.000000 pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     7258 2022-09-13 03:26:06.000000 pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.373884 pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-r--r--   0 likhitha   (505) staff       (20)    25615 2023-02-10 03:23:27.000000 pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     7177 2022-09-13 03:26:07.000000 pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.374238 pami-2023.4.1/PAMI/uncertainFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.377617 pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    24906 2022-09-13 07:44:04.000000 pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    25115 2023-02-28 09:14:04.000000 pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    17825 2022-09-13 03:26:05.000000 pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    26168 2023-03-31 03:36:16.000000 pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    26931 2023-03-31 03:36:16.000000 pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    24582 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    18153 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     4962 2022-09-13 07:44:04.000000 pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.377910 pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)      727 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.380190 pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    30266 2023-02-07 01:21:17.000000 pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    30696 2023-02-07 01:21:54.000000 pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6551 2022-09-13 07:44:04.000000 pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    30905 2022-10-03 07:07:51.000000 pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/basic/upfp.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    33359 2022-10-06 01:25:48.000000 pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/basic/upfpplus.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.380738 pami-2023.4.1/PAMI/uncertainProbablisticFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-27 07:43:30.000000 pami-2023.4.1/PAMI/uncertainProbablisticFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.380994 pami-2023.4.1/PAMI/uncertainProbablisticFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-27 07:43:44.000000 pami-2023.4.1/PAMI/uncertainProbablisticFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     4962 2022-09-27 07:44:21.000000 pami-2023.4.1/PAMI/uncertainProbablisticFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.381355 pami-2023.4.1/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-06-28 05:36:22.000000 pami-2023.4.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.382244 pami-2023.4.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    26149 2023-02-06 08:15:48.000000 pami-2023.4.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6693 2023-02-06 08:50:12.000000 pami-2023.4.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.382571 pami-2023.4.1/PAMI/weightedFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.383488 pami-2023.4.1/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    23009 2022-09-20 06:22:27.000000 pami-2023.4.1/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     6737 2022-09-13 07:44:04.000000 pami-2023.4.1/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.386093 pami-2023.4.1/PAMI/weightedFrequentRegularPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.386885 pami-2023.4.1/PAMI/weightedFrequentRegularPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    26702 2023-02-10 03:46:01.000000 pami-2023.4.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     7555 2022-09-13 07:44:04.000000 pami-2023.4.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.387191 pami-2023.4.1/PAMI/weightedUncertainFrequentPattern/
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2022-05-26 01:58:44.000000 pami-2023.4.1/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.388200 pami-2023.4.1/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 likhitha   (505) staff       (20)    28437 2023-02-28 09:14:04.000000 pami-2023.4.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-r--r--   0 likhitha   (505) staff       (20)        0 2022-09-13 07:44:03.000000 pami-2023.4.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 likhitha   (505) staff       (20)     4782 2023-02-10 23:22:45.000000 pami-2023.4.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 likhitha   (505) staff       (20)    34613 2023-06-01 12:58:36.389650 pami-2023.4.1/PKG-INFO
+-rw-r--r--   0 likhitha   (505) staff       (20)    34029 2023-06-01 12:40:35.000000 pami-2023.4.1/README.md
+drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-01 12:58:36.389355 pami-2023.4.1/pami.egg-info/
+-rw-r--r--   0 likhitha   (505) staff       (20)    34613 2023-06-01 12:58:36.000000 pami-2023.4.1/pami.egg-info/PKG-INFO
+-rw-r--r--   0 likhitha   (505) staff       (20)    13726 2023-06-01 12:58:36.000000 pami-2023.4.1/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-06-01 12:58:36.000000 pami-2023.4.1/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 likhitha   (505) staff       (20)       75 2023-06-01 12:58:36.000000 pami-2023.4.1/pami.egg-info/requires.txt
+-rw-r--r--   0 likhitha   (505) staff       (20)        5 2023-06-01 12:58:36.000000 pami-2023.4.1/pami.egg-info/top_level.txt
+-rw-r--r--   0 likhitha   (505) staff       (20)       38 2023-06-01 12:58:36.390008 pami-2023.4.1/setup.cfg
+-rw-r--r--   0 likhitha   (505) staff       (20)     1205 2023-06-01 12:56:05.000000 pami-2023.4.1/setup.py
```

### Comparing `pami-2023.3.1/LICENSE` & `pami-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/AssociationRules/basic/RuleMiner.py` & `pami-2023.4.1/PAMI/AssociationRules/basic/RuleMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/AssociationRules/basic/abstract.py` & `pami-2023.4.1/PAMI/AssociationRules/basic/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, measure, threshold, sep="\t"):
+    def __init__(self, iFile, threshold, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str or DataFrame
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
@@ -103,15 +103,14 @@
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._threshold = threshold
-        self._measure = measure
         self._finalPatterns = {}
         self._oFile = str()
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
```

### Comparing `pami-2023.3.1/PAMI/correlatedPattern/__init__.py` & `pami-2023.4.1/PAMI/correlatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/correlatedPattern/basic/CPGrowth.py` & `pami-2023.4.1/PAMI/correlatedPattern/basic/CPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/correlatedPattern/basic/CPGrowthPlus.py` & `pami-2023.4.1/PAMI/correlatedPattern/basic/CPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/correlatedPattern/basic/__init__.py` & `pami-2023.4.1/PAMI/correlatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/correlatedPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/correlatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/coveragePatterns/basic/CMine.py` & `pami-2023.4.1/PAMI/coveragePatterns/basic/CMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/coveragePatterns/basic/CPPG.py` & `pami-2023.4.1/PAMI/coveragePatterns/basic/CPPG.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/coveragePatterns/basic/abstract.py` & `pami-2023.4.1/PAMI/coveragePatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/DF2DB/DF2DB.py` & `pami-2023.4.1/PAMI/extras/DF2DB/DF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/DF2DB/DF2DBPlus.py` & `pami-2023.4.1/PAMI/extras/DF2DB/DF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/DF2DB/createTDB.py` & `pami-2023.4.1/PAMI/extras/DF2DB/createTDB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/DF2DB/denseDF2DB.py` & `pami-2023.4.1/PAMI/extras/DF2DB/denseDF2DB.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     def __init__(self, inputDF, condition, thresholdValue):
         self.inputDF = inputDF
         self.condition = condition
         self.thresholdValue = thresholdValue
         self.tids = []
         self.items = []
         self.outputFile = ' '
-        self.inputDF = self.inputDF.set_index('tid')
-        self.items = list(self.inputDF.columns.values)[1:]
+        self.inputDF = self.inputDF.set_index('tid', drop=True)
+        self.items = list(self.inputDF.columns.values)
 
         self.tids = list(self.inputDF.index)
 
 
     def createTransactional(self, outputFile):
         """
         Create transactional data base
```

### Comparing `pami-2023.3.1/PAMI/extras/DF2DB/denseDF2DBPlus.py` & `pami-2023.4.1/PAMI/extras/DF2DB/denseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/DF2DB/sparseDF2DB.py` & `pami-2023.4.1/PAMI/extras/DF2DB/sparseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py` & `pami-2023.4.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/calculateMISValues/usingBeta.py` & `pami-2023.4.1/PAMI/extras/calculateMISValues/usingBeta.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/calculateMISValues/usingSD.py` & `pami-2023.4.1/PAMI/extras/calculateMISValues/usingSD.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py` & `pami-2023.4.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/dbStats/temporalDatabaseStats.py` & `pami-2023.4.1/PAMI/extras/dbStats/temporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/dbStats/transactionalDatabaseStats.py` & `pami-2023.4.1/PAMI/extras/dbStats/transactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py` & `pami-2023.4.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py` & `pami-2023.4.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/dbStats/utilityDatabaseStats.py` & `pami-2023.4.1/PAMI/extras/dbStats/utilityDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/fuzzyTransformation/abstract.py` & `pami-2023.4.1/PAMI/extras/fuzzyTransformation/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py` & `pami-2023.4.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py` & `pami-2023.4.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py` & `pami-2023.4.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py` & `pami-2023.4.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py` & `pami-2023.4.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py` & `pami-2023.4.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/generateLatexGraphFile.py` & `pami-2023.4.1/PAMI/extras/generateLatexGraphFile.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/graph/dataFrameInToFigures.py` & `pami-2023.4.1/PAMI/extras/graph/dataFrameInToFigures.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py` & `pami-2023.4.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/graph/plotLineGraphFromDictionary.py` & `pami-2023.4.1/PAMI/extras/graph/plotLineGraphFromDictionary.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py` & `pami-2023.4.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/graph/visualizePatterns.py` & `pami-2023.4.1/PAMI/extras/graph/visualizePatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/imageProcessing/imagery2Databases.py` & `pami-2023.4.1/PAMI/extras/imageProcessing/imagery2Databases.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py` & `pami-2023.4.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/plotPointOnMap.py` & `pami-2023.4.1/PAMI/extras/plotPointOnMap.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/plotPointOnMap_dump.py` & `pami-2023.4.1/PAMI/extras/plotPointOnMap_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/scatterPlotSpatialPoints.py` & `pami-2023.4.1/PAMI/extras/scatterPlotSpatialPoints.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/extras/topKPatterns.py` & `pami-2023.4.1/PAMI/extras/topKPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py` & `pami-2023.4.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py` & `pami-2023.4.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py` & `pami-2023.4.1/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/faultTolerantFrequentPattern/maximal/abstract.py` & `pami-2023.4.1/PAMI/faultTolerantFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/faultTolerantFrequentPattern/maximal/maxFTP.py` & `pami-2023.4.1/PAMI/faultTolerantFrequentPattern/maximal/maxFTP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/__init__.py` & `pami-2023.4.1/PAMI/frequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/basic/Apriori.py` & `pami-2023.4.1/PAMI/frequentPattern/basic/Apriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/basic/ECLAT.py` & `pami-2023.4.1/PAMI/frequentPattern/basic/ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/basic/ECLATDiffset.py` & `pami-2023.4.1/PAMI/frequentPattern/basic/ECLATDiffset.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,15 +209,16 @@
                         else:
                             tidSets[item] = {transNum}
         for key, value in tidSets.items():
             supp = len(value)
             if supp >= self._minSup:
                 self._diffSets[key] = [supp, self._trans_set.difference(value)]
                 uniqueItem.append(key)
-
+        # for x, y in self._diffSets.items():
+        #     print(x, y)
         uniqueItem.sort()
         # print()
         return uniqueItem
 
     def _runDeclat(self, candidateList):
 
         newList = []
@@ -230,32 +231,40 @@
                 if iList[:-1] == jList[:-1]:
                     unionDiffSet = self._diffSets[item2][1].difference(self._diffSets[item1][1])
                     unionSup = self._diffSets[item1][0] - len(unionDiffSet)
                     if unionSup >= self._minSup:
                         newKey = item1 + "\t" + jList[-1]
                         self._diffSets[newKey] = [unionSup, unionDiffSet]
                         newList.append(newKey)
-                    else: break
+                    else: 
+                        break
 
         if len(newList) > 0:
             self._runDeclat(newList)
 
     def startMine(self):
         """Frequent pattern mining process will start from here"""
 
         self._startTime = _ab._time.time()
+        self._Database = []
+        self._finalPatterns = {}
+        self._diffSets = {}
+        self._trans_set = set()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
         if self._minSup is None:
             raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
+        #print(len(self._Database))
         self._minSup = self._convert(self._minSup)
+        uniqueItemList = []
         uniqueItemList = self._getUniqueItemList()
         self._runDeclat(uniqueItemList)
         self._finalPatterns = self._diffSets
+        #print(len(self._finalPatterns), len(uniqueItemList))
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
         print("Frequent patterns were generated successfully using ECLAT Diffset algorithm")
@@ -297,29 +306,29 @@
 
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b])
+            data.append([a.replace('\t', ' '), b[0]])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
     def save(self, outFile):
         """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            patternsAndSupport = x.strip() + ":" + str(y)
+            patternsAndSupport = x.strip() + ":" + str(y[0])
             writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
 
@@ -347,8 +356,7 @@
         print(_ap.getPatternsAsDataFrame())
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
-
```

### Comparing `pami-2023.3.1/PAMI/frequentPattern/basic/ECLATbitset.py` & `pami-2023.4.1/PAMI/frequentPattern/basic/ECLATbitset.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/basic/FPGrowth.py` & `pami-2023.4.1/PAMI/frequentPattern/basic/FPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/frequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/closed/CHARM.py` & `pami-2023.4.1/PAMI/frequentPattern/closed/CHARM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/closed/abstract.py` & `pami-2023.4.1/PAMI/frequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py` & `pami-2023.4.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py` & `pami-2023.4.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py` & `pami-2023.4.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py` & `pami-2023.4.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/maximal/__init__.py` & `pami-2023.4.1/PAMI/frequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/maximal/abstract.py` & `pami-2023.4.1/PAMI/frequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/pyspark/abstract.py` & `pami-2023.4.1/PAMI/frequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/pyspark/parallelApriori.py` & `pami-2023.4.1/PAMI/frequentPattern/pyspark/parallelApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/pyspark/parallelECLAT.py` & `pami-2023.4.1/PAMI/frequentPattern/pyspark/parallelECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py` & `pami-2023.4.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/topk/FAE.py` & `pami-2023.4.1/PAMI/frequentPattern/topk/FAE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentPattern/topk/abstract.py` & `pami-2023.4.1/PAMI/frequentPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentSpatialPattern/__init__.py` & `pami-2023.4.1/PAMI/frequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentSpatialPattern/basic/FSPGrowth.py` & `pami-2023.4.1/PAMI/frequentSpatialPattern/basic/FSPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py` & `pami-2023.4.1/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/frequentSpatialPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/frequentSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyCorrelatedPattern/__init__.py` & `pami-2023.4.1/PAMI/fuzzyCorrelatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py` & `pami-2023.4.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py` & `pami-2023.4.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyFrequentPatterns/__init__.py` & `pami-2023.4.1/PAMI/fuzzyFrequentPatterns/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py` & `pami-2023.4.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py` & `pami-2023.4.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyFrequentPatterns/basic/abstract.py` & `pami-2023.4.1/PAMI/fuzzyFrequentPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyFrequentSpatialPattern/__init__.py` & `pami-2023.4.1/PAMI/fuzzyFrequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py` & `pami-2023.4.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py` & `pami-2023.4.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py` & `pami-2023.4.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py` & `pami-2023.4.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py` & `pami-2023.4.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py` & `pami-2023.4.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py` & `pami-2023.4.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py` & `pami-2023.4.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/geoReferencedFrequentPattern/GFPGrowth.py` & `pami-2023.4.1/PAMI/geoReferencedFrequentPattern/GFPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from geoReferencedFrequentPatterns import abstract as _ab
+from PAMI.geoReferencedFrequentPatterns import abstract as _ab
 
 _minSup = str()
 _neighbourList = {}
 _ab._sys.setrecursionlimit(20000)
 _finalPatterns = {}
```

### Comparing `pami-2023.3.1/PAMI/geoReferencedFrequentPattern/abstract.py` & `pami-2023.4.1/PAMI/geoReferencedFrequentPattern/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
```

### Comparing `pami-2023.3.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py` & `pami-2023.4.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
         run = obj.getRuntime()
 
         print("Total ExecutionTime in seconds:", run)
 
     Credits:
     -------
-        The complete program was written by P. Likhitha under the supervision of Professor Rage Uday Kiran.
+        The complete program was written by P.RaviKumar under the supervision of Professor Rage Uday Kiran.
     """
 
     _minSup = " "
     _maxPer = " "
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
```

### Comparing `pami-2023.3.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py` & `pami-2023.4.1/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilityFrequentPatterns/basic/abstract.py` & `pami-2023.4.1/PAMI/highUtilityFrequentPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilityFrequentSpatialPattern/__init__.py` & `pami-2023.4.1/PAMI/highUtilityFrequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py` & `pami-2023.4.1/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilityPatterns/basic/EFIM.py` & `pami-2023.4.1/PAMI/highUtilityPatterns/basic/EFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilityPatterns/basic/HMiner.py` & `pami-2023.4.1/PAMI/highUtilityPatterns/basic/HMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilityPatterns/basic/UPGrowth.py` & `pami-2023.4.1/PAMI/highUtilityPatterns/basic/UPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilityPatterns/basic/abstract.py` & `pami-2023.4.1/PAMI/highUtilityPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilitySpatialPattern/__init__.py` & `pami-2023.4.1/PAMI/highUtilitySpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilitySpatialPattern/abstract.py` & `pami-2023.4.1/PAMI/highUtilitySpatialPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py` & `pami-2023.4.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py` & `pami-2023.4.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilitySpatialPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/highUtilitySpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py` & `pami-2023.4.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/highUtilitySpatialPattern/topk/abstract.py` & `pami-2023.4.1/PAMI/highUtilitySpatialPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py` & `pami-2023.4.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py` & `pami-2023.4.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py` & `pami-2023.4.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/localPeriodicPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/localPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py` & `pami-2023.4.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py` & `pami-2023.4.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py` & `pami-2023.4.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py` & `pami-2023.4.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/__init__.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/basic/Gabstract.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/basic/Gabstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         run = obj.getRuntime()
 
         print("Total ExecutionTime in seconds:", run)
 
         Credits:
         -------
 
-        The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.\n
+        The complete program was written by P.RaviKumar  under the supervision of Professor Rage Uday Kiran.\n
 
 
 
         """
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
```

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/basic/__init__.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/closed/PPPClose.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/closed/PPPClose.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/closed/abstract.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/maximal/__init__.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/maximal/abstract.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/timeSeries/abstract.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/timeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/topk/Topk_PPPGrowth.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/topk/Topk_PPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicPattern/topk/abstract.py` & `pami-2023.4.1/PAMI/partialPeriodicPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py` & `pami-2023.4.1/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/partialPeriodicSpatialPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/partialPeriodicSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py` & `pami-2023.4.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicCorrelatedPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/periodicCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/__init__.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
         Credits:
         -------
-            The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.\n
+            The complete program was written by P.RaviKumar  under the supervision of Professor Rage Uday Kiran.\n
 
         """
     
     _iFile = " "
     _oFile = " "
     _sep = " "
     _dbSize = None
```

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/basic/PFPMC.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/basic/PFPMC.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/basic/__init__.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/closed/__init__.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/closed/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/closed/abstract.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/maximal/__init__.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/maximal/abstract.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py` & `pami-2023.4.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/recurringPattern/basic/RPGrowth.py` & `pami-2023.4.1/PAMI/recurringPattern/basic/RPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/recurringPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/recurringPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py` & `pami-2023.4.1/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/relativeFrequentPatterns/basic/abstract.py` & `pami-2023.4.1/PAMI/relativeFrequentPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py` & `pami-2023.4.1/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/relativeHighUtilityPatterns/basic/abstract.py` & `pami-2023.4.1/PAMI/relativeHighUtilityPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/sequentialPatternMining/basic/SPADE.py` & `pami-2023.4.1/PAMI/sequentialPatternMining/basic/SPADE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/sequentialPatternMining/basic/abstract.py` & `pami-2023.4.1/PAMI/sequentialPatternMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/sequentialPatternMining/basic/prefixSpan.py` & `pami-2023.4.1/PAMI/sequentialPatternMining/basic/prefixSpan.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/sequentialPatternMining/closed/abstract.py` & `pami-2023.4.1/PAMI/sequentialPatternMining/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py` & `pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from PAMI.stablePeriodicFrequentPattern.basic import abstract as _ab
 
-class SPPEclat:
+class SPPEclat(_ab._stablePeriodicFrequentPatterns):
     """  Stable periodic pattern mining aims to dicover all interesting patterns in a temporal database using three contraints minimum support,
          maximum period and maximum lability, that have support no less than the user-specified minimum support  constraint and lability no
           greater than maximum lability.
 
             Reference:
             --------
-                Fournier-Viger, P., Yang, P., Lin, J. C.-W., Kiran, U. (2019). Discovering Stable Periodic-Frequent Patterns in Transactional Data. Proc.
-                 32nd Intern. Conf. on Industrial, Engineering and Other Applications of Applied Intelligent Systems (IEA AIE 2019), Springer LNAI, pp. 230-244
+                Dao, H.N. et al. (2022). Towards Efficient Discovery of Stable Periodic Patterns in Big Columnar Temporal Databases. 
+                In: Fujita, H., Fournier-Viger, P., Ali, M., Wang, Y. (eds) Advances and Trends in Artificial Intelligence.
+                Theory and Practices in Artificial Intelligence. IEA/AIE 2022. Lecture Notes in Computer Science(), vol 13343. Springer, Cham. 
+                https://doi.org/10.1007/978-3-031-08530-7_70
+
+
 
         Attributes:
         ---------
             iFile : file
                 Name of the Input file or path of the input file
             oFile : file
                 Name of the output file or path of the output file
```

### Comparing `pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py` & `pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
             for pat in range(len(patterns)):
                 conditionalTree.addTransaction(patterns[pat], timeStamps[pat])
             if len(patterns) > 0:
                 for q in conditionalTree.generatePatterns(pattern):
                     yield q
             self.removeNode(i)
 
-class SPPGrowth():
+class SPPGrowth(_ab._stablePeriodicFrequentPatterns):
     """ Stable periodic pattern mining aims to dicover all interesting patterns in a temporal database using three contraints minimum support,
          maximum period and maximum lability, that have support no less than the user-specified minimum support  constraint and lability no
           greater than maximum lability.
 
         Reference:
         --------
             Dao, H.N. et al. (2022). Towards Efficient Discovery of Stable Periodic Patterns in Big Columnar Temporal Databases.
```

### Comparing `pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py` & `pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py` & `pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py` & `pami-2023.4.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainFrequentPattern/__init__.py` & `pami-2023.4.1/PAMI/uncertainFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py` & `pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py` & `pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/TUFP.py` & `pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/TUFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/TubeP.py` & `pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/TubeP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/TubeS.py` & `pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/TubeS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py` & `pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py` & `pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainFrequentPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/uncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py` & `pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py` & `pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py` & `pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/basic/upfp.py` & `pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/basic/upfp.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainPeriodicFrequentPattern/basic/upfpplus.py` & `pami-2023.4.1/PAMI/uncertainPeriodicFrequentPattern/basic/upfpplus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/uncertainProbablisticFrequentPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/uncertainProbablisticFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py` & `pami-2023.4.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/weightedFrequentPattern/basic/WFIM.py` & `pami-2023.4.1/PAMI/weightedFrequentPattern/basic/WFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/weightedFrequentPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/weightedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py` & `pami-2023.4.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py` & `pami-2023.4.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py` & `pami-2023.4.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.3.1/PKG-INFO` & `pami-2023.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,76 +1,68 @@
-Metadata-Version: 2.1
-Name: pami
-Version: 2023.3.1
-Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
-Home-page: https://github.com/udayRage/PAMI
-Author: Rage Uday Kiran
-Author-email: uday.rage@gmail.com
-License: GPLv3
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
 ![AppVeyor](https://img.shields.io/appveyor/build/udayRage/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
 ![GitHub all releases](https://img.shields.io/github/downloads/udayRage/PAMI/total)
 [![GitHub license](https://img.shields.io/github/license/udayRage/PAMI)](https://github.com/udayRage/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
 [![GitHub issues](https://img.shields.io/github/issues/udayRage/PAMI)](https://github.com/udayRage/PAMI/issues)
 [![GitHub forks](https://img.shields.io/github/forks/udayRage/PAMI)](https://github.com/udayRage/PAMI/network)
 [![GitHub stars](https://img.shields.io/github/stars/udayRage/PAMI)](https://github.com/udayRage/PAMI/stargazers)
 
 
+# Introduction
+PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referencial/sequence databases across multiple computing platforms.
+
 
+1. User manual https://udayrage.github.io/PAMI/manuals/index.html
 
+2. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
-# Introduction
-PAMI stands for PAttern MIning. It constitutes several pattern mining algorithms to discover interesting patterns in transactional/temporal/spatiotemporal databases.
-This software is provided under [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://www.gnu.org/licenses/quick-guide-gplv3.html).
+3. Code documentation file:///Users/likhitha/Downloads/PAMI-main-docs/docs/_build/html/index.html
+
+4. Discussions on PAMI usage https://github.com/udayRage/PAMI/discussions
+
+5. Report issues https://github.com/udayRage/PAMI/issues
+  
+ __Recent versions__  
+
+- Version 2023.03.01: prefixSpan and SPADE   
 
-1. The user manual for PAMI library is available at https://udayrage.github.io/PAMI/index.html
-2. Datasets to implement PAMI algorithms are available at https://www.u-aizu.ac.jp/~udayrage/software.html
-3. Please report issues in the software at https://github.com/udayRage/PAMI/issues
+Total number of algorithms: 83
+
+# Maintenance
+
+  Installation
   
+       pip install pami    
   
-  __Contact us by Discord__ https://discord.gg/9WgKkrSJ
+  Updation
   
-# Installation
-
-       pip install pami
-       
-# Upgrade
-      
        pip install --upgrade pami
+  
+  Uninstallation
+  
+       pip uninstall pami 
        
-# Code documentation
-[Link](https://rawcdn.githack.com/udayRage/PAMI/5eea0f346bf7818c7345c8643428ad9ce5087f15/htmlDocs/_build/html/index.html)
-
-       
-# Details 
-Total available algorithms: 70
+# Tutorials 
 
-Click on __"Basic"__ link to view the basic tutorial on using the algorithm. Similarly, click on __"Adv"__ link to view the advanced tutorial on using a particular algorithm.
+- Click on __"Basic"__ link to view the basic tutorial on using the algorithm. 
+- Click on __"Adv"__ link to view the advanced tutorial on using a particular algorithm.
 
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
      
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Apriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
    | FP-growth  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
    | ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
    | ECLAT-bitSet [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
-   | ECLAT-diffset                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
+   | ECLAT-diffset [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
 
 2. Relative Frequent Patterns: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
     
 | Basic |
 |-------|
 | RSFP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
@@ -95,39 +87,39 @@
 
 | Basic                                                                                                                                                                                                                                 |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | spatialECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
 | FSP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
     
     
-6. Fuzzy Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyFrequentPatternMining.html)
+6. Fuzzy Frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                   |
 |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FFI-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
     
 7. Fuzzy correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                        |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
  
-8. Fuzzy frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyFrequentSpatialPatternMining.html)
+8. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentSpatialPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                  |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FFSP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
     
-9. Fuzzy periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyPeriodicFrequentPatternMining.html)
+9. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyPeriodicFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                    |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
  | FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
     
-9. Geo referenced Fuzzy periodic frequent pattern mining: 
+9. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html) 
 
 | Basic                                                                                                                                                                                                                                    |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
 
 10. High utility pattern mining:   [Sample](https://udayrage.github.io/PAMI/highUtilityPatternMining.html)
```

### Comparing `pami-2023.3.1/README.md` & `pami-2023.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,84 @@
+Metadata-Version: 2.1
+Name: pami
+Version: 2023.4.1
+Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
+Home-page: https://github.com/udayRage/PAMI
+Author: Rage Uday Kiran
+Author-email: uday.rage@gmail.com
+License: GPLv3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
 ![AppVeyor](https://img.shields.io/appveyor/build/udayRage/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
 ![GitHub all releases](https://img.shields.io/github/downloads/udayRage/PAMI/total)
 [![GitHub license](https://img.shields.io/github/license/udayRage/PAMI)](https://github.com/udayRage/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
 [![GitHub issues](https://img.shields.io/github/issues/udayRage/PAMI)](https://github.com/udayRage/PAMI/issues)
 [![GitHub forks](https://img.shields.io/github/forks/udayRage/PAMI)](https://github.com/udayRage/PAMI/network)
 [![GitHub stars](https://img.shields.io/github/stars/udayRage/PAMI)](https://github.com/udayRage/PAMI/stargazers)
 
 
+# Introduction
+PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referencial/sequence databases across multiple computing platforms.
+
 
+1. User manual https://udayrage.github.io/PAMI/manuals/index.html
 
+2. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
-# Introduction
-PAMI stands for PAttern MIning. It constitutes several pattern mining algorithms to discover interesting patterns in transactional/temporal/spatiotemporal databases.
-This software is provided under [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://www.gnu.org/licenses/quick-guide-gplv3.html).
+3. Code documentation file:///Users/likhitha/Downloads/PAMI-main-docs/docs/_build/html/index.html
+
+4. Discussions on PAMI usage https://github.com/udayRage/PAMI/discussions
+
+5. Report issues https://github.com/udayRage/PAMI/issues
+  
+ __Recent versions__  
+
+- Version 2023.03.01: prefixSpan and SPADE   
 
-1. The user manual for PAMI library is available at https://udayrage.github.io/PAMI/index.html
-2. Datasets to implement PAMI algorithms are available at https://www.u-aizu.ac.jp/~udayrage/software.html
-3. Please report issues in the software at https://github.com/udayRage/PAMI/issues
+Total number of algorithms: 83
+
+# Maintenance
+
+  Installation
   
+       pip install pami    
   
-  __Contact us by Discord__ https://discord.gg/9WgKkrSJ
+  Updation
   
-# Installation
-
-       pip install pami
-       
-# Upgrade
-      
        pip install --upgrade pami
+  
+  Uninstallation
+  
+       pip uninstall pami 
        
-# Code documentation
-[Link](https://rawcdn.githack.com/udayRage/PAMI/5eea0f346bf7818c7345c8643428ad9ce5087f15/htmlDocs/_build/html/index.html)
-
-       
-# Details 
-Total available algorithms: 70
+# Tutorials 
 
-Click on __"Basic"__ link to view the basic tutorial on using the algorithm. Similarly, click on __"Adv"__ link to view the advanced tutorial on using a particular algorithm.
+- Click on __"Basic"__ link to view the basic tutorial on using the algorithm. 
+- Click on __"Adv"__ link to view the advanced tutorial on using a particular algorithm.
 
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
      
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Apriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
    | FP-growth  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
    | ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
    | ECLAT-bitSet [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
-   | ECLAT-diffset                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
+   | ECLAT-diffset [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
 
 2. Relative Frequent Patterns: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
     
 | Basic |
 |-------|
 | RSFP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
@@ -79,39 +103,39 @@
 
 | Basic                                                                                                                                                                                                                                 |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | spatialECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
 | FSP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
     
     
-6. Fuzzy Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyFrequentPatternMining.html)
+6. Fuzzy Frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                   |
 |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FFI-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
     
 7. Fuzzy correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                        |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
  
-8. Fuzzy frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyFrequentSpatialPatternMining.html)
+8. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentSpatialPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                  |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FFSP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
     
-9. Fuzzy periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyPeriodicFrequentPatternMining.html)
+9. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyPeriodicFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                    |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
  | FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
     
-9. Geo referenced Fuzzy periodic frequent pattern mining: 
+9. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html) 
 
 | Basic                                                                                                                                                                                                                                    |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
 
 10. High utility pattern mining:   [Sample](https://udayrage.github.io/PAMI/highUtilityPatternMining.html)
```

### Comparing `pami-2023.3.1/pami.egg-info/PKG-INFO` & `pami-2023.4.1/pami.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.3.1
+Version: 2023.4.1
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayRage/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -23,54 +23,62 @@
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
 [![GitHub issues](https://img.shields.io/github/issues/udayRage/PAMI)](https://github.com/udayRage/PAMI/issues)
 [![GitHub forks](https://img.shields.io/github/forks/udayRage/PAMI)](https://github.com/udayRage/PAMI/network)
 [![GitHub stars](https://img.shields.io/github/stars/udayRage/PAMI)](https://github.com/udayRage/PAMI/stargazers)
 
 
+# Introduction
+PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referencial/sequence databases across multiple computing platforms.
 
 
+1. User manual https://udayrage.github.io/PAMI/manuals/index.html
 
-# Introduction
-PAMI stands for PAttern MIning. It constitutes several pattern mining algorithms to discover interesting patterns in transactional/temporal/spatiotemporal databases.
-This software is provided under [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://www.gnu.org/licenses/quick-guide-gplv3.html).
+2. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
+
+3. Code documentation file:///Users/likhitha/Downloads/PAMI-main-docs/docs/_build/html/index.html
+
+4. Discussions on PAMI usage https://github.com/udayRage/PAMI/discussions
 
-1. The user manual for PAMI library is available at https://udayrage.github.io/PAMI/index.html
-2. Datasets to implement PAMI algorithms are available at https://www.u-aizu.ac.jp/~udayrage/software.html
-3. Please report issues in the software at https://github.com/udayRage/PAMI/issues
+5. Report issues https://github.com/udayRage/PAMI/issues
   
+ __Recent versions__  
+
+- Version 2023.03.01: prefixSpan and SPADE   
+
+Total number of algorithms: 83
+
+# Maintenance
+
+  Installation
   
-  __Contact us by Discord__ https://discord.gg/9WgKkrSJ
+       pip install pami    
+  
+  Updation
   
-# Installation
-
-       pip install pami
-       
-# Upgrade
-      
        pip install --upgrade pami
+  
+  Uninstallation
+  
+       pip uninstall pami 
        
-# Code documentation
-[Link](https://rawcdn.githack.com/udayRage/PAMI/5eea0f346bf7818c7345c8643428ad9ce5087f15/htmlDocs/_build/html/index.html)
-
-       
-# Details 
-Total available algorithms: 70
+# Tutorials 
 
-Click on __"Basic"__ link to view the basic tutorial on using the algorithm. Similarly, click on __"Adv"__ link to view the advanced tutorial on using a particular algorithm.
+- Click on __"Basic"__ link to view the basic tutorial on using the algorithm. 
+- Click on __"Adv"__ link to view the advanced tutorial on using a particular algorithm.
 
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
      
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Apriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
    | FP-growth  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
    | ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
    | ECLAT-bitSet [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
-   | ECLAT-diffset                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
+   | ECLAT-diffset [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
 
 2. Relative Frequent Patterns: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
     
 | Basic |
 |-------|
 | RSFP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
@@ -95,39 +103,39 @@
 
 | Basic                                                                                                                                                                                                                                 |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | spatialECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
 | FSP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
     
     
-6. Fuzzy Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyFrequentPatternMining.html)
+6. Fuzzy Frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                   |
 |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FFI-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
     
 7. Fuzzy correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                        |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
  
-8. Fuzzy frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyFrequentSpatialPatternMining.html)
+8. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentSpatialPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                  |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FFSP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
     
-9. Fuzzy periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyPeriodicFrequentPatternMining.html)
+9. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyPeriodicFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                    |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
  | FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
     
-9. Geo referenced Fuzzy periodic frequent pattern mining: 
+9. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html) 
 
 | Basic                                                                                                                                                                                                                                    |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
 
 10. High utility pattern mining:   [Sample](https://udayrage.github.io/PAMI/highUtilityPatternMining.html)
```

### Comparing `pami-2023.3.1/pami.egg-info/SOURCES.txt` & `pami-2023.4.1/pami.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 LICENSE
 README.md
 setup.py
 PAMI/__init__.py
 PAMI/AssociationRules/__init__.py
+PAMI/AssociationRules/basic/ARWithConfidence.py
+PAMI/AssociationRules/basic/ARWithLeverage.py
+PAMI/AssociationRules/basic/ARWithLift.py
 PAMI/AssociationRules/basic/RuleMiner.py
 PAMI/AssociationRules/basic/__init__.py
 PAMI/AssociationRules/basic/abstract.py
 PAMI/correlatedPattern/__init__.py
 PAMI/correlatedPattern/basic/CPGrowth.py
 PAMI/correlatedPattern/basic/CPGrowthPlus.py
 PAMI/correlatedPattern/basic/__init__.py
```

### Comparing `pami-2023.3.1/setup.py` & `pami-2023.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = 'pami',
-    version = '2023.03.01',
+    version = '2023.04.01',
     author = 'Rage Uday Kiran',
     author_email = 'uday.rage@gmail.com',
     description = 'This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages=setuptools.find_packages(),
     url = 'https://github.com/udayRage/PAMI',
```

