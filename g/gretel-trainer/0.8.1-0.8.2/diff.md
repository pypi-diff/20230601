# Comparing `tmp/gretel-trainer-0.8.1.tar.gz` & `tmp/gretel-trainer-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gretel-trainer-0.8.1.tar", last modified: Tue May 16 19:06:21 2023, max compression
+gzip compressed data, was "gretel-trainer-0.8.2.tar", last modified: Thu Jun  1 19:27:37 2023, max compression
```

## Comparing `gretel-trainer-0.8.1.tar` & `gretel-trainer-0.8.2.tar`

### file list

```diff
@@ -1,135 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.163708 gretel-trainer-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.147708 gretel-trainer-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.147708 gretel-trainer-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-16 19:06:21.159708 gretel-trainer-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)   108190 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/data/cpu_states.csv
--rw-r--r--   0 runner    (1001) docker     (123)   629637 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/data/mitre-synthea-health.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/img/gretel-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/img/gretel_logo_white.png
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/trainer.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/notebooks/benchmark.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/notebooks/conditional-generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/notebooks/custom-example.py
--rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/notebooks/relational.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/notebooks/simple-conditional-generation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/notebooks/simple-example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/notebooks/trainer-examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 19:06:21.163708 gretel-trainer-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.147708 gretel-trainer-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/src/gretel_trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/custom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/custom/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/custom/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.155708 gretel-trainer-0.8.1/src/gretel_trainer/relational/
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/ancestry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    40587 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/multi_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.155708 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/figures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/key_highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report.css
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report_privacy_protection.css
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report_synthetic_quality.css
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/sdk_extras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.155708 gretel-trainer-0.8.1/src/gretel_trainer/relational/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)    13577 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/strategies/ancestral.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/strategies/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/strategies/independent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/table_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/task_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.155708 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/synthetics_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/synthetics_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/synthetics_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/transforms_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/transforms_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    29826 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/src/gretel_trainer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-16 19:06:21.000000 gretel-trainer-0.8.1/src/gretel_trainer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-16 19:06:21.000000 gretel-trainer-0.8.1/src/gretel_trainer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:06:21.000000 gretel-trainer-0.8.1/src/gretel_trainer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-16 19:06:21.000000 gretel-trainer-0.8.1/src/gretel_trainer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 19:06:21.000000 gretel-trainer-0.8.1/src/gretel_trainer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.155708 gretel-trainer-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.155708 gretel-trainer-0.8.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  2927798 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/data/core-221-train.csv
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/example_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.159708 gretel-trainer-0.8.1/tests/relational/
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.159708 gretel-trainer-0.8.1/tests/relational/example_dbs/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/example_dbs/art.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/example_dbs/ecom.sql
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/example_dbs/mutagenesis.sql
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/example_dbs/pets.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/example_dbs/tpch.sql
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/example_dbs/trips.sql
--rw-r--r--   0 runner    (1001) docker     (123)    21122 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_ancestral_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_ancestry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_common_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_independent_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_multi_table_config_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    25290 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_multi_table_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_synthetics_run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_task_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/test_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.825153 gretel-trainer-0.8.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.809153 gretel-trainer-0.8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.809153 gretel-trainer-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-01 19:27:37.825153 gretel-trainer-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.809153 gretel-trainer-0.8.2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   108190 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/data/cpu_states.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   629637 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/data/mitre-synthea-health.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.809153 gretel-trainer-0.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.813153 gretel-trainer-0.8.2/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/img/gretel-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/img/gretel_logo_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/trainer.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.813153 gretel-trainer-0.8.2/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/notebooks/benchmark.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/notebooks/conditional-generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/notebooks/custom-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/notebooks/relational.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/notebooks/simple-conditional-generation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/notebooks/simple-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/notebooks/trainer-examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:27:37.825153 gretel-trainer-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.809153 gretel-trainer-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.813153 gretel-trainer-0.8.2/src/gretel_trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.813153 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.813153 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/custom/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/custom/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.813153 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.817153 gretel-trainer-0.8.2/src/gretel_trainer/relational/
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26448 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45200 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/multi_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.817153 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/figures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/key_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report_privacy_protection.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report_synthetic_quality.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/sdk_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.817153 gretel-trainer-0.8.2/src/gretel_trainer/relational/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/strategies/ancestral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/strategies/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/strategies/independent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/table_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/task_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.817153 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/synthetics_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/synthetics_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/synthetics_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/transforms_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/transforms_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29826 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.813153 gretel-trainer-0.8.2/src/gretel_trainer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-01 19:27:37.000000 gretel-trainer-0.8.2/src/gretel_trainer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-01 19:27:37.000000 gretel-trainer-0.8.2/src/gretel_trainer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:27:37.000000 gretel-trainer-0.8.2/src/gretel_trainer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-01 19:27:37.000000 gretel-trainer-0.8.2/src/gretel_trainer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 19:27:37.000000 gretel-trainer-0.8.2/src/gretel_trainer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.817153 gretel-trainer-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.817153 gretel-trainer-0.8.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2927798 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/data/core-221-train.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/example_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.821153 gretel-trainer-0.8.2/tests/relational/
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.825153 gretel-trainer-0.8.2/tests/relational/example_dbs/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/example_dbs/art.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/example_dbs/documents.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/example_dbs/ecom.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/example_dbs/mutagenesis.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/example_dbs/pets.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/example_dbs/tpch.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/example_dbs/trips.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    20868 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_ancestral_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_common_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_independent_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_multi_table_config_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25141 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_multi_table_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30649 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_relational_data_with_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_synthetics_run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_task_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_train_synthetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_train_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/test_strategy.py
```

### Comparing `gretel-trainer-0.8.1/.github/workflows/python-publish.yml` & `gretel-trainer-0.8.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/.gitignore` & `gretel-trainer-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/LICENSE` & `gretel-trainer-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/PKG-INFO` & `gretel-trainer-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gretel-trainer
-Version: 0.8.1
+Version: 0.8.2
 Summary: Synthetic Data Generation with optional Differential Privacy
 Home-page: https://github.com/gretelai/gretel-trainer
 License: https://gretel.ai/license/source-available-license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `gretel-trainer-0.8.1/README.md` & `gretel-trainer-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/data/cpu_states.csv` & `gretel-trainer-0.8.2/data/cpu_states.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/data/mitre-synthea-health.csv` & `gretel-trainer-0.8.2/data/mitre-synthea-health.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/docs/Makefile` & `gretel-trainer-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/docs/conf.py` & `gretel-trainer-0.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/docs/img/gretel-logo.png` & `gretel-trainer-0.8.2/docs/img/gretel-logo.png`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/docs/img/gretel_logo_white.png` & `gretel-trainer-0.8.2/docs/img/gretel_logo_white.png`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/docs/index.rst` & `gretel-trainer-0.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/docs/make.bat` & `gretel-trainer-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/docs/quickstart.rst` & `gretel-trainer-0.8.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/notebooks/benchmark.ipynb` & `gretel-trainer-0.8.2/notebooks/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/notebooks/conditional-generation.py` & `gretel-trainer-0.8.2/notebooks/conditional-generation.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/notebooks/custom-example.py` & `gretel-trainer-0.8.2/notebooks/custom-example.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/notebooks/relational.ipynb` & `gretel-trainer-0.8.2/notebooks/relational.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9937530468918336%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 3: {'source': "*

 * *            "{insert: [(12, 'mt.train_synthetics()\\n')], delete: [12]}}, 4: {'attachments': "*

 * *            "OrderedDict()}, 18: {'source': {insert: [(2, 'Train Gretel Transforms models by "*

 * *            'providing a transforms model config. By default this config will be applied to all '*

 * *            'tables. You can limit the tables being transformed via the optional `only` (tables to '*

 * *            "include) o […]*

```diff
@@ -1,18 +1,20 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Gretel Relational\n",
                 "Synthetics and Transforms for relational data."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Quickstart"
             ]
         },
         {
@@ -40,21 +42,22 @@
                 "!curl -o \"ecom_xf.db\" \"https://gretel-blueprints-pub.s3.us-west-2.amazonaws.com/rdb/ecom_xf.db\"\n",
                 "\n",
                 "\n",
                 "connector = sqlite_conn(\"ecom_xf.db\")\n",
                 "relational_data = connector.extract()\n",
                 "\n",
                 "mt = MultiTable(relational_data)\n",
-                "mt.train()\n",
+                "mt.train_synthetics()\n",
                 "mt.generate()\n",
                 "\n",
                 "connector.save(mt.synthetic_output_tables, prefix=\"synthetic_\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Detailed walkthrough"
             ]
         },
         {
@@ -298,31 +301,32 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Transforms\n",
                 "\n",
-                "Train Gretel Transforms models by providing table-specific model configs. You only need to train models for tables you want to transform\u2014you do not need to supply a config for every table."
+                "Train Gretel Transforms models by providing a transforms model config. By default this config will be applied to all tables. You can limit the tables being transformed via the optional `only` (tables to include) or `ignore` (tables to exclude) arguments."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Transform some tables\n",
+                "config = \"https://raw.githubusercontent.com/gretelai/gdpr-helpers/main/src/config/transforms_config.yaml\"\n",
                 "\n",
-                "multitable.train_transform_models(\n",
-                "    configs={\n",
-                "        \"users\": \"https://gretel-blueprints-pub.s3.amazonaws.com/rdb/users_policy.yaml\",\n",
-                "        \"events\": \"https://gretel-blueprints-pub.s3.amazonaws.com/rdb/events_policy.yaml\",\n",
-                "    }\n",
-                ")"
+                "multitable.train_transforms(config)\n",
+                "\n",
+                "# Optionally limit which tables are trained for transforms via `only` (included) or `ignore` (excluded).\n",
+                "# Given our example data, the two calls below will lead to the same tables getting trained, just specified different ways.\n",
+                "#\n",
+                "# multitable.train_transforms(config, ignore={\"distribution_center\", \"products\"})\n",
+                "# multitable.train_transforms(config, only={\"users\", \"events\", \"inventory_items\", \"order_items\"})"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -370,22 +374,36 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Synthetics"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Start by training models for synthetics. By default, a synthetics model will be trained for every table in the `RelationalData`. However, this scope can be reduced to a subset of tables using the optional `only` (tables to include) or `ignore` (tables to exclude) arguments. This can be particularly useful if certain tables contain static reference data that should not be synthesized."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Train synthetic models for all tables\n",
                 "\n",
-                "multitable.train()"
+                "multitable.train_synthetics()\n",
+                "\n",
+                "# Optionally limit which tables are trained for synthetics via `only` (included) or `ignore` (excluded).\n",
+                "# Given our example data, the two calls below will lead to the same tables getting trained, just specified different ways.\n",
+                "#\n",
+                "# multitable.train_synthetics(ignore={\"distribution_center\", \"products\"})\n",
+                "# multitable.train_synthetics(only={\"users\", \"events\", \"inventory_items\", \"order_items\"})"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -406,15 +424,15 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Each synthetic data generation run is assigned (or supplied) a unique identifier. Look for a subdirectory with this identifier name in the working directory to find all synthetic outputs, including data and reports. An archive file containing all runs' outputs is also uploaded to the Gretel project as a project artifact, visible in the Data Sources tab in the Console.\n",
                 "\n",
-                "When you generate synthetic data, you can optionally change the amount of data to generate via `record_size_ratio`, as well as optionally preserve certain tables' source data via `preserve_tables`."
+                "When you generate synthetic data, you can optionally change the amount of data to generate via `record_size_ratio`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -423,18 +441,15 @@
                 "\n",
                 "multitable.generate()\n",
                 "\n",
                 "# Provide a specific identifier for the run (default is `synthetics_{timestamp}`)\n",
                 "# multitable.generate(identifier=\"my-synthetics-run\")\n",
                 "\n",
                 "# Generate twice as much synthetic data\n",
-                "# multitable.generate(record_size_ratio=2.0)\n",
-                "\n",
-                "# Treat certain tables as static reference data that should not be synthesized\n",
-                "# multitable.generate(preserve_tables=[\"distribution_center\"])"
+                "# multitable.generate(record_size_ratio=2.0)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `gretel-trainer-0.8.1/notebooks/simple-conditional-generation.ipynb` & `gretel-trainer-0.8.2/notebooks/simple-conditional-generation.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/notebooks/trainer-examples.ipynb` & `gretel-trainer-0.8.2/notebooks/trainer-examples.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/setup.py` & `gretel-trainer-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/__init__.py` & `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/compare.py` & `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/compare.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/core.py` & `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/core.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/custom/datasets.py` & `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/custom/datasets.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/custom/executor.py` & `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/custom/executor.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/datasets.py` & `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/datasets.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/executor.py` & `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/executor.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/models.py` & `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/models.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/sdk.py` & `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/sdk.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/models.py` & `gretel-trainer-0.8.2/src/gretel_trainer/models.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/README.md` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/README.md`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/ancestry.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/ancestry.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 import re
-from typing import Dict, List, Optional, Tuple
+from typing import Optional
 
 import pandas as pd
 
 from gretel_trainer.relational.core import ForeignKey, RelationalData
 
 _START_LINEAGE = "self"
 _GEN_DELIMITER = "."
 _COL_DELIMITER = "+"
 _END_LINEAGE = "|"
 
 
 def get_multigenerational_primary_key(
     rel_data: RelationalData, table: str
-) -> List[str]:
+) -> list[str]:
+    "Returns the provided table's primary key with the ancestral lineage prefix appended"
     return [
         f"{_START_LINEAGE}{_END_LINEAGE}{pk}" for pk in rel_data.get_primary_key(table)
     ]
 
 
 def get_ancestral_foreign_key_maps(
     rel_data: RelationalData, table: str
-) -> List[Tuple[str, str]]:
-    def _ancestral_fk_map(fk: ForeignKey) -> List[Tuple[str, str]]:
+) -> list[tuple[str, str]]:
+    """
+    Returns a list of two-element tuples where the first element is a foreign key column
+    with ancestral lineage prefix, and the second element is the ancestral-lineage-prefixed
+    referred column. This function ultimately provides a list of which columns are duplicates
+    in a fully-joined ancestral table (i.e. `get_table_data_with_ancestors`) (only between
+    the provided table and its direct parents, not between parents and grandparents).
+
+    For example: given an events table with foreign key `events.user_id` => `users.id`,
+    this method returns: [("self|user_id", "self.user_id|id")]
+    """
+
+    def _ancestral_fk_map(fk: ForeignKey) -> list[tuple[str, str]]:
         maps = []
         fk_lineage = _COL_DELIMITER.join(fk.columns)
 
         for i in range(len(fk.columns)):
             fk_col = fk.columns[i]
             ref_col = fk.parent_columns[i]
 
@@ -42,18 +54,41 @@
     return [
         fkmap
         for fk in rel_data.get_foreign_keys(table)
         for fkmap in _ancestral_fk_map(fk)
     ]
 
 
