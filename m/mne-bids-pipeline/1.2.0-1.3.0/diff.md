# Comparing `tmp/mne-bids-pipeline-1.2.0.tar.gz` & `tmp/mne-bids-pipeline-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mne-bids-pipeline-1.2.0.tar", last modified: Thu Mar 23 14:44:12 2023, max compression
+gzip compressed data, was "mne-bids-pipeline-1.3.0.tar", last modified: Thu Jun  1 14:51:09 2023, max compression
```

## Comparing `mne-bids-pipeline-1.2.0.tar` & `mne-bids-pipeline-1.3.0.tar`

### file list

```diff
@@ -1,177 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.082526 mne-bids-pipeline-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.066526 mne-bids-pipeline-1.2.0/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)    39920 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/.circleci/config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     3068 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/.circleci/setup_bash.sh
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.066526 mne-bids-pipeline-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/.github/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.066526 mne-bids-pipeline-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/.github/workflows/circleci-redirector.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/BUILDING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-03-23 14:44:12.082526 mne-bids-pipeline-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.066526 mne-bids-pipeline-1.2.0/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/build-docs.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.066526 mne-bids-pipeline-1.2.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.070526 mne-bids-pipeline-1.2.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.070526 mne-bids-pipeline-1.2.0/docs/source/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    97580 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/assets/mne.svg
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/changes.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.070526 mne-bids-pipeline-1.2.0/docs/source/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/doc-config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.070526 mne-bids-pipeline-1.2.0/docs/source/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10313 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/examples/gen_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.070526 mne-bids-pipeline-1.2.0/docs/source/features/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1618 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/features/gen_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/features/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.070526 mne-bids-pipeline-1.2.0/docs/source/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/getting_started/basic_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/getting_started/freesurfer.md
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/getting_started/install.md
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/governance.md
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.070526 mne-bids-pipeline-1.2.0/docs/source/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/general.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.070526 mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/artifacts.md
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/autobads.md
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/breaks.md
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/epochs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/filter.md
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/maxfilter.md
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/resample.md
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/ssp_ica.md
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/stim_artifact.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.070526 mne-bids-pipeline-1.2.0/docs/source/settings/reports/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/reports/report_generation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.070526 mne-bids-pipeline-1.2.0/docs/source/settings/sensor/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/sensor/contrasts.md
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/sensor/group_level.md
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/sensor/mvpa.md
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/sensor/time_freq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.070526 mne-bids-pipeline-1.2.0/docs/source/settings/source/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/source/bem.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/source/forward.md
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/source/general.md
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/settings/source/inverse.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/tags.md
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/v1.0.md.inc
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/v1.1.md.inc
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/docs/source/v1.2.md.inc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.074526 mne-bids-pipeline-1.2.0/mne_bids_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69106 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_config_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_config_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_import_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7811 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_reject.py
--rw-r--r--   0 runner    (1001) docker     (123)    40337 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.074526 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.074526 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/freesurfer/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/freesurfer/_01_recon_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/freesurfer/_02_coreg_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/freesurfer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.074526 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/freesurfer/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/freesurfer/contrib/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/freesurfer/contrib/README
--rwxr-xr-x   0 runner    (1001) docker     (123)    32882 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/freesurfer/contrib/run.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/freesurfer/contrib/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.074526 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/init/
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/init/_01_init_derivatives_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/init/_02_find_empty_room.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/init/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.078526 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_01_data_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_02_maxfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_03_frequency_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_04_make_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_05a_run_ica.py
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_05b_run_ssp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_06a_apply_ica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_06b_apply_ssp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_07_ptp_reject.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.078526 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/_01_make_evoked.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/_02_decoding_full_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/_03_decoding_time_by_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/_04_time_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/_05_decoding_csp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/_06_make_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    24373 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/_99_group_average.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.078526 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/source/_01_make_bem_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/source/_02_make_bem_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/source/_03_setup_source_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/source/_04_make_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/source/_05_make_inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/source/_99_group_average.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.082526 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.082526 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ERP_CORE.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000117.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000246.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000247.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000248_FLASH_BEM.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000248_T1_BEM.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000248_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000248_coreg_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000248_ica.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000248_no_mri.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds001810.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds001971.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds003104.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds003392.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds003775.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds004107.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds004229.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_eeg_matchingpennies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/ds000247_scans.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/ds001971_participants.tsv
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/freesurfer-license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/test_documented.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:44:12.074526 mne-bids-pipeline-1.2.0/mne_bids_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-03-23 14:44:12.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-03-23 14:44:12.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:44:12.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-23 14:44:12.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-23 14:44:12.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-23 14:44:12.000000 mne-bids-pipeline-1.2.0/mne_bids_pipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-23 14:43:56.000000 mne-bids-pipeline-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 14:44:12.082526 mne-bids-pipeline-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.923825 mne-bids-pipeline-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.875825 mne-bids-pipeline-1.3.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)    39920 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.circleci/config.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3135 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.circleci/setup_bash.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.875825 mne-bids-pipeline-1.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.github/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.879825 mne-bids-pipeline-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.github/workflows/circleci-redirector.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/BUILDING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-06-01 14:51:09.923825 mne-bids-pipeline-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.879825 mne-bids-pipeline-1.3.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/build-docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.879825 mne-bids-pipeline-1.3.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.883825 mne-bids-pipeline-1.3.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.883825 mne-bids-pipeline-1.3.0/docs/source/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    97580 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/assets/mne.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/changes.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.883825 mne-bids-pipeline-1.3.0/docs/source/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/doc-config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.883825 mne-bids-pipeline-1.3.0/docs/source/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10313 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/examples/gen_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.883825 mne-bids-pipeline-1.3.0/docs/source/features/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1618 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/features/gen_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/features/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.883825 mne-bids-pipeline-1.3.0/docs/source/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/getting_started/basic_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/getting_started/freesurfer.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/getting_started/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/governance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.883825 mne-bids-pipeline-1.3.0/docs/source/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/general.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.887825 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/artifacts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/autobads.md
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/breaks.md
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/epochs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/filter.md
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/maxfilter.md
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/resample.md
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/ssp_ica.md
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/stim_artifact.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.887825 mne-bids-pipeline-1.3.0/docs/source/settings/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/reports/report_generation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.891825 mne-bids-pipeline-1.3.0/docs/source/settings/sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/sensor/contrasts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/sensor/group_level.md
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/sensor/mvpa.md
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/sensor/time_freq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.891825 mne-bids-pipeline-1.3.0/docs/source/settings/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/source/bem.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/source/forward.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/source/general.md
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/settings/source/inverse.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/tags.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/v1.0.md.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/v1.1.md.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/v1.2.md.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/docs/source/v1.3.md.inc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.895825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69107 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_import_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7776 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_reject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40371 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.899825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.899825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/_01_recon_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/_02_coreg_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.903825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/contrib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/contrib/README
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32882 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/contrib/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/contrib/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.903825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/init/
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/init/_01_init_derivatives_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/init/_02_find_empty_room.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/init/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.907825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_01_data_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_02_maxfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_03_frequency_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_04_make_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_05a_run_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_05b_run_ssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_06a_apply_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_06b_apply_ssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_07_ptp_reject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.907825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_01_make_evoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_02_decoding_full_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_03_decoding_time_by_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_04_time_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_05_decoding_csp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_06_make_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24358 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_99_group_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.911825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_01_make_bem_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_02_make_bem_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_03_setup_source_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_04_make_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_05_make_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_99_group_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.915825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.923825 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ERP_CORE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000117.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000246.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000247.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_FLASH_BEM.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_T1_BEM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_coreg_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_no_mri.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds001810.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds001971.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds003104.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds003392.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds003775.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds004107.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds004229.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_eeg_matchingpennies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/ds000247_scans.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/ds001971_participants.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/freesurfer-license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_documented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:51:09.899825 mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-06-01 14:51:09.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-01 14:51:09.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:51:09.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 14:51:09.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-01 14:51:09.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 14:51:09.000000 mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-01 14:50:47.000000 mne-bids-pipeline-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:51:09.923825 mne-bids-pipeline-1.3.0/setup.cfg
```

### Comparing `mne-bids-pipeline-1.2.0/.circleci/config.yml` & `mne-bids-pipeline-1.3.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/.circleci/setup_bash.sh` & `mne-bids-pipeline-1.3.0/.circleci/setup_bash.sh`

 * *Files 2% similar despite different names*

```diff
@@ -52,11 +52,12 @@
 echo 'export MNE_DATA=$HOME/mne_data' >> "$BASH_ENV"
 echo "export PATH=~/.local/bin/:$PATH" >> "$BASH_ENV"
 echo 'export DISPLAY=:99' >> "$BASH_ENV"
 echo 'export XDG_RUNTIME_DIR=/tmp/runtime-circleci' >> "$BASH_ENV"
 echo 'export MPLBACKEND=Agg' >> "$BASH_ENV"
 echo "source ~/python_env/bin/activate" >> "$BASH_ENV"
 echo "export MNE_3D_OPTION_MULTI_SAMPLES=1" >> "$BASH_ENV"
