# Comparing `tmp/lsl_relay-3.1.0.tar.gz` & `tmp/lsl_relay-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsl_relay-3.1.0.tar", last modified: Mon May 29 10:17:38 2023, max compression
+gzip compressed data, was "lsl_relay-3.1.2.tar", last modified: Thu Jun  1 07:10:52 2023, max compression
```

## Comparing `lsl_relay-3.1.0.tar` & `lsl_relay-3.1.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.283628 lsl_relay-3.1.0/
--rw-r--r--   0 dom       (1000) dom       (1000)      121 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/.coveragerc
--rw-r--r--   0 dom       (1000) dom       (1000)      246 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/.editorconfig
--rw-r--r--   0 dom       (1000) dom       (1000)      207 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/.flake8
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.279628 lsl_relay-3.1.0/.github/
--rw-r--r--   0 dom       (1000) dom       (1000)      148 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/.github/dependabot.yml
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.279628 lsl_relay-3.1.0/.github/workflows/
--rw-r--r--   0 dom       (1000) dom       (1000)     1520 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/.github/workflows/main.yml
--rw-r--r--   0 dom       (1000) dom       (1000)     6172 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/.gitignore
--rw-r--r--   0 dom       (1000) dom       (1000)      902 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0 dom       (1000) dom       (1000)       48 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/.readthedocs.yml
--rw-r--r--   0 dom       (1000) dom       (1000)     2643 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/CHANGES.rst
--rw-r--r--   0 dom       (1000) dom       (1000)     1050 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/LICENSE
--rw-r--r--   0 dom       (1000) dom       (1000)     2127 2023-05-29 10:17:38.283628 lsl_relay-3.1.0/PKG-INFO
--rw-r--r--   0 dom       (1000) dom       (1000)     1137 2023-05-29 10:14:16.000000 lsl_relay-3.1.0/README.rst
--rw-r--r--   0 dom       (1000) dom       (1000)      117 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/conda-env.yml
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.279628 lsl_relay-3.1.0/docs/
--rw-r--r--   0 dom       (1000) dom       (1000)      503 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/docs/api.rst
--rw-r--r--   0 dom       (1000) dom       (1000)     1825 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/docs/conf.py
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.279628 lsl_relay-3.1.0/docs/guides/
--rw-r--r--   0 dom       (1000) dom       (1000)     3533 2023-05-26 22:24:10.000000 lsl_relay-3.1.0/docs/guides/device_sync.rst
--rw-r--r--   0 dom       (1000) dom       (1000)      189 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/docs/guides/index.rst
--rw-r--r--   0 dom       (1000) dom       (1000)     4707 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/docs/guides/overview.rst
--rw-r--r--   0 dom       (1000) dom       (1000)     5688 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/docs/guides/time_alignment.rst
--rw-r--r--   0 dom       (1000) dom       (1000)       89 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/docs/history.rst
--rw-r--r--   0 dom       (1000) dom       (1000)     2307 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/docs/index.rst
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.279628 lsl_relay-3.1.0/examples/
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.279628 lsl_relay-3.1.0/examples/cloud_recordings/
--rw-r--r--   0 dom       (1000) dom       (1000)      299 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/examples/cloud_recordings/time_alignment_parameters.json
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.275628 lsl_relay-3.1.0/examples/companion_app_exports/
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.279628 lsl_relay-3.1.0/examples/companion_app_exports/subject_1/
--rw-r--r--   0 dom       (1000) dom       (1000)   163603 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/examples/companion_app_exports/subject_1/PI left v1 ps1.illuminance.csv
--rw-r--r--   0 dom       (1000) dom       (1000)   167691 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/examples/companion_app_exports/subject_1/PI right v1 ps1.illuminance.csv
--rw-r--r--   0 dom       (1000) dom       (1000)      300 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/examples/companion_app_exports/subject_1/time_alignment_parameters.json
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.279628 lsl_relay-3.1.0/examples/companion_app_exports/subject_2/
--rw-r--r--   0 dom       (1000) dom       (1000)   165227 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/examples/companion_app_exports/subject_2/PI left v1 ps1.illuminance.csv
--rw-r--r--   0 dom       (1000) dom       (1000)   162539 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/examples/companion_app_exports/subject_2/PI right v1 ps1.illuminance.csv
--rw-r--r--   0 dom       (1000) dom       (1000)      300 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/examples/companion_app_exports/subject_2/time_alignment_parameters.json
--rw-r--r--   0 dom       (1000) dom       (1000)     2328 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/examples/device_vs_lsl_sync.py
--rw-r--r--   0 dom       (1000) dom       (1000)     2152 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/examples/linear_time_model.py
--rw-r--r--   0 dom       (1000) dom       (1000)      840 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/examples/time_mapping_from_parameters.py
--rw-r--r--   0 dom       (1000) dom       (1000)       37 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/mypy.ini
--rw-r--r--   0 dom       (1000) dom       (1000)      288 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/pyproject.toml
--rw-r--r--   0 dom       (1000) dom       (1000)      130 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/pytest.ini
--rw-r--r--   0 dom       (1000) dom       (1000)     1828 2023-05-29 10:17:38.283628 lsl_relay-3.1.0/setup.cfg
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.275628 lsl_relay-3.1.0/src/
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.279628 lsl_relay-3.1.0/src/lsl_relay.egg-info/
--rw-r--r--   0 dom       (1000) dom       (1000)     2127 2023-05-29 10:17:38.000000 lsl_relay-3.1.0/src/lsl_relay.egg-info/PKG-INFO
--rw-r--r--   0 dom       (1000) dom       (1000)     1652 2023-05-29 10:17:38.000000 lsl_relay-3.1.0/src/lsl_relay.egg-info/SOURCES.txt
--rw-r--r--   0 dom       (1000) dom       (1000)        1 2023-05-29 10:17:38.000000 lsl_relay-3.1.0/src/lsl_relay.egg-info/dependency_links.txt
--rw-r--r--   0 dom       (1000) dom       (1000)      225 2023-05-29 10:17:38.000000 lsl_relay-3.1.0/src/lsl_relay.egg-info/entry_points.txt
--rw-r--r--   0 dom       (1000) dom       (1000)      484 2023-05-29 10:17:38.000000 lsl_relay-3.1.0/src/lsl_relay.egg-info/requires.txt
--rw-r--r--   0 dom       (1000) dom       (1000)       11 2023-05-29 10:17:38.000000 lsl_relay-3.1.0/src/lsl_relay.egg-info/top_level.txt
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.275628 lsl_relay-3.1.0/src/pupil_labs/
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.279628 lsl_relay-3.1.0/src/pupil_labs/lsl_relay/
--rw-r--r--   0 dom       (1000) dom       (1000)      349 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/src/pupil_labs/lsl_relay/__init__.py
--rw-r--r--   0 dom       (1000) dom       (1000)       95 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/src/pupil_labs/lsl_relay/__main__.py
--rw-r--r--   0 dom       (1000) dom       (1000)     1727 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/src/pupil_labs/lsl_relay/channels.py
--rw-r--r--   0 dom       (1000) dom       (1000)     8260 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/src/pupil_labs/lsl_relay/cli.py
--rw-r--r--   0 dom       (1000) dom       (1000)     2901 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/src/pupil_labs/lsl_relay/linear_time_model.py
--rw-r--r--   0 dom       (1000) dom       (1000)     5071 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/src/pupil_labs/lsl_relay/outlets.py
--rw-r--r--   0 dom       (1000) dom       (1000)    10535 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/src/pupil_labs/lsl_relay/relay.py
--rw-r--r--   0 dom       (1000) dom       (1000)     7769 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/src/pupil_labs/lsl_relay/xdf_cloud_time_sync.py
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.283628 lsl_relay-3.1.0/tests/
--rw-r--r--   0 dom       (1000) dom       (1000)      180 2023-05-27 00:36:39.000000 lsl_relay-3.1.0/tests/test_api.py
-drwxr-xr-x   0 dom       (1000) dom       (1000)        0 2023-05-29 10:17:38.283628 lsl_relay-3.1.0/tools/
--rw-r--r--   0 dom       (1000) dom       (1000)     1999 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/tools/extract_eye_video_illuminance.py
--rw-r--r--   0 dom       (1000) dom       (1000)     1751 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/tools/monitor_relay.py
--rw-r--r--   0 dom       (1000) dom       (1000)     1782 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/tools/print_events.py
--rw-r--r--   0 dom       (1000) dom       (1000)      565 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/tools/show_relay_metadata.py
--rw-r--r--   0 dom       (1000) dom       (1000)      745 2023-05-16 06:30:31.000000 lsl_relay-3.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.449257 lsl_relay-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.425257 lsl_relay-3.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.429257 lsl_relay-3.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-01 07:10:52.449257 lsl_relay-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/conda-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.429257 lsl_relay-3.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.433257 lsl_relay-3.1.2/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/guides/device_sync.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/guides/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/guides/time_alignment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.433257 lsl_relay-3.1.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.433257 lsl_relay-3.1.2/examples/cloud_recordings/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/cloud_recordings/time_alignment_parameters.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.417257 lsl_relay-3.1.2/examples/companion_app_exports/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.437257 lsl_relay-3.1.2/examples/companion_app_exports/subject_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   163603 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/companion_app_exports/subject_1/PI left v1 ps1.illuminance.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   167691 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/companion_app_exports/subject_1/PI right v1 ps1.illuminance.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/companion_app_exports/subject_1/time_alignment_parameters.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.437257 lsl_relay-3.1.2/examples/companion_app_exports/subject_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   165227 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/companion_app_exports/subject_2/PI left v1 ps1.illuminance.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   162539 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/companion_app_exports/subject_2/PI right v1 ps1.illuminance.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/companion_app_exports/subject_2/time_alignment_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/device_vs_lsl_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/linear_time_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/time_mapping_from_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-01 07:10:52.449257 lsl_relay-3.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.417257 lsl_relay-3.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.441257 lsl_relay-3.1.2/src/lsl_relay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-01 07:10:52.000000 lsl_relay-3.1.2/src/lsl_relay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-01 07:10:52.000000 lsl_relay-3.1.2/src/lsl_relay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:10:52.000000 lsl_relay-3.1.2/src/lsl_relay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-01 07:10:52.000000 lsl_relay-3.1.2/src/lsl_relay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-01 07:10:52.000000 lsl_relay-3.1.2/src/lsl_relay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 07:10:52.000000 lsl_relay-3.1.2/src/lsl_relay.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.417257 lsl_relay-3.1.2/src/pupil_labs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.445257 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/linear_time_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/outlets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/xdf_cloud_time_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.445257 lsl_relay-3.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.449257 lsl_relay-3.1.2/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/tools/extract_eye_video_illuminance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/tools/monitor_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/tools/print_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/tools/show_relay_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/tox.ini
```

### Comparing `lsl_relay-3.1.0/.github/workflows/main.yml` & `lsl_relay-3.1.2/.github/workflows/main.yml`

 * *Files 3% similar despite different names*

```diff
@@ -49,22 +49,26 @@
           jobs: ${{ toJSON(needs) }}
 
   release:
     needs:
       - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
