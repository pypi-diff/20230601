# Comparing `tmp/calotron-0.0.8.tar.gz` & `tmp/calotron-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calotron-0.0.8.tar", last modified: Sat Feb  4 09:16:22 2023, max compression
+gzip compressed data, was "calotron-0.0.9.tar", last modified: Sun Feb  5 22:40:34 2023, max compression
```

## Comparing `calotron-0.0.8.tar` & `calotron-0.0.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-04 09:16:22.313543 calotron-0.0.8/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1072 2022-11-24 10:50:51.000000 calotron-0.0.8/LICENSE
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     3285 2023-02-04 09:16:22.313543 calotron-0.0.8/PKG-INFO
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2191 2023-02-03 23:54:56.000000 calotron-0.0.8/README.md
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1832 2023-02-02 10:31:01.000000 calotron-0.0.8/pyproject.toml
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-04 09:16:22.307543 calotron-0.0.8/requirements/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       23 2023-02-02 10:31:08.000000 calotron-0.0.8/requirements/base.txt
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      233 2023-02-04 09:16:22.314543 calotron-0.0.8/setup.cfg
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-04 09:16:22.306543 calotron-0.0.8/src/
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-04 09:16:22.308543 calotron-0.0.8/src/calotron/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       33 2023-01-23 11:39:52.000000 calotron-0.0.8/src/calotron/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-04 09:16:22.308543 calotron-0.0.8/src/calotron/callbacks/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2022-12-14 11:16:55.000000 calotron-0.0.8/src/calotron/callbacks/__init__.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     8285 2023-01-25 13:21:33.000000 calotron-0.0.8/src/calotron/callbacks/schedulers.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-04 09:16:22.309543 calotron-0.0.8/src/calotron/layers/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1171 2023-01-23 11:40:27.000000 calotron-0.0.8/src/calotron/layers/Attention.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     5505 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/layers/Decoder.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2127 2023-01-23 11:40:27.000000 calotron-0.0.8/src/calotron/layers/DeepSets.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     5107 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/layers/Encoder.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1789 2023-01-23 11:40:27.000000 calotron-0.0.8/src/calotron/layers/FeedForward.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1163 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/layers/MultiActivations.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2110 2023-01-23 11:40:27.000000 calotron-0.0.8/src/calotron/layers/PositionalEmbedding.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      306 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/layers/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-04 09:16:22.310543 calotron-0.0.8/src/calotron/losses/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      853 2023-01-23 13:54:49.000000 calotron-0.0.8/src/calotron/losses/BaseLoss.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1821 2023-02-02 10:19:59.000000 calotron-0.0.8/src/calotron/losses/BinaryCrossentropy.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2110 2023-02-02 10:19:59.000000 calotron-0.0.8/src/calotron/losses/CaloLoss.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1553 2023-02-02 10:19:59.000000 calotron-0.0.8/src/calotron/losses/JSDivergence.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1101 2023-02-02 10:19:59.000000 calotron-0.0.8/src/calotron/losses/KLDivergence.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1084 2023-02-02 10:19:59.000000 calotron-0.0.8/src/calotron/losses/MeanAbsoluteError.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1082 2023-02-02 10:19:59.000000 calotron-0.0.8/src/calotron/losses/MeanSquaredError.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      256 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/losses/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-04 09:16:22.311543 calotron-0.0.8/src/calotron/metrics/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      592 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/metrics/Accuracy.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      542 2023-01-23 13:53:25.000000 calotron-0.0.8/src/calotron/metrics/BaseMetric.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      668 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/metrics/BinaryCrossentropy.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      793 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/metrics/JSDivergence.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      512 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/metrics/KLDivergence.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      515 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/metrics/MeanAbsoluteError.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      513 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/metrics/MeanSquaredError.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      526 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/metrics/RootMeanSquaredError.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      311 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/metrics/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-04 09:16:22.312543 calotron-0.0.8/src/calotron/models/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      995 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/models/Calogantron.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     5872 2023-02-02 10:30:44.000000 calotron-0.0.8/src/calotron/models/Calotron.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2264 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/models/Discriminator.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       68 2023-01-23 13:56:33.000000 calotron-0.0.8/src/calotron/models/Generator.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     6913 2023-02-02 10:19:59.000000 calotron-0.0.8/src/calotron/models/Transformer.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      109 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/models/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-04 09:16:22.312543 calotron-0.0.8/src/calotron/simulators/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2022-12-15 16:20:53.000000 calotron-0.0.8/src/calotron/simulators/CaloSimulator.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-02-02 10:17:11.000000 calotron-0.0.8/src/calotron/simulators/ExportCaloSimulator.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      814 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/simulators/ExportSimulator.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1677 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/simulators/Simulator.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       78 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/simulators/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-04 09:16:22.313543 calotron-0.0.8/src/calotron/utils/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1354 2023-01-25 15:16:42.000000 calotron-0.0.8/src/calotron/utils/HPSingleton.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      248 2023-01-25 13:28:52.000000 calotron-0.0.8/src/calotron/utils/__init__.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1503 2023-01-23 11:41:30.000000 calotron-0.0.8/src/calotron/utils/checkActivations.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1038 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/utils/checkLoss.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1918 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/utils/checkMetrics.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      840 2023-01-23 16:41:54.000000 calotron-0.0.8/src/calotron/utils/checkOptimizer.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1013 2023-01-25 15:29:37.000000 calotron-0.0.8/src/calotron/utils/getModelSummary.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       22 2023-02-04 09:16:05.000000 calotron-0.0.8/src/calotron/version.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-04 09:16:22.308543 calotron-0.0.8/src/calotron.egg-info/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     3285 2023-02-04 09:16:22.000000 calotron-0.0.8/src/calotron.egg-info/PKG-INFO
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1932 2023-02-04 09:16:22.000000 calotron-0.0.8/src/calotron.egg-info/SOURCES.txt
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        1 2023-02-04 09:16:22.000000 calotron-0.0.8/src/calotron.egg-info/dependency_links.txt
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      222 2023-02-04 09:16:22.000000 calotron-0.0.8/src/calotron.egg-info/requires.txt
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        9 2023-02-04 09:16:22.000000 calotron-0.0.8/src/calotron.egg-info/top_level.txt
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:40:34.586936 calotron-0.0.9/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)    35148 2023-02-05 20:29:48.000000 calotron-0.0.9/LICENSE
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     3315 2023-02-05 22:40:34.586936 calotron-0.0.9/PKG-INFO
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2192 2023-02-05 22:38:49.000000 calotron-0.0.9/README.md
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1861 2023-02-05 22:38:58.000000 calotron-0.0.9/pyproject.toml
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:40:34.579936 calotron-0.0.9/requirements/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       23 2023-02-02 10:31:08.000000 calotron-0.0.9/requirements/base.txt
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      233 2023-02-05 22:40:34.586936 calotron-0.0.9/setup.cfg
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:40:34.578936 calotron-0.0.9/src/
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:40:34.579936 calotron-0.0.9/src/calotron/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       33 2023-01-23 11:39:52.000000 calotron-0.0.9/src/calotron/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:40:34.580936 calotron-0.0.9/src/calotron/callbacks/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2022-12-14 11:16:55.000000 calotron-0.0.9/src/calotron/callbacks/__init__.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     8285 2023-01-25 13:21:33.000000 calotron-0.0.9/src/calotron/callbacks/schedulers.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:40:34.581936 calotron-0.0.9/src/calotron/layers/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1171 2023-01-23 11:40:27.000000 calotron-0.0.9/src/calotron/layers/Attention.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     5505 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/layers/Decoder.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2127 2023-01-23 11:40:27.000000 calotron-0.0.9/src/calotron/layers/DeepSets.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     5107 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/layers/Encoder.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1789 2023-01-23 11:40:27.000000 calotron-0.0.9/src/calotron/layers/FeedForward.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1163 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/layers/MultiActivations.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2110 2023-01-23 11:40:27.000000 calotron-0.0.9/src/calotron/layers/PositionalEmbedding.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      306 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/layers/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:40:34.582936 calotron-0.0.9/src/calotron/losses/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      853 2023-01-23 13:54:49.000000 calotron-0.0.9/src/calotron/losses/BaseLoss.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1821 2023-02-02 10:19:59.000000 calotron-0.0.9/src/calotron/losses/BinaryCrossentropy.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2110 2023-02-02 10:19:59.000000 calotron-0.0.9/src/calotron/losses/CaloLoss.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1553 2023-02-02 10:19:59.000000 calotron-0.0.9/src/calotron/losses/JSDivergence.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1101 2023-02-02 10:19:59.000000 calotron-0.0.9/src/calotron/losses/KLDivergence.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1084 2023-02-02 10:19:59.000000 calotron-0.0.9/src/calotron/losses/MeanAbsoluteError.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1082 2023-02-02 10:19:59.000000 calotron-0.0.9/src/calotron/losses/MeanSquaredError.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      256 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/losses/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:40:34.584936 calotron-0.0.9/src/calotron/metrics/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      592 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/metrics/Accuracy.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      542 2023-01-23 13:53:25.000000 calotron-0.0.9/src/calotron/metrics/BaseMetric.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      668 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/metrics/BinaryCrossentropy.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      793 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/metrics/JSDivergence.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      512 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/metrics/KLDivergence.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      515 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/metrics/MeanAbsoluteError.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      513 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/metrics/MeanSquaredError.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      526 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/metrics/RootMeanSquaredError.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      311 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/metrics/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:40:34.584936 calotron-0.0.9/src/calotron/models/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      995 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/models/Calogantron.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     5872 2023-02-02 10:30:44.000000 calotron-0.0.9/src/calotron/models/Calotron.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2264 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/models/Discriminator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       68 2023-01-23 13:56:33.000000 calotron-0.0.9/src/calotron/models/Generator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     6913 2023-02-02 10:19:59.000000 calotron-0.0.9/src/calotron/models/Transformer.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      109 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/models/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:40:34.585936 calotron-0.0.9/src/calotron/simulators/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2022-12-15 16:20:53.000000 calotron-0.0.9/src/calotron/simulators/CaloSimulator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-02-02 10:17:11.000000 calotron-0.0.9/src/calotron/simulators/ExportCaloSimulator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      814 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/simulators/ExportSimulator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1677 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/simulators/Simulator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       78 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/simulators/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:40:34.586936 calotron-0.0.9/src/calotron/utils/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1354 2023-01-25 15:16:42.000000 calotron-0.0.9/src/calotron/utils/HPSingleton.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      248 2023-01-25 13:28:52.000000 calotron-0.0.9/src/calotron/utils/__init__.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1503 2023-01-23 11:41:30.000000 calotron-0.0.9/src/calotron/utils/checkActivations.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1038 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/utils/checkLoss.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1918 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/utils/checkMetrics.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      840 2023-01-23 16:41:54.000000 calotron-0.0.9/src/calotron/utils/checkOptimizer.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1013 2023-01-25 15:29:37.000000 calotron-0.0.9/src/calotron/utils/getModelSummary.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       22 2023-02-05 22:40:01.000000 calotron-0.0.9/src/calotron/version.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:40:34.580936 calotron-0.0.9/src/calotron.egg-info/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     3315 2023-02-05 22:40:34.000000 calotron-0.0.9/src/calotron.egg-info/PKG-INFO
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1932 2023-02-05 22:40:34.000000 calotron-0.0.9/src/calotron.egg-info/SOURCES.txt
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        1 2023-02-05 22:40:34.000000 calotron-0.0.9/src/calotron.egg-info/dependency_links.txt
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      222 2023-02-05 22:40:34.000000 calotron-0.0.9/src/calotron.egg-info/requires.txt
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        9 2023-02-05 22:40:34.000000 calotron-0.0.9/src/calotron.egg-info/top_level.txt
```

### Comparing `calotron-0.0.8/PKG-INFO` & `calotron-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: calotron
-Version: 0.0.8
-Summary: Transformer-based model to fast-simulate the LHCb ECAL detector
+Version: 0.0.9
+Summary: Transformer-based models to fast-simulate the LHCb ECAL detector
 Author-email: Matteo Barbetti <matteo.barbetti@fi.infn.it>, Lucio Anderlini <lucio.anderlini@fi.infn.it>
