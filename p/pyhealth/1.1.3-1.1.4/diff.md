# Comparing `tmp/pyhealth-1.1.3.tar.gz` & `tmp/pyhealth-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhealth-1.1.3.tar", last modified: Tue Jan 24 21:13:45 2023, max compression
+gzip compressed data, was "pyhealth-1.1.4.tar", last modified: Wed May 31 23:20:50 2023, max compression
```

## Comparing `pyhealth-1.1.3.tar` & `pyhealth-1.1.4.tar`

### file list

```diff
@@ -1,76 +1,113 @@
-drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-01-24 21:13:45.582268 pyhealth-1.1.3/
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    17196 2023-01-24 21:13:45.582268 pyhealth-1.1.3/PKG-INFO
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    16400 2023-01-21 20:32:12.000000 pyhealth-1.1.3/README.rst
-drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-01-24 21:13:45.567268 pyhealth-1.1.3/leaderboard/
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      107 2022-11-15 23:33:35.000000 pyhealth-1.1.3/leaderboard/__init__.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      997 2022-12-05 22:44:15.000000 pyhealth-1.1.3/leaderboard/ext_plot.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    11349 2023-01-21 20:32:12.000000 pyhealth-1.1.3/leaderboard/leaderboard_gen.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      659 2022-12-05 22:44:15.000000 pyhealth-1.1.3/leaderboard/rtd_build_trigger.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    15730 2023-01-21 20:32:12.000000 pyhealth-1.1.3/leaderboard/utils.py
-drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-01-24 21:13:45.568268 pyhealth-1.1.3/pyhealth/
--rwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      484 2023-01-24 21:13:19.000000 pyhealth-1.1.3/pyhealth/__init__.py
-drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-01-24 21:13:45.570268 pyhealth-1.1.3/pyhealth/data/
--rwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)       57 2022-10-25 21:09:46.000000 pyhealth-1.1.3/pyhealth/data/__init__.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    16059 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/data/data.py
-drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-01-24 21:13:45.572268 pyhealth-1.1.3/pyhealth/datasets/
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      324 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/datasets/__init__.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    13853 2023-01-22 04:25:41.000000 pyhealth-1.1.3/pyhealth/datasets/base_dataset.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    19361 2023-01-22 04:25:44.000000 pyhealth-1.1.3/pyhealth/datasets/eicu.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    12830 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/datasets/mimic3.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    13138 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/datasets/mimic4.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    15223 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/datasets/omop.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    17085 2023-01-22 17:53:39.000000 pyhealth-1.1.3/pyhealth/datasets/sample_dataset.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     3288 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/datasets/splitter.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     3235 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/datasets/utils.py
-drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-01-24 21:13:45.573268 pyhealth-1.1.3/pyhealth/medcode/
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      361 2022-11-20 05:36:01.000000 pyhealth-1.1.3/pyhealth/medcode/__init__.py
-drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-01-24 21:13:45.576268 pyhealth-1.1.3/pyhealth/medcode/codes/
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2022-10-23 04:16:03.000000 pyhealth-1.1.3/pyhealth/medcode/codes/__init__.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     2166 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/medcode/codes/atc.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      468 2022-11-16 04:04:19.000000 pyhealth-1.1.3/pyhealth/medcode/codes/ccscm.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      463 2022-11-16 04:04:19.000000 pyhealth-1.1.3/pyhealth/medcode/codes/ccsproc.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      760 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/medcode/codes/icd10cm.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      532 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/medcode/codes/icd10proc.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      919 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/medcode/codes/icd9cm.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      751 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/medcode/codes/icd9proc.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      526 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/medcode/codes/ndc.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      446 2022-11-16 04:04:19.000000 pyhealth-1.1.3/pyhealth/medcode/codes/rxnorm.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     4165 2023-01-22 21:13:02.000000 pyhealth-1.1.3/pyhealth/medcode/cross_map.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     5925 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/medcode/inner_map.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     1130 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/medcode/utils.py
-drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-01-24 21:13:45.577268 pyhealth-1.1.3/pyhealth/metrics/
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      182 2022-11-16 04:04:19.000000 pyhealth-1.1.3/pyhealth/metrics/__init__.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     3920 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/metrics/binary.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      915 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/metrics/drug_recommendation.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     6274 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/metrics/multiclass.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     9813 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/metrics/multilabel.py
-drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-01-24 21:13:45.580268 pyhealth-1.1.3/pyhealth/models/
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      413 2023-01-22 04:09:51.000000 pyhealth-1.1.3/pyhealth/models/__init__.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    11796 2023-01-22 17:36:05.000000 pyhealth-1.1.3/pyhealth/models/base_model.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    16767 2023-01-22 17:37:03.000000 pyhealth-1.1.3/pyhealth/models/cnn.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    13295 2023-01-22 18:02:41.000000 pyhealth-1.1.3/pyhealth/models/deepr.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    14744 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/models/gamenet.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     7802 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/models/micron.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    14146 2023-01-22 17:52:53.000000 pyhealth-1.1.3/pyhealth/models/mlp.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    19005 2023-01-22 17:45:36.000000 pyhealth-1.1.3/pyhealth/models/retain.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    17494 2023-01-22 17:49:54.000000 pyhealth-1.1.3/pyhealth/models/rnn.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    23965 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/models/safedrug.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    19220 2023-01-22 18:01:48.000000 pyhealth-1.1.3/pyhealth/models/transformer.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     1120 2022-11-16 04:04:19.000000 pyhealth-1.1.3/pyhealth/models/utils.py
-drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-01-24 21:13:45.581268 pyhealth-1.1.3/pyhealth/tasks/
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      742 2022-10-22 22:30:03.000000 pyhealth-1.1.3/pyhealth/tasks/__init__.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    12436 2023-01-24 05:59:57.000000 pyhealth-1.1.3/pyhealth/tasks/drug_recommendation.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    11374 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/tasks/length_of_stay_prediction.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    11213 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/tasks/mortality_prediction.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    12115 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/tasks/readmission_prediction.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     8814 2023-01-22 06:28:57.000000 pyhealth-1.1.3/pyhealth/tokenizer.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    13640 2023-01-21 20:32:12.000000 pyhealth-1.1.3/pyhealth/trainer.py
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      721 2022-11-16 04:04:19.000000 pyhealth-1.1.3/pyhealth/utils.py
-drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-01-24 21:13:45.570268 pyhealth-1.1.3/pyhealth.egg-info/
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    17196 2023-01-24 21:13:45.000000 pyhealth-1.1.3/pyhealth.egg-info/PKG-INFO
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     1824 2023-01-24 21:13:45.000000 pyhealth-1.1.3/pyhealth.egg-info/SOURCES.txt
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        1 2023-01-24 21:13:45.000000 pyhealth-1.1.3/pyhealth.egg-info/dependency_links.txt
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)       86 2023-01-24 21:13:45.000000 pyhealth-1.1.3/pyhealth.egg-info/requires.txt
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)       21 2023-01-24 21:13:45.000000 pyhealth-1.1.3/pyhealth.egg-info/top_level.txt
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)       80 2023-01-24 21:13:45.582268 pyhealth-1.1.3/setup.cfg
--rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     1825 2023-01-24 21:12:35.000000 pyhealth-1.1.3/setup.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.046789 pyhealth-1.1.4/
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    27573 2023-05-31 23:20:50.046789 pyhealth-1.1.4/PKG-INFO
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    26704 2023-05-31 23:20:13.000000 pyhealth-1.1.4/README.rst
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.030789 pyhealth-1.1.4/leaderboard/
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      107 2022-11-15 23:33:35.000000 pyhealth-1.1.4/leaderboard/__init__.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      997 2022-12-05 22:44:15.000000 pyhealth-1.1.4/leaderboard/ext_plot.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    11349 2023-01-21 20:32:12.000000 pyhealth-1.1.4/leaderboard/leaderboard_gen.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      659 2022-12-05 22:44:15.000000 pyhealth-1.1.4/leaderboard/rtd_build_trigger.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    15730 2023-01-21 20:32:12.000000 pyhealth-1.1.4/leaderboard/utils.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.031788 pyhealth-1.1.4/pyhealth/
+-rwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      480 2023-05-31 23:00:16.000000 pyhealth-1.1.4/pyhealth/__init__.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.032788 pyhealth-1.1.4/pyhealth/calib/
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)       54 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/calib/__init__.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      811 2023-05-26 05:41:50.000000 pyhealth-1.1.4/pyhealth/calib/base_classes.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.033789 pyhealth-1.1.4/pyhealth/calib/calibration/
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      369 2023-05-25 20:59:47.000000 pyhealth-1.1.4/pyhealth/calib/calibration/__init__.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     8625 2023-05-26 05:41:50.000000 pyhealth-1.1.4/pyhealth/calib/calibration/dircal.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     9715 2023-05-25 21:19:27.000000 pyhealth-1.1.4/pyhealth/calib/calibration/hb.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.033789 pyhealth-1.1.4/pyhealth/calib/calibration/kcal/
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    13358 2023-05-26 05:41:50.000000 pyhealth-1.1.4/pyhealth/calib/calibration/kcal/__init__.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     3820 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/calib/calibration/kcal/bw.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     4427 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/calib/calibration/kcal/embed_data.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     4411 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/calib/calibration/kcal/kde.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     6506 2023-05-26 05:41:50.000000 pyhealth-1.1.4/pyhealth/calib/calibration/temperature_scale.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.034788 pyhealth-1.1.4/pyhealth/calib/predictionset/
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      178 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/calib/predictionset/__init__.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     6962 2023-05-25 21:33:06.000000 pyhealth-1.1.4/pyhealth/calib/predictionset/label.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.034788 pyhealth-1.1.4/pyhealth/calib/predictionset/scrib/
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    12954 2023-05-26 05:52:58.000000 pyhealth-1.1.4/pyhealth/calib/predictionset/scrib/__init__.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    12536 2023-05-26 05:41:50.000000 pyhealth-1.1.4/pyhealth/calib/predictionset/scrib/quicksearch.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     2465 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/calib/utils.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.035788 pyhealth-1.1.4/pyhealth/data/
+-rwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)       57 2022-10-25 21:09:46.000000 pyhealth-1.1.4/pyhealth/data/__init__.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    16094 2023-02-27 02:46:09.000000 pyhealth-1.1.4/pyhealth/data/data.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.037788 pyhealth-1.1.4/pyhealth/datasets/
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      571 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/datasets/__init__.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    15709 2023-05-06 20:10:35.000000 pyhealth-1.1.4/pyhealth/datasets/base_ehr_dataset.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     5860 2023-05-31 21:34:22.000000 pyhealth-1.1.4/pyhealth/datasets/base_signal_dataset.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    25624 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/datasets/eicu.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     5295 2023-02-27 02:46:09.000000 pyhealth-1.1.4/pyhealth/datasets/isruc.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    14685 2023-02-27 02:46:09.000000 pyhealth-1.1.4/pyhealth/datasets/mimic3.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    16602 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/datasets/mimic4.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    25226 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/datasets/mimicextract.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    16569 2023-02-27 02:46:09.000000 pyhealth-1.1.4/pyhealth/datasets/omop.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    22006 2023-02-27 02:46:09.000000 pyhealth-1.1.4/pyhealth/datasets/sample_dataset.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     4960 2023-05-31 22:23:54.000000 pyhealth-1.1.4/pyhealth/datasets/shhs.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     5379 2023-02-27 02:46:09.000000 pyhealth-1.1.4/pyhealth/datasets/sleepedf.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     3308 2023-02-27 02:46:09.000000 pyhealth-1.1.4/pyhealth/datasets/splitter.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     3910 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/datasets/utils.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.038788 pyhealth-1.1.4/pyhealth/medcode/
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      361 2022-11-20 05:36:01.000000 pyhealth-1.1.4/pyhealth/medcode/__init__.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.040789 pyhealth-1.1.4/pyhealth/medcode/codes/
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2022-10-23 04:16:03.000000 pyhealth-1.1.4/pyhealth/medcode/codes/__init__.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     2166 2023-01-21 20:32:12.000000 pyhealth-1.1.4/pyhealth/medcode/codes/atc.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      468 2022-11-16 04:04:19.000000 pyhealth-1.1.4/pyhealth/medcode/codes/ccscm.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      463 2022-11-16 04:04:19.000000 pyhealth-1.1.4/pyhealth/medcode/codes/ccsproc.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      760 2023-01-21 20:32:12.000000 pyhealth-1.1.4/pyhealth/medcode/codes/icd10cm.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      532 2023-01-21 20:32:12.000000 pyhealth-1.1.4/pyhealth/medcode/codes/icd10proc.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      919 2023-01-21 20:32:12.000000 pyhealth-1.1.4/pyhealth/medcode/codes/icd9cm.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      751 2023-01-21 20:32:12.000000 pyhealth-1.1.4/pyhealth/medcode/codes/icd9proc.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      526 2023-01-21 20:32:12.000000 pyhealth-1.1.4/pyhealth/medcode/codes/ndc.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      446 2022-11-16 04:04:19.000000 pyhealth-1.1.4/pyhealth/medcode/codes/rxnorm.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     4341 2023-02-27 02:46:09.000000 pyhealth-1.1.4/pyhealth/medcode/cross_map.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     5983 2023-02-27 02:46:09.000000 pyhealth-1.1.4/pyhealth/medcode/inner_map.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     1258 2023-05-25 20:59:47.000000 pyhealth-1.1.4/pyhealth/medcode/utils.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.041788 pyhealth-1.1.4/pyhealth/metrics/
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      182 2022-11-16 04:04:19.000000 pyhealth-1.1.4/pyhealth/metrics/__init__.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     4420 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/metrics/binary.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     7713 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/metrics/calibration.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      915 2023-01-21 20:32:12.000000 pyhealth-1.1.4/pyhealth/metrics/drug_recommendation.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    10161 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/metrics/multiclass.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    10389 2023-05-25 20:59:47.000000 pyhealth-1.1.4/pyhealth/metrics/multilabel.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     4220 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/metrics/prediction_set.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.045788 pyhealth-1.1.4/pyhealth/models/
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     1010 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/__init__.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    23383 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/adacare.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    29600 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/agent.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    11804 2023-02-27 02:46:09.000000 pyhealth-1.1.4/pyhealth/models/base_model.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    17013 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/cnn.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    37784 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/concare.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    13936 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/contrawr.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    13607 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/deepr.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    14807 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/gamenet.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    25802 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/grasp.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     7808 2023-02-27 02:46:09.000000 pyhealth-1.1.4/pyhealth/models/micron.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    14475 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/mlp.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    27555 2023-05-10 02:09:57.000000 pyhealth-1.1.4/pyhealth/models/molerec.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    16779 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/retain.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    17762 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/rnn.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    23971 2023-03-06 18:28:48.000000 pyhealth-1.1.4/pyhealth/models/safedrug.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    14056 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/sparcnet.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    25422 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/stagenet.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    19184 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/tcn.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    19493 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/models/transformer.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     1222 2023-02-27 02:46:09.000000 pyhealth-1.1.4/pyhealth/models/utils.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.046789 pyhealth-1.1.4/pyhealth/tasks/
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      931 2023-05-31 22:31:40.000000 pyhealth-1.1.4/pyhealth/tasks/__init__.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    14328 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/tasks/drug_recommendation.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    11374 2023-01-21 20:32:12.000000 pyhealth-1.1.4/pyhealth/tasks/length_of_stay_prediction.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    14535 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/tasks/mortality_prediction.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    15585 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/tasks/readmission_prediction.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    13061 2023-05-31 23:00:01.000000 pyhealth-1.1.4/pyhealth/tasks/sleep_staging.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    13475 2023-02-27 02:46:09.000000 pyhealth-1.1.4/pyhealth/tokenizer.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    14469 2023-05-09 22:43:10.000000 pyhealth-1.1.4/pyhealth/trainer.py
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      721 2022-11-16 04:04:19.000000 pyhealth-1.1.4/pyhealth/utils.py
+drwxrwxr-x   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        0 2023-05-31 23:20:50.031788 pyhealth-1.1.4/pyhealth.egg-info/
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)    27573 2023-05-31 23:20:49.000000 pyhealth-1.1.4/pyhealth.egg-info/PKG-INFO
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     2905 2023-05-31 23:20:49.000000 pyhealth-1.1.4/pyhealth.egg-info/SOURCES.txt
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)        1 2023-05-31 23:20:49.000000 pyhealth-1.1.4/pyhealth.egg-info/dependency_links.txt
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)      142 2023-05-31 23:20:49.000000 pyhealth-1.1.4/pyhealth.egg-info/requires.txt
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)       21 2023-05-31 23:20:49.000000 pyhealth-1.1.4/pyhealth.egg-info/top_level.txt
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)       80 2023-05-31 23:20:50.047788 pyhealth-1.1.4/setup.cfg
+-rw-rw-r--   0 chaoqiy2 (1098463) chaoqiy2 (1098463)     1898 2023-05-31 23:07:53.000000 pyhealth-1.1.4/setup.py
```

### Comparing `pyhealth-1.1.3/PKG-INFO` & `pyhealth-1.1.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyhealth
-Version: 1.1.3
-Summary: A Python library for healthcare AI
+Version: 1.1.4
+Summary: A Deep Learning Python Toolkit for Healthcare Applications
 Home-page: https://github.com/sunlabuiuc/pyhealth
-Author: Chaoqi Yang, Zhenbang Wu, Patrick Jiang
+Author: Chaoqi Yang, Zhenbang Wu, Patrick Jiang, Zhen Lin, Benjamin Danek, Junyi Gao, Jimeng Sun
 Author-email: chaoqiy2@illinois.edu
 Keywords: heathcare AI,healthcare,electronic health records,EHRs,machine learning,data mining,neural networks,deep learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -25,32 +25,37 @@
 
 
 .. image:: https://readthedocs.org/projects/pyhealth/badge/?version=latest
    :target: https://pyhealth.readthedocs.io/en/latest/
    :alt: Documentation status
    
 
-.. image:: https://img.shields.io/github/stars/yzhao062/pyhealth.svg
+.. image:: https://img.shields.io/github/stars/sunlabuiuc/pyhealth.svg
    :target: https://github.com/sunlabuiuc/pyhealth/stargazers
    :alt: GitHub stars
 
 
-.. image:: https://img.shields.io/github/forks/yzhao062/pyhealth.svg?color=blue
+.. image:: https://img.shields.io/github/forks/sunlabuiuc/pyhealth.svg?color=blue
    :target: https://github.com/sunlabuiuc/pyhealth/network
    :alt: GitHub forks
 
 
 .. image:: https://pepy.tech/badge/pyhealth
    :target: https://pepy.tech/project/pyhealth
    :alt: Downloads
 
 
-.. image:: https://pepy.tech/badge/pyhealth/month
-   :target: https://pepy.tech/project/pyhealth
-   :alt: Downloads
+.. image:: https://img.shields.io/badge/Tutorials-Google%20Colab-red
+   :target: https://pyhealth.readthedocs.io/en/latest/tutorials.html
+   :alt: Tutorials
+
+
+.. image:: https://img.shields.io/badge/YouTube-16%20Videos-red
+   :target: https://www.youtube.com/playlist?list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV
+   :alt: YouTube
 
 
 
 .. -----
 
 
 .. **Build Status & Coverage & Maintainability & License**
@@ -71,271 +76,358 @@
 
 
 .. .. image:: https://img.shields.io/github/license/yzhao062/pyhealth
 ..    :target: https://github.com/yzhao062/pyhealth/blob/master/LICENSE
 ..    :alt: License
 
 PyHealth is designed for both **ML researchers and medical practitioners**. We can make your **healthcare AI applications** easier to deploy and more flexible and customizable. `[Tutorials] <https://pyhealth.readthedocs.io/>`_
- 
-**[News!]** We are running the "PyHealth Live" gathering at 8 PM CST every Wednesday night! Welcome to join over `zoom <https://illinois.zoom.us/j/87450975602?pwd=ckQyaHhkRitlUzlwYUY3NjdEQ0pFdz09>`_. Check out `PyHealth Live <https://github.com/sunlabuiuc/PyHealth/blob/master/docs/live.rst>`_ for more information and watch the `Live Videos <https://www.youtube.com/playlist?list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV>`_.
-
-----------
-
-
-1. Introduction
---------------------------
 
-.. .. image:: https://raw.githubusercontent.com/yzhao062/PyHealth/master/docs/images/logo.png
-..    :target: https://raw.githubusercontent.com/yzhao062/PyHealth/master/docs/images/logo.png
-..    :alt: PyHealth Logo
-..    :align: center
+ **[News!]** Our PyHealth is accepted by KDD 2023 Tutorial Track! We will present a 3-hour tutorial on PyHealth at `[KDD 2023] <https://kdd.org/kdd2023/>`_, August 6-10, Long Beach, CA.
 
-PyHealth can support **diverse electronic health records (EHRs)** such as MIMIC and eICU and all OMOP-CDM based databases and provide **various advanced deep learning algorithms** for handling **important healthcare tasks** such as diagnosis-based drug recommendation, patient hospitalization and mortality prediction, and ICU length stay forecasting, etc.  
+.. image:: figure/poster.png
+   :width: 810
 
-*Build a healthcare AI pipeline can be as short as 10 lines of code in PyHealth*.
+..
 
-2. Installation
------------------
+1. Installation :rocket:
+----------------------------
 
 - You could install from PyPi:
 
-.. code-block:: bash
+.. code-block:: sh
 
     pip install pyhealth
 
 - or from github source:
 
-.. code-block:: bash
+.. code-block:: sh
 
-   git clone https://github.com/sunlabuiuc/PyHealth.git
-   cd pyhealth
-   pip install .
+    pip install .
 
-- Required Dependencies
 
-.. code-block:: bash
+2. Introduction :book:
+--------------------------
+``pyhealth`` provides these functionalities (we are still enriching some modules):
 
-    python>=3.8
-    torch>=1.8.0
-    rdkit>=2022.03.4
-    scikit-learn>=0.24.2
-    networkx>=2.6.3
-    pandas>=1.3.2
-    tqdm
+.. image:: figure/overview.png
+   :width: 770
 
+You can use the following functions independently:
 
-3. Modules
---------------------------
+- **Dataset**: ``MIMIC-III``, ``MIMIC-IV``, ``eICU``, ``OMOP-CDM``, ``customized EHR datasets``, etc.
+- **Tasks**: ``diagnosis-based drug recommendation``, ``patient hospitalization and mortality prediction``, ``length stay forecasting``, etc. 
+- **ML models**: ``CNN``, ``LSTM``, ``GRU``, ``LSTM``, ``RETAIN``, ``SafeDrug``, ``Deepr``, etc.
+
+*Building a healthcare AI pipeline can be as short as 10 lines of code in PyHealth*.
+
+
+3. Build ML Pipelines :trophy:
+---------------------------------
 
 All healthcare tasks in our package follow a **five-stage pipeline**: 
 
- load dataset -> define task function -> build ML/DL model -> model training -> inference
+.. image:: figure/five-stage-pipeline.png
+   :width: 640
 
-! We try hard to make sure each stage is as separate as possibe, so that people can customize their own pipeline by only using our data processing steps or the ML models. Each step will call one module and we introduce them using an example.
+..
+
+ We try hard to make sure each stage is as separate as possible, so that people can customize their own pipeline by only using our data processing steps or the ML models.
 
-3.1 An ML Pipeline Example 
-^^^^^^^^^^^^^^^^^^^^^^^^^^
+Module 1: <pyhealth.datasets>
+""""""""""""""""""""""""""""""""""""
 
-* **STEP 1: <pyhealth.datasets>** provides a clean structure for the dataset, independent from the tasks. We support ``MIMIC-III``, ``MIMIC-IV`` and ``eICU``, as well as the standard ``OMOP-formatted data``. The dataset is stored in a unified ``Patient-Visit-Event`` structure.
+``pyhealth.datasets`` provides a clean structure for the dataset, independent from the tasks. We support `MIMIC-III`, `MIMIC-IV` and `eICU`, etc. The output (mimic3base) is a multi-level dictionary structure (see illustration below).
 
 .. code-block:: python
 
     from pyhealth.datasets import MIMIC3Dataset
+
     mimic3base = MIMIC3Dataset(
+        # root directory of the dataset
         root="https://storage.googleapis.com/pyhealth/Synthetic_MIMIC-III/", 
+        # raw CSV table name
         tables=["DIAGNOSES_ICD", "PROCEDURES_ICD", "PRESCRIPTIONS"],
-        # map all NDC codes to ATC 3-rd level codes in these tables
-        code_mapping={"NDC": ("ATC", {"target_kwargs": {"level": 3}})},
+        # map all NDC codes to CCS codes in these tables
+        code_mapping={"NDC": "CCSCM"},
     )
 
-User could also store their own dataset into our ``<pyhealth.datasets.SampleDataset>`` structure and then follow the same pipeline below, see `Tutorial <https://colab.research.google.com/drive/1UurxwAAov1bL_5OO3gQJ4gAa_paeJwJp?usp=sharing>`_
+.. image:: figure/structured-dataset.png
+   :width: 400
 
-* **STEP 2: <pyhealth.tasks>** inputs the ``<pyhealth.datasets>`` object and defines how to process each patient's data into a set of samples for the tasks. In the package, we provide several task examples, such as ``drug recommendation`` and ``length of stay prediction``.
+..
+
+Module 2: <pyhealth.tasks>
+""""""""""""""""""""""""""""""""""""
+
+``pyhealth.tasks`` defines how to process each patient's data into a set of samples for the tasks. In the package, we provide several task examples, such as ``drug recommendation`` and ``length of stay prediction``. **It is easy to customize your own tasks following our** `template <https://colab.research.google.com/drive/1r7MYQR_5yCJGpK_9I9-A10HmpupZuIN-?usp=sharing>`_.
 
 .. code-block:: python
 
-    from pyhealth.tasks import drug_recommendation_mimic3_fn
+    from pyhealth.tasks import readmission_prediction_mimic3_fn
+
+    mimic3sample = mimic3base.set_task(task_fn=readmission_prediction_mimic3_fn) # use default task
+    mimic3sample.samples[0] # show the information of the first sample
+    """
+    {
+        'visit_id': '100183',
+        'patient_id': '175',
+        'conditions': ['5990', '4280', '2851', '4240', '2749', '9982', 'E8499', '42831', '34600'],
+        'procedures': ['0040', '3931', '7769'],
+        'drugs': ['N06DA02', 'V06DC01', 'B01AB01', 'A06AA02', 'R03AC02', 'H03AA01', 'J01FA09'],
+        'label': 0
+    }
+    """
+
     from pyhealth.datasets import split_by_patient, get_dataloader
 
-    mimic3sample = mimic3base.set_task(task_fn=drug_recommendation_mimic3_fn) # use default task
     train_ds, val_ds, test_ds = split_by_patient(mimic3sample, [0.8, 0.1, 0.1])
-
-    # create dataloaders (torch.data.DataLoader)
     train_loader = get_dataloader(train_ds, batch_size=32, shuffle=True)
     val_loader = get_dataloader(val_ds, batch_size=32, shuffle=False)
     test_loader = get_dataloader(test_ds, batch_size=32, shuffle=False)
 
-* **STEP 3: <pyhealth.models>** provides the healthcare ML models using ``<pyhealth.models>``. This module also provides model layers, such as ``pyhealth.models.RETAINLayer`` for building customized ML architectures. Our model layers can used as easily as ``torch.nn.Linear``.
+Module 3: <pyhealth.models>
+""""""""""""""""""""""""""""""""""""
+
+``pyhealth.models`` provides different ML models with very similar argument configs.
 
 .. code-block:: python
 
     from pyhealth.models import Transformer
 
     model = Transformer(
         dataset=mimic3sample,
-        feature_keys=["conditions", "procedures"],
-        label_key="drugs",
-        mode="multilabel",
+        feature_keys=["conditions", "procedures", "drug"],
+        label_key="label",
+        mode="binary",
     )
 
-* **STEP 4: <pyhealth.trainer>** is the training manager with ``train_loader``, the ``val_loader``, ``val_metric``, and specify other arguemnts, such as epochs, optimizer, learning rate, etc. The trainer will automatically save the best model and output the path in the end.
+Module 4: <pyhealth.trainer>
+""""""""""""""""""""""""""""""""""""
+
+``pyhealth.trainer`` can specify training arguments, such as epochs, optimizer, learning rate, etc. The trainer will automatically save the best model and output the path in the end.
 
 .. code-block:: python
     
     from pyhealth.trainer import Trainer
 
     trainer = Trainer(model=model)
     trainer.train(
         train_dataloader=train_loader,
         val_dataloader=val_loader,
         epochs=50,
         monitor="pr_auc_samples",
     )
 
-* **STEP 5: <pyhealth.metrics>** provides several **common evaluation metrics** (refer to `Doc <https://pyhealth.readthedocs.io/en/latest/api/metrics.html>`_ and see what are available) and **special metrics** in healthcare, such as drug-drug interaction (DDI) rate.
+Module 5: <pyhealth.metrics>
+""""""""""""""""""""""""""""""""""""
+
+``pyhealth.metrics`` provides several **common evaluation metrics** (refer to `Doc <https://pyhealth.readthedocs.io/en/latest/api/metrics.html>`_ and see what are available).
 
 .. code-block:: python
-    
+
+    # method 1
     trainer.evaluate(test_loader)
+    
+    # method 2
+    from pyhealth.metrics.binary import binary_metrics_fn
 
-3.2 Medical Code Map
-^^^^^^^^^^^^^^^^^^^^^^^^^^
+    y_true, y_prob, loss = trainer.inference(test_loader)
+    binary_metrics_fn(y_true, y_prob, metrics=["pr_auc", "roc_auc"])
 
-* **<pyhealth.codemap>** provides two core functionalities: (i) looking up information for a given medical code (e.g., name, category, sub-concept); (ii) mapping codes across coding systems (e.g., ICD9CM to CCSCM). **This module can be independently applied to your research.**
+4. Medical Code Map :hospital: 
+---------------------------------
 
-* For code mapping between two coding systems
+``pyhealth.codemap`` provides two core functionalities. **This module can be used independently.**
 
-.. code-block:: python
+* For code ontology lookup within one medical coding system (e.g., name, category, sub-concept); 
 
-    from pyhealth.medcode import CrossMap
+.. code-block:: python
 
