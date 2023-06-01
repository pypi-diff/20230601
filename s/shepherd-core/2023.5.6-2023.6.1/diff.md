# Comparing `tmp/shepherd_core-2023.5.6.tar.gz` & `tmp/shepherd_core-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_core-2023.5.6.tar", last modified: Tue May 30 13:03:18 2023, max compression
+gzip compressed data, was "shepherd_core-2023.6.1.tar", last modified: Thu Jun  1 14:32:19 2023, max compression
```

## Comparing `shepherd_core-2023.5.6.tar` & `shepherd_core-2023.6.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.280735 shepherd_core-2023.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-30 13:03:18.280735 shepherd_core-2023.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-30 13:03:18.280735 shepherd_core-2023.5.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.268735 shepherd_core-2023.5.6/shepherd_core/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/calibration_hw_def.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.268735 shepherd_core-2023.5.6/shepherd_core/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.272735 shepherd_core-2023.5.6/shepherd_core/data_models/base/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/base/cal_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/base/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/base/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/base/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/base/shepherd.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/base/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.272735 shepherd_core-2023.5.6/shepherd_core/data_models/content/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/energy_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/energy_environment_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/firmware_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/virtual_harvester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/virtual_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/virtual_source_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/doc_virtual_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.272735 shepherd_core-2023.5.6/shepherd_core/data_models/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/experiment/observer_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/experiment/target_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.272735 shepherd_core-2023.5.6/shepherd_core/data_models/task/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/task/emulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/task/firmware_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/task/harvest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/task/observer_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/task/programming.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/task/testbed_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.276735 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/cape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/cape_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/gpio_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/mcu_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/observer_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/target_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/testbed.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/testbed_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.276735 shepherd_core-2023.5.6/shepherd_core/vsource/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/vsource/virtual_converter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/vsource/virtual_harvester_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/vsource/virtual_source_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.280735 shepherd_core-2023.5.6/shepherd_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-30 13:03:18.000000 shepherd_core-2023.5.6/shepherd_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-30 13:03:18.000000 shepherd_core-2023.5.6/shepherd_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:03:18.000000 shepherd_core-2023.5.6/shepherd_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-30 13:03:18.000000 shepherd_core-2023.5.6/shepherd_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 13:03:18.000000 shepherd_core-2023.5.6/shepherd_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:03:18.000000 shepherd_core-2023.5.6/shepherd_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.276735 shepherd_core-2023.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.280735 shepherd_core-2023.5.6/tests/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_cal_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_cal_data_faulty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_cal_meas.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_cal_meas_faulty1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_cal_meas_faulty2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_config_emulator.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_config_experiment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_config_experiment_alternative.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_config_harvester.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_config_testbed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_config_virtsource.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_base_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_content_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_content_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_experiment_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_task_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_task_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_testbed_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_testbed_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/test_cal_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.280735 shepherd_core-2023.5.6/tests/vsource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/vsource/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/vsource/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/vsource/test_harvester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.863205 shepherd_core-2023.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-01 14:32:19.863205 shepherd_core-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-01 14:32:19.863205 shepherd_core-2023.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.851205 shepherd_core-2023.6.1/shepherd_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/calibration_hw_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.851205 shepherd_core-2023.6.1/shepherd_core/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.851205 shepherd_core-2023.6.1/shepherd_core/data_models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/base/cal_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/base/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/base/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/base/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/base/shepherd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/base/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.855205 shepherd_core-2023.6.1/shepherd_core/data_models/content/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/energy_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/energy_environment_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/firmware_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_source_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/doc_virtual_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.855205 shepherd_core-2023.6.1/shepherd_core/data_models/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/experiment/observer_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/experiment/target_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.855205 shepherd_core-2023.6.1/shepherd_core/data_models/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/task/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/task/firmware_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/task/harvest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/task/observer_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/task/programming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/task/testbed_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.855205 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/cape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/cape_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/gpio_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/mcu_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/observer_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/target_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/testbed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/testbed_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20835 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.859205 shepherd_core-2023.6.1/shepherd_core/vsource/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/vsource/virtual_converter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/vsource/virtual_harvester_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/vsource/virtual_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13204 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.863205 shepherd_core-2023.6.1/shepherd_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-01 14:32:19.000000 shepherd_core-2023.6.1/shepherd_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-01 14:32:19.000000 shepherd_core-2023.6.1/shepherd_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:32:19.000000 shepherd_core-2023.6.1/shepherd_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-01 14:32:19.000000 shepherd_core-2023.6.1/shepherd_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 14:32:19.000000 shepherd_core-2023.6.1/shepherd_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:32:19.000000 shepherd_core-2023.6.1/shepherd_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.859205 shepherd_core-2023.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.863205 shepherd_core-2023.6.1/tests/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_cal_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_cal_data_faulty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_cal_meas.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_cal_meas_faulty1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_cal_meas_faulty2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_config_emulator.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_config_experiment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_config_experiment_alternative.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_config_harvester.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_config_testbed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_config_virtsource.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_base_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_content_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_content_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_experiment_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_task_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_task_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_testbed_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_testbed_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/test_cal_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.863205 shepherd_core-2023.6.1/tests/vsource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/vsource/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/vsource/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/vsource/test_harvester.py
```

### Comparing `shepherd_core-2023.5.6/PKG-INFO` & `shepherd_core-2023.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_core
-Version: 2023.5.6
+Version: 2023.6.1
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-core/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
```

### Comparing `shepherd_core-2023.5.6/README.md` & `shepherd_core-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/setup.cfg` & `shepherd_core-2023.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/shepherd_core/__init__.py` & `shepherd_core-2023.6.1/shepherd_core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .data_models.task import Compression
 from .logger import get_verbose_level
 from .logger import logger
 from .logger import set_verbose_level
 from .reader import BaseReader
 from .writer import BaseWriter
 
-__version__ = "2023.5.6"
+__version__ = "2023.6.1"
 
 __all__ = [
     "BaseReader",
     "BaseWriter",
     "get_verbose_level",
     "set_verbose_level",
     "logger",
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/calibration_hw_def.py` & `shepherd_core-2023.6.1/shepherd_core/calibration_hw_def.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/__init__.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+from pathlib import Path
+from typing import Optional
+
 from .base.calibration import CalibrationCape
 from .base.calibration import CalibrationEmulator
 from .base.calibration import CalibrationHarvester
 from .base.calibration import CalibrationPair
 from .base.calibration import CalibrationSeries
 from .base.content import ContentModel
 from .base.fixture import Fixtures
 from .base.shepherd import ShpModel
 from .base.wrapper import Wrapper
 from .content.energy_environment import EnergyDType
 from .content.energy_environment import EnergyEnvironment
 from .content.firmware import Firmware
 from .content.firmware import FirmwareDType
-from .content.virtual_harvester import VirtualHarvester
-from .content.virtual_source import VirtualSource
+from .content.virtual_harvester import VirtualHarvesterConfig
+from .content.virtual_source import VirtualSourceConfig
 from .experiment.experiment import Experiment
 from .experiment.observer_features import GpioActuation
 from .experiment.observer_features import GpioEvent
 from .experiment.observer_features import GpioLevel
 from .experiment.observer_features import GpioTracing
 from .experiment.observer_features import PowerTracing
 from .experiment.observer_features import SystemLogging
@@ -42,10 +45,24 @@
     "PowerTracing",
     "GpioTracing",
     "GpioActuation",
     "GpioEvent",
     "GpioLevel",
     "EnergyEnvironment",
     "EnergyDType",
-    "VirtualSource",
-    "VirtualHarvester",
+    "VirtualSourceConfig",
+    "VirtualHarvesterConfig",
+    # test-container & placeholder
+    "fixtures",
 ]
+
+
+class FixtureSet:
+    def __init__(self):
+        self.path = Path(__file__) / "fixtures"
+
+    def load(self, path: Optional[Path] = None) -> None:
+        if path:
+            self.path = path
+
+
+fixtures = FixtureSet()
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/base/cal_measurement.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/base/cal_measurement.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/base/calibration.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/base/calibration.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/base/content.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/base/content.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/base/fixture.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/base/fixture.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,23 +27,20 @@
             fixtures = yaml.safe_load(fix_data)
             for fixture in fixtures:
                 if not isinstance(fixture, dict):
                     continue
                 fwrap = Wrapper(**fixture)
                 if fwrap.model.lower() != model_name.lower():
                     continue
-                if "name" not in fwrap.fields:
+                if "name" not in fwrap.parameters:
                     continue
-                name = str(fwrap.fields["name"]).lower()
-                if "id" not in fwrap.fields:
-                    fwrap.fields["id"] = fwrap.id
-                _id = fwrap.fields["id"]
-                data = (
-                    fwrap.fields
-                )  # TODO: could get easier if not model_name but class used
+                name = str(fwrap.parameters["name"]).lower()
+                _id = fwrap.parameters["id"]
+                data = fwrap.parameters
+                # ⤷ TODO: could get easier if not model_name but class used
                 self.elements_by_name[name] = data
                 self.elements_by_id[_id] = data
         # for iterator
         self._iter_index: int = 0
         self._iter_list: list = list(self.elements_by_name.values())
 
     def __getitem__(self, key) -> dict:
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/base/shepherd.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/base/shepherd.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         extra = Extra.forbid  # no unnamed attributes allowed
         validate_all = True  # also checks defaults
         validate_assignment = True
         min_anystr_length = 4
         max_anystr_length = 512
         # ⤷ local str-length constraints overrule global ones!
         anystr_strip_whitespace = True  # strip leading & trailing whitespaces
-        use_enum_values = True  # cleaner export of enum-fields
+        use_enum_values = True  # cleaner export of enum-parameters
         allow_inf_nan = False  # float without +-inf or NaN
         underscore_attrs_are_private = True  # allows using them
         # Options:
         # - https://docs.pydantic.dev/usage/schema/#field-customization
         # - https://docs.pydantic.dev/usage/model_config/
         # "fields["name"].description = ... should be usable to modify model
 
@@ -75,18 +75,17 @@
     ) -> Path:
         if minimal:
             model_dict = self._min_dict
         else:
             model_dict = self.dict()
         model_wrap = Wrapper(
             model=type(self).__name__,
-            id=model_dict.get("id"),
             comment=comment,
             created=datetime.now(),
-            fields=model_dict,
+            parameters=model_dict,
         )
         model_yaml = yaml.dump(
             model_wrap.dict(), default_flow_style=False, sort_keys=False
         )
         model_path = Path(path).with_suffix(".yaml")
         with open(model_path, "w") as f:
             f.write(model_yaml)