-License: MIT License
+License: GPLv3 License
 Project-URL: repository, https://github.com/mbarbetti/calotron
 Keywords: tensorflow,machine learning,deep learning,transformer,lhcb experiment,lamarr,ultra-fast simulation,calorimeter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: <=3.10,>=3.7
@@ -24,15 +24,15 @@
 License-File: LICENSE
 
 <div align="center">
   <img alt="calotron logo" src="https://raw.githubusercontent.com/mbarbetti/calotron/main/.github/images/calotron-logo.png" width="500"/>
 </div>
 
 <h3 align="center">
-  <em>Transformer-based model to fast-simulate the LHCb ECAL detector</em>
+  <em>Transformer-based models to fast-simulate the LHCb ECAL detector</em>
 </h3>
 
 <p align="center">
   <a href="https://www.tensorflow.org/versions"><img alt="TensorFlow versions" src="https://img.shields.io/badge/tensorflow-2.10%20|%202.11-f57000?style=flat"></a>
   <a href="https://pypi.python.org/pypi/calotron"><img alt="PyPI - Python versions" src="https://img.shields.io/pypi/pyversions/calotron"></a>
   <a href="https://pypi.python.org/pypi/calotron"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/calotron"></a>
   <!--
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: calotron Version: 0.0.8 Summary: Transformer-based
-model to fast-simulate the LHCb ECAL detector Author-email: Matteo Barbetti
+Metadata-Version: 2.1 Name: calotron Version: 0.0.9 Summary: Transformer-based
+models to fast-simulate the LHCb ECAL detector Author-email: Matteo Barbetti
 barbetti@fi.infn.it>, Lucio Anderlini