-    codemap = CrossMap.load("ICD9CM", "CCSCM")
-    codemap.map("82101") # use it like a dict
+    from pyhealth.medcode import InnerMap
 
-    codemap = CrossMap.load("NDC", "ATC")
-    codemap.map("00527051210")
+    icd9cm = InnerMap.load("ICD9CM")
+    icd9cm.lookup("428.0")
+    # `Congestive heart failure, unspecified`
+    icd9cm.get_ancestors("428.0")
+    # ['428', '420-429.99', '390-459.99', '001-999.99']
+    
+    atc = InnerMap.load("ATC")
+    atc.lookup("M01AE51")
+    # `ibuprofen, combinations`
+    atc.lookup("M01AE51", "drugbank_id")
+    # `DB01050`
+    atc.lookup("M01AE51", "description")
+    # Ibuprofen is a non-steroidal anti-inflammatory drug (NSAID) derived ...
+    atc.lookup("M01AE51", "indication")
+    # Ibuprofen is the most commonly used and prescribed NSAID. It is very common over the ...
 
-* For code ontology lookup within one system
+* For code mapping between two coding systems (e.g., ICD9CM to CCSCM). 
 
 .. code-block:: python
 
-    from pyhealth.medcode import InnerMap
+    from pyhealth.medcode import CrossMap
 
-    icd9cm = InnerMap.load("ICD9CM")
-    icd9cm.lookup("428.0") # get detailed info
-    icd9cm.get_ancestors("428.0") # get parents
+    codemap = CrossMap.load("ICD9CM", "CCSCM")
+    codemap.map("428.0")
+    # ['108']
+
+    codemap = CrossMap.load("NDC", "RxNorm")
+    codemap.map("50580049698")
+    # ['209387']
+
+    codemap = CrossMap.load("NDC", "ATC")
+    codemap.map("50090539100")
+    # ['A10AC04', 'A10AD04', 'A10AB04']
 
-3.3 Medical Code Tokenizer
-^^^^^^^^^^^^^^^^^^^^^^^^^^
+5. Medical Code Tokenizer :speech_balloon:
+---------------------------------------------
 
-* **<pyhealth.tokenizer>** is used for transformations between string-based tokens and integer-based indices, based on the overall token space. We provide flexible functions to tokenize 1D, 2D and 3D lists. **This module can be independently applied to your research.**
+``pyhealth.tokenizer`` is used for transformations between string-based tokens and integer-based indices, based on the overall token space. We provide flexible functions to tokenize 1D, 2D and 3D lists. **This module can be used independently.**
 
 .. code-block:: python
 
     from pyhealth.tokenizer import Tokenizer
 
     # Example: we use a list of ATC3 code as the token
     token_space = ['A01A', 'A02A', 'A02B', 'A02X', 'A03A', 'A03B', 'A03C', 'A03D', \
             'A03F', 'A04A', 'A05A', 'A05B', 'A05C', 'A06A', 'A07A', 'A07B', 'A07C', \
             'A12B', 'A12C', 'A13A', 'A14A', 'A14B', 'A16A']
     tokenizer = Tokenizer(tokens=token_space, special_tokens=["<pad>", "<unk>"])
 
     # 2d encode 
     tokens = [['A03C', 'A03D', 'A03E', 'A03F'], ['A04A', 'B035', 'C129']]
-    indices = tokenizer.batch_encode_2d(tokens) # [[8, 9, 10, 11], [12, 1, 1, 0]]
+    indices = tokenizer.batch_encode_2d(tokens) 
+    # [[8, 9, 10, 11], [12, 1, 1, 0]]
 
     # 2d decode 
     indices = [[8, 9, 10, 11], [12, 1, 1, 0]]
-    tokens = tokenizer.batch_decode_2d(indices) # [['A03C', 'A03D', 'A03E', 'A03F'], ['A04A', '<unk>', '<unk>']]
+    tokens = tokenizer.batch_decode_2d(indices)
+    # [['A03C', 'A03D', 'A03E', 'A03F'], ['A04A', '<unk>', '<unk>']]
 
+    # 3d encode
+    tokens = [[['A03C', 'A03D', 'A03E', 'A03F'], ['A08A', 'A09A']], \
+        [['A04A', 'B035', 'C129']]]
+    indices = tokenizer.batch_encode_3d(tokens)
+    # [[[8, 9, 10, 11], [24, 25, 0, 0]], [[12, 1, 1, 0], [0, 0, 0, 0]]]
+
+    # 3d decode
+    indices = [[[8, 9, 10, 11], [24, 25, 0, 0]], \
+        [[12, 1, 1, 0], [0, 0, 0, 0]]]
+    tokens = tokenizer.batch_decode_3d(indices)
+    # [[['A03C', 'A03D', 'A03E', 'A03F'], ['A08A', 'A09A']], [['A04A', '<unk>', '<unk>']]]
 ..
 
-4. Tutorials
-------------
+6. Tutorials :teacher:
+----------------------------
 
- We provide the following tutorials to help users get started with our pyhealth.
+.. image:: https://colab.research.google.com/assets/colab-badge.svg
+    :target: https://pyhealth.readthedocs.io/en/latest/tutorials.html
 
+..
 
-`Tutorial 0: Introduction to pyhealth.data <https://colab.research.google.com/drive/1y9PawgSbyMbSSMw1dpfwtooH7qzOEYdN?usp=sharing>`_ 
+ We provide the following tutorials to help users get started with our pyhealth. 
 
-`Tutorial 1: Introduction to pyhealth.datasets <https://colab.research.google.com/drive/18kbzEQAj1FMs_J9rTGX8eCoxnWdx4Ltn?usp=sharing>`_ 
+`Tutorial 0: Introduction to pyhealth.data <https://colab.research.google.com/drive/1y9PawgSbyMbSSMw1dpfwtooH7qzOEYdN?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=Nk1itBoLOX8&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=2>`__  
 
-`Tutorial 2: Introduction to pyhealth.tasks <https://colab.research.google.com/drive/1r7MYQR_5yCJGpK_9I9-A10HmpupZuIN-?usp=sharing>`_ 
+`Tutorial 1: Introduction to pyhealth.datasets <https://colab.research.google.com/drive/18kbzEQAj1FMs_J9rTGX8eCoxnWdx4Ltn?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=c1InKqFJbsI&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=3>`__  
 
-`Tutorial 3: Introduction to pyhealth.models <https://colab.research.google.com/drive/1LcXZlu7ZUuqepf269X3FhXuhHeRvaJX5?usp=sharing>`_ 
+`Tutorial 2: Introduction to pyhealth.tasks <https://colab.research.google.com/drive/1r7MYQR_5yCJGpK_9I9-A10HmpupZuIN-?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=CxESe1gYWU4&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=4>`__  
 
-`Tutorial 4: Introduction to pyhealth.trainer <https://colab.research.google.com/drive/1L1Nz76cRNB7wTp5Pz_4Vp4N2eRZ9R6xl?usp=sharing>`_ 
+`Tutorial 3: Introduction to pyhealth.models <https://colab.research.google.com/drive/1LcXZlu7ZUuqepf269X3FhXuhHeRvaJX5?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=fRc0ncbTgZA&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=6>`__  
 
-`Tutorial 5: Introduction to pyhealth.metrics <https://colab.research.google.com/drive/1Mrs77EJ92HwMgDaElJ_CBXbi4iABZBeo?usp=sharing>`_ 
+`Tutorial 4: Introduction to pyhealth.trainer <https://colab.research.google.com/drive/1L1Nz76cRNB7wTp5Pz_4Vp4N2eRZ9R6xl?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=5Hyw3of5pO4&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=7>`__  
 
-`Tutorial 6: Introduction to pyhealth.tokenizer <https://colab.research.google.com/drive/1bDOb0A5g0umBjtz8NIp4wqye7taJ03D0?usp=sharing>`_
+`Tutorial 5: Introduction to pyhealth.metrics <https://colab.research.google.com/drive/1Mrs77EJ92HwMgDaElJ_CBXbi4iABZBeo?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=d-Kx_xCwre4&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=8>`__ 
 
-`Tutorial 7: Introduction to pyhealth.medcode <https://colab.research.google.com/drive/1xrp_ACM2_Hg5Wxzj0SKKKgZfMY0WwEj3?usp=sharing>`_
 
- The following tutorials will help users build their own task pipelines.
+`Tutorial 6: Introduction to pyhealth.tokenizer <https://colab.research.google.com/drive/1bDOb0A5g0umBjtz8NIp4wqye7taJ03D0?usp=sharing>`_ `[Video] <https://www.youtube.com/watch?v=CeXJtf0lfs0&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=10>`__ 
 
-`Pipeline 1: Drug Recommendation <https://colab.research.google.com/drive/10CSb4F4llYJvv42yTUiRmvSZdoEsbmFF?usp=sharing>`_ 
 
-`Pipeline 2: Length of Stay Prediction <https://colab.research.google.com/drive/1JoPpXqqB1_lGF1XscBOsDHMLtgvlOYI1?usp=sharing>`_ 
+`Tutorial 7: Introduction to pyhealth.medcode <https://colab.research.google.com/drive/1xrp_ACM2_Hg5Wxzj0SKKKgZfMY0WwEj3?usp=sharing>`_ `[Video] <https://www.youtube.com/watch?v=MmmfU6_xkYg&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=9>`__  
 
-`Pipeline 3: Readmission Prediction <https://colab.research.google.com/drive/1bhCwbXce1YFtVaQLsOt4FcyZJ1_my7Cs?usp=sharing>`_ 
 
-`Pipeline 4: Mortality Prediction <https://colab.research.google.com/drive/1Qblpcv4NWjrnADT66TjBcNwOe8x6wU4c?usp=sharing>`_ 
+ The following tutorials will help users build their own task pipelines.
 
- The following tutorials will help users to explore advanced features of pyhealth.
+`Pipeline 1: Drug Recommendation <https://colab.research.google.com/drive/10CSb4F4llYJvv42yTUiRmvSZdoEsbmFF?usp=sharing>`_ `[Video] <https://
+www.youtube.com/watch?v=GGP3Dhfyisc&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=12>`__  
 
-`Advanced Tutorial 1: Fit your dataset into our pipeline <https://colab.research.google.com/drive/1UurxwAAov1bL_5OO3gQJ4gAa_paeJwJp?usp=sharing>`_
+`Pipeline 2: Length of Stay Prediction <https://colab.research.google.com/drive/1JoPpXqqB1_lGF1XscBOsDHMLtgvlOYI1?usp=sharing>`_ `[Video] <https://
+www.youtube.com/watch?v=GGP3Dhfyisc&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=12>`__  
 
-`Advanced Tutorial 2: Define your own healthcare task <https://colab.research.google.com/drive/1gK6zPXvfFGBM1uNaLP32BOKrnnJdqRq2?usp=sharing>`_ 
+`Pipeline 3: Readmission Prediction <https://colab.research.google.com/drive/1bhCwbXce1YFtVaQLsOt4FcyZJ1_my7Cs?usp=sharing>`_ `[Video] <https://
+www.youtube.com/watch?v=GGP3Dhfyisc&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=12>`__  
 
-`Advanced Tutorial 3: Adopt customized model into pyhealth <https://colab.research.google.com/drive/1F_NJ90GC8_Eq-vKTf7Tyziew4gWjjKoH?usp=sharing>`_ 
+`Pipeline 4: Mortality Prediction <https://colab.research.google.com/drive/1Qblpcv4NWjrnADT66TjBcNwOe8x6wU4c?usp=sharing>`_ `[Video] <https://
+www.youtube.com/watch?v=GGP3Dhfyisc&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=12>`__ 
 
-`Advanced Tutorial 4: Load your own processed data into pyhealth and try out our ML models <https://colab.research.google.com/drive/1ZRnKch2EyJLrI3G5AvDXVpeE2wwgBWfw?usp=sharing>`_
+`Pipeline 5: Sleep Staging <https://colab.research.google.com/drive/1mpSeNCAthXG3cqROkdUcUdozIPIMTCuo?usp=sharing>`_ `[Video] <https://www.youtube.com/watch?v=ySAIU-rO6so&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=16>`__  
 
 
+ We provided the advanced tutorials for supporting various needs. 
 
-----
+`Advanced Tutorial 1: Fit your dataset into our pipeline <https://colab.research.google.com/drive/1UurxwAAov1bL_5OO3gQJ4gAa_paeJwJp?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=xw2hGLEQ4Y0&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=13>`__ 
 
+`Advanced Tutorial 2: Define your own healthcare task <https://colab.research.google.com/drive/1gK6zPXvfFGBM1uNaLP32BOKrnnJdqRq2?usp=sharing>`_ 
 
-5. Datasets
---------------------------
+`Advanced Tutorial 3: Adopt customized model into pyhealth <https://colab.research.google.com/drive/1F_NJ90GC8_Eq-vKTf7Tyziew4gWjjKoH?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=lADFlcmLtdE&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=14>`__ 
+
+`Advanced Tutorial 4: Load your own processed data into pyhealth and try out our ML models <https://colab.research.google.com/drive/1ZRnKch2EyJLrI3G5AvDXVpeE2wwgBWfw?usp=sharing>`_ `[Video] <https://www.youtube.com/watch?v=xw2hGLEQ4Y0&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=13>`__ 
+
+
+7. Datasets :mountain_snow:
+-----------------------------
 We provide the processing files for the following open EHR datasets:
 
 ===================  =======================================  ========================================  ======================================================================================================== 
 Dataset              Module                                   Year                                      Information                                                             
 ===================  =======================================  ========================================  ========================================================================================================
-MIMIC-III            ``pyhealth.datasets.MIMIC3BaseDataset``  2016                                      `MIMIC-III Clinical Database <https://physionet.org/content/mimiciii/1.4//>`_    
-MIMIC-IV             ``pyhealth.datasets.MIMIC4BaseDataset``  2020                                      `MIMIC-IV Clinical Database <https://physionet.org/content/mimiciv/0.4/>`_  
-eICU                 ``pyhealth.datasets.eICUBaseDataset``    2018                                      `eICU Collaborative Research Database <https://eicu-crd.mit.edu//>`_                 
-OMOP                 ``pyhealth.datasets.OMOPBaseDataset``                                              `OMOP-CDM schema based dataset <https://www.ohdsi.org/data-standardization/the-common-data-model/>`_                                    
+MIMIC-III            ``pyhealth.datasets.MIMIC3Dataset``      2016                                      `MIMIC-III Clinical Database <https://physionet.org/content/mimiciii/1.4//>`_    
+MIMIC-IV             ``pyhealth.datasets.MIMIC4Dataset``      2020                                      `MIMIC-IV Clinical Database <https://physionet.org/content/mimiciv/0.4/>`_  
+eICU                 ``pyhealth.datasets.eICUDataset``        2018                                      `eICU Collaborative Research Database <https://eicu-crd.mit.edu//>`_                 
+OMOP                 ``pyhealth.datasets.OMOPDataset``                                                  `OMOP-CDM schema based dataset <https://www.ohdsi.org/data-standardization/the-common-data-model/>`_    
+SleepEDF             ``pyhealth.datasets.SleepEDFDataset``    2018                                      `Sleep-EDF dataset <https://physionet.org/content/sleep-edfx/1.0.0/>`_
+SHHS                 ``pyhealth.datasets.SHHSDataset``        2016                                      `Sleep Heart Health Study dataset <https://sleepdata.org/datasets/shhs>`_   
+ISRUC                ``pyhealth.datasets.ISRUCDataset``       2016                                      `ISRUC-SLEEP dataset <https://sleeptight.isr.uc.pt/?page_id=48>`_                               
 ===================  =======================================  ========================================  ========================================================================================================
 
 
-6. Machine/Deep Learning Models and Benchmarks
-------------------------------------------------
+8. Machine/Deep Learning Models and Benchmarks :airplane:
+------------------------------------------------------------
 
-==================================    ================  =================================  ======  ===========================================================================================================================================
-Model Name                            Type              Module                             Year    Reference
-==================================    ================  =================================  ======  ===========================================================================================================================================
-Convolutional Neural Network (CNN)    deep learning     ``pyhealth.models.CNN``            1989    `Handwritten Digit Recognition with a Back-Propagation Network <https://proceedings.neurips.cc/paper/1989/file/53c3bce66e43be4f209556518c2fcb54-Paper.pdf>`_
-Recurrent Neural Nets (RNN)           deep Learning     ``pyhealth.models.RNN``            2011    `Recurrent neural network based language model <http://www.fit.vutbr.cz/research/groups/speech/servite/2010/rnnlm_mikolov.pdf>`_
-Transformer                           deep Learning     ``pyhealth.models.Transformer``    2017    `Atention is All you Need <https://arxiv.org/abs/1706.03762>`_
-RETAIN                                deep Learning     ``pyhealth.models.RETAIN``         2016    `RETAIN: An Interpretable Predictive Model for Healthcare using Reverse Time Attention Mechanism <https://arxiv.org/abs/1608.05745>`_
-GAMENet                               deep Learning     ``pyhealth.models.GAMENet``        2019    `GAMENet: Graph Attention Mechanism for Explainable Electronic Health Record Prediction <https://arxiv.org/abs/1809.01852>`_
-MICRON                                deep Learning     ``pyhealth.models.MICRON``         2021    `Change Matters: Medication Change Prediction with Recurrent Residual Networks <https://www.ijcai.org/proceedings/2021/0513>`_
-SafeDrug                              deep Learning     ``pyhealth.models.SafeDrug``       2021    `SafeDrug: Dual Molecular Graph Encoders for Recommending Effective and Safe Drug Combinations <https://arxiv.org/abs/2105.02711>`_
-==================================    ================  =================================  ======  ===========================================================================================================================================
+==================================    ================  =================================  ======  ============================================================================================================================================================================  =======================================================================================================================================================================================
+Model Name                            Type              Module                             Year    Summary                                                                                                                                                                       Reference
+==================================    ================  =================================  ======  ============================================================================================================================================================================  =======================================================================================================================================================================================
+Multi-layer Perceptron                deep learning     ``pyhealth.models.MLP``            1986    MLP treats each feature as static                                                                                                                                             `Backpropagation: theory, architectures, and applications <https://www.taylorfrancis.com/books/mono/10.4324/9780203763247/backpropagation-yves-chauvin-david-rumelhart>`_
+Convolutional Neural Network (CNN)    deep learning     ``pyhealth.models.CNN``            1989    CNN runs on the conceptual patient-by-visit grids                                                                                                                             `Handwritten Digit Recognition with a Back-Propagation Network <https://proceedings.neurips.cc/paper/1989/file/53c3bce66e43be4f209556518c2fcb54-Paper.pdf>`_
+Recurrent Neural Nets (RNN)           deep Learning     ``pyhealth.models.RNN``            2011    RNN (includes LSTM and GRU) can run on any sequential level (e.g., visit by visit sequences)                                                                                  `Recurrent neural network based language model <http://www.fit.vutbr.cz/research/groups/speech/servite/2010/rnnlm_mikolov.pdf>`_
+Transformer                           deep Learning     ``pyhealth.models.Transformer``    2017    Transformer can run on any sequential level (e.g., visit by visit sequences)                                                                                                  `Atention is All you Need <https://arxiv.org/abs/1706.03762>`_
+RETAIN                                deep Learning     ``pyhealth.models.RETAIN``         2016    RETAIN uses two RNN to learn patient embeddings while providing feature-level and visit-level importance.                                                                     `RETAIN: An Interpretable Predictive Model for Healthcare using Reverse Time Attention Mechanism <https://arxiv.org/abs/1608.05745>`_
+GAMENet                               deep Learning     ``pyhealth.models.GAMENet``        2019    GAMENet uses memory networks, used only for drug recommendation task                                                                                                          `GAMENet: Graph Attention Mechanism for Explainable Electronic Health Record Prediction <https://arxiv.org/abs/1809.01852>`_
+MICRON                                deep Learning     ``pyhealth.models.MICRON``         2021    MICRON predicts the future drug combination by instead predicting the changes w.r.t. the current combination, used only for drug recommendation task                          `Change Matters: Medication Change Prediction with Recurrent Residual Networks <https://www.ijcai.org/proceedings/2021/0513>`_
+SafeDrug                              deep Learning     ``pyhealth.models.SafeDrug``       2021    SafeDrug encodes drug molecule structures by graph neural networks, used only for drug recommendation task                                                                    `SafeDrug: Dual Molecular Graph Encoders for Recommending Effective and Safe Drug Combinations <https://arxiv.org/abs/2105.02711>`_
+MoleRec                               deep Learning     ``pyhealth.models.MoleRec``        2023    MoleRec encodes drug molecule in a substructure level as well as the patient's information into a drug combination representation, used only for drug recommendation task     `MoleRec: Combinatorial Drug Recommendation with Substructure-Aware Molecular Representation Learning <https://dl.acm.org/doi/10.1145/3543507.3583872>`_
+Deepr                                 deep Learning     ``pyhealth.models.Deepr``          2017    Deepr is based on 1D CNN. General purpose.                                                                                                                                    `Deepr : A Convolutional Net for Medical Records <https://arxiv.org/abs/1607.07519>`_
+ContraWR Encoder (STFT+CNN)           deep Learning     ``pyhealth.models.ContraWR``       2021    ContraWR encoder uses short time Fourier transform (STFT) + 2D CNN, used for biosignal learning                                                                               `Self-supervised EEG Representation Learning for Automatic Sleep Staging <https://arxiv.org/abs/2110.15278>`_
+SparcNet (1D CNN)                     deep Learning     ``pyhealth.models.SparcNet``       2023    SparcNet is based on 1D CNN, used for biosignal learning                                                                                                                      `Development of Expert-level Classification of Seizures and Rhythmic and Periodic Patterns During EEG Interpretation <#>`_
+TCN                                   deep learning     ``pyhealth.models.TCN``            2018    TCN is based on dilated 1D CNN. General purpose                                                                                                                               `Temporal Convolutional Networks <https://arxiv.org/abs/1803.01271>`_
+AdaCare                               deep learning     ``pyhealth.models.AdaCare``        2020    AdaCare uses CNNs with dilated filters to learn enriched patient embedding. It uses feature calibration module to provide the feature-level and visit-level interpretability  `AdaCare: Explainable Clinical Health Status Representation Learning via Scale-Adaptive Feature Extraction and Recalibration <https://arxiv.org/abs/1911.12205>`_
+ConCare                               deep learning     ``pyhealth.models.ConCare``        2020    ConCare uses transformers to learn patient embedding and calculate inter-feature correlations.                                                                                `ConCare: Personalized Clinical Feature Embedding via Capturing the Healthcare Context <https://arxiv.org/abs/1911.12216>`_
+StageNet                              deep learning     ``pyhealth.models.StageNet``       2020    StageNet uses stage-aware LSTM to conduct clinical predictive tasks while learning patient disease progression stage change unsupervisedly                                    `StageNet: Stage-Aware Neural Networks for Health Risk Prediction <https://arxiv.org/abs/2001.10054>`_
+Dr. Agent                             deep learning     ``pyhealth.models.Agent``          2020    Dr. Agent uses two reinforcement learning agents to learn patient embeddings by mimicking clinical second opinions                                                            `Dr. Agent: Clinical predictive model via mimicked second opinions <https://academic.oup.com/jamia/article/27/7/1084/5858308>`_
+GRASP                                 deep learning     ``pyhealth.models.GRASP``          2021    GRASP uses graph neural network to identify latent patient clusters and uses the clustering information to learn patient                                                      `GRASP: Generic Framework for Health Status Representation Learning Based on Incorporating Knowledge from Similar Patients <https://ojs.aaai.org/index.php/AAAI/article/view/16152>`_
+==================================    ================  =================================  ======  ============================================================================================================================================================================  =======================================================================================================================================================================================
 
 * Check the `interactive map on benchmark EHR predictive tasks <https://pyhealth.readthedocs.io/en/latest/index.html#benchmark-on-healthcare-tasks>`_.
 
-7. Citing PyHealth
+9. Citing PyHealth :handshake:
 ----------------------------------
 
 .. code-block:: bibtex
 
-    @software{pyhealth2022github,
-        author = {Chaoqi Yang and Zhenbang Wu and Patrick Jiang and Jimeng Sun},
+    @inproceedings{pyhealth2023yang,
+        author = {Yang, Chaoqi and Wu, Zhenbang and Jiang, Patrick and Lin, Zhen and Gao, Junyi and Danek, Benjamin and Sun, Jimeng},
         title = {{PyHealth}: A Deep Learning Toolkit for Healthcare Predictive Modeling},
         url = {https://github.com/sunlabuiuc/PyHealth},
-        year = {2022},
+        booktitle = {Proceedings of the 27th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD) 2023},
+        year = {2023}
     }
```

### Comparing `pyhealth-1.1.3/leaderboard/ext_plot.py` & `pyhealth-1.1.4/leaderboard/ext_plot.py`

 * *Files identical despite different names*

### Comparing `pyhealth-1.1.3/leaderboard/leaderboard_gen.py` & `pyhealth-1.1.4/leaderboard/leaderboard_gen.py`

 * *Files identical despite different names*

### Comparing `pyhealth-1.1.3/leaderboard/rtd_build_trigger.py` & `pyhealth-1.1.4/leaderboard/rtd_build_trigger.py`

 * *Files identical despite different names*

### Comparing `pyhealth-1.1.3/leaderboard/utils.py` & `pyhealth-1.1.4/leaderboard/utils.py`

 * *Files identical despite different names*

### Comparing `pyhealth-1.1.3/pyhealth/data/data.py` & `pyhealth-1.1.4/pyhealth/data/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,19 +37,19 @@
         Event with NDC code 00069153041 from table PRESCRIPTIONS
         >>> event.attr_dict
         {'dosage': '250mg'}
     """
 
     def __init__(
         self,
-        code: str,
-        table: str,
-        vocabulary: str,
-        visit_id: str,
-        patient_id: str,
+        code: str = None,
+        table: str = None,
+        vocabulary: str = None,
+        visit_id: str = None,
+        patient_id: str = None,
         timestamp: Optional[datetime] = None,
         **attr,
     ):
         assert timestamp is None or isinstance(
             timestamp, datetime
         ), "timestamp must be a datetime object"
         self.code = code
```

### Comparing `pyhealth-1.1.3/pyhealth/datasets/base_dataset.py` & `pyhealth-1.1.4/pyhealth/datasets/base_ehr_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import logging
+import time
 import os
 from abc import ABC
 from collections import Counter
 from copy import deepcopy
 from typing import Dict, Callable, Tuple, Union, List, Optional
 
+import pandas as pd
 from tqdm import tqdm
+from pandarallel import pandarallel
 
 from pyhealth.data import Patient, Event
-from pyhealth.datasets.sample_dataset import SampleDataset
-from pyhealth.datasets.utils import MODULE_CACHE_PATH
+from pyhealth.datasets.sample_dataset import SampleEHRDataset
+from pyhealth.datasets.utils import MODULE_CACHE_PATH, DATASET_BASIC_TABLES
 from pyhealth.datasets.utils import hash_str
 from pyhealth.medcode import CrossMap
 from pyhealth.utils import load_pickle, save_pickle
 
 logger = logging.getLogger(__name__)
 
 INFO_MSG = """
@@ -32,27 +35,27 @@
             - other event-level info
 """
 
 
 # TODO: parse_tables is too slow
 
 
-class BaseDataset(ABC):
+class BaseEHRDataset(ABC):
     """Abstract base dataset class.
 
-    This abstract class defines a uniform interface for all datasets
+    This abstract class defines a uniform interface for all EHR datasets
     (e.g., MIMIC-III, MIMIC-IV, eICU, OMOP).
 
     Each specific dataset will be a subclass of this abstract class, which can then
     be converted to samples dataset for different tasks by calling `self.set_task()`.
 
     Args:
         dataset_name: name of the dataset.
         root: root directory of the raw data (should contain many csv files).
-        tables: list of tables to be loaded (e.g., ["DIAGNOSES_ICD", "PROCEDURES_ICD"]).
+        tables: list of tables to be loaded (e.g., ["DIAGNOSES_ICD", "PROCEDURES_ICD"]). Basic tables will be loaded by default.
         code_mapping: a dictionary containing the code mapping information.
             The key is a str of the source code vocabulary and the value is of
             two formats:
                 - a str of the target code vocabulary. E.g., {"NDC", "ATC"}.
                 - a tuple with two elements. The first element is a str of the
                     target code vocabulary and the second element is a dict with
                     keys "source_kwargs" or "target_kwargs" and values of the
@@ -80,31 +83,43 @@
             code_mapping = {}
 
         # base attributes
         self.dataset_name = (
             self.__class__.__name__ if dataset_name is None else dataset_name
         )
         self.root = root
-        self.tables = tables
+
         self.code_mapping = code_mapping
         self.dev = dev
 
+        # if we are using a premade dataset, no basic tables need to be provided.
+        if self.dataset_name in DATASET_BASIC_TABLES and [
+            table
+            for table in tables
+            if table in DATASET_BASIC_TABLES[self.dataset_name]
+        ]:
+            raise AttributeError(
+                f"Basic tables are parsed by default and do not need to be explicitly selected. Basic tables for {self.dataset_name}: {DATASET_BASIC_TABLES[self.dataset_name]}"
+            )
+
+        self.tables = tables
+
         # load medcode for code mapping
         self.code_mapping_tools = self._load_code_mapping_tools()
 
         # hash filename for cache
         args_to_hash = (
             [self.dataset_name, root]
             + sorted(tables)
             + sorted(code_mapping.items())
             + ["dev" if dev else "prod"]
         )
         filename = hash_str("+".join([str(arg) for arg in args_to_hash])) + ".pkl"
         self.filepath = os.path.join(MODULE_CACHE_PATH, filename)
-
+        
         # check if cache exists or refresh_cache is True
         if os.path.exists(self.filepath) and (not refresh_cache):
             # load from cache
             logger.debug(
                 f"Loaded {self.dataset_name} base dataset from {self.filepath}"
             )
             self.patients = load_pickle(self.filepath)
@@ -153,37 +168,68 @@
         basic patient information, and then call `self.parse_[table_name]()` to
         parse the table with name `table_name`. Both `self.parse_basic_info()` and
         `self.parse_[table_name]()` should be implemented in the subclass.
 
         Returns:
            A dict mapping patient_id to `Patient` object.
         """
+        pandarallel.initialize(progress_bar=False)
+
         # patients is a dict of Patient objects indexed by patient_id
         patients: Dict[str, Patient] = dict()
         # process basic information (e.g., patients and visits)
+        tic = time.time()
         patients = self.parse_basic_info(patients)
+        print(
+            "finish basic patient information parsing : {}s".format(time.time() - tic)
+        )
         # process clinical tables
         for table in self.tables:
             try:
                 # use lower case for function name
+                tic = time.time()
                 patients = getattr(self, f"parse_{table.lower()}")(patients)
+                print(f"finish parsing {table} : {time.time() - tic}s")
             except AttributeError:
                 raise NotImplementedError(
                     f"Parser for table {table} is not implemented yet."
                 )
         return patients
 
+    def _add_events_to_patient_dict(
+        self,
+        patient_dict: Dict[str, Patient],
+        group_df: pd.DataFrame,
+    ) -> Dict[str, Patient]:
+        """Helper function which adds the events column of a df.groupby object to the patient dict.
+
+        Will be called at the end of each `self.parse_[table_name]()` function.
+
+        Args:
+            patient_dict: a dict mapping patient_id to `Patient` object.
+            group_df: a df.groupby object, having two columns: patient_id and events.
+                - the patient_id column is the index of the patient
+                - the events column is a list of <Event> objects
+
+        Returns:
+            The updated patient dict.
+        """
+        for _, events in group_df.items():
+            for event in events:
+                patient_dict = self._add_event_to_patient_dict(patient_dict, event)
+        return patient_dict
+
     @staticmethod
     def _add_event_to_patient_dict(
         patient_dict: Dict[str, Patient],
         event: Event,
     ) -> Dict[str, Patient]:
         """Helper function which adds an event to the patient dict.
 
-        Will be called in `self.parse_tables()`.
+        Will be called in `self._add_events_to_patient_dict`.
 
         Note that if the patient of the event is not in the patient dict, or the
         visit of the event is not in the patient, this function will do nothing.
 
         Args:
             patient_dict: a dict mapping patient_id to `Patient` object.
             event: an event to be added to the patient dict.
@@ -321,15 +367,15 @@
         """Prints the output format."""
         print(INFO_MSG)
 
     def set_task(
         self,
         task_fn: Callable,
         task_name: Optional[str] = None,
-    ) -> SampleDataset:
+    ) -> SampleEHRDataset:
         """Processes the base dataset to generate the task-specific sample dataset.
 
         This function should be called by the user after the base dataset is
         initialized. It will iterate through all patients in the base dataset
         and call `task_fn` which should be implemented by the specific task.
 
         Args:
@@ -353,13 +399,13 @@
         if task_name is None:
             task_name = task_fn.__name__
         samples = []
         for patient_id, patient in tqdm(
             self.patients.items(), desc=f"Generating samples for {task_name}"
         ):
             samples.extend(task_fn(patient))
-        sample_dataset = SampleDataset(
+        sample_dataset = SampleEHRDataset(
             samples,
             dataset_name=self.dataset_name,
             task_name=task_name,
         )
         return sample_dataset
```

### Comparing `pyhealth-1.1.3/pyhealth/datasets/mimic3.py` & `pyhealth-1.1.4/pyhealth/datasets/mimic3.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import os
 from typing import Optional, List, Dict, Tuple, Union
 
 import pandas as pd
-from tqdm import tqdm
 
 from pyhealth.data import Event, Visit, Patient
-from pyhealth.datasets import BaseDataset
+from pyhealth.datasets import BaseEHRDataset
 from pyhealth.datasets.utils import strptime
 
-
 # TODO: add other tables
 
 
-class MIMIC3Dataset(BaseDataset):
+class MIMIC3Dataset(BaseEHRDataset):
     """Base dataset for MIMIC-III dataset.
 
     The MIMIC-III dataset is a large dataset of de-identified health records of ICU
     patients. The dataset is available at https://mimic.physionet.org/.
 
     The basic information is stored in the following tables:
         - PATIENTS: defines a patient in the database, SUBJECT_ID.