@@ -99,15 +98,15 @@
     @classmethod
     def from_file(cls, path: Union[str, Path]):
         with open(Path(path)) as shp_file:
             shp_dict = yaml.safe_load(shp_file)
         shp_wrap = Wrapper(**shp_dict)
         if shp_wrap.model != cls.__name__:
             raise ValueError("Model in file does not match the requirement")
-        return cls(**shp_wrap.fields)
+        return cls(**shp_wrap.parameters)
 
     @classmethod  # @root_validator(pre=True, allow_reuse=True)
     def pre_snitch(cls, values):  # TODO: useless
         values["_min_dict"] = values
         return values
 
     def get_hash(self):
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/content/energy_environment.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/content/energy_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,11 +28,11 @@
     data_type: EnergyDType
 
     duration: PositiveFloat
     energy_Ws: PositiveFloat
     valid: bool = False
 
     @root_validator(pre=True)
-    def from_fixture(cls, values: dict) -> dict:
+    def query_database(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
         values, _ = fixtures.inheritance(values)
         return values
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/content/firmware.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/content/firmware.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,11 +27,11 @@
 
     mcu: MCU
 
     data: Union[constr(min_length=3, max_length=1_000_000), Path]
     data_type: FirmwareDType
 
     @root_validator(pre=True)
-    def from_fixture(cls, values: dict) -> dict:
+    def query_database(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
         values, _ = fixtures.inheritance(values)
         return values
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/content/virtual_harvester.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_harvester.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from enum import Enum
 from pathlib import Path
 from typing import Optional
 from typing import Tuple
-from typing import Union
 
 from pydantic import confloat
 from pydantic import conint
 from pydantic import root_validator
 
 from ...commons import samplerate_sps_default
 from ...logger import logger
 from ..base.calibration import CalibrationHarvester
 from ..base.content import ContentModel
 from ..base.fixture import Fixtures
 from ..base.shepherd import ShpModel
 from .energy_environment import EnergyDType
 
 fixture_path = Path(__file__).resolve().with_name("virtual_harvester_fixture.yaml")
-fixtures = Fixtures(fixture_path, "VirtualHarvester")
+fixtures = Fixtures(fixture_path, "VirtualHarvesterConfig")
 
 
 class AlgorithmDType(str, Enum):
     isc_voc = "isc_voc"
     ivcurve = ("ivcurve",)
     ivcurves = ("ivcurve",)
     cv = "cv"
@@ -30,18 +29,17 @@
     mppt_voc = "mppt_voc"
     mppt_po = "mppt_po"
     perturb_observe = "mppt_po"
     mppt_opt = "mppt_opt"
     optimal = "mppt_opt"
 
 
-class VirtualHarvester(ContentModel, title="Config for the Harvester"):
+class VirtualHarvesterConfig(ContentModel, title="Config for the Harvester"):
     """A Harvester is needed when the file-based energy environment
     of the virtual source is not already supplied as ivsample
-    TODO: Should be named -Config internally
     """
 
     # General Metadata & Ownership -> ContentModel
 
     algorithm: AlgorithmDType
     # ⤷ used to harvest energy
 
@@ -67,15 +65,15 @@
     # ⤷ direction of sawtooth
 
     # Underlying recorder
     wait_cycles: conint(ge=0, le=100) = 1
     # ⤷ first cycle: ADC-Sampling & DAC-Writing, further steps: waiting
 
     @root_validator(pre=True)
-    def from_fixture(cls, values: dict) -> dict:
+    def query_database(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
         values, chain = fixtures.inheritance(values)
         if values["name"] == "neutral":
             # TODO: same test is later done in calc_algorithm_num() again
             raise ValueError("Resulting Harvester can't be neutral")
         logger.debug("VHrv-Inheritances: %s", chain)
         return values
@@ -141,15 +139,17 @@
                 _ratio,
             )
         return interval_ms, duration_ms
 
     def get_datatype(self) -> EnergyDType:
         return algo_to_dtype[self.algorithm]
 
-    def calc_window_size(self, for_emu: bool, dtype_in: EnergyDType) -> int:
+    def calc_window_size(
+        self, for_emu: bool, dtype_in: Optional[EnergyDType] = EnergyDType.ivsample
+    ) -> int:
         if for_emu:
             if dtype_in == EnergyDType.ivcurve:
                 return self.samples_n * (1 + self.wait_cycles)
             elif dtype_in == EnergyDType.ivsample:
                 return 0
             # isc_voc: 2 * (1 + wait_cycles), noqa
             raise ValueError("Not Implemented")
@@ -185,18 +185,19 @@
     "mppt_po": EnergyDType.ivsample,
     "mppt_opt": EnergyDType.ivsample,
 }
 
 
 class HarvesterPRUConfig(ShpModel):
     """
-    Kernel-Task -> Map settings-list to internal state-vars struct ConverterConfig
+    Map settings-list to internal state-vars struct HarvesterConfig
     NOTE:
       - yaml is based on si-units like nA, mV, ms, uF
       - c-code and py-copy is using nA, uV, ns, nF, fW, raw
+      - ordering is intentional and in sync with shepherd/commons.h
     """
 
     algorithm: u32
     hrv_mode: u32
     window_size: u32
     voltage_uV: u32
     voltage_min_uV: u32
@@ -212,17 +213,17 @@
     # ⤷ of measurement
     wait_cycles_n: u32
     # ⤷ for DAC to settle
 
     @classmethod
     def from_vhrv(
         cls,
-        data: VirtualHarvester,
+        data: VirtualHarvesterConfig,
         for_emu: bool = False,
-        dtype_in: Union[str, EnergyDType] = EnergyDType.ivsample,
+        dtype_in: Optional[EnergyDType] = EnergyDType.ivsample,
         window_size: Optional[u32] = None,
     ):
         if isinstance(dtype_in, str):
             dtype_in = EnergyDType[dtype_in]
         if for_emu and dtype_in not in [EnergyDType.ivsample, EnergyDType.ivcurve]:
             raise ValueError("Not Implemented")
         # TODO: use dtype properly in shepherd
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/content/virtual_harvester_fixture.yaml` & `shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_harvester_fixture.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,159 +1,159 @@
 # info:
 # - compendium of all parameters & description
 # - look into the implementation to see which parameters are used
 # - base for neutral fallback values if provided yml is sparse
 # - -> it is encouraged to omit redundant parameters in your own implementation
-- model: VirtualHarvester
-  id: 1000
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1000
     name: neutral
     owner: Ingmar
     group: NES Lab
     visible2group: true
     visible2all: true
     created: 2022-12-12 12:12:12
 
-- model: VirtualHarvester
-  id: 1010
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1010
     name: ivcurve
     description: Postpone harvesting by sampling ivcurves (voltage stepped as sawtooth-wave)
     comment: ~200 Hz
     inherit_from: neutral
     algorithm: ivcurve
     samples_n: 250
     voltage_min_mV: 0
     voltage_max_mV: 5000
     wait_cycles: 1  # results in 200 Hz (= 100kHz /(2*250))
     rising: false # downward sawtooth seems to have advantages for solar cells
     # todo: also add switch for sawtooth- vs triangle-wave?
     # todo: could also include a version with dynamic upper-boundary, varied if voc is reached very early
 
-- model: VirtualHarvester
-  id: 1011
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1011
     name: ivcurves  # synonym
     inherit_from: ivcurve
 
-- model: VirtualHarvester
-  id: 1012
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1012
     name: iv1000
     comment: Name relates to curves per second
     inherit_from: ivcurve
     samples_n: 100
     wait_cycles: 0
 
-- model: VirtualHarvester
-  id: 1013
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1013
     name: iv110
     comment: Between 50 & 60 Hz line-frequency to avoid standing waves
     inherit_from: ivcurve
     samples_n: 909
     wait_cycles: 0
 
-- model: VirtualHarvester
-  id: 1020
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1020
     name: isc_voc
     description: Postpone harvesting by sampling short circuit current & open circuit voltage
     inherit_from: neutral
     algorithm: isc_voc
     wait_cycles: 1  # results in 25 kHz (isc, wait, voc, wait)
 
-- model: VirtualHarvester
-  id: 1030
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1030
     name: cv20
     description: Harvesting with constant Voltage
     inherit_from: neutral
     algorithm: cv
     voltage_mV: 2000
 
-- model: VirtualHarvester
-  id: 1031
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1031
     name: cv24
     inherit_from: cv20
     voltage_mV: 2400
 
-- model: VirtualHarvester
-  id: 1032
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1032
     name: cv33
     inherit_from: cv20
     voltage_mV: 3300
 
-- model: VirtualHarvester
-  id: 1032
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1032
     name: cv10
     inherit_from: cv20
     voltage_mV: 1000
 
-- model: VirtualHarvester
-  id: 1040
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1040
     name: mppt_voc
     description: MPPT based on open circuit voltage for solar
     inherit_from: neutral
     algorithm: mppt_voc
     setpoint_n: 0.76
     interval_ms: 100     # between measurements
     duration_ms: 1.2     # solar can overshoot when load is removed
     current_limit_uA: 5  # boundary for detecting open circuit in emulated version (working on IV-Curves)
 
-- model: VirtualHarvester
-  id: 1041
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1041
     name: mppt_bq
     description: MPPT of TI BQ-Converters for solar
     inherit_from: mppt_voc
     setpoint_n: 0.76
     interval_ms: 16000  # between measurements
     duration_ms: 256    # of measurement
 
-- model: VirtualHarvester
-  id: 1042
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1042
     name: mppt_bqt
     description: MPPT of TI BQ-Converters for thermoelectric
     inherit_from: mppt_voc
     setpoint_n: 0.50
     interval_ms: 16000  # between measurements
     duration_ms: 256    # of measurement
 
-- model: VirtualHarvester
-  id: 1043
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1043
     name: mppt_bq_solar # explicit naming
     inherit_from: mppt_bq
 
-- model: VirtualHarvester
-  id: 1044
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1044
     name: mppt_bq_thermoelectric # explicit naming
     inherit_from: mppt_bqt
 
-- model: VirtualHarvester
-  id: 1045
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1045
     name: mppt_po
     description: MPPT based on perturb & observe algorithm
     inherit_from: neutral
     algorithm: mppt_po
     voltage_min_mV: 0
     voltage_max_mV: 5000
     voltage_step_mV: 10
     interval_ms: 18   # between steps
 
-- model: VirtualHarvester
-  id: 1046
-  fields:
+- model: VirtualHarvesterConfig
+  parameters:
+    id: 1046
     name: mppt_opt
     description: Power-Optimum with very fast PO-Variant (harvesting) or special max-pwr-picker (emulator / ivcurve)
     inherit_from: mppt_po
     algorithm: mppt_opt
     voltage_step_mV: 1
     interval_ms: 0.01
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/content/virtual_source.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,42 +7,41 @@
 
 from ...commons import samplerate_sps_default
 from ...logger import logger
 from .. import ShpModel
 from ..base.content import ContentModel
 from ..base.fixture import Fixtures
 from .virtual_harvester import HarvesterPRUConfig
-from .virtual_harvester import VirtualHarvester
+from .virtual_harvester import VirtualHarvesterConfig
 
 fixture_path = Path(__file__).resolve().with_name("virtual_source_fixture.yaml")
-fixtures = Fixtures(fixture_path, "VirtualSource")
+fixtures = Fixtures(fixture_path, "VirtualSourceConfig")
 
 
-class VirtualSource(ContentModel, title="Config for the virtual Source"):
+class VirtualSourceConfig(ContentModel, title="Config for the virtual Source"):
     """The virtual Source uses the energy environment (file)
     for supplying the Target Node during the experiment.
     If not already done, the energy will be harvested and then converted.
     The converter-stage is software defined and offers:
       buck-boost-combinations,
       a simple diode + resistor and
       an intermediate buffer capacitor.
-      TODO: Should be named -Config internally
       TODO: I,V,R should be in regular unit (V, A, Ohm)
     """
 
     # General Metadata & Ownership -> ContentModel
 
     enable_boost: bool = False
     # ⤷ if false -> v_intermediate = v_input, output-switch-hysteresis is still usable
     enable_buck: bool = False
     # ⤷ if false -> v_output = v_intermediate
 
     interval_startup_delay_drain_ms: confloat(ge=0, le=10_000) = 0
 
-    harvester: VirtualHarvester = VirtualHarvester(name="mppt_opt")
+    harvester: VirtualHarvesterConfig = VirtualHarvesterConfig(name="mppt_opt")
 
     V_input_max_mV: confloat(ge=0, le=10_000) = 10_000
     I_input_max_mA: confloat(ge=0, le=4.29e3) = 4_200
     V_input_drop_mV: confloat(ge=0, le=4.29e6) = 0
     # ⤷ simulate input-diode
     R_input_mOhm: confloat(ge=0, le=4.29e6) = 0
     # ⤷ resistance only active with disabled boost, range [1 mOhm; 1MOhm]
@@ -104,15 +103,15 @@
         max_items=12,
     ) = 12 * [1.00]
     # ⤷ array[12] depending on output_current
     LUT_output_I_min_log2_nA: conint(ge=0, le=20) = 0
     # ⤷ 2^8 = 256 nA -> LUT[0] is for inputs < 256 nA, see notes on LUT_input for explanation
 
     @root_validator(pre=True)