+def get_seed_safe_multigenerational_columns(
+    rel_data: RelationalData,
+) -> dict[str, list[str]]:
+    """
+    Returns a dict with Scope.MODELABLE table names as keys and lists of columns to use
+    for conditional seeding as values. By using a tableset of empty dataframes, this provides
+    a significantly faster / less resource-intensive way to get just the column names
+    from the results of `get_table_data_with_ancestors` for all tables.
+    """
+    tableset = {
+        table: pd.DataFrame(columns=list(rel_data.get_table_columns(table)))
+        for table in rel_data.list_all_tables()
+    }
+    return {
+        table: list(
+            get_table_data_with_ancestors(
+                rel_data, table, tableset, ancestral_seeding=True
+            ).columns
+        )
+        for table in rel_data.list_all_tables()
+    }
+
+
 def get_table_data_with_ancestors(
     rel_data: RelationalData,
     table: str,
-    tableset: Optional[Dict[str, pd.DataFrame]] = None,
+    tableset: Optional[dict[str, pd.DataFrame]] = None,
     ancestral_seeding: bool = False,
 ) -> pd.DataFrame:
     """
     Returns a data frame with all ancestral data joined to each record.
     Column names are modified to the format `LINAGE|COLUMN_NAME`.
     Lineage begins with `self` for the supplied `table`, and as older
     generations are joined, the foreign keys to those generations are appended,
@@ -71,15 +106,15 @@
 
 
 def _join_parents(
     rel_data: RelationalData,
     df: pd.DataFrame,
     table: str,
     lineage: str,
-    tableset: Optional[Dict[str, pd.DataFrame]],
+    tableset: Optional[dict[str, pd.DataFrame]],
     ancestral_seeding: bool,
 ) -> pd.DataFrame:
     for foreign_key in rel_data.get_foreign_keys(table):
         fk_lineage = _COL_DELIMITER.join(foreign_key.columns)
         next_lineage = f"{lineage}{_GEN_DELIMITER}{fk_lineage}"
 
         parent_table_name = foreign_key.parent_table_name
@@ -89,18 +124,17 @@
         else:
             usecols = rel_data.get_table_columns(parent_table_name)
 
         if tableset is not None:
             parent_data = tableset[parent_table_name][list(usecols)]
         else:
             parent_data = rel_data.get_table_data(parent_table_name, usecols=usecols)
-        parent_data = parent_data.add_prefix(f"{next_lineage}{_END_LINEAGE}")
 
         df = df.merge(
-            parent_data,
+            parent_data.add_prefix(f"{next_lineage}{_END_LINEAGE}"),
             how="left",
             left_on=[f"{lineage}{_END_LINEAGE}{col}" for col in foreign_key.columns],
             right_on=[
                 f"{next_lineage}{_END_LINEAGE}{parent_col}"
                 for parent_col in foreign_key.parent_columns
             ],
         )
@@ -130,15 +164,15 @@
     ]
     mapper = {
         col: col.removeprefix(f"{_START_LINEAGE}{_END_LINEAGE}") for col in root_columns
     }
     return df[root_columns].rename(columns=mapper)
 
 
-def prepend_foreign_key_lineage(df: pd.DataFrame, fk_cols: List[str]) -> pd.DataFrame:
+def prepend_foreign_key_lineage(df: pd.DataFrame, fk_cols: list[str]) -> pd.DataFrame:
     """
     Given a multigenerational dataframe, renames all columns such that the provided
     foreign key columns act as the lineage from some child table to the provided data.
     The resulting column names are elder-generation ancestral column names from the
     perspective of a child table that relates to that parent via the provided foreign key.
     """
     fk_lineage = _COL_DELIMITER.join(fk_cols)
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/artifacts.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/artifacts.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/backup.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/backup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,109 @@
 from __future__ import annotations
 
 from dataclasses import asdict, dataclass
-from typing import Any, Dict, List, Optional
+from typing import Any, Optional
 
 from gretel_trainer.relational.artifacts import ArtifactCollection
 from gretel_trainer.relational.core import ForeignKey, RelationalData
 
 
 @dataclass
 class BackupRelationalDataTable:
-    primary_key: List[str]
+    primary_key: list[str]
+    invented_table_metadata: Optional[dict[str, Any]] = None
 
 
 @dataclass
 class BackupForeignKey:
     table: str
-    constrained_columns: List[str]
+    constrained_columns: list[str]
     referred_table: str
-    referred_columns: List[str]
+    referred_columns: list[str]
 
     @classmethod
     def from_fk(cls, fk: ForeignKey) -> BackupForeignKey:
         return BackupForeignKey(
             table=fk.table_name,
             constrained_columns=fk.columns,
             referred_table=fk.parent_table_name,
             referred_columns=fk.parent_columns,
         )
 
 
 @dataclass
+class BackupRelationalJson:
+    original_table_name: str
+    original_primary_key: list[str]
+    original_columns: list[str]
+    table_name_mappings: dict[str, str]
+
+
+@dataclass
 class BackupRelationalData:
-    tables: Dict[str, BackupRelationalDataTable]
-    foreign_keys: List[BackupForeignKey]
+    tables: dict[str, BackupRelationalDataTable]
+    foreign_keys: list[BackupForeignKey]
+    relational_jsons: dict[str, BackupRelationalJson]
 
     @classmethod
     def from_relational_data(cls, rel_data: RelationalData) -> BackupRelationalData:
         tables = {}
         foreign_keys = []
+        relational_jsons = {}
         for table in rel_data.list_all_tables():
-            tables[table] = BackupRelationalDataTable(
+            backup_table = BackupRelationalDataTable(
                 primary_key=rel_data.get_primary_key(table),
             )
+            if (
+                invented_table_metadata := rel_data.get_invented_table_metadata(table)
+            ) is not None:
+                backup_table.invented_table_metadata = asdict(invented_table_metadata)
+            tables[table] = backup_table
             foreign_keys.extend(
                 [
                     BackupForeignKey.from_fk(key)
                     for key in rel_data.get_foreign_keys(table)
                 ]
             )
-        return BackupRelationalData(tables=tables, foreign_keys=foreign_keys)
+        for key, rel_json in rel_data.relational_jsons.items():
+            relational_jsons[key] = BackupRelationalJson(
+                original_table_name=rel_json.original_table_name,
+                original_primary_key=rel_json.original_primary_key,
+                original_columns=rel_json.original_columns,
+                table_name_mappings=rel_json.table_name_mappings,
+            )
+        return BackupRelationalData(
+            tables=tables, foreign_keys=foreign_keys, relational_jsons=relational_jsons
+        )
 
 
 @dataclass
 class BackupClassify:
-    model_ids: Dict[str, str]
+    model_ids: dict[str, str]
 
 
 @dataclass
 class BackupTransformsTrain:
-    model_ids: Dict[str, str]
-    lost_contact: List[str]
+    model_ids: dict[str, str]
+    lost_contact: list[str]
 
 
 @dataclass
 class BackupSyntheticsTrain:
-    model_ids: Dict[str, str]
-    lost_contact: List[str]
-    training_columns: Dict[str, List[str]]
+    model_ids: dict[str, str]
+    lost_contact: list[str]
 
 
 @dataclass
 class BackupGenerate:
     identifier: str
-    preserved: List[str]
+    preserved: list[str]
     record_size_ratio: float
-    record_handler_ids: Dict[str, str]
-    lost_contact: List[str]
-    missing_model: List[str]
+    record_handler_ids: dict[str, str]
+    lost_contact: list[str]
 
 
 @dataclass
 class Backup:
     project_name: str
     strategy: str
     gretel_model: str
@@ -94,15 +117,15 @@
     generate: Optional[BackupGenerate] = None
 
     @property
     def as_dict(self):
         return asdict(self)
 
     @classmethod
-    def from_dict(cls, b: Dict[str, Any]):
+    def from_dict(cls, b: dict[str, Any]):
         relational_data = b["relational_data"]
         brd = BackupRelationalData(
             tables={
                 k: BackupRelationalDataTable(**v)
                 for k, v in relational_data.get("tables", {}).items()
             },
             foreign_keys=[
@@ -110,14 +133,18 @@
                     table=fk["table"],
                     constrained_columns=fk["constrained_columns"],
                     referred_table=fk["referred_table"],
                     referred_columns=fk["referred_columns"],
                 )
                 for fk in relational_data.get("foreign_keys", [])
             ],
+            relational_jsons={
+                k: BackupRelationalJson(**v)
+                for k, v in relational_data.get("relational_jsons", {}).items()
+            },
         )
 
         backup = Backup(
             project_name=b["project_name"],
             strategy=b["strategy"],
             gretel_model=b["gretel_model"],
             working_dir=b["working_dir"],
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/connectors.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/connectors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import logging
-from typing import Dict, List, Optional, Tuple
+from typing import Optional
 
 import pandas as pd
 from sqlalchemy import create_engine, inspect
 from sqlalchemy.engine.base import Engine
 from sqlalchemy.exc import OperationalError
 
-from gretel_trainer.relational.core import MultiTableException, RelationalData
+from gretel_trainer.relational.core import (
+    MultiTableException,
+    RelationalData,
+    skip_table,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class Connector:
     """
     Wraps connections to relational databases and backups.
@@ -34,37 +38,42 @@
             self.engine.connect()
         except OperationalError as e:
             logger.error(f"{e}, {e.__cause__}")
             raise e
         logger.info("Successfully connected to db")
 
     def extract(
-        self, only: Optional[List[str]] = None, ignore: Optional[List[str]] = None
+        self,
+        only: Optional[set[str]] = None,
+        ignore: Optional[set[str]] = None,
+        schema: Optional[str] = None,
     ) -> RelationalData:
         """
-        Extracts table data and relationships from the database.
-        To scope to a subset of a database, use either `only` (inclusive) or `ignore` (exclusive).
+        Extracts table data and relationships from the database. Optional args include:
+        - `only` (restrict extraction to these tables; cannot be used with `ignore`)
+        - `ignore` (exclude these tables from extraction; cannot be used with `only`)
+        - `schema` (limit scope to a specific schema; this is dialect-specific and not supported by all databases)
         """
         if only is not None and ignore is not None:
             raise MultiTableException("Cannot specify both `only` and `ignore`.")
 
         inspector = inspect(self.engine)
 
         relational_data = RelationalData()
-        foreign_keys: List[Tuple[str, dict]] = []
+        foreign_keys: list[tuple[str, dict]] = []
 
-        for table_name in inspector.get_table_names():
-            if _skip_table(table_name, only, ignore):
+        for table_name in inspector.get_table_names(schema=schema):
+            if skip_table(table_name, only, ignore):
                 continue
 
             logger.debug(f"Extracting source data from `{table_name}`")
-            df = pd.read_sql_table(table_name, self.engine)
+            df = pd.read_sql_table(table_name, self.engine, schema=schema)
             primary_key = inspector.get_pk_constraint(table_name)["constrained_columns"]
             for fk in inspector.get_foreign_keys(table_name):
-                if _skip_table(fk["referred_table"], only, ignore):
+                if skip_table(fk["referred_table"], only, ignore):
                     continue
                 else:
                     foreign_keys.append((table_name, fk))
 
             relational_data.add_table(name=table_name, primary_key=primary_key, data=df)
 
         for foreign_key in foreign_keys:
@@ -74,33 +83,21 @@
                 constrained_columns=fk["constrained_columns"],
                 referred_table=fk["referred_table"],
                 referred_columns=fk["referred_columns"],
             )
 
         return relational_data
 
-    def save(self, tables: Dict[str, pd.DataFrame], prefix: str = "") -> None:
+    def save(self, tables: dict[str, pd.DataFrame], prefix: str = "") -> None:
         for name, data in tables.items():
             data.to_sql(
                 f"{prefix}{name}", con=self.engine, if_exists="replace", index=False
             )
 
 