-anderlini@fi.infn.it> License: MIT License Project-URL: repository, https://
+anderlini@fi.infn.it> License: GPLv3 License Project-URL: repository, https://
 github.com/mbarbetti/calotron Keywords: tensorflow,machine learning,deep
 learning,transformer,lhcb experiment,lamarr,ultra-fast simulation,calorimeter
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
-Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
-Engineering :: Physics Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: <=3.10,>=3.7 Description-Content-Type:
-text/markdown Provides-Extra: standard Provides-Extra: advanced Provides-Extra:
-style Provides-Extra: tests License-File: LICENSE
+Science/Research Classifier: License :: OSI Approved :: GNU General Public
+License v3 (GPLv3) Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Physics Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: <=3.10,>=3.7
+Description-Content-Type: text/markdown Provides-Extra: standard Provides-
+Extra: advanced Provides-Extra: style Provides-Extra: tests License-File:
+LICENSE
                                 [calotron logo]
-   **** Transformer-based model to fast-simulate the LHCb ECAL detector ****
+  **** Transformer-based models to fast-simulate the LHCb ECAL detector ****
   [TensorFlow_versions] [PyPI_-_Python_versions] [PyPI_-_Version]  [GitHub_-
                        Style] [GitHub_-_Tests] [Codecov]
```

### Comparing `calotron-0.0.8/README.md` & `calotron-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <div align="center">
   <img alt="calotron logo" src="https://raw.githubusercontent.com/mbarbetti/calotron/main/.github/images/calotron-logo.png" width="500"/>
 </div>
 
 <h3 align="center">