@@ -76,15 +74,15 @@
         Will be called in `self.parse_tables()`
 
         Docs:
             - PATIENTS: https://mimic.mit.edu/docs/iii/tables/patients/
             - ADMISSIONS: https://mimic.mit.edu/docs/iii/tables/admissions/
 
         Args:
-            patients: a dict of `Patient` objects indexed by patient_id.
+            patients: a dict of `Patient` objects indexed by patient_id which is updated with the mimic-3 table result.
 
         Returns:
             The updated patients dict.
         """
         # read patients table
         patients_df = pd.read_csv(
             os.path.join(self.root, "PATIENTS.csv"),
@@ -98,16 +96,17 @@
         )
         # merge patient and admission tables
         df = pd.merge(patients_df, admissions_df, on="SUBJECT_ID", how="inner")
         # sort by admission and discharge time
         df = df.sort_values(["SUBJECT_ID", "ADMITTIME", "DISCHTIME"], ascending=True)
         # group by patient
         df_group = df.groupby("SUBJECT_ID")
-        # load patients
-        for p_id, p_info in tqdm(df_group, desc="Parsing PATIENTS and ADMISSIONS"):
+
+        # parallel unit of basic information (per patient)
+        def basic_unit(p_id, p_info):
             patient = Patient(
                 patient_id=p_id,
                 birth_datetime=strptime(p_info["DOB"].values[0]),
                 death_datetime=strptime(p_info["DOD_HOSP"].values[0]),
                 gender=p_info["GENDER"].values[0],
                 ethnicity=p_info["ETHNICITY"].values[0],
             )
@@ -118,16 +117,24 @@
                     patient_id=p_id,
                     encounter_time=strptime(v_info["ADMITTIME"].values[0]),
                     discharge_time=strptime(v_info["DISCHTIME"].values[0]),
                     discharge_status=v_info["HOSPITAL_EXPIRE_FLAG"].values[0],
                 )
                 # add visit
                 patient.add_visit(visit)
-            # add patient
-            patients[p_id] = patient
+            return patient
+
+        # parallel apply
+        df_group = df_group.parallel_apply(
+            lambda x: basic_unit(x.SUBJECT_ID.unique()[0], x)
+        )
+        # summarize the results
+        for pat_id, pat in df_group.items():
+            patients[pat_id] = pat
+
         return patients
 
     def parse_diagnoses_icd(self, patients: Dict[str, Patient]) -> Dict[str, Patient]:
         """Helper function which parses DIAGNOSES_ICD table.
 
         Will be called in `self.parse_tables()`
 
@@ -146,32 +153,45 @@
         """
         table = "DIAGNOSES_ICD"
         # read table
         df = pd.read_csv(
             os.path.join(self.root, f"{table}.csv"),
             dtype={"SUBJECT_ID": str, "HADM_ID": str, "ICD9_CODE": str},
         )
+        # drop records of the other patients
+        df = df[df["SUBJECT_ID"].isin(patients.keys())]
         # drop rows with missing values
         df = df.dropna(subset=["SUBJECT_ID", "HADM_ID", "ICD9_CODE"])
         # sort by sequence number (i.e., priority)
         df = df.sort_values(["SUBJECT_ID", "HADM_ID", "SEQ_NUM"], ascending=True)
         # group by patient and visit
-        group_df = df.groupby(["SUBJECT_ID", "HADM_ID"])
-        # iterate over each patient and visit
-        for (p_id, v_id), v_info in tqdm(group_df, desc=f"Parsing {table}"):
-            for code in v_info["ICD9_CODE"]:
-                event = Event(
-                    code=code,
-                    table=table,
-                    vocabulary="ICD9CM",
-                    visit_id=v_id,
-                    patient_id=p_id,
-                )
-                # update patients
-                patients = self._add_event_to_patient_dict(patients, event)
+        group_df = df.groupby("SUBJECT_ID")
+
+        # parallel unit of diagnosis (per patient)
+        def diagnosis_unit(p_id, p_info):
+            events = []
+            for v_id, v_info in p_info.groupby("HADM_ID"):
+                for code in v_info["ICD9_CODE"]:
+                    event = Event(
+                        code=code,
+                        table=table,
+                        vocabulary="ICD9CM",
+                        visit_id=v_id,
+                        patient_id=p_id,
+                    )
+                    events.append(event)
+            return events
+
+        # parallel apply
+        group_df = group_df.parallel_apply(
+            lambda x: diagnosis_unit(x.SUBJECT_ID.unique()[0], x)
+        )
+
+        # summarize the results
+        patients = self._add_events_to_patient_dict(patients, group_df)
         return patients
 
     def parse_procedures_icd(self, patients: Dict[str, Patient]) -> Dict[str, Patient]:
         """Helper function which parses PROCEDURES_ICD table.
 
         Will be called in `self.parse_tables()`
 
@@ -190,32 +210,45 @@
         """
         table = "PROCEDURES_ICD"
         # read table
         df = pd.read_csv(
             os.path.join(self.root, f"{table}.csv"),
             dtype={"SUBJECT_ID": str, "HADM_ID": str, "ICD9_CODE": str},
         )
+        # drop records of the other patients
+        df = df[df["SUBJECT_ID"].isin(patients.keys())]
         # drop rows with missing values
         df = df.dropna(subset=["SUBJECT_ID", "HADM_ID", "SEQ_NUM", "ICD9_CODE"])
         # sort by sequence number (i.e., priority)
         df = df.sort_values(["SUBJECT_ID", "HADM_ID", "SEQ_NUM"], ascending=True)
         # group by patient and visit
-        group_df = df.groupby(["SUBJECT_ID", "HADM_ID"])
-        # iterate over each patient and visit
-        for (p_id, v_id), v_info in tqdm(group_df, desc=f"Parsing {table}"):
-            for code in v_info["ICD9_CODE"]:
-                event = Event(
-                    code=code,
-                    table=table,
-                    vocabulary="ICD9PROC",
-                    visit_id=v_id,
-                    patient_id=p_id,
-                )
-                # update patients
-                patients = self._add_event_to_patient_dict(patients, event)
+        group_df = df.groupby("SUBJECT_ID")
+
+        # parallel unit of procedure (per patient)
+        def procedure_unit(p_id, p_info):
+            events = []
+            for v_id, v_info in p_info.groupby("HADM_ID"):
+                for code in v_info["ICD9_CODE"]:
+                    event = Event(
+                        code=code,
+                        table=table,
+                        vocabulary="ICD9PROC",
+                        visit_id=v_id,
+                        patient_id=p_id,
+                    )
+                    events.append(event)
+            return events
+
+        # parallel apply
+        group_df = group_df.parallel_apply(
+            lambda x: procedure_unit(x.SUBJECT_ID.unique()[0], x)
+        )
+
+        # summarize the results
+        patients = self._add_events_to_patient_dict(patients, group_df)
         return patients
 
     def parse_prescriptions(self, patients: Dict[str, Patient]) -> Dict[str, Patient]:
         """Helper function which parses PRESCRIPTIONS table.
 
         Will be called in `self.parse_tables()`
 
@@ -231,35 +264,48 @@
         table = "PRESCRIPTIONS"
         # read table
         df = pd.read_csv(
             os.path.join(self.root, f"{table}.csv"),
             low_memory=False,
             dtype={"SUBJECT_ID": str, "HADM_ID": str, "NDC": str},
         )
+        # drop records of the other patients
+        df = df[df["SUBJECT_ID"].isin(patients.keys())]
         # drop rows with missing values
         df = df.dropna(subset=["SUBJECT_ID", "HADM_ID", "NDC"])
         # sort by start date and end date
         df = df.sort_values(
             ["SUBJECT_ID", "HADM_ID", "STARTDATE", "ENDDATE"], ascending=True
         )
         # group by patient and visit
-        group_df = df.groupby(["SUBJECT_ID", "HADM_ID"])
-        # iterate over each patient and visit
-        for (p_id, v_id), v_info in tqdm(group_df, desc=f"Parsing {table}"):
-            for timestamp, code in zip(v_info["STARTDATE"], v_info["NDC"]):
-                event = Event(
-                    code=code,
-                    table=table,
-                    vocabulary="NDC",
-                    visit_id=v_id,
-                    patient_id=p_id,
-                    timestamp=strptime(timestamp),
-                )
-                # update patients
-                patients = self._add_event_to_patient_dict(patients, event)
+        group_df = df.groupby("SUBJECT_ID")
+
+        # parallel unit for prescription (per patient)
+        def prescription_unit(p_id, p_info):
+            events = []
+            for v_id, v_info in p_info.groupby("HADM_ID"):
+                for timestamp, code in zip(v_info["STARTDATE"], v_info["NDC"]):
+                    event = Event(
+                        code=code,
+                        table=table,
+                        vocabulary="NDC",
+                        visit_id=v_id,
+                        patient_id=p_id,
+                        timestamp=strptime(timestamp),
+                    )
+                    events.append(event)
+            return events
+
+        # parallel apply
+        group_df = group_df.parallel_apply(
+            lambda x: prescription_unit(x.SUBJECT_ID.unique()[0], x)
+        )
+
+        # summarize the results
+        patients = self._add_events_to_patient_dict(patients, group_df)
         return patients
 
     def parse_labevents(self, patients: Dict[str, Patient]) -> Dict[str, Patient]:
         """Helper function which parses LABEVENTS table.
 
         Will be called in `self.parse_tables()`
 
@@ -274,41 +320,60 @@
         """
         table = "LABEVENTS"
         # read table
         df = pd.read_csv(
             os.path.join(self.root, f"{table}.csv"),
             dtype={"SUBJECT_ID": str, "HADM_ID": str, "ITEMID": str},
         )
+        # drop records of the other patients
+        df = df[df["SUBJECT_ID"].isin(patients.keys())]
         # drop rows with missing values
         df = df.dropna(subset=["SUBJECT_ID", "HADM_ID", "ITEMID"])
         # sort by charttime
         df = df.sort_values(["SUBJECT_ID", "HADM_ID", "CHARTTIME"], ascending=True)
         # group by patient and visit
-        group_df = df.groupby(["SUBJECT_ID", "HADM_ID"])
-        # iterate over each patient and visit
-        for (p_id, v_id), v_info in tqdm(group_df, desc=f"Parsing {table}"):
-            for timestamp, code in zip(v_info["CHARTTIME"], v_info["ITEMID"]):
-                event = Event(
-                    code=code,
-                    table=table,
-                    vocabulary="MIMIC3_ITEMID",
-                    visit_id=v_id,
-                    patient_id=p_id,
-                    timestamp=strptime(timestamp),
-                )
-                # update patients
-                patients = self._add_event_to_patient_dict(patients, event)
+        group_df = df.groupby("SUBJECT_ID")
+
+        # parallel unit for lab (per patient)
+        def lab_unit(p_id, p_info):
+            events = []
+            for v_id, v_info in p_info.groupby("HADM_ID"):
+                for timestamp, code in zip(v_info["CHARTTIME"], v_info["ITEMID"]):
+                    event = Event(
+                        code=code,
+                        table=table,
+                        vocabulary="MIMIC3_ITEMID",
+                        visit_id=v_id,
+                        patient_id=p_id,
+                        timestamp=strptime(timestamp),
+                    )
+                    events.append(event)
+            return events
+
+        # parallel apply
+        group_df = group_df.parallel_apply(
+            lambda x: lab_unit(x.SUBJECT_ID.unique()[0], x)
+        )
+
+        # summarize the results
+        patients = self._add_events_to_patient_dict(patients, group_df)
         return patients
 
 
 if __name__ == "__main__":
     dataset = MIMIC3Dataset(
-        root="/srv/local/data/physionet.org/files/mimiciii/1.4",
-        tables=["DIAGNOSES_ICD", "PROCEDURES_ICD", "PRESCRIPTIONS", "LABEVENTS"],
+        root="https://storage.googleapis.com/pyhealth/mimiciii-demo/1.4/",
+        tables=[
+            "DIAGNOSES_ICD",
+            "PROCEDURES_ICD",
+            "PRESCRIPTIONS",
+            "LABEVENTS",
+        ],
         code_mapping={"NDC": "ATC"},
+        dev=True,
         refresh_cache=True,
     )
     dataset.stat()
     dataset.info()
 
     # dataset = MIMIC3Dataset(
     #     root="/srv/local/data/physionet.org/files/mimiciii/1.4",
```

### Comparing `pyhealth-1.1.3/pyhealth/datasets/mimic4.py` & `pyhealth-1.1.4/pyhealth/datasets/mimic4.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import os
 from typing import Optional, List, Dict, Union, Tuple
 
 import pandas as pd
-from tqdm import tqdm
 
 from pyhealth.data import Event, Visit, Patient
-from pyhealth.datasets import BaseDataset
+from pyhealth.datasets import BaseEHRDataset
 from pyhealth.datasets.utils import strptime
 
-
 # TODO: add other tables
 
 
-class MIMIC4Dataset(BaseDataset):
+class MIMIC4Dataset(BaseEHRDataset):
     """Base dataset for MIMIC-IV dataset.
 
     The MIMIC-IV dataset is a large dataset of de-identified health records of ICU
     patients. The dataset is available at https://mimic.physionet.org/.
 
     The basic information is stored in the following tables:
         - patients: defines a patient in the database, subject_id.
@@ -100,16 +98,17 @@
         )
         # merge patients and admissions tables
         df = pd.merge(patients_df, admissions_df, on="subject_id", how="inner")
         # sort by admission and discharge time
         df = df.sort_values(["subject_id", "admittime", "dischtime"], ascending=True)
         # group by patient
         df_group = df.groupby("subject_id")
-        # load patients
-        for p_id, p_info in tqdm(df_group, desc="Parsing patients and admissions"):
+
+        # parallel unit of basic information (per patient)
+        def basic_unit(p_id, p_info):
             # no exact birth datetime in MIMIC-IV
             # use anchor_year and anchor_age to approximate birth datetime
             anchor_year = int(p_info["anchor_year"].values[0])
             anchor_age = int(p_info["anchor_age"].values[0])
             birth_year = anchor_year - anchor_age
             patient = Patient(
                 patient_id=p_id,
@@ -128,16 +127,24 @@
                     patient_id=p_id,
                     encounter_time=strptime(v_info["admittime"].values[0]),
                     discharge_time=strptime(v_info["dischtime"].values[0]),
                     discharge_status=v_info["hospital_expire_flag"].values[0],
                 )
                 # add visit
                 patient.add_visit(visit)
-            # add patient
-            patients[p_id] = patient
+            return patient
+
+        # parallel apply
+        df_group = df_group.parallel_apply(
+            lambda x: basic_unit(x.subject_id.unique()[0], x)
+        )
+        # summarize the results
+        for pat_id, pat in df_group.items():
+            patients[pat_id] = pat
+
         return patients
 
     def parse_diagnoses_icd(self, patients: Dict[str, Patient]) -> Dict[str, Patient]:
         """Helper function which parses diagnosis_icd table.
 
         Will be called in `self.parse_tables()`
 
@@ -161,27 +168,39 @@
             dtype={"subject_id": str, "hadm_id": str, "icd_code": str},
         )
         # drop rows with missing values
         df = df.dropna(subset=["subject_id", "hadm_id", "icd_code", "icd_version"])
         # sort by sequence number (i.e., priority)
         df = df.sort_values(["subject_id", "hadm_id", "seq_num"], ascending=True)
         # group by patient and visit
-        group_df = df.groupby(["subject_id", "hadm_id"])
-        # iterate over each patient and visit
-        for (p_id, v_id), v_info in tqdm(group_df, desc=f"Parsing {table}"):
-            for code, version in zip(v_info["icd_code"], v_info["icd_version"]):
-                event = Event(
-                    code=code,
-                    table=table,
-                    vocabulary=f"ICD{version}CM",
-                    visit_id=v_id,
-                    patient_id=p_id,
-                )
-                # update patients
-                patients = self._add_event_to_patient_dict(patients, event)
+        group_df = df.groupby("subject_id")
+
+        # parallel unit of diagnosis (per patient)
+        def diagnosis_unit(p_id, p_info):
+            events = []
+            # iterate over each patient and visit
+            for v_id, v_info in p_info.groupby("hadm_id"):
+                for code, version in zip(v_info["icd_code"], v_info["icd_version"]):
+                    event = Event(
+                        code=code,
+                        table=table,
+                        vocabulary=f"ICD{version}CM",
+                        visit_id=v_id,
+                        patient_id=p_id,
+                    )
+                    events.append(event)
+            return events
+
+        # parallel apply
+        group_df = group_df.parallel_apply(
+            lambda x: diagnosis_unit(x.subject_id.unique()[0], x)
+        )
+
+        # summarize the results
+        patients = self._add_events_to_patient_dict(patients, group_df)
         return patients
 
     def parse_procedures_icd(self, patients: Dict[str, Patient]) -> Dict[str, Patient]:
         """Helper function which parses procedures_icd table.
 
         Will be called in `self.parse_tables()`
 
@@ -205,27 +224,40 @@
             dtype={"subject_id": str, "hadm_id": str, "icd_code": str},
         )
         # drop rows with missing values
         df = df.dropna(subset=["subject_id", "hadm_id", "icd_code", "icd_version"])
         # sort by sequence number (i.e., priority)
         df = df.sort_values(["subject_id", "hadm_id", "seq_num"], ascending=True)
         # group by patient and visit
-        group_df = df.groupby(["subject_id", "hadm_id"])
-        # iterate over each patient and visit
-        for (p_id, v_id), v_info in tqdm(group_df, desc=f"Parsing {table}"):
-            for code, version in zip(v_info["icd_code"], v_info["icd_version"]):
-                event = Event(
-                    code=code,
-                    table=table,
-                    vocabulary=f"ICD{version}PROC",
-                    visit_id=v_id,
-                    patient_id=p_id,
-                )
-                # update patients
-                patients = self._add_event_to_patient_dict(patients, event)
+        group_df = df.groupby("subject_id")
+
+        # parallel unit of procedure (per patient)
+        def procedure_unit(p_id, p_info):
+            events = []
+            for v_id, v_info in p_info.groupby("hadm_id"):
+                for code, version in zip(v_info["icd_code"], v_info["icd_version"]):
+                    event = Event(
+                        code=code,
+                        table=table,
+                        vocabulary=f"ICD{version}PROC",
+                        visit_id=v_id,
+                        patient_id=p_id,
+                    )
+                    # update patients
+                    events.append(event)
+            return events
+
+        # parallel apply
+        group_df = group_df.parallel_apply(
+            lambda x: procedure_unit(x.subject_id.unique()[0], x)
+        )
+
+        # summarize the results
+        patients = self._add_events_to_patient_dict(patients, group_df)
+
         return patients
 
     def parse_prescriptions(self, patients: Dict[str, Patient]) -> Dict[str, Patient]:
         """Helper function which parses prescriptions table.
 
         Will be called in `self.parse_tables()`
 
@@ -248,28 +280,41 @@
         # drop rows with missing values
         df = df.dropna(subset=["subject_id", "hadm_id", "ndc"])
         # sort by start date and end date
         df = df.sort_values(
             ["subject_id", "hadm_id", "starttime", "stoptime"], ascending=True
         )
         # group by patient and visit
-        group_df = df.groupby(["subject_id", "hadm_id"])
-        # iterate over each patient and visit
-        for (p_id, v_id), v_info in tqdm(group_df, desc=f"Parsing {table}"):
-            for timestamp, code in zip(v_info["starttime"], v_info["ndc"]):
-                event = Event(
-                    code=code,
-                    table=table,
-                    vocabulary="NDC",
-                    visit_id=v_id,
-                    patient_id=p_id,
-                    timestamp=strptime(timestamp),
-                )
-                # update patients
-                patients = self._add_event_to_patient_dict(patients, event)
+        group_df = df.groupby("subject_id")
+
+        # parallel unit of prescription (per patient)
+        def prescription_unit(p_id, p_info):
+            events = []
+            for v_id, v_info in p_info.groupby("hadm_id"):
+                for timestamp, code in zip(v_info["starttime"], v_info["ndc"]):
+                    event = Event(
+                        code=code,
+                        table=table,
+                        vocabulary="NDC",
+                        visit_id=v_id,
+                        patient_id=p_id,
+                        timestamp=strptime(timestamp),
+                    )
+                    # update patients
+                    events.append(event)
+            return events
+
+        # parallel apply
+        group_df = group_df.parallel_apply(
+            lambda x: prescription_unit(x.subject_id.unique()[0], x)
+        )
+
+        # summarize the results
+        patients = self._add_events_to_patient_dict(patients, group_df)
+
         return patients
 
     def parse_labevents(self, patients: Dict[str, Patient]) -> Dict[str, Patient]:
         """Helper function which parses labevents table.
 
         Will be called in `self.parse_tables()`
 
@@ -289,34 +334,100 @@
             dtype={"subject_id": str, "hadm_id": str, "itemid": str},
         )
         # drop rows with missing values
         df = df.dropna(subset=["subject_id", "hadm_id", "itemid"])
         # sort by charttime
         df = df.sort_values(["subject_id", "hadm_id", "charttime"], ascending=True)
         # group by patient and visit
-        group_df = df.groupby(["subject_id", "hadm_id"])
-        # iterate over each patient and visit
-        for (p_id, v_id), v_info in tqdm(group_df, desc=f"Parsing {table}"):
-            for timestamp, code in zip(v_info["charttime"], v_info["itemid"]):
-                event = Event(
-                    code=code,
-                    table=table,
-                    vocabulary="MIMIC4_ITEMID",
-                    visit_id=v_id,
-                    patient_id=p_id,
-                    timestamp=strptime(timestamp),
-                )
-                # update patients
-                patients = self._add_event_to_patient_dict(patients, event)
+        group_df = df.groupby("subject_id")
+
+        # parallel unit of labevent (per patient)
+        def lab_unit(p_id, p_info):
+            events = []
+            for v_id, v_info in p_info.groupby("hadm_id"):
+                for timestamp, code in zip(v_info["charttime"], v_info["itemid"]):
+                    event = Event(
+                        code=code,
+                        table=table,
+                        vocabulary="MIMIC4_ITEMID",
+                        visit_id=v_id,
+                        patient_id=p_id,
+                        timestamp=strptime(timestamp),
+                    )
+                    events.append(event)
+            return events
+
+        # parallel apply
+        group_df = group_df.parallel_apply(
+            lambda x: lab_unit(x.subject_id.unique()[0], x)
+        )
+
+        # summarize the results
+        patients = self._add_events_to_patient_dict(patients, group_df)
         return patients
 
+    def parse_hcpcsevents(self, patients: Dict[str, Patient]) -> Dict[str, Patient]:
+        """Helper function which parses hcpcsevents table.
+
+        Will be called in `self.parse_tables()`
+
+        Docs:
+            - hcpcsevents: https://mimic.mit.edu/docs/iv/modules/hosp/hcpcsevents/
+
+        Args:
+            patients: a dict of `Patient` objects indexed by patient_id.
+
+        Returns:
+            The updated patients dict.
+
+        Note:
+            MIMIC-IV does not provide specific timestamps in hcpcsevents
+                table, so we set it to None.
+        """
+        table = "hcpcsevents"
+        # read table
+        df = pd.read_csv(
+            os.path.join(self.root, f"{table}.csv"),
+            dtype={"subject_id": str, "hadm_id": str, "hcpcs_cd": str},
+        )
+        # drop rows with missing values
+        df = df.dropna(subset=["subject_id", "hadm_id", "hcpcs_cd"])
+        # sort by sequence number (i.e., priority)
+        df = df.sort_values(["subject_id", "hadm_id", "seq_num"], ascending=True)
+        # group by patient and visit
+        group_df = df.groupby("subject_id")
 
+        # parallel unit of hcpcsevents (per patient)
+        def hcpcsevents_unit(p_id, p_info):
+            events = []
+            for v_id, v_info in p_info.groupby("hadm_id"):
+                for code in v_info["hcpcs_cd"]:
+                    event = Event(
+                        code=code,
+                        table=table,
+                        vocabulary="MIMIC4_HCPCS_CD",
+                        visit_id=v_id,
+                        patient_id=p_id,
+                    )
+                    # update patients
+                    events.append(event)
+            return events
+            
+        # parallel apply
+        group_df = group_df.parallel_apply(
+            lambda x: hcpcsevents_unit(x.subject_id.unique()[0], x)
+        )
+
+        # summarize the results
+        patients = self._add_events_to_patient_dict(patients, group_df)
+        
+        return patients
+        
 if __name__ == "__main__":
     dataset = MIMIC4Dataset(
         root="/srv/local/data/physionet.org/files/mimiciv/2.0/hosp",
-        tables=["diagnoses_icd", "procedures_icd", "prescriptions", "labevents"],
-        dev=True,
+        tables=["diagnoses_icd", "procedures_icd", "prescriptions", "labevents", "hcpcsevents"],
         code_mapping={"NDC": "ATC"},
         refresh_cache=False,
     )
     dataset.stat()
     dataset.info()
```

### Comparing `pyhealth-1.1.3/pyhealth/datasets/omop.py` & `pyhealth-1.1.4/pyhealth/datasets/omop.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
 from typing import Optional, List, Dict, Tuple, Union
 
 import pandas as pd
-from tqdm import tqdm
 
 from pyhealth.data import Event, Visit, Patient
-from pyhealth.datasets import BaseDataset
+from pyhealth.datasets import BaseEHRDataset
 from pyhealth.datasets.utils import strptime
 
 
 # TODO: add other tables
 
 
-class OMOPDataset(BaseDataset):
+class OMOPDataset(BaseEHRDataset):
     """Base dataset for OMOP dataset.
 
     The Observational Medical Outcomes Partnership (OMOP) Common Data Model (CDM)
     is an open community data standard, designed to standardize the structure
     and content of observational data and to enable efficient analyses that
     can produce reliable evidence.
 
@@ -119,18 +118,18 @@
         df = pd.merge(df, death_df, on="person_id", how="left")
         # sort by admission time
         df = df.sort_values(
             ["person_id", "visit_occurrence_id", "visit_start_datetime"], ascending=True
         )
         # group by patient
         df_group = df.groupby("person_id")