-def _skip_table(
-    table: str, only: Optional[List[str]], ignore: Optional[List[str]]
-) -> bool:
-    skip = False
-    if only is not None and table not in only:
-        skip = True
-    if ignore is not None and table in ignore:
-        skip = True
-
-    return skip
-
-
 def sqlite_conn(path: str) -> Connector:
     engine = create_engine(f"sqlite:///{path}")
     return Connector(engine)
 
 
 def postgres_conn(
     *, user: str, password: str, host: str, port: int, database: str
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/log.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/log.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 
 # Clear out any existing root handlers
 # (This prevents duplicate log output in Colab)
 for root_handler in logging.root.handlers:
     logging.root.removeHandler(root_handler)
 
 
+def set_log_level(level: str):
+    logger = logging.getLogger(RELATIONAL)
+    logger.setLevel(level)
+
+
 @contextmanager
 def silent_logs():
     logger = logging.getLogger(RELATIONAL)
     current_level = logger.getEffectiveLevel()
     logger.setLevel("CRITICAL")
     try:
         yield
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/model_config.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/model_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 from copy import deepcopy
-from typing import Any, Dict, List
+from typing import Any
 
 from gretel_client.projects.models import read_model_config
 
 from gretel_trainer.relational.core import (
     GretelModelConfig,
     MultiTableException,
     RelationalData,
 )
 
 
-def _ingest(config: GretelModelConfig) -> Dict[str, Any]:
+def _ingest(config: GretelModelConfig) -> dict[str, Any]:
     return read_model_config(deepcopy(config))
 
 
 def _model_name(workflow: str, table: str) -> str:
     ok_table_name = table.replace("--", "__")
     return f"{workflow}-{ok_table_name}"
 
 
-def make_classify_config(table: str, config: GretelModelConfig) -> Dict[str, Any]:
+def make_classify_config(table: str, config: GretelModelConfig) -> dict[str, Any]:
     tailored_config = _ingest(config)
     tailored_config["name"] = _model_name("classify", table)
     return tailored_config
 
 
-def make_evaluate_config(table: str) -> Dict[str, Any]:
+def make_evaluate_config(table: str) -> dict[str, Any]:
     tailored_config = _ingest("evaluate/default")
     tailored_config["name"] = _model_name("evaluate", table)
     return tailored_config
 
 
-def make_synthetics_config(table: str, config: GretelModelConfig) -> Dict[str, Any]:
+def make_synthetics_config(table: str, config: GretelModelConfig) -> dict[str, Any]:
     tailored_config = _ingest(config)
     tailored_config["name"] = _model_name("synthetics", table)
     return tailored_config
 
 
 def make_transform_config(
     rel_data: RelationalData, table: str, config: GretelModelConfig
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     tailored_config = _ingest(config)
     tailored_config["name"] = _model_name("transforms", table)
 
     key_columns = rel_data.get_all_key_columns(table)
     if len(key_columns) > 0:
         try:
             model = tailored_config["models"][0]
@@ -61,15 +61,15 @@
         adjusted_policies = [passthrough_policy] + policies
 
         tailored_config["models"][0][model_key]["policies"] = adjusted_policies
 
     return tailored_config
 
 
-def _passthrough_policy(columns: List[str]) -> Dict[str, Any]:
+def _passthrough_policy(columns: list[str]) -> dict[str, Any]:
     return {
         "name": "ignore-keys",
         "rules": [
             {
                 "name": "ignore-key-columns",
                 "conditions": {"field_name": columns},
                 "transforms": [
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/multi_table.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/multi_table.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import shutil
 import tarfile
 from collections import defaultdict
 from contextlib import suppress
 from dataclasses import replace
 from datetime import datetime
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Optional, Union
 
 import pandas as pd
 import smart_open
 from gretel_client.config import RunnerMode, get_session_config
 from gretel_client.projects import Project, create_project, get_project
 from gretel_client.projects.jobs import ACTIVE_STATES, END_STATES, Status
 from gretel_client.projects.records import RecordHandler
@@ -28,15 +28,18 @@
     BackupSyntheticsTrain,
     BackupTransformsTrain,
 )
 from gretel_trainer.relational.core import (
     GretelModelConfig,
     MultiTableException,
     RelationalData,
+    Scope,
+    skip_table,
 )
+from gretel_trainer.relational.json import InventedTableMetadata, RelationalJson
 from gretel_trainer.relational.log import silent_logs
 from gretel_trainer.relational.model_config import (
     make_classify_config,
     make_evaluate_config,
     make_synthetics_config,
     make_transform_config,
 )
@@ -94,19 +97,19 @@
         self._set_refresh_interval(refresh_interval)
         self.relational_data = relational_data
         self._artifact_collection = ArtifactCollection(hybrid=self._hybrid)
         self._extended_sdk = ExtendedGretelSDK(hybrid=self._hybrid)
         self._latest_backup: Optional[Backup] = None
         self._classify = Classify()
         self._transforms_train = TransformsTrain()
-        self.transform_output_tables: Dict[str, pd.DataFrame] = {}
+        self.transform_output_tables: dict[str, pd.DataFrame] = {}
         self._synthetics_train = SyntheticsTrain()
         self._synthetics_run: Optional[SyntheticsRun] = None
-        self.synthetic_output_tables: Dict[str, pd.DataFrame] = {}
-        self.evaluations = defaultdict(lambda: TableEvaluation())
+        self.synthetic_output_tables: dict[str, pd.DataFrame] = {}
+        self._evaluations = defaultdict(lambda: TableEvaluation())
 
         if backup is None:
             self._complete_fresh_init(project_display_name)
         else:
             self._complete_init_from_backup(backup)
 
     def _complete_fresh_init(self, project_display_name: Optional[str]) -> None:
@@ -142,24 +145,43 @@
             raise MultiTableException(
                 "Cannot restore from backup: source archive is missing."
             )
         with tarfile.open(source_archive_path, "r:gz") as tar:
             tar.extractall(path=self._working_dir)
         for table_name, table_backup in backup.relational_data.tables.items():
             source_data = pd.read_csv(self._working_dir / f"source_{table_name}.csv")
-            self.relational_data.add_table(
-                name=table_name, primary_key=table_backup.primary_key, data=source_data
+            invented_table_metadata = None
+            if (imeta := table_backup.invented_table_metadata) is not None:
+                invented_table_metadata = InventedTableMetadata(
+                    invented_root_table_name=imeta["invented_root_table_name"],
+                    original_table_name=imeta["original_table_name"],
+                    empty=imeta["empty"],
+                )
+            self.relational_data._add_single_table(
+                name=table_name,
+                primary_key=table_backup.primary_key,
+                data=source_data,
+                invented_table_metadata=invented_table_metadata,
             )
         for fk_backup in backup.relational_data.foreign_keys:
             self.relational_data.add_foreign_key_constraint(
                 table=fk_backup.table,
                 constrained_columns=fk_backup.constrained_columns,
                 referred_table=fk_backup.referred_table,
                 referred_columns=fk_backup.referred_columns,
             )
+        for key, rel_json_backup in backup.relational_data.relational_jsons.items():
+            relational_json = RelationalJson(
+                original_table_name=rel_json_backup.original_table_name,
+                original_primary_key=rel_json_backup.original_primary_key,
+                original_columns=rel_json_backup.original_columns,
+                original_data=None,
+                table_name_mappings=rel_json_backup.table_name_mappings,
+            )
+            self.relational_data.relational_jsons[key] = relational_json
 
         # Debug summary
         debug_summary_id = backup.artifact_collection.gretel_debug_summary
         if debug_summary_id is not None:
             self._extended_sdk.download_file_artifact(
                 self._project,
                 debug_summary_id,
@@ -226,17 +248,14 @@
                 synthetics_training_archive_id,
                 synthetics_training_archive_path,
             )
         if synthetics_training_archive_path.exists():
             with tarfile.open(synthetics_training_archive_path, "r:gz") as tar:
                 tar.extractall(path=self._working_dir)
 
-        self._synthetics_train.training_columns = (
-            backup_synthetics_train.training_columns
-        )
         self._synthetics_train.lost_contact = backup_synthetics_train.lost_contact
         self._synthetics_train.models = {
             table: self._project.get_model(model_id)
             for table, model_id in backup_synthetics_train.model_ids.items()
         }
 
         still_in_progress = [
@@ -254,23 +273,24 @@
 
         training_succeeded = [
             table
             for table, model in self._synthetics_train.models.items()
             if model.status == Status.COMPLETED
         ]
         for table in training_succeeded:
-            model = self._synthetics_train.models[table]
-            with silent_logs():
-                self._strategy.update_evaluation_from_model(
-                    table,
-                    self.evaluations,
-                    model,
-                    self._working_dir,
-                    self._extended_sdk,
-                )
+            if table in self.relational_data.list_all_tables(Scope.EVALUATABLE):
+                model = self._synthetics_train.models[table]
+                with silent_logs():
+                    self._strategy.update_evaluation_from_model(
+                        table,
+                        self._evaluations,
+                        model,
+                        self._working_dir,
+                        self._extended_sdk,
+                    )
 
         training_failed = [
             table
             for table, model in self._synthetics_train.models.items()
             if model.status in END_STATES and table not in training_succeeded
         ]
         if len(training_failed) > 0:
@@ -313,15 +333,14 @@
             table: self._synthetics_train.models[table].get_record_handler(rh_id)
             for table, rh_id in backup_generate.record_handler_ids.items()
         }
         self._synthetics_run = SyntheticsRun(
             identifier=backup_generate.identifier,
             record_size_ratio=backup_generate.record_size_ratio,
             preserved=backup_generate.preserved,
-            missing_model=backup_generate.missing_model,
             lost_contact=backup_generate.lost_contact,
             record_handlers=record_handlers,
         )
 
         latest_run_id = self._synthetics_run.identifier
         if latest_run_id in os.listdir(self._working_dir):
             # Latest backup was taken at a stable point (nothing actively in progress).
@@ -432,37 +451,45 @@
         if len(self._synthetics_train.models) > 0:
             backup.synthetics_train = BackupSyntheticsTrain(
                 model_ids={
                     table: model.model_id
                     for table, model in self._synthetics_train.models.items()
                 },
                 lost_contact=self._synthetics_train.lost_contact,
-                training_columns=self._synthetics_train.training_columns,
             )
 
         # Generate
         if self._synthetics_run is not None:
             backup.generate = BackupGenerate(
                 identifier=self._synthetics_run.identifier,
                 record_size_ratio=self._synthetics_run.record_size_ratio,
                 preserved=self._synthetics_run.preserved,
-                missing_model=self._synthetics_run.missing_model,
                 lost_contact=self._synthetics_run.lost_contact,
                 record_handler_ids={
                     table: rh.record_id
                     for table, rh in self._synthetics_run.record_handlers.items()
                 },
             )
 
         return backup
 
     @property
     def _hybrid(self) -> bool:
         return get_session_config().default_runner == RunnerMode.HYBRID
 
+    @property
+    def evaluations(self) -> dict[str, TableEvaluation]:
+        evaluations = defaultdict(lambda: TableEvaluation())
+
+        for table, evaluation in self._evaluations.items():
+            if (public_name := self.relational_data.get_public_name(table)) is not None:
+                evaluations[public_name] = evaluation
+
+        return evaluations
+
     def _set_refresh_interval(self, interval: Optional[int]) -> None:
         if interval is None:
             self._refresh_interval = 60
         else:
             if interval < 30:
                 logger.warning(
                     "Refresh interval must be at least 30 seconds. Setting to 30."
@@ -521,15 +548,17 @@
         archive_path = self._working_dir / "classify_outputs.tar.gz"
         for arcname, path in task.result_filepaths.items():
             add_to_tar(archive_path, path, arcname)
         self._artifact_collection.upload_classify_outputs_archive(
             self._project, str(archive_path)
         )
 
-    def train_transform_models(self, configs: Dict[str, GretelModelConfig]) -> None:
+    def _setup_transforms_train_state(
+        self, configs: dict[str, GretelModelConfig]
+    ) -> None:
         for table, config in configs.items():
             transform_config = make_transform_config(
                 self.relational_data, table, config
             )
 
             # Ensure consistent, friendly data source names in Console
             table_data = self.relational_data.get_table_data(table)
@@ -540,25 +569,61 @@
             model = self._project.create_model_obj(
                 model_config=transform_config, data_source=str(transforms_train_path)
             )
             self._transforms_train.models[table] = model
 
         self._backup()
 
+    def train_transform_models(self, configs: dict[str, GretelModelConfig]) -> None:
+        """
+        DEPRECATED: Please use `train_transforms` instead.
+        """
+        logger.warning(
+            "This method is deprecated and will be removed in a future release. "
+            "Please use `train_transforms` instead."
+        )
+        use_configs = {}
+        for table, config in configs.items():
+            for m_table in self.relational_data.get_modelable_table_names(table):
+                use_configs[m_table] = config
+
+        self._setup_transforms_train_state(use_configs)
+        task = TransformsTrainTask(
+            transforms_train=self._transforms_train,
+            multitable=self,
+        )
+        run_task(task, self._extended_sdk)
+
+    def train_transforms(
+        self,
+        config: GretelModelConfig,
+        *,
+        only: Optional[set[str]] = None,
+        ignore: Optional[set[str]] = None,
+    ) -> None:
+        only, ignore = self._get_only_and_ignore(only, ignore)
+
+        configs = {
+            table: config
+            for table in self.relational_data.list_all_tables()
+            if not skip_table(table, only, ignore)
+        }
+
+        self._setup_transforms_train_state(configs)
         task = TransformsTrainTask(
             transforms_train=self._transforms_train,
             multitable=self,
         )
         run_task(task, self._extended_sdk)
 
     def run_transforms(
         self,
         identifier: Optional[str] = None,
         in_place: bool = False,
-        data: Optional[Dict[str, pd.DataFrame]] = None,
+        data: Optional[dict[str, pd.DataFrame]] = None,
     ) -> None:
         """
         identifier: (str, optional): Unique string identifying a specific call to this method. Defaults to "transforms_" + current timestamp
 
         If `in_place` set to True, overwrites source data in all locations
         (internal Python state, local working directory, project artifact archive).
         Used for transforms->synthetics workflows.
@@ -589,15 +654,15 @@
         }
 
         for table, df in data.items():
             transforms_run_path = run_dir / f"transforms_input_{table}.csv"
             df.to_csv(transforms_run_path, index=False)
             transforms_run_paths[table] = transforms_run_path
 
-        transforms_record_handlers: Dict[str, RecordHandler] = {}
+        transforms_record_handlers: dict[str, RecordHandler] = {}
 
         for table_name, transforms_run_path in transforms_run_paths.items():
             model = self._transforms_train.models[table_name]
             record_handler = model.create_record_handler_obj(
                 data_source=str(transforms_run_path)
             )
             transforms_record_handlers[table_name] = record_handler
@@ -613,85 +678,148 @@
         )
 
         if in_place:
             for table_name, transformed_table in output_tables.items():
                 self.relational_data.update_table_data(table_name, transformed_table)
             self._upload_sources_to_project()
 
-        for table, df in output_tables.items():
+        reshaped_tables = self.relational_data.restore(output_tables)
+
+        for table, df in reshaped_tables.items():
             filename = f"transformed_{table}.csv"
             out_path = run_dir / filename
             df.to_csv(out_path, index=False)
 
         archive_path = self._working_dir / "transforms_outputs.tar.gz"
         add_to_tar(archive_path, run_dir, identifier)
 
         self._artifact_collection.upload_transforms_outputs_archive(
             self._project, str(archive_path)
         )
         self._backup()
-        self.transform_output_tables = output_tables
+        self.transform_output_tables = reshaped_tables
+
+    def _get_only_and_ignore(
+        self, only: Optional[set[str]], ignore: Optional[set[str]]
+    ) -> tuple[Optional[set[str]], Optional[set[str]]]:
+        if only is not None and ignore is not None:
+            raise MultiTableException("Cannot specify both `only` and `ignore`.")
+
+        modelable_tables = set()
+        for table in only or ignore or {}:
+            m_names = self.relational_data.get_modelable_table_names(table)
+            if len(m_names) == 0:
+                raise MultiTableException(f"Unrecognized table name: `{table}`")
+            modelable_tables.update(m_names)
+
+        if only is None:
+            return (None, modelable_tables)
+        elif ignore is None:
+            return (modelable_tables, None)
+        else:
+            return (None, None)
 
-    def _prepare_training_data(self, tables: List[str]) -> Dict[str, Path]:
+    def _prepare_training_data(self, tables: list[str]) -> dict[str, Path]:
         """
         Exports a copy of each table prepared for training by the configured strategy
         to the working directory. Returns a dict with table names as keys and Paths
         to the CSVs as values.
         """
-        training_data = self._strategy.prepare_training_data(self.relational_data)
-        for table, df in training_data.items():
-            self._synthetics_train.training_columns[table] = list(df.columns)
+        training_data = self._strategy.prepare_training_data(
+            self.relational_data, tables
+        )
         training_paths = {}
 
         for table_name in tables:
             training_path = self._working_dir / f"synthetics_train_{table_name}.csv"
             training_data[table_name].to_csv(training_path, index=False)
             training_paths[table_name] = training_path
 
         return training_paths
 
-    def _train_synthetics_models(self, training_data: Dict[str, Path]) -> None:
+    def _train_synthetics_models(self, training_data: dict[str, Path]) -> None:
         for table_name, training_csv in training_data.items():
             synthetics_config = make_synthetics_config(table_name, self._model_config)
             model = self._project.create_model_obj(
                 model_config=synthetics_config, data_source=str(training_csv)
             )
             self._synthetics_train.models[table_name] = model
 
+        archive_path = self._working_dir / "synthetics_training.tar.gz"
+        for table_name, csv_path in training_data.items():
+            add_to_tar(archive_path, csv_path, csv_path.name)
+        self._artifact_collection.upload_synthetics_training_archive(
+            self._project, str(archive_path)
+        )
+
         self._backup()
 
         task = SyntheticsTrainTask(
             synthetics_train=self._synthetics_train,
             multitable=self,
         )
         run_task(task, self._extended_sdk)
 
         for table in task.completed:
-            model = self._synthetics_train.models[table]
-            self._strategy.update_evaluation_from_model(
-                table, self.evaluations, model, self._working_dir, self._extended_sdk
-            )
-
-        # TODO: consider moving this to before running the task
-        archive_path = self._working_dir / "synthetics_training.tar.gz"
-        for table_name, csv_path in training_data.items():
-            add_to_tar(archive_path, csv_path, csv_path.name)
-        self._artifact_collection.upload_synthetics_training_archive(
-            self._project, str(archive_path)
-        )
+            if table in self.relational_data.list_all_tables(Scope.EVALUATABLE):
+                model = self._synthetics_train.models[table]
+                self._strategy.update_evaluation_from_model(
+                    table,
+                    self._evaluations,
+                    model,
+                    self._working_dir,
+                    self._extended_sdk,
+                )
 
     def train(self) -> None:
-        """Train synthetic data models on each table in the relational dataset"""
+        """
+        DEPRECATED: Please use `train_synthetics` instead.
+        """
+        logger.warning(
+            "This method is deprecated and will be removed in a future release. "
+            "Please use `train_synthetics` instead."
+        )
         tables = self.relational_data.list_all_tables()
         self._synthetics_train = SyntheticsTrain()
 
         training_data = self._prepare_training_data(tables)
         self._train_synthetics_models(training_data)
 
-    def retrain_tables(self, tables: Dict[str, pd.DataFrame]) -> None:
+    def train_synthetics(
+        self,
+        *,
+        only: Optional[set[str]] = None,
+        ignore: Optional[set[str]] = None,
+    ) -> None:
+        """
+        Train synthetic data models for the tables in the tableset,
+        optionally scoped by either `only` or `ignore`.
+        """
+        only, ignore = self._get_only_and_ignore(only, ignore)
+
+        all_tables = self.relational_data.list_all_tables()
+        include_tables = []
+        omit_tables = []
+        for table in all_tables:
+            if skip_table(table, only, ignore):
+                omit_tables.append(table)
+            else:
+                include_tables.append(table)
+
+        # TODO: Ancestral strategy requires that for each table omitted from synthetics ("preserved"),
+        # all its ancestors must also be omitted. In the future, it'd be nice to either find a way to
+        # eliminate this requirement completely, or (less ideal) allow incremental training of tables,
+        # e.g. train a few in one "batch", then a few more before generating (perhaps with some logs
+        # along the way informing the user of which required tables are missing).
+        self._strategy.validate_preserved_tables(omit_tables, self.relational_data)
+
+        training_data = self._prepare_training_data(include_tables)
+        self._train_synthetics_models(training_data)
+
+    def retrain_tables(self, tables: dict[str, pd.DataFrame]) -> None:
         """
         Provide updated table data and retrain. This method overwrites the table data in the
         `RelationalData` instance. It should be used when initial training fails and source data
         needs to be altered, but progress on other tables can be left as-is.
         """
         for table_name, table_data in tables.items():
             self.relational_data.update_table_data(table_name, table_data)
@@ -701,36 +829,35 @@
         tables_to_retrain = self._strategy.tables_to_retrain(
             list(tables.keys()), self.relational_data
         )
 
         for table in tables_to_retrain:
             with suppress(KeyError):
                 del self._synthetics_train.models[table]
-                del self._synthetics_train.training_columns[table]
         training_data = self._prepare_training_data(tables_to_retrain)
         self._train_synthetics_models(training_data)
 
     def _upload_sources_to_project(self) -> None:
         archive_path = self._working_dir / "source_tables.tar.gz"
         with tarfile.open(archive_path, "w:gz") as tar:
-            for table in self.relational_data.list_all_tables():
+            for table in self.relational_data.list_all_tables(Scope.ALL):
                 filename = f"source_{table}.csv"
                 out_path = self._working_dir / filename
                 df = self.relational_data.get_table_data(table)
                 df.to_csv(out_path, index=False)
                 tar.add(out_path, arcname=filename)
         self._artifact_collection.upload_source_archive(
             self._project, str(archive_path)
         )
         self._backup()
 
     def generate(
         self,
         record_size_ratio: float = 1.0,
-        preserve_tables: Optional[List[str]] = None,
+        preserve_tables: Optional[list[str]] = None,
         identifier: Optional[str] = None,
         resume: bool = False,
     ) -> None:
         """
         Sample synthetic data from trained models.
         Tables that did not train successfully will be omitted from the output dictionary.
         Tables listed in `preserve_tables` *may differ* from source tables in foreign key columns, to ensure
@@ -761,26 +888,31 @@
             if self._synthetics_run is None:
                 raise MultiTableException(
                     "Cannot resume a synthetics generation run without existing run information."
                 )
             logger.info(f"Resuming synthetics run `{self._synthetics_run.identifier}`")
         else:
             preserve_tables = preserve_tables or []
+            preserve_tables.extend(
+                [
+                    table
+                    for table in self.relational_data.list_all_tables()
+                    if table not in self._synthetics_train.models
+                ]
+            )
             self._strategy.validate_preserved_tables(
                 preserve_tables, self.relational_data
             )
 
             identifier = identifier or f"synthetics_{_timestamp()}"
-            missing_model = self._list_tables_with_missing_models()
 
             self._synthetics_run = SyntheticsRun(
                 identifier=identifier,
                 record_size_ratio=record_size_ratio,
                 preserved=preserve_tables,
-                missing_model=missing_model,
                 record_handlers={},
                 lost_contact=[],
             )
             logger.info(f"Starting synthetics run `{self._synthetics_run.identifier}`")
 
         run_dir = _mkdir(str(self._working_dir / self._synthetics_run.identifier))
 
@@ -795,26 +927,34 @@
         output_tables = self._strategy.post_process_synthetic_results(
             synth_tables=task.output_tables,
             preserved=self._synthetics_run.preserved,
             rel_data=self.relational_data,
             record_size_ratio=self._synthetics_run.record_size_ratio,
         )
 
-        for table, synth_df in output_tables.items():
+        reshaped_tables = self.relational_data.restore(output_tables)
+
+        for table, synth_df in reshaped_tables.items():
             synth_csv_path = run_dir / f"synth_{table}.csv"
             synth_df.to_csv(synth_csv_path, index=False)
 
         evaluate_project = create_project(
             display_name=f"evaluate-{self._project.display_name}"
         )
         evaluate_models = {}
         for table, synth_df in output_tables.items():
             if table in self._synthetics_run.preserved:
                 continue
 
+            if table not in self._synthetics_train.models:
+                continue
+
+            if table not in self.relational_data.list_all_tables(Scope.EVALUATABLE):
+                continue
+
             evaluate_data = self._strategy.get_evaluate_model_data(
                 rel_data=self.relational_data,
                 table_name=table,
                 synthetic_tables=output_tables,
             )
             if evaluate_data is None:
                 continue
@@ -828,19 +968,20 @@
         synthetics_evaluate_task = SyntheticsEvaluateTask(
             evaluate_models=evaluate_models,
             project=evaluate_project,
             multitable=self,
         )
         run_task(synthetics_evaluate_task, self._extended_sdk)
 
+        # Tables passed to task were already scoped to evaluatable tables
         for table in synthetics_evaluate_task.completed:
             self._strategy.update_evaluation_from_evaluate(
                 table_name=table,
                 evaluate_model=evaluate_models[table],
-                evaluations=self.evaluations,
+                evaluations=self._evaluations,
                 working_dir=self._working_dir,
                 extended_sdk=self._extended_sdk,
             )
 
         evaluate_project.delete()
 
         for table_name in output_tables:
@@ -861,44 +1002,29 @@
 
         archive_path = self._working_dir / "synthetics_outputs.tar.gz"
         add_to_tar(archive_path, run_dir, self._synthetics_run.identifier)
 
         self._artifact_collection.upload_synthetics_outputs_archive(
             self._project, str(archive_path)
         )
-        self.synthetic_output_tables = output_tables
+        self.synthetic_output_tables = reshaped_tables
         self._backup()
 
     def create_relational_report(self, run_identifier: str, target_dir: Path) -> None:
         presenter = ReportPresenter(
             rel_data=self.relational_data,
             evaluations=self.evaluations,
             now=datetime.utcnow(),
             run_identifier=run_identifier,
         )
         output_path = target_dir / "relational_report.html"
         with open(output_path, "w") as report:
             html_content = ReportRenderer().render(presenter)
             report.write(html_content)
 
-    def _list_tables_with_missing_models(self) -> List[str]:
-        missing_model = set()
-        for table in self.relational_data.list_all_tables():
-            if not _table_trained_successfully(self._synthetics_train, table):
-                logger.info(
-                    f"Skipping synthetic data generation for `{table}` because it does not have a trained model"
-                )
-                missing_model.add(table)
-                for descendant in self.relational_data.get_descendants(table):
-                    logger.info(
-                        f"Skipping synthetic data generation for `{descendant}` because it depends on `{table}`"
-                    )
-                    missing_model.add(table)
-        return list(missing_model)
-
     def _attach_existing_reports(self, run_id: str, table: str) -> None:
         individual_path = (
             self._working_dir
             / run_id
             / f"synthetics_individual_evaluation_{table}.json"
         )
         cross_table_path = (
@@ -906,18 +1032,18 @@
             / run_id
             / f"synthetics_cross_table_evaluation_{table}.json"
         )
 
         individual_report_json = json.loads(smart_open.open(individual_path).read())
         cross_table_report_json = json.loads(smart_open.open(cross_table_path).read())
 
-        self.evaluations[table].individual_report_json = individual_report_json
-        self.evaluations[table].cross_table_report_json = cross_table_report_json
+        self._evaluations[table].individual_report_json = individual_report_json
+        self._evaluations[table].cross_table_report_json = cross_table_report_json
 
-    def _validate_gretel_model(self, gretel_model: Optional[str]) -> Tuple[str, str]:
+    def _validate_gretel_model(self, gretel_model: Optional[str]) -> tuple[str, str]:
         gretel_model = (gretel_model or self._strategy.default_model).lower()
         supported_models = self._strategy.supported_models
         if gretel_model not in supported_models:
             msg = f"Invalid gretel model requested: {gretel_model}. The selected strategy supports: {supported_models}."
             logger.warning(msg)
             raise MultiTableException(msg)
 
@@ -940,17 +1066,15 @@
         return AncestralStrategy()
     else:
         msg = f"Unrecognized strategy requested: {strategy}. Supported strategies are `independent` and `ancestral`."
         logger.warning(msg)
         raise MultiTableException(msg)
 
 
-def _table_trained_successfully(
-    train_state: Union[TransformsTrain, SyntheticsTrain], table: str
-) -> bool:
+def _table_trained_successfully(train_state: TransformsTrain, table: str) -> bool:
     model = train_state.models.get(table)
     if model is None:
         return False
     else:
         return model.status == Status.COMPLETED
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/report/figures.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/report/figures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import math
-from typing import List, Optional
+from typing import Optional
 
 import plotly.graph_objects as go
 
 _GRETEL_PALETTE = ["#A051FA", "#18E7AA"]
 
 SCORE_VALUES = [
     {"label": "Very poor", "color": "rgb(229, 60, 26)"},
@@ -51,15 +51,15 @@
         {size * math.sin(math.radians(theta + 90)) + 0.5}
     Z"""
 
 
 def gauge_and_needle_chart(
     score: Optional[int],
     display_score: bool = True,
-    marker_colors: Optional[List[str]] = None,
+    marker_colors: Optional[list[str]] = None,
 ) -> go.Figure:
     """
     The 'fancy' gauge and needle chart to go with the overall score of the report.  Has colored segments for
     each grade range and an svg pointer supplied by _generate_pointer_path
 
     Args:
         score: Integer score in [0,100].  Pointer path will point at this value on the gauge.
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/report/key_highlight.js` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/report/key_highlight.js`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report.css` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 import datetime
 from dataclasses import dataclass
 from functools import cached_property
 from math import ceil
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple
+from typing import Optional
 
 import plotly.graph_objects as go
 from jinja2 import Environment, FileSystemLoader
 
-from gretel_trainer.relational.core import ForeignKey, RelationalData
+from gretel_trainer.relational.core import ForeignKey, RelationalData, Scope
 from gretel_trainer.relational.report.figures import (
     PRIVACY_LEVEL_VALUES,
     gauge_and_needle_chart,
 )
 from gretel_trainer.relational.table_evaluation import TableEvaluation
 
 _TEMPLATE_DIR = str(Path(__file__).parent)
@@ -30,35 +30,35 @@
     def render(self, presenter: ReportPresenter) -> str:
         return self.template.render(presenter=presenter)
 
 
 @dataclass
 class ReportTableData:
     table: str
-    pk: List[str]
-    fks: List[ForeignKey]
+    pk: list[str]
+    fks: list[ForeignKey]
 
 
 @dataclass
 class ReportPresenter:
     rel_data: RelationalData
     now: datetime.datetime
     run_identifier: str
-    evaluations: Dict[str, TableEvaluation]
+    evaluations: dict[str, TableEvaluation]
 
     @property
     def generated_at(self) -> str:
         return self.now.strftime("%Y-%m-%d")
 
     @property
     def copyright_year(self) -> str:
         return self.now.strftime("%Y")
 
     @cached_property
-    def composite_sqs_score_and_grade(self) -> Tuple[Optional[int], str]:
+    def composite_sqs_score_and_grade(self) -> tuple[Optional[int], str]:
         # Add up all the non-None SQS scores and track how many there are.
         _total_score = 0
         _num_scores = 0
         for eval in self.evaluations.values():
             if eval.individual_sqs is not None:
                 _total_score += eval.individual_sqs
                 _num_scores += 1
@@ -81,15 +81,15 @@
 
     @property
     def composite_sqs_figure(self) -> go.Figure:
         score, grade = self.composite_sqs_score_and_grade
         return gauge_and_needle_chart(score)
 
     @cached_property
-    def composite_ppl_score_and_grade(self) -> Tuple[Optional[int], str]:
+    def composite_ppl_score_and_grade(self) -> tuple[Optional[int], str]:
         # Collect all the non-None PPLs, individual and cross-table.
         scores = [
             eval.individual_ppl
             for eval in self.evaluations.values()
             if eval.individual_ppl is not None
         ]
         scores += [
@@ -129,19 +129,19 @@
         return gauge_and_needle_chart(
             ppl_score,
             display_score=False,
             marker_colors=[s["color"] for s in PRIVACY_LEVEL_VALUES],
         )
 
     @property
-    def report_table_data(self) -> List[ReportTableData]:
+    def report_table_data(self) -> list[ReportTableData]:
         table_data = []
-        for table in self.rel_data.list_all_tables():
+        for table in self.rel_data.list_all_tables(Scope.PUBLIC):
             pk = self.rel_data.get_primary_key(table)
-            fks = self.rel_data.get_foreign_keys(table)
+            fks = self.rel_data.get_foreign_keys(table, rename_invented_tables=True)
             table_data.append(ReportTableData(table=table, pk=pk, fks=fks))
 
         # Sort tables alphabetically because that's nice.
         table_data = sorted(table_data, key=lambda x: x.table)
         return table_data
 
     # Helper, making it "just a method" so it is easily accessible in jinja template.
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report_privacy_protection.css` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report_privacy_protection.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report_synthetic_quality.css` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report_synthetic_quality.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report_template.html` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report_template.html`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/sdk_extras.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/sdk_extras.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import shutil
 from contextlib import suppress
 from pathlib import Path
-from typing import Any, Dict, Optional, Union
+from typing import Any, Optional, Union
 
 import pandas as pd
 import requests
 import smart_open
 from gretel_client.projects.jobs import Job, Status
 from gretel_client.projects.models import Model
 from gretel_client.projects.projects import Project
@@ -32,15 +32,15 @@
             raise MultiTableException("Unexpected job object")
 
     def delete_data_source(self, project: Project, job: Job) -> None:
         if not self._hybrid and job.data_source is not None:
             project.delete_artifact(job.data_source)
 
     def cautiously_refresh_status(
-        self, job: Job, key: str, refresh_attempts: Dict[str, int]
+        self, job: Job, key: str, refresh_attempts: dict[str, int]
     ) -> Status:
         try:
             job.refresh()
             refresh_attempts[key] = 0
         except:
             refresh_attempts[key] = refresh_attempts[key] + 1
 
@@ -69,15 +69,15 @@
             response = requests.get(download_link)
             if response.status_code == 200:
                 with open(out_path, "wb") as out:
                     out.write(response.content)
         except:
             logger.warning(f"Failed to download `{artifact_name}`")
 
-    def sqs_score_from_full_report(self, report: Dict[str, Any]) -> Optional[int]:
+    def sqs_score_from_full_report(self, report: dict[str, Any]) -> Optional[int]:
         with suppress(KeyError):
             for field_dict in report["summary"]:
                 if field_dict["field"] == "synthetic_data_quality_score":
                     return field_dict["value"]
 
     def get_record_handler_data(self, record_handler: RecordHandler) -> pd.DataFrame:
         return pd.read_csv(record_handler.get_artifact_link("data"), compression="gzip")
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/strategies/ancestral.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/strategies/ancestral.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Optional, Union
 
 import pandas as pd
 from gretel_client.projects.models import Model
 
 import gretel_trainer.relational.ancestry as ancestry
 import gretel_trainer.relational.strategies.common as common
 from gretel_trainer.relational.core import MultiTableException, RelationalData
@@ -20,73 +20,78 @@
         return "ancestral"
 
     @property
     def default_model(self) -> str:
         return "amplify"
 
     @property
-    def supported_models(self) -> List[str]:
+    def supported_models(self) -> list[str]:
         return ["amplify"]
 
     def label_encode_keys(
-        self, rel_data: RelationalData, tables: Dict[str, pd.DataFrame]
-    ) -> Dict[str, pd.DataFrame]:
+        self, rel_data: RelationalData, tables: dict[str, pd.DataFrame]
+    ) -> dict[str, pd.DataFrame]:
         return common.label_encode_keys(rel_data, tables)
 
     def prepare_training_data(
-        self, rel_data: RelationalData
-    ) -> Dict[str, pd.DataFrame]:
+        self, rel_data: RelationalData, tables: list[str]
+    ) -> dict[str, pd.DataFrame]:
         """
         Returns tables with:
         - all safe-for-seed ancestor fields added
         - columns in multigenerational format
         - all keys translated to contiguous integers
         - artificial min/max seed records added
         """
         all_tables = rel_data.list_all_tables()
+        omitted_tables = [t for t in all_tables if t not in tables]
         altered_tableset = {}
         training_data = {}
 
         # Create a new table set identical to source data
         for table_name in all_tables:
             altered_tableset[table_name] = rel_data.get_table_data(table_name).copy()
 
         # Translate all keys to a contiguous list of integers
-        altered_tableset = common.label_encode_keys(rel_data, altered_tableset)
+        altered_tableset = common.label_encode_keys(
+            rel_data, altered_tableset, omit=omitted_tables
+        )
 
         # Add artificial rows to support seeding
-        altered_tableset = _add_artifical_rows_for_seeding(rel_data, altered_tableset)
+        altered_tableset = _add_artifical_rows_for_seeding(
+            rel_data, altered_tableset, omitted_tables
+        )
 
         # Collect all data in multigenerational format
-        for table_name in all_tables:
+        for table_name in tables:
             data = ancestry.get_table_data_with_ancestors(
                 rel_data=rel_data,
                 table=table_name,
                 tableset=altered_tableset,
                 ancestral_seeding=True,
             )
             training_data[table_name] = data
 
         return training_data
 
     def tables_to_retrain(
-        self, tables: List[str], rel_data: RelationalData
-    ) -> List[str]:
+        self, tables: list[str], rel_data: RelationalData
+    ) -> list[str]:
         """
         Given a set of tables requested to retrain, returns those tables with all their
         descendants, because those descendant tables were trained with data from their
         parents appended.
         """
         retrain = set(tables)
         for table in tables:
             retrain.update(rel_data.get_descendants(table))
         return list(retrain)
 
     def validate_preserved_tables(
-        self, tables: List[str], rel_data: RelationalData
+        self, tables: list[str], rel_data: RelationalData
     ) -> None:
         """
         Ensures that for every table marked as preserved, all its ancestors are also preserved.
         """
         for table in tables:
             for parent in rel_data.get_parents(table):
                 if parent not in tables:
@@ -100,17 +105,17 @@
         to reference during generation post-processing.
         """
         return ancestry.get_table_data_with_ancestors(rel_data, table)
 
     def ready_to_generate(
         self,
         rel_data: RelationalData,
-        in_progress: List[str],
-        finished: List[str],
-    ) -> List[str]:
+        in_progress: list[str],
+        finished: list[str],
+    ) -> list[str]:
         """
         Tables with no parents are immediately ready for generation.
         Tables with parents are ready once their parents are finished.
         All tables are no longer considered ready once they are at least in progress.
         """
         ready = []
 
@@ -127,46 +132,45 @@
         return ready
 
     def get_generation_job(
         self,
         table: str,
         rel_data: RelationalData,
         record_size_ratio: float,
-        output_tables: Dict[str, pd.DataFrame],
+        output_tables: dict[str, pd.DataFrame],
         target_dir: Path,
-        training_columns: List[str],
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """
         Returns kwargs for creating a record handler job via the Gretel SDK.
 
         If the table does not have any parents, job requests an output
         record count based on the initial table data size and the record size ratio.
 
         If the table does have parents, builds a seed dataframe to use in generation.
         """
         source_data_size = len(rel_data.get_table_data(table))
         synth_size = int(source_data_size * record_size_ratio)
         if len(rel_data.get_parents(table)) == 0:
             return {"params": {"num_records": synth_size}}
         else:
             seed_df = self._build_seed_data_for_table(
-                table, output_tables, rel_data, synth_size, training_columns
+                table, output_tables, rel_data, synth_size
             )
             seed_path = target_dir / f"synthetics_seed_{table}.csv"
             seed_df.to_csv(seed_path, index=False)
             return {"data_source": str(seed_path)}
 
     def _build_seed_data_for_table(
         self,
         table: str,
-        output_tables: Dict[str, pd.DataFrame],
+        output_tables: dict[str, pd.DataFrame],
         rel_data: RelationalData,
         synth_size: int,
-        training_columns: List[str],
     ) -> pd.DataFrame:
+        column_legend = ancestry.get_seed_safe_multigenerational_columns(rel_data)
         seed_df = pd.DataFrame()
 
         source_data = rel_data.get_table_data(table)
         for fk in rel_data.get_foreign_keys(table):
             parent_table_data = output_tables[fk.parent_table_name]
             parent_table_data = ancestry.prepend_foreign_key_lineage(
                 parent_table_data, fk.columns
@@ -198,15 +202,17 @@
                 how="left",
                 left_on=tmp_column_name,
                 right_index=True,
             )
 
             # Drop any columns that weren't used in training, as well as the temporary merge column
             columns_to_drop = [
-                col for col in this_fk_seed_df.columns if col not in training_columns
+                col
+                for col in this_fk_seed_df.columns
+                if col not in column_legend[table]
             ]
             columns_to_drop.append(tmp_column_name)
             this_fk_seed_df = this_fk_seed_df.drop(columns=columns_to_drop)
 
             seed_df = pd.concat(
                 [
                     seed_df.reset_index(drop=True),
@@ -215,15 +221,15 @@
                 axis=1,
             )
 
         return seed_df
 
     def tables_to_skip_when_failed(
         self, table: str, rel_data: RelationalData
-    ) -> List[str]:
+    ) -> list[str]:
         return rel_data.get_descendants(table)
 
     def post_process_individual_synthetic_result(
         self,
         table_name: str,
         rel_data: RelationalData,
         synthetic_table: pd.DataFrame,
@@ -261,31 +267,31 @@
             fk_col, parent_pk_col = fk_map
             processed[fk_col] = processed[parent_pk_col]
 
         return processed
 
     def post_process_synthetic_results(
         self,
-        synth_tables: Dict[str, pd.DataFrame],
-        preserved: List[str],
+        synth_tables: dict[str, pd.DataFrame],
+        preserved: list[str],
         rel_data: RelationalData,
         record_size_ratio: float,
-    ) -> Dict[str, pd.DataFrame]:
+    ) -> dict[str, pd.DataFrame]:
         """
         Restores tables from multigenerational to original shape
         """
         return {
             table_name: ancestry.drop_ancestral_data(df)
             for table_name, df in synth_tables.items()
         }
 
     def update_evaluation_from_model(
         self,
         table_name: str,
-        evaluations: Dict[str, TableEvaluation],
+        evaluations: dict[str, TableEvaluation],
         model: Model,
         working_dir: Path,
         extended_sdk: ExtendedGretelSDK,
     ) -> None:
         logger.info(f"Downloading cross_table evaluation reports for `{table_name}`.")
         out_filepath = working_dir / f"synthetics_cross_table_evaluation_{table_name}"
         common.download_artifacts(model, out_filepath, extended_sdk)
@@ -295,25 +301,25 @@
             model, out_filepath
         )
 
     def get_evaluate_model_data(
         self,
         table_name: str,
         rel_data: RelationalData,
-        synthetic_tables: Dict[str, pd.DataFrame],
-    ) -> Optional[Dict[str, pd.DataFrame]]:
+        synthetic_tables: dict[str, pd.DataFrame],
+    ) -> Optional[dict[str, pd.DataFrame]]:
         return {
             "source": rel_data.get_table_data(table_name),
             "synthetic": synthetic_tables[table_name],
         }
 
     def update_evaluation_from_evaluate(
         self,
         table_name: str,
-        evaluations: Dict[str, TableEvaluation],
+        evaluations: dict[str, TableEvaluation],
         evaluate_model: Model,
         working_dir: Path,
         extended_sdk: ExtendedGretelSDK,
     ) -> None:
         logger.info(f"Downloading individual evaluation reports for `{table_name}`.")
         out_filepath = working_dir / f"synthetics_individual_evaluation_{table_name}"
         common.download_artifacts(evaluate_model, out_filepath, extended_sdk)
@@ -321,52 +327,62 @@
         evaluation = evaluations[table_name]
         evaluation.individual_report_json = common.read_report_json_data(
             evaluate_model, out_filepath
         )
 
 
 def _add_artifical_rows_for_seeding(
-    rel_data: RelationalData, tables: Dict[str, pd.DataFrame]
-) -> Dict[str, pd.DataFrame]:
+    rel_data: RelationalData, tables: dict[str, pd.DataFrame], omitted: list[str]
+) -> dict[str, pd.DataFrame]:
     # On each table, add an artifical row with the max possible PK value
+    # unless the table is omitted from synthetics
     max_pk_values = {}
     for table_name, data in tables.items():
+        if table_name in omitted:
+            continue
         max_pk_values[table_name] = len(data) * 50
 
         random_record = tables[table_name].sample().copy()
         for pk_col in rel_data.get_primary_key(table_name):
             random_record[pk_col] = max_pk_values[table_name]
         tables[table_name] = pd.concat([data, random_record]).reset_index(drop=True)
 
     # On each table with foreign keys, add two more artificial rows containing the min and max FK values
     for table_name, data in tables.items():
         foreign_keys = rel_data.get_foreign_keys(table_name)
         if len(foreign_keys) == 0:
             continue
 
+        # Skip if the parent table is omitted and is the only parent
+        if len(foreign_keys) == 1 and foreign_keys[0].parent_table_name in omitted:
+            continue
+
         two_records = tables[table_name].sample(2)
         min_fk_record = two_records.head(1).copy()
         max_fk_record = two_records.tail(1).copy()
 
         # By default, just auto-increment the primary key
         for pk_col in rel_data.get_primary_key(table_name):
             min_fk_record[pk_col] = max_pk_values[table_name] + 1
             max_fk_record[pk_col] = max_pk_values[table_name] + 2
 
         # This can potentially overwrite the auto-incremented primary keys above in the case of composite keys
         for foreign_key in foreign_keys:
+            # Treat FK columns to omitted parents as normal columns
+            if foreign_key.parent_table_name in omitted:
+                continue
             for fk_col in foreign_key.columns:
                 min_fk_record[fk_col] = 0
                 max_fk_record[fk_col] = max_pk_values[foreign_key.parent_table_name]
 
         tables[table_name] = pd.concat(
             [data, min_fk_record, max_fk_record]
         ).reset_index(drop=True)
 
     return tables
 
 
-def _safe_inc(i: int, col: Union[List[Any], range]) -> int:
+def _safe_inc(i: int, col: Union[list, range]) -> int:
     i = i + 1
     if i == len(col):
         i = 0
     return i
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/strategies/common.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/strategies/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import logging
 import math
 import random
 from pathlib import Path
-from typing import Dict, List, Optional, Set, Tuple
+from typing import Optional
 
 import pandas as pd
 import smart_open
 from gretel_client.projects.models import Model
 from sklearn import preprocessing
 
 from gretel_trainer.relational.core import RelationalData
@@ -25,47 +25,53 @@
     legend = {"html": "report", "json": "report_json"}
 
     for filetype, artifact_name in legend.items():
         out_path = f"{out_filepath}.{filetype}"
         extended_sdk.download_file_artifact(model, artifact_name, out_path)
 
 
-def read_report_json_data(model: Model, report_path: Path) -> Optional[Dict]:
+def read_report_json_data(model: Model, report_path: Path) -> Optional[dict]:
     full_path = f"{report_path}.json"
     try:
         return json.loads(smart_open.open(full_path).read())
     except:
         return _get_report_json(model)
 
 
-def _get_report_json(model: Model) -> Optional[Dict]:
+def _get_report_json(model: Model) -> Optional[dict]:
     try:
         return json.loads(
             smart_open.open(model.get_artifact_link("report_json")).read()
         )
     except:
         logger.warning("Failed to fetch model evaluation report JSON.")
         return None
 
 
 def label_encode_keys(
-    rel_data: RelationalData, tables: Dict[str, pd.DataFrame]
-) -> Dict[str, pd.DataFrame]:
+    rel_data: RelationalData,
+    tables: dict[str, pd.DataFrame],
+    omit: Optional[list[str]] = None,
+) -> dict[str, pd.DataFrame]:
     """
     Crawls tables for all key columns (primary and foreign). For each PK (and FK columns referencing it),
     runs all values through a LabelEncoder and updates tables' columns to use LE-transformed values.
     """
+    omit = omit or []
     for table_name in rel_data.list_tables_parents_before_children():
+        if table_name in omit:
+            continue
+
         df = tables.get(table_name)
         if df is None:
             continue
 
         for primary_key_column in rel_data.get_primary_key(table_name):
             # Get a set of the tables and columns in `tables` referencing this PK
-            fk_references: Set[Tuple[str, str]] = set()
+            fk_references: set[tuple[str, str]] = set()
             for descendant in rel_data.get_descendants(table_name):
                 if tables.get(descendant) is None:
                     continue
                 fks = rel_data.get_foreign_keys(descendant)
                 for fk in fks:
                     if fk.parent_table_name != table_name:
                         continue
@@ -100,18 +106,18 @@
 
     return tables
 
 
 def make_composite_pk_columns(
     table_name: str,
     rel_data: RelationalData,
-    primary_key: List[str],
+    primary_key: list[str],
     synth_row_count: int,
     record_size_ratio: float,
-) -> List[Tuple]:
+) -> list[tuple]:
     source_pk_columns = rel_data.get_table_data(table_name)[primary_key]
     unique_counts = source_pk_columns.nunique(axis=0)
     new_key_columns_values = []
     for col in primary_key:
         synth_values_count = math.ceil(unique_counts[col] * record_size_ratio)
         new_key_columns_values.append(range(synth_values_count))
 
@@ -121,9 +127,9 @@
             [random.choice(vals) for vals in new_key_columns_values]
         )
         results.add(key_combination)
 
     return list(zip(*results))
 
 
-def get_frequencies(table_data: pd.DataFrame, cols: List[str]) -> List[int]:
+def get_frequencies(table_data: pd.DataFrame, cols: list[str]) -> list[int]:
     return list(table_data.groupby(cols).size().reset_index()[0])
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/strategies/independent.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/strategies/independent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import random
 from pathlib import Path
-from typing import Any, Dict, List, Optional
+from typing import Any, Optional
 
 import pandas as pd
 from gretel_client.projects.models import Model
 
 import gretel_trainer.relational.ancestry as ancestry
 import gretel_trainer.relational.strategies.common as common
 from gretel_trainer.relational.core import RelationalData
@@ -21,53 +21,53 @@
         return "independent"
 
     @property
     def default_model(self) -> str:
         return "amplify"
 
     @property
-    def supported_models(self) -> List[str]:
+    def supported_models(self) -> list[str]:
         return ["amplify", "actgan", "lstm", "tabular-dp"]
 
     def label_encode_keys(
-        self, rel_data: RelationalData, tables: Dict[str, pd.DataFrame]
-    ) -> Dict[str, pd.DataFrame]:
+        self, rel_data: RelationalData, tables: dict[str, pd.DataFrame]
+    ) -> dict[str, pd.DataFrame]:
         return common.label_encode_keys(rel_data, tables)
 
     def prepare_training_data(
-        self, rel_data: RelationalData
-    ) -> Dict[str, pd.DataFrame]:
+        self, rel_data: RelationalData, tables: list[str]
+    ) -> dict[str, pd.DataFrame]:
         """
         Returns source tables with primary and foreign keys removed
         """
         training_data = {}
 
-        for table_name in rel_data.list_all_tables():
+        for table_name in tables:
             columns_to_drop = []
             columns_to_drop.extend(rel_data.get_primary_key(table_name))
             for foreign_key in rel_data.get_foreign_keys(table_name):
                 columns_to_drop.extend(foreign_key.columns)
 
             data = rel_data.get_table_data(table_name)
             data = data.drop(columns=columns_to_drop)
 
             training_data[table_name] = data
 
         return training_data
 
     def tables_to_retrain(
-        self, tables: List[str], rel_data: RelationalData
-    ) -> List[str]:
+        self, tables: list[str], rel_data: RelationalData
+    ) -> list[str]:
         """
         Returns the provided tables requested to retrain, unaltered.
         """
         return tables
 
     def validate_preserved_tables(
-        self, tables: List[str], rel_data: RelationalData
+        self, tables: list[str], rel_data: RelationalData
     ) -> None:
         """
         No-op. Under this strategy, any collection of tables can be preserved.
         """
         pass
 
     def get_preserved_data(self, table: str, rel_data: RelationalData) -> pd.DataFrame:
@@ -76,17 +76,17 @@
         to reference during generation post-processing.
         """
         return rel_data.get_table_data(table)
 
     def ready_to_generate(
         self,
         rel_data: RelationalData,
-        in_progress: List[str],
-        finished: List[str],
-    ) -> List[str]:
+        in_progress: list[str],
+        finished: list[str],
+    ) -> list[str]:
         """
         All tables are immediately ready for generation. Once they are
         at least in progress, they are no longer ready.
         """
         return [
             table
             for table in rel_data.list_all_tables()
@@ -94,29 +94,28 @@
         ]
 
     def get_generation_job(
         self,
         table: str,
         rel_data: RelationalData,
         record_size_ratio: float,
-        output_tables: Dict[str, pd.DataFrame],
+        output_tables: dict[str, pd.DataFrame],
         target_dir: Path,
-        training_columns: List[str],
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """
         Returns kwargs for a record handler job requesting an output record
         count based on the initial table data size and the record size ratio.
         """
         source_data_size = len(rel_data.get_table_data(table))
         synth_size = int(source_data_size * record_size_ratio)
         return {"params": {"num_records": synth_size}}
 
     def tables_to_skip_when_failed(
         self, table: str, rel_data: RelationalData
-    ) -> List[str]:
+    ) -> list[str]:
         return []
 
     def post_process_individual_synthetic_result(
         self,
         table_name: str,
         rel_data: RelationalData,
         synthetic_table: pd.DataFrame,
@@ -126,30 +125,30 @@
         No-op. This strategy does not apply any changes to individual table results upon record handler completion.
         All post-processing is performed on the output tables collectively when they are all finished.
         """
         return synthetic_table
 
     def post_process_synthetic_results(
         self,
-        synth_tables: Dict[str, pd.DataFrame],
-        preserved: List[str],
+        synth_tables: dict[str, pd.DataFrame],
+        preserved: list[str],
         rel_data: RelationalData,
         record_size_ratio: float,
-    ) -> Dict[str, pd.DataFrame]:
+    ) -> dict[str, pd.DataFrame]:
         "Synthesizes primary and foreign keys"
         synth_tables = _synthesize_primary_keys(
             synth_tables, preserved, rel_data, record_size_ratio
         )
         synth_tables = _synthesize_foreign_keys(synth_tables, rel_data)
         return synth_tables
 
     def update_evaluation_from_model(
         self,
         table_name: str,
-        evaluations: Dict[str, TableEvaluation],
+        evaluations: dict[str, TableEvaluation],
         model: Model,
         working_dir: Path,
         extended_sdk: ExtendedGretelSDK,
     ) -> None:
         logger.info(f"Downloading individual evaluation reports for `{table_name}`.")
         out_filepath = working_dir / f"synthetics_individual_evaluation_{table_name}"
         common.download_artifacts(model, out_filepath, extended_sdk)
@@ -159,16 +158,16 @@
             model, out_filepath
         )
 
     def get_evaluate_model_data(
         self,
         table_name: str,
         rel_data: RelationalData,
-        synthetic_tables: Dict[str, pd.DataFrame],
-    ) -> Optional[Dict[str, pd.DataFrame]]:
+        synthetic_tables: dict[str, pd.DataFrame],
+    ) -> Optional[dict[str, pd.DataFrame]]:
         missing_ancestors = [
             ancestor
             for ancestor in rel_data.get_ancestors(table_name)
             if ancestor not in synthetic_tables
         ]
         if len(missing_ancestors) > 0:
             logger.info(
@@ -184,15 +183,15 @@
             "source": source_data,
             "synthetic": synthetic_data,
         }
 
     def update_evaluation_from_evaluate(
         self,
         table_name: str,
-        evaluations: Dict[str, TableEvaluation],
+        evaluations: dict[str, TableEvaluation],
         evaluate_model: Model,
         working_dir: Path,
         extended_sdk: ExtendedGretelSDK,
     ) -> None:
         logger.info(f"Downloading cross table evaluation reports for `{table_name}`.")
         out_filepath = working_dir / f"synthetics_cross_table_evaluation_{table_name}"
         common.download_artifacts(evaluate_model, out_filepath, extended_sdk)
@@ -200,19 +199,19 @@
         evaluation = evaluations[table_name]
         evaluation.cross_table_report_json = common.read_report_json_data(
             evaluate_model, out_filepath
         )
 
 
 def _synthesize_primary_keys(
-    synth_tables: Dict[str, pd.DataFrame],
-    preserved: List[str],
+    synth_tables: dict[str, pd.DataFrame],
+    preserved: list[str],
     rel_data: RelationalData,
     record_size_ratio: float,
-) -> Dict[str, pd.DataFrame]:
+) -> dict[str, pd.DataFrame]:
     """
     Alters primary key columns on all tables *except* preserved.
     Assumes the primary key column is of type integer.
     """
     processed = {}
     for table_name, synth_data in synth_tables.items():
         processed[table_name] = synth_data.copy()
@@ -237,16 +236,16 @@
             for index, col in enumerate(primary_key):
                 processed[table_name][col] = synthetic_pk_columns[index]
 
     return processed
 
 
 def _synthesize_foreign_keys(
-    synth_tables: Dict[str, pd.DataFrame], rel_data: RelationalData
-) -> Dict[str, pd.DataFrame]:
+    synth_tables: dict[str, pd.DataFrame], rel_data: RelationalData
+) -> dict[str, pd.DataFrame]:
     """
     Alters foreign key columns on all tables (*including* those flagged as not to
     be synthesized to ensure joining to a synthesized parent table continues to work)
     by replacing foreign key column values with valid values from the parent table column
     being referenced.
     """
     processed = {}
@@ -278,18 +277,18 @@
 
         processed[table_name] = out_df
 
     return processed
 
 
 def _collect_values(
-    values: List[Any],
-    frequencies: List[int],
+    values: list,
+    frequencies: list[int],
     total: int,
-) -> List[Any]:
+) -> list:
     freqs = sorted(frequencies)
 
     # Loop through frequencies in ascending order,
     # adding "that many" of the next valid value
     # to the output collection
     v = 0
     f = 0
@@ -308,12 +307,12 @@
 
     # shuffle for realism
     random.shuffle(new_values)
 
     return new_values
 
 
-def _safe_inc(i: int, col: List[Any]) -> int:
+def _safe_inc(i: int, col: list) -> int:
     i = i + 1
     if i == len(col):
         i = 0
     return i
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/table_evaluation.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/table_evaluation.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/task_runner.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/task_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 from collections import defaultdict
-from typing import Dict, List
 
 from gretel_client.projects.jobs import END_STATES, Job, Status
 from gretel_client.projects.projects import Project
 from typing_extensions import Protocol
 
 from gretel_trainer.relational.sdk_extras import ExtendedGretelSDK
 
@@ -14,15 +13,15 @@
 
 
 class Task(Protocol):
     def action(self, job: Job) -> str:
         ...
 
     @property
-    def table_collection(self) -> List[str]:
+    def table_collection(self) -> list[str]:
         ...
 
     @property
     def artifacts_per_job(self) -> int:
         ...
 
     @property
@@ -54,15 +53,15 @@
         ...
 
     def each_iteration(self) -> None:
         ...
 
 
 def run_task(task: Task, extended_sdk: ExtendedGretelSDK) -> None:
-    refresh_attempts: Dict[str, int] = defaultdict(int)
+    refresh_attempts: dict[str, int] = defaultdict(int)
     first_pass = True
 
     while task.more_to_do():
         if first_pass:
             first_pass = False
         else:
             task.wait()
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/classify.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/classify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import shutil
 from pathlib import Path
-from typing import Dict, List
 
 import smart_open
 from gretel_client.projects.jobs import Job
 from gretel_client.projects.models import Model
 from gretel_client.projects.projects import Project
 from gretel_client.projects.records import RecordHandler
 
@@ -12,30 +11,30 @@
 from gretel_trainer.relational.workflow_state import Classify
 
 
 class ClassifyTask:
     def __init__(
         self,
         classify: Classify,
-        data_sources: Dict[str, str],
+        data_sources: dict[str, str],
         all_rows: bool,
         multitable: common._MultiTable,
         out_dir: Path,
     ):
         self.classify = classify
         self.data_sources = data_sources
         self.all_rows = all_rows
         self.multitable = multitable
         self.out_dir = out_dir
-        self.classify_record_handlers: Dict[str, RecordHandler] = {}
+        self.classify_record_handlers: dict[str, RecordHandler] = {}
         self.completed_models = []
         self.failed_models = []
         self.completed_record_handlers = []
         self.failed_record_handlers = []
-        self.result_filepaths: Dict[str, Path] = {}
+        self.result_filepaths: dict[str, Path] = {}
 
     def action(self, job: Job) -> str:
         if self.all_rows:
             if isinstance(job, Model):
                 return "classify training"
             else:
                 return "classification (all rows)"
@@ -47,15 +46,15 @@
         return self.multitable._project
 
     @property
     def artifacts_per_job(self) -> int:
         return 1
 
     @property
-    def table_collection(self) -> List[str]:
+    def table_collection(self) -> list[str]:
         return list(self.classify.models.keys())
 
     def more_to_do(self) -> bool:
         total_tables = len(self.classify.models)
         any_unfinished_models = len(self._finished_models) < total_tables
         any_unfinished_record_handlers = (
             len(self._finished_record_handlers) < total_tables
@@ -70,19 +69,19 @@
         if self.all_rows:
             duration = self.multitable._refresh_interval
         else:
             duration = 15
         common.wait(duration)
 
     @property
-    def _finished_models(self) -> List[str]:
+    def _finished_models(self) -> list[str]:
         return self.completed_models + self.failed_models
 
     @property
-    def _finished_record_handlers(self) -> List[str]:
+    def _finished_record_handlers(self) -> list[str]:
         return self.completed_record_handlers + self.failed_record_handlers
 
     def is_finished(self, table: str) -> bool:
         if self.all_rows:
             return (
                 table in self._finished_models
                 and table in self._finished_record_handlers
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/common.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/common.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/synthetics_evaluate.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/synthetics_evaluate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-from typing import Dict, List
-
 from gretel_client.projects.jobs import Job
 from gretel_client.projects.models import Model
 from gretel_client.projects.projects import Project
 
 import gretel_trainer.relational.tasks.common as common
 
 ACTION = "synthetic data evaluation"
 
 
 class SyntheticsEvaluateTask:
     def __init__(
         self,
-        evaluate_models: Dict[str, Model],
+        evaluate_models: dict[str, Model],
         project: Project,
         multitable: common._MultiTable,
     ):
         self.evaluate_models = evaluate_models
         self.project = project
         self.multitable = multitable
         self.completed = []
         self.failed = []
 
     def action(self, job: Job) -> str:
         return ACTION
 
     @property
-    def table_collection(self) -> List[str]:
+    def table_collection(self) -> list[str]:
         return list(self.evaluate_models.keys())
 
     @property
     def artifacts_per_job(self) -> int:
         return 2
 
     def more_to_do(self) -> bool:
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/synthetics_run.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/synthetics_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from pathlib import Path
-from typing import Dict, List, Optional
+from typing import Optional
 
 import pandas as pd
-from gretel_client.projects.jobs import ACTIVE_STATES, Job
+from gretel_client.projects.jobs import ACTIVE_STATES, Job, Status
 from gretel_client.projects.projects import Project
 from gretel_client.projects.records import RecordHandler
 
 import gretel_trainer.relational.tasks.common as common
 from gretel_trainer.relational.workflow_state import SyntheticsRun, SyntheticsTrain
 
 logger = logging.getLogger(__name__)
@@ -25,44 +25,50 @@
     ):
         self.synthetics_run = synthetics_run
         self.synthetics_train = synthetics_train
         self.run_dir = run_dir
         self.multitable = multitable
         self.working_tables = self._setup_working_tables()
 
-    def _setup_working_tables(self) -> Dict[str, Optional[pd.DataFrame]]:
+    def _setup_working_tables(self) -> dict[str, Optional[pd.DataFrame]]:
         working_tables = {}
+        all_tables = self.multitable.relational_data.list_all_tables()
 
-        for table in self.synthetics_run.missing_model:
-            working_tables[table] = None
+        for table in all_tables:
+            model = self.synthetics_train.models.get(table)
 
-        for table in self.synthetics_run.preserved:
-            working_tables[table] = self.multitable._strategy.get_preserved_data(
-                table, self.multitable.relational_data
-            )
+            # Table was either omitted from training or marked as to-be-preserved during generation
+            if model is None or table in self.synthetics_run.preserved:
+                working_tables[table] = self.multitable._strategy.get_preserved_data(
+                    table, self.multitable.relational_data
+                )
+
+            # Table was included in training, but failed at that step
+            elif model.status != Status.COMPLETED:
+                working_tables[table] = None
 
         return working_tables
 
     @property
-    def output_tables(self) -> Dict[str, pd.DataFrame]:
+    def output_tables(self) -> dict[str, pd.DataFrame]:
         return {
             table: data
             for table, data in self.working_tables.items()
             if data is not None
         }
 
     def action(self, job: Job) -> str:
         return ACTION
 
     @property
     def project(self) -> Project:
         return self.multitable._project
 
     @property
-    def table_collection(self) -> List[str]:
+    def table_collection(self) -> list[str]:
         return list(self.synthetics_run.record_handlers.keys())
 
     @property
     def artifacts_per_job(self) -> int:
         return 1
 
     def more_to_do(self) -> bool:
@@ -135,15 +141,14 @@
 
             table_job = self.multitable._strategy.get_generation_job(
                 table_name,
                 self.multitable.relational_data,
                 self.synthetics_run.record_size_ratio,
                 present_working_tables,
                 self.run_dir,
-                self.synthetics_train.training_columns[table_name],
             )
             model = self.synthetics_train.models[table_name]
             record_handler = model.create_record_handler_obj(**table_job)
             self.synthetics_run.record_handlers[table_name] = record_handler
             # Attempt starting the record handler right away. If it can't start right at this moment,
             # the regular task runner check will handle starting it when possible.
             self.multitable._extended_sdk.start_job_if_possible(
@@ -153,15 +158,15 @@
                 project=self.project,
                 number_of_artifacts=self.artifacts_per_job,
             )
 
         self.multitable._backup()
 
     @property
-    def _all_tables(self) -> List[str]:
+    def _all_tables(self) -> list[str]:
         return self.multitable.relational_data.list_all_tables()
 
     def _fail_table(self, table: str) -> None:
         self.working_tables[table] = None
         for other_table in self.multitable._strategy.tables_to_skip_when_failed(
             table, self.multitable.relational_data
         ):
@@ -172,15 +177,15 @@
 def _log_skipping(skip: str, failed_parent: str) -> None:
     logger.info(
         f"Skipping synthetic data generation for `{skip}` because it depends on `{failed_parent}`"
     )
 
 
 def _table_is_in_progress(
-    record_handlers: Dict[str, RecordHandler], table: str
+    record_handlers: dict[str, RecordHandler], table: str
 ) -> bool:
     in_progress = False
 
     record_handler = record_handlers.get(table)
     if record_handler is not None and record_handler.record_id is not None:
         in_progress = record_handler.status in ACTIVE_STATES
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/synthetics_train.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/synthetics_train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List
-
 from gretel_client.projects.jobs import Job
 from gretel_client.projects.projects import Project
 
 import gretel_trainer.relational.tasks.common as common
 from gretel_trainer.relational.workflow_state import SyntheticsTrain
 
 ACTION = "synthetics model training"
@@ -24,15 +22,15 @@
         return ACTION
 
     @property
     def project(self) -> Project:
         return self.multitable._project
 
     @property
-    def table_collection(self) -> List[str]:
+    def table_collection(self) -> list[str]:
         return list(self.synthetics_train.models.keys())
 
     @property
     def artifacts_per_job(self) -> int:
         return 1
 
     def more_to_do(self) -> bool:
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/transforms_run.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/transforms_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from typing import Dict, List, Optional
+from typing import Optional
 
 import pandas as pd
 from gretel_client.projects.jobs import Job
 from gretel_client.projects.projects import Project
 from gretel_client.projects.records import RecordHandler
 
 import gretel_trainer.relational.tasks.common as common
 
 ACTION = "transforms run"
 
 
 class TransformsRunTask:
     def __init__(
         self,
-        record_handlers: Dict[str, RecordHandler],
+        record_handlers: dict[str, RecordHandler],
         multitable: common._MultiTable,
     ):
         self.record_handlers = record_handlers
         self.multitable = multitable
-        self.working_tables: Dict[str, Optional[pd.DataFrame]] = {}
+        self.working_tables: dict[str, Optional[pd.DataFrame]] = {}
 
     @property
-    def output_tables(self) -> Dict[str, pd.DataFrame]:
+    def output_tables(self) -> dict[str, pd.DataFrame]:
         return {
             table: data
             for table, data in self.working_tables.items()
             if data is not None
         }
 
     def action(self, job: Job) -> str:
         return ACTION
 
     @property
     def project(self) -> Project:
         return self.multitable._project
 
     @property
-    def table_collection(self) -> List[str]:
+    def table_collection(self) -> list[str]:
         return list(self.record_handlers.keys())
 
     @property
     def artifacts_per_job(self) -> int:
         return 1
 
     def more_to_do(self) -> bool:
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/transforms_train.py` & `gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/transforms_train.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List
-
 from gretel_client.projects.jobs import Job
 from gretel_client.projects.projects import Project
 
 import gretel_trainer.relational.tasks.common as common
 from gretel_trainer.relational.workflow_state import TransformsTrain
 
 ACTION = "transforms model training"
@@ -24,15 +22,15 @@
         return ACTION
 
     @property
     def project(self) -> Project:
         return self.multitable._project
 
     @property
-    def table_collection(self) -> List[str]:
+    def table_collection(self) -> list[str]:
         return list(self.transforms_train.models.keys())
 
     @property
     def artifacts_per_job(self) -> int:
         return 1
 
     def more_to_do(self) -> bool:
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/runner.py` & `gretel-trainer-0.8.2/src/gretel_trainer/runner.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/strategy.py` & `gretel-trainer-0.8.2/src/gretel_trainer/strategy.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer/trainer.py` & `gretel-trainer-0.8.2/src/gretel_trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer.egg-info/PKG-INFO` & `gretel-trainer-0.8.2/src/gretel_trainer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gretel-trainer
-Version: 0.8.1
+Version: 0.8.2
 Summary: Synthetic Data Generation with optional Differential Privacy
 Home-page: https://github.com/gretelai/gretel-trainer
 License: https://gretel.ai/license/source-available-license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `gretel-trainer-0.8.1/src/gretel_trainer.egg-info/SOURCES.txt` & `gretel-trainer-0.8.2/src/gretel_trainer.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 src/gretel_trainer/relational/__init__.py
 src/gretel_trainer/relational/ancestry.py
 src/gretel_trainer/relational/artifacts.py
 src/gretel_trainer/relational/backup.py
 src/gretel_trainer/relational/connectors.py
 src/gretel_trainer/relational/core.py
 src/gretel_trainer/relational/drawing.py
+src/gretel_trainer/relational/json.py
 src/gretel_trainer/relational/log.py
 src/gretel_trainer/relational/model_config.py
 src/gretel_trainer/relational/multi_table.py
 src/gretel_trainer/relational/sdk_extras.py
 src/gretel_trainer/relational/table_evaluation.py
 src/gretel_trainer/relational/task_runner.py
 src/gretel_trainer/relational/workflow_state.py
@@ -97,16 +98,20 @@
 tests/relational/test_common_strategy.py
 tests/relational/test_connectors.py
 tests/relational/test_independent_strategy.py
 tests/relational/test_model_config.py
 tests/relational/test_multi_table_config_options.py
 tests/relational/test_multi_table_restore.py
 tests/relational/test_relational_data.py
+tests/relational/test_relational_data_with_json.py
 tests/relational/test_report.py
 tests/relational/test_synthetics_run_task.py
 tests/relational/test_task_runner.py
+tests/relational/test_train_synthetics.py
+tests/relational/test_train_transforms.py
 tests/relational/example_dbs/art.sql
+tests/relational/example_dbs/documents.sql
 tests/relational/example_dbs/ecom.sql
 tests/relational/example_dbs/mutagenesis.sql
 tests/relational/example_dbs/pets.sql
 tests/relational/example_dbs/tpch.sql
 tests/relational/example_dbs/trips.sql
```

### Comparing `gretel-trainer-0.8.1/tests/data/core-221-train.csv` & `gretel-trainer-0.8.2/tests/data/core-221-train.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/tests/mocks.py` & `gretel-trainer-0.8.2/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/tests/relational/conftest.py` & `gretel-trainer-0.8.2/tests/relational/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import sqlite3
 from pathlib import Path
-from typing import Tuple
 from unittest.mock import Mock, patch
 
 import pandas as pd
 import pytest
 from sqlalchemy import create_engine
 
 from gretel_trainer.relational.connectors import Connector
@@ -15,14 +14,21 @@
 
 
 @pytest.fixture()
 def extended_sdk():
     return ExtendedGretelSDK(hybrid=False)
 
 
+@pytest.fixture(autouse=True)
+def static_suffix():
+    with patch("gretel_trainer.relational.json.make_suffix") as make_suffix:
+        make_suffix.return_value = "sfx"
+        yield
+
+
 @pytest.fixture()
 def project():
     with patch(
         "gretel_trainer.relational.multi_table.create_project"
     ) as create_project, patch(
         "gretel_trainer.relational.multi_table.get_project"
     ) as get_project:
@@ -74,14 +80,19 @@
 
 @pytest.fixture()
 def art() -> RelationalData:
     return rel_data_from_example_db("art")
 
 
 @pytest.fixture()
+def documents() -> RelationalData:
+    return rel_data_from_example_db("documents")
+
+
+@pytest.fixture()
 def trips() -> RelationalData:
     rel_data = rel_data_from_example_db("trips")
     rel_data.update_table_data(
         table="trips",
         data=pd.DataFrame(
             data={
                 "id": list(range(100)),
@@ -90,26 +101,26 @@
             }
         ),
     )
     return rel_data
 
 
 @pytest.fixture()
-def source_nba() -> Tuple[RelationalData, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
+def source_nba() -> tuple[RelationalData, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
     return _setup_nba(synthetic=False)
 
 
 @pytest.fixture()
-def synthetic_nba() -> Tuple[RelationalData, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
+def synthetic_nba() -> tuple[RelationalData, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
     return _setup_nba(synthetic=True)
 
 
 def _setup_nba(
     synthetic: bool,
-) -> Tuple[RelationalData, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
+) -> tuple[RelationalData, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
     if synthetic:
         states = ["PA", "FL"]
         cities = ["Philadelphia", "Miami"]
         teams = ["Sixers", "Heat"]
     else:
         states = ["CA", "TN"]
         cities = ["Los Angeles", "Memphis"]
```

### Comparing `gretel-trainer-0.8.1/tests/relational/example_dbs/art.sql` & `gretel-trainer-0.8.2/tests/relational/example_dbs/art.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/tests/relational/example_dbs/ecom.sql` & `gretel-trainer-0.8.2/tests/relational/example_dbs/ecom.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/tests/relational/example_dbs/mutagenesis.sql` & `gretel-trainer-0.8.2/tests/relational/example_dbs/mutagenesis.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/tests/relational/example_dbs/pets.sql` & `gretel-trainer-0.8.2/tests/relational/example_dbs/pets.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/tests/relational/example_dbs/tpch.sql` & `gretel-trainer-0.8.2/tests/relational/example_dbs/tpch.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/tests/relational/test_ancestral_strategy.py` & `gretel-trainer-0.8.2/tests/relational/test_ancestral_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,26 +18,42 @@
     for rel_data in [pets, art]:
         original_tables = {
             table: rel_data.get_table_data(table).copy()
             for table in rel_data.list_all_tables()
         }
 
         strategy = AncestralStrategy()
-        strategy.prepare_training_data(rel_data)
+        strategy.prepare_training_data(rel_data, rel_data.list_all_tables())
 
         for table in rel_data.list_all_tables():
             pdtest.assert_frame_equal(
                 original_tables[table], rel_data.get_table_data(table)
             )
 
 
+def test_prepare_training_data_subset_of_tables(pets):
+    strategy = AncestralStrategy()
+
+    # We aren't synthesizing the "humans" table, so it is not in this list argument...
+    training_data = strategy.prepare_training_data(pets, ["pets"])
+    # ...nor do we create training data for it
+    assert set(training_data.keys()) == {"pets"}
+
+    # Since the humans table is omitted from synthetics, we leave the FK values alone; specifically:
+    # - they are not label-encoded (which would effectively zero-index them)
+    # - we do not add artificial min/max values
+    assert set(training_data["pets"]["self|human_id"].values) == {1, 2, 3, 4, 5}
+    # We do add the artificial max PK row, though, since this table is being synthesized
+    assert len(training_data["pets"]) == 6
+
+
 def test_prepare_training_data_returns_multigenerational_data(pets):
     strategy = AncestralStrategy()
 
-    training_data = strategy.prepare_training_data(pets)
+    training_data = strategy.prepare_training_data(pets, pets.list_all_tables())
 
     for expected_column in ["self|id", "self|name", "self.human_id|id"]:
         assert expected_column in training_data["pets"]
 
 
 def test_prepare_training_data_drops_highly_unique_categorical_ancestor_fields(art):
     art.update_table_data(
@@ -57,15 +73,15 @@
                 "artist_id": [f"A{i}" for i in range(100)],
                 "name": [str(i) for i in range(100)],
             }
         ),
     )
 
     strategy = AncestralStrategy()
-    training_data = strategy.prepare_training_data(art)
+    training_data = strategy.prepare_training_data(art, art.list_all_tables())
 
     # Does not contain `self.artist_id|name` because it is highly unique categorical
     assert set(training_data["paintings"].columns) == {
         "self|id",
         "self|name",
         "self|artist_id",
         "self.artist_id|id",
@@ -96,30 +112,30 @@
                 "artist_id": [f"A{i}" for i in range(100)],
                 "name": [str(i) for i in range(100)],
             }
         ),
     )
 
     strategy = AncestralStrategy()
-    training_data = strategy.prepare_training_data(art)
+    training_data = strategy.prepare_training_data(art, art.list_all_tables())
 
     # Does not contain `self.artist_id|name` because it is highly NaN
     assert set(training_data["paintings"].columns) == {
         "self|id",
         "self|name",
         "self|artist_id",
         "self.artist_id|id",
     }
 
 
 def test_prepare_training_data_translates_alphanumeric_keys_and_adds_min_max_records(
     art,
 ):
     strategy = AncestralStrategy()
-    training_data = strategy.prepare_training_data(art)
+    training_data = strategy.prepare_training_data(art, art.list_all_tables())
 
     # Artists, a parent table, should have 1 additional row
     assert len(training_data["artists"]) == len(art.get_table_data("artists")) + 1
     # The last record has the artifical max PK
     assert training_data["artists"]["self|id"].to_list() == [0, 1, 2, 3, 200]
     # We do not assert on the value of "self|name" because the artificial max PK record is
     # randomly sampled from source and so the exact value is not deterministic
@@ -138,15 +154,15 @@
     # FKs on last two rows (artifical FKs) are min, max
     assert last_two["self|artist_id"].to_list() == [0, 200]
     assert last_two["self.artist_id|id"].to_list() == [0, 200]
 
 
 def test_prepare_training_data_with_composite_keys(tpch):
     strategy = AncestralStrategy()
-    training_data = strategy.prepare_training_data(tpch)
+    training_data = strategy.prepare_training_data(tpch, tpch.list_all_tables())
 
     l_max = len(tpch.get_table_data("lineitem")) * 50
     ps_max = len(tpch.get_table_data("partsupp")) * 50
     p_max = len(tpch.get_table_data("part")) * 50
     s_max = len(tpch.get_table_data("supplier")) * 50
 
     # partsupp table, composite PK
@@ -335,36 +351,19 @@
         == set()
     )
 
 
 def test_generation_job(pets):
     strategy = AncestralStrategy()
 
-    training_columns = {
-        "humans": [
-            "self|id",
-            "self|name",
-            "self|city",
-        ],
-        "pets": [
-            "self|id",
-            "self|name",
-            "self|age",
-            "self|human_id",
-            "self.human_id|id",
-            # "self.human_id|name", # highly unique categorical
-            "self.human_id|city",
-        ],
-    }
-
     # Table with no ancestors
     with tempfile.TemporaryDirectory() as tmp:
         working_dir = Path(tmp)
         parent_table_job = strategy.get_generation_job(
-            "humans", pets, 2.0, {}, working_dir, training_columns["humans"]
+            "humans", pets, 2.0, {}, working_dir
         )
         assert len(os.listdir(working_dir)) == 0
         assert parent_table_job == {"params": {"num_records": 10}}
 
     # Table with ancestors
     synthetic_humans = pd.DataFrame(
         data={
@@ -385,15 +384,15 @@
             "self|id": [1, 2, 3, 4, 5],
         }
     )
     output_tables = {"humans": synthetic_humans}
     with tempfile.TemporaryDirectory() as tmp:
         working_dir = Path(tmp)
         child_table_job = strategy.get_generation_job(
-            "pets", pets, 2.0, output_tables, working_dir, training_columns["pets"]
+            "pets", pets, 2.0, output_tables, working_dir
         )
 
         assert len(os.listdir(working_dir)) == 1
         assert set(child_table_job.keys()) == {"data_source"}
         child_table_seed_df = pd.read_csv(child_table_job["data_source"])
 
     # `self.human_id|name` should not be present in seed because it was
@@ -425,49 +424,25 @@
 def test_generation_job_seeds_go_back_multiple_generations(source_nba, synthetic_nba):
     source_nba = source_nba[0]
     synthetic_nba = synthetic_nba[0]
     output_tables = {
         "cities": ancestry.get_table_data_with_ancestors(synthetic_nba, "cities"),
         "states": ancestry.get_table_data_with_ancestors(synthetic_nba, "states"),
     }
-    training_columns = {
-        "teams": [
-            "self|name",
-            "self|id",
-            "self|city_id",
-            "self.city_id|id",
-            "self.city_id|state_id",
-            # "self.city_id|name", # highly unique categorical
-            "self.city_id.state_id|id",
-            # "self.city_id.state_id|name", # highly unique categorical
-        ],
-        "cities": [
-            "self|id",
-            "self|state_id",
-            # "self|name", # highly unique categorical
-            "self.state_id|id",
-            # "self.state_id|name", # highly unique categorical
-        ],
-        "states": [
-            "self|id",
-            "self|name",
-        ],
-    }
 
     strategy = AncestralStrategy()
 
     with tempfile.TemporaryDirectory() as tmp:
         working_dir = Path(tmp)
         job = strategy.get_generation_job(
             "teams",
             source_nba,
             1.0,
             output_tables,
             working_dir,
-            training_columns["teams"],
         )
         seed_df = pd.read_csv(job["data_source"])
 
     expected_seed_df_columns = {
         "self.city_id|id",
         # "self.city_id|name", # highly unique categorical
         "self.city_id|state_id",
```

### Comparing `gretel-trainer-0.8.1/tests/relational/test_ancestry.py` & `gretel-trainer-0.8.2/tests/relational/test_ancestry.py`

 * *Files 26% similar despite different names*

```diff
@@ -183,7 +183,61 @@
         "self.inventory_item_id.product_id|brand",
         "self.inventory_item_id.product_id|distribution_center_id",
         "self.inventory_item_id.product_distribution_center_id|id",
         "self.inventory_item_id.product_distribution_center_id|name",
         "self.inventory_item_id.product_id.distribution_center_id|id",
         "self.inventory_item_id.product_id.distribution_center_id|name",
     }
+
+
+def test_get_seed_safe_multigenerational_columns_1(pets):
+    table_cols = ancestry.get_seed_safe_multigenerational_columns(pets)
+
+    expected = {
+        "humans": {"self|id", "self|name", "self|city"},
+        "pets": {
+            "self|id",
+            "self|name",
+            "self|age",
+            "self|human_id",
+            "self.human_id|id",
+            # "self.human_id|name", # highly unique categorical
+            "self.human_id|city",
+        },
+    }
+
+    assert set(table_cols.keys()) == set(expected.keys())
+    for table, expected_cols in expected.items():
+        assert set(table_cols[table]) == expected_cols
+
+
+def test_get_seed_safe_multigenerational_columns_2(source_nba):
+    source_nba = source_nba[0]
+    table_cols = ancestry.get_seed_safe_multigenerational_columns(source_nba)
+
+    expected = {
+        "teams": {
+            "self|name",
+            "self|id",
+            "self|city_id",
+            "self.city_id|id",
+            "self.city_id|state_id",
+            # "self.city_id|name", # highly unique categorical
+            "self.city_id.state_id|id",
+            # "self.city_id.state_id|name", # highly unique categorical
+        },
+        "cities": {
+            "self|id",
+            "self|state_id",
+            "self|name",
+            "self.state_id|id",
+            # "self.state_id|name", # highly unique categorical
+        },
+        "states": {
+            "self|id",
+            "self|name",
+        },
+    }
+
+    assert set(table_cols.keys()) == set(expected.keys())
+    for table, expected_cols in expected.items():
+        assert set(table_cols[table]) == expected_cols
```

### Comparing `gretel-trainer-0.8.1/tests/relational/test_artifacts.py` & `gretel-trainer-0.8.2/tests/relational/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/tests/relational/test_backup.py` & `gretel-trainer-0.8.2/tests/relational/test_backup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from gretel_trainer.relational.backup import (
     Backup,
     BackupClassify,
     BackupForeignKey,
     BackupGenerate,
     BackupRelationalData,
     BackupRelationalDataTable,
+    BackupRelationalJson,
     BackupSyntheticsTrain,
     BackupTransformsTrain,
 )
 
 
 def test_backup_relational_data(trips):
     expected = BackupRelationalData(
@@ -23,19 +24,78 @@
             BackupForeignKey(
                 table="trips",
                 constrained_columns=["vehicle_type_id"],
                 referred_table="vehicle_types",
                 referred_columns=["id"],
             )
         ],
+        relational_jsons={},
     )
 
     assert BackupRelationalData.from_relational_data(trips) == expected
 
 
+def test_backup_relational_data_with_json(documents):
+    expected = BackupRelationalData(
+        tables={
+            "users": BackupRelationalDataTable(primary_key=["id"]),
+            "purchases-sfx": BackupRelationalDataTable(
+                primary_key=["id", "~PRIMARY_KEY_ID~"],
+                invented_table_metadata={
+                    "invented_root_table_name": "purchases-sfx",
+                    "original_table_name": "purchases",
+                    "empty": False,
+                },
+            ),
+            "purchases-data-years-sfx": BackupRelationalDataTable(
+                primary_key=["~PRIMARY_KEY_ID~"],
+                invented_table_metadata={
+                    "invented_root_table_name": "purchases-sfx",
+                    "original_table_name": "purchases",
+                    "empty": False,
+                },
+            ),
+            "payments": BackupRelationalDataTable(primary_key=["id"]),
+        },
+        foreign_keys=[
+            BackupForeignKey(
+                table="payments",
+                constrained_columns=["purchase_id"],
+                referred_table="purchases-sfx",
+                referred_columns=["id"],
+            ),
+            BackupForeignKey(
+                table="purchases-sfx",
+                constrained_columns=["user_id"],
+                referred_table="users",
+                referred_columns=["id"],
+            ),
+            BackupForeignKey(
+                table="purchases-data-years-sfx",
+                constrained_columns=["purchases~id"],
+                referred_table="purchases-sfx",
+                referred_columns=["~PRIMARY_KEY_ID~"],
+            ),
+        ],
+        relational_jsons={
+            "purchases": BackupRelationalJson(
+                original_table_name="purchases",
+                original_primary_key=["id"],
+                original_columns=["id", "user_id", "data"],
+                table_name_mappings={
+                    "purchases": "purchases-sfx",
+                    "purchases^data>years": "purchases-data-years-sfx",
+                },
+            ),
+        },
+    )
+
+    assert BackupRelationalData.from_relational_data(documents) == expected
+
+
 def test_backup():
     backup_relational = BackupRelationalData(
         tables={
             "customer": BackupRelationalDataTable(
                 primary_key=["id"],
             ),
             "address": BackupRelationalDataTable(
@@ -46,14 +106,15 @@
             BackupForeignKey(
                 table="address",
                 constrained_columns=["customer_id"],
                 referred_table="customer",
                 referred_columns=["id"],
             )
         ],
+        relational_jsons={},
     )
     backup_classify = BackupClassify(
         model_ids={
             "customer": "aaabbbccc",
             "address": "dddeeefff",
         },
     )
@@ -65,26 +126,21 @@
         lost_contact=[],
     )
     backup_synthetics_train = BackupSyntheticsTrain(
         model_ids={
             "customer": "1234567890",
             "address": "0987654321",
         },
-        training_columns={
-            "customer": ["id", "first", "last"],
-            "address": ["customer_id", "street", "city"],
-        },
         lost_contact=[],
     )
     backup_generate = BackupGenerate(
         identifier="run-id",
         preserved=[],
         record_size_ratio=1.0,
         lost_contact=[],
-        missing_model=[],
         record_handler_ids={
             "customer": "555444666",
             "address": "333111222",
         },
     )
     artifact_collection = ArtifactCollection(
         gretel_debug_summary="gretel_abc__gretel_debug_summary.json",
```

### Comparing `gretel-trainer-0.8.1/tests/relational/test_common_strategy.py` & `gretel-trainer-0.8.2/tests/relational/test_common_strategy.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/tests/relational/test_connectors.py` & `gretel-trainer-0.8.2/tests/relational/test_connectors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import sqlite3
 import tempfile
 
 import pytest
 
 from gretel_trainer.relational.connectors import sqlite_conn
-from gretel_trainer.relational.core import MultiTableException
+from gretel_trainer.relational.core import MultiTableException, Scope
 
 
 def test_extract_subsets_of_relational_data(example_dbs):
     with tempfile.NamedTemporaryFile() as f:
         con = sqlite3.connect(f.name)
         cur = con.cursor()
         with open(example_dbs / "ecom.sql") as sql_script:
             cur.executescript(sql_script.read())
 
         connector = sqlite_conn(f.name)
 
         with pytest.raises(MultiTableException):
-            connector.extract(only=["users"], ignore=["events"])
+            connector.extract(only={"users"}, ignore={"events"})
 
-        only = connector.extract(only=["users", "events", "products"])
+        only = connector.extract(only={"users", "events", "products"})
         ignore = connector.extract(
-            ignore=["distribution_center", "order_items", "inventory_items"]
+            ignore={"distribution_center", "order_items", "inventory_items"}
         )
 
     expected_tables = {"users", "events", "products"}
-    assert set(only.list_all_tables()) == expected_tables
-    assert set(ignore.list_all_tables()) == expected_tables
+    assert set(only.list_all_tables(Scope.ALL)) == expected_tables
+    assert set(ignore.list_all_tables(Scope.ALL)) == expected_tables
 
     # `products` has a foreign key to `distribution_center` in the source, but because the
     # latter table was not extracted, the relationship is not recognized
     assert only.get_parents("products") == []
     assert ignore.get_parents("products") == []
```

### Comparing `gretel-trainer-0.8.1/tests/relational/test_independent_strategy.py` & `gretel-trainer-0.8.2/tests/relational/test_independent_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,30 +15,38 @@
     for rel_data in [pets, art]:
         original_tables = {
             table: rel_data.get_table_data(table).copy()
             for table in rel_data.list_all_tables()
         }
 
         strategy = IndependentStrategy()
-        strategy.prepare_training_data(rel_data)
+        strategy.prepare_training_data(rel_data, rel_data.list_all_tables())
 
         for table in rel_data.list_all_tables():
             pdtest.assert_frame_equal(
                 original_tables[table], rel_data.get_table_data(table)
             )
 
 
 def test_prepare_training_data_removes_primary_and_foreign_keys(pets):
     strategy = IndependentStrategy()
 
-    training_data = strategy.prepare_training_data(pets)
+    training_data = strategy.prepare_training_data(pets, pets.list_all_tables())
 
     assert set(training_data["pets"].columns) == {"name", "age"}
 
 
+def test_prepare_training_data_subset_of_tables(pets):
+    strategy = IndependentStrategy()
+
+    training_data = strategy.prepare_training_data(pets, ["humans"])
+
+    assert set(training_data.keys()) == {"humans"}
+
+
 def test_retraining_a_set_of_tables_only_retrains_those_tables(ecom):
     strategy = IndependentStrategy()
     assert set(strategy.tables_to_retrain(["users"], ecom)) == {"users"}
     assert set(strategy.tables_to_retrain(["users", "events"], ecom)) == {
         "users",
         "events",
     }
@@ -65,15 +73,15 @@
         "inventory_items",
         "order_items",
     }
 
 
 def test_generation_job_requests_num_records(pets):
     strategy = IndependentStrategy()
-    job = strategy.get_generation_job("pets", pets, 2.0, {}, Path("/working"), [])
+    job = strategy.get_generation_job("pets", pets, 2.0, {}, Path("/working"))
 
     assert job == {"params": {"num_records": 10}}
 
 
 def test_post_processing_one_to_one(pets):
     strategy = IndependentStrategy()
```

### Comparing `gretel-trainer-0.8.1/tests/relational/test_model_config.py` & `gretel-trainer-0.8.2/tests/relational/test_model_config.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/tests/relational/test_multi_table_config_options.py` & `gretel-trainer-0.8.2/tests/relational/test_multi_table_config_options.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/tests/relational/test_multi_table_restore.py` & `gretel-trainer-0.8.2/tests/relational/test_multi_table_restore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import shutil
 import tarfile
 import tempfile
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Optional
 from unittest.mock import Mock, patch
 
 import pytest
 
 import gretel_trainer.relational.backup as b
 from gretel_trainer.relational.artifacts import ArtifactCollection
 from gretel_trainer.relational.core import MultiTableException, RelationalData
@@ -60,17 +60,17 @@
 }
 
 
 def make_backup(
     rel_data: RelationalData,
     working_dir: Path,
     artifact_collection: ArtifactCollection,
-    transforms_models: Dict[str, Mock] = {},
-    synthetics_models: Dict[str, Mock] = {},
-    synthetics_record_handlers: Dict[str, Mock] = {},
+    transforms_models: dict[str, Mock] = {},
+    synthetics_models: dict[str, Mock] = {},
+    synthetics_record_handlers: dict[str, Mock] = {},
 ) -> b.Backup:
     backup = b.Backup(
         project_name="project_name",
         strategy="independent",
         gretel_model="amplify",
         refresh_interval=60,
         working_dir=str(working_dir),
@@ -85,24 +85,22 @@
             lost_contact=[],
         )
     if len(synthetics_models) > 0:
         backup.synthetics_train = b.BackupSyntheticsTrain(
             model_ids={
                 table: mock.model_id for table, mock in synthetics_models.items()
             },
-            training_columns={table: ["col1", "col2"] for table in synthetics_models},
             lost_contact=[],
         )
     if len(synthetics_record_handlers) > 0:
         backup.generate = b.BackupGenerate(
             identifier="run-id",
             preserved=[],
             record_size_ratio=1.0,
             lost_contact=[],
-            missing_model=[],
             record_handler_ids={
                 table: mock.record_id
                 for table, mock in synthetics_record_handlers.items()
             },
         )
     return backup
 
@@ -113,19 +111,19 @@
         json.dump(backup.as_dict, b)
     return str(dest)
 
 
 def create_backup(
     rel_data: RelationalData,
     working_dir: Path,
-    synthetics_models: Dict[str, Mock] = {},
-    synthetics_record_handlers: Dict[str, Mock] = {},
+    synthetics_models: dict[str, Mock] = {},
+    synthetics_record_handlers: dict[str, Mock] = {},
     training_archive_present: bool = False,
     output_archive_present: bool = False,
-    transforms_models: Dict[str, Mock] = {},
+    transforms_models: dict[str, Mock] = {},
 ) -> str:
     artifact_collection = ArtifactCollection(
         gretel_debug_summary=ARTIFACTS["debug_summary"]["artifact_id"],
         source_archive=ARTIFACTS["source_archive"]["artifact_id"],
         hybrid=False,
     )
     if training_archive_present:
@@ -172,15 +170,15 @@
         src = setup_path / local_name
         dest = working_path / local_name
         shutil.copyfile(src, dest)
 
     return download_tar_artifact
 
 
-def make_mock_get_model(models: Dict[str, Mock]):
+def make_mock_get_model(models: dict[str, Mock]):
     def get_model(model_id):
         return models[model_id]
 
     return get_model
 
 
 def make_mock_model(
@@ -304,15 +302,15 @@
 # in the test setup dir in place of HTTPS links (smart_open can treat these identically).
 # For tar files, though, which require using requests, we patch the entire download_tar_artifact function
 def configure_mocks(
     project: Mock,
     download_tar_artifact: Mock,
     setup_path: Path,
     working_path: Path,
-    models: Dict[str, Mock] = {},
+    models: dict[str, Mock] = {},
 ) -> None:
     project.get_artifact_link = make_mock_get_artifact_link(setup_path)
     project.get_model = make_mock_get_model(models)
     download_tar_artifact.side_effect = make_mock_download_tar_artifact(
         setup_path,
         working_path,
     )
@@ -668,15 +666,14 @@
 
     # Generate state is partially restored
     assert mt._synthetics_run == SyntheticsRun(
         identifier="run-id",
         preserved=[],
         record_size_ratio=1.0,
         lost_contact=[],
-        missing_model=[],
         record_handlers=synthetics_record_handlers,
     )
     assert len(mt.synthetic_output_tables) == 0
     assert mt.evaluations["humans"].individual_sqs == 95
     assert mt.evaluations["humans"].cross_table_sqs is None
     assert mt.evaluations["pets"].individual_sqs == 95
     assert mt.evaluations["pets"].cross_table_sqs is None
```

### Comparing `gretel-trainer-0.8.1/tests/relational/test_relational_data.py` & `gretel-trainer-0.8.2/tests/relational/test_relational_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import os
-import tempfile
-
 import pandas as pd
 import pytest
 
 from gretel_trainer.relational.core import MultiTableException, RelationalData
 
 
 def test_ecommerce_relational_data(ecom):
@@ -218,149 +215,60 @@
     assert in_order(tables, "distribution_center", "products")
     assert in_order(tables, "distribution_center", "inventory_items")
     assert in_order(tables, "products", "inventory_items")
     assert in_order(tables, "inventory_items", "order_items")
     assert in_order(tables, "users", "order_items")
 
 
-def test_relational_data_as_dict(ecom):
-    as_dict = ecom.as_dict("test_out")
-
-    assert as_dict["tables"] == {
-        "users": {"primary_key": ["id"], "csv_path": "test_out/users.csv"},
-        "events": {"primary_key": ["id"], "csv_path": "test_out/events.csv"},
-        "distribution_center": {
-            "primary_key": ["id"],
-            "csv_path": "test_out/distribution_center.csv",
-        },
-        "products": {"primary_key": ["id"], "csv_path": "test_out/products.csv"},
-        "inventory_items": {
-            "primary_key": ["id"],
-            "csv_path": "test_out/inventory_items.csv",
-        },
-        "order_items": {"primary_key": ["id"], "csv_path": "test_out/order_items.csv"},
-    }
-    expected_foreign_keys = [
-        {
-            "table": "events",
-            "constrained_columns": ["user_id"],
-            "referred_table": "users",
-            "referred_columns": ["id"],
-        },
-        {
-            "table": "order_items",
-            "constrained_columns": ["user_id"],
-            "referred_table": "users",
-            "referred_columns": ["id"],
-        },
-        {
-            "table": "order_items",
-            "constrained_columns": ["inventory_item_id"],
-            "referred_table": "inventory_items",
-            "referred_columns": ["id"],
-        },
-        {
-            "table": "inventory_items",
-            "constrained_columns": ["product_id"],
-            "referred_table": "products",
-            "referred_columns": ["id"],
-        },
-        {
-            "table": "inventory_items",
-            "constrained_columns": ["product_distribution_center_id"],
-            "referred_table": "distribution_center",
-            "referred_columns": ["id"],
-        },
-        {
-            "table": "products",
-            "constrained_columns": ["distribution_center_id"],
-            "referred_table": "distribution_center",
-            "referred_columns": ["id"],
-        },
-    ]
-    for expected_fk in expected_foreign_keys:
-        assert expected_fk in as_dict["foreign_keys"]
-
-
-def test_ecommerce_filesystem_serde(ecom):
-    with tempfile.TemporaryDirectory() as tmp:
-        ecom.to_filesystem(tmp)
-
-        expected_files = [
-            f"{tmp}/metadata.json",
-            f"{tmp}/events.csv",
-            f"{tmp}/users.csv",
-            f"{tmp}/distribution_center.csv",
-            f"{tmp}/products.csv",
-            f"{tmp}/inventory_items.csv",
-            f"{tmp}/order_items.csv",
-        ]
-        for expected_file in expected_files:
-            assert os.path.exists(expected_file)
-
-        from_json = RelationalData.from_filesystem(f"{tmp}/metadata.json")
-
-    for table in ecom.list_all_tables():
-        assert set(ecom.get_table_data(table).columns) == set(
-            from_json.get_table_data(table).columns
-        )
-        assert ecom.get_parents(table) == from_json.get_parents(table)
-        assert ecom.get_foreign_keys(table) == from_json.get_foreign_keys(table)
-
-
-def test_filesystem_serde_accepts_composite_primary_keys(mutagenesis):
-    with tempfile.TemporaryDirectory() as tmp:
-        mutagenesis.to_filesystem(tmp)
-        from_json = RelationalData.from_filesystem(f"{tmp}/metadata.json")
-
-    assert from_json.get_primary_key("bond") == ["atom1_id", "atom2_id"]
-    assert from_json.get_primary_key("atom") == ["atom_id"]
-
-
 def test_debug_summary(ecom, mutagenesis):
     assert ecom.debug_summary() == {
         "foreign_key_count": 6,
         "max_depth": 3,
-        "table_count": 6,
+        "public_table_count": 6,
+        "invented_table_count": 0,
         "tables": {
             "users": {
                 "column_count": 3,
                 "primary_key": ["id"],
                 "foreign_key_count": 0,
                 "foreign_keys": [],
+                "is_invented_table": False,
             },
             "events": {
                 "column_count": 4,
                 "primary_key": ["id"],
                 "foreign_key_count": 1,
                 "foreign_keys": [
                     {
                         "columns": ["user_id"],
                         "parent_table_name": "users",
                         "parent_columns": ["id"],
                     }
                 ],
+                "is_invented_table": False,
             },
             "distribution_center": {
                 "column_count": 2,
                 "primary_key": ["id"],
                 "foreign_key_count": 0,
                 "foreign_keys": [],
+                "is_invented_table": False,
             },
             "products": {
                 "column_count": 4,
                 "primary_key": ["id"],
                 "foreign_key_count": 1,
                 "foreign_keys": [
                     {
                         "columns": ["distribution_center_id"],
                         "parent_table_name": "distribution_center",
                         "parent_columns": ["id"],
                     }
                 ],
+                "is_invented_table": False,
             },
             "inventory_items": {
                 "column_count": 5,
                 "primary_key": ["id"],
                 "foreign_key_count": 2,
                 "foreign_keys": [
                     {
@@ -370,14 +278,15 @@
                     },
                     {
                         "columns": ["product_distribution_center_id"],
                         "parent_table_name": "distribution_center",
                         "parent_columns": ["id"],
                     },
                 ],
+                "is_invented_table": False,
             },
             "order_items": {
                 "column_count": 5,
                 "primary_key": ["id"],
                 "foreign_key_count": 2,
                 "foreign_keys": [
                     {
@@ -387,22 +296,24 @@
                     },
                     {
                         "columns": ["inventory_item_id"],
                         "parent_table_name": "inventory_items",
                         "parent_columns": ["id"],
                     },
                 ],
+                "is_invented_table": False,
             },
         },
     }
 
     assert mutagenesis.debug_summary() == {
         "foreign_key_count": 3,
         "max_depth": 2,
-        "table_count": 3,
+        "public_table_count": 3,
+        "invented_table_count": 0,
         "tables": {
             "bond": {
                 "column_count": 3,
                 "primary_key": ["atom1_id", "atom2_id"],
                 "foreign_key_count": 2,
                 "foreign_keys": [
                     {
@@ -412,28 +323,31 @@
                     },
                     {
                         "columns": ["atom2_id"],
                         "parent_table_name": "atom",
                         "parent_columns": ["atom_id"],
                     },
                 ],
+                "is_invented_table": False,
             },
             "atom": {
                 "column_count": 4,
                 "primary_key": ["atom_id"],
                 "foreign_key_count": 1,
                 "foreign_keys": [
                     {
                         "columns": ["molecule_id"],
                         "parent_table_name": "molecule",
                         "parent_columns": ["molecule_id"],
                     }
                 ],
+                "is_invented_table": False,
             },
             "molecule": {
                 "column_count": 2,
                 "primary_key": ["molecule_id"],
                 "foreign_key_count": 0,
                 "foreign_keys": [],
+                "is_invented_table": False,
             },
         },
     }
```

### Comparing `gretel-trainer-0.8.1/tests/relational/test_synthetics_run_task.py` & `gretel-trainer-0.8.2/tests/relational/test_synthetics_run_task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import tempfile
 from dataclasses import dataclass
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import Optional, Union
 from unittest.mock import Mock, patch
 
 import pandas as pd
 import pandas.testing as pdtest
 import pytest
+from gretel_client.projects.jobs import Status
 from gretel_client.projects.projects import Project
 
 from gretel_trainer.relational.core import RelationalData
 from gretel_trainer.relational.sdk_extras import (
     MAX_PROJECT_ARTIFACTS,
     ExtendedGretelSDK,
 )
@@ -37,65 +38,74 @@
     with tempfile.TemporaryDirectory() as tmpdir:
         yield Path(tmpdir)
 
 
 def make_task(
     rel_data: RelationalData,
     run_dir: Path,
-    preserved: Optional[List[str]] = None,
-    missing_model: Optional[List[str]] = None,
+    preserved: Optional[list[str]] = None,
+    failed: Optional[list[str]] = None,
+    omitted: Optional[list[str]] = None,
 ) -> SyntheticsRunTask:
+    def _status_for_table(table: str, failed: list[str]) -> Status:
+        if table in failed:
+            return Status.ERROR
+        else:
+            return Status.COMPLETED
+
     multitable = MockMultiTable(relational_data=rel_data)
     return SyntheticsRunTask(
         synthetics_run=SyntheticsRun(
             identifier="generate",
             record_handlers={},
             lost_contact=[],
             preserved=preserved or [],
-            missing_model=missing_model or [],
             record_size_ratio=1.0,
         ),
         synthetics_train=SyntheticsTrain(
-            training_columns={
-                table: list(rel_data.get_table_data(table).columns)
-                for table in rel_data.list_all_tables()
-            },
             models={
-                table: Mock(create_record_handler=Mock())
+                table: Mock(
+                    create_record_handler=Mock(),
+                    status=_status_for_table(table, failed or []),
+                )
                 for table in rel_data.list_all_tables()
+                if table not in (omitted or [])
             },
         ),
         run_dir=run_dir,
         multitable=multitable,
     )
 
 
 def test_ignores_preserved_tables(pets, tmpdir):
     task = make_task(pets, tmpdir, preserved=["pets"])
 
+    # Source data is used
     assert task.working_tables["pets"] is not None
     assert "pets" in task.output_tables
     task.each_iteration()
     assert "pets" not in task.synthetics_run.record_handlers
 
 
-def test_ignores_tables_that_failed_to_train(pets, tmpdir):
-    task = make_task(pets, tmpdir, missing_model=["pets"])
+def test_ignores_tables_that_were_omitted_from_training(pets, tmpdir):
+    task = make_task(pets, tmpdir, omitted=["pets"])
 
-    assert task.working_tables["pets"] is None
-    assert "pets" not in task.output_tables
+    # Source data is used
+    assert task.working_tables["pets"] is not None
+    assert "pets" in task.output_tables
     task.each_iteration()
     assert "pets" not in task.synthetics_run.record_handlers
 
 
-def test_preserve_takes_precedence_over_missing_model(pets, tmpdir):
-    task = make_task(pets, tmpdir, preserved=["pets"], missing_model=["pets"])
+def test_ignores_tables_that_failed_during_training(pets, tmpdir):
+    task = make_task(pets, tmpdir, failed=["pets"])
 
-    assert task.working_tables["pets"] is not None
-    assert "pets" in task.output_tables
+    # We set tables that failed to explicit None
+    assert task.working_tables["pets"] is None
+    assert "pets" not in task.output_tables
     task.each_iteration()
     assert "pets" not in task.synthetics_run.record_handlers
 
 
 def test_runs_post_processing_when_table_completes(pets, tmpdir):
     task = make_task(pets, tmpdir)
```

### Comparing `gretel-trainer-0.8.1/tests/relational/test_task_runner.py` & `gretel-trainer-0.8.2/tests/relational/test_task_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import List
 from unittest.mock import Mock, PropertyMock, patch
 
 import pytest
 from gretel_client.projects.jobs import Job, Status
 
 from gretel_trainer.relational.sdk_extras import MAX_PROJECT_ARTIFACTS
 from gretel_trainer.relational.task_runner import run_task
@@ -25,15 +24,15 @@
         return 3
 
     @property
     def multitable(self):
         return Mock()
 
     @property
-    def table_collection(self) -> List[str]:
+    def table_collection(self) -> list[str]:
         return list(self.models.keys())
 
     def more_to_do(self) -> bool:
         return len(self.completed + self.failed + self.lost_contact) < len(self.models)
 
     def wait(self) -> None:
         pass
```

### Comparing `gretel-trainer-0.8.1/tests/test_benchmark.py` & `gretel-trainer-0.8.2/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.1/tests/test_strategy.py` & `gretel-trainer-0.8.2/tests/test_strategy.py`

 * *Files identical despite different names*