-  <em>Transformer-based model to fast-simulate the LHCb ECAL detector</em>
+  <em>Transformer-based models to fast-simulate the LHCb ECAL detector</em>
 </h3>
 
 <p align="center">
   <a href="https://www.tensorflow.org/versions"><img alt="TensorFlow versions" src="https://img.shields.io/badge/tensorflow-2.10%20|%202.11-f57000?style=flat"></a>
   <a href="https://pypi.python.org/pypi/calotron"><img alt="PyPI - Python versions" src="https://img.shields.io/pypi/pyversions/calotron"></a>
   <a href="https://pypi.python.org/pypi/calotron"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/calotron"></a>
   <!--
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
                                 [calotron logo]
-   **** Transformer-based model to fast-simulate the LHCb ECAL detector ****
+  **** Transformer-based models to fast-simulate the LHCb ECAL detector ****
   [TensorFlow_versions] [PyPI_-_Python_versions] [PyPI_-_Version]  [GitHub_-
                        Style] [GitHub_-_Tests] [Codecov]
```

### Comparing `calotron-0.0.8/pyproject.toml` & `calotron-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calotron"
 dynamic = ["version"]
-description = "Transformer-based model to fast-simulate the LHCb ECAL detector"
+description = "Transformer-based models to fast-simulate the LHCb ECAL detector"
 readme = "README.md"
 requires-python = ">=3.7, <=3.10"