+echo "export MNE_BIDS_PIPELINE_FORCE_TERMINAL=true" >> "$BASH_ENV"
 mkdir -p ~/.local/bin
 if [[ ! -f ~/.local/bin/python ]]; then
     ln -s ~/python_env/bin/python ~/.local/bin/python
 fi
```

### Comparing `mne-bids-pipeline-1.2.0/.github/config.yml` & `mne-bids-pipeline-1.3.0/.github/config.yml`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/.github/workflows/release.yml` & `mne-bids-pipeline-1.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/.github/workflows/run-tests.yml` & `mne-bids-pipeline-1.3.0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/CONTRIBUTING.md` & `mne-bids-pipeline-1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/LICENSE.txt` & `mne-bids-pipeline-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/Makefile` & `mne-bids-pipeline-1.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/PKG-INFO` & `mne-bids-pipeline-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mne-bids-pipeline
-Version: 1.2.0
+Version: 1.3.0
 Summary: A full-flegded processing pipeline for your MEG and EEG data
 Author: Eric Larson, Alexandre Gramfort, Mainak Jas
 Author-email: Richard Höchenberger <richard.hoechenberger@gmail.com>
 License: Copyright © 2019-2022, authors of MNE-BIDS-Pipeline
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `mne-bids-pipeline-1.2.0/README.md` & `mne-bids-pipeline-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/codecov.yml` & `mne-bids-pipeline-1.3.0/codecov.yml`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/hooks.py` & `mne-bids-pipeline-1.3.0/docs/hooks.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/mkdocs.yml` & `mne-bids-pipeline-1.3.0/docs/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     name: material
     logo: assets/mne.svg
     favicon: assets/favicon.ico
     features:
         - navigation.tabs
         - navigation.instant  # Load pages via XMLHttpRequest (XHR)
         - navigation.tracking
+        - content.code.copy  # copy button
     palette:
       # Palette toggle for automated theme selection
       # Currently only available to sponsors
       #
       # - media: "(prefers-color-scheme)"
       #   toggle:
       #     icon: material/brightness-auto
```