-    def from_fixture(cls, values: dict) -> dict:
+    def query_database(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
         values, chain = fixtures.inheritance(values)
         logger.debug("VSrc-Inheritances: %s", chain)
         return values
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
@@ -234,14 +233,22 @@
     min_items=LUT_SIZE,
     max_items=LUT_SIZE,
 )
 lut_o = conlist(u32, min_items=LUT_SIZE, max_items=LUT_SIZE)
 
 
 class ConverterPRUConfig(ShpModel):
+    """
+    Map settings-list to internal state-vars struct ConverterConfig
+    NOTE:
+      - yaml is based on si-units like nA, mV, ms, uF
+      - c-code and py-copy is using nA, uV, ns, nF, fW, raw
+      - ordering is intentional and in sync with shepherd/commons.h
+    """
+
     converter_mode: u32
     interval_startup_delay_drain_n: u32
 
     V_input_max_uV: u32
     I_input_max_nA: u32
     V_input_drop_uV: u32
     R_input_kOhm_n22: u32
@@ -269,18 +276,17 @@
     V_buck_drop_uV: u32
 
     LUT_input_V_min_log2_uV: u32
     LUT_input_I_min_log2_nA: u32
     LUT_output_I_min_log2_nA: u32
     LUT_inp_efficiency_n8: lut_i
     LUT_out_inv_efficiency_n4: lut_o
-    LUT_size: u32 = LUT_SIZE
 
     @classmethod
-    def from_vsrc(cls, data: VirtualSource, log_intermediate_node: bool = False):
+    def from_vsrc(cls, data: VirtualSourceConfig, log_intermediate_node: bool = False):
         states = data.calc_internal_states()
         return cls(
             # General
             converter_mode=data.calc_converter_mode(log_intermediate_node),
             interval_startup_delay_drain_n=data.interval_startup_delay_drain_ms
             * samplerate_sps_default
             * 1e-3,
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/content/virtual_source_fixture.yaml` & `shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_source_fixture.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # info:
 # - compendium of all parameters & description
 # - base for neutral fallback values if provided yml is sparse
 # - -> it is encouraged to omit redundant parameters
 ---
-- model: VirtualSource
-  id: 1000
-  fields:
+- model: VirtualSourceConfig
+  parameters:
+    id: 1000
     name: neutral
     description: Direct feed-through of energy environment with no converter (allows on-off-patters)
     # General Config
     enable_boost: false # if false -> v_intermediate = v_input, output-switch-hysteresis is still usable
     enable_buck: false # if false -> v_output = v_intermediate
 
     interval_startup_delay_drain_ms: 0
@@ -69,53 +69,53 @@
 
     owner: Ingmar
     group: NES Lab
     visible2group: true
     visible2all: true
     created: 2022-12-12 12:12:12
 
-- model: VirtualSource
-  id: 1010
-  fields:
+- model: VirtualSourceConfig
+  parameters:
+    id: 1010
     name: direct
     inherit_from: neutral
     # Note: current input has no influence
 
-- model: VirtualSource
-  id: 1011
-  fields:
+- model: VirtualSourceConfig
+  parameters:
+    id: 1011
     name: diode+capacitor
     description: Simple Converter based on diode and buffer capacitor
     inherit_from: neutral
     V_input_drop_mV: 300  # simulate input-diode
     C_intermediate_uF: 10  # primary storage-Cap
 
-- model: VirtualSource
-  id: 1012
-  fields:
+- model: VirtualSourceConfig
+  parameters:
+    id: 1012
     name: dio_cap # simpler naming
     inherit_from: diode+capacitor
 
-- model: VirtualSource
-  id: 1013
-  fields:
+- model: VirtualSourceConfig
+  parameters:
+    id: 1013
     name: diode+resistor+capacitor
     description: Simple Converter based on diode, current limiting resistor and buffer capacitor
     inherit_from: diode+capacitor
     R_input_mOhm: 10000
 
-- model: VirtualSource
-  id: 1014
-  fields:
+- model: VirtualSourceConfig
+  parameters:
+    id: 1014
     name: dio_res_cap # simpler naming
     inherit_from: diode+resistor+capacitor
 
-- model: VirtualSource
-  id: 1020
-  fields:
+- model: VirtualSourceConfig
+  parameters:
+    id: 1020
     name: BQ25504
     description: TI BQ25504 with integrated boost-converter
     inherit_from: neutral # to complete undefined vars
     enable_boost: true # if false -> v_intermediate = v_input, output-switch-hysteresis is still usable
 
     harvester:
       name: mppt_bq_solar # harvester only active if input is "ivcurves"
@@ -153,31 +153,31 @@
       [ 0.56, 0.78, 0.79, 0.81, 0.83, 0.85, 0.87, 0.88, 0.88, 0.88, 0.88, 0.89 ], # > 1152 mV
       [ 0.58, 0.79, 0.80, 0.82, 0.84, 0.86, 0.88, 0.89, 0.89, 0.89, 0.89, 0.90 ], # > 1280 mV
       [ 0.60, 0.80, 0.81, 0.83, 0.85, 0.87, 0.89, 0.90, 0.90, 0.90, 0.90, 0.90 ], # > 1408 mV
     ] # input-array[12][12] depending on array[inp_voltage][log(inp_current)], influence of cap-voltage is not implemented
     LUT_input_V_min_log2_uV: 17 # example: 2^7 = 128 uV -> array[0] is for inputs < 128 uV
     LUT_input_I_min_log2_nA: 13 # example: 2^8 = 256 nA -> array[0] is for inputs < 256 nA
 
-- model: VirtualSource
-  id: 1021
-  fields:
+- model: VirtualSourceConfig
+  parameters:
+    id: 1021
     name: BQ25504s # Version with Schmitt-Trigger
     description: TI BQ25504 with Schmitt-Trigger for a faster power-good-signal
     inherit_from: BQ25504
     immediate_pwr_good_signal: true
 
-- model: VirtualSource
-  id: 1022
-  fields:
+- model: VirtualSourceConfig
+  parameters:
+    id: 1022
     name: BQ25504-Schmitt
     inherit_from: BQ25504s
 
-- model: VirtualSource
-  id: 1030
-  fields:
+- model: VirtualSourceConfig
+  parameters:
+    id: 1030
     name: BQ25570
     description: TI BQ25570 with integrated boost- & buck-converter
     inherit_from: BQ25504 # inherit Input-LUT that is similar enough
     enable_boost: true # if false -> v_intermediate = v_input, output-switch-hysteresis is still usable
     enable_buck: true # if false -> v_output = v_intermediate
 
     V_input_max_mV: 5100
@@ -205,25 +205,25 @@
     V_output_mV: 2200
     V_buck_drop_mV: 200.0  # simulate LDO min voltage differential or output-diode
 
     #                        <1u   1u    2u    4u    8u    16u   32u   64u   128u  256u  512u  >1m
     LUT_output_efficiency: [ 0.40, 0.50, 0.60, 0.73, 0.82, 0.86, 0.88, 0.90, 0.91, 0.92, 0.93, 0.92] # array[12] depending on output_current
     LUT_output_I_min_log2_nA: 10  # example: 2^8 = 256 nA -> array[0] is for inputs < 256 nA, see notes on LUT_input for explanation
 