-license = {text = "MIT License"}
+license = {text = "GPLv3 License"}
 authors = [
   {name = "Matteo Barbetti", email = "matteo.barbetti@fi.infn.it"},
   {name = "Lucio Anderlini", email = "lucio.anderlini@fi.infn.it"},
 ]
 keywords = [
   "tensorflow",
   "machine learning",
@@ -22,15 +22,15 @@
   "lamarr",
   "ultra-fast simulation",
   "calorimeter",
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
-  "License :: OSI Approved :: MIT License",
+  "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: Scientific/Engineering :: Physics",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
```

### Comparing `calotron-0.0.8/src/calotron/callbacks/schedulers.py` & `calotron-0.0.9/src/calotron/callbacks/schedulers.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/layers/Attention.py` & `calotron-0.0.9/src/calotron/layers/Attention.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/layers/Decoder.py` & `calotron-0.0.9/src/calotron/layers/Decoder.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/layers/DeepSets.py` & `calotron-0.0.9/src/calotron/layers/DeepSets.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/layers/Encoder.py` & `calotron-0.0.9/src/calotron/layers/Encoder.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/layers/FeedForward.py` & `calotron-0.0.9/src/calotron/layers/FeedForward.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/layers/MultiActivations.py` & `calotron-0.0.9/src/calotron/layers/MultiActivations.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/layers/PositionalEmbedding.py` & `calotron-0.0.9/src/calotron/layers/PositionalEmbedding.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/losses/BaseLoss.py` & `calotron-0.0.9/src/calotron/losses/BaseLoss.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/losses/BinaryCrossentropy.py` & `calotron-0.0.9/src/calotron/losses/BinaryCrossentropy.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/losses/CaloLoss.py` & `calotron-0.0.9/src/calotron/losses/CaloLoss.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/losses/JSDivergence.py` & `calotron-0.0.9/src/calotron/losses/JSDivergence.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/losses/KLDivergence.py` & `calotron-0.0.9/src/calotron/losses/KLDivergence.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/losses/MeanAbsoluteError.py` & `calotron-0.0.9/src/calotron/losses/MeanAbsoluteError.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/losses/MeanSquaredError.py` & `calotron-0.0.9/src/calotron/losses/MeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/metrics/Accuracy.py` & `calotron-0.0.9/src/calotron/metrics/Accuracy.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/metrics/BaseMetric.py` & `calotron-0.0.9/src/calotron/metrics/BaseMetric.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/metrics/BinaryCrossentropy.py` & `calotron-0.0.9/src/calotron/metrics/BinaryCrossentropy.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/metrics/JSDivergence.py` & `calotron-0.0.9/src/calotron/metrics/JSDivergence.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/metrics/KLDivergence.py` & `calotron-0.0.9/src/calotron/metrics/KLDivergence.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/metrics/MeanAbsoluteError.py` & `calotron-0.0.9/src/calotron/metrics/MeanAbsoluteError.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/metrics/MeanSquaredError.py` & `calotron-0.0.9/src/calotron/metrics/MeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/metrics/RootMeanSquaredError.py` & `calotron-0.0.9/src/calotron/metrics/RootMeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/models/Calogantron.py` & `calotron-0.0.9/src/calotron/models/Calogantron.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/models/Calotron.py` & `calotron-0.0.9/src/calotron/models/Calotron.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/models/Discriminator.py` & `calotron-0.0.9/src/calotron/models/Discriminator.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/models/Transformer.py` & `calotron-0.0.9/src/calotron/models/Transformer.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/simulators/ExportSimulator.py` & `calotron-0.0.9/src/calotron/simulators/ExportSimulator.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/simulators/Simulator.py` & `calotron-0.0.9/src/calotron/simulators/Simulator.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/utils/HPSingleton.py` & `calotron-0.0.9/src/calotron/utils/HPSingleton.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/utils/checkActivations.py` & `calotron-0.0.9/src/calotron/utils/checkActivations.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/utils/checkLoss.py` & `calotron-0.0.9/src/calotron/utils/checkLoss.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/utils/checkMetrics.py` & `calotron-0.0.9/src/calotron/utils/checkMetrics.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/utils/checkOptimizer.py` & `calotron-0.0.9/src/calotron/utils/checkOptimizer.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron/utils/getModelSummary.py` & `calotron-0.0.9/src/calotron/utils/getModelSummary.py`

 * *Files identical despite different names*

### Comparing `calotron-0.0.8/src/calotron.egg-info/PKG-INFO` & `calotron-0.0.9/src/calotron.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: calotron
-Version: 0.0.8
-Summary: Transformer-based model to fast-simulate the LHCb ECAL detector
+Version: 0.0.9
+Summary: Transformer-based models to fast-simulate the LHCb ECAL detector
 Author-email: Matteo Barbetti <matteo.barbetti@fi.infn.it>, Lucio Anderlini <lucio.anderlini@fi.infn.it>
-License: MIT License
+License: GPLv3 License
 Project-URL: repository, https://github.com/mbarbetti/calotron
 Keywords: tensorflow,machine learning,deep learning,transformer,lhcb experiment,lamarr,ultra-fast simulation,calorimeter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: <=3.10,>=3.7
@@ -24,15 +24,15 @@
 License-File: LICENSE
 
 <div align="center">
   <img alt="calotron logo" src="https://raw.githubusercontent.com/mbarbetti/calotron/main/.github/images/calotron-logo.png" width="500"/>
 </div>
 
 <h3 align="center">
-  <em>Transformer-based model to fast-simulate the LHCb ECAL detector</em>
+  <em>Transformer-based models to fast-simulate the LHCb ECAL detector</em>
 </h3>
 
 <p align="center">
   <a href="https://www.tensorflow.org/versions"><img alt="TensorFlow versions" src="https://img.shields.io/badge/tensorflow-2.10%20|%202.11-f57000?style=flat"></a>
   <a href="https://pypi.python.org/pypi/calotron"><img alt="PyPI - Python versions" src="https://img.shields.io/pypi/pyversions/calotron"></a>
   <a href="https://pypi.python.org/pypi/calotron"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/calotron"></a>
   <!--
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: calotron Version: 0.0.8 Summary: Transformer-based
-model to fast-simulate the LHCb ECAL detector Author-email: Matteo Barbetti
+Metadata-Version: 2.1 Name: calotron Version: 0.0.9 Summary: Transformer-based
+models to fast-simulate the LHCb ECAL detector Author-email: Matteo Barbetti
 barbetti@fi.infn.it>, Lucio Anderlini
-anderlini@fi.infn.it> License: MIT License Project-URL: repository, https://
+anderlini@fi.infn.it> License: GPLv3 License Project-URL: repository, https://
 github.com/mbarbetti/calotron Keywords: tensorflow,machine learning,deep
 learning,transformer,lhcb experiment,lamarr,ultra-fast simulation,calorimeter
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
-Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
-Engineering :: Physics Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: <=3.10,>=3.7 Description-Content-Type:
-text/markdown Provides-Extra: standard Provides-Extra: advanced Provides-Extra:
-style Provides-Extra: tests License-File: LICENSE
+Science/Research Classifier: License :: OSI Approved :: GNU General Public
+License v3 (GPLv3) Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Physics Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: <=3.10,>=3.7
+Description-Content-Type: text/markdown Provides-Extra: standard Provides-
+Extra: advanced Provides-Extra: style Provides-Extra: tests License-File:
+LICENSE
                                 [calotron logo]
-   **** Transformer-based model to fast-simulate the LHCb ECAL detector ****
+  **** Transformer-based models to fast-simulate the LHCb ECAL detector ****
   [TensorFlow_versions] [PyPI_-_Python_versions] [PyPI_-_Version]  [GitHub_-
                        Style] [GitHub_-_Tests] [Codecov]
```

### Comparing `calotron-0.0.8/src/calotron.egg-info/SOURCES.txt` & `calotron-0.0.9/src/calotron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