### Comparing `mne-bids-pipeline-1.2.0/docs/source/assets/favicon.ico` & `mne-bids-pipeline-1.3.0/docs/source/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/assets/mne.svg` & `mne-bids-pipeline-1.3.0/docs/source/assets/mne.svg`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/css/extra.css` & `mne-bids-pipeline-1.3.0/docs/source/css/extra.css`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/examples/gen_examples.py` & `mne-bids-pipeline-1.3.0/docs/source/examples/gen_examples.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/features/gen_steps.py` & `mne-bids-pipeline-1.3.0/docs/source/features/gen_steps.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/features/overview.md` & `mne-bids-pipeline-1.3.0/docs/source/features/overview.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/getting_started/basic_usage.md` & `mne-bids-pipeline-1.3.0/docs/source/getting_started/basic_usage.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/getting_started/freesurfer.md` & `mne-bids-pipeline-1.3.0/docs/source/getting_started/freesurfer.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/getting_started/install.md` & `mne-bids-pipeline-1.3.0/docs/source/getting_started/install.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/index.md` & `mne-bids-pipeline-1.3.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/settings/general.md` & `mne-bids-pipeline-1.3.0/docs/source/settings/general.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/autobads.md` & `mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/autobads.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/epochs.md` & `mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/epochs.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/filter.md` & `mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/filter.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/resample.md` & `mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/resample.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/settings/preprocessing/ssp_ica.md` & `mne-bids-pipeline-1.3.0/docs/source/settings/preprocessing/ssp_ica.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/settings/sensor/mvpa.md` & `mne-bids-pipeline-1.3.0/docs/source/settings/sensor/mvpa.md`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/docs/source/v1.0.md.inc` & `mne-bids-pipeline-1.3.0/docs/source/v1.0.md.inc`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/_config.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -965,15 +965,15 @@
 contrasts: Iterable[Union[Tuple[str, str], ArbitraryContrast]] = []
 """
 The conditions to contrast via a subtraction of ERPs / ERFs. The list elements
 can either be tuples or dictionaries (or a mix of both). Each element in the
 list corresponds to a single contrast.
 
 A tuple specifies a one-vs-one contrast, where the second condition is
-subtraced from the first.
+subtracted from the first.
 
 If a dictionary, must contain the following keys:
 
 - `name`: a custom name of the contrast
 - `conditions`: the conditions to contrast
 - `weights`: the weights associated with each condition.
```

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/_config_import.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config_import.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/_config_template.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config_template.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/_config_utils.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_config_utils.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/_decoding.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_decoding.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/_download.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_download.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/_import_data.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_import_data.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/_io.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_io.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/_main.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from types import ModuleType, SimpleNamespace
 
 import numpy as np
 
 from ._config_utils import _get_step_modules
 from ._config_import import _import_config
 from ._config_template import create_template_config
-from ._logging import logger, gen_log_kwargs, _install_logs
+from ._logging import logger, gen_log_kwargs
 from ._run import _short_step_path
 
 
 def main():
     from . import __version__
 
     parser = argparse.ArgumentParser()
@@ -189,15 +189,14 @@
 
     if processing_stages[0] != "all":
         # Always run the directory initialization steps, but skip for 'all',
         # because it already includes them – and we want to avoid running
         # them twice.
         step_modules = [*STEP_MODULES["init"], *step_modules]
 
-    _install_logs()
     msg = "Welcome aboard the MNE BIDS Pipeline!"
     logger.info(**gen_log_kwargs(message=msg, emoji="👋", box="╶╴", step=""))
     msg = f"Using configuration: {config}"
     logger.info(**gen_log_kwargs(message=msg, emoji="🧾", box="╶╴", step=""))
 
     config_imported = _import_config(
         config_path=config_path,
```

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/_parallel.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_parallel.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/_reject.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_reject.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/_report.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,16 +74,16 @@
                 _finalize(
                     report=report,
                     exec_params=exec_params,
                     subject=subject,
                     session=session,
                     run=run,
                 )
-            except Exception:
-                pass
+            except Exception as exc:
+                logger.warning(f"Failed: {exc}")
             fname_report_html = fname_report.with_suffix(".html")
             msg = f"Saving report: {fname_report_html}"
             logger.info(**gen_log_kwargs(message=msg))
             report.save(fname_report, overwrite=True)
             report.save(fname_report_html, overwrite=True, open_browser=False)
 
 
@@ -532,15 +532,15 @@
     if css not in report.include:
         report.add_custom_css(css=css)
 
 
 # We make a lot of calls to this function and it takes > 1 sec generally
 # to run, so run it just once (it shouldn't meaningfully change anyway)
 @lru_cache(maxsize=1)
-def _cached_sys_info(f):
+def _cached_sys_info():
     with StringIO() as f:
         mne.sys_info(f)
         return f.getvalue()
 
 
 def _all_conditions(*, cfg):
     if isinstance(cfg.conditions, dict):
```

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/_run.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 import pathlib
 import pdb
 import sys
 import traceback
 import time
 from typing import Callable, Optional, Dict, List
 from types import SimpleNamespace
-import warnings
 
+from filelock import FileLock
 from joblib import Memory
 import json_tricks
-from openpyxl import load_workbook
 import pandas as pd
 from mne_bids import BIDSPath
 
 from ._config_utils import get_task
 from ._logging import logger, gen_log_kwargs
 
 
@@ -79,30 +78,30 @@
                         message += "\n".join(
                             traceback.format_exception(
                                 etype=type(e), value=e, tb=e.__traceback__
                             )
                         )
                     if os.getenv("_MNE_BIDS_STUDY_TESTING", "") == "true":
                         raise
-                    logger.critical(
+                    logger.error(
                         **gen_log_kwargs(message=message, **kwargs_copy, emoji="❌")
                     )
                     sys.exit(1)
                 elif on_error == "debug":
                     message += "\n\nStarting post-mortem debugger."
-                    logger.critical(
+                    logger.error(
                         **gen_log_kwargs(message=message, **kwargs_copy, emoji="🐛")
                     )
                     extype, value, tb = sys.exc_info()
                     traceback.print_exc()
                     pdb.post_mortem(tb)
                     sys.exit(1)
                 else:
                     message += "\n\nContinuing pipeline run."
-                    logger.critical(
+                    logger.error(
                         **gen_log_kwargs(message=message, **kwargs_copy, emoji="🔂")
                     )
             log_info["time"] = round(time.time() - t0, ndigits=1)
             return log_info
 
         return wrapper
 
@@ -298,39 +297,24 @@
         columns = list(columns)
         idx = columns.index("cfg")
         del columns[idx]
         columns.insert(-3, "cfg")  # put it before time, success & err cols
 
     df = df[columns]
 
-    if fname.exists():
-        book = None
-        try:
-            book = load_workbook(fname)
-        except Exception:  # bad file
-            pass
-        else:
-            if sheet_name in book:
-                book.remove(book[sheet_name])
-        writer = pd.ExcelWriter(fname, engine="openpyxl")
-        if book is not None:
-            try:
-                writer.book = book
-            except Exception:
-                pass  # AttributeError: can't set attribute 'book' (?)
-    else:
-        writer = pd.ExcelWriter(fname, engine="openpyxl")
-
-    df.to_excel(writer, sheet_name=sheet_name, index=False)
-    # TODO: "Future!!! warning save is not part of the public API, usage can give
-    # in unexpected results and will be removed in a future version"
-    with warnings.catch_warnings(record=True):
-        warnings.simplefilter("ignore")
-        writer.save()
-    writer.close()
+    with FileLock(fname.with_suffix(fname.suffix + ".lock")):
+        append = fname.exists()
+        writer = pd.ExcelWriter(
+            fname,
+            engine="openpyxl",
+            mode="a" if append else "w",
+            if_sheet_exists="replace" if append else None,
+        )
+        with writer:
+            df.to_excel(writer, sheet_name=sheet_name, index=False)
 
 
 def _update_for_splits(
     files_dict: Dict[str, BIDSPath],
     key: str,
     *,
     single: bool = False,
```

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/_viz.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/_viz.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/freesurfer/_01_recon_all.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/_01_recon_all.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/freesurfer/_02_coreg_surfaces.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/_02_coreg_surfaces.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/freesurfer/contrib/LICENSE` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/contrib/LICENSE`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/freesurfer/contrib/run.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/freesurfer/contrib/run.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/init/_01_init_derivatives_dir.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/init/_01_init_derivatives_dir.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/init/_02_find_empty_room.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/init/_02_find_empty_room.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_01_data_quality.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_01_data_quality.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_02_maxfilter.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_02_maxfilter.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_03_frequency_filter.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_03_frequency_filter.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_04_make_epochs.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_04_make_epochs.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_05a_run_ica.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_05a_run_ica.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_05b_run_ssp.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_05b_run_ssp.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_06a_apply_ica.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_06a_apply_ica.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_06b_apply_ssp.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_06b_apply_ssp.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/preprocessing/_07_ptp_reject.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/preprocessing/_07_ptp_reject.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/_01_make_evoked.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_01_make_evoked.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/_02_decoding_full_epochs.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_02_decoding_full_epochs.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/_03_decoding_time_by_time.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_03_decoding_time_by_time.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/_04_time_frequency.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_04_time_frequency.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/_05_decoding_csp.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_05_decoding_csp.py`

 * *Files 1% similar despite different names*

```diff
@@ -540,15 +540,15 @@
     """Run all subjects decoding in parallel."""
     if not config.contrasts or not config.decoding_csp:
         if not config.contrasts:
             msg = "No contrasts specified. "
         else:
             msg = "No CSP analysis requested. "
 
-        msg = "Skipping …"
+        msg += "Skipping …"
         logger.info(**gen_log_kwargs(message=msg, emoji="skip"))
         return
 
     with get_parallel_backend(config.exec_params):
         parallel, run_func = parallel_func(
             one_subject_decoding, exec_params=config.exec_params
         )
```

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/_06_make_cov.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_06_make_cov.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/sensor/_99_group_average.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/sensor/_99_group_average.py`

 * *Files 0% similar despite different names*

```diff
@@ -661,15 +661,15 @@
             if exec_params.interactive:
                 for evoked in evokeds:
                     evoked.plot()
 
             if cfg.decode:
                 average_full_epochs_decoding(cfg, session)
                 average_time_by_time_decoding(cfg, session)
-        if cfg.decode and cfg.decoding_csp:
+        if cfg.decoding_csp:
             parallel, run_func = parallel_func(
                 average_csp_decoding, exec_params=exec_params
             )
             parallel(
                 run_func(
                     cfg=cfg,
                     session=session,
```

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/source/_01_make_bem_surfaces.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_01_make_bem_surfaces.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/source/_02_make_bem_solution.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_02_make_bem_solution.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/source/_03_setup_source_space.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_03_setup_source_space.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/source/_04_make_forward.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_04_make_forward.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/source/_05_make_inverse.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_05_make_inverse.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/steps/source/_99_group_average.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/steps/source/_99_group_average.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ERP_CORE.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ERP_CORE.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000117.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000117.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000246.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000246.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000247.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000247.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000248_base.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_base.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000248_ica.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_ica.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds000248_no_mri.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds000248_no_mri.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds003392.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds003392.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds003775.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds003775.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds004107.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds004107.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/configs/config_ds004229.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/configs/config_ds004229.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/conftest.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,12 +26,13 @@
     ignore:make_current is deprecated.*:DeprecationWarning
     ignore:`np.*` is a deprecated alias for .*:DeprecationWarning
     ignore:.*implicit namespace.*:DeprecationWarning
     ignore:Deprecated call to `pkg_resources.*:DeprecationWarning
     ignore:.*declare_namespace.*mpl_toolkits.*:DeprecationWarning
     ignore:_SixMetaPathImporter\.find_spec.*:ImportWarning
     ignore:pkg_resources is deprecated.*:DeprecationWarning
+    ignore:`product` is deprecated as of NumPy.*:DeprecationWarning
     """
     for warning_line in warning_lines.split("\n"):
         warning_line = warning_line.strip()
         if warning_line and not warning_line.startswith("#"):
             config.addinivalue_line("filterwarnings", warning_line)