-        # load patients
-        for p_id, p_info in tqdm(
-            df_group, desc="Parsing person, visit_occurrence and death"
-        ):
+
+        # parallel unit of basic informatin (per patient)
+        def basic_unit(p_info):
+            p_id = p_info["person_id"].values[0]
             birth_y = p_info["year_of_birth"].values[0]
             birth_m = p_info["month_of_birth"].values[0]
             birth_d = p_info["day_of_birth"].values[0]
             birth_date = f"{birth_y}-{birth_m}-{birth_d}"
             patient = Patient(
                 patient_id=p_id,
                 # no exact time, use 00:00:00
@@ -155,16 +154,22 @@
                     patient_id=p_id,
                     encounter_time=strptime(visit_start_date),
                     discharge_time=strptime(visit_end_date),
                     discharge_status=discharge_status,
                 )
                 # add visit
                 patient.add_visit(visit)
-            # add patient
-            patients[p_id] = patient
+            return patient
+
+        # parallel apply
+        df_group = df_group.parallel_apply(lambda x: basic_unit(x))
+        # summarize the results
+        for pat_id, pat in df_group.items():
+            patients[pat_id] = pat
+
         return patients
 
     def parse_condition_occurrence(
         self, patients: Dict[str, Patient]
     ) -> Dict[str, Patient]:
         """Helper function which parses condition_occurrence table.
 
@@ -196,30 +201,42 @@
         )
         # sort by condition_start_datetime
         df = df.sort_values(
             ["person_id", "visit_occurrence_id", "condition_start_datetime"],
             ascending=True,
         )
         # group by patient and visit
-        group_df = df.groupby(["person_id", "visit_occurrence_id"])
-        # iterate over each patient and visit
-        for (p_id, v_id), v_info in tqdm(group_df, desc=f"Parsing {table}"):
-            for timestamp, code in zip(
-                v_info["condition_start_datetime"], v_info["condition_concept_id"]
-            ):
-                event = Event(
-                    code=code,
-                    table=table,
-                    vocabulary="CONDITION_CONCEPT_ID",
-                    visit_id=v_id,
-                    patient_id=p_id,
-                    timestamp=strptime(timestamp),
-                )
-                # update patients
-                patients = self._add_event_to_patient_dict(patients, event)
+        group_df = df.groupby("person_id")
+
+        # parallel unit of condition occurrence (per patient)
+        def condition_unit(p_info):
+            p_id = p_info["person_id"].values[0]
+
+            events = []
+            for v_id, v_info in p_info.groupby("visit_occurrence_id"):
+                for timestamp, code in zip(
+                    v_info["condition_start_datetime"], v_info["condition_concept_id"]
+                ):
+                    event = Event(
+                        code=code,
+                        table=table,
+                        vocabulary="CONDITION_CONCEPT_ID",
+                        visit_id=v_id,
+                        patient_id=p_id,
+                        timestamp=strptime(timestamp),
+                    )
+                    # update patients
+                    events.append(event)
+
+        # parallel apply
+        group_df = group_df.parallel_apply(lambda x: condition_unit(x))
+
+        # summarize the results
+        patients = self._add_events_to_patient_dict(patients, group_df)
+
         return patients
 
     def parse_procedure_occurrence(
         self, patients: Dict[str, Patient]
     ) -> Dict[str, Patient]:
         """Helper function which parses procedure_occurrence table.
 
@@ -250,30 +267,41 @@
             subset=["person_id", "visit_occurrence_id", "procedure_concept_id"]
         )
         # sort by procedure_datetime
         df = df.sort_values(
             ["person_id", "visit_occurrence_id", "procedure_datetime"], ascending=True
         )
         # group by patient and visit
-        group_df = df.groupby(["person_id", "visit_occurrence_id"])
-        # iterate over each patient and visit
-        for (p_id, v_id), v_info in tqdm(group_df, desc=f"Parsing {table}"):
-            for timestamp, code in zip(
-                v_info["procedure_datetime"], v_info["procedure_concept_id"]
-            ):
-                event = Event(
-                    code=code,
-                    table=table,
-                    vocabulary="PROCEDURE_CONCEPT_ID",
-                    visit_id=v_id,
-                    patient_id=p_id,
-                    timestamp=strptime(timestamp),
-                )
-                # update patients
-                patients = self._add_event_to_patient_dict(patients, event)
+        group_df = df.groupby("person_id")
+
+        # parallel unit of procedure occurrence (per patient)
+        def procedure_unit(p_info):
+            p_id = p_info["person_id"].values[0]
+
+            events = []
+            for v_id, v_info in p_info.groupby("visit_occurrence_id"):
+                for timestamp, code in zip(
+                    v_info["procedure_datetime"], v_info["procedure_concept_id"]
+                ):
+                    event = Event(
+                        code=code,
+                        table=table,
+                        vocabulary="PROCEDURE_CONCEPT_ID",
+                        visit_id=v_id,
+                        patient_id=p_id,
+                        timestamp=strptime(timestamp),
+                    )
+                    events.append(event)
+            return events
+
+        # parallel apply
+        group_df = group_df.parallel_apply(lambda x: procedure_unit(x))
+
+        # summarize the results
+        patients = self._add_events_to_patient_dict(patients, group_df)
         return patients
 
     def parse_drug_exposure(self, patients: Dict[str, Patient]) -> Dict[str, Patient]:
         """Helper function which parses drug_exposure table.
 
         Will be called in `self.parse_tables()`
 
@@ -301,30 +329,42 @@
         df = df.dropna(subset=["person_id", "visit_occurrence_id", "drug_concept_id"])
         # sort by drug_exposure_start_datetime
         df = df.sort_values(
             ["person_id", "visit_occurrence_id", "drug_exposure_start_datetime"],
             ascending=True,
         )
         # group by patient and visit
-        group_df = df.groupby(["person_id", "visit_occurrence_id"])
-        # iterate over each patient and visit
-        for (p_id, v_id), v_info in tqdm(group_df, desc=f"Parsing {table}"):
-            for timestamp, code in zip(
-                v_info["drug_exposure_start_datetime"], v_info["drug_concept_id"]
-            ):
-                event = Event(
-                    code=code,
-                    table=table,
-                    vocabulary="DRUG_CONCEPT_ID",
-                    visit_id=v_id,
-                    patient_id=p_id,
-                    timestamp=strptime(timestamp),
-                )
-                # update patients
-                patients = self._add_event_to_patient_dict(patients, event)
+        group_df = df.groupby("person_id")
+
+        # parallel unit of drug exposure (per patient)
+        def drug_unit(p_info):
+            p_id = p_info["person_id"].values[0]
+
+            events = []
+            for v_id, v_info in p_info.groupby("visit_occurrence_id"):
+                for timestamp, code in zip(
+                    v_info["drug_exposure_start_datetime"], v_info["drug_concept_id"]
+                ):
+                    event = Event(
+                        code=code,
+                        table=table,
+                        vocabulary="DRUG_CONCEPT_ID",
+                        visit_id=v_id,
+                        patient_id=p_id,
+                        timestamp=strptime(timestamp),
+                    )
+                    events.append(event)
+            return events
+
+        # parallel apply
+        group_df = group_df.parallel_apply(lambda x: drug_unit(x))
+
+        # summarize the results
+        patients = self._add_events_to_patient_dict(patients, group_df)
+
         return patients
 
     def parse_measurement(self, patients: Dict[str, Patient]) -> Dict[str, Patient]:
         """Helper function which parses measurement table.
 
         Will be called in `self.parse_tables()`
 
@@ -353,40 +393,52 @@
             subset=["person_id", "visit_occurrence_id", "measurement_concept_id"]
         )
         # sort by measurement_datetime
         df = df.sort_values(
             ["person_id", "visit_occurrence_id", "measurement_datetime"], ascending=True
         )
         # group by patient and visit
-        group_df = df.groupby(["person_id", "visit_occurrence_id"])
-        # iterate over each patient and visit
-        for (p_id, v_id), v_info in tqdm(group_df, desc=f"Parsing {table}"):
-            for timestamp, code in zip(
-                v_info["measurement_datetime"], v_info["measurement_concept_id"]
-            ):
-                event = Event(
-                    code=code,
-                    table=table,
-                    vocabulary="MEASUREMENT_CONCEPT_ID",
-                    visit_id=v_id,
-                    patient_id=p_id,
-                    timestamp=strptime(timestamp),
-                )
-                # update patients
-                patients = self._add_event_to_patient_dict(patients, event)
+        group_df = df.groupby("person_id")
+
+        # parallel unit of measurement (per patient)
+        def measurement_unit(p_info):
+            p_id = p_info["person_id"].values[0]
+
+            events = []
+            for v_id, v_info in p_info.groupby("visit_occurrence_id"):
+                for timestamp, code in zip(
+                    v_info["measurement_datetime"], v_info["measurement_concept_id"]
+                ):
+                    event = Event(
+                        code=code,
+                        table=table,
+                        vocabulary="MEASUREMENT_CONCEPT_ID",
+                        visit_id=v_id,
+                        patient_id=p_id,
+                        timestamp=strptime(timestamp),
+                    )
+                    events.append(event)
+            return events
+
+        # parallel apply
+        group_df = group_df.parallel_apply(lambda x: measurement_unit(x))
+
+        # summarize the results
+        patients = self._add_events_to_patient_dict(patients, group_df)
+
         return patients
 
 
 if __name__ == "__main__":
     dataset = OMOPDataset(
         root="/srv/local/data/zw12/pyhealth/raw_data/synpuf1k_omop_cdm_5.2.2",
         tables=[
             "condition_occurrence",
             "procedure_occurrence",
             "drug_exposure",
             "measurement",
         ],
         dev=False,
-        refresh_cache=False,
+        refresh_cache=True,
     )
     dataset.stat()
     dataset.info()
```

### Comparing `pyhealth-1.1.3/pyhealth/datasets/sample_dataset.py` & `pyhealth-1.1.4/pyhealth/datasets/sample_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,207 @@
 from collections import Counter
 from typing import Dict, List
+import pickle
 
 from torch.utils.data import Dataset
 
 from pyhealth.datasets.utils import list_nested_levels, flatten_list
 
 
-class SampleDataset(Dataset):
-    """Sample dataset class.
+class SampleBaseDataset(Dataset):
+    """Sample base dataset class.
 
     This class the takes a list of samples as input (either from
     `BaseDataset.set_task()` or user-provided input), and provides
     a uniform interface for accessing the samples.
 
     Args:
         samples: a list of samples, each sample is a dict with
             patient_id, visit_id, and other task-specific attributes as key.
         dataset_name: the name of the dataset. Default is None.
         task_name: the name of the task. Default is None.
+    """
+
+    def __init__(self, samples: List[Dict], dataset_name="", task_name=""):
+        self.samples = samples
+        self.dataset_name: str = dataset_name
+        self.task_name: str = task_name
+        self.type_ = "base"
+
+    def __getitem__(self, index) -> Dict:
+        """Returns a sample by index.
+
+        Returns:
+             Dict, a dict with patient_id, visit_id/record_id, and other task-specific
+                attributes as key. Conversion to index/tensor will be done
+                in the model.
+        """
+        return self.samples[index]
+
+    def __str__(self):
+        """Prints some information of the dataset."""
+        return f"Sample dataset {self.dataset_name} {self.task_name}"
+
+    def __len__(self):
+        """Returns the number of samples in the dataset."""
+        return len(self.samples)
+
+    def get_all_tokens(
+        self, key: str, remove_duplicates: bool = True, sort: bool = True
+    ) -> List[str]:
+        """Gets all tokens with a specific key in the samples.
+
+        Args:
+            key: the key of the tokens in the samples.
+            remove_duplicates: whether to remove duplicates. Default is True.
+            sort: whether to sort the tokens by alphabet order. Default is True.
+
+        Returns:
+            tokens: a list of tokens.
+        """
+        input_type = self.input_info[key]["type"]
+        input_dim = self.input_info[key]["dim"]
+        if input_type in [float, int]:
+            assert input_dim == 0, f"Cannot get tokens for vector with key {key}"
+
+        tokens = []
+        for sample in self.samples:
+            if input_dim == 0:
+                # a single value
+                tokens.append(sample[key])
+            elif input_dim == 2:
+                # a list of codes
+                tokens.extend(sample[key])
+            elif input_dim == 3:
+                # a list of list of codes
+                tokens.extend(flatten_list(sample[key]))
+            else:
+                raise NotImplementedError
+        if remove_duplicates:
+            tokens = list(set(tokens))
+        if sort:
+            tokens.sort()
+        return tokens
+
+
+class SampleSignalDataset(SampleBaseDataset):
+    """Sample signal dataset class.
+
+    This class the takes a list of samples as input (either from
+    `BaseDataset.set_task()` or user-provided input), and provides
+    a uniform interface for accessing the samples.
+
+    Args:
+        samples: a list of samples, each sample is a dict with
+            patient_id, record_id, and other task-specific attributes as key.
+        classes: a list of classes, e.g., ["W", "1", "2", "3", "R"].
+        dataset_name: the name of the dataset. Default is None.
+        task_name: the name of the task. Default is None.
+    """
+
+    def __init__(self, samples: List[Dict], dataset_name="", task_name=""):
+        super().__init__(samples, dataset_name, task_name)
+        self.patient_to_index: Dict[str, List[int]] = self._index_patient()
+        self.record_to_index: Dict[str, List[int]] = self._index_record()
+        self.input_info: Dict = self._validate()
+        self.type_ = "signal"
+
+    def _index_patient(self) -> Dict[str, List[int]]:
+        """Helper function which indexes the samples by patient_id.
+
+        Will be called in `self.__init__()`.
+        Returns:
+            patient_to_index: Dict[str, int], a dict mapping patient_id to a list
+                of sample indices.
+        """
+        patient_to_index = {}
+        for idx, sample in enumerate(self.samples):
+            patient_to_index.setdefault(sample["patient_id"], []).append(idx)
+        return patient_to_index
+
+    def _index_record(self) -> Dict[str, List[int]]:
+        """Helper function which indexes the samples by record_id.
+
+        Will be called in `self.__init__()`.
+
+        Returns:
+            visit_to_index: Dict[str, int], a dict mapping record_id to a list
+                of sample indices.
+        """
+        record_to_index = {}
+        for idx, sample in enumerate(self.samples):
+            record_to_index.setdefault(sample["record_id"], []).append(idx)
+        return record_to_index
+
+    def _validate(self) -> Dict:
+        """Helper function which gets the input information of each attribute.
+
+        Will be called in `self.__init__()`.
+
+        Returns:
+            input_info: Dict, a dict whose keys are the same as the keys in the
+                samples, and values are the corresponding input information:
+                - "length": the length of the input.
+                - "n_channels": the number of channels of the input.
+
+        """
+        input_info = {}
+        # get signal info
+        sample_path_0 = self.samples[0]["epoch_path"]
+        sample = pickle.load(open(sample_path_0, "rb"))
+        n_channels, length = sample["signal"].shape
+        input_info["signal"] = {"length": length, "n_channels": n_channels}
+        # get label signal info
+        input_info["label"] = {"type": str, "dim": 0}
+        return input_info
+
+    def __getitem__(self, index) -> Dict:
+        """Returns a sample by index.
+
+        Returns:
+             Dict, a dict with patient_id, visit_id/record_id, and other task-specific
+                attributes as key. Conversion to index/tensor will be done
+                in the model.
+        """
+        sample = self.samples[index]
+        loaded_sample = pickle.load(open(sample["epoch_path"], "rb"))
+        cur_sample = sample.copy()
+        cur_sample.update(loaded_sample)
+        cur_sample.pop("epoch_path", None)
+        return cur_sample
+
+    def stat(self) -> str:
+        """Returns some statistics of the task-specific dataset."""
+        lines = list()
+        lines.append(f"Statistics of sample dataset:")
+        lines.append(f"\t- Dataset: {self.dataset_name}")
+        lines.append(f"\t- Task: {self.task_name}")
+        lines.append(f"\t- Number of samples: {len(self)}")
+        num_patients = len(set([sample["patient_id"] for sample in self.samples]))
+        lines.append(f"\t- Number of patients: {num_patients}")
+        num_records = len(set([sample["record_id"] for sample in self.samples]))
+        lines.append(f"\t- Number of visits: {num_records}")
+        lines.append(
+            f"\t- Number of samples per patient: {len(self) / num_patients:.4f}"
+        )
+        print("\n".join(lines))
+        return "\n".join(lines)
+
+
+class SampleEHRDataset(SampleBaseDataset):
+    """Sample EHR dataset class.
+
+    This class inherits from `SampleBaseDataset` and is specifically designed
+        for EHR datasets.
+
+    Args:
+        samples: a list of samples, each sample is a dict with
+            patient_id, visit_id, and other task-specific attributes as key.
+        dataset_name: the name of the dataset. Default is None.
+        task_name: the name of the task. Default is None.
 
     Currently, the following types of attributes are supported:
         - a single value. Type: int/float/str. Dim: 0.
         - a single vector. Type: int/float. Dim: 1.
         - a list of codes. Type: str. Dim: 2.
         - a list of vectors. Type: int/float. Dim: 2.
         - a list of list of codes. Type: str. Dim: 3.
@@ -35,15 +215,15 @@
             - "len": the length of the vector, only valid for vector-based attributes.
         patient_to_index: Dict[str, List[int]], a dict mapping patient_id to
             a list of sample indices.
         visit_to_index: Dict[str, List[int]], a dict mapping visit_id to a list
             of sample indices.
 
     Examples:
-        >>> from pyhealth.datasets import SampleDataset
+        >>> from pyhealth.datasets import SampleEHRDataset
         >>> samples = [
         ...         {
         ...             "patient_id": "patient-0",
         ...             "visit_id": "visit-0",
         ...             "single_vector": [1, 2, 3],
         ...             "list_codes": ["505800458", "50580045810", "50580045811"],  # NDC
         ...             "list_vectors": [[1.0, 2.55, 3.4], [4.1, 5.5, 6.0]],
@@ -70,30 +250,29 @@
         ...             "list_list_vectors": [
         ...                 [[1.0, 2.8, 3.3], [4.9, 5.0, 6.6]],
         ...                 [[7.7, 8.4, 1.3]],
         ...             ],
         ...             "label": 0,
         ...         },
         ...     ]
-        >>> dataset = SampleDataset(samples=samples)
+        >>> dataset = SampleEHRDataset(samples=samples)
         >>> dataset.input_info
         {'patient_id': {'type': <class 'str'>, 'dim': 0}, 'visit_id': {'type': <class 'str'>, 'dim': 0}, 'single_vector': {'type': <class 'int'>, 'dim': 1, 'len': 3}, 'list_codes': {'type': <class 'str'>, 'dim': 2}, 'list_vectors': {'type': <class 'float'>, 'dim': 2, 'len': 3}, 'list_list_codes': {'type': <class 'str'>, 'dim': 3}, 'list_list_vectors': {'type': <class 'float'>, 'dim': 3, 'len': 3}, 'label': {'type': <class 'int'>, 'dim': 0}}
         >>> dataset.patient_to_index
         {'patient-0': [0, 1]}
         >>> dataset.visit_to_index
         {'visit-0': [0], 'visit-1': [1]}
     """
 
     def __init__(self, samples: List[Dict], dataset_name="", task_name=""):
-        self.samples = samples
-        self.dataset_name: str = dataset_name
-        self.task_name: str = task_name
+        super().__init__(samples, dataset_name, task_name)
         self.input_info: Dict = self._validate()
         self.patient_to_index: Dict[str, List[int]] = self._index_patient()
         self.visit_to_index: Dict[str, List[int]] = self._index_visit()
+        self.type_ = "ehr"
 
     def _validate(self) -> Dict:
         """Helper function which validates the samples.
 
         Will be called in `self.__init__()`.
 
         Returns:
@@ -248,83 +427,28 @@
 
         Returns:
             List of available keys.
         """
         keys = self.samples[0].keys()
         return list(keys)
 
-    def get_all_tokens(
-        self, key: str, remove_duplicates: bool = True, sort: bool = True
-    ) -> List[str]:
-        """Gets all tokens with a specific key in the samples.
-
-        Args:
-            key: the key of the tokens in the samples.
-            remove_duplicates: whether to remove duplicates. Default is True.
-            sort: whether to sort the tokens by alphabet order. Default is True.
-
-        Returns:
-            tokens: a list of tokens.
-        """
-        input_type = self.input_info[key]["type"]
-        input_dim = self.input_info[key]["dim"]
-        if input_type in [float, int]:
-            assert input_dim == 0, f"Cannot get tokens for vector with key {key}"
-
-        tokens = []
-        for sample in self.samples:
-            if input_dim == 0:
-                # a single value
-                tokens.append(sample[key])
-            elif input_dim == 2:
-                # a list of codes
-                tokens.extend(sample[key])
-            elif input_dim == 3:
-                # a list of list of codes
-                tokens.extend(flatten_list(sample[key]))
-            else:
-                raise NotImplementedError
-        if remove_duplicates:
-            tokens = list(set(tokens))
-        if sort:
-            tokens.sort()
-        return tokens
-
     def get_distribution_tokens(self, key: str) -> Dict[str, int]:
         """Gets the distribution of tokens with a specific key in the samples.
 
         Args:
             key: the key of the tokens in the samples.
 
         Returns:
             distribution: a dict mapping token to count.
         """
 
         tokens = self.get_all_tokens(key, remove_duplicates=False, sort=False)
         counter = Counter(tokens)
         return counter
 
-    def __getitem__(self, index) -> Dict:
-        """Returns a sample by index.
-
-        Returns:
-             Dict, a dict with patient_id, visit_id, and other task-specific
-                attributes as key. Conversion to index/tensor will be done
-                in the model.
-        """
-        return self.samples[index]
-
-    def __str__(self):
-        """Prints some information of the dataset."""
-        return f"Sample dataset {self.dataset_name} {self.task_name}"
-
-    def __len__(self):
-        """Returns the number of samples in the dataset."""
-        return len(self.samples)
-
     def stat(self) -> str:
         """Returns some statistics of the task-specific dataset."""
         lines = list()
         lines.append(f"Statistics of sample dataset:")
         lines.append(f"\t- Dataset: {self.dataset_name}")
         lines.append(f"\t- Task: {self.task_name}")
         lines.append(f"\t- Number of samples: {len(self)}")
@@ -407,12 +531,12 @@
                 [[1.0, 2.8, 3.3], [4.9, 5.0, 6.6]],
                 [[7.7, 8.4, 1.3]],
             ],
             "label": 0,
         },
     ]
 
-    dataset = SampleDataset(samples=samples)
+    dataset = SampleEHRDataset(samples=samples)
 
     dataset.stat()
     data = iter(dataset)
     print(next(data))
```

### Comparing `pyhealth-1.1.3/pyhealth/datasets/splitter.py` & `pyhealth-1.1.4/pyhealth/datasets/splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from itertools import chain
 from typing import Optional, Tuple, Union, List
 
 import numpy as np
 import torch
 
-from pyhealth.datasets import SampleDataset
+from pyhealth.datasets import SampleBaseDataset
 
 
 # TODO: train_dataset.dataset still access the whole dataset which may leak information
 # TODO: add more splitting methods
 
 
 def split_by_visit(
-    dataset: SampleDataset,
+    dataset: SampleBaseDataset,
     ratios: Union[Tuple[float, float, float], List[float]],
     seed: Optional[int] = None,
 ):
     """Splits the dataset by visit (i.e., samples).
 
     Args:
-        dataset: a `SampleDataset` object
+        dataset: a `SampleBaseDataset` object
         ratios: a list/tuple of ratios for train / val / test
         seed: random seed for shuffling the dataset
 
     Returns:
         train_dataset, val_dataset, test_dataset: three subsets of the dataset of
             type `torch.utils.data.Subset`.
 
@@ -44,22 +44,22 @@
     train_dataset = torch.utils.data.Subset(dataset, train_index)
     val_dataset = torch.utils.data.Subset(dataset, val_index)
     test_dataset = torch.utils.data.Subset(dataset, test_index)
     return train_dataset, val_dataset, test_dataset
 
 
 def split_by_patient(
-    dataset: SampleDataset,
+    dataset: SampleBaseDataset,
     ratios: Union[Tuple[float, float, float], List[float]],
     seed: Optional[int] = None,
 ):
     """Splits the dataset by patient.
 
     Args:
-        dataset: a `SampleDataset` object
+        dataset: a `SampleBaseDataset` object
         ratios: a list/tuple of ratios for train / val / test
         seed: random seed for shuffling the dataset
 
     Returns:
         train_dataset, val_dataset, test_dataset: three subsets of the dataset of
             type `torch.utils.data.Subset`.
```

### Comparing `pyhealth-1.1.3/pyhealth/datasets/utils.py` & `pyhealth-1.1.4/pyhealth/datasets/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import hashlib
 import os
 from datetime import datetime
 from typing import List, Tuple, Optional
+import pickle
 
 from dateutil.parser import parse as dateutil_parse
 from torch.utils.data import DataLoader
 
 from pyhealth import BASE_CACHE_PATH
 from pyhealth.utils import create_directory
 
 MODULE_CACHE_PATH = os.path.join(BASE_CACHE_PATH, "datasets")
 create_directory(MODULE_CACHE_PATH)
 
 
+# basic tables which are a part of the defined datasets
+DATASET_BASIC_TABLES = {
+    "MIMIC3Dataset": {"PATIENTS", "ADMISSIONS"},
+    "MIMIC4Dataset": {"patients", "admission"},
+}
+
+
 def hash_str(s):
     return hashlib.md5(s.encode()).hexdigest()
 
 
 def strptime(s: str) -> Optional[datetime]:
     """Helper function which parses a string to datetime object.
 
@@ -27,14 +35,27 @@
         Optional[datetime], parsed datetime object. If s is nan, return None.
     """
     # return None if s is nan
     if s != s:
         return None
     return dateutil_parse(s)
 
+def padyear(year: str, month='1', day='1') -> str:
+    """Pad a date time year of format 'YYYY' to format 'YYYY-MM-DD'
+    
+    Args: 
+        year: str, year to be padded. Must be non-zero value.
+        month: str, month string to be used as padding. Must be in [1, 12]
+        day: str, day string to be used as padding. Must be in [1, 31]
+        
+    Returns:
+        padded_date: str, padded year.
+    
+    """
+    return f"{year}-{month}-{day}"
 
 def flatten_list(l: List) -> List:
     """Flattens a list of list.
 
     Args:
         l: List, the list of list to be flattened.
 
@@ -113,17 +134,22 @@
 
 
 def collate_fn_dict(batch):
     return {key: [d[key] for d in batch] for key in batch[0]}
 
 
 def get_dataloader(dataset, batch_size, shuffle=False):
+
     dataloader = DataLoader(
-        dataset, batch_size=batch_size, shuffle=shuffle, collate_fn=collate_fn_dict
+        dataset,
+        batch_size=batch_size,
+        shuffle=shuffle,
+        collate_fn=collate_fn_dict,
     )
+
     return dataloader
 
 
 if __name__ == "__main__":
     print(list_nested_levels([1, 2, 3]))
     print(list_nested_levels([1, [2], 3]))
     print(list_nested_levels([[1, [2], [[3]]]]))
```

### Comparing `pyhealth-1.1.3/pyhealth/medcode/codes/atc.py` & `pyhealth-1.1.4/pyhealth/medcode/codes/atc.py`

 * *Files identical despite different names*

### Comparing `pyhealth-1.1.3/pyhealth/medcode/codes/icd10cm.py` & `pyhealth-1.1.4/pyhealth/medcode/codes/icd10cm.py`

 * *Files identical despite different names*

### Comparing `pyhealth-1.1.3/pyhealth/medcode/codes/icd10proc.py` & `pyhealth-1.1.4/pyhealth/medcode/codes/icd10proc.py`

 * *Files identical despite different names*

### Comparing `pyhealth-1.1.3/pyhealth/medcode/codes/icd9cm.py` & `pyhealth-1.1.4/pyhealth/medcode/codes/icd9cm.py`

 * *Files identical despite different names*

### Comparing `pyhealth-1.1.3/pyhealth/medcode/codes/icd9proc.py` & `pyhealth-1.1.4/pyhealth/medcode/codes/icd9proc.py`

 * *Files identical despite different names*

### Comparing `pyhealth-1.1.3/pyhealth/medcode/codes/ndc.py` & `pyhealth-1.1.4/pyhealth/medcode/codes/ndc.py`

 * *Files identical despite different names*

### Comparing `pyhealth-1.1.3/pyhealth/medcode/cross_map.py` & `pyhealth-1.1.4/pyhealth/medcode/cross_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,17 @@
             save_pickle(self.mapping, pickle_filepath)
 
         # load source and target vocabulary classes
         self.s_class = getattr(medcode, source_vocabulary)()
         self.t_class = getattr(medcode, target_vocabulary)()
         return
 
+    def __repr__(self):
+        return f"CrossMap(source_vocabulary={self.s_vocab}, source_class={self.s_class} target_vocabulary={self.t_vocab}, target_class={self.t_class})"
+
     @classmethod
     def load(
         cls,
         source_vocabulary: str,
         target_vocabulary: str,
         refresh_cache: bool = False,
     ):
@@ -106,8 +109,8 @@
             source_kwargs = {}
         if target_kwargs is None:
             target_kwargs = {}
         source_code = self.s_class.standardize(source_code)
         source_code = self.s_class.convert(source_code, **source_kwargs)
         target_codes = self.mapping[source_code]
         target_codes = [self.t_class.convert(c, **target_kwargs) for c in target_codes]
-        return target_codes
+        return target_codes
```

### Comparing `pyhealth-1.1.3/pyhealth/medcode/inner_map.py` & `pyhealth-1.1.4/pyhealth/medcode/inner_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     def __init__(
         self,
         vocabulary: str,
         refresh_cache: bool = False,
     ):
         # abstractmethod prevents initialization of this class
         self.vocabulary = vocabulary
-        self.refresh_cache = refresh_cache
 
         pickle_filepath = os.path.join(MODULE_CACHE_PATH, self.vocabulary + ".pkl")
         csv_filename = self.vocabulary + ".csv"
         if os.path.exists(pickle_filepath) and (not refresh_cache):
             logger.debug(f"Loaded {vocabulary} code from {pickle_filepath}")
             self.graph = load_pickle(pickle_filepath)
         else:
@@ -56,14 +55,17 @@
                 if "parent_code" in row:
                     if not pd.isna(row["parent_code"]):
                         self.graph.add_edge(row["parent_code"], code)
             logger.debug(f"Saved {vocabulary} code to {pickle_filepath}")
             save_pickle(self.graph, pickle_filepath)
         return
 