+    permissions:
+      id-token: write
+      contents: write
 
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.11-dev"
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Release
         run: tox -e release
         env:
-          TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+      - name: Publish to PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `lsl_relay-3.1.0/.gitignore` & `lsl_relay-3.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/.pre-commit-config.yaml` & `lsl_relay-3.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/CHANGES.rst` & `lsl_relay-3.1.2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 3.1.0 (2023-05-25)
 ##################
 - Adds official support for Neon modules
-- New project name
+- New project name pupil-labs-lsl-relay
 
 3.0.2 (2022-11-09)
 ##################
 - Gracefully handle xdf files without required time alignment information
 
 3.0.1 (2022-10-25)
 ##################
```

### Comparing `lsl_relay-3.1.0/LICENSE` & `lsl_relay-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/PKG-INFO` & `lsl_relay-3.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsl_relay
-Version: 3.1.0
+Version: 3.1.2
 Summary: Relay data from Pupil Labs Companion apps to LabStreamingLayer
 Home-page: https://github.com/pupil-labs/lsl-relay/
 Author: Pupil Labs GmbH
 Author-email: info@pupil-labs.com
 License: MIT
 Project-URL: Documentation, https://lsl-relay.readthedocs.io/en/stable/
 Project-URL: History, https://lsl-relay.readthedocs.io/en/latest/history.html