```

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/datasets.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/datasets.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/test_cli.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/test_documented.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_documented.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/test_run.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline/tests/test_validation.py` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline/tests/test_validation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from mne_bids_pipeline._config_import import _import_config
 
 
-def test_validation(tmp_path, caplog):
+def test_validation(tmp_path, capsys):
     """Test that misspellings are caught by our config import validator."""
     config_path = tmp_path / "config.py"
     bad_text = ""
     # no bids_root
     config_path.write_text(bad_text)
     with pytest.raises(ValueError, match="You need to specify `bids_root`"):
         _import_config(config_path=config_path)
@@ -27,24 +27,26 @@
     # misspelled sessions
     bad_text += "session = ['foo']\n"
     config_path.write_text(bad_text)
     with pytest.raises(ValueError, match=r".*did you mean 'sessions'\?"):
         _import_config(config_path=config_path)
     bad_text += "config_validation = 'warn'\n"
     config_path.write_text(bad_text)
-    assert caplog.record_tuples == []
+    capsys.readouterr()
     _import_config(config_path=config_path)
-    assert len(caplog.record_tuples) == 1
-    assert caplog.record_tuples[0][:2] == ("mne-bids-pipeline", 30)
-    msg = caplog.record_tuples[0][2]
+    msg, err = capsys.readouterr()
+    assert err == ""
+    assert len(msg.splitlines()) == 1
     assert "did you mean 'sessions'?" in msg
     bad_text += "config_validation = 'ignore'\n"
     config_path.write_text(bad_text)
