# Comparing `tmp/sleepecg-0.5.4.tar.gz` & `tmp/sleepecg-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepecg-0.5.4.tar", last modified: Thu Apr 13 05:51:12 2023, max compression
+gzip compressed data, was "sleepecg-0.5.5.tar", last modified: Thu Jun  1 08:48:02 2023, max compression
```

## Comparing `sleepecg-0.5.4.tar` & `sleepecg-0.5.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.763930 sleepecg-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.751929 sleepecg-0.5.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.755930 sleepecg-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-13 05:51:04.000000 sleepecg-0.5.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-13 05:51:04.000000 sleepecg-0.5.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-13 05:51:04.000000 sleepecg-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-13 05:51:04.000000 sleepecg-0.5.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-04-13 05:51:04.000000 sleepecg-0.5.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-13 05:51:04.000000 sleepecg-0.5.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-13 05:51:04.000000 sleepecg-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 05:51:04.000000 sleepecg-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-13 05:51:12.763930 sleepecg-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-13 05:51:04.000000 sleepecg-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.755930 sleepecg-0.5.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.755930 sleepecg-0.5.4/examples/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/benchmark/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/benchmark/benchmark_detectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/benchmark/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/benchmark/plot_benchmark_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/benchmark/requirements-benchmark.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/benchmark/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.755930 sleepecg-0.5.4/examples/classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/classifiers/wrn_gru_mesa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/classifiers/wrn_gru_mesa_weighted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/classifiers/ws_gru_mesa.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/heartbeat_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/try_ws_gru_mesa.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-13 05:51:04.000000 sleepecg-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-13 05:51:04.000000 sleepecg-0.5.4/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-13 05:51:12.763930 sleepecg-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 05:51:04.000000 sleepecg-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.755930 sleepecg-0.5.4/sleepecg/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/_heartbeat_detection.c
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/_heartbeat_detection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18850 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.759930 sleepecg-0.5.4/sleepecg/classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)   775585 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/classifiers/wrn-gru-mesa-weighted.zip
--rw-r--r--   0 runner    (1001) docker     (123)   764383 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/classifiers/wrn-gru-mesa.zip
--rw-r--r--   0 runner    (1001) docker     (123)   775057 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/classifiers/ws-gru-mesa.zip
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    26627 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    27521 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/heartbeats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.759930 sleepecg-0.5.4/sleepecg/io/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/io/ecg_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29259 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/io/gudb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/io/nsrr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/io/physionet.py
--rw-r--r--   0 runner    (1001) docker     (123)    24290 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/io/sleep_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.763930 sleepecg-0.5.4/sleepecg/test/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/test/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/test/test_feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/test/test_heartbeat_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/test/test_heartbeats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/test/test_sleep_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.759930 sleepecg-0.5.4/sleepecg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-13 05:51:12.000000 sleepecg-0.5.4/sleepecg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-13 05:51:12.000000 sleepecg-0.5.4/sleepecg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 05:51:12.000000 sleepecg-0.5.4/sleepecg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-13 05:51:12.000000 sleepecg-0.5.4/sleepecg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 05:51:12.000000 sleepecg-0.5.4/sleepecg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:48:02.234109 sleepecg-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:48:02.222109 sleepecg-0.5.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:48:02.222109 sleepecg-0.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-01 08:47:45.000000 sleepecg-0.5.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 08:47:45.000000 sleepecg-0.5.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 08:47:45.000000 sleepecg-0.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-01 08:47:45.000000 sleepecg-0.5.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-01 08:47:45.000000 sleepecg-0.5.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-01 08:47:45.000000 sleepecg-0.5.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-01 08:47:45.000000 sleepecg-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-01 08:47:45.000000 sleepecg-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-01 08:48:02.230109 sleepecg-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-01 08:47:45.000000 sleepecg-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:48:02.226109 sleepecg-0.5.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-01 08:47:45.000000 sleepecg-0.5.5/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:48:02.226109 sleepecg-0.5.5/examples/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-01 08:47:45.000000 sleepecg-0.5.5/examples/benchmark/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-01 08:47:45.000000 sleepecg-0.5.5/examples/benchmark/benchmark_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-01 08:47:45.000000 sleepecg-0.5.5/examples/benchmark/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-01 08:47:45.000000 sleepecg-0.5.5/examples/benchmark/plot_benchmark_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-01 08:47:45.000000 sleepecg-0.5.5/examples/benchmark/requirements-benchmark.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-01 08:47:45.000000 sleepecg-0.5.5/examples/benchmark/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:48:02.226109 sleepecg-0.5.5/examples/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-01 08:47:45.000000 sleepecg-0.5.5/examples/classifiers/wrn_gru_mesa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-01 08:47:45.000000 sleepecg-0.5.5/examples/classifiers/wrn_gru_mesa_weighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-01 08:47:45.000000 sleepecg-0.5.5/examples/classifiers/ws_gru_mesa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-01 08:47:45.000000 sleepecg-0.5.5/examples/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-01 08:47:45.000000 sleepecg-0.5.5/examples/heartbeat_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-01 08:47:45.000000 sleepecg-0.5.5/examples/try_ws_gru_mesa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-01 08:47:45.000000 sleepecg-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-01 08:47:45.000000 sleepecg-0.5.5/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 08:48:02.234109 sleepecg-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-01 08:47:45.000000 sleepecg-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:48:02.226109 sleepecg-0.5.5/sleepecg/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/_heartbeat_detection.c
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/_heartbeat_detection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19356 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:48:02.230109 sleepecg-0.5.5/sleepecg/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)   775585 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/classifiers/wrn-gru-mesa-weighted.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   764383 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/classifiers/wrn-gru-mesa.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   775057 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/classifiers/ws-gru-mesa.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    26643 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27558 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/heartbeats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:48:02.230109 sleepecg-0.5.5/sleepecg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/io/ecg_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29277 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/io/gudb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/io/nsrr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/io/physionet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24326 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/io/sleep_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:48:02.230109 sleepecg-0.5.5/sleepecg/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/test/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/test/test_feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/test/test_heartbeat_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/test/test_heartbeats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/test/test_sleep_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-01 08:47:45.000000 sleepecg-0.5.5/sleepecg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:48:02.226109 sleepecg-0.5.5/sleepecg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-01 08:48:02.000000 sleepecg-0.5.5/sleepecg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-01 08:48:02.000000 sleepecg-0.5.5/sleepecg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:48:02.000000 sleepecg-0.5.5/sleepecg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-01 08:48:02.000000 sleepecg-0.5.5/sleepecg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 08:48:02.000000 sleepecg-0.5.5/sleepecg.egg-info/top_level.txt
```

### Comparing `sleepecg-0.5.4/.github/workflows/release.yml` & `sleepecg-0.5.5/.github/workflows/release.yml`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.11.2
+        uses: pypa/cibuildwheel@v2.12.1
 
       - uses: actions/upload-artifact@v3
         with:
           path: ./wheelhouse/*.whl
 
 
   build_sdist:
@@ -47,16 +47,16 @@
       - uses: actions/setup-python@v4
         name: Install Python
         with:
           python-version: 3.8
 
       - name: Build sdist
         run: |
-          python -m pip install numpy
-          python setup.py sdist
+          python -m pip install build numpy
+          python -m build --sdist
 
       - uses: actions/upload-artifact@v3
         with:
           path: dist/*.tar.gz
 
 
   upload_pypi:
@@ -64,11 +64,11 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@v1.5.0
+      - uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `sleepecg-0.5.4/.github/workflows/test.yml` & `sleepecg-0.5.5/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -36,12 +36,12 @@
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Build wheels and run pytest
-        uses: pypa/cibuildwheel@v2.11.2
+        uses: pypa/cibuildwheel@v2.12.1
 
       - uses: actions/upload-artifact@v3
         with:
           path: ./wheelhouse/*.whl
```

### Comparing `sleepecg-0.5.4/.pre-commit-config.yaml` & `sleepecg-0.5.5/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 repos:
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
     - id: check-case-conflict
     - id: check-merge-conflict
     - id: check-yaml
     - id: check-toml
     - id: mixed-line-ending
     - id: check-builtin-literals
 
-  - repo: https://github.com/pycqa/flake8
-    rev: 4.0.1
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: v0.0.269
     hooks:
-    - id: flake8
-
-  - repo: https://github.com/pycqa/pydocstyle
-    rev: 6.1.1
-    hooks:
-    - id: pydocstyle
-      files: ^sleepecg/
+      - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.2.0
     hooks:
     - id: mypy
       exclude: ^sleepecg/test/|^examples
       additional_dependencies:
       - types-PyYAML
       - types-requests
       - types-urllib3
```

### Comparing `sleepecg-0.5.4/CHANGELOG.md` & `sleepecg-0.5.5/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## [0.5.5] - 2023-06-01
+### Changed
+- Use absolute imports internally ([#170](https://github.com/cbrnr/sleepecg/pull/170) by [Clemens Brunner](https://github.com/cbrnr))
+
 ## [0.5.4] - 2023-04-13
 ### Changed
 - Remove dependency on pandas for `read_gudb` ([#134](https://github.com/cbrnr/sleepecg/pull/134) by [Florian Hofer](https://github.com/hofaflo))
 - Update SHHS encoding and missing data handling for `read_shhs` ([#139](https://github.com/cbrnr/sleepecg/pull/139) by [Andrew Gilbert](https://github.com/adgilbert))
 - Ignore expected warnings during feature extraction ([#142](https://github.com/cbrnr/sleepecg/pull/142) by [Florian Hofer](https://github.com/hofaflo))
 
 ## [0.5.3] - 2022-12-05
```

### Comparing `sleepecg-0.5.4/CONTRIBUTING.md` & `sleepecg-0.5.5/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 - Push to your remote fork: `git push` (might require `git push --force`)
 
 
 ## Development enviroment
 Make sure to use Python 3.8. You might want to [create a virtual environment](https://docs.python.org/3/library/venv.html#creating-virtual-environments) instead of working your main environment. In the root of the local clone of your fork, install SleepECG as follows:
 
 ```
-pip install -e .[dev]
+pip install -e ".[dev]"
 ```
 
 When using the flag [`-e`](https://pip.pypa.io/en/stable/cli/pip_install/#install-editable), pip does not copy the package to `site-packages/`, but creates a link to your local repository. Any changes to the source code are directly reflected in the "installed" package. Installing the optional `[dev]` dependencies makes sure all tools for style checking, testing, and building documentation are locally available.
 
 
 ## Code style
 SleepECG adheres to [PEP 8](https://www.python.org/dev/peps/pep-0008/) and [Black](https://black.readthedocs.io/en/stable/index.html), with the following exceptions/specifications:
```

### Comparing `sleepecg-0.5.4/LICENSE` & `sleepecg-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/PKG-INFO` & `sleepecg-0.5.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,106 @@
 Metadata-Version: 2.1
 Name: sleepecg
-Version: 0.5.4
+Version: 0.5.5
 Summary: A package for sleep stage classification using ECG data
-Home-page: https://github.com/cbrnr/sleepecg
-Author: Florian Hofer
-Author-email: hofaflo@gmail.com
-Maintainer: Clemens Brunner
-Maintainer-email: clemens.brunner@gmail.com
-License: BSD 3-Clause License
-Description: ![Python](https://img.shields.io/pypi/pyversions/sleepecg.svg?logo=python&logoColor=white)
-        [![PyPI](https://img.shields.io/pypi/v/sleepecg)](https://pypi.org/project/sleepecg/)
-        [![conda-forge](https://img.shields.io/conda/v/conda-forge/sleepecg.svg?label=conda-forge)](https://anaconda.org/conda-forge/sleepecg)
-        [![Docs](https://readthedocs.org/projects/sleepecg/badge/?version=latest)](https://sleepecg.readthedocs.io/en/stable/index.html)
-        [![License](https://img.shields.io/github/license/cbrnr/sleepecg)](LICENSE)
-        
-        ## SleepECG
-        SleepECG provides tools for sleep stage classification when [EEG](https://en.wikipedia.org/wiki/Electroencephalography) signals are not available. Based only on [ECG](https://en.wikipedia.org/wiki/Electrocardiography) (and to a lesser extent also movement data), SleepECG provides functions for
-        
-        - downloading and reading open polysomnography datasets,
-        - detecting heartbeats from ECG signals, and
-        - classifying sleep stages (which includes preprocessing, feature extraction, and classification).
-        
-        ### Documentation
-        Documentation for SleepECG is available on [Read the Docs](https://sleepecg.readthedocs.io/en/stable/index.html).
-        
-        ### Changelog
-        Check out the [changelog](https://github.com/cbrnr/sleepecg/blob/main/CHANGELOG.md) to learn what we added, changed, or fixed.
-        
-        ### Dependencies
-        SleepECG requires Python ≥ 3.8 and the following packages:
-        
-        - [numpy](http://www.numpy.org/) ≥ 1.20.0
-        - [requests](https://requests.readthedocs.io/en/latest/) ≥ 2.25.0
-        - [scipy](https://scipy.org/) ≥ 1.7.0
-        - [tqdm](https://tqdm.github.io/) ≥ 4.60.0
-        - [PyYAML](https://pyyaml.org/) ≥ 5.4.0
-        
-        Optional dependencies provide additional features:
-        
-        - [joblib](https://joblib.readthedocs.io/en/latest/) ≥ 1.0.0 (parallelized feature extraction)
-        - [matplotlib](https://matplotlib.org/) ≥ 3.5.0 (plot ECG time courses, hypnograms, and confusion matrices)
-        - [mne](https://mne.tools/stable/index.html) ≥ 1.0.0 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
-        - [numba](https://numba.pydata.org/) ≥ 0.55.0 (JIT-compiled heartbeat detector)
-        - [tensorflow](https://www.tensorflow.org/) ≥ 2.7.0 (sleep stage classification with Keras models)
-        - [wfdb](https://github.com/MIT-LCP/wfdb-python/) ≥ 3.4.0 (read data from [SLPDB](https://physionet.org/content/slpdb), [MITDB](https://physionet.org/content/mitdb), and [LTDB](https://physionet.org/content/ltdb))
-        
-        ### Installation
-        SleepECG is available on PyPI and can be installed with [pip](https://pip.pypa.io/en/stable/):
-        
-        ```
-        pip install sleepecg
-        ```
-        
-        Alternatively, an unofficial [conda](https://docs.conda.io/en/latest/) package is available:
-        
-        ```
-        conda install -c conda-forge sleepecg
-        ```
-        
-        SleepECG with all optional dependencies can be installed with the following command:
-        
-        ```
-        pip install sleepecg[full]
-        ```
-        
-        If you want the latest development version, use the following command:
-        
-        ```
-        pip install git+https://github.com/cbrnr/sleepecg
-        ```
-        
-        ### Contributing
-        The [contributing guide](https://github.com/cbrnr/sleepecg/blob/main/CONTRIBUTING.md) contains detailed instructions on how to contribute to SleepECG.
-        
+Author-email: Florian Hofer <hofaflo@gmail.com>, Clemens Brunner <clemens.brunner@gmail.com>
+License: BSD 3-Clause
+Project-URL: homepage, https://github.com/cbrnr/sleepecg
+Project-URL: documentation, https://sleepecg.readthedocs.io/en/latest/
+Project-URL: repository, https://github.com/cbrnr/sleepecg
+Project-URL: changelog, https://github.com/cbrnr/sleepecg/blob/main/CHANGELOG.md
 Keywords: sleep,ecg,qrs,peak
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: cibw
+License-File: LICENSE
+
+![Python](https://img.shields.io/pypi/pyversions/sleepecg.svg?logo=python&logoColor=white)
+[![PyPI](https://img.shields.io/pypi/v/sleepecg)](https://pypi.org/project/sleepecg/)
+[![conda-forge](https://img.shields.io/conda/v/conda-forge/sleepecg.svg?label=conda-forge)](https://anaconda.org/conda-forge/sleepecg)
+[![Docs](https://readthedocs.org/projects/sleepecg/badge/?version=latest)](https://sleepecg.readthedocs.io/en/stable/index.html)
+[![License](https://img.shields.io/github/license/cbrnr/sleepecg)](LICENSE)
+
+## SleepECG
+SleepECG provides tools for sleep stage classification when [EEG](https://en.wikipedia.org/wiki/Electroencephalography) signals are not available. Based only on [ECG](https://en.wikipedia.org/wiki/Electrocardiography), SleepECG provides functions for
+
+- downloading and reading open polysomnography datasets,
+- detecting heartbeats from ECG signals, and
+- classifying sleep stages (which includes preprocessing, feature extraction, and classification).
+
+### Documentation
+Documentation for SleepECG is available on [Read the Docs](https://sleepecg.readthedocs.io/en/stable/index.html).
+
+### Changelog
+Check out the [changelog](https://github.com/cbrnr/sleepecg/blob/main/CHANGELOG.md) to learn what we added, changed, or fixed.
+
+### Dependencies
+SleepECG requires Python ≥ 3.8 and the following packages:
+
+- [numpy](http://www.numpy.org/) ≥ 1.20.0
+- [requests](https://requests.readthedocs.io/en/latest/) ≥ 2.25.0
+- [scipy](https://scipy.org/) ≥ 1.7.0
+- [tqdm](https://tqdm.github.io/) ≥ 4.60.0
+- [PyYAML](https://pyyaml.org/) ≥ 5.4.0
+
+Optional dependencies provide additional features:
+
+- [joblib](https://joblib.readthedocs.io/en/latest/) ≥ 1.0.0 (parallelized feature extraction)
+- [matplotlib](https://matplotlib.org/) ≥ 3.5.0 (plot ECG time courses, hypnograms, and confusion matrices)
+- [mne](https://mne.tools/stable/index.html) ≥ 1.0.0 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
+- [numba](https://numba.pydata.org/) ≥ 0.55.0 (JIT-compiled heartbeat detector)
+- [tensorflow](https://www.tensorflow.org/) ≥ 2.7.0 (sleep stage classification with Keras models)
+- [wfdb](https://github.com/MIT-LCP/wfdb-python/) ≥ 3.4.0 (read data from [SLPDB](https://physionet.org/content/slpdb), [MITDB](https://physionet.org/content/mitdb), and [LTDB](https://physionet.org/content/ltdb))
+
+### Installation
+SleepECG is available on PyPI and can be installed with [pip](https://pip.pypa.io/en/stable/):
+
+```
+pip install sleepecg
+```
+
+Alternatively, an unofficial [conda](https://docs.conda.io/en/latest/) package is available:
+
+```
+conda install -c conda-forge sleepecg
+```
+
+SleepECG with all optional dependencies can be installed with the following command:
+
+```
+pip install "sleepecg[full]"
+```
+
+If you want the latest development version, use the following command:
+
+```
+pip install git+https://github.com/cbrnr/sleepecg
+```
+
+### Example
+The following example detects heartbeats in a short ECG (a one-dimensional NumPy array):
+
+```python
+import numpy as np
+from scipy.misc import electrocardiogram
+from sleepecg import detect_heartbeats
+
+ecg = electrocardiogram()  # 5 min of ECG data at 360 Hz
+fs = 360  # sampling frequency
+beats = detect_heartbeats(ecg, fs)  # indices of detected heartbeats
+```
+
+More examples are available at https://github.com/cbrnr/sleepecg/tree/main/examples.
+
+### Contributing
+The [contributing guide](https://github.com/cbrnr/sleepecg/blob/main/CONTRIBUTING.md) contains detailed instructions on how to contribute to SleepECG.
```

### Comparing `sleepecg-0.5.4/README.md` & `sleepecg-0.5.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![Python](https://img.shields.io/pypi/pyversions/sleepecg.svg?logo=python&logoColor=white)
 [![PyPI](https://img.shields.io/pypi/v/sleepecg)](https://pypi.org/project/sleepecg/)
 [![conda-forge](https://img.shields.io/conda/v/conda-forge/sleepecg.svg?label=conda-forge)](https://anaconda.org/conda-forge/sleepecg)
 [![Docs](https://readthedocs.org/projects/sleepecg/badge/?version=latest)](https://sleepecg.readthedocs.io/en/stable/index.html)
 [![License](https://img.shields.io/github/license/cbrnr/sleepecg)](LICENSE)
 
 ## SleepECG
-SleepECG provides tools for sleep stage classification when [EEG](https://en.wikipedia.org/wiki/Electroencephalography) signals are not available. Based only on [ECG](https://en.wikipedia.org/wiki/Electrocardiography) (and to a lesser extent also movement data), SleepECG provides functions for
+SleepECG provides tools for sleep stage classification when [EEG](https://en.wikipedia.org/wiki/Electroencephalography) signals are not available. Based only on [ECG](https://en.wikipedia.org/wiki/Electrocardiography), SleepECG provides functions for
 
 - downloading and reading open polysomnography datasets,
 - detecting heartbeats from ECG signals, and
 - classifying sleep stages (which includes preprocessing, feature extraction, and classification).
 
 ### Documentation
 Documentation for SleepECG is available on [Read the Docs](https://sleepecg.readthedocs.io/en/stable/index.html).
@@ -47,18 +47,33 @@
 ```
 conda install -c conda-forge sleepecg
 ```
 
 SleepECG with all optional dependencies can be installed with the following command:
 
 ```
-pip install sleepecg[full]
+pip install "sleepecg[full]"
 ```
 
 If you want the latest development version, use the following command:
 
 ```
 pip install git+https://github.com/cbrnr/sleepecg
 ```
 
+### Example
+The following example detects heartbeats in a short ECG (a one-dimensional NumPy array):
+
+```python
+import numpy as np
+from scipy.misc import electrocardiogram
+from sleepecg import detect_heartbeats
+
+ecg = electrocardiogram()  # 5 min of ECG data at 360 Hz
+fs = 360  # sampling frequency
+beats = detect_heartbeats(ecg, fs)  # indices of detected heartbeats
+```
+
+More examples are available at https://github.com/cbrnr/sleepecg/tree/main/examples.
+
 ### Contributing
 The [contributing guide](https://github.com/cbrnr/sleepecg/blob/main/CONTRIBUTING.md) contains detailed instructions on how to contribute to SleepECG.
```

### Comparing `sleepecg-0.5.4/examples/benchmark/README.md` & `sleepecg-0.5.5/examples/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/examples/benchmark/benchmark_detectors.py` & `sleepecg-0.5.5/examples/benchmark/benchmark_detectors.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/examples/benchmark/config.yml` & `sleepecg-0.5.5/examples/benchmark/config.yml`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/examples/benchmark/plot_benchmark_results.py` & `sleepecg-0.5.5/examples/benchmark/plot_benchmark_results.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/examples/benchmark/utils.py` & `sleepecg-0.5.5/examples/benchmark/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 
 from __future__ import annotations
 
 import time
 from typing import Any, Iterator
 
 import numpy as np
+
 import sleepecg
 from sleepecg.io.ecg_readers import ECGRecord
 
 
 class HeartpyWarning(Warning):
+    """Warning for all Heartpy-related warnings."""
+
     pass
 
 
 def reader_dispatch(db_slug: str, data_dir: str) -> Iterator[ECGRecord]:
     """
     Read ECG records from mitdb, ltdb or gudb.
```

### Comparing `sleepecg-0.5.4/examples/classifiers/wrn_gru_mesa.py` & `sleepecg-0.5.5/examples/classifiers/wrn_gru_mesa.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/examples/classifiers/wrn_gru_mesa_weighted.py` & `sleepecg-0.5.5/examples/classifiers/wrn_gru_mesa_weighted.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/examples/classifiers/ws_gru_mesa.py` & `sleepecg-0.5.5/examples/classifiers/ws_gru_mesa.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/examples/feature_extraction.py` & `sleepecg-0.5.5/examples/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/examples/heartbeat_detection.py` & `sleepecg-0.5.5/examples/heartbeat_detection.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/examples/try_ws_gru_mesa.py` & `sleepecg-0.5.5/examples/try_ws_gru_mesa.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # %%
+import matplotlib.pyplot as plt
+
 from sleepecg import load_classifier, plot_hypnogram, read_slpdb, stage
 
 # The model was built using tensorflow 2.7, running on higher versions might create warnings
 # but should not influence the results.
 clf = load_classifier("ws-gru-mesa", "SleepECG")
 
 # %% Load record
@@ -14,7 +16,9 @@
 
 plot_hypnogram(
     rec,
     stages_pred,
     stages_mode=clf.stages_mode,
     merge_annotations=True,
 )
+
+plt.show()
```

### Comparing `sleepecg-0.5.4/sleepecg/__init__.py` & `sleepecg-0.5.5/sleepecg/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """A package for sleep stage classification using ECG data."""
 
-from .classification import (
+from sleepecg.classification import (
     SleepClassifier,
     evaluate,
     list_classifiers,
     load_classifier,
     prepare_data_keras,
     print_class_balance,
     save_classifier,
     stage,
 )
-from .config import get_config, set_config
-from .feature_extraction import extract_features, preprocess_rri
-from .heartbeats import compare_heartbeats, detect_heartbeats, rri_similarity
-from .io import *  # noqa: F403
-from .plot import plot_ecg, plot_hypnogram
+from sleepecg.config import get_config, set_config
+from sleepecg.feature_extraction import extract_features, preprocess_rri
+from sleepecg.heartbeats import compare_heartbeats, detect_heartbeats, rri_similarity
+from sleepecg.io import *  # noqa: F403
+from sleepecg.plot import plot_ecg, plot_hypnogram
 
-__version__ = "0.5.4"
+__version__ = "0.5.5"
```

### Comparing `sleepecg-0.5.4/sleepecg/_heartbeat_detection.c` & `sleepecg-0.5.5/sleepecg/_heartbeat_detection.c`

 * *Files 2% similar despite different names*

```diff
@@ -228,29 +228,34 @@
 
     // tracking the number of peaks found is required to calculate the
     // average RR intervals correctly during the first 8 beats (also needed
     // for access to RR_intervals)
     int num_peaks_found = 0;
 
     double RR_missed_limit;
+    double PEAKF;
+
+    // RR_log_limit, RR_high_limit, and PEAKI are initialized here to avoid
+    // compiler warnings. The initialization value does not matter as their
+    // values will be set before being used for the first time.
+    double RR_low_limit = 0.0;
+    double RR_high_limit = 0.0;
+    double PEAKI = 0.0;
 
     // in case a searchback was unsuccessful, no new searchback will be
     // performed until another signal peak has been found regularly
     char do_searchback = 1;
 
     // initialize, so searchback before any peak has been detected works
     int peak_index = -REFRACTORY_SAMPLES + 1;
     int previous_peak_index = -REFRACTORY_SAMPLES + 1;
 
     int index = 1;
     while (index < signal_len - 1)
     {
-        double PEAKF;
-        double PEAKI;
-
         char signal_peak_found = 0;
         char noise_peak_found = 0;
         // ----------------------------------------------------------------
         // Searchback
         // ----------------------------------------------------------------
         // During a "searchback", detection thresholds are reduced by one
         // half. The peak with highest amplitude between 200ms (i.e. the
@@ -438,17 +443,14 @@
 
             // calculating RR averages only makes sense once 2 peaks have
             // been found
             if (num_peaks_found > 1)
             {
                 RR_intervals[num_peaks_found] = peak_index - previous_peak_index;
 
-                double RR_low_limit;
-                double RR_high_limit;
-
                 // --------------------------------------------------------
                 // Learning phase 2
                 // --------------------------------------------------------
                 // "Learning phase 2 requires two heartbeats to initialize
                 // RR interval average and RR interval limit values."
                 // (from Pan & Tompkins, 1985)
                 if (num_peaks_found == 2)
```

### Comparing `sleepecg-0.5.4/sleepecg/classification.py` & `sleepecg-0.5.5/sleepecg/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from tempfile import TemporaryDirectory
 from typing import Any, Optional, Protocol
 from zipfile import ZipFile
 
 import numpy as np
 import yaml
 
-from .config import get_config
-from .feature_extraction import extract_features
-from .io.sleep_readers import SleepRecord, SleepStage
-from .utils import _STAGE_NAMES, _merge_sleep_stages
+from sleepecg.config import get_config
+from sleepecg.feature_extraction import extract_features
+from sleepecg.io.sleep_readers import SleepRecord, SleepStage
+from sleepecg.utils import _STAGE_NAMES, _merge_sleep_stages
 
 
 def prepare_data_keras(
     features: list[np.ndarray],
     stages: list[np.ndarray],
     stages_mode: str,
     mask_value: int = -1,
@@ -248,14 +248,15 @@
             f"    source file: {self.source_file}\n"
         )
 
 
 def load_classifier(
     name: str,
     classifiers_dir: Optional[str | Path] = None,
+    silence_tf_messages: bool = True,
 ) -> SleepClassifier:
     """
     Load a `SleepClassifier` from disk.
 
     This functions reads `.zip` files saved by `save_classifier()`. Pass `'SleepECG'` as the
     second argument to load a classifier bundled with SleepECG.
 
@@ -263,14 +264,17 @@
     ----------
     name : str
         The identifier of the classifier to load.
     classifiers_dir : str | pathlib.Path, optional
         Directory in which to look for `<name>.zip`. If `None` (default), the value is taken
         from the configuration. If `'SleepECG'`, load classifiers from
         `site-packages/sleepecg/classifiers`.
+    silence_tf_messages : bool, optional
+        Whether or not to silence messages from TensorFlow when loading a model. By default
+        `True`.
 
     Returns
     -------
     SleepClassifier
         Contains the model and metadata required for feature extraction and preprocessing.
         Can be passed to `stage()`.
 
@@ -288,17 +292,27 @@
     with TemporaryDirectory() as tmpdir:
         shutil.unpack_archive(soure_file, tmpdir)
 
         with open(f"{tmpdir}/info.yml") as infofile:
             classifier_info = yaml.safe_load(infofile)
 
         if classifier_info["model_type"] == "keras":
+            import os
+
+            environ_orig = os.environ.copy()
+            if silence_tf_messages:
+                os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
+
             from tensorflow import keras
 
-            classifier = keras.models.load_model(f"{tmpdir}/classifier")
+            try:
+                classifier = keras.models.load_model(f"{tmpdir}/classifier")
+            finally:
+                os.environ.clear()
+                os.environ.update(environ_orig)
 
         else:
             raise ValueError(
                 f"Loading model of type {classifier_info['model_type']} is not supported"
             )
 
     return SleepClassifier(
```

### Comparing `sleepecg-0.5.4/sleepecg/classifiers/wrn-gru-mesa-weighted.zip` & `sleepecg-0.5.5/sleepecg/classifiers/wrn-gru-mesa-weighted.zip`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/sleepecg/classifiers/wrn-gru-mesa.zip` & `sleepecg-0.5.5/sleepecg/classifiers/wrn-gru-mesa.zip`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/sleepecg/classifiers/ws-gru-mesa.zip` & `sleepecg-0.5.5/sleepecg/classifiers/ws-gru-mesa.zip`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/sleepecg/config.py` & `sleepecg-0.5.5/sleepecg/config.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/sleepecg/feature_extraction.py` & `sleepecg-0.5.5/sleepecg/feature_extraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from typing import Iterable, Optional
 
 import numpy as np
 from numpy.lib.stride_tricks import sliding_window_view
 from scipy.interpolate import interp1d
 from scipy.signal import periodogram
 
-from .io.sleep_readers import SleepRecord
-from .utils import _parallel, _time_to_sec
+from sleepecg.io.sleep_readers import SleepRecord
+from sleepecg.utils import _parallel, _time_to_sec
 
 _FEATURE_GROUPS = {
     "hrv-time": (
         "meanNN",
         "maxNN",
         "minNN",
         "rangeNN",
```

### Comparing `sleepecg-0.5.4/sleepecg/heartbeats.py` & `sleepecg-0.5.5/sleepecg/heartbeats.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import scipy.signal
 import scipy.stats
 
 _all_backends = ("c", "numba", "python")
 _available_backends = list(_all_backends)
 
 try:
-    from ._heartbeat_detection import _squared_moving_integration, _thresholding
+    from sleepecg._heartbeat_detection import _squared_moving_integration, _thresholding
 except ImportError:
     _available_backends.remove("c")
 
 try:
     from numba import jit
 except ImportError:
     _available_backends.remove("numba")
@@ -438,15 +438,14 @@
                 num_peaks_found > 1
                 and index - previous_peak_index > RR_missed_limit
                 and do_searchback
             )
             or (num_peaks_found == 0 and index > fs)  # original criterion
             or (num_peaks_found == 1 and index - previous_peak_index > 1.5 * fs)  # (1)
         ):  # (2)
-
             for i in range(1, 16):
                 found_a_candidate = False
 
                 searchback_divisor = 1 << i  # 2^i
                 best_searchback_index = previous_peak_index + REFRACTORY_SAMPLES
                 best_candidate_amplitude = -1
                 searchback_index = best_searchback_index
@@ -633,9 +632,9 @@
         index += 1
 
     # return an array containing `1`s at beat positions and `0`s elsewhere
     return beat_mask
 
 
 if "numba" in _available_backends:
-    _squared_moving_integration_numba = jit(_squared_moving_integration_py)
-    _thresholding_numba = jit(_thresholding_py)
+    _squared_moving_integration_numba = jit(_squared_moving_integration_py, nopython=True)
+    _thresholding_numba = jit(_thresholding_py, nopython=True)
```

### Comparing `sleepecg-0.5.4/sleepecg/io/ecg_readers.py` & `sleepecg-0.5.5/sleepecg/io/ecg_readers.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 
 import numpy as np
 from tqdm import tqdm
 
 if TYPE_CHECKING:
     import matplotlib.pyplot as plt
 
-from ..config import get_config
-from ..plot import plot_ecg
-from .gudb import _GUDB_MD5
-from .physionet import _list_physionet, download_physionet
-from .utils import _download_file
+from sleepecg.config import get_config
+from sleepecg.io.gudb import _GUDB_MD5
+from sleepecg.io.physionet import _list_physionet, download_physionet
+from sleepecg.io.utils import _download_file
+from sleepecg.plot import plot_ecg
 
 
 @dataclass
 class ECGRecord:
     """
     Store a single ECG record.
 
     Attributes
     ----------
     ecg : np.ndarray
         The ECG signal.
     fs : float
-        The sampling frequency.
+        The sampling frequency in Hz.
     annotation : np.ndarray
         Indices of annotated heartbeats.
     lead : str, optional
         Which ECG lead the signal was recorded from, by default `None`.
     id : str, optional
         The record ID, by default `None`.
     """
```

### Comparing `sleepecg-0.5.4/sleepecg/io/gudb.py` & `sleepecg-0.5.5/sleepecg/io/gudb.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 """Utilities for downloading GUDB data."""
 
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Optional
 
-from ..config import get_config
-from .utils import _calculate_checksum
+from sleepecg.config import get_config
+from sleepecg.io.utils import _calculate_checksum
 
 _GUDB_MD5 = {
     "subject_00/sitting/ECG.tsv": "06cdda76a17ff6efe4d4b18ccbc66e0f",
     "subject_00/sitting/annotation_cs.tsv": "fd0e6f5796a103637e29c4f9c14d155c",
     "subject_00/sitting/annotation_cables.tsv": "f5dfb5b4073974cc6aaf8ca3cc262002",
     "subject_00/maths/ECG.tsv": "c45d6702d76cb4083592b2c5ff2a298f",
     "subject_00/maths/annotation_cs.tsv": "839a5708475774a3a8ab6d7f31ac1646",
```

### Comparing `sleepecg-0.5.4/sleepecg/io/nsrr.py` & `sleepecg-0.5.5/sleepecg/io/nsrr.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from fnmatch import fnmatch
 from json.decoder import JSONDecodeError
 from pathlib import Path
 
 import requests
 from tqdm import tqdm
 
-from .utils import _download_file
+from sleepecg.io.utils import _download_file
 
 _nsrr_token = None
 
 
 def set_nsrr_token(token: str) -> None:
     """
     Set and verify the [NSRR](https://sleepdata.org) download token.
```

### Comparing `sleepecg-0.5.4/sleepecg/io/physionet.py` & `sleepecg-0.5.5/sleepecg/io/physionet.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import fnmatch
 from pathlib import Path
 from typing import Iterable
 
 from tqdm import tqdm
 
-from .utils import _download_file
+from sleepecg.io.utils import _download_file
 
 _PHYSIONET_FILES_URL = "https://physionet.org/files/"
 _CHECKSUM_FILENAME = "SHA256SUMS.txt"
 _RECORDS_FILENAME = "RECORDS"
 _CHECKSUM_TYPE = "sha256"
```

### Comparing `sleepecg-0.5.4/sleepecg/io/sleep_readers.py` & `sleepecg-0.5.5/sleepecg/io/sleep_readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from enum import IntEnum
 from pathlib import Path
 from typing import Iterator, NamedTuple, Optional
 from xml.etree import ElementTree
 
 import numpy as np
 
-from ..config import get_config
-from ..heartbeats import detect_heartbeats
-from .nsrr import _download_nsrr_file, _get_nsrr_url, _list_nsrr, download_nsrr
-from .physionet import _list_physionet, download_physionet
+from sleepecg.config import get_config
+from sleepecg.heartbeats import detect_heartbeats
+from sleepecg.io.nsrr import _download_nsrr_file, _get_nsrr_url, _list_nsrr, download_nsrr
+from sleepecg.io.physionet import _list_physionet, download_physionet
 
 
 class SleepStage(IntEnum):
     """
     Mapping of AASM sleep stages to integers.
 
     To facilitate hypnogram plotting, values start with zero and increase with wakefulness.
```

### Comparing `sleepecg-0.5.4/sleepecg/io/utils.py` & `sleepecg-0.5.5/sleepecg/io/utils.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/sleepecg/plot.py` & `sleepecg-0.5.5/sleepecg/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from typing import TYPE_CHECKING, Optional
 
 import numpy as np
 
 if TYPE_CHECKING:
     import matplotlib.pyplot as plt
 
-from .io.sleep_readers import SleepRecord, SleepStage
-from .utils import _STAGE_INTS, _STAGE_NAMES, _merge_sleep_stages, _time_to_sec
+from sleepecg.io.sleep_readers import SleepRecord, SleepStage
+from sleepecg.utils import _STAGE_INTS, _STAGE_NAMES, _merge_sleep_stages, _time_to_sec
 
 
 def plot_ecg(
     ecg: np.ndarray,
     fs: float,
     title: Optional[str] = None,
     **kwargs: np.ndarray,
```

### Comparing `sleepecg-0.5.4/sleepecg/test/test_classification.py` & `sleepecg-0.5.5/sleepecg/test/test_classification.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/sleepecg/test/test_config.py` & `sleepecg-0.5.5/sleepecg/test/test_config.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/sleepecg/test/test_examples.py` & `sleepecg-0.5.5/sleepecg/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/sleepecg/test/test_feature_extraction.py` & `sleepecg-0.5.5/sleepecg/test/test_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.4/sleepecg/test/test_heartbeat_detection.py` & `sleepecg-0.5.5/sleepecg/test/test_heartbeat_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 
 """Tests for heartbeat detection."""
 
 import sys
 
 import numpy as np
 import pytest
-from scipy.misc import electrocardiogram
+
+try:
+    from scipy.datasets import electrocardiogram  # SciPy ≥ 1.10
+except ImportError:
+    from scipy.misc import electrocardiogram  # SciPy < 1.10
 from scipy.signal import resample_poly
 
 from sleepecg import compare_heartbeats, detect_heartbeats
 
 pytestmark = pytest.mark.c_extension
 ecg = electrocardiogram()
 fs = 360
```

### Comparing `sleepecg-0.5.4/sleepecg/test/test_heartbeats.py` & `sleepecg-0.5.5/sleepecg/test/test_heartbeats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # © SleepECG developers
 #
 # License: BSD (3-clause)
 
 """Tests for heartbeat detection and detector evaluation."""
 
-import sys
-
 import numpy as np
 import pytest
 
 from sleepecg import compare_heartbeats, detect_heartbeats, read_mitdb
 
 
 def test_compare_heartbeats():
@@ -27,27 +25,15 @@
 
 @pytest.fixture(scope="session")
 def mitdb_234_MLII():
     """Fetch record for detector tests."""
     return next(read_mitdb(records_pattern="234"))
 
 
-@pytest.mark.parametrize(
-    "backend",
-    [
-        "c",
-        pytest.param(
-            "numba",
-            marks=pytest.mark.skipif(
-                sys.version_info >= (3, 11), reason="numba does not support Python 3.11 yet"
-            ),
-        ),
-        "python",
-    ],
-)
+@pytest.mark.parametrize("backend", ["c", "numba", "python"])
 def test_detect_heartbeats(mitdb_234_MLII, backend):
     """Test heartbeat detection on mitdb:234:MLII."""
     record = mitdb_234_MLII
     detection = detect_heartbeats(record.ecg, record.fs, backend=backend)
     TP, FP, FN = compare_heartbeats(detection, record.annotation, int(record.fs / 10))
 
     # Changes in the heartbeat detector should not lead to worse results!
```

### Comparing `sleepecg-0.5.4/sleepecg/test/test_sleep_readers.py` & `sleepecg-0.5.5/sleepecg/test/test_sleep_readers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 
 from __future__ import annotations
 
 import datetime
 from pathlib import Path
 
 import numpy as np
-import scipy.misc
+
+try:
+    from scipy.datasets import electrocardiogram  # SciPy ≥ 1.10
+except ImportError:
+    from scipy.misc import electrocardiogram  # SciPy < 1.10
 from pyedflib import highlevel
 
 from sleepecg import SleepStage, read_mesa, read_shhs, read_slpdb
 from sleepecg.io.sleep_readers import Gender
 
 
 def _dummy_nsrr_edf(filename: str, hours: float, ecg_channel: str):
     ECG_FS = 360
-    ecg_5_min = scipy.misc.electrocardiogram()
+    ecg_5_min = electrocardiogram()
     seconds = int(hours * 60 * 60)
     ecg = np.tile(ecg_5_min, int(np.ceil(seconds / 300)))[np.newaxis, : seconds * ECG_FS]
     signal_headers = highlevel.make_signal_headers([ecg_channel], sample_frequency=ECG_FS)
     highlevel.write_edf(filename, ecg, signal_headers)
 
 
 def _dummy_nsrr_xml(filename: str, hours: float, random_state: int):
```

### Comparing `sleepecg-0.5.4/sleepecg/utils.py` & `sleepecg-0.5.5/sleepecg/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import datetime
 import warnings
 from typing import Any, Callable, Iterable, TypeVar
 
 import numpy as np
 
-from .io.sleep_readers import SleepStage
+from sleepecg.io.sleep_readers import SleepStage
 
 # required to propagate the return type annotation through _parallel
 _Returnable = TypeVar("_Returnable")
 
 
 def _parallel(
     n_jobs: int,
```

### Comparing `sleepecg-0.5.4/sleepecg.egg-info/PKG-INFO` & `sleepecg-0.5.5/sleepecg.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,106 @@
 Metadata-Version: 2.1
 Name: sleepecg
-Version: 0.5.4
+Version: 0.5.5
 Summary: A package for sleep stage classification using ECG data
-Home-page: https://github.com/cbrnr/sleepecg
-Author: Florian Hofer
-Author-email: hofaflo@gmail.com
-Maintainer: Clemens Brunner
-Maintainer-email: clemens.brunner@gmail.com
-License: BSD 3-Clause License
-Description: ![Python](https://img.shields.io/pypi/pyversions/sleepecg.svg?logo=python&logoColor=white)
-        [![PyPI](https://img.shields.io/pypi/v/sleepecg)](https://pypi.org/project/sleepecg/)
-        [![conda-forge](https://img.shields.io/conda/v/conda-forge/sleepecg.svg?label=conda-forge)](https://anaconda.org/conda-forge/sleepecg)
-        [![Docs](https://readthedocs.org/projects/sleepecg/badge/?version=latest)](https://sleepecg.readthedocs.io/en/stable/index.html)
-        [![License](https://img.shields.io/github/license/cbrnr/sleepecg)](LICENSE)
-        
-        ## SleepECG
-        SleepECG provides tools for sleep stage classification when [EEG](https://en.wikipedia.org/wiki/Electroencephalography) signals are not available. Based only on [ECG](https://en.wikipedia.org/wiki/Electrocardiography) (and to a lesser extent also movement data), SleepECG provides functions for
-        
-        - downloading and reading open polysomnography datasets,
-        - detecting heartbeats from ECG signals, and
-        - classifying sleep stages (which includes preprocessing, feature extraction, and classification).
-        
-        ### Documentation
-        Documentation for SleepECG is available on [Read the Docs](https://sleepecg.readthedocs.io/en/stable/index.html).
-        
-        ### Changelog
-        Check out the [changelog](https://github.com/cbrnr/sleepecg/blob/main/CHANGELOG.md) to learn what we added, changed, or fixed.
-        
-        ### Dependencies
-        SleepECG requires Python ≥ 3.8 and the following packages:
-        
-        - [numpy](http://www.numpy.org/) ≥ 1.20.0
-        - [requests](https://requests.readthedocs.io/en/latest/) ≥ 2.25.0
-        - [scipy](https://scipy.org/) ≥ 1.7.0
-        - [tqdm](https://tqdm.github.io/) ≥ 4.60.0
-        - [PyYAML](https://pyyaml.org/) ≥ 5.4.0
-        
-        Optional dependencies provide additional features:
-        
-        - [joblib](https://joblib.readthedocs.io/en/latest/) ≥ 1.0.0 (parallelized feature extraction)
-        - [matplotlib](https://matplotlib.org/) ≥ 3.5.0 (plot ECG time courses, hypnograms, and confusion matrices)
-        - [mne](https://mne.tools/stable/index.html) ≥ 1.0.0 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
-        - [numba](https://numba.pydata.org/) ≥ 0.55.0 (JIT-compiled heartbeat detector)
-        - [tensorflow](https://www.tensorflow.org/) ≥ 2.7.0 (sleep stage classification with Keras models)
-        - [wfdb](https://github.com/MIT-LCP/wfdb-python/) ≥ 3.4.0 (read data from [SLPDB](https://physionet.org/content/slpdb), [MITDB](https://physionet.org/content/mitdb), and [LTDB](https://physionet.org/content/ltdb))
-        
-        ### Installation
-        SleepECG is available on PyPI and can be installed with [pip](https://pip.pypa.io/en/stable/):
-        
-        ```
-        pip install sleepecg
-        ```
-        
-        Alternatively, an unofficial [conda](https://docs.conda.io/en/latest/) package is available:
-        
-        ```
-        conda install -c conda-forge sleepecg
-        ```
-        
-        SleepECG with all optional dependencies can be installed with the following command:
-        
-        ```
-        pip install sleepecg[full]
-        ```
-        
-        If you want the latest development version, use the following command:
-        
-        ```
-        pip install git+https://github.com/cbrnr/sleepecg
-        ```
-        
-        ### Contributing
-        The [contributing guide](https://github.com/cbrnr/sleepecg/blob/main/CONTRIBUTING.md) contains detailed instructions on how to contribute to SleepECG.
-        
+Author-email: Florian Hofer <hofaflo@gmail.com>, Clemens Brunner <clemens.brunner@gmail.com>
+License: BSD 3-Clause
+Project-URL: homepage, https://github.com/cbrnr/sleepecg
+Project-URL: documentation, https://sleepecg.readthedocs.io/en/latest/
+Project-URL: repository, https://github.com/cbrnr/sleepecg
+Project-URL: changelog, https://github.com/cbrnr/sleepecg/blob/main/CHANGELOG.md
 Keywords: sleep,ecg,qrs,peak
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: cibw
+License-File: LICENSE
+
+![Python](https://img.shields.io/pypi/pyversions/sleepecg.svg?logo=python&logoColor=white)
+[![PyPI](https://img.shields.io/pypi/v/sleepecg)](https://pypi.org/project/sleepecg/)
+[![conda-forge](https://img.shields.io/conda/v/conda-forge/sleepecg.svg?label=conda-forge)](https://anaconda.org/conda-forge/sleepecg)
+[![Docs](https://readthedocs.org/projects/sleepecg/badge/?version=latest)](https://sleepecg.readthedocs.io/en/stable/index.html)
+[![License](https://img.shields.io/github/license/cbrnr/sleepecg)](LICENSE)
+
+## SleepECG
+SleepECG provides tools for sleep stage classification when [EEG](https://en.wikipedia.org/wiki/Electroencephalography) signals are not available. Based only on [ECG](https://en.wikipedia.org/wiki/Electrocardiography), SleepECG provides functions for
+
+- downloading and reading open polysomnography datasets,
+- detecting heartbeats from ECG signals, and
+- classifying sleep stages (which includes preprocessing, feature extraction, and classification).
+
+### Documentation
+Documentation for SleepECG is available on [Read the Docs](https://sleepecg.readthedocs.io/en/stable/index.html).
+
+### Changelog
+Check out the [changelog](https://github.com/cbrnr/sleepecg/blob/main/CHANGELOG.md) to learn what we added, changed, or fixed.
+
+### Dependencies
+SleepECG requires Python ≥ 3.8 and the following packages:
+
+- [numpy](http://www.numpy.org/) ≥ 1.20.0
+- [requests](https://requests.readthedocs.io/en/latest/) ≥ 2.25.0
+- [scipy](https://scipy.org/) ≥ 1.7.0
+- [tqdm](https://tqdm.github.io/) ≥ 4.60.0
+- [PyYAML](https://pyyaml.org/) ≥ 5.4.0
+
+Optional dependencies provide additional features:
+
+- [joblib](https://joblib.readthedocs.io/en/latest/) ≥ 1.0.0 (parallelized feature extraction)
+- [matplotlib](https://matplotlib.org/) ≥ 3.5.0 (plot ECG time courses, hypnograms, and confusion matrices)
+- [mne](https://mne.tools/stable/index.html) ≥ 1.0.0 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
+- [numba](https://numba.pydata.org/) ≥ 0.55.0 (JIT-compiled heartbeat detector)
+- [tensorflow](https://www.tensorflow.org/) ≥ 2.7.0 (sleep stage classification with Keras models)
+- [wfdb](https://github.com/MIT-LCP/wfdb-python/) ≥ 3.4.0 (read data from [SLPDB](https://physionet.org/content/slpdb), [MITDB](https://physionet.org/content/mitdb), and [LTDB](https://physionet.org/content/ltdb))
+
+### Installation
+SleepECG is available on PyPI and can be installed with [pip](https://pip.pypa.io/en/stable/):
+
+```
+pip install sleepecg
+```
+
+Alternatively, an unofficial [conda](https://docs.conda.io/en/latest/) package is available:
+
+```
+conda install -c conda-forge sleepecg
+```
+
+SleepECG with all optional dependencies can be installed with the following command:
+
+```
+pip install "sleepecg[full]"
+```
+
+If you want the latest development version, use the following command:
+
+```
+pip install git+https://github.com/cbrnr/sleepecg
+```
+
+### Example
+The following example detects heartbeats in a short ECG (a one-dimensional NumPy array):
+
+```python
+import numpy as np
+from scipy.misc import electrocardiogram
+from sleepecg import detect_heartbeats
+
+ecg = electrocardiogram()  # 5 min of ECG data at 360 Hz
+fs = 360  # sampling frequency
+beats = detect_heartbeats(ecg, fs)  # indices of detected heartbeats
+```
+
+More examples are available at https://github.com/cbrnr/sleepecg/tree/main/examples.
+
+### Contributing
+The [contributing guide](https://github.com/cbrnr/sleepecg/blob/main/CONTRIBUTING.md) contains detailed instructions on how to contribute to SleepECG.
```

### Comparing `sleepecg-0.5.4/sleepecg.egg-info/SOURCES.txt` & `sleepecg-0.5.5/sleepecg.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 readthedocs.yml
-setup.cfg
 setup.py
 .github/workflows/release.yml
 .github/workflows/test.yml
 examples/README.md
 examples/feature_extraction.py
 examples/heartbeat_detection.py
 examples/try_ws_gru_mesa.py
```