-- model: VirtualSource
-  id: 1031
-  fields:
+- model: VirtualSourceConfig
+  parameters:
+    id: 1031
     name: BQ25570s
     description: TI BQ25570 with Schmitt-Trigger for a faster power-good-signal
     inherit_from: BQ25570
     immediate_pwr_good_signal: true
 
-- model: VirtualSource
-  id: 1032
-  fields:
+- model: VirtualSourceConfig
+  parameters:
+    id: 1032
     name: BQ25570-Schmitt
     inherit_from: BQ25570s
-- model: VirtualSource
-  id: 1033
-  fields:
+- model: VirtualSourceConfig
+  parameters:
+    id: 1033
     name: default
     inherit_from: BQ25570s
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/doc_virtual_source.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/doc_virtual_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pydantic import conlist
 from pydantic import root_validator
 
 from shepherd_core.data_models import Fixtures
 from shepherd_core.data_models import ShpModel
 
 from .. import logger
-from .content import VirtualHarvester
+from .content import VirtualHarvesterConfig
 
 fixture_path = Path(__file__).resolve().with_name("content/virtual_source_fixture.yaml")
 fixtures = Fixtures(fixture_path, "content.VirtualSource")
 
 
 @DeprecationWarning
 class VirtualSourceDoc(ShpModel, title="Virtual Source (Documented, Testversion)"):
@@ -46,17 +46,17 @@
     interval_startup_delay_drain_ms: float = Field(
         description="Model begins running but Target is not draining the buffer",
         default=0,
         ge=0,
         le=10e3,
     )
 