@@ -18,34 +18,34 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: pupil_cloud_alignment
 Provides-Extra: testing
 License-File: LICENSE
 
-.. image:: https://img.shields.io/pypi/v/pupil-invisible-lsl-relay.svg
+.. image:: https://img.shields.io/pypi/v/lsl-relay.svg
    :target: `PyPI link`_
 
-.. image:: https://img.shields.io/pypi/pyversions/pupil-invisible-lsl-relay.svg
+.. image:: https://img.shields.io/pypi/pyversions/lsl-relay.svg
    :target: `PyPI link`_
 
-.. _PyPI link: https://pypi.org/project/pupil-invisible-lsl-relay
+.. _PyPI link: https://pypi.org/project/lsl-relay
 
-.. image:: https://github.com/pupil-labs/pupil-invisible-lsl-relay/workflows/tests/badge.svg
-   :target: https://github.com/pupil-labs/pupil-invisible-lsl-relay/actions?query=workflow%3A%22tests%22
+.. image:: https://github.com/pupil-labs/lsl-relay/workflows/tests/badge.svg
+   :target: https://github.com/pupil-labs/lsl-relay/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. image:: https://readthedocs.org/projects/pupil-invisible-lsl-relay/badge/?version=latest
-   :target: https://pupil-invisible-lsl-relay.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/lsl-relay/badge/?version=latest
+   :target: https://lsl-relay.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2022-informational
    :target: https://blog.jaraco.com/skeleton
 
 *************************************************
 Pupil Labs LSL Relay for Neon and Pupil Invisible
 *************************************************
 