+    def __repr__(self):
+        return f"InnerMap(vocabulary={self.vocabulary}, graph={self.graph})"
+
     @classmethod
     def load(_, vocabulary: str, refresh_cache: bool = False):
         """Initializes a specific medical code system inheriting from `InnerMap`.
 
         Args:
             vocabulary: vocabulary name. E.g., "ICD9CM", "ICD9PROC".
             refresh_cache: whether to refresh the cache. Default is False.
@@ -173,8 +175,8 @@
 
 if __name__ == "__main__":
     icd9cm = InnerMap.load("ICD9CM")
     print(icd9cm.stat())
     print("428.0" in icd9cm)
     print(icd9cm.lookup("4280"))
     print(icd9cm.get_ancestors("428.0"))
-    print(icd9cm.get_descendants("428.0"))
+    print(icd9cm.get_descendants("428.0"))
```

### Comparing `pyhealth-1.1.3/pyhealth/metrics/binary.py` & `pyhealth-1.1.4/pyhealth/metrics/binary.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from typing import List, Optional, Dict
+from typing import Dict, List, Optional
 
 import numpy as np
 import sklearn.metrics as sklearn_metrics
 
+import pyhealth.metrics.calibration as calib
+
 
 def binary_metrics_fn(
     y_true: np.ndarray,
     y_prob: np.ndarray,
     metrics: Optional[List[str]] = None,
     threshold: float = 0.5,
 ) -> Dict[str, float]:
@@ -14,20 +16,22 @@
 
     User can specify which metrics to compute by passing a list of metric names.
     The accepted metric names are:
         - pr_auc: area under the precision-recall curve
         - roc_auc: area under the receiver operating characteristic curve
         - accuracy: accuracy score
         - balanced_accuracy: balanced accuracy score (usually used for imbalanced
-            datasets)
+          datasets)
         - f1: f1 score
         - precision: precision score
         - recall: recall score
         - cohen_kappa: Cohen's kappa score
         - jaccard: Jaccard similarity coefficient score
+        - ECE: Expected Calibration Error (with 20 equal-width bins). Check :func:`pyhealth.metrics.calibration.ece_confidence_binary`.
+        - ECE_adapt: adaptive ECE (with 20 equal-size bins). Check :func:`pyhealth.metrics.calibration.ece_confidence_binary`.
     If no metrics are specified, pr_auc, roc_auc and f1 are computed by default.
 
     This function calls sklearn.metrics functions to compute the metrics. For
     more information on the metrics, please refer to the documentation of the
     corresponding sklearn.metrics functions.
 
     Args:
@@ -79,14 +83,18 @@
             output["recall"] = recall
         elif metric == "cohen_kappa":
             cohen_kappa = sklearn_metrics.cohen_kappa_score(y_true, y_pred)
             output["cohen_kappa"] = cohen_kappa
         elif metric == "jaccard":
             jaccard = sklearn_metrics.jaccard_score(y_true, y_pred)
             output["jaccard"] = jaccard
+        elif metric in {"ECE", "ECE_adapt"}:
+            output[metric] = calib.ece_confidence_binary(
+                y_prob, y_true, bins=20, adaptive=metric.endswith("_adapt")
+            )
         else:
             raise ValueError(f"Unknown metric for binary classification: {metric}")
     return output
 
 
 if __name__ == "__main__":
     all_metrics = [
```

### Comparing `pyhealth-1.1.3/pyhealth/metrics/drug_recommendation.py` & `pyhealth-1.1.4/pyhealth/metrics/drug_recommendation.py`

 * *Files identical despite different names*

### Comparing `pyhealth-1.1.3/pyhealth/metrics/multilabel.py` & `pyhealth-1.1.4/pyhealth/metrics/multilabel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-from typing import List, Optional, Dict
+from typing import Dict, List, Optional
 
 import numpy as np
 import sklearn.metrics as sklearn_metrics
 
+import pyhealth.metrics.calibration as calib
+
 
 def multilabel_metrics_fn(
     y_true: np.ndarray,
     y_prob: np.ndarray,
     metrics: Optional[List[str]] = None,
     threshold: float = 0.5,
 ) -> Dict[str, float]:
     """Computes metrics for multilabel classification.
 
     User can specify which metrics to compute by passing a list of metric names.
     The accepted metric names are:
         - roc_auc_micro: area under the receiver operating characteristic curve,
-            micro averaged
+          micro averaged
         - roc_auc_macro: area under the receiver operating characteristic curve,
-            macro averaged
+          macro averaged
         - roc_auc_weighted: area under the receiver operating characteristic curve,
-            weighted averaged
+          weighted averaged
         - roc_auc_samples: area under the receiver operating characteristic curve,
-            samples averaged
+          samples averaged
         - pr_auc_micro: area under the precision recall curve, micro averaged
         - pr_auc_macro: area under the precision recall curve, macro averaged
         - pr_auc_weighted: area under the precision recall curve, weighted averaged
         - pr_auc_samples: area under the precision recall curve, samples averaged
         - accuracy: accuracy score
         - f1_micro: f1 score, micro averaged
         - f1_macro: f1 score, macro averaged
@@ -40,14 +42,17 @@
         - recall_weighted: recall score, weighted averaged
         - recall_samples: recall score, samples averaged
         - jaccard_micro: Jaccard similarity coefficient score, micro averaged
         - jaccard_macro: Jaccard similarity coefficient score, macro averaged
         - jaccard_weighted: Jaccard similarity coefficient score, weighted averaged
         - jaccard_samples: Jaccard similarity coefficient score, samples averaged
         - hamming_loss: Hamming loss
+        - cwECE: classwise ECE (with 20 equal-width bins). Check :func:`pyhealth.metrics.calibration.ece_classwise`.
+        - cwECE_adapt: classwise adaptive ECE (with 20 equal-size bins). Check :func:`pyhealth.metrics.calibration.ece_classwise`.
+
     If no metrics are specified, pr_auc_samples is computed by default.
 
     This function calls sklearn.metrics functions to compute the metrics. For
     more information on the metrics, please refer to the documentation of the
     corresponding sklearn.metrics functions.
 
     Args:
@@ -113,15 +118,15 @@
             output["pr_auc_weighted"] = pr_auc_weighted
         elif metric == "pr_auc_samples":
             pr_auc_samples = sklearn_metrics.average_precision_score(
                 y_true, y_prob, average="samples"
             )
             output["pr_auc_samples"] = pr_auc_samples
         elif metric == "accuracy":
-            accuracy = sklearn_metrics.accuracy_score(y_true, y_pred)
+            accuracy = sklearn_metrics.accuracy_score(y_true.flatten(), y_pred.flatten())
             output["accuracy"] = accuracy
         elif metric == "f1_micro":
             f1_micro = sklearn_metrics.f1_score(y_true, y_pred, average="micro")
             output["f1_micro"] = f1_micro
         elif metric == "f1_macro":
             f1_macro = sklearn_metrics.f1_score(y_true, y_pred, average="macro")
             output["f1_macro"] = f1_macro
@@ -186,14 +191,22 @@
             jaccard_samples = sklearn_metrics.jaccard_score(
                 y_true, y_pred, average="samples"
             )
             output["jaccard_samples"] = jaccard_samples
         elif metric == "hamming_loss":
             hamming_loss = sklearn_metrics.hamming_loss(y_true, y_pred)
             output["hamming_loss"] = hamming_loss
+        elif metric in {"cwECE", "cwECE_adapt"}:
+            output[metric] = calib.ece_classwise(
+                y_prob,
+                y_true,
+                bins=20,
+                adaptive=metric.endswith("_adapt"),
+                threshold=0.0,
+            )
         else:
             raise ValueError(f"Unknown metric for multilabel classification: {metric}")
 
     return output
 
 
 if __name__ == "__main__":
```

### Comparing `pyhealth-1.1.3/pyhealth/models/base_model.py` & `pyhealth-1.1.4/pyhealth/models/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC
 from typing import List, Dict, Union, Callable
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from pyhealth.datasets import SampleDataset
+from pyhealth.datasets import SampleBaseDataset
 from pyhealth.models.utils import batch_to_multihot
 from pyhealth.tokenizer import Tokenizer
 
 # TODO: add support for regression
 VALID_MODE = ["binary", "multiclass", "multilabel"]
 
 
@@ -23,15 +23,15 @@
             e.g. ["conditions", "procedures"].
         label_key: key in samples to use as label (e.g., "drugs").
         mode: one of "binary", "multiclass", or "multilabel".
     """
 
     def __init__(
         self,
-        dataset: SampleDataset,
+        dataset: SampleBaseDataset,
         feature_keys: List[str],
         label_key: str,
         mode: str,
     ):
         super(BaseModel, self).__init__()
         assert mode in VALID_MODE, f"mode must be one of {VALID_MODE}"
         self.dataset = dataset
```

### Comparing `pyhealth-1.1.3/pyhealth/models/cnn.py` & `pyhealth-1.1.4/pyhealth/models/cnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import List, Tuple, Dict
+from typing import Dict, List, Tuple
 
 import torch
 import torch.nn as nn
 
-from pyhealth.datasets import SampleDataset
+from pyhealth.datasets import SampleEHRDataset
 from pyhealth.models import BaseModel
 
 VALID_OPERATION_LEVEL = ["visit", "event"]
 
 
 class CNNBlock(nn.Module):
     """Convolutional neural network block.
@@ -162,15 +162,15 @@
         label_key: key in samples to use as label (e.g., "drugs").
         mode: one of "binary", "multiclass", or "multilabel".
         embedding_dim: the embedding dimension. Default is 128.
         hidden_dim: the hidden dimension. Default is 128.
         **kwargs: other parameters for the CNN layer.
 
     Examples:
-        >>> from pyhealth.datasets import SampleDataset
+        >>> from pyhealth.datasets import SampleEHRDataset
         >>> samples = [
         ...         {
         ...             "patient_id": "patient-0",
         ...             "visit_id": "visit-0",
         ...             "list_codes": ["505800458", "50580045810", "50580045811"],  # NDC
         ...             "list_vectors": [[1.0, 2.55, 3.4], [4.1, 5.5, 6.0]],
         ...             "list_list_codes": [["A05B", "A05C", "A06A"], ["A11D", "A11E"]],  # ATC-4
@@ -195,15 +195,15 @@
         ...             "list_list_vectors": [
         ...                 [[1.0, 2.8, 3.3], [4.9, 5.0, 6.6]],
         ...                 [[7.7, 8.4, 1.3]],
         ...             ],
         ...             "label": 0,
         ...         },
         ...     ]