+    capsys.readouterr()
     _import_config(config_path=config_path)
-    assert len(caplog.record_tuples) == 1  # no new message
+    msg, err = capsys.readouterr()
+    assert msg == err == ""  # no new message
     # old values
     bad_text = working_text
     bad_text += "debug = True\n"
     config_path.write_text(bad_text)
     with pytest.raises(ValueError, match="Found a variable.*use on_error=.*"):
         _import_config(config_path=config_path)
     bad_text += "on_error = 'debug' if debug else 'raise'\n"
```

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline.egg-info/PKG-INFO` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mne-bids-pipeline
-Version: 1.2.0
+Version: 1.3.0
 Summary: A full-flegded processing pipeline for your MEG and EEG data
 Author: Eric Larson, Alexandre Gramfort, Mainak Jas
 Author-email: Richard Höchenberger <richard.hoechenberger@gmail.com>
 License: Copyright © 2019-2022, authors of MNE-BIDS-Pipeline
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline.egg-info/SOURCES.txt` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 docs/source/doc-config.py
 docs/source/governance.md
 docs/source/index.md
 docs/source/tags.md
 docs/source/v1.0.md.inc
 docs/source/v1.1.md.inc
 docs/source/v1.2.md.inc
+docs/source/v1.3.md.inc
 docs/source/assets/favicon.ico
 docs/source/assets/mne.svg
 docs/source/css/extra.css
 docs/source/examples/gen_examples.py
 docs/source/features/gen_steps.py
 docs/source/features/overview.md
 docs/source/getting_started/basic_usage.md
```