-- `Documentation <https://pupil-invisible-lsl-relay.readthedocs.io/>`_
+- `Documentation <https://pupil-labs-lsl-relay.readthedocs.io>`_
```

### Comparing `lsl_relay-3.1.0/docs/conf.py` & `lsl_relay-3.1.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         None,
     ),
 }
 
 html_theme = "furo"
 autosummary_generate = True
 
-project = "Pupil Labs Companion LSL Relay"
+project = "Pupil Labs LSL Relay"
 release = import_version("lsl_relay")
 # for example take major/minor
 version = ".".join(release.split(".")[:2])
 html_title = f"{project} {release}"
 
 output = subprocess.check_output(
     ["python", "device_vs_lsl_sync.py"], cwd="../examples/"
```

### Comparing `lsl_relay-3.1.0/docs/guides/device_sync.rst` & `lsl_relay-3.1.2/docs/guides/device_sync.rst`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/docs/guides/overview.rst` & `lsl_relay-3.1.2/docs/guides/overview.rst`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/docs/guides/time_alignment.rst` & `lsl_relay-3.1.2/docs/guides/time_alignment.rst`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/docs/index.rst` & `lsl_relay-3.1.2/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 *******************************
-Pupil Labs Companion LSL Relay
+Pupil Labs LSL Relay
 *******************************
 
-The Pupil Labs Companion LSL Relay (Relay) allows you to stream gaze and event data from your
-Pupil Labs Companion device to the `labstreaminglayer <https://github.com/sccn/labstreaminglayer>`_ (LSL).
+The Pupil Labs LSL Relay (Relay) allows you to stream gaze and event data from your
+Pupil Labs device to the `labstreaminglayer <https://github.com/sccn/labstreaminglayer>`_ (LSL).
 
 For integration between Pupil Core software and LSL, see https://github.com/labstreaminglayer/App-PupilLabs instead.
 
 Install and Usage
 ==================
-Install the Pupil Labs Companion LSL Relay with pip::
+Install the Pupil Labs LSL Relay with pip::
 
    pip install lsl-relay
 
 After you installed the relay, you can start it by executing::
 
    lsl_relay
```

### Comparing `lsl_relay-3.1.0/examples/companion_app_exports/subject_1/PI left v1 ps1.illuminance.csv` & `lsl_relay-3.1.2/examples/companion_app_exports/subject_1/PI left v1 ps1.illuminance.csv`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/examples/companion_app_exports/subject_1/PI right v1 ps1.illuminance.csv` & `lsl_relay-3.1.2/examples/companion_app_exports/subject_1/PI right v1 ps1.illuminance.csv`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/examples/companion_app_exports/subject_2/PI left v1 ps1.illuminance.csv` & `lsl_relay-3.1.2/examples/companion_app_exports/subject_2/PI left v1 ps1.illuminance.csv`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/examples/companion_app_exports/subject_2/PI right v1 ps1.illuminance.csv` & `lsl_relay-3.1.2/examples/companion_app_exports/subject_2/PI right v1 ps1.illuminance.csv`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/examples/device_vs_lsl_sync.py` & `lsl_relay-3.1.2/examples/device_vs_lsl_sync.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/examples/linear_time_model.py` & `lsl_relay-3.1.2/examples/linear_time_model.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/examples/time_mapping_from_parameters.py` & `lsl_relay-3.1.2/examples/time_mapping_from_parameters.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/setup.cfg` & `lsl_relay-3.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/src/lsl_relay.egg-info/PKG-INFO` & `lsl_relay-3.1.2/src/lsl_relay.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsl-relay
-Version: 3.1.0
+Version: 3.1.2
 Summary: Relay data from Pupil Labs Companion apps to LabStreamingLayer
 Home-page: https://github.com/pupil-labs/lsl-relay/
 Author: Pupil Labs GmbH
 Author-email: info@pupil-labs.com
 License: MIT
 Project-URL: Documentation, https://lsl-relay.readthedocs.io/en/stable/
 Project-URL: History, https://lsl-relay.readthedocs.io/en/latest/history.html
@@ -18,34 +18,34 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: pupil_cloud_alignment
 Provides-Extra: testing
 License-File: LICENSE
 
-.. image:: https://img.shields.io/pypi/v/pupil-invisible-lsl-relay.svg
+.. image:: https://img.shields.io/pypi/v/lsl-relay.svg
    :target: `PyPI link`_
 
-.. image:: https://img.shields.io/pypi/pyversions/pupil-invisible-lsl-relay.svg
+.. image:: https://img.shields.io/pypi/pyversions/lsl-relay.svg
    :target: `PyPI link`_
 
-.. _PyPI link: https://pypi.org/project/pupil-invisible-lsl-relay
+.. _PyPI link: https://pypi.org/project/lsl-relay
 
-.. image:: https://github.com/pupil-labs/pupil-invisible-lsl-relay/workflows/tests/badge.svg
-   :target: https://github.com/pupil-labs/pupil-invisible-lsl-relay/actions?query=workflow%3A%22tests%22
+.. image:: https://github.com/pupil-labs/lsl-relay/workflows/tests/badge.svg
+   :target: https://github.com/pupil-labs/lsl-relay/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. image:: https://readthedocs.org/projects/pupil-invisible-lsl-relay/badge/?version=latest
-   :target: https://pupil-invisible-lsl-relay.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/lsl-relay/badge/?version=latest
+   :target: https://lsl-relay.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2022-informational
    :target: https://blog.jaraco.com/skeleton
 
 *************************************************
 Pupil Labs LSL Relay for Neon and Pupil Invisible
 *************************************************
 
-- `Documentation <https://pupil-invisible-lsl-relay.readthedocs.io/>`_
+- `Documentation <https://pupil-labs-lsl-relay.readthedocs.io>`_
```

### Comparing `lsl_relay-3.1.0/src/lsl_relay.egg-info/SOURCES.txt` & `lsl_relay-3.1.2/src/lsl_relay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/src/pupil_labs/lsl_relay/channels.py` & `lsl_relay-3.1.2/src/pupil_labs/lsl_relay/channels.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/src/pupil_labs/lsl_relay/cli.py` & `lsl_relay-3.1.2/src/pupil_labs/lsl_relay/cli.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/src/pupil_labs/lsl_relay/linear_time_model.py` & `lsl_relay-3.1.2/src/pupil_labs/lsl_relay/linear_time_model.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/src/pupil_labs/lsl_relay/outlets.py` & `lsl_relay-3.1.2/src/pupil_labs/lsl_relay/outlets.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/src/pupil_labs/lsl_relay/relay.py` & `lsl_relay-3.1.2/src/pupil_labs/lsl_relay/relay.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/src/pupil_labs/lsl_relay/xdf_cloud_time_sync.py` & `lsl_relay-3.1.2/src/pupil_labs/lsl_relay/xdf_cloud_time_sync.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/tools/extract_eye_video_illuminance.py` & `lsl_relay-3.1.2/tools/extract_eye_video_illuminance.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/tools/monitor_relay.py` & `lsl_relay-3.1.2/tools/monitor_relay.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/tools/print_events.py` & `lsl_relay-3.1.2/tools/print_events.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.0/tools/show_relay_metadata.py` & `lsl_relay-3.1.2/tools/show_relay_metadata.py`

 * *Files identical despite different names*