-    harvester: VirtualHarvester = Field(
+    harvester: VirtualHarvesterConfig = Field(
         description="Only active / needed if input is 'ivcurves'",
-        default=VirtualHarvester(name="mppt_opt"),
+        default=VirtualHarvesterConfig(name="mppt_opt"),
     )
 
     V_input_max_mV: float = Field(
         description="Maximum input Voltage [mV]",
         default=10_000,
         ge=0,
         le=10e3,
@@ -220,12 +220,12 @@
         "see notes on LUT_input for explanation",
         default=0,
         ge=0,
         le=20,
     )
 
     @root_validator(pre=True)
-    def from_fixture(cls, values: dict) -> dict:
+    def query_database(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
         values, chain = fixtures.inheritance(values)
         logger.debug("VSrc-Inheritances: %s", chain)
         return values
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/experiment/__init__.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/experiment/experiment.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/experiment/observer_features.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/experiment/observer_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 class PowerTracing(ShpModel, title="Config for Power-Tracing"):
     """Configuration for recording the Power-Consumption of the Target Nodes
     TODO: postprocessing not implemented ATM
     """
 
     intermediate_voltage: bool = False
-    # ⤷ record buffer capacitor instead of output (good for V_out = const)
-    # TODO: also switch current to buffer-cap? seems reasonable
+    # ⤷ for EMU: record buffer capacitor instead of output (good for V_out = const)
+    #            this also includes current!
 
     # time
     delay: conint(ge=0) = 0
     duration: Optional[conint(ge=0)] = None  # will be max
 
     # post-processing
     calculate_power: bool = False
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/experiment/target_config.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/experiment/target_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pydantic import conlist
 from pydantic import root_validator
 
 from ..base.content import IdInt
 from ..base.shepherd import ShpModel
 from ..content.energy_environment import EnergyEnvironment
 from ..content.firmware import Firmware
-from ..content.virtual_source import VirtualSource
+from ..content.virtual_source import VirtualSourceConfig
 from ..testbed.target import IdInt16
 from ..testbed.target import Target
 from .observer_features import GpioActuation
 from .observer_features import GpioTracing
 from .observer_features import PowerTracing
 
 
@@ -20,15 +20,15 @@
     """Configuration for Target Nodes (DuT)"""
 
     target_IDs: conlist(item_type=IdInt, min_items=1, max_items=64)
     custom_IDs: Optional[conlist(item_type=IdInt16, min_items=1, max_items=64)]
     # ⤷ will replace 'const uint16_t SHEPHERD_NODE_ID' in firmware
 
     energy_env: EnergyEnvironment  # alias: input
-    virtual_source: VirtualSource = VirtualSource(name="neutral")
+    virtual_source: VirtualSourceConfig = VirtualSourceConfig(name="neutral")
     target_delays: Optional[conlist(item_type=conint(ge=0), min_items=1, max_items=64)]
     # ⤷ individual starting times -> allows to use the same environment
 
     firmware1: Firmware
     firmware2: Optional[Firmware] = None
 
     power_tracing: Optional[PowerTracing]
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/task/emulation.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/task/emulation.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pydantic import root_validator
 from pydantic import validate_arguments
 
 from shepherd_core.data_models.testbed import Testbed
 
 from ..base.content import IdInt
 from ..base.shepherd import ShpModel
-from ..content.virtual_source import VirtualSource
+from ..content.virtual_source import VirtualSourceConfig
 from ..experiment.experiment import Experiment
 from ..experiment.observer_features import GpioActuation
 from ..experiment.observer_features import GpioTracing
 from ..experiment.observer_features import PowerTracing
 from ..experiment.observer_features import SystemLogging
 from ..testbed.cape import TargetPort
 
@@ -73,15 +73,17 @@
     voltage_aux: Union[confloat(ge=0, le=4.5), str] = 0
     # ⤷ aux_voltage options:
     #   - 0-4.5 for specific const Voltage (0 V = disabled),
     #   - "buffer" will output intermediate voltage (storage cap of vsource),
     #   - "main" will mirror main target voltage
 
     # sub-elements, could be partly moved to emulation
-    virtual_source: VirtualSource = VirtualSource(name="neutral")  # {"name": "neutral"}
+    virtual_source: VirtualSourceConfig = VirtualSourceConfig(
+        name="neutral"
+    )  # {"name": "neutral"}
     # ⤷ Use the desired setting for the virtual source,
     #   provide parameters or name like BQ25570
 
     power_tracing: Optional[PowerTracing] = PowerTracing()
     gpio_tracing: Optional[GpioTracing] = GpioTracing()
     gpio_actuation: Optional[GpioActuation] = None
     sys_logging: Optional[SystemLogging] = SystemLogging()
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/task/firmware_mod.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/task/firmware_mod.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/task/harvest.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/task/harvest.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from datetime import timedelta
 from pathlib import Path
 from typing import Optional
 
 from pydantic import root_validator
 
 from ..base.shepherd import ShpModel
-from ..content.virtual_harvester import VirtualHarvester
+from ..content.virtual_harvester import VirtualHarvesterConfig
+from ..experiment.observer_features import PowerTracing
+from ..experiment.observer_features import SystemLogging
 from .emulation import Compression
 
 
 class HarvestTask(ShpModel):
     """Configuration for the Observer in Harvest-Mode
     Record IV data from a harvest-source
     """
@@ -32,18 +34,21 @@
     # ⤷ Duration of recording in seconds, None = till EOF
     abort_on_error: bool = False
 
     # emulation-specific
     use_cal_default: bool = False
     # ⤷ Use default calibration values, skip loading from EEPROM
 
-    virtual_harvester: VirtualHarvester = VirtualHarvester(name="mppt_opt")
+    virtual_harvester: VirtualHarvesterConfig = VirtualHarvesterConfig(name="mppt_opt")
     # ⤷ Choose one of the predefined virtual harvesters
     #   or configure a new one
 
+    power_tracing: Optional[PowerTracing] = PowerTracing()
+    sys_logging: Optional[SystemLogging] = SystemLogging()
+
     # TODO: there is an unused DAC-Output patched to the harvesting-port
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         # TODO: limit paths
         has_start = values.get("time_start") is not None
         if has_start and values["time_start"] < datetime.utcnow():
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/task/observer_tasks.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/task/observer_tasks.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/task/programming.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/task/programming.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/task/testbed_tasks.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/task/testbed_tasks.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/__init__.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/cape.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/cape.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     created: Union[date, datetime] = Field(default_factory=datetime.now)
     calibrated: Union[date, datetime, None] = None
 
     def __str__(self):
         return self.name
 
     @root_validator(pre=True)
-    def from_fixture(cls, values: dict) -> dict:
+    def query_database(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
         values, _ = fixtures.inheritance(values)
         return values
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/gpio.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/gpio.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     reg_sys: Optional[conint(ge=0)] = None
     pin_sys: Optional[constr(max_length=10)] = None
 
     def __str__(self):
         return self.name
 
     @root_validator(pre=True)
-    def from_fixture(cls, values: dict) -> dict:
+    def query_database(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
         values, _ = fixtures.inheritance(values)
         return values
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         # ensure that either pru or sys is used, otherwise instance is considered faulty
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/gpio_fixture.yaml` & `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/gpio_fixture.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,166 +1,166 @@
 --- # add with >>> python manage.py loaddata <fixturename>
 # cape v2.4
 - model: gpio
-  id: 1000
-  fields:
+  parameters:
+    id: 1000
     name: GPIO0
     # description:
     # comment:
     direction: IO
     dir_switch: DIR1
     reg_pru: r31_00
     pin_pru: P8_45
     reg_sys: 26
     pin_sys: P8_14
 - model: gpio
-  id: 1001
-  fields:
+  parameters:
+    id: 1001
     name: GPIO1
     direction: IO
     dir_switch: DIR1
     reg_pru: r31_01
     pin_pru: P8_46
     reg_sys: 27
     pin_sys: P8_17
 - model: gpio
-  id: 1002
-  fields:
+  parameters:
+    id: 1002
     name: GPIO2
     direction: IO
     dir_switch: DIR1
     reg_pru: r31_02
     pin_pru: P8_43
     reg_sys: 46
     pin_sys: P8_16
 - model: gpio
-  id: 1003
-  fields:
+  parameters:
+    id: 1003
     name: GPIO3
     direction: IO
     dir_switch: DIR1
     reg_pru: r31_03
     pin_pru: P8_44
     reg_sys: 47
     pin_sys: P8_15
 - model: gpio
-  id: 1004
-  fields:
+  parameters:
+    id: 1004
     name: GPIO4
     direction: IN
     reg_pru: r31_04
     pin_pru: P8_41
     reg_sys: 61
     pin_sys: P8_26
 - model: gpio
-  id: 1005
-  fields:
+  parameters:
+    id: 1005
     name: GPIO5
     direction: IN
     reg_pru: r31_05
     pin_pru: P8_42
     reg_sys: 80
     pin_sys: P8_36
 - model: gpio
-  id: 1006
-  fields:
+  parameters:
+    id: 1006
     name: GPIO6
     direction: IN
     reg_pru: r31_06
     pin_pru: P8_39
     reg_sys: 81
     pin_sys: P8_34
 - model: gpio
-  id: 1007
-  fields:
+  parameters:
+    id: 1007
     name: GPIO7
     description: alias UART_RX
     direction: IN
     reg_pru: r31_07
     pin_pru: P8_40
     reg_sys: 14
     pin_sys: P9_26
 - model: gpio
-  id: 1008
-  fields:
+  parameters:
+    id: 1008
     name: GPIO8
     description: alias UART_TX
     direction: IO
     dir_switch: DIR2
     reg_pru: r31_08
     pin_pru: P8_27
     reg_sys: 15
     pin_sys: P9_24
 - model: gpio
-  id: 1009
-  fields:
+  parameters:
+    id: 1009
     name: BAT_OK
     description: signal from vSource (PRU) to target
     direction: OUT
     reg_pru: r30_09
     pin_pru: P8_29
 - model: gpio
-  id: 2000
-  fields:
+  parameters:
+    id: 2000
     name: PRG1_CLK
     description: alias JTAG_TCK
     direction: OUT
     reg_sys: 5
     pin_sys: P9_17
 - model: gpio
-  id: 2001
-  fields:
+  parameters:
+    id: 2001
     name: PRG1_IO
     description: alias JTAG_TDI
     direction: IO
     dir_switch: PDIR1
     reg_sys: 4
     pin_sys: P9_18
 - model: gpio
-  id: 2010
-  fields:
+  parameters:
+    id: 2010
     name: PRG2_CLK
     description: alias JTAG_TDO
     direction: OUT
     reg_sys: 8
     pin_sys: P8_35
 - model: gpio
-  id: 2011
-  fields:
+  parameters:
+    id: 2011
     name: PRG2_IO
     description: alias JTAG_TMS
     direction: IO
     dir_switch: PDIR2
     reg_sys: 9
     pin_sys: P8_33
 - model: gpio
-  id: 3000
-  fields:
+  parameters:
+    id: 3000
     name: DIR1
     description: changes direction of GPIO[0:3]
     direction: OUT
     reg_sys: 78
     pin_sys: P8_37
 - model: gpio
-  id: 3001
-  fields:
+  parameters:
+    id: 3001
     name: DIR2
     description: changes direction of GPIO8
     direction: OUT
     reg_sys: 79
     pin_sys: P8_38
 - model: gpio
-  id: 3002
-  fields:
+  parameters:
+    id: 3002
     name: PDIR1
     description: changes direction PRG1_IO
     direction: OUT
     reg_sys: 10
     pin_sys: P8_31
 - model: gpio
-  id: 3003
-  fields:
+  parameters:
+    id: 3003
     name: PDIR2
     description: changes direction PRG2_IO
     direction: OUT
     reg_sys: 11
     pin_sys: P8_32
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/mcu.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/mcu.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,11 +41,11 @@
     fw_name_default: str
     # ⤷ can't be FW-Object (circular import)
 
     def __str__(self):
         return self.name
 
     @root_validator(pre=True)
-    def from_fixture(cls, values: dict) -> dict:
+    def query_database(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
         values, _ = fixtures.inheritance(values)
         return values
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/observer.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/observer.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     created: datetime = Field(default_factory=datetime.now)
     alive_last: Optional[datetime]
 
     def __str__(self):
         return self.name
 
     @root_validator(pre=True)
-    def from_fixture(cls, values: dict) -> dict:
+    def query_database(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
         values, _ = fixtures.inheritance(values)
         return values
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         has_cape = values.get("cape") is not None
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/target.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/target.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     # TODO programming pins per mcu should be here (or better in Cape)
 
     def __str__(self):
         return self.name
 
     @root_validator(pre=True)
-    def from_fixture(cls, values: dict) -> dict:
+    def query_database(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
         values, _ = fixtures.inheritance(values)
         return values
 
     @root_validator(pre=False)
     def post_correction(cls, values: dict) -> dict:
         if isinstance(values.get("mcu1"), str):
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/testbed.py` & `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/testbed.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     data_on_observer: Path
     # ⤷ storage layout: root_path/content_type/group/owner/[object]
 
     prep_duration: timedelta = timedelta(minutes=5)
     # TODO: one BBone is currently time-keeper
 
     @root_validator(pre=True)
-    def from_fixture(cls, values: dict) -> dict:
+    def query_database(cls, values: dict) -> dict:
         values = fixtures.lookup(values)  # TODO: load from url
         values, _ = fixtures.inheritance(values)
         return values
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         observers = []
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/logger.py` & `shepherd_core-2023.6.1/shepherd_core/logger.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/shepherd_core/reader.py` & `shepherd_core-2023.6.1/shepherd_core/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,19 +34,19 @@
         verbose: more info during usage, 'None' skips the setter
     """
 
     samples_per_buffer: int = 10_000
 
     mode_dtype_dict = {
         "harvester": [
-            EnergyDType.ivsample.name,
-            EnergyDType.ivcurve.name,
-            EnergyDType.isc_voc.name,
+            EnergyDType.ivsample,
+            EnergyDType.ivcurve,
+            EnergyDType.isc_voc,
         ],
-        "emulator": [EnergyDType.ivsample.name],
+        "emulator": [EnergyDType.ivsample],
     }
 
     @validate_arguments
     def __init__(self, file_path: Optional[Path], verbose: Optional[bool] = True):
         if not hasattr(self, "file_path"):
             self.file_path: Optional[Path] = None
             if isinstance(file_path, (Path, str)):
@@ -214,18 +214,21 @@
         return {}
 
     def get_hostname(self) -> str:
         if "hostname" in self.h5file.attrs:
             return self.h5file.attrs["hostname"]
         return "unknown"
 
-    def get_datatype(self) -> str:
-        if "datatype" in self.h5file["data"].attrs:
-            return self.h5file["data"].attrs["datatype"]
-        return ""
+    def get_datatype(self) -> Optional[EnergyDType]:
+        try:
+            if "datatype" in self.h5file["data"].attrs:
+                return EnergyDType[self.h5file["data"].attrs["datatype"]]
+            return None
+        except KeyError:
+            return None
 
     def get_hrv_config(self) -> dict:
         """essential info for harvester
         :return: config-dict directly for vHarvester to be used during emulation
         """
         return {
             "dtype": self.get_datatype(),
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/vsource/virtual_converter_model.py` & `shepherd_core-2023.6.1/shepherd_core/vsource/virtual_converter_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 """
 
 import math
 from typing import Optional
 
 from shepherd_core import CalibrationEmulator
+from shepherd_core.data_models.content.virtual_source import LUT_SIZE
 from shepherd_core.data_models.content.virtual_source import ConverterPRUConfig
 
 
 class PruCalibration:
     """part of calibration.h"""
 
     def __init__(self, cal_emu: Optional[CalibrationEmulator] = None):
@@ -220,25 +221,25 @@
         return self.V_out_dac_raw
 
     def get_input_efficiency(self, voltage_uV: float, current_nA: float) -> float:
         voltage_n = int(voltage_uV / (2**self._cfg.LUT_input_V_min_log2_uV))
         current_n = int(current_nA / (2**self._cfg.LUT_input_I_min_log2_nA))
         pos_v = int(voltage_n) if (voltage_n > 0) else 0  # V-Scale is Linear!
         pos_c = int(math.log2(current_n)) if (current_n > 0) else 0
-        if pos_v >= self._cfg.LUT_size:
-            pos_v = self._cfg.LUT_size - 1
-        if pos_c >= self._cfg.LUT_size:
-            pos_c = self._cfg.LUT_size - 1
+        if pos_v >= LUT_SIZE:
+            pos_v = LUT_SIZE - 1
+        if pos_c >= LUT_SIZE:
+            pos_c = LUT_SIZE - 1
         return self._cfg.LUT_inp_efficiency_n8[pos_v][pos_c] / (2**8)
 
     def get_output_inv_efficiency(self, current_nA: float) -> float:
         current_n = int(current_nA / (2**self._cfg.LUT_output_I_min_log2_nA))
         pos_c = int(math.log2(current_n)) if (current_n > 0) else 0
-        if pos_c >= self._cfg.LUT_size:
-            pos_c = self._cfg.LUT_size - 1
+        if pos_c >= LUT_SIZE:
+            pos_c = LUT_SIZE - 1
         return self._cfg.LUT_out_inv_efficiency_n4[pos_c] / (2**4)
 
     def set_P_input_fW(self, value: float) -> None:
         self.P_inp_fW = value
 
     def set_P_output_fW(self, value: float) -> None:
         self.P_out_fW = value
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/vsource/virtual_harvester_model.py` & `shepherd_core-2023.6.1/shepherd_core/vsource/virtual_harvester_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/shepherd_core/vsource/virtual_source_model.py` & `shepherd_core-2023.6.1/shepherd_core/vsource/virtual_source_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,37 +9,37 @@
 
 """
 from typing import Optional
 
 from shepherd_core import CalibrationEmulator
 
 from ..data_models import EnergyDType
-from ..data_models import VirtualSource
+from ..data_models import VirtualSourceConfig
 from ..data_models.content.virtual_harvester import HarvesterPRUConfig
 from ..data_models.content.virtual_source import ConverterPRUConfig
 from .virtual_converter_model import PruCalibration
 from .virtual_converter_model import VirtualConverterModel
 from .virtual_harvester_model import VirtualHarvesterModel
 
 
 class VirtualSourceModel:
     """part of sampling.c"""
 
     def __init__(
         self,
-        vsrc: Optional[VirtualSource],
+        vsrc: Optional[VirtualSourceConfig],
         cal_emu: CalibrationEmulator,
         log_intermediate: bool = False,
         dtype_in: EnergyDType = EnergyDType.ivsample,
         window_size: Optional[int] = None,
     ):
         self._cal_emu: CalibrationEmulator = cal_emu
         self._cal_pru: PruCalibration = PruCalibration(cal_emu)
 
-        self.cfg_src = VirtualSource() if vsrc is None else vsrc
+        self.cfg_src = VirtualSourceConfig() if vsrc is None else vsrc
         cnv_config = ConverterPRUConfig.from_vsrc(
             self.cfg_src, log_intermediate_node=log_intermediate
         )
         self.cnv: VirtualConverterModel = VirtualConverterModel(
             cnv_config, self._cal_pru
         )
 
@@ -69,15 +69,15 @@
 
         P_inp_fW = self.cnv.calc_inp_power(V_inp_uV, I_inp_nA)
 
         # fake ADC read
         A_out_raw = self._cal_emu.adc_C_A.si_to_raw(I_out_nA * 10**-9)
 
         P_out_fW = self.cnv.calc_out_power(A_out_raw)
-        self.cnv.update_cap_storage()
+        V_mid_uV = self.cnv.update_cap_storage()
         V_out_raw = self.cnv.update_states_and_output()
         V_out_uV = int(self._cal_emu.dac_V_A.raw_to_si(V_out_raw) * 10**6)
 
         self.W_inp_fWs += P_inp_fW
         self.W_out_fWs += P_out_fW
 
-        return V_out_uV
+        return V_mid_uV if self.cnv.get_state_log_intermediate() else V_out_uV
```

### Comparing `shepherd_core-2023.5.6/shepherd_core/writer.py` & `shepherd_core-2023.6.1/shepherd_core/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,24 +62,24 @@
             otherwise a unique name will be found
         compression: (str) use either None, lzf or "1" (gzips compression level)
         verbose: (bool) provides more info instead of just warnings / errors
     """
 
     comp_default: int = 1
     mode_default: str = "harvester"
-    datatype_default: str = EnergyDType.ivsample.name
+    datatype_default: str = EnergyDType.ivsample
 
     _chunk_shape: tuple = (BaseReader.samples_per_buffer,)
 
     @validate_arguments
     def __init__(
         self,
         file_path: Path,
         mode: Optional[str] = None,
-        datatype: Optional[str] = None,
+        datatype: Union[str, EnergyDType, None] = None,
         window_samples: Optional[int] = None,
         cal_data: Union[CalSeries, CalEmu, CalHrv, None] = None,
         compression: Compression = Compression.default,
         modify_existing: bool = False,
         force_overwrite: bool = False,
         verbose: Optional[bool] = True,
     ):
@@ -106,28 +106,30 @@
 
         if isinstance(mode, str) and mode not in self.mode_dtype_dict:
             raise ValueError(
                 f"Can't handle mode '{mode}' " f"(choose one of {self.mode_dtype_dict})"
             )
 
         _dtypes = self.mode_dtype_dict[mode if mode else self.mode_default]
-        if isinstance(datatype, str) and datatype not in _dtypes:
+        if isinstance(datatype, str):
+            datatype = EnergyDType[datatype]
+        if isinstance(datatype, EnergyDType) and datatype not in _dtypes:
             raise ValueError(
                 f"Can't handle value '{datatype}' of datatype "
                 f"(choose one of {_dtypes})"
             )
 
         if self._modify:
             self._mode = mode
             self._datatype = datatype
             self._window_samples = window_samples
         else:
             self._mode = mode if isinstance(mode, str) else self.mode_default
             self._datatype = (
-                datatype if isinstance(datatype, str) else self.datatype_default
+                datatype if isinstance(datatype, EnergyDType) else self.datatype_default
             )
             self._window_samples = (
                 window_samples if isinstance(window_samples, int) else 0
             )
 
         if isinstance(cal_data, (CalEmu, CalHrv)):
             self._cal = CalSeries.from_cal(cal_data)
@@ -151,18 +153,18 @@
         )
 
         # Store the mode in order to allow user to differentiate harvesting vs emulation data
         if isinstance(self._mode, str) and self._mode in self.mode_dtype_dict:
             self.h5file.attrs["mode"] = self._mode
 
         if (
-            isinstance(self._datatype, str)
+            isinstance(self._datatype, EnergyDType)
             and self._datatype in self.mode_dtype_dict[self.get_mode()]
         ):
-            self.h5file["data"].attrs["datatype"] = self._datatype
+            self.h5file["data"].attrs["datatype"] = self._datatype.name
         elif not self._modify:
             self._logger.error("datatype invalid? '%s' not written", self._datatype)
 
         if isinstance(self._window_samples, int):
             self.h5file["data"].attrs["window_samples"] = self._window_samples
         if datatype == EnergyDType.ivcurve and (self._window_samples in [None, 0]):
             raise ValueError("Window Size argument needed for ivcurve-Datatype")
```

### Comparing `shepherd_core-2023.5.6/shepherd_core.egg-info/PKG-INFO` & `shepherd_core-2023.6.1/shepherd_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd-core
-Version: 2023.5.6
+Version: 2023.6.1
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-core/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
```

### Comparing `shepherd_core-2023.5.6/shepherd_core.egg-info/SOURCES.txt` & `shepherd_core-2023.6.1/shepherd_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/tests/conftest.py` & `shepherd_core-2023.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/tests/data_models/example_cal_data.yaml` & `shepherd_core-2023.6.1/tests/data_models/example_cal_data.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 model: CalibrationCape
 comment: sheep0
-fields:
+parameters:
   emulator:
     adc_C_A:
       gain: 2.2306053900482405e-07
       offset: -0.0026222400965270985
     adc_C_B:
       gain: 2.2306053900482405e-07
       offset: -0.0026222400965270985
```

### Comparing `shepherd_core-2023.5.6/tests/data_models/example_cal_data_faulty.yaml` & `shepherd_core-2023.6.1/tests/data_models/example_cal_data_faulty.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 model: CalibrationCape
 comment: sheep0
-fields:
+parameters:
   emulator:
     adc_C_A:  # faulty 1
       gain: 512
       offset: -128000
     adc_C_B:
       gain: 2.2306053900482405
       offset: -0.0026222400965270985
```

### Comparing `shepherd_core-2023.5.6/tests/data_models/example_cal_meas.yaml` & `shepherd_core-2023.6.1/tests/data_models/example_cal_meas.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 model: CalMeasurementCape
 comment: sheep0
-fields:
+parameters:
   emulator:
     adc_C_A:
     - reference_si: 1.0e-05
       shepherd_raw: 647.0605606009001
     - reference_si: 3.0e-05
       shepherd_raw: 759.2687092956633
     - reference_si: 0.0001
```

### Comparing `shepherd_core-2023.5.6/tests/data_models/example_cal_meas_faulty1.yaml` & `shepherd_core-2023.6.1/tests/data_models/example_cal_meas_faulty1.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 model: CalMeasurementCape
 comment: sheep0
-fields:
+parameters:
   emulator:
     adc_C_A: # should trigger faulty correlation
     - reference_si: 1.0e-05
       shepherd_raw: 647.0605606009001
     - reference_si: 2.0e-05
       shepherd_raw: 1247.0605606009001
     - reference_si: 3.0e-05
```

### Comparing `shepherd_core-2023.5.6/tests/data_models/example_cal_meas_faulty2.yaml` & `shepherd_core-2023.6.1/tests/data_models/example_cal_meas_faulty2.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 model: CalMeasurementCape
 comment: sheep0
-fields:
+parameters:
   emulator:
     adc_C_A:
     - reference_si: 1.0e-05
       shepherd_raw: 647.0605606009001
     - reference_si: 1.0e-05
       shepherd_raw: 647.0605606009001
     - reference_si: 1.0e-05
```

### Comparing `shepherd_core-2023.5.6/tests/data_models/example_config_emulator.yaml` & `shepherd_core-2023.6.1/tests/data_models/example_config_emulator.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/tests/data_models/example_config_harvester.yaml` & `shepherd_core-2023.6.1/tests/data_models/example_config_harvester.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/tests/data_models/example_config_virtsource.yaml` & `shepherd_core-2023.6.1/tests/data_models/example_config_virtsource.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/tests/data_models/test_base_models.py` & `shepherd_core-2023.6.1/tests/data_models/test_base_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/tests/data_models/test_content_fixtures.py` & `shepherd_core-2023.6.1/tests/data_models/test_content_fixtures.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from shepherd_core.data_models.content.energy_environment import EnergyEnvironment
 from shepherd_core.data_models.content.energy_environment import fixtures as fix_ee
 from shepherd_core.data_models.content.firmware import Firmware
 from shepherd_core.data_models.content.firmware import fixtures as fix_firmware
 from shepherd_core.data_models.content.virtual_harvester import HarvesterPRUConfig
-from shepherd_core.data_models.content.virtual_harvester import VirtualHarvester
+from shepherd_core.data_models.content.virtual_harvester import VirtualHarvesterConfig
 from shepherd_core.data_models.content.virtual_harvester import fixtures as fix_hrv
 from shepherd_core.data_models.content.virtual_source import ConverterPRUConfig
-from shepherd_core.data_models.content.virtual_source import VirtualSource
+from shepherd_core.data_models.content.virtual_source import VirtualSourceConfig
 from shepherd_core.data_models.content.virtual_source import fixtures as fix_src
 
 
 def test_testbed_fixture_energy_environment() -> None:
     for fix in fix_ee:
         EnergyEnvironment(name=fix["name"])
         EnergyEnvironment(id=fix["id"])
@@ -23,22 +23,22 @@
             continue
         Firmware(name=fix["name"])
         Firmware(id=fix["id"])
 
 
 def test_experiment_fixture_vsrc() -> None:
     for fix in fix_src:
-        vsrc = VirtualSource(name=fix["name"])
-        VirtualSource(id=fix["id"])
+        vsrc = VirtualSourceConfig(name=fix["name"])
+        VirtualSourceConfig(id=fix["id"])
         ConverterPRUConfig.from_vsrc(vsrc, log_intermediate_node=False)
         ConverterPRUConfig.from_vsrc(vsrc, log_intermediate_node=True)
 
 
 def test_experiment_fixture_vhrv() -> None:
     for fix in fix_hrv:
         if fix["name"] == "neutral":
             continue
-        vhrv = VirtualHarvester(name=fix["name"])
-        VirtualHarvester(id=fix["id"])
+        vhrv = VirtualHarvesterConfig(name=fix["name"])
+        VirtualHarvesterConfig(id=fix["id"])
         HarvesterPRUConfig.from_vhrv(vhrv, for_emu=False)
         if int(fix["id"]) >= 1030:
             HarvesterPRUConfig.from_vhrv(vhrv, for_emu=True)
```

### Comparing `shepherd_core-2023.5.6/tests/data_models/test_content_models.py` & `shepherd_core-2023.6.1/tests/data_models/test_content_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 from pydantic import ValidationError
 
 from shepherd_core.data_models.content import EnergyDType
 from shepherd_core.data_models.content import EnergyEnvironment
 from shepherd_core.data_models.content import Firmware
 from shepherd_core.data_models.content import FirmwareDType
-from shepherd_core.data_models.content import VirtualHarvester
-from shepherd_core.data_models.content import VirtualSource
+from shepherd_core.data_models.content import VirtualHarvesterConfig
+from shepherd_core.data_models.content import VirtualSourceConfig
 from shepherd_core.data_models.content.virtual_source import ConverterPRUConfig
 from shepherd_core.data_models.testbed import MCU
 
 
 def test_content_model_ee_min1() -> None:
     EnergyEnvironment(
         id=9999,
@@ -46,107 +46,109 @@
         data_type=FirmwareDType.base64_hex,
         owner="Obelix",
         group="Gaul",
     )
 
 
 def test_content_model_hrv_min() -> None:
-    hrv = VirtualHarvester(
+    hrv = VirtualHarvesterConfig(
         id=9999,
         name="whatever",
         owner="jane",
         group="wayne",
         algorithm="mppt_opt",
     )
     assert hrv.get_datatype() == "ivsample"
 
 
 def test_content_model_hrv_neutral() -> None:
     with pytest.raises(ValueError):
-        _ = VirtualHarvester(name="neutral")
+        _ = VirtualHarvesterConfig(name="neutral")
 
 
 @pytest.mark.parametrize("name", ["iv110", "cv24", "mppt_voc", "mppt_po"])
 def test_content_model_hrv_by_name(name: str) -> None:
-    _ = VirtualHarvester(name=name)
+    _ = VirtualHarvesterConfig(name=name)
 
 
 @pytest.mark.parametrize("uid", [1013, 1020, 1032, 1044, 1045, 1046])
 def test_content_model_hrv_by_id(uid: int) -> None:
-    _ = VirtualHarvester(id=uid)
+    _ = VirtualHarvesterConfig(id=uid)
 
 
 def test_content_model_hrv_steps() -> None:
-    hrv = VirtualHarvester(
+    hrv = VirtualHarvesterConfig(
         name="ivcurves", voltage_min_mV=1000, voltage_max_mV=4000, samples_n=11
     )
     assert hrv.voltage_step_mV == 300
 
 
 def test_content_model_hrv_faulty_voltage0() -> None:
     with pytest.raises(ValidationError):
-        _ = VirtualHarvester(name="iv110", voltage_max_mV=5001)
+        _ = VirtualHarvesterConfig(name="iv110", voltage_max_mV=5001)
     with pytest.raises(ValidationError):
-        _ = VirtualHarvester(name="iv110", voltage_min_mV=-1)
+        _ = VirtualHarvesterConfig(name="iv110", voltage_min_mV=-1)
 
 
 def test_content_model_hrv_faulty_voltage1() -> None:
     with pytest.raises(ValueError):
-        _ = VirtualHarvester(name="iv110", voltage_min_mV=4001, voltage_max_mV=4000)
+        _ = VirtualHarvesterConfig(
+            name="iv110", voltage_min_mV=4001, voltage_max_mV=4000
+        )
 
 
 def test_content_model_hrv_faulty_voltage2() -> None:
     with pytest.raises(ValueError):
-        _ = VirtualHarvester(name="iv110", voltage_mV=4001, voltage_max_mV=4000)
+        _ = VirtualHarvesterConfig(name="iv110", voltage_mV=4001, voltage_max_mV=4000)
 
 
 def test_content_model_hrv_faulty_voltage3() -> None:
     with pytest.raises(ValueError):
-        _ = VirtualHarvester(name="iv110", voltage_mV=4000, voltage_min_mV=4001)
+        _ = VirtualHarvesterConfig(name="iv110", voltage_mV=4000, voltage_min_mV=4001)
 
 
 @pytest.mark.parametrize("name", ["ivcurves", "iv1000", "isc_voc"])
 def test_content_model_hrv_faulty_emu(name: str) -> None:
-    hrv = VirtualHarvester(name=name)
+    hrv = VirtualHarvesterConfig(name=name)
     with pytest.raises(ValueError):
-        _ = VirtualSource(name="dio_cap", harvester=hrv)
+        _ = VirtualSourceConfig(name="dio_cap", harvester=hrv)
 
 
 def test_content_model_src_min() -> None:
-    VirtualSource(
+    VirtualSourceConfig(
         id=9999,
         name="new_src",
         owner="jane",
         group="wayne",
     )
 
 
 def test_content_model_src_force_warning() -> None:
-    src = VirtualSource(
+    src = VirtualSourceConfig(
         name="BQ25570",
         C_output_uF=200,
         C_intermediate_uF=100,
     )
     ConverterPRUConfig.from_vsrc(src)
     # -> triggers warning currently
 
 
 def test_content_model_src_force_other_hysteresis1() -> None:
-    src = VirtualSource(
+    src = VirtualSourceConfig(
         name="BQ25570",
         V_intermediate_enable_threshold_mV=4000,
         V_intermediate_disable_threshold_mV=3999,
         V_output_mV=2000,
         V_buck_drop_mV=100,
     )
     ConverterPRUConfig.from_vsrc(src)
 
 
 def test_content_model_src_force_other_hysteresis2() -> None:
-    src = VirtualSource(
+    src = VirtualSourceConfig(
         name="BQ25570",
         V_intermediate_enable_threshold_mV=1000,
         V_intermediate_disable_threshold_mV=999,
         V_output_mV=2000,
         V_buck_drop_mV=100,
     )
     ConverterPRUConfig.from_vsrc(src)
```

### Comparing `shepherd_core-2023.5.6/tests/data_models/test_examples.py` & `shepherd_core-2023.6.1/tests/data_models/test_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from shepherd_core.data_models.content import VirtualSource
+from shepherd_core.data_models.content import VirtualSourceConfig
 from shepherd_core.data_models.experiment import Experiment
 from shepherd_core.data_models.task import EmulationTask
 from shepherd_core.data_models.task import HarvestTask
 from shepherd_core.data_models.testbed.testbed import Testbed as TasteBad
 
 from .conftest import load_yaml
 
@@ -41,8 +41,8 @@
     data_dict = load_yaml("example_config_testbed.yaml")
     print(data_dict)
     TasteBad(**data_dict)
 
 
 def test_example_vsrc() -> None:
     data_dict = load_yaml("example_config_virtsource.yaml")
-    VirtualSource(**data_dict["VirtualSource"])
+    VirtualSourceConfig(**data_dict["VirtualSource"])
```

### Comparing `shepherd_core-2023.5.6/tests/data_models/test_experiment_models.py` & `shepherd_core-2023.6.1/tests/data_models/test_experiment_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 from datetime import timedelta
 
 import pytest
 from pydantic import ValidationError
 
-from shepherd_core.data_models import VirtualHarvester
-from shepherd_core.data_models import VirtualSource
+from shepherd_core.data_models import VirtualHarvesterConfig
+from shepherd_core.data_models import VirtualSourceConfig
 from shepherd_core.data_models.content import EnergyEnvironment
 from shepherd_core.data_models.content import Firmware
 from shepherd_core.data_models.experiment import Experiment
 from shepherd_core.data_models.experiment import GpioActuation
 from shepherd_core.data_models.experiment import GpioEvent
 from shepherd_core.data_models.experiment import GpioLevel
 from shepherd_core.data_models.experiment import GpioTracing
@@ -58,101 +58,103 @@
         time_start="2023-12-12 12:12:12",
         target_configs=[target_cfgs],
     )
     assert exp1.get_hash() == exp2.get_hash()
 
 
 def test_experiment_model_exp_collision_target_id() -> None:
-    hrv = VirtualHarvester(name="mppt_bq_thermoelectric")
+    hrv = VirtualHarvesterConfig(name="mppt_bq_thermoelectric")
     target_cfgs = [
         TargetConfig(
             target_IDs=[3001, 3002, 3003, 2001],  # <- collision
             custom_IDs=[0, 1, 2, 3],
             energy_env={"name": "SolarSunny"},
             virtual_source={"name": "diode+capacitor"},
             firmware1={"name": "nrf52_demo_rf"},
         ),
         TargetConfig(
             target_IDs=list(range(2001, 2005)),  # <- collision
             custom_IDs=list(range(7, 18)),  # note: longer list is OK
             energy_env=EnergyEnvironment(name="ThermoelectricWashingMachine"),
-            virtual_source=VirtualSource(name="BQ25570-Schmitt", harvester=hrv),
+            virtual_source=VirtualSourceConfig(name="BQ25570-Schmitt", harvester=hrv),
             firmware1=Firmware(name="nrf52_demo_rf"),
             firmware2=Firmware(name="msp430_deep_sleep"),
         ),
     ]
     with pytest.raises(ValueError):
         _ = Experiment(
             id="4567",
             name="meaningful Test-Name",
             time_start=datetime.utcnow() + timedelta(minutes=30),
             target_configs=target_cfgs,
         )
 
 
 def test_experiment_model_exp_collision_custom_id() -> None:
-    hrv = VirtualHarvester(name="mppt_bq_thermoelectric")
+    hrv = VirtualHarvesterConfig(name="mppt_bq_thermoelectric")
     target_cfgs = [
         TargetConfig(
             target_IDs=[3001, 3002, 3003],
             custom_IDs=[0, 1, 7],  # <- collision
             energy_env={"name": "SolarSunny"},
             virtual_source={"name": "diode+capacitor"},
             firmware1={"name": "nrf52_demo_rf"},
         ),
         TargetConfig(
             target_IDs=list(range(2001, 2005)),
             custom_IDs=list(range(7, 18)),  # <- collision
             energy_env=EnergyEnvironment(name="ThermoelectricWashingMachine"),
-            virtual_source=VirtualSource(name="BQ25570-Schmitt", harvester=hrv),
+            virtual_source=VirtualSourceConfig(name="BQ25570-Schmitt", harvester=hrv),
             firmware1=Firmware(name="nrf52_demo_rf"),
             firmware2=Firmware(name="msp430_deep_sleep"),
         ),
     ]
     with pytest.raises(ValueError):
         _ = Experiment(
             id="4567",
             name="meaningful Test-Name",
             time_start=datetime.utcnow() + timedelta(minutes=30),
             target_configs=target_cfgs,
         )
 
 
 def test_experiment_model_exp_collision_observer() -> None:
-    hrv = VirtualHarvester(name="mppt_bq_thermoelectric")
+    hrv = VirtualHarvesterConfig(name="mppt_bq_thermoelectric")
     target_cfgs = [
         TargetConfig(
             target_IDs=[2005, 3001],  # <- both on same observer
             custom_IDs=list(range(7, 18)),
             energy_env=EnergyEnvironment(name="ThermoelectricWashingMachine"),
-            virtual_source=VirtualSource(name="BQ25570-Schmitt", harvester=hrv),
+            virtual_source=VirtualSourceConfig(name="BQ25570-Schmitt", harvester=hrv),
             firmware1=Firmware(name="nrf52_demo_rf"),
             firmware2=Firmware(name="msp430_deep_sleep"),
         ),
     ]
     with pytest.raises(ValueError):
         _ = Experiment(
             id="4567",
             name="meaningful Test-Name",
             time_start=datetime.utcnow() + timedelta(minutes=30),
             target_configs=target_cfgs,
         )
 
 
 def test_experiment_model_exp_missing_target() -> None:
-    hrv = VirtualHarvester(name="mppt_bq_thermoelectric")
+    hrv = VirtualHarvesterConfig(name="mppt_bq_thermoelectric")
     with pytest.raises(ValidationError):
         # should raise ValueError in Experiment
         # buts gets already caught in target_config
         _ = [
             TargetConfig(
                 target_IDs=[1234567],  # <- not existent
                 custom_IDs=list(range(7, 18)),
                 energy_env=EnergyEnvironment(name="ThermoelectricWashingMachine"),
-                virtual_source=VirtualSource(name="BQ25570-Schmitt", harvester=hrv),
+                virtual_source=VirtualSourceConfig(
+                    name="BQ25570-Schmitt", harvester=hrv
+                ),
                 firmware1=Firmware(name="nrf52_demo_rf"),
                 firmware2=Firmware(name="msp430_deep_sleep"),
             ),
         ]
         # experiment (like above) removed
```

### Comparing `shepherd_core-2023.5.6/tests/data_models/test_task_generation.py` & `shepherd_core-2023.6.1/tests/data_models/test_task_generation.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from datetime import timedelta
 from pathlib import Path
 
 from shepherd_core.data_models import EnergyEnvironment
 from shepherd_core.data_models import Experiment
 from shepherd_core.data_models import Firmware
 from shepherd_core.data_models import TargetConfig
-from shepherd_core.data_models import VirtualHarvester
-from shepherd_core.data_models import VirtualSource
+from shepherd_core.data_models import VirtualHarvesterConfig
+from shepherd_core.data_models import VirtualSourceConfig
 from shepherd_core.data_models.task import TestbedTasks as TasteBadTasks
 
 
 def test_task_generation_file(tmp_path: Path) -> None:
     path = Path(__file__).with_name("example_config_experiment.yaml")
     xp1 = Experiment.from_file(path)
     tb_tasks = TasteBadTasks.from_xp(xp1)
     tb_tasks.to_file(tmp_path / "tbt1.yaml")
 
 
 def test_task_generation_script(tmp_path: Path) -> None:
-    hrv = VirtualHarvester(name="mppt_bq_thermoelectric")
+    hrv = VirtualHarvesterConfig(name="mppt_bq_thermoelectric")
 
     target_cfgs = [
         # first init similar to yaml
         TargetConfig(
             target_IDs=list(range(3001, 3004)),
             custom_IDs=list(range(0, 3)),
             energy_env={"name": "SolarSunny"},
@@ -31,15 +31,15 @@
             firmware1={"name": "nrf52_demo_rf"},
         ),
         # second Instance fully object-oriented
         TargetConfig(
             target_IDs=list(range(2001, 2005)),
             custom_IDs=list(range(7, 18)),
             energy_env=EnergyEnvironment(name="ThermoelectricWashingMachine"),
-            virtual_source=VirtualSource(name="BQ25570-Schmitt", harvester=hrv),
+            virtual_source=VirtualSourceConfig(name="BQ25570-Schmitt", harvester=hrv),
             firmware1=Firmware(name="nrf52_demo_rf"),
             firmware2=Firmware(name="msp430_deep_sleep"),
         ),
     ]
 
     xperi = Experiment(
         id="4567",
```

### Comparing `shepherd_core-2023.5.6/tests/data_models/test_task_models.py` & `shepherd_core-2023.6.1/tests/data_models/test_task_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/tests/data_models/test_testbed_fixtures.py` & `shepherd_core-2023.6.1/tests/data_models/test_testbed_fixtures.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/tests/data_models/test_testbed_models.py` & `shepherd_core-2023.6.1/tests/data_models/test_testbed_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/tests/test_cal_hw.py` & `shepherd_core-2023.6.1/tests/test_cal_hw.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/tests/test_reader.py` & `shepherd_core-2023.6.1/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/tests/test_writer.py` & `shepherd_core-2023.6.1/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/tests/vsource/conftest.py` & `shepherd_core-2023.6.1/tests/vsource/conftest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.6/tests/vsource/test_converter.py` & `shepherd_core-2023.6.1/tests/vsource/test_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import pytest
 from pytest import approx
 
 from shepherd_core import BaseReader
 from shepherd_core import CalibrationEmulator
 from shepherd_core.data_models import EnergyDType
-from shepherd_core.data_models import VirtualSource
+from shepherd_core.data_models import VirtualSourceConfig
 from shepherd_core.vsource import VirtualSourceModel
 
 # virtual_converter_model gets tested below with vsrc_model
 
 src_list = [
     "direct",
     "diode+capacitor",
@@ -24,20 +24,20 @@
 
 
 def src_model(
     name: str,
     dtype_in: EnergyDType = EnergyDType.ivsample,
     window_size: Optional[int] = None,
 ) -> VirtualSourceModel:
-    src_config = VirtualSource(name=name)
+    src_config = VirtualSourceConfig(name=name)
     cal_emu = CalibrationEmulator()
     return VirtualSourceModel(
         src_config,
         cal_emu,
-        log_intermediate=True,
+        log_intermediate=False,
         dtype_in=dtype_in,
         window_size=window_size,
     )
 
 
 def c_leak_fWs(src: VirtualSourceModel, iterations: int) -> float:
     return iterations * src.cnv.V_mid_uV * src.cfg_src.I_intermediate_leak_nA
```

### Comparing `shepherd_core-2023.5.6/tests/vsource/test_harvester.py` & `shepherd_core-2023.6.1/tests/vsource/test_harvester.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 import pytest
 
 from shepherd_core import BaseReader
 from shepherd_core.data_models import EnergyDType
-from shepherd_core.data_models import VirtualHarvester
+from shepherd_core.data_models import VirtualHarvesterConfig
 from shepherd_core.data_models.content.virtual_harvester import HarvesterPRUConfig
 from shepherd_core.vsource import VirtualHarvesterModel
 
 hrv_list = [
     "ivcurve",
     "iv1000",
     "isc_voc",
@@ -19,39 +19,39 @@
     "mppt_po",
     "mppt_opt",
 ]
 
 
 @pytest.mark.parametrize("hrv_name", hrv_list)
 def test_vsource_hrv_min(hrv_name: str) -> None:
-    hrv_config = VirtualHarvester(name=hrv_name)
+    hrv_config = VirtualHarvesterConfig(name=hrv_name)
     hrv_pru = HarvesterPRUConfig.from_vhrv(hrv_config)
     _ = VirtualHarvesterModel(hrv_pru)
 
 
 def test_vsource_hrv_create_files(
     file_ivcurve: Path, file_ivsample: Path, file_isc_voc: Path
 ) -> None:
     pass
 
 
 @pytest.mark.parametrize("hrv_name", hrv_list[:3])
 def test_vsource_hrv_fail_ivcurve(hrv_name: str) -> None:
     # the first algos are not usable for ivcurve
     with pytest.raises(ValueError):
-        hrv_config = VirtualHarvester(name=hrv_name)
+        hrv_config = VirtualHarvesterConfig(name=hrv_name)
         _ = HarvesterPRUConfig.from_vhrv(
             hrv_config, for_emu=True, dtype_in=EnergyDType.ivcurve
         )
 
 
 @pytest.mark.parametrize("hrv_name", hrv_list[3:])
 def test_vsource_hrv_sim(hrv_name: str, file_ivcurve: Path) -> None:
     with BaseReader(file_ivcurve) as file:
-        hrv_config = VirtualHarvester(name=hrv_name)
+        hrv_config = VirtualHarvesterConfig(name=hrv_name)
         hrv_pru = HarvesterPRUConfig.from_vhrv(
             hrv_config,
             for_emu=True,
             dtype_in=file.get_datatype(),
             window_size=file.get_window_samples(),
         )
         hrv = VirtualHarvesterModel(hrv_pru)
@@ -63,17 +63,17 @@
                 )
 
 
 @pytest.mark.parametrize("hrv_name", hrv_list[3:])
 def test_vsource_hrv_fail_isc_voc(hrv_name: str) -> None:
     # not implemented ATM
     with pytest.raises(ValueError):
-        hrv_config = VirtualHarvester(name=hrv_name)
+        hrv_config = VirtualHarvesterConfig(name=hrv_name)
         _ = HarvesterPRUConfig.from_vhrv(
             hrv_config, for_emu=True, dtype_in=EnergyDType.isc_voc
         )
 
 
 def test_vsource_hrv_fail_unknown_type() -> None:
     with pytest.raises(KeyError):
-        hrv_config = VirtualHarvester(name="mppt_voc")
+        hrv_config = VirtualHarvesterConfig(name="mppt_voc")
         _ = HarvesterPRUConfig.from_vhrv(hrv_config, for_emu=True, dtype_in="xyz")
```