-        >>> dataset = SampleDataset(samples=samples, dataset_name="test")
+        >>> dataset = SampleEHRDataset(samples=samples, dataset_name="test")
         >>>
         >>> from pyhealth.models import CNN
         >>> model = CNN(
         ...         dataset=dataset,
         ...         feature_keys=[
         ...             "list_codes",
         ...             "list_vectors",
@@ -216,23 +216,26 @@
         >>>
         >>> from pyhealth.datasets import get_dataloader
         >>> train_loader = get_dataloader(dataset, batch_size=2, shuffle=True)
         >>> data_batch = next(iter(train_loader))
         >>>
         >>> ret = model(**data_batch)
         >>> print(ret)
-        {'loss': tensor(0.8725, grad_fn=<BinaryCrossEntropyWithLogitsBackward0>), 'y_prob': tensor([[0.7620],
-                [0.7339]], grad_fn=<SigmoidBackward0>), 'y_true': tensor([[0.],
-                [1.]])}
+        {
+            'loss': tensor(0.8872, grad_fn=<BinaryCrossEntropyWithLogitsBackward0>),
+            'y_prob': tensor([[0.5008], [0.6614]], grad_fn=<SigmoidBackward0>),
+            'y_true': tensor([[1.], [0.]]),
+            'logit': tensor([[0.0033], [0.6695]], grad_fn=<AddmmBackward0>)
+        }
         >>>
     """
 
     def __init__(
         self,
-        dataset: SampleDataset,
+        dataset: SampleEHRDataset,
         feature_keys: List[str],
         label_key: str,
         mode: str,
         embedding_dim: int = 128,
         hidden_dim: int = 128,
         **kwargs,
     ):
@@ -357,23 +360,27 @@
         patient_emb = torch.cat(patient_emb, dim=1)
         # (patient, label_size)
         logits = self.fc(patient_emb)
         # obtain y_true, loss, y_prob
         y_true = self.prepare_labels(kwargs[self.label_key], self.label_tokenizer)
         loss = self.get_loss_function()(logits, y_true)
         y_prob = self.prepare_y_prob(logits)
-        return {
+        results = {
             "loss": loss,
             "y_prob": y_prob,
             "y_true": y_true,
+            "logit": logits,
         }
+        if kwargs.get("embed", False):
+            results["embed"] = patient_emb
+        return results
 
 
 if __name__ == "__main__":
-    from pyhealth.datasets import SampleDataset
+    from pyhealth.datasets import SampleEHRDataset
 
     samples = [
         {
             "patient_id": "patient-0",
             "visit_id": "visit-0",
             # "single_vector": [1, 2, 3],
             "list_codes": ["505800458", "50580045810", "50580045811"],  # NDC
@@ -402,15 +409,15 @@
                 [[1.0, 2.8, 3.3], [4.9, 5.0, 6.6], [7.7, 8.4, 1.3], [7.7, 8.4, 1.3]],
             ],
             "label": 0,
         },
     ]
 
     # dataset
-    dataset = SampleDataset(samples=samples, dataset_name="test")
+    dataset = SampleEHRDataset(samples=samples, dataset_name="test")
     print(dataset.input_info)
 
     # data loader
     from pyhealth.datasets import get_dataloader
 
     train_loader = get_dataloader(dataset, batch_size=2, shuffle=True)
```

### Comparing `pyhealth-1.1.3/pyhealth/models/deepr.py` & `pyhealth-1.1.4/pyhealth/models/deepr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Tuple, List, Dict, Optional
 import functools
+from typing import Dict, List, Optional, Tuple
 
 import torch
 import torch.nn as nn
 
-from pyhealth.datasets import BaseDataset
+from pyhealth.datasets import BaseEHRDataset
 from pyhealth.models import BaseModel
 
 
 class DeeprLayer(nn.Module):
     """Deepr layer.
 
     Paper: P. Nguyen, T. Tran, N. Wickramasinghe and S. Venkatesh,
@@ -111,15 +111,15 @@
         label_key: key in samples to use as label (e.g., "drugs").
         mode: one of "binary", "multiclass", or "multilabel".
         embedding_dim: the embedding dimension. Default is 128.
         hidden_dim: the hidden dimension. Default is 128.
         **kwargs: other parameters for the Deepr layer.
 
     Examples:
-        >>> from pyhealth.datasets import SampleDataset
+        >>> from pyhealth.datasets import SampleEHRDataset
         >>> samples = [
         ...         {
         ...             "patient_id": "patient-0",
         ...             "visit_id": "visit-0",
         ...             "list_codes": ["505800458", "50580045810", "50580045811"],  # NDC
         ...             "list_vectors": [[1.0, 2.55, 3.4], [4.1, 5.5, 6.0]],
         ...             "list_list_codes": [["A05B", "A05C", "A06A"], ["A11D", "A11E"]],  # ATC-4
@@ -143,15 +143,15 @@
         ...             "list_list_codes": [["A04A", "B035", "C129"]],
         ...             "list_list_vectors": [
         ...                 [[1.0, 2.8, 3.3], [4.9, 5.0, 6.6], [7.7, 8.4, 1.3], [7.7, 8.4, 1.3]],
         ...             ],
         ...             "label": 0,
         ...         },
         ...     ]
-        >>> dataset = SampleDataset(samples=samples, dataset_name="test")
+        >>> dataset = SampleEHRDataset(samples=samples, dataset_name="test")
         >>>
         >>> from pyhealth.models import Deepr
         >>> model = Deepr(
         ...         dataset=dataset,
         ...         feature_keys=[
         ...             "list_list_codes",
         ...             "list_list_vectors",
@@ -162,25 +162,28 @@
         >>>
         >>> from pyhealth.datasets import get_dataloader
         >>> train_loader = get_dataloader(dataset, batch_size=2, shuffle=True)
         >>> data_batch = next(iter(train_loader))
         >>>
         >>> ret = model(**data_batch)
         >>> print(ret)
-        {'loss': tensor(0.9139, device='cuda:0',
-            grad_fn=<BinaryCrossEntropyWithLogitsBackward0>), 'y_prob': tensor([[0.7530],
-                [0.6510]], device='cuda:0', grad_fn=<SigmoidBackward0>), 'y_true': tensor([[0.],
-                [1.]], device='cuda:0')}
-        >>>
-
+        {
+            'loss': tensor(0.8908, device='cuda:0', grad_fn=<BinaryCrossEntropyWithLogitsBackward0>),
+            'y_prob': tensor([[0.2295],
+                        [0.2665]], device='cuda:0', grad_fn=<SigmoidBackward0>),
+            'y_true': tensor([[1.],
+                        [0.]], device='cuda:0'),
+            'logit': tensor([[-1.2110],
+                        [-1.0126]], device='cuda:0', grad_fn=<AddmmBackward0>)
+        }
     """
 
     def __init__(
         self,
-        dataset: BaseDataset,
+        dataset: BaseEHRDataset,
         feature_keys: List[str],
         label_key: str,
         mode: str,
         embedding_dim: int = 128,
         hidden_dim: int = 128,
         **kwargs,
     ):
@@ -280,23 +283,27 @@
         patient_emb = torch.cat(patient_emb, dim=1)
         # (patient, label_size)
         logits = self.fc(patient_emb)
         # obtain y_true, loss, y_prob
         y_true = self.prepare_labels(kwargs[self.label_key], self.label_tokenizer)
         loss = self.get_loss_function()(logits, y_true)
         y_prob = self.prepare_y_prob(logits)
-        return {
+        results = {
             "loss": loss,
             "y_prob": y_prob,
             "y_true": y_true,
+            "logit": logits,
         }
+        if kwargs.get("embed", False):
+            results["embed"] = patient_emb
+        return results
 
 
 if __name__ == "__main__":
-    from pyhealth.datasets import SampleDataset
+    from pyhealth.datasets import SampleEHRDataset
 
     samples = [
         {
             "patient_id": "patient-0",
             "visit_id": "visit-0",
             "single_vector": [1, 2, 3],
             "list_codes": ["505800458", "50580045810", "50580045811"],  # NDC
@@ -325,15 +332,15 @@
                 [[1.0, 2.8, 3.3], [4.9, 5.0, 6.6], [7.7, 8.4, 1.3], [7.7, 8.4, 1.3]],
             ],
             "label": 0,
         },
     ]
 
     # dataset
-    dataset = SampleDataset(samples=samples, dataset_name="test")
+    dataset = SampleEHRDataset(samples=samples, dataset_name="test")
 
     # data loader
     from pyhealth.datasets import get_dataloader
 
     train_loader = get_dataloader(dataset, batch_size=2, shuffle=True)
 
     # model
```

### Comparing `pyhealth-1.1.3/pyhealth/models/gamenet.py` & `pyhealth-1.1.4/pyhealth/models/gamenet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 from typing import Tuple, List, Dict, Optional
 
 import torch
 import torch.nn as nn
 
-from pyhealth.datasets import SampleDataset
+from pyhealth.datasets import SampleEHRDataset
 from pyhealth.medcode import ATC
 from pyhealth.models import BaseModel
 from pyhealth.models.utils import get_last_visit, batch_to_multihot
 
 
 class GCNLayer(nn.Module):
     """GCN layer.
@@ -218,16 +218,16 @@
     """GAMENet model.
 
     Paper: Junyuan Shang et al. GAMENet: Graph Augmented MEmory Networks for
     Recommending Medication Combination AAAI 2019.
 
     Note:
         This model is only for medication prediction which takes conditions
-        and procedures as feature_keys, and drugs_all as label_key (i.e., both
-        current and previous drugs). It only operates on the visit level.
+        and procedures as feature_keys, and drugs as label_key.
+        It only operates on the visit level.
 
     Note:
         This model only accepts ATC level 3 as medication codes.
 
     Args:
         dataset: the dataset to train the model. It is used to query certain
             information such as the set of all tokens.
@@ -236,25 +236,25 @@
         num_layers: the number of layers used in RNN. Default is 1.
         dropout: the dropout rate. Default is 0.5.
         **kwargs: other parameters for the GAMENet layer.
     """
 
     def __init__(
         self,
-        dataset: SampleDataset,
+        dataset: SampleEHRDataset,
         embedding_dim: int = 128,
         hidden_dim: int = 128,
         num_layers: int = 1,
         dropout: float = 0.5,
         **kwargs
     ):
         super(GAMENet, self).__init__(
             dataset=dataset,
             feature_keys=["conditions", "procedures"],
-            label_key="drugs_all",
+            label_key="drugs",
             mode="multilabel",
         )
         self.embedding_dim = embedding_dim
         self.hidden_dim = hidden_dim
         self.num_layers = num_layers
         self.dropout = dropout
 
@@ -300,15 +300,15 @@
         )
 
     def generate_ehr_adj(self) -> torch.tensor:
         """Generates the EHR graph adjacency matrix."""
         label_size = self.label_tokenizer.get_vocabulary_size()
         ehr_adj = torch.zeros((label_size, label_size))
         for sample in self.dataset:
-            curr_drugs = sample["drugs_all"][-1]
+            curr_drugs = sample["drugs"]
             encoded_drugs = self.label_tokenizer.convert_tokens_to_indices(curr_drugs)
             for idx1, med1 in enumerate(encoded_drugs):
                 for idx2, med2 in enumerate(encoded_drugs):
                     if idx1 >= idx2:
                         continue
                     ehr_adj[med1, med2] = 1
                     ehr_adj[med2, med1] = 1
@@ -330,23 +330,25 @@
                 ddi_adj[vocab_to_index(atc_j), vocab_to_index(atc_i)] = 1
         return ddi_adj
 
     def forward(
         self,
         conditions: List[List[List[str]]],
         procedures: List[List[List[str]]],
-        drugs_all: List[List[List[str]]],
+        drugs_hist: List[List[List[str]]],
+        drugs: List[List[str]],
         **kwargs
     ) -> Dict[str, torch.Tensor]:
         """Forward propagation.
 
         Args:
             conditions: a nested list in three levels [patient, visit, condition].
             procedures: a nested list in three levels [patient, visit, procedure].
-            drugs_all: a nested list in three levels [patient, visit, drug].
+            drugs_hist: a nested list in three levels [patient, visit, drug], up to visit (N-1)
+            drugs: a nested list in two levels [patient, drug], at visit N
 
         Returns:
             A dictionary with the following keys:
                 loss: a scalar tensor representing the loss.
                 y_prob: a tensor of shape [patient, visit, num_labels] representing
                     the probability of each drug.
                 y_true: a tensor of shape [patient, visit, num_labels] representing
@@ -375,23 +377,23 @@
 
         # (batch, visit, 2 * hidden_size)
         patient_representations = torch.cat([conditions, procedures], dim=-1)
         # (batch, visit, hidden_size)
         queries = self.query(patient_representations)
 
         label_size = self.label_tokenizer.get_vocabulary_size()
-        drugs_all = self.label_tokenizer.batch_encode_3d(
-            drugs_all, padding=(False, False), truncation=(True, False)
+        drugs_hist = self.label_tokenizer.batch_encode_3d(
+            drugs_hist, padding=(False, False), truncation=(True, False)
         )
 
-        curr_drugs = [p[-1] for p in drugs_all]
+        curr_drugs = [p[-1] for p in drugs_hist]
         curr_drugs = batch_to_multihot(curr_drugs, label_size)
         curr_drugs = curr_drugs.to(self.device)
 
-        prev_drugs = [p[:-1] for p in drugs_all]
+        prev_drugs = drugs_hist
         max_num_visit = max([len(p) for p in prev_drugs])
         prev_drugs = [p + [[]] * (max_num_visit - len(p)) for p in prev_drugs]
         prev_drugs = [batch_to_multihot(p, label_size) for p in prev_drugs]
         prev_drugs = torch.stack(prev_drugs, dim=0)
         prev_drugs = prev_drugs.to(self.device)
 
         # get mask
```

### Comparing `pyhealth-1.1.3/pyhealth/models/micron.py` & `pyhealth-1.1.4/pyhealth/models/micron.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Tuple, Dict, Optional
 
 import torch
 import torch.nn as nn
 
-from pyhealth.datasets import SampleDataset
+from pyhealth.datasets import SampleEHRDataset
 from pyhealth.models import BaseModel
 from pyhealth.models.utils import get_last_visit
 
 
 class MICRONLayer(nn.Module):
     """MICRON layer.
 
@@ -125,15 +125,15 @@
         embedding_dim: the embedding dimension. Default is 128.
         hidden_dim: the hidden dimension. Default is 128.
         **kwargs: other parameters for the MICRON layer.
     """
 
     def __init__(
         self,
-        dataset: SampleDataset,
+        dataset: SampleEHRDataset,
         embedding_dim: int = 128,
         hidden_dim: int = 128,
         **kwargs
     ):
         super(MICRON, self).__init__(
             dataset=dataset,
             feature_keys=["conditions", "procedures"],
```

### Comparing `pyhealth-1.1.3/pyhealth/models/mlp.py` & `pyhealth-1.1.4/pyhealth/models/mlp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from typing import List, Tuple, Dict, Optional
+from typing import Dict, List, Optional, Tuple
 
 import torch
 import torch.nn as nn
-from pyhealth.datasets import SampleDataset
+
+from pyhealth.datasets import SampleEHRDataset
 from pyhealth.models import BaseModel
 
 
 class MLP(BaseModel):
     """Multi-layer perceptron model.
 
     This model applies a separate MLP layer for each feature, and then concatenates
@@ -47,15 +48,15 @@
         embedding_dim: the embedding dimension. Default is 128.
         hidden_dim: the hidden dimension. Default is 128.
         n_layers: the number of layers. Default is 2.
         activation: the activation function. Default is "relu".
         **kwargs: other parameters for the RNN layer.
 
     Examples:
-        >>> from pyhealth.datasets import SampleDataset
+        >>> from pyhealth.datasets import SampleEHRDataset
         >>> samples = [
         ...         {
         ...             "patient_id": "patient-0",
         ...             "visit_id": "visit-0",
         ...             "conditions": ["cond-33", "cond-86", "cond-80"],
         ...             "procedures": [1.0, 2.0, 3.5, 4],
         ...             "label": 0,
@@ -64,15 +65,15 @@
         ...             "patient_id": "patient-0",
         ...             "visit_id": "visit-0",
         ...             "conditions": ["cond-33", "cond-86", "cond-80"],
         ...             "procedures": [5.0, 2.0, 3.5, 4],
         ...             "label": 1,
         ...         },
         ...     ]
-        >>> dataset = SampleDataset(samples=samples, dataset_name="test")
+        >>> dataset = SampleEHRDataset(samples=samples, dataset_name="test")
         >>>
         >>> from pyhealth.models import MLP
         >>> model = MLP(
         ...         dataset=dataset,
         ...         feature_keys=["conditions", "procedures"],
         ...         label_key="label",
         ...         mode="binary",
@@ -80,24 +81,30 @@
         >>>
         >>> from pyhealth.datasets import get_dataloader
         >>> train_loader = get_dataloader(dataset, batch_size=2, shuffle=True)
         >>> data_batch = next(iter(train_loader))
         >>>
         >>> ret = model(**data_batch)
         >>> print(ret)
-        {'loss': tensor(0.6816, grad_fn=<BinaryCrossEntropyWithLogitsBackward0>), 'y_prob': tensor([[0.5418],
-                [0.5584]], grad_fn=<SigmoidBackward0>), 'y_true': tensor([[0.],
-                [1.]])}
+        {
+            'loss': tensor(0.6659, grad_fn=<BinaryCrossEntropyWithLogitsBackward0>),
+            'y_prob': tensor([[0.5680],
+                            [0.5352]], grad_fn=<SigmoidBackward0>),
+            'y_true': tensor([[1.],
+                            [0.]]),
+            'logit': tensor([[0.2736],
+                            [0.1411]], grad_fn=<AddmmBackward0>)
+        }
         >>>
 
     """
 
     def __init__(
         self,
-        dataset: SampleDataset,
+        dataset: SampleEHRDataset,
         feature_keys: List[str],
         label_key: str,
         mode: str,
         embedding_dim: int = 128,
         hidden_dim: int = 128,
         n_layers: int = 2,
         activation: str = "relu",
@@ -232,15 +239,15 @@
                     kwargs[feature_key]
                 )
                 # (patient, event)
                 x = torch.tensor(x, dtype=torch.long, device=self.device)
                 # (patient, event, embedding_dim)
                 x = self.embeddings[feature_key](x)
                 # (patient, event)
-                mask = torch.sum(x, dim=2) != 0
+                mask = torch.any(x !=0, dim=2)
                 # (patient, embedding_dim)
                 x = self.mean_pooling(x, mask)
 
             # for case 2: [[code1, code2], [code3, ...], ...]
             elif (dim_ == 3) and (type_ == str):
                 x = self.feat_tokenizers[feature_key].batch_encode_3d(
                     kwargs[feature_key]
@@ -248,15 +255,15 @@
                 # (patient, visit, event)
                 x = torch.tensor(x, dtype=torch.long, device=self.device)
                 # (patient, visit, event, embedding_dim)
                 x = self.embeddings[feature_key](x)
                 # (patient, visit, embedding_dim)
                 x = torch.sum(x, dim=2)
                 # (patient, visit)
-                mask = torch.sum(x, dim=2) != 0
+                mask = torch.any(x !=0, dim=2)
                 # (patient, embedding_dim)
                 x = self.mean_pooling(x, mask)
 
             # for case 3: [1.5, 2.0, 0.0]
             elif (dim_ == 1) and (type_ in [float, int]):
                 # (patient, values)
                 x = torch.tensor(
@@ -298,23 +305,27 @@
         patient_emb = torch.cat(patient_emb, dim=1)
         # (patient, label_size)
         logits = self.fc(patient_emb)
         # obtain y_true, loss, y_prob
         y_true = self.prepare_labels(kwargs[self.label_key], self.label_tokenizer)
         loss = self.get_loss_function()(logits, y_true)
         y_prob = self.prepare_y_prob(logits)
-        return {
+        results = {
             "loss": loss,
             "y_prob": y_prob,
             "y_true": y_true,
+            "logit": logits,
         }
+        if kwargs.get("embed", False):
+            results["embed"] = patient_emb
+        return results
 
 
 if __name__ == "__main__":
-    from pyhealth.datasets import SampleDataset
+    from pyhealth.datasets import SampleEHRDataset
 
     samples = [
         {
             "patient_id": "patient-0",
             "visit_id": "visit-0",
             "conditions": ["cond-33", "cond-86", "cond-80"],
             "procedures": [1.0, 2.0, 3.5, 4],
@@ -326,15 +337,15 @@
             "conditions": ["cond-33", "cond-86", "cond-80"],
             "procedures": [5.0, 2.0, 3.5, 4],
             "label": 1,
         },
     ]
 
     # dataset
-    dataset = SampleDataset(samples=samples, dataset_name="test")
+    dataset = SampleEHRDataset(samples=samples, dataset_name="test")
 
     # data loader
     from pyhealth.datasets import get_dataloader
 
     train_loader = get_dataloader(dataset, batch_size=2, shuffle=True)
 
     # model
```

### Comparing `pyhealth-1.1.3/pyhealth/models/retain.py` & `pyhealth-1.1.4/pyhealth/models/retain.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import List, Tuple, Dict, Optional
+from typing import Dict, List, Optional, Tuple
 
 import torch
 import torch.nn as nn
 import torch.nn.utils.rnn as rnn_utils
 
-from pyhealth.datasets import SampleDataset
+from pyhealth.datasets import SampleEHRDataset
 from pyhealth.models import BaseModel
 
 # VALID_OPERATION_LEVEL = ["visit", "event"]
 
 
 class RETAINLayer(nn.Module):
     """RETAIN layer.
@@ -144,76 +144,17 @@
         feature_keys:  list of keys in samples to use as features,
             e.g. ["conditions", "procedures"].
         label_key: key in samples to use as label (e.g., "drugs").
         mode: one of "binary", "multiclass", or "multilabel".
         embedding_dim: the embedding dimension. Default is 128.
         **kwargs: other parameters for the RETAIN layer.
 
-    Examples:
-        >>> from pyhealth.datasets import SampleDataset
-        >>> samples = [
-        ...         {
-        ...             "patient_id": "patient-0",
-        ...             "visit_id": "visit-0",
-        ...             "list_codes": ["505800458", "50580045810", "50580045811"],  # NDC
-        ...             "list_vectors": [[1.0, 2.55, 3.4], [4.1, 5.5, 6.0]],
-        ...             "list_list_codes": [["A05B", "A05C", "A06A"], ["A11D", "A11E"]],  # ATC-4
-        ...             "list_list_vectors": [
-        ...                 [[1.8, 2.25, 3.41], [4.50, 5.9, 6.0]],
-        ...                 [[7.7, 8.5, 9.4]],
-        ...             ],
-        ...             "label": 1,
-        ...         },
-        ...         {
-        ...             "patient_id": "patient-0",
-        ...             "visit_id": "visit-1",
-        ...             "list_codes": [
-        ...                 "55154191800",
-        ...                 "551541928",
-        ...                 "55154192800",
-        ...                 "705182798",
-        ...                 "70518279800",
-        ...             ],
-        ...             "list_vectors": [[1.4, 3.2, 3.5], [4.1, 5.9, 1.7]],
-        ...             "list_list_codes": [["A04A", "B035", "C129"], ["A07B", "A07C"]],
-        ...             "list_list_vectors": [
-        ...                 [[1.0, 2.8, 3.3], [4.9, 5.0, 6.6]],
-        ...                 [[7.7, 8.4, 1.3]],
-        ...             ],
-        ...             "label": 0,
-        ...         },
-        ...     ]
-        >>> dataset = SampleDataset(samples=samples, dataset_name="test")
-        >>>
-        >>> from pyhealth.models import CNN
-        >>> model = CNN(
-        ...         dataset=dataset,
-        ...         feature_keys=[
-        ...             "list_codes",
-        ...             "list_vectors",
-        ...             "list_list_codes",
-        ...             # "list_list_vectors",
-        ...         ],
-        ...         label_key="label",
-        ...         mode="binary",
-        ...     )
-        >>>
-        >>> from pyhealth.datasets import get_dataloader
-        >>> train_loader = get_dataloader(dataset, batch_size=2, shuffle=True)
-        >>> data_batch = next(iter(train_loader))
-        >>>
-        >>> ret = model(**data_batch)
-        >>> print(ret)
-        {'loss': tensor(0.8725, grad_fn=<BinaryCrossEntropyWithLogitsBackward0>), 'y_prob': tensor([[0.7620],
-                [0.7339]], grad_fn=<SigmoidBackward0>), 'y_true': tensor([[0.],
-                [1.]])}
-        >>>
 
     Examples:
-        >>> from pyhealth.datasets import SampleDataset
+        >>> from pyhealth.datasets import SampleEHRDataset
         >>> samples = [
         ...         {
         ...             "patient_id": "patient-0",
         ...             "visit_id": "visit-0",
         ...             "list_codes": ["505800458", "50580045810", "50580045811"],  # NDC
         ...             "list_vectors": [[1.0, 2.55, 3.4], [4.1, 5.5, 6.0]],
         ...             "list_list_codes": [["A05B", "A05C", "A06A"], ["A11D", "A11E"]],  # ATC-4
@@ -237,15 +178,15 @@
         ...             "list_list_codes": [["A04A", "B035", "C129"]],
         ...             "list_list_vectors": [
         ...                 [[1.0, 2.8, 3.3], [4.9, 5.0, 6.6], [7.7, 8.4, 1.3], [7.7, 8.4, 1.3]],
         ...             ],
         ...             "label": 0,
         ...         },
         ...     ]
-        >>> dataset = SampleDataset(samples=samples, dataset_name="test")
+        >>> dataset = SampleEHRDataset(samples=samples, dataset_name="test")
         >>>
         >>> from pyhealth.models import RETAIN
         >>> model = RETAIN(
         ...         dataset=dataset,
         ...         feature_keys=[
         ...             "list_codes",
         ...             "list_vectors",
@@ -258,24 +199,30 @@
         >>>
         >>> from pyhealth.datasets import get_dataloader
         >>> train_loader = get_dataloader(dataset, batch_size=2, shuffle=True)
         >>> data_batch = next(iter(train_loader))
         >>>
         >>> ret = model(**data_batch)
         >>> print(ret)
-        {'loss': tensor(0.7234, grad_fn=<BinaryCrossEntropyWithLogitsBackward0>), 'y_prob': tensor([[0.5423],
-                [0.5142]], grad_fn=<SigmoidBackward0>), 'y_true': tensor([[0.],
-                [1.]])}
+        {
+            'loss': tensor(0.5640, grad_fn=<BinaryCrossEntropyWithLogitsBackward0>),
+            'y_prob': tensor([[0.5325],
+                            [0.3922]], grad_fn=<SigmoidBackward0>),
+            'y_true': tensor([[1.],
+                            [0.]]),
+            'logit': tensor([[ 0.1303],
+                            [-0.4382]], grad_fn=<AddmmBackward0>)
+        }
         >>>
 
     """
 
     def __init__(
         self,
-        dataset: SampleDataset,
+        dataset: SampleEHRDataset,
         feature_keys: List[str],
         label_key: str,
         mode: str,
         embedding_dim: int = 128,
         **kwargs,
     ):
         super(RETAIN, self).__init__(
@@ -404,23 +351,27 @@
         patient_emb = torch.cat(patient_emb, dim=1)
         # (patient, label_size)
         logits = self.fc(patient_emb)
         # obtain y_true, loss, y_prob
         y_true = self.prepare_labels(kwargs[self.label_key], self.label_tokenizer)
         loss = self.get_loss_function()(logits, y_true)
         y_prob = self.prepare_y_prob(logits)
-        return {
+        results = {
             "loss": loss,
             "y_prob": y_prob,
             "y_true": y_true,
+            "logit": logits,
         }
+        if kwargs.get("embed", False):
+            results["embed"] = patient_emb
+        return results
 
 
 if __name__ == "__main__":
-    from pyhealth.datasets import SampleDataset
+    from pyhealth.datasets import SampleEHRDataset
 
     samples = [
         {
             "patient_id": "patient-0",
             "visit_id": "visit-0",
             # "single_vector": [1, 2, 3],
             "list_codes": ["505800458", "50580045810", "50580045811"],  # NDC
@@ -449,15 +400,15 @@
                 [[1.0, 2.8, 3.3], [4.9, 5.0, 6.6], [7.7, 8.4, 1.3], [7.7, 8.4, 1.3]],
             ],
             "label": 0,
         },
     ]
 
     # dataset
-    dataset = SampleDataset(samples=samples, dataset_name="test")
+    dataset = SampleEHRDataset(samples=samples, dataset_name="test")
 
     # data loader
     from pyhealth.datasets import get_dataloader
 
     train_loader = get_dataloader(dataset, batch_size=2, shuffle=True)
 
     # model
```

### Comparing `pyhealth-1.1.3/pyhealth/models/rnn.py` & `pyhealth-1.1.4/pyhealth/models/rnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from typing import List, Tuple, Dict, Optional
+from typing import Dict, List, Optional, Tuple
 
 import torch
 import torch.nn as nn
 import torch.nn.utils.rnn as rnn_utils
 
-from pyhealth.datasets import SampleDataset
+from pyhealth.datasets import SampleEHRDataset
 from pyhealth.models import BaseModel
 
-
 # VALID_OPERATION_LEVEL = ["visit", "event"]
 
 
 class RNNLayer(nn.Module):
     """Recurrent neural network layer.
 
     This layer wraps the PyTorch RNN layer with masking and dropout support. It is
@@ -155,15 +154,15 @@
         label_key: key in samples to use as label (e.g., "drugs").
         mode: one of "binary", "multiclass", or "multilabel".
         embedding_dim: the embedding dimension. Default is 128.
         hidden_dim: the hidden dimension. Default is 128.
         **kwargs: other parameters for the RNN layer.
 
     Examples:
-        >>> from pyhealth.datasets import SampleDataset
+        >>> from pyhealth.datasets import SampleEHRDataset
         >>> samples = [
         ...         {
         ...             "patient_id": "patient-0",
         ...             "visit_id": "visit-0",
         ...             "list_codes": ["505800458", "50580045810", "50580045811"],  # NDC
         ...             "list_vectors": [[1.0, 2.55, 3.4], [4.1, 5.5, 6.0]],
         ...             "list_list_codes": [["A05B", "A05C", "A06A"], ["A11D", "A11E"]],  # ATC-4
@@ -187,15 +186,15 @@
         ...             "list_list_codes": [["A04A", "B035", "C129"]],
         ...             "list_list_vectors": [
         ...                 [[1.0, 2.8, 3.3], [4.9, 5.0, 6.6], [7.7, 8.4, 1.3], [7.7, 8.4, 1.3]],
         ...             ],
         ...             "label": 0,
         ...         },
         ...     ]
-        >>> dataset = SampleDataset(samples=samples, dataset_name="test")
+        >>> dataset = SampleEHRDataset(samples=samples, dataset_name="test")
         >>>
         >>> from pyhealth.models import RNN
         >>> model = RNN(
         ...         dataset=dataset,
         ...         feature_keys=[
         ...             "list_codes",
         ...             "list_vectors",
@@ -208,25 +207,31 @@
         >>>
         >>> from pyhealth.datasets import get_dataloader
         >>> train_loader = get_dataloader(dataset, batch_size=2, shuffle=True)
         >>> data_batch = next(iter(train_loader))
         >>>
         >>> ret = model(**data_batch)
         >>> print(ret)
-        {'loss': tensor(0.7664, grad_fn=<BinaryCrossEntropyWithLogitsBackward0>), 'y_prob': tensor([[0.4714],
-                [0.4085]], grad_fn=<SigmoidBackward0>), 'y_true': tensor([[0.],
-                [1.]])}
+        {
+            'loss': tensor(0.8056, grad_fn=<BinaryCrossEntropyWithLogitsBackward0>),
+            'y_prob': tensor([[0.5906],
+                            [0.6620]], grad_fn=<SigmoidBackward0>),
+            'y_true': tensor([[1.],
+                            [0.]]),
+            'logit': tensor([[0.3666],
+                            [0.6721]], grad_fn=<AddmmBackward0>)
+        }
         >>>
 
 
     """
 
     def __init__(
         self,
-        dataset: SampleDataset,
+        dataset: SampleEHRDataset,
         feature_keys: List[str],
         label_key: str,
         mode: str,
         embedding_dim: int = 128,
         hidden_dim: int = 128,
         **kwargs
     ):
@@ -309,29 +314,29 @@
                     kwargs[feature_key]
                 )
                 # (patient, event)
                 x = torch.tensor(x, dtype=torch.long, device=self.device)
                 # (patient, event, embedding_dim)
                 x = self.embeddings[feature_key](x)
                 # (patient, event)
-                mask = torch.sum(x, dim=2) != 0
+                mask = torch.any(x !=0, dim=2)
 
             # for case 2: [[code1, code2], [code3, ...], ...]
             elif (dim_ == 3) and (type_ == str):
                 x = self.feat_tokenizers[feature_key].batch_encode_3d(
                     kwargs[feature_key]
                 )
                 # (patient, visit, event)
                 x = torch.tensor(x, dtype=torch.long, device=self.device)
                 # (patient, visit, event, embedding_dim)
                 x = self.embeddings[feature_key](x)
                 # (patient, visit, embedding_dim)
                 x = torch.sum(x, dim=2)
                 # (patient, visit)
-                mask = torch.sum(x, dim=2) != 0
+                mask = torch.any(x !=0, dim=2)
 
             # for case 3: [[1.5, 2.0, 0.0], ...]
             elif (dim_ == 2) and (type_ in [float, int]):
                 x, mask = self.padding2d(kwargs[feature_key])
                 # (patient, event, values)
                 x = torch.tensor(x, dtype=torch.float, device=self.device)
                 # (patient, event, embedding_dim)
@@ -360,23 +365,22 @@
         patient_emb = torch.cat(patient_emb, dim=1)
         # (patient, label_size)
         logits = self.fc(patient_emb)
         # obtain y_true, loss, y_prob
         y_true = self.prepare_labels(kwargs[self.label_key], self.label_tokenizer)
         loss = self.get_loss_function()(logits, y_true)
         y_prob = self.prepare_y_prob(logits)
-        return {
-            "loss": loss,
-            "y_prob": y_prob,
-            "y_true": y_true,
-        }
+        results = {"loss": loss, "y_prob": y_prob, "y_true": y_true, "logit": logits}
+        if kwargs.get("embed", False):
+            results["embed"] = patient_emb
+        return results
 
 
 if __name__ == "__main__":
-    from pyhealth.datasets import SampleDataset
+    from pyhealth.datasets import SampleEHRDataset
 
     samples = [
         {
             "patient_id": "patient-0",
             "visit_id": "visit-0",
             # "single_vector": [1, 2, 3],
             "list_codes": ["505800458", "50580045810", "50580045811"],  # NDC
@@ -405,15 +409,15 @@
                 [[1.0, 2.8, 3.3], [4.9, 5.0, 6.6], [7.7, 8.4, 1.3], [7.7, 8.4, 1.3]],
             ],
             "label": 0,
         },
     ]
 
     # dataset
-    dataset = SampleDataset(samples=samples, dataset_name="test")
+    dataset = SampleEHRDataset(samples=samples, dataset_name="test")
 
     # data loader
     from pyhealth.datasets import get_dataloader
 
     train_loader = get_dataloader(dataset, batch_size=2, shuffle=True)
 
     # model
```

### Comparing `pyhealth-1.1.3/pyhealth/models/safedrug.py` & `pyhealth-1.1.4/pyhealth/models/safedrug.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 import rdkit.Chem.BRICS as BRICS
 import torch
 import torch.nn as nn
 from rdkit import Chem
 
-from pyhealth.datasets import SampleDataset
+from pyhealth.datasets import SampleEHRDataset
 from pyhealth.medcode import ATC
 from pyhealth.metrics import ddi_rate_score
 from pyhealth.models import BaseModel
 from pyhealth.models.utils import get_last_visit
 
 
 class MaskLinear(nn.Module):
@@ -305,15 +305,15 @@
         num_layers: the number of layers used in RNN. Default is 1.
         dropout: the dropout rate. Default is 0.5.
         **kwargs: other parameters for the SafeDrug layer.
     """
 
     def __init__(
         self,
-        dataset: SampleDataset,
+        dataset: SampleEHRDataset,
         embedding_dim: int = 128,
         hidden_dim: int = 128,
         num_layers: int = 1,
         dropout: float = 0.5,
         **kwargs,
     ):
         super(SafeDrug, self).__init__(
```

### Comparing `pyhealth-1.1.3/pyhealth/models/transformer.py` & `pyhealth-1.1.4/pyhealth/models/transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
-from typing import List, Optional, Tuple, Dict
+from typing import Dict, List, Optional, Tuple
 
 import torch
 from torch import nn
 
-from pyhealth.datasets import SampleDataset
+from pyhealth.datasets import SampleEHRDataset
 from pyhealth.models import BaseModel
 from pyhealth.tokenizer import Tokenizer
 
 # VALID_OPERATION_LEVEL = ["visit", "event"]
 
 
 class Attention(nn.Module):
@@ -215,15 +215,15 @@
             e.g. ["conditions", "procedures"].
         label_key: key in samples to use as label (e.g., "drugs").
         mode: one of "binary", "multiclass", or "multilabel".
         embedding_dim: the embedding dimension. Default is 128.
         **kwargs: other parameters for the Transformer layer.
 
     Examples:
-        >>> from pyhealth.datasets import SampleDataset
+        >>> from pyhealth.datasets import SampleEHRDataset
         >>> samples = [
         ...         {
         ...             "patient_id": "patient-0",
         ...             "visit_id": "visit-0",
         ...             "list_codes": ["505800458", "50580045810", "50580045811"],  # NDC
         ...             "list_vectors": [[1.0, 2.55, 3.4], [4.1, 5.5, 6.0]],
         ...             "list_list_codes": [["A05B", "A05C", "A06A"], ["A11D", "A11E"]],  # ATC-4
@@ -247,44 +247,50 @@
         ...             "list_list_codes": [["A04A", "B035", "C129"]],
         ...             "list_list_vectors": [
         ...                 [[1.0, 2.8, 3.3], [4.9, 5.0, 6.6], [7.7, 8.4, 1.3], [7.7, 8.4, 1.3]],
         ...             ],
         ...             "label": 0,
         ...         },
         ...     ]
-        >>> dataset = SampleDataset(samples=samples, dataset_name="test")
+        >>> dataset = SampleEHRDataset(samples=samples, dataset_name="test")
         >>>
         >>> from pyhealth.models import Transformer
         >>> model = Transformer(
         ...         dataset=dataset,
         ...         feature_keys=[
         ...             "list_codes",
         ...             "list_vectors",
         ...             "list_list_codes",
         ...             "list_list_vectors",
         ...         ],
         ...         label_key="label",
-        ...         mode="binary",
+        ...         mode="multiclass",
         ...     )
         >>>
         >>> from pyhealth.datasets import get_dataloader
         >>> train_loader = get_dataloader(dataset, batch_size=2, shuffle=True)
         >>> data_batch = next(iter(train_loader))
         >>>
         >>> ret = model(**data_batch)
         >>> print(ret)
-        {'loss': tensor(0.4234, grad_fn=<NllLossBackward0>), 'y_prob': tensor([[9.9998e-01, 2.2920e-05],
-                [5.7120e-01, 4.2880e-01]], grad_fn=<SoftmaxBackward0>), 'y_true': tensor([0, 1])}
+        {
+            'loss': tensor(4.0555, grad_fn=<NllLossBackward0>),
+            'y_prob': tensor([[1.0000e+00, 1.8206e-06],
+                        [9.9970e-01, 3.0020e-04]], grad_fn=<SoftmaxBackward0>),
+            'y_true': tensor([0, 1]),
+            'logit': tensor([[ 7.6283, -5.5881],
+                        [ 1.0898, -7.0210]], grad_fn=<AddmmBackward0>)
+        }
         >>>
 
     """
 
     def __init__(
         self,
-        dataset: SampleDataset,
+        dataset: SampleEHRDataset,
         feature_keys: List[str],
         label_key: str,
         mode: str,
         embedding_dim: int = 128,
         **kwargs
     ):
         super(Transformer, self).__init__(
@@ -364,29 +370,29 @@
                     kwargs[feature_key]
                 )
                 # (patient, event)
                 x = torch.tensor(x, dtype=torch.long, device=self.device)
                 # (patient, event, embedding_dim)
                 x = self.embeddings[feature_key](x)
                 # (patient, event)
-                mask = torch.sum(x, dim=2) != 0
+                mask = torch.any(x !=0, dim=2)
 
             # for case 2: [[code1, code2], [code3, ...], ...]
             elif (dim_ == 3) and (type_ == str):
                 x = self.feat_tokenizers[feature_key].batch_encode_3d(
                     kwargs[feature_key]
                 )
                 # (patient, visit, event)
                 x = torch.tensor(x, dtype=torch.long, device=self.device)
                 # (patient, visit, event, embedding_dim)
                 x = self.embeddings[feature_key](x)
                 # (patient, visit, embedding_dim)
                 x = torch.sum(x, dim=2)
                 # (patient, visit)
-                mask = torch.sum(x, dim=2) != 0
+                mask = torch.any(x !=0, dim=2)
 
             # for case 3: [[1.5, 2.0, 0.0], ...]
             elif (dim_ == 2) and (type_ in [float, int]):
                 x, mask = self.padding2d(kwargs[feature_key])
                 # (patient, event, values)
                 x = torch.tensor(x, dtype=torch.float, device=self.device)
                 # (patient, event, embedding_dim)
@@ -414,23 +420,22 @@
         patient_emb = torch.cat(patient_emb, dim=1)
         # (patient, label_size)
         logits = self.fc(patient_emb)
         # obtain y_true, loss, y_prob
         y_true = self.prepare_labels(kwargs[self.label_key], self.label_tokenizer)
         loss = self.get_loss_function()(logits, y_true)
         y_prob = self.prepare_y_prob(logits)
-        return {
-            "loss": loss,
-            "y_prob": y_prob,
-            "y_true": y_true,
-        }
+        results = {"loss": loss, "y_prob": y_prob, "y_true": y_true, "logit": logits}
+        if kwargs.get("embed", False):
+            results["embed"] = patient_emb
+        return results
 
 
 if __name__ == "__main__":
-    from pyhealth.datasets import SampleDataset
+    from pyhealth.datasets import SampleEHRDataset
 
     samples = [
         {
             "patient_id": "patient-0",
             "visit_id": "visit-0",
             "single_vector": [1, 2, 3],
             "list_codes": ["505800458", "50580045810", "50580045811"],  # NDC
@@ -459,15 +464,15 @@
                 [[1.0, 2.8, 3.3], [4.9, 5.0, 6.6], [7.7, 8.4, 1.3], [7.7, 8.4, 1.3]],
             ],
             "label": 0,
         },
     ]
 
     # dataset
-    dataset = SampleDataset(samples=samples, dataset_name="test")
+    dataset = SampleEHRDataset(samples=samples, dataset_name="test")
 
     # data loader
     from pyhealth.datasets import get_dataloader
 
     train_loader = get_dataloader(dataset, batch_size=2, shuffle=True)
 
     # model
```

### Comparing `pyhealth-1.1.3/pyhealth/models/utils.py` & `pyhealth-1.1.4/pyhealth/models/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,18 @@
     Args:
         hidden_states: [batch size, seq len, hidden_size]
         mask: [batch size, seq len]
 
     Returns:
         last_visit: [batch size, hidden_size]
     """
-    mask = mask.long()
-    last_visit = torch.sum(mask, 1) - 1
-    last_visit = last_visit.unsqueeze(-1)
-    last_visit = last_visit.expand(-1, hidden_states.shape[1] * hidden_states.shape[2])
-    last_visit = torch.reshape(last_visit, hidden_states.shape)
-    last_hidden_states = torch.gather(hidden_states, 1, last_visit)
-    last_hidden_state = last_hidden_states[:, 0, :]
-    return last_hidden_state
+    if mask is None:
+        return hidden_states[:, -1, :]
+    else:
+        mask = mask.long()
+        last_visit = torch.sum(mask, 1) - 1
+        last_visit = last_visit.unsqueeze(-1)
+        last_visit = last_visit.expand(-1, hidden_states.shape[1] * hidden_states.shape[2])
+        last_visit = torch.reshape(last_visit, hidden_states.shape)
+        last_hidden_states = torch.gather(hidden_states, 1, last_visit)
+        last_hidden_state = last_hidden_states[:, 0, :]
+        return last_hidden_state
```

### Comparing `pyhealth-1.1.3/pyhealth/tasks/drug_recommendation.py` & `pyhealth-1.1.4/pyhealth/tasks/drug_recommendation.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,27 +8,42 @@
     history  (e.g., conditions and procedures).
 
     Args:
         patient: a Patient object
 
     Returns:
         samples: a list of samples, each sample is a dict with patient_id, visit_id,
-            and other task-specific attributes as key
+            and other task-specific attributes as key, like this
+            {
+                "patient_id": xxx,
+                "visit_id": xxx,
+                "conditions": [list of diag in visit 1, list of diag in visit 2, ..., list of diag in visit N],
+                "procedures": [list of prod in visit 1, list of prod in visit 2, ..., list of prod in visit N],
+                "drugs_hist": [list of drug in visit 1, list of drug in visit 2, ..., list of drug in visit (N-1)],
+                "drugs": list of drug in visit N, # this is the predicted target
+            }
 
     Examples:
         >>> from pyhealth.datasets import MIMIC3Dataset
         >>> mimic3_base = MIMIC3Dataset(
         ...    root="/srv/local/data/physionet.org/files/mimiciii/1.4",
         ...    tables=["DIAGNOSES_ICD", "PROCEDURES_ICD", "PRESCRIPTIONS"],
         ...    code_mapping={"ICD9CM": "CCSCM"},
         ... )
         >>> from pyhealth.tasks import drug_recommendation_mimic3_fn
         >>> mimic3_sample = mimic3_base.set_task(drug_recommendation_mimic3_fn)
         >>> mimic3_sample.samples[0]
-        [{'visit_id': '130744', 'patient_id': '103', 'conditions': [['42', '109', '19', '122', '98', '663', '58', '51']], 'procedures': [['1']], 'label': [['2', '3', '4']]}]
+        {
+            'visit_id': '174162',
+            'patient_id': '107',
+            'conditions': [['139', '158', '237', '99', '60', '101', '51', '54', '53', '133', '143', '140', '117', '138', '55']],
+            'procedures': [['4443', '4513', '3995']],
+            'drugs_hist': [[]],
+            'drugs': ['0000', '0033', '5817', '0057', '0090', '0053', '0', '0012', '6332', '1001', '6155', '1001', '6332', '0033', '5539', '6332', '5967', '0033', '0040', '5967', '5846', '0016', '5846', '5107', '5551', '6808', '5107', '0090', '5107', '5416', '0033', '1150', '0005', '6365', '0090', '6155', '0005', '0090', '0000', '6373'],
+        }
     """
     samples = []
     for i in range(len(patient)):
         visit: Visit = patient[i]
         conditions = visit.get_code_list(table="DIAGNOSES_ICD")
         procedures = visit.get_code_list(table="PROCEDURES_ICD")
         drugs = visit.get_code_list(table="PRESCRIPTIONS")
@@ -41,36 +56,40 @@
         samples.append(
             {
                 "visit_id": visit.visit_id,
                 "patient_id": patient.patient_id,
                 "conditions": conditions,
                 "procedures": procedures,
                 "drugs": drugs,
-                "drugs_all": drugs,
+                "drugs_hist": drugs,
             }
         )
     # exclude: patients with less than 2 visit
     if len(samples) < 2:
         return []
     # add history
     samples[0]["conditions"] = [samples[0]["conditions"]]
     samples[0]["procedures"] = [samples[0]["procedures"]]
-    samples[0]["drugs_all"] = [samples[0]["drugs_all"]]
+    samples[0]["drugs_hist"] = [samples[0]["drugs_hist"]]
 
     for i in range(1, len(samples)):
         samples[i]["conditions"] = samples[i - 1]["conditions"] + [
             samples[i]["conditions"]
         ]
         samples[i]["procedures"] = samples[i - 1]["procedures"] + [
             samples[i]["procedures"]
         ]
-        samples[i]["drugs_all"] = samples[i - 1]["drugs_all"] + [
-            samples[i]["drugs_all"]
+        samples[i]["drugs_hist"] = samples[i - 1]["drugs_hist"] + [
+            samples[i]["drugs_hist"]
         ]
 
+    # remove the target drug from the history
+    for i in range(len(samples)):
+        samples[i]["drugs_hist"][i] = []
+
     return samples
 
 
 def drug_recommendation_mimic4_fn(patient: Patient):
     """Processes a single patient for the drug recommendation task.
 
     Drug recommendation aims at recommending a set of drugs given the patient health
@@ -78,14 +97,22 @@
 
     Args:
         patient: a Patient object
 
     Returns:
         samples: a list of samples, each sample is a dict with patient_id, visit_id,
             and other task-specific attributes as key
+            {
+                "patient_id": xxx,
+                "visit_id": xxx,
+                "conditions": [list of diag in visit 1, list of diag in visit 2, ..., list of diag in visit N],
+                "procedures": [list of prod in visit 1, list of prod in visit 2, ..., list of prod in visit N],
+                "drugs_hist": [list of drug in visit 1, list of drug in visit 2, ..., list of drug in visit (N-1)],
+                "drugs": list of drug in visit N, # this is the predicted target
+            }
 
     Examples:
         >>> from pyhealth.datasets import MIMIC4Dataset
         >>> mimic4_base = MIMIC4Dataset(
         ...     root="/srv/local/data/physionet.org/files/mimiciv/2.0/hosp",
         ...     tables=["diagnoses_icd", "procedures_icd"],
         ...     code_mapping={"ICD10PROC": "CCSPROC"},
@@ -110,36 +137,40 @@
         samples.append(
             {
                 "visit_id": visit.visit_id,
                 "patient_id": patient.patient_id,
                 "conditions": conditions,
                 "procedures": procedures,
                 "drugs": drugs,
-                "drugs_all": drugs,
+                "drugs_hist": drugs,
             }
         )
     # exclude: patients with less than 2 visit
     if len(samples) < 2:
         return []
     # add history
     samples[0]["conditions"] = [samples[0]["conditions"]]
     samples[0]["procedures"] = [samples[0]["procedures"]]
-    samples[0]["drugs_all"] = [samples[0]["drugs_all"]]
+    samples[0]["drugs_hist"] = [samples[0]["drugs_hist"]]
 
     for i in range(1, len(samples)):
         samples[i]["conditions"] = samples[i - 1]["conditions"] + [
             samples[i]["conditions"]
         ]
         samples[i]["procedures"] = samples[i - 1]["procedures"] + [
             samples[i]["procedures"]
         ]
-        samples[i]["drugs_all"] = samples[i - 1]["drugs_all"] + [
-            samples[i]["drugs_all"]
+        samples[i]["drugs_hist"] = samples[i - 1]["drugs_hist"] + [
+            samples[i]["drugs_hist"]
         ]
 
+    # remove the target drug from the history
+    for i in range(len(samples)):
+        samples[i]["drugs_hist"][i] = []
+
     return samples
 
 
 def drug_recommendation_eicu_fn(patient: Patient):
     """Processes a single patient for the drug recommendation task.
 
     Drug recommendation aims at recommending a set of drugs given the patient health
@@ -272,56 +303,57 @@
             samples[i]["drugs_all"]
         ]
 
     return samples
 
 
 if __name__ == "__main__":
-    from pyhealth.datasets import MIMIC3Dataset
-
-    base_dataset = MIMIC3Dataset(
-        root="/srv/local/data/physionet.org/files/mimiciii/1.4",
-        tables=["DIAGNOSES_ICD", "PROCEDURES_ICD", "PRESCRIPTIONS"],
-        dev=True,
-        code_mapping={"ICD9CM": "CCSCM", "NDC": "ATC"},
-        refresh_cache=False,
-    )
-    sample_dataset = base_dataset.set_task(task_fn=drug_recommendation_mimic3_fn)
-    sample_dataset.stat()
-    print(sample_dataset.available_keys)
+    # from pyhealth.datasets import MIMIC3Dataset
+    # base_dataset = MIMIC3Dataset(
+    #     root="/srv/local/data/physionet.org/files/mimiciii/1.4",
+    #     tables=["DIAGNOSES_ICD", "PROCEDURES_ICD", "PRESCRIPTIONS"],
+    #     dev=True,
+    #     code_mapping={"ICD9CM": "CCSCM"},
+    #     refresh_cache=False,
+    # )
+    # sample_dataset = base_dataset.set_task(task_fn=drug_recommendation_mimic3_fn)
+    # sample_dataset.stat()
+    # print(sample_dataset.available_keys)
+    # print(sample_dataset.samples[0])
 
     from pyhealth.datasets import MIMIC4Dataset
 
     base_dataset = MIMIC4Dataset(
         root="/srv/local/data/physionet.org/files/mimiciv/2.0/hosp",
         tables=["diagnoses_icd", "procedures_icd", "prescriptions"],
         dev=True,
         code_mapping={"NDC": "ATC"},
         refresh_cache=False,
     )
     sample_dataset = base_dataset.set_task(task_fn=drug_recommendation_mimic4_fn)
     sample_dataset.stat()
     print(sample_dataset.available_keys)
+    print(sample_dataset.samples[0])
 
-    from pyhealth.datasets import eICUDataset
+    # from pyhealth.datasets import eICUDataset
 
-    base_dataset = eICUDataset(
-        root="/srv/local/data/physionet.org/files/eicu-crd/2.0",
-        tables=["diagnosis", "medication", "physicalExam"],
-        dev=True,
-        refresh_cache=False,
-    )
-    sample_dataset = base_dataset.set_task(task_fn=drug_recommendation_eicu_fn)
-    sample_dataset.stat()
-    print(sample_dataset.available_keys)
-
-    from pyhealth.datasets import OMOPDataset
-
-    base_dataset = OMOPDataset(
-        root="/srv/local/data/zw12/pyhealth/raw_data/synpuf1k_omop_cdm_5.2.2",
-        tables=["condition_occurrence", "procedure_occurrence", "drug_exposure"],
-        dev=True,
-        refresh_cache=False,
-    )
-    sample_dataset = base_dataset.set_task(task_fn=drug_recommendation_omop_fn)
-    sample_dataset.stat()
-    print(sample_dataset.available_keys)
+    # base_dataset = eICUDataset(
+    #     root="/srv/local/data/physionet.org/files/eicu-crd/2.0",
+    #     tables=["diagnosis", "medication", "physicalExam"],
+    #     dev=True,
+    #     refresh_cache=False,
+    # )
+    # sample_dataset = base_dataset.set_task(task_fn=drug_recommendation_eicu_fn)
+    # sample_dataset.stat()
+    # print(sample_dataset.available_keys)
+
+    # from pyhealth.datasets import OMOPDataset
+
+    # base_dataset = OMOPDataset(
+    #     root="/srv/local/data/zw12/pyhealth/raw_data/synpuf1k_omop_cdm_5.2.2",
+    #     tables=["condition_occurrence", "procedure_occurrence", "drug_exposure"],
+    #     dev=True,
+    #     refresh_cache=False,
+    # )
+    # sample_dataset = base_dataset.set_task(task_fn=drug_recommendation_omop_fn)
+    # sample_dataset.stat()
+    # print(sample_dataset.available_keys)
```

### Comparing `pyhealth-1.1.3/pyhealth/tasks/length_of_stay_prediction.py` & `pyhealth-1.1.4/pyhealth/tasks/length_of_stay_prediction.py`

 * *Files identical despite different names*

### Comparing `pyhealth-1.1.3/pyhealth/tasks/mortality_prediction.py` & `pyhealth-1.1.4/pyhealth/tasks/mortality_prediction.py`

 * *Files 16% similar despite different names*

```diff
@@ -126,28 +126,33 @@
 def mortality_prediction_eicu_fn(patient: Patient):
     """Processes a single patient for the mortality prediction task.
 
     Mortality prediction aims at predicting whether the patient will decease in the
     next hospital visit based on the clinical information from current visit
     (e.g., conditions and procedures).
 
+    Features key-value pairs:
+    - using diagnosis table (ICD9CM and ICD10CM) as condition codes
+    - using physicalExam table as procedure codes
+    - using medication table as drugs codes
+
     Args:
         patient: a Patient object
 
     Returns:
         samples: a list of samples, each sample is a dict with patient_id,
             visit_id, and other task-specific attributes as key
 
     Note that we define the task as a binary classification task.
 
     Examples:
         >>> from pyhealth.datasets import eICUDataset
         >>> eicu_base = eICUDataset(
         ...     root="/srv/local/data/physionet.org/files/eicu-crd/2.0",
-        ...     tables=["diagnosis", "medication"],
+        ...     tables=["diagnosis", "medication", "physicalExam"],
         ...     code_mapping={},
         ...     dev=True
         ... )
         >>> from pyhealth.tasks import mortality_prediction_eicu_fn
         >>> eicu_sample = eicu_base.set_task(mortality_prediction_eicu_fn)
         >>> eicu_sample.samples[0]
         [{'visit_id': '130744', 'patient_id': '103', 'conditions': [['42', '109', '98', '663', '58', '51']], 'procedures': [['1']], 'label': 0}]
@@ -180,14 +185,87 @@
                 "label": mortality_label,
             }
         )
     # no cohort selection
     return samples
 
 
+def mortality_prediction_eicu_fn2(patient: Patient):
+    """Processes a single patient for the mortality prediction task.
+
+    Mortality prediction aims at predicting whether the patient will decease in the
+    next hospital visit based on the clinical information from current visit
+    (e.g., conditions and procedures).
+
+    Similar to mortality_prediction_eicu_fn, but with different code mapping:
+    - using admissionDx table and diagnosisString under diagnosis table as condition codes
+    - using treatment table as procedure codes
+
+    Args:
+        patient: a Patient object
+
+    Returns:
+        samples: a list of samples, each sample is a dict with patient_id,
+            visit_id, and other task-specific attributes as key
+
+    Note that we define the task as a binary classification task.
+
+    Examples:
+        >>> from pyhealth.datasets import eICUDataset
+        >>> eicu_base = eICUDataset(
+        ...     root="/srv/local/data/physionet.org/files/eicu-crd/2.0",
+        ...     tables=["diagnosis", "admissionDx", "treatment"],
+        ...     code_mapping={},
+        ...     dev=True
+        ... )
+        >>> from pyhealth.tasks import mortality_prediction_eicu_fn2
+        >>> eicu_sample = eicu_base.set_task(mortality_prediction_eicu_fn2)
+        >>> eicu_sample.samples[0]
+        {'visit_id': '130744', 'patient_id': '103', 'conditions': [['42', '109', '98', '663', '58', '51']], 'procedures': [['1']], 'label': 0}
+    """
+    samples = []
+    # we will drop the last visit
+    for i in range(len(patient) - 1):
+        visit: Visit = patient[i]
+        next_visit: Visit = patient[i + 1]
+
+        if next_visit.discharge_status not in ["Alive", "Expired"]:
+            mortality_label = 0
+        else:
+            mortality_label = 0 if next_visit.discharge_status == "Alive" else 1
+
+        admissionDx = visit.get_code_list(table="admissionDx")
+        diagnosisString = list(
+            set(
+                [
+                    dx.attr_dict["diagnosisString"]
+                    for dx in visit.get_event_list("diagnosis")
+                ]
+            )
+        )
+        treatment = visit.get_code_list(table="treatment")
+
+        # exclude: visits without treatment, admissionDx, diagnosisString
+        if len(admissionDx) + len(diagnosisString) * len(treatment) == 0:
+            continue
+        # TODO: should also exclude visit with age < 18
+        samples.append(
+            {
+                "visit_id": visit.visit_id,
+                "patient_id": patient.patient_id,
+                "conditions": admissionDx + diagnosisString,
+                "procedures": treatment,
+                "label": mortality_label,
+            }
+        )
+    print(samples)
+    # no cohort selection
+    return samples
+
+
 def mortality_prediction_omop_fn(patient: Patient):
     """Processes a single patient for the mortality prediction task.
 
     Mortality prediction aims at predicting whether the patient will decease in the
     next hospital visit based on the clinical information from current visit
     (e.g., conditions and procedures).
 
@@ -277,14 +355,24 @@
         dev=True,
         refresh_cache=False,
     )
     sample_dataset = base_dataset.set_task(task_fn=mortality_prediction_eicu_fn)
     sample_dataset.stat()
     print(sample_dataset.available_keys)
 
+    base_dataset = eICUDataset(
+        root="/srv/local/data/physionet.org/files/eicu-crd/2.0",
+        tables=["diagnosis", "admissionDx", "treatment"],
+        dev=True,
+        refresh_cache=False,
+    )
+    sample_dataset = base_dataset.set_task(task_fn=mortality_prediction_eicu_fn2)
+    sample_dataset.stat()
+    print(sample_dataset.available_keys)
+
     from pyhealth.datasets import OMOPDataset
 
     base_dataset = OMOPDataset(
         root="/srv/local/data/zw12/pyhealth/raw_data/synpuf1k_omop_cdm_5.2.2",
         tables=["condition_occurrence", "procedure_occurrence", "drug_exposure"],
         dev=True,
         refresh_cache=False,
```

### Comparing `pyhealth-1.1.3/pyhealth/tasks/readmission_prediction.py` & `pyhealth-1.1.4/pyhealth/tasks/readmission_prediction.py`

 * *Files 12% similar despite different names*

```diff
@@ -129,14 +129,19 @@
 def readmission_prediction_eicu_fn(patient: Patient, time_window=5):
     """Processes a single patient for the readmission prediction task.
 
     Readmission prediction aims at predicting whether the patient will be readmitted
     into hospital within time_window days based on the clinical information from
     current visit (e.g., conditions and procedures).
 
+    Features key-value pairs:
+    - using diagnosis table (ICD9CM and ICD10CM) as condition codes
+    - using physicalExam table as procedure codes
+    - using medication table as drugs codes
+
     Args:
         patient: a Patient object
         time_window: the time window threshold (gap < time_window means label=1 for
             the task)
 
     Returns:
         samples: a list of samples, each sample is a dict with patient_id, visit_id,
@@ -144,15 +149,15 @@
 
     Note that we define the task as a binary classification task.
 
     Examples:
         >>> from pyhealth.datasets import eICUDataset
         >>> eicu_base = eICUDataset(
         ...     root="/srv/local/data/physionet.org/files/eicu-crd/2.0",
-        ...     tables=["diagnosis", "medication"],
+        ...     tables=["diagnosis", "medication", "physicalExam"],
         ...     code_mapping={},
         ...     dev=True
         ... )
         >>> from pyhealth.tasks import readmission_prediction_eicu_fn
         >>> eicu_sample = eicu_base.set_task(readmission_prediction_eicu_fn)
         >>> eicu_sample.samples[0]
         [{'visit_id': '130744', 'patient_id': '103', 'conditions': [['42', '109', '98', '663', '58', '51']], 'procedures': [['1']], 'label': 1}]
@@ -183,14 +188,86 @@
                 "label": readmission_label,
             }
         )
     # no cohort selection
     return samples
 
 
+def readmission_prediction_eicu_fn2(patient: Patient, time_window=5):
+    """Processes a single patient for the readmission prediction task.
+
+    Readmission prediction aims at predicting whether the patient will be readmitted
+    into hospital within time_window days based on the clinical information from
+    current visit (e.g., conditions and procedures).
+
+    Similar to readmission_prediction_eicu_fn, but with different code mapping:
+    - using admissionDx table and diagnosisString under diagnosis table as condition codes
+    - using treatment table as procedure codes
+
+    Args:
+        patient: a Patient object
+        time_window: the time window threshold (gap < time_window means label=1 for
+            the task)
+
+    Returns:
+        samples: a list of samples, each sample is a dict with patient_id, visit_id,
+            and other task-specific attributes as key
+
+    Note that we define the task as a binary classification task.
+
+    Examples:
+        >>> from pyhealth.datasets import eICUDataset
+        >>> eicu_base = eICUDataset(
+        ...     root="/srv/local/data/physionet.org/files/eicu-crd/2.0",
+        ...     tables=["diagnosis", "treatment", "admissionDx"],
+        ...     code_mapping={},
+        ...     dev=True
+        ... )
+        >>> from pyhealth.tasks import readmission_prediction_eicu_fn2
+        >>> eicu_sample = eicu_base.set_task(readmission_prediction_eicu_fn2)
+        >>> eicu_sample.samples[0]
+        [{'visit_id': '130744', 'patient_id': '103', 'conditions': [['42', '109', '98', '663', '58', '51']], 'procedures': [['1']], 'label': 1}]
+    """
+    samples = []
+    # we will drop the last visit
+    for i in range(len(patient) - 1):
+        visit: Visit = patient[i]
+        next_visit: Visit = patient[i + 1]
+        # get time difference between current visit and next visit
+        time_diff = (next_visit.encounter_time - visit.encounter_time).days
+        readmission_label = 1 if time_diff < time_window else 0
+
+        admissionDx = visit.get_code_list(table="admissionDx")
+        diagnosisString = list(
+            set(
+                [
+                    dx.attr_dict["diagnosisString"]
+                    for dx in visit.get_event_list("diagnosis")
+                ]
+            )
+        )
+        treatment = visit.get_code_list(table="treatment")
+
+        # exclude: visits without treatment, admissionDx, diagnosisString
+        if len(admissionDx) * len(diagnosisString) * len(treatment) == 0:
+            continue
+        # TODO: should also exclude visit with age < 18
+        samples.append(
+            {
+                "visit_id": visit.visit_id,
+                "patient_id": patient.patient_id,
+                "conditions": admissionDx + diagnosisString,
+                "procedures": treatment,
+                "label": readmission_label,
+            }
+        )
+    # no cohort selection
+    return samples
+
+
 def readmission_prediction_omop_fn(patient: Patient, time_window=15):
     """Processes a single patient for the readmission prediction task.
 
     Readmission prediction aims at predicting whether the patient will be readmitted
     into hospital within time_window days based on the clinical information from
     current visit (e.g., conditions and procedures).
 
@@ -285,14 +362,24 @@
         dev=True,
         refresh_cache=False,
     )
     sample_dataset = base_dataset.set_task(task_fn=readmission_prediction_eicu_fn)
     sample_dataset.stat()
     print(sample_dataset.available_keys)
 
+    base_dataset = eICUDataset(
+        root="/srv/local/data/physionet.org/files/eicu-crd/2.0",
+        tables=["diagnosis", "admissionDx", "treatment"],
+        dev=True,
+        refresh_cache=False,
+    )
+    sample_dataset = base_dataset.set_task(task_fn=readmission_prediction_eicu_fn2)
+    sample_dataset.stat()
+    print(sample_dataset.available_keys)
+
     from pyhealth.datasets import OMOPDataset
 
     base_dataset = OMOPDataset(
         root="/srv/local/data/zw12/pyhealth/raw_data/synpuf1k_omop_cdm_5.2.2",
         tables=["condition_occurrence", "procedure_occurrence", "drug_exposure"],
         dev=True,
         refresh_cache=False,
```

### Comparing `pyhealth-1.1.3/pyhealth/trainer.py` & `pyhealth-1.1.4/pyhealth/trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import logging
 import os
 from datetime import datetime
-from typing import Dict, List, Type, Callable
-from typing import Optional
+from typing import Callable, Dict, List, Optional, Type
 
 import numpy as np
 import torch
 from torch import nn
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 from tqdm.autonotebook import trange
 
-from pyhealth.metrics import (
-    binary_metrics_fn,
-    multiclass_metrics_fn,
-    multilabel_metrics_fn,
-)
+from pyhealth.metrics import (binary_metrics_fn, multiclass_metrics_fn,
+                              multilabel_metrics_fn)
 from pyhealth.utils import create_directory
 
 logger = logging.getLogger(__name__)
 
 
 def is_best(best_score: float, score: float, monitor_criterion: str) -> bool:
     if monitor_criterion == "max":
@@ -230,54 +226,66 @@
                             f"at epoch-{epoch}, step-{global_step}"
                         )
                         best_score = score
                         if self.exp_path is not None:
                             self.save_ckpt(os.path.join(self.exp_path, "best.ckpt"))
 
         # load best model
-        if load_best_model_at_last and self.exp_path is not None:
+        if load_best_model_at_last and self.exp_path is not None and os.path.isfile(os.path.join(self.exp_path, "best.ckpt")):
             logger.info("Loaded best model")
             self.load_ckpt(os.path.join(self.exp_path, "best.ckpt"))
 
         # test
         if test_dataloader is not None:
             scores = self.evaluate(test_dataloader)
             logger.info(f"--- Test ---")
             for key in scores.keys():
                 logger.info("{}: {:.4f}".format(key, scores[key]))
 
         return
 
-    def inference(self, dataloader) -> Dict[str, float]:
+    def inference(self, dataloader, additional_outputs=None) -> Dict[str, float]:
         """Model inference.
 
         Args:
             dataloader: Dataloader for evaluation.
+            additional_outputs: List of additional output to collect.
+                Defaults to None ([]).
 
         Returns:
             y_true_all: List of true labels.
             y_prob_all: List of predicted probabilities.
             loss_mean: Mean loss over batches.
+            additional_outputs (only if requested): Dict of additional results.
         """
         loss_all = []
         y_true_all = []
         y_prob_all = []
+        if additional_outputs is not None:
+            additional_outputs = {k: [] for k in additional_outputs}
         for data in tqdm(dataloader, desc="Evaluation"):
             self.model.eval()
             with torch.no_grad():
                 output = self.model(**data)
                 loss = output["loss"]
                 y_true = output["y_true"].cpu().numpy()
                 y_prob = output["y_prob"].cpu().numpy()
                 loss_all.append(loss.item())
                 y_true_all.append(y_true)
                 y_prob_all.append(y_prob)
+                if additional_outputs is not None:
+                    for key in additional_outputs.keys():
+                        additional_outputs[key].append(output[key].cpu().numpy())
         loss_mean = sum(loss_all) / len(loss_all)
         y_true_all = np.concatenate(y_true_all, axis=0)
         y_prob_all = np.concatenate(y_prob_all, axis=0)
+        if additional_outputs is not None:
+            additional_outputs = {key: np.concatenate(val)
+                                  for key, val in additional_outputs.items()}
+            return y_true_all, y_prob_all, loss_mean, additional_outputs
         return y_true_all, y_prob_all, loss_mean
 
     def evaluate(self, dataloader) -> Dict[str, float]:
         """Evaluates the model.
 
         Args:
             dataloader: Dataloader for evaluation.
@@ -307,14 +315,15 @@
 
 
 if __name__ == "__main__":
     import torch
     import torch.nn as nn
     from torch.utils.data import DataLoader, Dataset
     from torchvision import datasets, transforms
+
     from pyhealth.datasets.utils import collate_fn_dict
 
     class MNISTDataset(Dataset):
         def __init__(self, train=True):
             transform = transforms.Compose(
                 [transforms.ToTensor(), transforms.Normalize((0.1307,), (0.3081,))]
             )
```

### Comparing `pyhealth-1.1.3/pyhealth/utils.py` & `pyhealth-1.1.4/pyhealth/utils.py`

 * *Files identical despite different names*

### Comparing `pyhealth-1.1.3/pyhealth.egg-info/PKG-INFO` & `pyhealth-1.1.4/pyhealth.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyhealth
-Version: 1.1.3
-Summary: A Python library for healthcare AI
+Version: 1.1.4
+Summary: A Deep Learning Python Toolkit for Healthcare Applications
 Home-page: https://github.com/sunlabuiuc/pyhealth
-Author: Chaoqi Yang, Zhenbang Wu, Patrick Jiang
+Author: Chaoqi Yang, Zhenbang Wu, Patrick Jiang, Zhen Lin, Benjamin Danek, Junyi Gao, Jimeng Sun
 Author-email: chaoqiy2@illinois.edu
 Keywords: heathcare AI,healthcare,electronic health records,EHRs,machine learning,data mining,neural networks,deep learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -25,32 +25,37 @@
 
 
 .. image:: https://readthedocs.org/projects/pyhealth/badge/?version=latest
    :target: https://pyhealth.readthedocs.io/en/latest/
    :alt: Documentation status
    
 
-.. image:: https://img.shields.io/github/stars/yzhao062/pyhealth.svg
+.. image:: https://img.shields.io/github/stars/sunlabuiuc/pyhealth.svg
    :target: https://github.com/sunlabuiuc/pyhealth/stargazers
    :alt: GitHub stars
 
 
-.. image:: https://img.shields.io/github/forks/yzhao062/pyhealth.svg?color=blue
+.. image:: https://img.shields.io/github/forks/sunlabuiuc/pyhealth.svg?color=blue
    :target: https://github.com/sunlabuiuc/pyhealth/network
    :alt: GitHub forks
 
 
 .. image:: https://pepy.tech/badge/pyhealth
    :target: https://pepy.tech/project/pyhealth
    :alt: Downloads
 
 
-.. image:: https://pepy.tech/badge/pyhealth/month
-   :target: https://pepy.tech/project/pyhealth
-   :alt: Downloads
+.. image:: https://img.shields.io/badge/Tutorials-Google%20Colab-red
+   :target: https://pyhealth.readthedocs.io/en/latest/tutorials.html
+   :alt: Tutorials
+
+
+.. image:: https://img.shields.io/badge/YouTube-16%20Videos-red
+   :target: https://www.youtube.com/playlist?list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV
+   :alt: YouTube
 
 
 
 .. -----
 
 
 .. **Build Status & Coverage & Maintainability & License**
@@ -71,271 +76,358 @@
 
 
 .. .. image:: https://img.shields.io/github/license/yzhao062/pyhealth
 ..    :target: https://github.com/yzhao062/pyhealth/blob/master/LICENSE
 ..    :alt: License
 
 PyHealth is designed for both **ML researchers and medical practitioners**. We can make your **healthcare AI applications** easier to deploy and more flexible and customizable. `[Tutorials] <https://pyhealth.readthedocs.io/>`_
- 
-**[News!]** We are running the "PyHealth Live" gathering at 8 PM CST every Wednesday night! Welcome to join over `zoom <https://illinois.zoom.us/j/87450975602?pwd=ckQyaHhkRitlUzlwYUY3NjdEQ0pFdz09>`_. Check out `PyHealth Live <https://github.com/sunlabuiuc/PyHealth/blob/master/docs/live.rst>`_ for more information and watch the `Live Videos <https://www.youtube.com/playlist?list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV>`_.
-
-----------
-
-
-1. Introduction
---------------------------
 
-.. .. image:: https://raw.githubusercontent.com/yzhao062/PyHealth/master/docs/images/logo.png
-..    :target: https://raw.githubusercontent.com/yzhao062/PyHealth/master/docs/images/logo.png
-..    :alt: PyHealth Logo
-..    :align: center
+ **[News!]** Our PyHealth is accepted by KDD 2023 Tutorial Track! We will present a 3-hour tutorial on PyHealth at `[KDD 2023] <https://kdd.org/kdd2023/>`_, August 6-10, Long Beach, CA.
 
-PyHealth can support **diverse electronic health records (EHRs)** such as MIMIC and eICU and all OMOP-CDM based databases and provide **various advanced deep learning algorithms** for handling **important healthcare tasks** such as diagnosis-based drug recommendation, patient hospitalization and mortality prediction, and ICU length stay forecasting, etc.  
+.. image:: figure/poster.png
+   :width: 810
 
-*Build a healthcare AI pipeline can be as short as 10 lines of code in PyHealth*.
+..
 
-2. Installation
------------------
+1. Installation :rocket:
+----------------------------
 
 - You could install from PyPi:
 
-.. code-block:: bash
+.. code-block:: sh
 
     pip install pyhealth
 
 - or from github source:
 
-.. code-block:: bash
+.. code-block:: sh
 
-   git clone https://github.com/sunlabuiuc/PyHealth.git
-   cd pyhealth
-   pip install .
+    pip install .
 
-- Required Dependencies
 
-.. code-block:: bash
+2. Introduction :book:
+--------------------------
+``pyhealth`` provides these functionalities (we are still enriching some modules):
 
-    python>=3.8
-    torch>=1.8.0
-    rdkit>=2022.03.4
-    scikit-learn>=0.24.2
-    networkx>=2.6.3
-    pandas>=1.3.2
-    tqdm
+.. image:: figure/overview.png
+   :width: 770
 
+You can use the following functions independently:
 
-3. Modules
---------------------------
+- **Dataset**: ``MIMIC-III``, ``MIMIC-IV``, ``eICU``, ``OMOP-CDM``, ``customized EHR datasets``, etc.
+- **Tasks**: ``diagnosis-based drug recommendation``, ``patient hospitalization and mortality prediction``, ``length stay forecasting``, etc. 
+- **ML models**: ``CNN``, ``LSTM``, ``GRU``, ``LSTM``, ``RETAIN``, ``SafeDrug``, ``Deepr``, etc.
+
+*Building a healthcare AI pipeline can be as short as 10 lines of code in PyHealth*.
+
+
+3. Build ML Pipelines :trophy:
+---------------------------------
 
 All healthcare tasks in our package follow a **five-stage pipeline**: 
 
- load dataset -> define task function -> build ML/DL model -> model training -> inference
+.. image:: figure/five-stage-pipeline.png
+   :width: 640
 
-! We try hard to make sure each stage is as separate as possibe, so that people can customize their own pipeline by only using our data processing steps or the ML models. Each step will call one module and we introduce them using an example.
+..
+
+ We try hard to make sure each stage is as separate as possible, so that people can customize their own pipeline by only using our data processing steps or the ML models.
 
-3.1 An ML Pipeline Example 
-^^^^^^^^^^^^^^^^^^^^^^^^^^
+Module 1: <pyhealth.datasets>
+""""""""""""""""""""""""""""""""""""
 
-* **STEP 1: <pyhealth.datasets>** provides a clean structure for the dataset, independent from the tasks. We support ``MIMIC-III``, ``MIMIC-IV`` and ``eICU``, as well as the standard ``OMOP-formatted data``. The dataset is stored in a unified ``Patient-Visit-Event`` structure.
+``pyhealth.datasets`` provides a clean structure for the dataset, independent from the tasks. We support `MIMIC-III`, `MIMIC-IV` and `eICU`, etc. The output (mimic3base) is a multi-level dictionary structure (see illustration below).
 
 .. code-block:: python
 
     from pyhealth.datasets import MIMIC3Dataset
+
     mimic3base = MIMIC3Dataset(
+        # root directory of the dataset
         root="https://storage.googleapis.com/pyhealth/Synthetic_MIMIC-III/", 
+        # raw CSV table name
         tables=["DIAGNOSES_ICD", "PROCEDURES_ICD", "PRESCRIPTIONS"],
-        # map all NDC codes to ATC 3-rd level codes in these tables
-        code_mapping={"NDC": ("ATC", {"target_kwargs": {"level": 3}})},
+        # map all NDC codes to CCS codes in these tables
+        code_mapping={"NDC": "CCSCM"},
     )
 
-User could also store their own dataset into our ``<pyhealth.datasets.SampleDataset>`` structure and then follow the same pipeline below, see `Tutorial <https://colab.research.google.com/drive/1UurxwAAov1bL_5OO3gQJ4gAa_paeJwJp?usp=sharing>`_
+.. image:: figure/structured-dataset.png
+   :width: 400
 
-* **STEP 2: <pyhealth.tasks>** inputs the ``<pyhealth.datasets>`` object and defines how to process each patient's data into a set of samples for the tasks. In the package, we provide several task examples, such as ``drug recommendation`` and ``length of stay prediction``.
+..
+
+Module 2: <pyhealth.tasks>
+""""""""""""""""""""""""""""""""""""
+
+``pyhealth.tasks`` defines how to process each patient's data into a set of samples for the tasks. In the package, we provide several task examples, such as ``drug recommendation`` and ``length of stay prediction``. **It is easy to customize your own tasks following our** `template <https://colab.research.google.com/drive/1r7MYQR_5yCJGpK_9I9-A10HmpupZuIN-?usp=sharing>`_.
 
 .. code-block:: python
 
-    from pyhealth.tasks import drug_recommendation_mimic3_fn
+    from pyhealth.tasks import readmission_prediction_mimic3_fn
+
+    mimic3sample = mimic3base.set_task(task_fn=readmission_prediction_mimic3_fn) # use default task
+    mimic3sample.samples[0] # show the information of the first sample
+    """
+    {
+        'visit_id': '100183',
+        'patient_id': '175',
+        'conditions': ['5990', '4280', '2851', '4240', '2749', '9982', 'E8499', '42831', '34600'],
+        'procedures': ['0040', '3931', '7769'],
+        'drugs': ['N06DA02', 'V06DC01', 'B01AB01', 'A06AA02', 'R03AC02', 'H03AA01', 'J01FA09'],
+        'label': 0
+    }
+    """
+
     from pyhealth.datasets import split_by_patient, get_dataloader
 
-    mimic3sample = mimic3base.set_task(task_fn=drug_recommendation_mimic3_fn) # use default task
     train_ds, val_ds, test_ds = split_by_patient(mimic3sample, [0.8, 0.1, 0.1])
-
-    # create dataloaders (torch.data.DataLoader)
     train_loader = get_dataloader(train_ds, batch_size=32, shuffle=True)
     val_loader = get_dataloader(val_ds, batch_size=32, shuffle=False)
     test_loader = get_dataloader(test_ds, batch_size=32, shuffle=False)
 
-* **STEP 3: <pyhealth.models>** provides the healthcare ML models using ``<pyhealth.models>``. This module also provides model layers, such as ``pyhealth.models.RETAINLayer`` for building customized ML architectures. Our model layers can used as easily as ``torch.nn.Linear``.
+Module 3: <pyhealth.models>
+""""""""""""""""""""""""""""""""""""
+
+``pyhealth.models`` provides different ML models with very similar argument configs.
 
 .. code-block:: python
 
     from pyhealth.models import Transformer
 
     model = Transformer(
         dataset=mimic3sample,
-        feature_keys=["conditions", "procedures"],
-        label_key="drugs",
-        mode="multilabel",
+        feature_keys=["conditions", "procedures", "drug"],
+        label_key="label",
+        mode="binary",
     )
 
-* **STEP 4: <pyhealth.trainer>** is the training manager with ``train_loader``, the ``val_loader``, ``val_metric``, and specify other arguemnts, such as epochs, optimizer, learning rate, etc. The trainer will automatically save the best model and output the path in the end.
+Module 4: <pyhealth.trainer>
+""""""""""""""""""""""""""""""""""""
+
+``pyhealth.trainer`` can specify training arguments, such as epochs, optimizer, learning rate, etc. The trainer will automatically save the best model and output the path in the end.
 
 .. code-block:: python
     
     from pyhealth.trainer import Trainer
 
     trainer = Trainer(model=model)
     trainer.train(
         train_dataloader=train_loader,
         val_dataloader=val_loader,
         epochs=50,
         monitor="pr_auc_samples",
     )
 
-* **STEP 5: <pyhealth.metrics>** provides several **common evaluation metrics** (refer to `Doc <https://pyhealth.readthedocs.io/en/latest/api/metrics.html>`_ and see what are available) and **special metrics** in healthcare, such as drug-drug interaction (DDI) rate.
+Module 5: <pyhealth.metrics>
+""""""""""""""""""""""""""""""""""""
+
+``pyhealth.metrics`` provides several **common evaluation metrics** (refer to `Doc <https://pyhealth.readthedocs.io/en/latest/api/metrics.html>`_ and see what are available).
 
 .. code-block:: python
-    
+
+    # method 1
     trainer.evaluate(test_loader)
+    
+    # method 2
+    from pyhealth.metrics.binary import binary_metrics_fn
 
-3.2 Medical Code Map
-^^^^^^^^^^^^^^^^^^^^^^^^^^
+    y_true, y_prob, loss = trainer.inference(test_loader)
+    binary_metrics_fn(y_true, y_prob, metrics=["pr_auc", "roc_auc"])
 
-* **<pyhealth.codemap>** provides two core functionalities: (i) looking up information for a given medical code (e.g., name, category, sub-concept); (ii) mapping codes across coding systems (e.g., ICD9CM to CCSCM). **This module can be independently applied to your research.**
+4. Medical Code Map :hospital: 
+---------------------------------
 
-* For code mapping between two coding systems
+``pyhealth.codemap`` provides two core functionalities. **This module can be used independently.**
 
-.. code-block:: python
+* For code ontology lookup within one medical coding system (e.g., name, category, sub-concept); 
 
-    from pyhealth.medcode import CrossMap
+.. code-block:: python
 
-    codemap = CrossMap.load("ICD9CM", "CCSCM")
-    codemap.map("82101") # use it like a dict
+    from pyhealth.medcode import InnerMap
 
-    codemap = CrossMap.load("NDC", "ATC")
-    codemap.map("00527051210")
+    icd9cm = InnerMap.load("ICD9CM")
+    icd9cm.lookup("428.0")
+    # `Congestive heart failure, unspecified`
+    icd9cm.get_ancestors("428.0")
+    # ['428', '420-429.99', '390-459.99', '001-999.99']
+    
+    atc = InnerMap.load("ATC")
+    atc.lookup("M01AE51")
+    # `ibuprofen, combinations`
+    atc.lookup("M01AE51", "drugbank_id")
+    # `DB01050`
+    atc.lookup("M01AE51", "description")
+    # Ibuprofen is a non-steroidal anti-inflammatory drug (NSAID) derived ...
+    atc.lookup("M01AE51", "indication")
+    # Ibuprofen is the most commonly used and prescribed NSAID. It is very common over the ...
 
-* For code ontology lookup within one system
+* For code mapping between two coding systems (e.g., ICD9CM to CCSCM). 
 
 .. code-block:: python
 
-    from pyhealth.medcode import InnerMap
+    from pyhealth.medcode import CrossMap
 
-    icd9cm = InnerMap.load("ICD9CM")
-    icd9cm.lookup("428.0") # get detailed info
-    icd9cm.get_ancestors("428.0") # get parents
+    codemap = CrossMap.load("ICD9CM", "CCSCM")
+    codemap.map("428.0")
+    # ['108']
+
+    codemap = CrossMap.load("NDC", "RxNorm")
+    codemap.map("50580049698")
+    # ['209387']
+
+    codemap = CrossMap.load("NDC", "ATC")
+    codemap.map("50090539100")
+    # ['A10AC04', 'A10AD04', 'A10AB04']
 
-3.3 Medical Code Tokenizer
-^^^^^^^^^^^^^^^^^^^^^^^^^^
+5. Medical Code Tokenizer :speech_balloon:
+---------------------------------------------
 
-* **<pyhealth.tokenizer>** is used for transformations between string-based tokens and integer-based indices, based on the overall token space. We provide flexible functions to tokenize 1D, 2D and 3D lists. **This module can be independently applied to your research.**
+``pyhealth.tokenizer`` is used for transformations between string-based tokens and integer-based indices, based on the overall token space. We provide flexible functions to tokenize 1D, 2D and 3D lists. **This module can be used independently.**
 
 .. code-block:: python
 
     from pyhealth.tokenizer import Tokenizer
 
     # Example: we use a list of ATC3 code as the token
     token_space = ['A01A', 'A02A', 'A02B', 'A02X', 'A03A', 'A03B', 'A03C', 'A03D', \
             'A03F', 'A04A', 'A05A', 'A05B', 'A05C', 'A06A', 'A07A', 'A07B', 'A07C', \
             'A12B', 'A12C', 'A13A', 'A14A', 'A14B', 'A16A']
     tokenizer = Tokenizer(tokens=token_space, special_tokens=["<pad>", "<unk>"])
 
     # 2d encode 
     tokens = [['A03C', 'A03D', 'A03E', 'A03F'], ['A04A', 'B035', 'C129']]
-    indices = tokenizer.batch_encode_2d(tokens) # [[8, 9, 10, 11], [12, 1, 1, 0]]
+    indices = tokenizer.batch_encode_2d(tokens) 
+    # [[8, 9, 10, 11], [12, 1, 1, 0]]
 
     # 2d decode 
     indices = [[8, 9, 10, 11], [12, 1, 1, 0]]
-    tokens = tokenizer.batch_decode_2d(indices) # [['A03C', 'A03D', 'A03E', 'A03F'], ['A04A', '<unk>', '<unk>']]
+    tokens = tokenizer.batch_decode_2d(indices)
+    # [['A03C', 'A03D', 'A03E', 'A03F'], ['A04A', '<unk>', '<unk>']]
 
+    # 3d encode
+    tokens = [[['A03C', 'A03D', 'A03E', 'A03F'], ['A08A', 'A09A']], \
+        [['A04A', 'B035', 'C129']]]
+    indices = tokenizer.batch_encode_3d(tokens)
+    # [[[8, 9, 10, 11], [24, 25, 0, 0]], [[12, 1, 1, 0], [0, 0, 0, 0]]]
+
+    # 3d decode
+    indices = [[[8, 9, 10, 11], [24, 25, 0, 0]], \
+        [[12, 1, 1, 0], [0, 0, 0, 0]]]
+    tokens = tokenizer.batch_decode_3d(indices)
+    # [[['A03C', 'A03D', 'A03E', 'A03F'], ['A08A', 'A09A']], [['A04A', '<unk>', '<unk>']]]
 ..
 
-4. Tutorials
-------------
+6. Tutorials :teacher:
+----------------------------
 
- We provide the following tutorials to help users get started with our pyhealth.
+.. image:: https://colab.research.google.com/assets/colab-badge.svg
+    :target: https://pyhealth.readthedocs.io/en/latest/tutorials.html
 
+..
 
-`Tutorial 0: Introduction to pyhealth.data <https://colab.research.google.com/drive/1y9PawgSbyMbSSMw1dpfwtooH7qzOEYdN?usp=sharing>`_ 
+ We provide the following tutorials to help users get started with our pyhealth. 
 
-`Tutorial 1: Introduction to pyhealth.datasets <https://colab.research.google.com/drive/18kbzEQAj1FMs_J9rTGX8eCoxnWdx4Ltn?usp=sharing>`_ 
+`Tutorial 0: Introduction to pyhealth.data <https://colab.research.google.com/drive/1y9PawgSbyMbSSMw1dpfwtooH7qzOEYdN?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=Nk1itBoLOX8&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=2>`__  
 
-`Tutorial 2: Introduction to pyhealth.tasks <https://colab.research.google.com/drive/1r7MYQR_5yCJGpK_9I9-A10HmpupZuIN-?usp=sharing>`_ 
+`Tutorial 1: Introduction to pyhealth.datasets <https://colab.research.google.com/drive/18kbzEQAj1FMs_J9rTGX8eCoxnWdx4Ltn?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=c1InKqFJbsI&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=3>`__  
 
-`Tutorial 3: Introduction to pyhealth.models <https://colab.research.google.com/drive/1LcXZlu7ZUuqepf269X3FhXuhHeRvaJX5?usp=sharing>`_ 
+`Tutorial 2: Introduction to pyhealth.tasks <https://colab.research.google.com/drive/1r7MYQR_5yCJGpK_9I9-A10HmpupZuIN-?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=CxESe1gYWU4&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=4>`__  
 
-`Tutorial 4: Introduction to pyhealth.trainer <https://colab.research.google.com/drive/1L1Nz76cRNB7wTp5Pz_4Vp4N2eRZ9R6xl?usp=sharing>`_ 
+`Tutorial 3: Introduction to pyhealth.models <https://colab.research.google.com/drive/1LcXZlu7ZUuqepf269X3FhXuhHeRvaJX5?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=fRc0ncbTgZA&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=6>`__  
 
-`Tutorial 5: Introduction to pyhealth.metrics <https://colab.research.google.com/drive/1Mrs77EJ92HwMgDaElJ_CBXbi4iABZBeo?usp=sharing>`_ 
+`Tutorial 4: Introduction to pyhealth.trainer <https://colab.research.google.com/drive/1L1Nz76cRNB7wTp5Pz_4Vp4N2eRZ9R6xl?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=5Hyw3of5pO4&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=7>`__  
 
-`Tutorial 6: Introduction to pyhealth.tokenizer <https://colab.research.google.com/drive/1bDOb0A5g0umBjtz8NIp4wqye7taJ03D0?usp=sharing>`_
+`Tutorial 5: Introduction to pyhealth.metrics <https://colab.research.google.com/drive/1Mrs77EJ92HwMgDaElJ_CBXbi4iABZBeo?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=d-Kx_xCwre4&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=8>`__ 
 
-`Tutorial 7: Introduction to pyhealth.medcode <https://colab.research.google.com/drive/1xrp_ACM2_Hg5Wxzj0SKKKgZfMY0WwEj3?usp=sharing>`_
 
- The following tutorials will help users build their own task pipelines.
+`Tutorial 6: Introduction to pyhealth.tokenizer <https://colab.research.google.com/drive/1bDOb0A5g0umBjtz8NIp4wqye7taJ03D0?usp=sharing>`_ `[Video] <https://www.youtube.com/watch?v=CeXJtf0lfs0&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=10>`__ 
 
-`Pipeline 1: Drug Recommendation <https://colab.research.google.com/drive/10CSb4F4llYJvv42yTUiRmvSZdoEsbmFF?usp=sharing>`_ 
 
-`Pipeline 2: Length of Stay Prediction <https://colab.research.google.com/drive/1JoPpXqqB1_lGF1XscBOsDHMLtgvlOYI1?usp=sharing>`_ 
+`Tutorial 7: Introduction to pyhealth.medcode <https://colab.research.google.com/drive/1xrp_ACM2_Hg5Wxzj0SKKKgZfMY0WwEj3?usp=sharing>`_ `[Video] <https://www.youtube.com/watch?v=MmmfU6_xkYg&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=9>`__  
 
-`Pipeline 3: Readmission Prediction <https://colab.research.google.com/drive/1bhCwbXce1YFtVaQLsOt4FcyZJ1_my7Cs?usp=sharing>`_ 
 
-`Pipeline 4: Mortality Prediction <https://colab.research.google.com/drive/1Qblpcv4NWjrnADT66TjBcNwOe8x6wU4c?usp=sharing>`_ 
+ The following tutorials will help users build their own task pipelines.
 
- The following tutorials will help users to explore advanced features of pyhealth.
+`Pipeline 1: Drug Recommendation <https://colab.research.google.com/drive/10CSb4F4llYJvv42yTUiRmvSZdoEsbmFF?usp=sharing>`_ `[Video] <https://
+www.youtube.com/watch?v=GGP3Dhfyisc&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=12>`__  
 
-`Advanced Tutorial 1: Fit your dataset into our pipeline <https://colab.research.google.com/drive/1UurxwAAov1bL_5OO3gQJ4gAa_paeJwJp?usp=sharing>`_
+`Pipeline 2: Length of Stay Prediction <https://colab.research.google.com/drive/1JoPpXqqB1_lGF1XscBOsDHMLtgvlOYI1?usp=sharing>`_ `[Video] <https://
+www.youtube.com/watch?v=GGP3Dhfyisc&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=12>`__  
 
-`Advanced Tutorial 2: Define your own healthcare task <https://colab.research.google.com/drive/1gK6zPXvfFGBM1uNaLP32BOKrnnJdqRq2?usp=sharing>`_ 
+`Pipeline 3: Readmission Prediction <https://colab.research.google.com/drive/1bhCwbXce1YFtVaQLsOt4FcyZJ1_my7Cs?usp=sharing>`_ `[Video] <https://
+www.youtube.com/watch?v=GGP3Dhfyisc&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=12>`__  
 
-`Advanced Tutorial 3: Adopt customized model into pyhealth <https://colab.research.google.com/drive/1F_NJ90GC8_Eq-vKTf7Tyziew4gWjjKoH?usp=sharing>`_ 
+`Pipeline 4: Mortality Prediction <https://colab.research.google.com/drive/1Qblpcv4NWjrnADT66TjBcNwOe8x6wU4c?usp=sharing>`_ `[Video] <https://
+www.youtube.com/watch?v=GGP3Dhfyisc&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=12>`__ 
 
-`Advanced Tutorial 4: Load your own processed data into pyhealth and try out our ML models <https://colab.research.google.com/drive/1ZRnKch2EyJLrI3G5AvDXVpeE2wwgBWfw?usp=sharing>`_
+`Pipeline 5: Sleep Staging <https://colab.research.google.com/drive/1mpSeNCAthXG3cqROkdUcUdozIPIMTCuo?usp=sharing>`_ `[Video] <https://www.youtube.com/watch?v=ySAIU-rO6so&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=16>`__  
 
 
+ We provided the advanced tutorials for supporting various needs. 
 
-----
+`Advanced Tutorial 1: Fit your dataset into our pipeline <https://colab.research.google.com/drive/1UurxwAAov1bL_5OO3gQJ4gAa_paeJwJp?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=xw2hGLEQ4Y0&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=13>`__ 
 
+`Advanced Tutorial 2: Define your own healthcare task <https://colab.research.google.com/drive/1gK6zPXvfFGBM1uNaLP32BOKrnnJdqRq2?usp=sharing>`_ 
 
-5. Datasets
---------------------------
+`Advanced Tutorial 3: Adopt customized model into pyhealth <https://colab.research.google.com/drive/1F_NJ90GC8_Eq-vKTf7Tyziew4gWjjKoH?usp=sharing>`_  `[Video] <https://www.youtube.com/watch?v=lADFlcmLtdE&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=14>`__ 
+
+`Advanced Tutorial 4: Load your own processed data into pyhealth and try out our ML models <https://colab.research.google.com/drive/1ZRnKch2EyJLrI3G5AvDXVpeE2wwgBWfw?usp=sharing>`_ `[Video] <https://www.youtube.com/watch?v=xw2hGLEQ4Y0&list=PLR3CNIF8DDHJUl8RLhyOVpX_kT4bxulEV&index=13>`__ 
+
+
+7. Datasets :mountain_snow:
+-----------------------------
 We provide the processing files for the following open EHR datasets:
 
 ===================  =======================================  ========================================  ======================================================================================================== 
 Dataset              Module                                   Year                                      Information                                                             
 ===================  =======================================  ========================================  ========================================================================================================
-MIMIC-III            ``pyhealth.datasets.MIMIC3BaseDataset``  2016                                      `MIMIC-III Clinical Database <https://physionet.org/content/mimiciii/1.4//>`_    
-MIMIC-IV             ``pyhealth.datasets.MIMIC4BaseDataset``  2020                                      `MIMIC-IV Clinical Database <https://physionet.org/content/mimiciv/0.4/>`_  
-eICU                 ``pyhealth.datasets.eICUBaseDataset``    2018                                      `eICU Collaborative Research Database <https://eicu-crd.mit.edu//>`_                 
-OMOP                 ``pyhealth.datasets.OMOPBaseDataset``                                              `OMOP-CDM schema based dataset <https://www.ohdsi.org/data-standardization/the-common-data-model/>`_                                    
+MIMIC-III            ``pyhealth.datasets.MIMIC3Dataset``      2016                                      `MIMIC-III Clinical Database <https://physionet.org/content/mimiciii/1.4//>`_    
+MIMIC-IV             ``pyhealth.datasets.MIMIC4Dataset``      2020                                      `MIMIC-IV Clinical Database <https://physionet.org/content/mimiciv/0.4/>`_  
+eICU                 ``pyhealth.datasets.eICUDataset``        2018                                      `eICU Collaborative Research Database <https://eicu-crd.mit.edu//>`_                 
+OMOP                 ``pyhealth.datasets.OMOPDataset``                                                  `OMOP-CDM schema based dataset <https://www.ohdsi.org/data-standardization/the-common-data-model/>`_    
+SleepEDF             ``pyhealth.datasets.SleepEDFDataset``    2018                                      `Sleep-EDF dataset <https://physionet.org/content/sleep-edfx/1.0.0/>`_
+SHHS                 ``pyhealth.datasets.SHHSDataset``        2016                                      `Sleep Heart Health Study dataset <https://sleepdata.org/datasets/shhs>`_   
+ISRUC                ``pyhealth.datasets.ISRUCDataset``       2016                                      `ISRUC-SLEEP dataset <https://sleeptight.isr.uc.pt/?page_id=48>`_                               
 ===================  =======================================  ========================================  ========================================================================================================
 
 
-6. Machine/Deep Learning Models and Benchmarks
-------------------------------------------------
+8. Machine/Deep Learning Models and Benchmarks :airplane:
+------------------------------------------------------------
 
-==================================    ================  =================================  ======  ===========================================================================================================================================
-Model Name                            Type              Module                             Year    Reference
-==================================    ================  =================================  ======  ===========================================================================================================================================
-Convolutional Neural Network (CNN)    deep learning     ``pyhealth.models.CNN``            1989    `Handwritten Digit Recognition with a Back-Propagation Network <https://proceedings.neurips.cc/paper/1989/file/53c3bce66e43be4f209556518c2fcb54-Paper.pdf>`_
-Recurrent Neural Nets (RNN)           deep Learning     ``pyhealth.models.RNN``            2011    `Recurrent neural network based language model <http://www.fit.vutbr.cz/research/groups/speech/servite/2010/rnnlm_mikolov.pdf>`_
-Transformer                           deep Learning     ``pyhealth.models.Transformer``    2017    `Atention is All you Need <https://arxiv.org/abs/1706.03762>`_
-RETAIN                                deep Learning     ``pyhealth.models.RETAIN``         2016    `RETAIN: An Interpretable Predictive Model for Healthcare using Reverse Time Attention Mechanism <https://arxiv.org/abs/1608.05745>`_
-GAMENet                               deep Learning     ``pyhealth.models.GAMENet``        2019    `GAMENet: Graph Attention Mechanism for Explainable Electronic Health Record Prediction <https://arxiv.org/abs/1809.01852>`_
-MICRON                                deep Learning     ``pyhealth.models.MICRON``         2021    `Change Matters: Medication Change Prediction with Recurrent Residual Networks <https://www.ijcai.org/proceedings/2021/0513>`_
-SafeDrug                              deep Learning     ``pyhealth.models.SafeDrug``       2021    `SafeDrug: Dual Molecular Graph Encoders for Recommending Effective and Safe Drug Combinations <https://arxiv.org/abs/2105.02711>`_
-==================================    ================  =================================  ======  ===========================================================================================================================================
+==================================    ================  =================================  ======  ============================================================================================================================================================================  =======================================================================================================================================================================================
+Model Name                            Type              Module                             Year    Summary                                                                                                                                                                       Reference
+==================================    ================  =================================  ======  ============================================================================================================================================================================  =======================================================================================================================================================================================
+Multi-layer Perceptron                deep learning     ``pyhealth.models.MLP``            1986    MLP treats each feature as static                                                                                                                                             `Backpropagation: theory, architectures, and applications <https://www.taylorfrancis.com/books/mono/10.4324/9780203763247/backpropagation-yves-chauvin-david-rumelhart>`_
+Convolutional Neural Network (CNN)    deep learning     ``pyhealth.models.CNN``            1989    CNN runs on the conceptual patient-by-visit grids                                                                                                                             `Handwritten Digit Recognition with a Back-Propagation Network <https://proceedings.neurips.cc/paper/1989/file/53c3bce66e43be4f209556518c2fcb54-Paper.pdf>`_
+Recurrent Neural Nets (RNN)           deep Learning     ``pyhealth.models.RNN``            2011    RNN (includes LSTM and GRU) can run on any sequential level (e.g., visit by visit sequences)                                                                                  `Recurrent neural network based language model <http://www.fit.vutbr.cz/research/groups/speech/servite/2010/rnnlm_mikolov.pdf>`_
+Transformer                           deep Learning     ``pyhealth.models.Transformer``    2017    Transformer can run on any sequential level (e.g., visit by visit sequences)                                                                                                  `Atention is All you Need <https://arxiv.org/abs/1706.03762>`_
+RETAIN                                deep Learning     ``pyhealth.models.RETAIN``         2016    RETAIN uses two RNN to learn patient embeddings while providing feature-level and visit-level importance.                                                                     `RETAIN: An Interpretable Predictive Model for Healthcare using Reverse Time Attention Mechanism <https://arxiv.org/abs/1608.05745>`_
+GAMENet                               deep Learning     ``pyhealth.models.GAMENet``        2019    GAMENet uses memory networks, used only for drug recommendation task                                                                                                          `GAMENet: Graph Attention Mechanism for Explainable Electronic Health Record Prediction <https://arxiv.org/abs/1809.01852>`_
+MICRON                                deep Learning     ``pyhealth.models.MICRON``         2021    MICRON predicts the future drug combination by instead predicting the changes w.r.t. the current combination, used only for drug recommendation task                          `Change Matters: Medication Change Prediction with Recurrent Residual Networks <https://www.ijcai.org/proceedings/2021/0513>`_
+SafeDrug                              deep Learning     ``pyhealth.models.SafeDrug``       2021    SafeDrug encodes drug molecule structures by graph neural networks, used only for drug recommendation task                                                                    `SafeDrug: Dual Molecular Graph Encoders for Recommending Effective and Safe Drug Combinations <https://arxiv.org/abs/2105.02711>`_
+MoleRec                               deep Learning     ``pyhealth.models.MoleRec``        2023    MoleRec encodes drug molecule in a substructure level as well as the patient's information into a drug combination representation, used only for drug recommendation task     `MoleRec: Combinatorial Drug Recommendation with Substructure-Aware Molecular Representation Learning <https://dl.acm.org/doi/10.1145/3543507.3583872>`_
+Deepr                                 deep Learning     ``pyhealth.models.Deepr``          2017    Deepr is based on 1D CNN. General purpose.                                                                                                                                    `Deepr : A Convolutional Net for Medical Records <https://arxiv.org/abs/1607.07519>`_
+ContraWR Encoder (STFT+CNN)           deep Learning     ``pyhealth.models.ContraWR``       2021    ContraWR encoder uses short time Fourier transform (STFT) + 2D CNN, used for biosignal learning                                                                               `Self-supervised EEG Representation Learning for Automatic Sleep Staging <https://arxiv.org/abs/2110.15278>`_
+SparcNet (1D CNN)                     deep Learning     ``pyhealth.models.SparcNet``       2023    SparcNet is based on 1D CNN, used for biosignal learning                                                                                                                      `Development of Expert-level Classification of Seizures and Rhythmic and Periodic Patterns During EEG Interpretation <#>`_
+TCN                                   deep learning     ``pyhealth.models.TCN``            2018    TCN is based on dilated 1D CNN. General purpose                                                                                                                               `Temporal Convolutional Networks <https://arxiv.org/abs/1803.01271>`_
+AdaCare                               deep learning     ``pyhealth.models.AdaCare``        2020    AdaCare uses CNNs with dilated filters to learn enriched patient embedding. It uses feature calibration module to provide the feature-level and visit-level interpretability  `AdaCare: Explainable Clinical Health Status Representation Learning via Scale-Adaptive Feature Extraction and Recalibration <https://arxiv.org/abs/1911.12205>`_
+ConCare                               deep learning     ``pyhealth.models.ConCare``        2020    ConCare uses transformers to learn patient embedding and calculate inter-feature correlations.                                                                                `ConCare: Personalized Clinical Feature Embedding via Capturing the Healthcare Context <https://arxiv.org/abs/1911.12216>`_
+StageNet                              deep learning     ``pyhealth.models.StageNet``       2020    StageNet uses stage-aware LSTM to conduct clinical predictive tasks while learning patient disease progression stage change unsupervisedly                                    `StageNet: Stage-Aware Neural Networks for Health Risk Prediction <https://arxiv.org/abs/2001.10054>`_
+Dr. Agent                             deep learning     ``pyhealth.models.Agent``          2020    Dr. Agent uses two reinforcement learning agents to learn patient embeddings by mimicking clinical second opinions                                                            `Dr. Agent: Clinical predictive model via mimicked second opinions <https://academic.oup.com/jamia/article/27/7/1084/5858308>`_
+GRASP                                 deep learning     ``pyhealth.models.GRASP``          2021    GRASP uses graph neural network to identify latent patient clusters and uses the clustering information to learn patient                                                      `GRASP: Generic Framework for Health Status Representation Learning Based on Incorporating Knowledge from Similar Patients <https://ojs.aaai.org/index.php/AAAI/article/view/16152>`_
+==================================    ================  =================================  ======  ============================================================================================================================================================================  =======================================================================================================================================================================================
 
 * Check the `interactive map on benchmark EHR predictive tasks <https://pyhealth.readthedocs.io/en/latest/index.html#benchmark-on-healthcare-tasks>`_.
 
-7. Citing PyHealth
+9. Citing PyHealth :handshake:
 ----------------------------------
 
 .. code-block:: bibtex
 
-    @software{pyhealth2022github,
-        author = {Chaoqi Yang and Zhenbang Wu and Patrick Jiang and Jimeng Sun},
+    @inproceedings{pyhealth2023yang,
+        author = {Yang, Chaoqi and Wu, Zhenbang and Jiang, Patrick and Lin, Zhen and Gao, Junyi and Danek, Benjamin and Sun, Jimeng},
         title = {{PyHealth}: A Deep Learning Toolkit for Healthcare Predictive Modeling},
         url = {https://github.com/sunlabuiuc/PyHealth},
-        year = {2022},
+        booktitle = {Proceedings of the 27th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD) 2023},
+        year = {2023}
     }
```

### Comparing `pyhealth-1.1.3/setup.py` & `pyhealth-1.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,23 +18,23 @@
         return f.read()
 
 
 # read the contents of requirements.txt
 with open(path.join(this_directory, "requirements.txt"), encoding="utf-8") as f:
     requirements = f.read().splitlines()
 
-VERSION = "1.1.3"
+VERSION = "1.1.4"
 
 setup(
     name="pyhealth",
     version=VERSION,
-    description="A Python library for healthcare AI",
+    description="A Deep Learning Python Toolkit for Healthcare Applications",
     long_description=readme(),
     long_description_content_type="text/x-rst",
-    author="Chaoqi Yang, Zhenbang Wu, Patrick Jiang",
+    author="Chaoqi Yang, Zhenbang Wu, Patrick Jiang, Zhen Lin, Benjamin Danek, Junyi Gao, Jimeng Sun",
     author_email="chaoqiy2@illinois.edu",
     url="https://github.com/sunlabuiuc/pyhealth",
     keywords=[
         "heathcare AI",
         "healthcare",
         "electronic health records",
         "EHRs",
```