### Comparing `mne-bids-pipeline-1.2.0/mne_bids_pipeline.egg-info/requires.txt` & `mne-bids-pipeline-1.3.0/mne_bids_pipeline.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 dask[distributed]
 bokeh<3
 jupyter-server-proxy
 scikit-learn
 pandas
 seaborn
 json_tricks
-coloredlogs
+rich
 python-picard
 qtpy
 pyvista
 pyvistaqt
 openpyxl
 autoreject
-mne[hdf5]
+mne[hdf5]>=1.2
 mne-bids[full]
 filelock
 setuptools>=65
 
 [:python_version < "3.8"]
 typing_extensions
 importlib_metadata
```

### Comparing `mne-bids-pipeline-1.2.0/pyproject.toml` & `mne-bids-pipeline-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,22 +26,22 @@
     "dask[distributed]",
     "bokeh < 3",  # for distributed dashboard
     "jupyter-server-proxy",  # to have dask and jupyter working together
     "scikit-learn",
     "pandas",
     "seaborn",
     "json_tricks",
-    "coloredlogs",
+    "rich",
     "python-picard",
     "qtpy",
     "pyvista",
     "pyvistaqt",
     "openpyxl",
     "autoreject",
-    "mne[hdf5]",
+    "mne[hdf5] >=1.2",
     "mne-bids[full]",
     "filelock",
     "setuptools >=65",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
```

